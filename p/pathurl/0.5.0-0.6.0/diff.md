# Comparing `tmp/pathurl-0.5.0.tar.gz` & `tmp/pathurl-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathurl-0.5.0.tar", max compression
+gzip compressed data, was "pathurl-0.6.0.tar", max compression
```

## Comparing `pathurl-0.5.0.tar` & `pathurl-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     7652 2021-05-05 13:55:06.247270 pathurl-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1537 2022-01-19 14:48:13.357790 pathurl-0.5.0/README.rst
--rw-r--r--   0        0        0     1363 2022-01-19 14:47:32.074965 pathurl-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      126 2022-01-18 15:16:53.210015 pathurl-0.5.0/src/pathurl/__init__.py
--rw-r--r--   0        0        0      362 2022-01-18 15:16:53.210015 pathurl-0.5.0/src/pathurl/_constants.py
--rw-r--r--   0        0        0      918 2022-01-18 16:03:17.347128 pathurl-0.5.0/src/pathurl/path.py
--rw-r--r--   0        0        0        0 2021-08-05 15:56:38.773478 pathurl-0.5.0/src/pathurl/py.typed
--rw-r--r--   0        0        0     2764 2022-01-19 14:44:07.874149 pathurl-0.5.0/src/pathurl/query.py
--rw-r--r--   0        0        0     3692 2022-01-19 14:44:08.040814 pathurl-0.5.0/src/pathurl/url.py
--rw-r--r--   0        0        0     2196 2022-01-19 14:49:37.693508 pathurl-0.5.0/setup.py
--rw-r--r--   0        0        0     2316 2022-01-19 14:49:37.693689 pathurl-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-01-28 23:28:28.010464 pathurl-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     1730 2023-06-29 14:56:38.858233 pathurl-0.6.0/README.rst
+-rw-r--r--   0        0        0     2572 2023-06-29 14:56:38.839108 pathurl-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      126 2023-01-28 23:28:28.011188 pathurl-0.6.0/src/pathurl/__init__.py
+-rw-r--r--   0        0        0      458 2023-03-05 22:42:54.891380 pathurl-0.6.0/src/pathurl/_constants.py
+-rw-r--r--   0        0        0     1250 2023-06-29 13:56:06.801723 pathurl-0.6.0/src/pathurl/path.py
+-rw-r--r--   0        0        0        0 2023-01-28 23:28:28.011349 pathurl-0.6.0/src/pathurl/py.typed
+-rw-r--r--   0        0        0     3042 2023-06-29 14:23:43.799591 pathurl-0.6.0/src/pathurl/query.py
+-rw-r--r--   0        0        0     3878 2023-06-29 13:58:47.111208 pathurl-0.6.0/src/pathurl/url.py
+-rw-r--r--   0        0        0     2582 1970-01-01 00:00:00.000000 pathurl-0.6.0/PKG-INFO
```

### Comparing `pathurl-0.5.0/LICENSE.txt` & `pathurl-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pathurl-0.5.0/README.rst` & `pathurl-0.6.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 =============================
 pathurl: object-oriented URLs
 =============================
 
-.. image:: https://github.com/spapanik/pathurl/actions/workflows/build.yml/badge.svg
-  :alt: Build
-  :target: https://github.com/spapanik/pathurl/actions/workflows/build.yml
-.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/pathurl.svg
-  :alt: Total alerts
-  :target: https://lgtm.com/projects/g/spapanik/pathurl/alerts/
+.. image:: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/pathurl/actions/workflows/tests.yml
 .. image:: https://img.shields.io/github/license/spapanik/pathurl
   :alt: License
   :target: https://github.com/spapanik/pathurl/blob/main/LICENSE.txt
 .. image:: https://img.shields.io/pypi/v/pathurl
   :alt: PyPI
   :target: https://pypi.org/project/pathurl
 .. image:: https://pepy.tech/badge/pathurl
   :alt: Downloads
   :target: https://pepy.tech/project/pathurl
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: Code style
+  :alt: code style: black
   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
 
 ``pathurl`` is an objected-oriented way of manipulating URLs.
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `poetry`_ to manage your dependencies and add *pathurl* to them.
 
 .. code-block:: toml
 
     [tool.poetry.dependencies]
