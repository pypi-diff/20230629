# Comparing `tmp/atomcache-0.7.2.tar.gz` & `tmp/atomcache-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomcache-0.7.2.tar", max compression
+gzip compressed data, was "atomcache-0.7.3.tar", max compression
```

## Comparing `atomcache-0.7.2.tar` & `atomcache-0.7.3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.2/LICENSE
--rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.2/README.md
--rw-r--r--   0        0        0      160 2023-05-02 08:09:07.408140 atomcache-0.7.2/atomcache/__init__.py
--rw-r--r--   0        0        0     1421 2023-05-02 08:34:44.766221 atomcache-0.7.2/atomcache/backend.py
--rw-r--r--   0        0        0     9930 2023-05-02 08:34:44.775221 atomcache-0.7.2/atomcache/base.py
--rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.2/atomcache/py.typed
--rw-r--r--   0        0        0     4962 2023-05-02 08:34:44.768221 atomcache-0.7.2/atomcache/redis.py
--rw-r--r--   0        0        0      951 2023-05-02 08:36:16.764119 atomcache-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5034 1970-01-01 00:00:00.000000 atomcache-0.7.2/setup.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2021-10-31 14:30:27.194665 atomcache-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4164 2022-12-02 13:52:44.271882 atomcache-0.7.3/README.md
+-rw-r--r--   0        0        0      160 2023-06-29 14:56:27.625934 atomcache-0.7.3/atomcache/__init__.py
+-rw-r--r--   0        0        0     1421 2023-06-29 14:55:22.713233 atomcache-0.7.3/atomcache/backend.py
+-rw-r--r--   0        0        0    10452 2023-06-29 14:55:22.723234 atomcache-0.7.3/atomcache/base.py
+-rw-r--r--   0        0        0        0 2022-03-11 07:33:27.689230 atomcache-0.7.3/atomcache/py.typed
+-rw-r--r--   0        0        0     4962 2023-06-29 14:55:22.716234 atomcache-0.7.3/atomcache/redis.py
+-rw-r--r--   0        0        0      951 2023-06-29 14:56:34.604009 atomcache-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 atomcache-0.7.3/PKG-INFO
```

### Comparing `atomcache-0.7.2/LICENSE` & `atomcache-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.2/README.md` & `atomcache-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.2/atomcache/backend.py` & `atomcache-0.7.3/atomcache/backend.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.2/atomcache/base.py` & `atomcache-0.7.3/atomcache/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,19 +66,24 @@
         self.auto_refresh = auto_refresh
         self._expire = exp
         self.namespace = namespace
         self._lock_timeout = lock_timeout
         self._allow_cache_control = cache_control
         self._autorefresh_callback: Union[Callable, Awaitable, None] = None
         self._autorefresh_task: Optional[asyncio.Future] = None
+        self._refreshing: bool = False
         self._no_cache: bool = False
 
     async def __call__(self, request: Request):
         if self._allow_cache_control:
             self._no_cache = "no-cache" in CommaSeparatedStrings(request.headers.get("Cache-Control", ""))
+        if self._refreshing:
+            cached_content, ttl = await self.backend.get(self.get_key(), with_lock=False)
+            if cached_content is not None:
+                raise CachedResponse(content=cached_content, ttl=ttl)
         return self
 
     def set_namespace(self, namespace: str):  # noqa: WPS615 FIXME: unpythonic setter
         self.namespace = namespace
 
     def set_autorefresh_callback(self, endpoint: Union[Callable, Coroutine]):  # noqa: WPS231 WPS615
         kwargs = {}
@@ -89,15 +94,22 @@
             elif isinstance(prm.default, params.Depends) and isinstance(prm.default.dependency, Cache):
                 default = self
             else:
                 default = prm.default
             kwargs[prm.name] = default
             if default == inspect._empty or isinstance(default, params.Depends):  # noqa: WPS437
                 raise ValueError(f"{endpoint} does not support auto cache refresh. Args {prm.name} has no default")
-        self._autorefresh_callback = partial(endpoint, **kwargs)
+
+        autorefresh_callback = partial(endpoint, **kwargs)
+        if asyncio.iscoroutinefunction(endpoint):
+            self._autorefresh_callback = autorefresh_callback
+        else:
+            loop = asyncio.get_running_loop()
+            self._autorefresh_callback = partial(loop.run_in_executor, None, autorefresh_callback)
+
         Cache.autorefresh[self.namespace] = self
 
     def get_key(self, cache_id: str = "") -> str:
         return f"{self.namespace}{cache_id}"
 
     def set(self, response: _ResponseT, cache_id: str = "") -> _ResponseT:  # noqa: WPS125
         if isinstance(response, Response):
