# Comparing `tmp/configzen-0.4.6.tar.gz` & `tmp/configzen-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.6.tar", max compression
+gzip compressed data, was "configzen-0.4.7.tar", max compression
```

## Comparing `configzen-0.4.6.tar` & `configzen-0.4.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.6/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.6/configzen/__main__.py
--rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.6/configzen/_isolation.py
--rw-r--r--   0        0        0     2916 2023-06-29 09:09:47.165217 configzen-0.4.6/configzen/_setup.py
--rw-r--r--   0        0        0    74687 2023-06-29 09:23:25.826027 configzen-0.4.6/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.6/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.6/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.6/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.6/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.6/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.6/configzen/route.py
--rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.6/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.6/LICENSE
--rw-r--r--   0        0        0     1473 2023-06-29 09:24:58.049052 configzen-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.6/README.md
--rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-29 09:13:33.339374 configzen-0.4.7/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.7/configzen/__main__.py
+-rw-r--r--   0        0        0     1437 2023-06-29 09:14:40.075983 configzen-0.4.7/configzen/_isolation.py
+-rw-r--r--   0        0        0     2925 2023-06-29 09:31:01.297959 configzen-0.4.7/configzen/_setup.py
+-rw-r--r--   0        0        0    74695 2023-06-29 09:31:41.082550 configzen-0.4.7/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.7/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.7/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.7/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.7/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.7/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.7/configzen/route.py
+-rw-r--r--   0        0        0     1168 2023-06-29 08:15:33.949387 configzen-0.4.7/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.7/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 09:32:17.326519 configzen-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    12655 2023-06-29 08:54:11.087815 configzen-0.4.7/README.md
+-rw-r--r--   0        0        0    13246 1970-01-01 00:00:00.000000 configzen-0.4.7/PKG-INFO
```

### Comparing `configzen-0.4.6/configzen/__init__.py` & `configzen-0.4.7/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/__main__.py` & `configzen-0.4.7/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/_isolation.py` & `configzen-0.4.7/configzen/_isolation.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/_setup.py` & `configzen-0.4.7/configzen/_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Convenience hooks for quicker development with _configzen_.
 
-You can replace this module with a custom one and then set it
-in the CONFIGZEN_SETUP_MODULE environment variable to use it.
+For advanced use cases, you can prevent this module from executing
+by setting the environment variable ``CONFIGZEN_SETUP`` to ``0``.
 """
 
 from __future__ import annotations
 
 import ast
 import collections.abc
 import pathlib
```

### Comparing `configzen-0.4.6/configzen/config.py` & `configzen-0.4.7/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -2356,8 +2356,9 @@
         reload_async = isolate_calls(reload_async)
         save = isolate_calls(save)
         save_async = isolate_calls(save_async)
         export = isolate_calls(export)
         export_async = isolate_calls(export_async)
 
 
-importlib.import_module(os.getenv("CONFIGZEN_SETUP_MODULE", "configzen._setup"))
+if os.getenv("CONFIGZEN_SETUP") != "0":
+    importlib.import_module("configzen._setup")
```

### Comparing `configzen-0.4.6/configzen/decorators.py` & `configzen-0.4.7/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/errors.py` & `configzen-0.4.7/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/field.py` & `configzen-0.4.7/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/processor.py` & `configzen-0.4.7/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/route.py` & `configzen-0.4.7/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/configzen/typedefs.py` & `configzen-0.4.7/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/LICENSE` & `configzen-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/pyproject.toml` & `configzen-0.4.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4.6"
+version = "0.4.7"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4.6/README.md` & `configzen-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.4.6/PKG-INFO` & `configzen-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4.6
+Version: 0.4.7
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

