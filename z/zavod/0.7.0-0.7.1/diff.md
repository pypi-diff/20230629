# Comparing `tmp/zavod-0.7.0.tar.gz` & `tmp/zavod-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zavod-0.7.0.tar", last modified: Wed Jun 28 10:44:24 2023, max compression
+gzip compressed data, was "zavod-0.7.1.tar", last modified: Thu Jun 29 07:46:26 2023, max compression
```

## Comparing `zavod-0.7.0.tar` & `zavod-0.7.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:44:23.995987 zavod-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-28 10:42:35.000000 zavod-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 10:42:35.000000 zavod-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-28 10:44:23.995987 zavod-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-28 10:42:35.000000 zavod-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 10:44:23.995987 zavod-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-28 10:42:35.000000 zavod-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:44:23.995987 zavod-0.7.0/zavod/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/audit.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:44:23.995987 zavod-0.7.0/zavod/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/parse/addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/parse/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/parse/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:44:23.995987 zavod-0.7.0/zavod/sinks/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/sinks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/sinks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/sinks/json_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/sinks/json_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/sinks/pack_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-28 10:42:35.000000 zavod-0.7.0/zavod/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:44:23.995987 zavod-0.7.0/zavod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:44:08.000000 zavod-0.7.0/zavod.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-28 10:44:23.000000 zavod-0.7.0/zavod.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-29 07:44:20.000000 zavod-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 07:44:20.000000 zavod-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:46:26.196416 zavod-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 07:44:20.000000 zavod-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:46:26.196416 zavod-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-29 07:44:20.000000 zavod-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.192416 zavod-0.7.1/zavod/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/parse/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod/sinks/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/json_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/json_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/sinks/pack_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 07:44:20.000000 zavod-0.7.1/zavod/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:46:26.196416 zavod-0.7.1/zavod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:46:07.000000 zavod-0.7.1/zavod.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 07:46:26.000000 zavod-0.7.1/zavod.egg-info/top_level.txt
```

### Comparing `zavod-0.7.0/LICENSE` & `zavod-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/PKG-INFO` & `zavod-0.7.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.0
+Version: 0.7.1
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.7.0/setup.py` & `zavod-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="zavod",
-    version="0.7.0",
+    version="0.7.1",
     description="Data factory for followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney etl parsing",
     author="Friedrich Lindenberg",
     author_email="friedrich@opensanctions.org",
     url="https://github.com/opensanctions/zavod",
@@ -18,15 +18,15 @@
     packages=find_packages(exclude=["ez_setup", "examples", "tests"]),
     namespace_packages=[],
     include_package_data=True,
     package_data={"": ["zavod/data/*", "zavod/py.typed"]},
     zip_safe=False,
     install_requires=[
         "followthemoney >= 3.2.0, < 4.0.0",
-        "nomenklatura >= 3.0.1, < 4.0.0",
+        "nomenklatura >= 3.0.2, < 4.0.0",
         "addressformatting >= 1.3.0, < 2.0.0",
         "datapatch >= 0.2.1",
         "click >= 8.0.0, < 8.2.0",
         "requests",
         "structlog",
         "lxml",
     ],
```

### Comparing `zavod-0.7.0/zavod/__init__.py` & `zavod-0.7.1/zavod/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from zavod import settings
 from zavod.context import GenericZavod
 from zavod.dataset import ZavodDataset, ZD
 from zavod.logs import configure_logging, get_logger
 from zavod.sinks.common import Sink
 from zavod.sinks.json_entity import JSONEntitySink
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __all__ = [
     "init",
     "context",
     "Zavod",
     "ZavodDataset",
     "ZD",
     "PathLike",
```

### Comparing `zavod-0.7.0/zavod/audit.py` & `zavod-0.7.1/zavod/audit.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/context.py` & `zavod-0.7.1/zavod/context.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/dataset.py` & `zavod-0.7.1/zavod/dataset.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/http.py` & `zavod-0.7.1/zavod/http.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/logs.py` & `zavod-0.7.1/zavod/logs.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/parse/addresses.py` & `zavod-0.7.1/zavod/parse/addresses.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/parse/names.py` & `zavod-0.7.1/zavod/parse/names.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/parse/xml.py` & `zavod-0.7.1/zavod/parse/xml.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/sinks/common.py` & `zavod-0.7.1/zavod/sinks/common.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod/sinks/pack_statement.py` & `zavod-0.7.1/zavod/sinks/pack_statement.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,29 @@
-import sys
-import csv
 import _csv
 from io import TextIOWrapper
 from typing import Optional
 from nomenklatura.entity import CE
-from nomenklatura.statement.serialize import pack_statement, PACK_COLUMNS
+from nomenklatura.statement.serialize import pack_row, pack_writer
 from followthemoney.util import PathLike
 
 from zavod.sinks.common import FileSink
 
 
 class PackStatementSink(FileSink[CE]):
     def __init__(self, path: PathLike) -> None:
         super().__init__(path)
-        self.wrapper: Optional[TextIOWrapper] = None
-        self.writer: Optional[_csv._writer] = None
+        self.fh = open(self.path, "wb")
+        self.wrapper = TextIOWrapper(self.fh, encoding="utf-8")
+        self.writer = pack_writer(self.wrapper)
 
     def emit(self, entity: CE) -> None:
         with self.lock:
-            if self.fh is None:
-                self.fh = open(self.path, "wb")
-            if self.wrapper is None and self.fh is not None:
-                self.wrapper = TextIOWrapper(self.fh, encoding="utf-8")
-            if self.writer is None and self.wrapper is not None:
-                self.writer = csv.writer(
-                    self.wrapper,
-                    dialect=csv.unix_dialect,
-                    quoting=csv.QUOTE_MINIMAL,
-                )
-            if self.writer is not None:
-                for stmt in entity.statements:
-                    row = pack_statement(stmt)
-                    self.writer.writerow([row.get(c) for c in PACK_COLUMNS])
+            for stmt in entity.statements:
+                self.writer.writerow(pack_row(stmt))
 
     def close(self) -> None:
         with self.lock:
-            if self.wrapper is not None:
-                self.wrapper.close()
-                self.wrapper = None
+            self.wrapper.close()
             super().close()
 
     def __repr__(self) -> str:
         return f"<PackStatementSink({self.path!r})>"
```

### Comparing `zavod-0.7.0/zavod/util.py` & `zavod-0.7.1/zavod/util.py`

 * *Files identical despite different names*

### Comparing `zavod-0.7.0/zavod.egg-info/PKG-INFO` & `zavod-0.7.1/zavod.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: zavod
-Version: 0.7.0
+Version: 0.7.1
 Summary: Data factory for followthemoney data.
 Home-page: https://github.com/opensanctions/zavod
 Author: Friedrich Lindenberg
 Author-email: friedrich@opensanctions.org
 License: MIT
 Keywords: data mapping identity followthemoney etl parsing
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # zavod
 
 Zavod is the FollowTheMoney data factory. It contains a variety of useful functions for building small and reproducible data pipelines that generate FtM graphs.
-
```

### Comparing `zavod-0.7.0/zavod.egg-info/SOURCES.txt` & `zavod-0.7.1/zavod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