-    pathurl = "^0.5.0"
+    pathurl = "^0.6.0"
 
 Usage
 ^^^^^
 
 ``pathurl`` offers classes to manipulate URLs, paths and query strings. All objects are immutable.
 
 Links
```

### Comparing `pathurl-0.5.0/src/pathurl/path.py` & `pathurl-0.6.0/src/pathurl/path.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,40 +1,51 @@
-from typing import List
+from __future__ import annotations
 
 
 class Path:
-    __slots__ = ["_string"]
+    __slots__ = ("_string",)
 
     def __init__(self, string: str = ""):
         self._string = string
 
-    def __str__(self):
+    @classmethod
+    def from_segments(
+        cls, *segments: str, is_dir: bool = False, is_absolute: bool = True
+    ) -> Path:
+        string = "/".join(segments)
+        if is_dir:
+            string = f"{string}/"
+        if is_absolute:
+            string = f"/{string}"
+        return cls(string)
+
+    def __str__(self) -> str:
         return self._string
 
     def __hash__(self) -> int:
         return hash(self._string)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
         return self._string == other._string
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Path('{self}')"
 
     def __bool__(self) -> bool:
         return bool(self._string)
 
     @property
     def string(self) -> str:
         return self._string
 
     @property
     def is_absolute(self) -> bool:
         return self._string.startswith("/")
 
     @property
-    def segments(self) -> List[str]:
+    def segments(self) -> list[str]:
         split = self._string.rstrip("/").split("/")
         if self.is_absolute or not self:
             return split[1:]
         return split
```

### Comparing `pathurl-0.5.0/src/pathurl/query.py` & `pathurl-0.6.0/src/pathurl/query.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,89 +1,100 @@
+from __future__ import annotations
+
 from copy import deepcopy
-from typing import Dict, List, Tuple, Union
+from typing import Any, List, Union
 from urllib.parse import parse_qs, urlencode
 
 qs_value = Union[str, List[str]]
 
 
 class Query:
-    __slots__ = ["_string", "_data"]
+    __slots__ = ("_string", "_data")
 
     def __init__(self, _string: str = ""):
         self._data = self._str_to_dict(_string)
         self._string = self._dict_to_str(self._data)
 
+    @classmethod
+    def from_dict(
+        cls, dict_: dict[str, qs_value] | None = None, **kwargs: qs_value
+    ) -> Query:
+        dict_ = dict(dict_ or {}, **kwargs)
+        return cls(cls._dict_to_str(dict_))
+
     def __str__(self) -> str:
         return self._string
 
     def __hash__(self) -> int:
         return hash(self._string)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
         return self._string == other._string
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Query('{self}')"
 
     def __bool__(self) -> bool:
         return bool(self._string)
 
     @property
     def string(self) -> str:
         return self._string
 
     @property
-    def data(self) -> Dict[str, List[str]]:
+    def data(self) -> dict[str, list[str]]:
         return self._data
 
     @staticmethod
-    def _str_to_dict(string: str) -> Dict[str, List[str]]:
+    def _str_to_dict(string: str) -> dict[str, list[str]]:
         return parse_qs(string, keep_blank_values=True)
 
     @staticmethod
-    def _dict_to_str(data_: Dict[str, List[str]]) -> str:
+    def _dict_to_str(data_: dict[str, Any]) -> str:
         return urlencode(data_, doseq=True)
 
-    def get(self, key: str) -> List[str]:
+    def get(self, key: str) -> list[str] | None:
         return self._data.get(key)
 
