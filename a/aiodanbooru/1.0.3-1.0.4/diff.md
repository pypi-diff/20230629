# Comparing `tmp/aiodanbooru-1.0.3.tar.gz` & `tmp/aiodanbooru-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodanbooru-1.0.3.tar", last modified: Thu Jun 29 20:37:02 2023, max compression
+gzip compressed data, was "aiodanbooru-1.0.4.tar", last modified: Thu Jun 29 21:22:21 2023, max compression
```

## Comparing `aiodanbooru-1.0.3.tar` & `aiodanbooru-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.220804 aiodanbooru-1.0.3/
--rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     3022 2023-06-29 20:37:02.219763 aiodanbooru-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.212764 aiodanbooru-1.0.3/aiodanbooru/
--rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.3/aiodanbooru/__init__.py
--rw-rw-rw-   0        0        0     1668 2023-06-29 20:32:36.000000 aiodanbooru-1.0.3/aiodanbooru/api.py
--rw-rw-rw-   0        0        0     3140 2023-06-29 20:34:45.000000 aiodanbooru-1.0.3/aiodanbooru/models.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.217763 aiodanbooru-1.0.3/aiodanbooru.egg-info/
--rw-rw-rw-   0        0        0     3022 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-29 20:37:02.000000 aiodanbooru-1.0.3/aiodanbooru.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:37:02.220804 aiodanbooru-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-06-29 20:36:41.000000 aiodanbooru-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:37:02.218763 aiodanbooru-1.0.3/tests/
--rw-rw-rw-   0        0        0     1466 2023-06-29 20:35:36.000000 aiodanbooru-1.0.3/tests/test_api.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.260038 aiodanbooru-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-06-29 10:35:25.000000 aiodanbooru-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3022 2023-06-29 21:22:21.259005 aiodanbooru-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2003 2023-06-29 11:13:08.000000 aiodanbooru-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.248487 aiodanbooru-1.0.4/aiodanbooru/
+-rw-rw-rw-   0        0        0        0 2023-06-29 10:45:27.000000 aiodanbooru-1.0.4/aiodanbooru/__init__.py
+-rw-rw-rw-   0        0        0     1778 2023-06-29 20:53:59.000000 aiodanbooru-1.0.4/aiodanbooru/api.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.257003 aiodanbooru-1.0.4/aiodanbooru/dispatcher/
+-rw-rw-rw-   0        0        0        0 2023-06-29 21:07:02.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/__init__.py
+-rw-rw-rw-   0        0        0     3184 2023-06-29 21:13:02.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/filters.py
+-rw-rw-rw-   0        0        0     1017 2023-06-29 21:05:35.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher/handler.py
+-rw-rw-rw-   0        0        0     1971 2023-06-29 21:19:41.000000 aiodanbooru-1.0.4/aiodanbooru/dispatcher.py
+-rw-rw-rw-   0        0        0     3247 2023-06-29 21:18:06.000000 aiodanbooru-1.0.4/aiodanbooru/models.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.255003 aiodanbooru-1.0.4/aiodanbooru.egg-info/
+-rw-rw-rw-   0        0        0     3022 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-29 21:22:21.000000 aiodanbooru-1.0.4/aiodanbooru.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:22:21.260038 aiodanbooru-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-06-29 21:22:02.000000 aiodanbooru-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:22:21.258003 aiodanbooru-1.0.4/tests/
+-rw-rw-rw-   0        0        0     1466 2023-06-29 20:35:36.000000 aiodanbooru-1.0.4/tests/test_api.py
```

### Comparing `aiodanbooru-1.0.3/LICENSE` & `aiodanbooru-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.3/PKG-INFO` & `aiodanbooru-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.3/README.md` & `aiodanbooru-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aiodanbooru-1.0.3/aiodanbooru/api.py` & `aiodanbooru-1.0.4/aiodanbooru/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from typing import List
 
 import aiohttp
 
 from aiodanbooru.models import DanbooruPost
 
 
@@ -32,16 +33,18 @@
             endpoint = "/posts.json"
             params = {}
             if tags is not None:
                 params["tags"] = " ".join(tags)
             if limit is not None:
                 params["limit"] = str(limit)
             response = await self._get(session, endpoint, params)
-            posts = [DanbooruPost(**post) for post in response]
+            posts = [
+                DanbooruPost(**post, loop=asyncio.get_event_loop()) for post in response
+            ]
             return posts
 
     async def get_random_post(self) -> DanbooruPost:
         async with aiohttp.ClientSession() as session:
             endpoint = "/posts/random.json"
             response = await self._get(session, endpoint)
-            post = DanbooruPost(**response)
+            post = DanbooruPost(**response, loop=asyncio.get_event_loop())
             return post
```

### Comparing `aiodanbooru-1.0.3/aiodanbooru/models.py` & `aiodanbooru-1.0.4/aiodanbooru/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from typing import Optional
 
 import aiohttp
 from pydantic import BaseModel, Field, HttpUrl, validator
 
 
 class DanbooruPost(BaseModel):
@@ -61,14 +62,18 @@
         )
         async with aiohttp.ClientSession() as session:
             async with session.get(url) as response:
                 response.raise_for_status()
                 return await response.read()
 
     @property
+    def tags(self) -> list[str]:
+        return self.tag_string.split()
+
+    @property
     def link(self):
         return f"https://danbooru.donmai.us/posts/{self.id}"
 
     @property
     def media_url(self):
         return (
             self.large_file_url if self.large_file_url else self.file_url or self.source
```

### Comparing `aiodanbooru-1.0.3/aiodanbooru.egg-info/PKG-INFO` & `aiodanbooru-1.0.4/aiodanbooru.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodanbooru
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python library for interacting with the Danbooru API
 Author: lrdcxdes
 Author-email: lordgrief176@email.com
 License: MIT
 Project-URL: Source, https://github.com/lrdcxdes/aiodanbooru
 Project-URL: Bug Reports, https://github.com/lrdcxdes/aiodanbooru/issues
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `aiodanbooru-1.0.3/setup.py` & `aiodanbooru-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="aiodanbooru",
-    version="1.0.3",
+    version="1.0.4",
     description="A Python library for interacting with the Danbooru API",
     author="lrdcxdes",
     author_email="lordgrief176@email.com",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         "aiohttp",
         "pydantic",
```

### Comparing `aiodanbooru-1.0.3/tests/test_api.py` & `aiodanbooru-1.0.4/tests/test_api.py`

 * *Files identical despite different names*