@@ -142,15 +154,15 @@
             cache_id (str, optional): Cache identifier. Defaults to "".
             with_lock (bool, optional): Lock the cache if there is no response. Defaults to True.
             lockspace (str, optional): Key to use for lock
 
         Raises:
             CachedResponse: generate response from cache.
         """
-        if self._no_cache:
+        if self._refreshing or self._no_cache:
             return
         cached_content, ttl = await self.backend.get(
             self.get_key(cache_id),
             timeout=self._lock_timeout,
             with_lock=with_lock,
             lockspace=lockspace,
         )
@@ -183,15 +195,15 @@
             if not isinstance(route, APIRoute):
                 continue
             signature = inspect.signature(route.endpoint)
             for prm in signature.parameters.values():
                 default = prm.default
                 if not default or not isinstance(default, params.Depends) or not isinstance(default.dependency, cls):
                     continue
-                cache: cls = default.dependency
+                cache = default.dependency
                 if cache.namespace is None:
                     cache.set_namespace(route.path)
                 if cache.auto_refresh:
                     cache.set_autorefresh_callback(route.endpoint)
 
     async def _autorefresh(self):
         key = self.get_key()
@@ -199,20 +211,20 @@
         ttl = await self.backend.ttl(key)
 
         time_until_refresh = ttl - self._lock_timeout  # In case key is not setted ttl is -2
 
         if time_until_refresh > 0:
             await asyncio.sleep(time_until_refresh)
         if await self.backend.lock(key, timeout=self._lock_timeout):
-            if asyncio.iscoroutinefunction(self._autorefresh_callback):
+            self._autorefresh_task = asyncio.ensure_future(self._autorefresh())
+            self._refreshing = True
+            try:  # noqa: WPS501
                 await self._autorefresh_callback()
-            else:
-                self._autorefresh_callback()
-            await self.backend.unlock(key)
-        self._autorefresh_task = asyncio.ensure_future(self._autorefresh())
+            finally:
+                self._refreshing = False
 
 
 def cached_response_handler(request: Request, exc: CachedResponse) -> Response:
     if_none_match = request.headers.get("if-none-match")
     etag = f"W/{hashsum(exc.content)}"
     if if_none_match == etag:
         response = Response(status_code=304, headers={"Cache-Control": f"max-age={exc.ttl}"})  # noqa:WPS432
```

### Comparing `atomcache-0.7.2/atomcache/redis.py` & `atomcache-0.7.3/atomcache/redis.py`

 * *Files identical despite different names*

### Comparing `atomcache-0.7.2/pyproject.toml` & `atomcache-0.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atomcache"
-version = "0.7.2"
+version = "0.7.3"
 description = "Asynchronous cache manager designed for horizontally scaled web applications."
 authors = ["Serghei Ungurean <srg@intelbit.io>", "Nichita Morcotilo <nmorkotilo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/pysergio/atomcache"
 repository = "https://github.com/pysergio/atomcache"
```

### Comparing `atomcache-0.7.2/setup.py` & `atomcache-0.7.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,172 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: atomcache
+Version: 0.7.3
+Summary: Asynchronous cache manager designed for horizontally scaled web applications.
+Home-page: https://github.com/pysergio/atomcache
+License: MIT
+Author: Serghei Ungurean
+Author-email: srg@intelbit.io
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.61.2)
+Requires-Dist: redis (>=4.5.4,<5.0.0)
+Project-URL: Repository, https://github.com/pysergio/atomcache
+Description-Content-Type: text/markdown
+
+<p align="center">
+<a href="https://codecov.io/gh/pysergio/atomcache"> 
+ <img src="https://codecov.io/gh/pysergio/atomcache/branch/master/graph/badge.svg?token=OVZABBE1UJ"/> 
+</a>
+<a href="https://pypi.org/project/atomcache" target="_blank">
+    <img src="https://img.shields.io/pypi/v/atomcache?color=%2334D058&label=pypi%20package" alt="Package version">
+</a>
+<a href="https://pypi.org/project/atomcache" target="_blank">
+    <img src="https://img.shields.io/pypi/pyversions/atomcache.svg?color=%2334D058" alt="Supported Python versions">
+</a>
+</p>
+
+## Introduction
+Asynchronous cache manager designed for horizontally scaled web applications.
+**NOTE:** _Currently has implementation only for FastAPI using Redis._
+
+## Requirements
+
+Python 3.7+
+
+* <a href="https://redis.readthedocs.io/en/latest/_modules/redis/asyncio/client.html?" class="external-link" target="_blank">redis</a> for cache implementation.
+* <a href="https://fastapi.tiangolo.com" class="external-link" target="_blank">FastAPI</a> for the web parts.
+  
+## Installation
+
+<div class="termy">
+
+```console
+$ pip install atomcache
+
+---> 100%
+```
+
+## Explanation schema
+
+![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/pysergio/atomcache/master/README.md)
+
+<details markdown="1">
+<summary>As UML</summary>
+
+```plantuml
+@startuml
+    !theme materia
+    participant Redis
+    participant Instance_A as A
+    participant Instance_B as B
+    participant Instance_N as C
+
+
+    B <-> Redis: GET: Cache=null & GET: Lock=null
+
+    B <-> Redis: SET: Lock = true
+
+    activate B #Red
+    A <--> Redis: GET: Cache=null & GET: Lock=true
+    activate A #Transparent
+    C <--> Redis: GET: Cache=null & GET: Lock=true
+    activate C #Transparent
+    B <--> B: Do the computation
+    B -> Redis: SET: Cache={...}
+    deactivate B
+
+    group Notify Cache SET
+        Redis -> C
+        Redis -> A
+    end
+    group GET Cache
+        Redis <-> C
+    deactivate C
+        Redis <-> A
+    deactivate A
+    end
+@enduml
+```
+</details>
+
+## Examples:
+
+### Usage as FastAPI Dependency
+
+* Create a file `events.py` with:
+
+```Python
+from typing import Optional, Callable
+
+from redis.asyncio import Redis
+from fastapi import FastAPI, Depends
+from atomcache import Cache
+
+
+def create_start_app_handler(app: FastAPI) -> Callable:
+    async def start_app() -> None:
+        redis: Redis = await Redis.from_url(url="redis://localhost", encoding="utf-8")
+        await Cache.init(app, redis)
+
+    return start_app
+
+
+def create_stop_app_handler(app: FastAPI) -> Callable:
+    async def stop_app() -> None:
+        await Cache.backend.close()
+
+    return stop_app
+```
+
+* Create a file `main.py` with:
+
+```Python
+from typing import Optional
+
+from fastapi import FastAPI, Depends
+from atomcache import Cache
+
+from .events import create_start_app_handler, create_stop_app_handler
+
+app = FastAPI()
+
+app.add_event_handler("startup", create_start_app_handler(app))
+app.add_event_handler("shutdown", create_stop_app_handler(app))
+
+
+@router.get("/resources", response_model=List[TheResponseModel], name="main:test-example")
+async def resources(offset: int = 0, items: int = 10, cache: Cache = Depends(Cache(exp=600)):
+    cache_id = f"{offset}-{items}"  # Build cache identifier
+    await cache.raise_try(cache_id)  # Try to respond from cache
+    response = await db.find(TheResponseModel, skip=offset, limit=items)
+    await asyncio.sleep(10)  # Do some heavy work for 10 sec, see `lock_timeout`
+    return cache.set(response, cache_id=cache_id)
+```
+
+### Direct cache usage for avoiding repetitive calling on external resources:
+
+```Python
+from aiohttp import ClientSession
+from atomcache import Cache
+
+cache = Cache(exp=1200, namespace="my-namespace:")
+
+
+async def requesting_helper(ref: str) -> List[dict]:
+    cached_value = await cache.get(cache_id=ref)
+    if cached_value is not None:
+        return cached_value
+
+    async with ClientSession() as session:
+        async with session.get(f"https://external-api.io/{ref}") as response:
+            if response.ok:
+                cached_value = response.json()
+                return cache.set(cached_value, cache_id=ref)
+    return []
+```
 
-packages = \
-['atomcache']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fastapi>=0.61.2', 'redis>=4.5.4,<5.0.0']
-
-setup_kwargs = {
-    'name': 'atomcache',
-    'version': '0.7.2',
-    'description': 'Asynchronous cache manager designed for horizontally scaled web applications.',
-    'long_description': '<p align="center">\n<a href="https://codecov.io/gh/pysergio/atomcache"> \n <img src="https://codecov.io/gh/pysergio/atomcache/branch/master/graph/badge.svg?token=OVZABBE1UJ"/> \n</a>\n<a href="https://pypi.org/project/atomcache" target="_blank">\n    <img src="https://img.shields.io/pypi/v/atomcache?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/atomcache" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/atomcache.svg?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Introduction\nAsynchronous cache manager designed for horizontally scaled web applications.\n**NOTE:** _Currently has implementation only for FastAPI using Redis._\n\n## Requirements\n\nPython 3.7+\n\n* <a href="https://redis.readthedocs.io/en/latest/_modules/redis/asyncio/client.html?" class="external-link" target="_blank">redis</a> for cache implementation.\n* <a href="https://fastapi.tiangolo.com" class="external-link" target="_blank">FastAPI</a> for the web parts.\n  \n## Installation\n\n<div class="termy">\n\n```console\n$ pip install atomcache\n\n---> 100%\n```\n\n## Explanation schema\n\n![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://raw.githubusercontent.com/pysergio/atomcache/master/README.md)\n\n<details markdown="1">\n<summary>As UML</summary>\n\n```plantuml\n@startuml\n    !theme materia\n    participant Redis\n    participant Instance_A as A\n    participant Instance_B as B\n    participant Instance_N as C\n\n\n    B <-> Redis: GET: Cache=null & GET: Lock=null\n\n    B <-> Redis: SET: Lock = true\n\n    activate B #Red\n    A <--> Redis: GET: Cache=null & GET: Lock=true\n    activate A #Transparent\n    C <--> Redis: GET: Cache=null & GET: Lock=true\n    activate C #Transparent\n    B <--> B: Do the computation\n    B -> Redis: SET: Cache={...}\n    deactivate B\n\n    group Notify Cache SET\n        Redis -> C\n        Redis -> A\n    end\n    group GET Cache\n        Redis <-> C\n    deactivate C\n        Redis <-> A\n    deactivate A\n    end\n@enduml\n```\n</details>\n\n## Examples:\n\n### Usage as FastAPI Dependency\n\n* Create a file `events.py` with:\n\n```Python\nfrom typing import Optional, Callable\n\nfrom redis.asyncio import Redis\nfrom fastapi import FastAPI, Depends\nfrom atomcache import Cache\n\n\ndef create_start_app_handler(app: FastAPI) -> Callable:\n    async def start_app() -> None:\n        redis: Redis = await Redis.from_url(url="redis://localhost", encoding="utf-8")\n        await Cache.init(app, redis)\n\n    return start_app\n\n\ndef create_stop_app_handler(app: FastAPI) -> Callable:\n    async def stop_app() -> None:\n        await Cache.backend.close()\n\n    return stop_app\n```\n\n* Create a file `main.py` with:\n\n```Python\nfrom typing import Optional\n\nfrom fastapi import FastAPI, Depends\nfrom atomcache import Cache\n\nfrom .events import create_start_app_handler, create_stop_app_handler\n\napp = FastAPI()\n\napp.add_event_handler("startup", create_start_app_handler(app))\napp.add_event_handler("shutdown", create_stop_app_handler(app))\n\n\n@router.get("/resources", response_model=List[TheResponseModel], name="main:test-example")\nasync def resources(offset: int = 0, items: int = 10, cache: Cache = Depends(Cache(exp=600)):\n    cache_id = f"{offset}-{items}"  # Build cache identifier\n    await cache.raise_try(cache_id)  # Try to respond from cache\n    response = await db.find(TheResponseModel, skip=offset, limit=items)\n    await asyncio.sleep(10)  # Do some heavy work for 10 sec, see `lock_timeout`\n    return cache.set(response, cache_id=cache_id)\n```\n\n### Direct cache usage for avoiding repetitive calling on external resources:\n\n```Python\nfrom aiohttp import ClientSession\nfrom atomcache import Cache\n\ncache = Cache(exp=1200, namespace="my-namespace:")\n\n\nasync def requesting_helper(ref: str) -> List[dict]:\n    cached_value = await cache.get(cache_id=ref)\n    if cached_value is not None:\n        return cached_value\n\n    async with ClientSession() as session:\n        async with session.get(f"https://external-api.io/{ref}") as response:\n            if response.ok:\n                cached_value = response.json()\n                return cache.set(cached_value, cache_id=ref)\n    return []\n```\n',
-    'author': 'Serghei Ungurean',
-    'author_email': 'srg@intelbit.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/pysergio/atomcache',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,56 +1,53 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['atomcache']
-package_data = \ {'': ['*']} install_requires = \ ['fastapi>=0.61.2',
-'redis>=4.5.4,<5.0.0'] setup_kwargs = { 'name': 'atomcache', 'version':
-'0.7.2', 'description': 'Asynchronous cache manager designed for horizontally
-scaled web applications.', 'long_description': '
-      \n\n_[https://codecov.io/gh/pysergio/atomcache/branch/master/graph/
- badge.svg?token=OVZABBE1UJ]_\n\n\n_[Package_version]\n\n\n_[Supported_Python
-                                 versions]\n\n
-\n\n## Introduction\nAsynchronous cache manager designed for horizontally
-scaled web applications.\n**NOTE:** _Currently has implementation only for
-FastAPI using Redis._\n\n## Requirements\n\nPython 3.7+\n\n* redis for cache
-implementation.\n* FastAPI for the web parts.\n \n## Installation\n\n
-\n\n```console\n$ pip install atomcache\n\n---> 100%\n```\n\n## Explanation
-schema\n\n![Class Diagram](http://www.plantuml.com/plantuml/proxy?src=https://
-raw.githubusercontent.com/pysergio/atomcache/master/README.md)\n\n\nAs
-UML\n\n```plantuml\n@startuml\n !theme materia\n participant Redis\n
-participant Instance_A as A\n participant Instance_B as B\n participant
-Instance_N as C\n\n\n B <-> Redis: GET: Cache=null & GET: Lock=null\n\n B <-
-> Redis: SET: Lock = true\n\n activate B #Red\n A <--> Redis: GET: Cache=null &
-GET: Lock=true\n activate A #Transparent\n C <--> Redis: GET: Cache=null & GET:
-Lock=true\n activate C #Transparent\n B <--> B: Do the computation\n B -
-> Redis: SET: Cache={...}\n deactivate B\n\n group Notify Cache SET\n Redis -
-> C\n Redis -> A\n end\n group GET Cache\n Redis <-> C\n deactivate C\n Redis
-<-> A\n deactivate A\n end\n@enduml\n```\n\n\n## Examples:\n\n### Usage as
-FastAPI Dependency\n\n* Create a file `events.py` with:\n\n```Python\nfrom
-typing import Optional, Callable\n\nfrom redis.asyncio import Redis\nfrom
-fastapi import FastAPI, Depends\nfrom atomcache import Cache\n\n\ndef
-create_start_app_handler(app: FastAPI) -> Callable:\n async def start_app() -
-> None:\n redis: Redis = await Redis.from_url(url="redis://localhost",
-encoding="utf-8")\n await Cache.init(app, redis)\n\n return start_app\n\n\ndef
-create_stop_app_handler(app: FastAPI) -> Callable:\n async def stop_app() -
-> None:\n await Cache.backend.close()\n\n return stop_app\n```\n\n* Create a
-file `main.py` with:\n\n```Python\nfrom typing import Optional\n\nfrom fastapi
-import FastAPI, Depends\nfrom atomcache import Cache\n\nfrom .events import
-create_start_app_handler, create_stop_app_handler\n\napp = FastAPI
-()\n\napp.add_event_handler("startup", create_start_app_handler
-(app))\napp.add_event_handler("shutdown", create_stop_app_handler
-(app))\n\n\n@router.get("/resources", response_model=List[TheResponseModel],
-name="main:test-example")\nasync def resources(offset: int = 0, items: int =
-10, cache: Cache = Depends(Cache(exp=600)):\n cache_id = f"{offset}-{items}" #
-Build cache identifier\n await cache.raise_try(cache_id) # Try to respond from
-cache\n response = await db.find(TheResponseModel, skip=offset, limit=items)\n
-await asyncio.sleep(10) # Do some heavy work for 10 sec, see `lock_timeout`\n
-return cache.set(response, cache_id=cache_id)\n```\n\n### Direct cache usage
-for avoiding repetitive calling on external resources:\n\n```Python\nfrom
-aiohttp import ClientSession\nfrom atomcache import Cache\n\ncache = Cache
-(exp=1200, namespace="my-namespace:")\n\n\nasync def requesting_helper(ref:
-str) -> List[dict]:\n cached_value = await cache.get(cache_id=ref)\n if
-cached_value is not None:\n return cached_value\n\n async with ClientSession()
-as session:\n async with session.get(f"https://external-api.io/{ref}") as
-response:\n if response.ok:\n cached_value = response.json()\n return cache.set
-(cached_value, cache_id=ref)\n return []\n```\n', 'author': 'Serghei Ungurean',
-'author_email': 'srg@intelbit.io', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/pysergio/atomcache', 'packages': packages,
-'package_data': package_data, 'install_requires': install_requires,
-'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: atomcache Version: 0.7.3 Summary: Asynchronous
+cache manager designed for horizontally scaled web applications. Home-page:
+https://github.com/pysergio/atomcache License: MIT Author: Serghei Ungurean
+Author-email: srg@intelbit.io Requires-Python: >=3.8,<4.0 Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: fastapi
+(>=0.61.2) Requires-Dist: redis (>=4.5.4,<5.0.0) Project-URL: Repository,
+https://github.com/pysergio/atomcache Description-Content-Type: text/markdown
+        [https://codecov.io/gh/pysergio/atomcache/branch/master/graph/
+   badge.svg?token=OVZABBE1UJ] [Package_version] [Supported_Python_versions]
+## Introduction Asynchronous cache manager designed for horizontally scaled web
+applications. **NOTE:** _Currently has implementation only for FastAPI using
+Redis._ ## Requirements Python 3.7+ * redis for cache implementation. * FastAPI
+for the web parts. ## Installation
+```console $ pip install atomcache ---> 100% ``` ## Explanation schema ![Class
+Diagram](http://www.plantuml.com/plantuml/proxy?src=https://
+raw.githubusercontent.com/pysergio/atomcache/master/README.md)  As UML
+```plantuml @startuml !theme materia participant Redis participant Instance_A
+as A participant Instance_B as B participant Instance_N as C B <-> Redis: GET:
+Cache=null & GET: Lock=null B <-> Redis: SET: Lock = true activate B #Red A <--
+> Redis: GET: Cache=null & GET: Lock=true activate A #Transparent C <--> Redis:
+GET: Cache=null & GET: Lock=true activate C #Transparent B <--> B: Do the
+computation B -> Redis: SET: Cache={...} deactivate B group Notify Cache SET
+Redis -> C Redis -> A end group GET Cache Redis <-> C deactivate C Redis <-> A
+deactivate A end @enduml ```  ## Examples: ### Usage as FastAPI Dependency *
+Create a file `events.py` with: ```Python from typing import Optional, Callable
+from redis.asyncio import Redis from fastapi import FastAPI, Depends from
+atomcache import Cache def create_start_app_handler(app: FastAPI) -> Callable:
+async def start_app() -> None: redis: Redis = await Redis.from_url(url="redis:/
+/localhost", encoding="utf-8") await Cache.init(app, redis) return start_app
+def create_stop_app_handler(app: FastAPI) -> Callable: async def stop_app() -
+> None: await Cache.backend.close() return stop_app ``` * Create a file
+`main.py` with: ```Python from typing import Optional from fastapi import
+FastAPI, Depends from atomcache import Cache from .events import
+create_start_app_handler, create_stop_app_handler app = FastAPI()
+app.add_event_handler("startup", create_start_app_handler(app))
+app.add_event_handler("shutdown", create_stop_app_handler(app)) @router.get("/
+resources", response_model=List[TheResponseModel], name="main:test-example")
+async def resources(offset: int = 0, items: int = 10, cache: Cache = Depends
+(Cache(exp=600)): cache_id = f"{offset}-{items}" # Build cache identifier await
+cache.raise_try(cache_id) # Try to respond from cache response = await db.find
+(TheResponseModel, skip=offset, limit=items) await asyncio.sleep(10) # Do some
+heavy work for 10 sec, see `lock_timeout` return cache.set(response,
+cache_id=cache_id) ``` ### Direct cache usage for avoiding repetitive calling
+on external resources: ```Python from aiohttp import ClientSession from
+atomcache import Cache cache = Cache(exp=1200, namespace="my-namespace:") async
+def requesting_helper(ref: str) -> List[dict]: cached_value = await cache.get
+(cache_id=ref) if cached_value is not None: return cached_value async with
+ClientSession() as session: async with session.get(f"https://external-api.io/
+{ref}") as response: if response.ok: cached_value = response.json() return
+cache.set(cached_value, cache_id=ref) return [] ```
```