-    def add(self, dict_: Dict[str, qs_value] = None, **kwargs: qs_value) -> "Query":
+    def add(
+        self, dict_: dict[str, qs_value] | None = None, **kwargs: qs_value
+    ) -> Query:
         data = deepcopy(self._data)
         dict_ = dict(dict_ or {}, **kwargs)
         for key, value in dict_.items():
             data.setdefault(key, [])
             if isinstance(value, list):
                 data[key].extend(value)
             else:
                 data[key].append(value)
         return self.__class__(self._dict_to_str(data))
 
     def set(  # noqa: A003
-        self, dict_: Dict[str, qs_value] = None, **kwargs: qs_value
-    ) -> "Query":
+        self, dict_: dict[str, qs_value] | None = None, **kwargs: qs_value
+    ) -> Query:
         data = deepcopy(self._data)
         dict_ = dict(dict_ or {}, **kwargs)
         for key, value in dict_.items():
             data.setdefault(key, [])
             if isinstance(value, list):
                 data[key] = value
             else:
                 data[key] = [value]
         return self.__class__(self._dict_to_str(data))
 
     def replace(
-        self, dict_: Dict[str, Tuple[str, str]] = None, **kwargs: Tuple[str, str]
-    ) -> "Query":
+        self, dict_: dict[str, tuple[str, str]] | None = None, **kwargs: tuple[str, str]
+    ) -> Query:
         data = deepcopy(self._data)
         dict_ = dict(dict_ or {}, **kwargs)
         for key, (old_value, new_value) in dict_.items():
             for i, value in enumerate(data.get(key, [])):
                 if value == old_value:
                     data[key][i] = new_value
         return self.__class__(self._dict_to_str(data))
 
-    def remove(self, key: str) -> "Query":
+    def remove(self, key: str) -> Query:
         data = deepcopy(self._data)
         del data[key]
         return self.__class__(self._dict_to_str(data))
```

### Comparing `pathurl-0.5.0/src/pathurl/url.py` & `pathurl-0.6.0/src/pathurl/url.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,71 @@
-from typing import Union
+from __future__ import annotations
+
+from typing import Any
 from urllib.parse import urljoin, urlsplit, urlunsplit
 
 from pathurl._constants import Port
 from pathurl.path import Path
 from pathurl.query import Query
 
 
 class URL:
-    __slots__ = [
+    __slots__ = (
         "_string",
         "_netloc",
         "_scheme",
         "_username",
         "_password",
         "_hostname",
         "_port",
         "_path",
         "_query",
         "_fragment",
-    ]
+    )
 
     def __init__(self, string: str = ""):
         parsed_url = urlsplit(string)
         self._string = string
         self._netloc = parsed_url.netloc
         self._scheme = parsed_url.scheme
         self._username = parsed_url.username
         self._hostname = parsed_url.hostname
         self._password = parsed_url.password
         self._port = parsed_url.port or self._infer_port(self._scheme)
         self._path = Path(parsed_url.path)
         self._query = Query(parsed_url.query)
         self._fragment = parsed_url.fragment
 
-    def __str__(self):
+    @classmethod
+    def from_parts(
+        cls,
+        scheme: str,
+        username: str | None = None,
+        password: str | None = None,
+        hostname: str = "",
+        port: int | None = None,
+        path: str | Path = "",
+        query: str | Query = "",
+        fragment: str = "",
+    ) -> URL:
+        netloc = cls._create_netloc(scheme, username, password, hostname, port)
+        return cls(urlunsplit((scheme, netloc, str(path), str(query), fragment)))
+
+    def __str__(self) -> str:
         return self._string
 
     def __hash__(self) -> int:
         return hash(self._string)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, self.__class__):
             return NotImplemented
         return self._string == other._string
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"URL('{self}')"
 
     def __bool__(self) -> bool:
         return bool(self._string)
 
     @property
     def string(self) -> str:
@@ -59,27 +76,27 @@
         return self._netloc
 
     @property
     def scheme(self) -> str:
         return self._scheme
 
     @property
-    def username(self) -> str:
+    def username(self) -> str | None:
         return self._username
 
     @property
-    def hostname(self) -> str:
+    def hostname(self) -> str | None:
         return self._hostname
 
     @property
-    def password(self) -> str:
+    def password(self) -> str | None:
         return self._password
 
     @property
-    def port(self) -> int:
+    def port(self) -> int | None:
         return self._port
 
     @property
     def path(self) -> Path:
         return self._path
 
     @property
@@ -87,63 +104,53 @@
         return self._query
 
     @property
     def fragment(self) -> str:
         return self._fragment
 
     @staticmethod
