# Comparing `tmp/configzen-0.4.tar.gz` & `tmp/configzen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.4.tar", max compression
+gzip compressed data, was "configzen-0.4.1.tar", max compression
```

## Comparing `configzen-0.4.tar` & `configzen-0.4.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.4/configzen/__init__.py
--rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4/configzen/__main__.py
--rw-r--r--   0        0        0     1286 2023-06-29 07:05:41.644836 configzen-0.4/configzen/_isolation.py
--rw-r--r--   0        0        0    79152 2023-06-29 07:05:45.058201 configzen-0.4/configzen/config.py
--rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4/configzen/decorators.py
--rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4/configzen/errors.py
--rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4/configzen/field.py
--rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4/configzen/py.typed
--rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4/configzen/route.py
--rw-r--r--   0        0        0     1126 2023-06-29 07:06:09.671161 configzen-0.4/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4/LICENSE
--rw-r--r--   0        0        0     1471 2023-06-29 07:10:09.485977 configzen-0.4/pyproject.toml
--rw-r--r--   0        0        0    12653 2023-06-29 05:44:52.044957 configzen-0.4/README.md
--rw-r--r--   0        0        0    13242 1970-01-01 00:00:00.000000 configzen-0.4/PKG-INFO
+-rw-r--r--   0        0        0      979 2023-06-15 09:10:26.257090 configzen-0.4.1/configzen/__init__.py
+-rw-r--r--   0        0        0      935 2023-06-12 23:31:06.893355 configzen-0.4.1/configzen/__main__.py
+-rw-r--r--   0        0        0     1286 2023-06-29 07:05:41.644836 configzen-0.4.1/configzen/_isolation.py
+-rw-r--r--   0        0        0    79093 2023-06-29 07:15:43.040767 configzen-0.4.1/configzen/config.py
+-rw-r--r--   0        0        0     4828 2023-06-29 06:34:50.665979 configzen-0.4.1/configzen/decorators.py
+-rw-r--r--   0        0        0     3756 2023-06-29 05:23:10.057981 configzen-0.4.1/configzen/errors.py
+-rw-r--r--   0        0        0      531 2023-06-27 21:14:31.456634 configzen-0.4.1/configzen/field.py
+-rw-r--r--   0        0        0    26250 2023-06-29 07:04:59.758193 configzen-0.4.1/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.4.1/configzen/py.typed
+-rw-r--r--   0        0        0     4694 2023-06-29 07:04:59.733190 configzen-0.4.1/configzen/route.py
+-rw-r--r--   0        0        0     1126 2023-06-29 07:06:09.671161 configzen-0.4.1/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-06-12 23:31:22.580649 configzen-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1473 2023-06-29 07:16:22.443336 configzen-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12653 2023-06-29 05:44:52.044957 configzen-0.4.1/README.md
+-rw-r--r--   0        0        0    13244 1970-01-01 00:00:00.000000 configzen-0.4.1/PKG-INFO
```

### Comparing `configzen-0.4/configzen/__init__.py` & `configzen-0.4.1/configzen/__init__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/__main__.py` & `configzen-0.4.1/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/_isolation.py` & `configzen-0.4.1/configzen/_isolation.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/config.py` & `configzen-0.4.1/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,25 +396,23 @@
     value
         The value to load.
 
     Returns
     -------
     The loaded value.
     """
-    if isinstance(value, cls):
-        return value
     if isinstance(value, str):
         try:
             data = ast.literal_eval(value)
         except (SyntaxError, ValueError):
             # There might be some following validator, let it be like that
             return value
         else:
             return cls(data)
-    return cls(value)
+    return value
 
 
 def _delegate_ac_options(
     load_options: dict[str, Any], dump_options: dict[str, Any], options: dict[str, Any]
 ) -> None:
     for key, value in options.items():
         if key.startswith("dump_"):
```

### Comparing `configzen-0.4/configzen/decorators.py` & `configzen-0.4.1/configzen/decorators.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/errors.py` & `configzen-0.4.1/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/field.py` & `configzen-0.4.1/configzen/field.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/processor.py` & `configzen-0.4.1/configzen/processor.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/route.py` & `configzen-0.4.1/configzen/route.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/configzen/typedefs.py` & `configzen-0.4.1/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.4/LICENSE` & `configzen-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.4/pyproject.toml` & `configzen-0.4.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.4"
+version = "0.4.1"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bswck/configzen"
 
 [tool.poetry.dependencies]
```

### Comparing `configzen-0.4/README.md` & `configzen-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.4/PKG-INFO` & `configzen-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.4
+Version: 0.4.1
 Summary: The easiest way to manage configuration files in Python
 Home-page: https://github.com/bswck/configzen
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

