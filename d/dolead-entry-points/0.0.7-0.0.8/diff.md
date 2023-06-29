# Comparing `tmp/dolead_entry_points-0.0.7.tar.gz` & `tmp/dolead_entry_points-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolead_entry_points-0.0.7.tar", max compression
+gzip compressed data, was "dolead_entry_points-0.0.8.tar", max compression
```

## Comparing `dolead_entry_points-0.0.7.tar` & `dolead_entry_points-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    18046 2018-05-23 12:43:02.497364 dolead_entry_points-0.0.7/LICENSE
--rw-r--r--   0        0        0      100 2019-04-04 16:09:37.026841 dolead_entry_points-0.0.7/dolead_entry_points/__init__.py
--rw-r--r--   0        0        0     1930 2019-04-04 16:09:28.198854 dolead_entry_points-0.0.7/dolead_entry_points/client.py
--rw-r--r--   0        0        0     6074 2020-10-28 14:24:40.460408 dolead_entry_points-0.0.7/dolead_entry_points/server.py
--rw-r--r--   0        0        0      492 2021-07-01 09:07:46.523901 dolead_entry_points-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      666 2021-07-01 09:08:11.332756 dolead_entry_points-0.0.7/setup.py
--rw-r--r--   0        0        0      531 2021-07-01 09:08:11.332960 dolead_entry_points-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    18046 2022-06-17 10:03:58.232981 dolead_entry_points-0.0.8/LICENSE
+-rw-r--r--   0        0        0       38 2022-06-17 10:03:58.232981 dolead_entry_points-0.0.8/README.md
+-rw-r--r--   0        0        0      100 2022-06-17 10:03:58.232981 dolead_entry_points-0.0.8/dolead_entry_points/__init__.py
+-rw-r--r--   0        0        0     1930 2022-06-17 10:03:58.232981 dolead_entry_points-0.0.8/dolead_entry_points/client.py
+-rw-r--r--   0        0        0     6606 2023-02-07 09:18:58.040183 dolead_entry_points-0.0.8/dolead_entry_points/server.py
+-rw-r--r--   0        0        0      423 2023-02-07 09:20:37.996417 dolead_entry_points-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 dolead_entry_points-0.0.8/setup.py
+-rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 dolead_entry_points-0.0.8/PKG-INFO
```

### Comparing `dolead_entry_points-0.0.7/LICENSE` & `dolead_entry_points-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dolead_entry_points-0.0.7/dolead_entry_points/client.py` & `dolead_entry_points-0.0.8/dolead_entry_points/client.py`

 * *Files identical despite different names*

### Comparing `dolead_entry_points-0.0.7/dolead_entry_points/server.py` & `dolead_entry_points-0.0.8/dolead_entry_points/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import collections
+import resource
 import inspect
 import json
 import logging
 from functools import wraps
 from gzip import GzipFile
 from io import BytesIO
 
@@ -36,14 +37,15 @@
 _DEFAULTS = {'flask_app': None,
              'flask_formatter': jsonify,
              'flask_code_exec_ctx_cls': CodeExecContext,
              'flask_swagger': None,
              'task_prefix': 'core',
              'celery_app': None,
              'celery_formatter': lambda x: x,
+             'prometeus_histogram': None,
              'celery_code_exec_ctx_cls': CodeExecContext}
 
 
 def kwargs_or_defaults(key, kwargs):
     if key in kwargs:
         return kwargs[key]
     return _DEFAULTS[key]
@@ -175,13 +177,21 @@
         swag_from = _DEFAULTS.get('flask_swagger', None)
         if swag_from is not None:
             func, specs = swag_specs_from_func(prefix, func, swagger_specs)
             func = swag_from(specs=specs)(func)
 
         map_in_flask(func, path, qualname, method, **kwargs)
 
+        histogram = kwargs_or_defaults('prometeus_histogram', kwargs)
+        project = kwargs_or_defaults('task_prefix', kwargs)
         @wraps(func)
         def wrapper(*args, **kwargs):
-            return func(*args, **kwargs)
-
+            start = None
+            if histogram:
+                start = resource.getrusage(resource.RUSAGE_BOTH).ru_utime
+            result = func(*args, **kwargs)
+            if histogram and start is not None:
+                histogram.labels(prefix, route, method).observe(
+                    resource.getrusage(resource.RUSAGE_BOTH).ru_utime - start)
+            return result
         return wrapper
     return metawrapper
```

### Comparing `dolead_entry_points-0.0.7/PKG-INFO` & `dolead_entry_points-0.0.8/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 Metadata-Version: 2.1
 Name: dolead-entry-points
-Version: 0.0.7
-Summary: Multi transport client/server solution
-License: GPLv2
+Version: 0.0.8
+Summary: Multiple entry points generator
+License: GPLv3
 Author: François Schmidts
 Author-email: francois@schmidts.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: celery (>=3.1.17)
 Requires-Dist: requests (>=2.13.0)
+Description-Content-Type: text/markdown
+
+# Dolead Simple multi entry point lib
+
```