-    def _infer_port(scheme: str) -> int:
+    def _infer_port(scheme: str) -> int | None:
         try:
             port = Port[scheme]
         except KeyError:
             return None
 
         return port.value
 
     @classmethod
     def _create_netloc(
-        cls, scheme: str, username: str, password: str, hostname: str, port: int
+        cls,
+        scheme: str,
+        username: str | None,
+        password: str | None,
+        hostname: str,
+        port: int | None,
     ) -> str:
         parts = []
         if username or password:
             if username:
                 parts.append(username)
             if password:
                 parts.append(f":{password}")
             parts.append("@")
         parts.append(hostname)
         if port and port != cls._infer_port(scheme):
             parts.append(f":{port}")
         return "".join(parts)
 
-    @classmethod
-    def _from_parts(
-        cls,
-        scheme: str,
-        username: str,
-        password: str,
-        hostname: str,
-        port: int,
-        path: Union[str, Path],
-        query: Union[str, Query],
-        fragment: str,
-    ) -> "URL":
-        netloc = cls._create_netloc(scheme, username, password, hostname, port)
-        return cls(urlunsplit((scheme, netloc, str(path), str(query), fragment)))
-
-    def replace(self, **kwargs) -> "URL":
+    def replace(self, **kwargs: Any) -> URL:
         parts = {
             "scheme",
             "username",
             "password",
             "hostname",
             "port",
             "path",
             "query",
             "fragment",
         }
         for part in parts:
             kwargs.setdefault(part, getattr(self, part))
-        return self._from_parts(**kwargs)
+        return self.from_parts(**kwargs)
 
-    def join(self, path: Union[str, Path]) -> "URL":
+    def join(self, path: str | Path) -> URL:
         return self.__class__(urljoin(str(self), str(path)))
```

### Comparing `pathurl-0.5.0/PKG-INFO` & `pathurl-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 Metadata-Version: 2.1
 Name: pathurl
-Version: 0.5.0
+Version: 0.6.0
 Summary: url manipulation
-Home-page: https://github.com/spapanik/pathurl
+Home-page: https://pathurl.readthedocs.io/en/stable/
 License: LGPL-3.0+
 Keywords: url
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Documentation, https://pathurl.readthedocs.io/en/stable/
 Project-URL: Repository, https://github.com/spapanik/pathurl
 Description-Content-Type: text/x-rst
 
 =============================
 pathurl: object-oriented URLs
 =============================
 
-.. image:: https://github.com/spapanik/pathurl/actions/workflows/build.yml/badge.svg
-  :alt: Build
-  :target: https://github.com/spapanik/pathurl/actions/workflows/build.yml
-.. image:: https://img.shields.io/lgtm/alerts/g/spapanik/pathurl.svg
-  :alt: Total alerts
-  :target: https://lgtm.com/projects/g/spapanik/pathurl/alerts/
+.. image:: https://github.com/spapanik/pathurl/actions/workflows/tests.yml/badge.svg
+  :alt: Tests
+  :target: https://github.com/spapanik/pathurl/actions/workflows/tests.yml
 .. image:: https://img.shields.io/github/license/spapanik/pathurl
   :alt: License
   :target: https://github.com/spapanik/pathurl/blob/main/LICENSE.txt
 .. image:: https://img.shields.io/pypi/v/pathurl
   :alt: PyPI
   :target: https://pypi.org/project/pathurl
 .. image:: https://pepy.tech/badge/pathurl
   :alt: Downloads
   :target: https://pepy.tech/project/pathurl
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-  :alt: Code style
+  :alt: code style: black
   :target: https://github.com/psf/black
+.. image:: https://img.shields.io/badge/build%20automation-yamk-success
+  :alt: build automation: yam
+  :target: https://github.com/spapanik/yamk
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json
+  :alt: Lint: ruff
+  :target: https://github.com/charliermarsh/ruff
 
 ``pathurl`` is an objected-oriented way of manipulating URLs.
 
 In a nutshell
 -------------
 
 Installation
 ^^^^^^^^^^^^
 
 The easiest way is to use `poetry`_ to manage your dependencies and add *pathurl* to them.
 
 .. code-block:: toml
 
     [tool.poetry.dependencies]
-    pathurl = "^0.5.0"
+    pathurl = "^0.6.0"
 
 Usage
 ^^^^^
 
 ``pathurl`` offers classes to manipulate URLs, paths and query strings. All objects are immutable.
 
 Links
```

