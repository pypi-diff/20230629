# Comparing `tmp/lazydocs2-0.1.1.tar.gz` & `tmp/lazydocs2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazydocs2-0.1.1.tar", max compression
+gzip compressed data, was "lazydocs2-0.1.2.tar", max compression
```

## Comparing `lazydocs2-0.1.1.tar` & `lazydocs2-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-06-29 20:18:11.409494 lazydocs2-0.1.1/LICENSE
--rw-r--r--   0        0        0    13489 2023-06-29 20:18:11.409494 lazydocs2-0.1.1/README.md
--rw-r--r--   0        0        0      417 2023-06-29 20:32:56.195027 lazydocs2-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      179 2023-06-29 20:18:11.413495 lazydocs2-0.1.1/src/lazydocs2/__init__.py
--rw-r--r--   0        0        0       29 2023-06-29 20:18:11.413495 lazydocs2-0.1.1/src/lazydocs2/__main__.py
--rw-r--r--   0        0        0      124 2023-06-29 20:33:01.445961 lazydocs2-0.1.1/src/lazydocs2/_about.py
--rw-r--r--   0        0        0     2218 2023-06-29 20:26:59.524440 lazydocs2-0.1.1/src/lazydocs2/_cli.py
--rwxr-xr-x   0        0        0    38005 2023-06-29 20:22:31.854704 lazydocs2-0.1.1/src/lazydocs2/generation.py
--rw-r--r--   0        0        0    14127 1970-01-01 00:00:00.000000 lazydocs2-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-06-29 20:18:11.409494 lazydocs2-0.1.2/LICENSE
+-rw-r--r--   0        0        0    13489 2023-06-29 20:18:11.409494 lazydocs2-0.1.2/README.md
+-rw-r--r--   0        0        0      417 2023-06-29 20:37:54.427893 lazydocs2-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      179 2023-06-29 20:18:11.413495 lazydocs2-0.1.2/src/lazydocs2/__init__.py
+-rw-r--r--   0        0        0       29 2023-06-29 20:18:11.413495 lazydocs2-0.1.2/src/lazydocs2/__main__.py
+-rw-r--r--   0        0        0      124 2023-06-29 20:37:45.852597 lazydocs2-0.1.2/src/lazydocs2/_about.py
+-rw-r--r--   0        0        0     2218 2023-06-29 20:26:59.524440 lazydocs2-0.1.2/src/lazydocs2/_cli.py
+-rwxr-xr-x   0        0        0    38005 2023-06-29 20:36:50.997516 lazydocs2-0.1.2/src/lazydocs2/generation.py
+-rw-r--r--   0        0        0    14127 1970-01-01 00:00:00.000000 lazydocs2-0.1.2/PKG-INFO
```

### Comparing `lazydocs2-0.1.1/LICENSE` & `lazydocs2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lazydocs2-0.1.1/README.md` & `lazydocs2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `lazydocs2-0.1.1/src/lazydocs2/_cli.py` & `lazydocs2-0.1.2/src/lazydocs2/_cli.py`

 * *Files identical despite different names*

### Comparing `lazydocs2-0.1.1/src/lazydocs2/generation.py` & `lazydocs2-0.1.2/src/lazydocs2/generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
         # Do not generate anything if docstring contains ignore instruction
         return True
     return False
 
 
 def _is_module_ignored(module_name: str, ignored_modules: List[str],include_under: bool = False) -> bool:
     """Checks if a given module is ignored."""
-    if module_name.split(".")[-1].startswith("_") and module_name[1] != "_" and not include_under:
+    if module_name.split('.')[-1].startswith("_") and module_name[1] != "_" and not include_under:
         return True
 
     for ignored_module in ignored_modules:
         if module_name == ignored_module:
             return True
 
         # Check is module is subpackage of an ignored package
```

### Comparing `lazydocs2-0.1.1/PKG-INFO` & `lazydocs2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazydocs2
-Version: 0.1.1
+Version: 0.1.2
 Summary: A fork of lazydocs for additional features
 License: MIT
 Author: khalidelborai
 Author-email: elboraikhalid@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lazydocs2 Version: 0.1.1 Summary: A fork of
+Metadata-Version: 2.1 Name: lazydocs2 Version: 0.1.2 Summary: A fork of
 lazydocs for additional features License: MIT Author: khalidelborai Author-
 email: elboraikhalid@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: typer (>=0.9.0,<0.10.0) Description-
```

