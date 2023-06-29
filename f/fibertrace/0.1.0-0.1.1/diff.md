# Comparing `tmp/fibertrace-0.1.0.tar.gz` & `tmp/fibertrace-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibertrace-0.1.0.tar", last modified: Thu Jun 29 08:28:41 2023, max compression
+gzip compressed data, was "fibertrace-0.1.1.tar", last modified: Thu Jun 29 08:37:01 2023, max compression
```

## Comparing `fibertrace-0.1.0.tar` & `fibertrace-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:41.529347 fibertrace-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:28:41.525347 fibertrace-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 08:28:15.000000 fibertrace-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 08:28:15.000000 fibertrace-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:28:41.529347 fibertrace-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 08:28:15.000000 fibertrace-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:41.525347 fibertrace-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:41.525347 fibertrace-0.1.0/src/fibertrace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:15.000000 fibertrace-0.1.0/src/fibertrace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-29 08:28:15.000000 fibertrace-0.1.0/src/fibertrace/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:28:41.525347 fibertrace-0.1.0/src/fibertrace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:28:41.000000 fibertrace-0.1.0/src/fibertrace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 08:28:41.000000 fibertrace-0.1.0/src/fibertrace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:28:41.000000 fibertrace-0.1.0/src/fibertrace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 08:28:41.000000 fibertrace-0.1.0/src/fibertrace.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:37:01.791706 fibertrace-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:37:01.791706 fibertrace-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-29 08:36:36.000000 fibertrace-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 08:36:36.000000 fibertrace-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:37:01.791706 fibertrace-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-29 08:36:36.000000 fibertrace-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:37:01.787706 fibertrace-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:37:01.791706 fibertrace-0.1.1/src/fibertrace/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 08:36:36.000000 fibertrace-0.1.1/src/fibertrace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-29 08:36:36.000000 fibertrace-0.1.1/src/fibertrace/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:37:01.791706 fibertrace-0.1.1/src/fibertrace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-29 08:37:01.000000 fibertrace-0.1.1/src/fibertrace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 08:37:01.000000 fibertrace-0.1.1/src/fibertrace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:37:01.000000 fibertrace-0.1.1/src/fibertrace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 08:37:01.000000 fibertrace-0.1.1/src/fibertrace.egg-info/top_level.txt
```

### Comparing `fibertrace-0.1.0/PKG-INFO` & `fibertrace-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibertrace
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for simple logging
 Home-page: https://github.com/bytesentinel-io/fibertrace.py
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fibertrace-0.1.0/README.md` & `fibertrace-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fibertrace-0.1.0/pyproject.toml` & `fibertrace-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "fibertrace"
-version = "0.1.0"
+version = "0.1.1"
 description = "A library for simple logging"
 long_description = """
 A library for simple logging
 """
 license = "MIT"
 author = "ByteSentinel.io"
 author-email = "dev@bytesentinel.io"
```

### Comparing `fibertrace-0.1.0/setup.py` & `fibertrace-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="fibertrace",
-    version="0.1.0",
+    version="0.1.1",
     author="ByteSentinel.io",
     author_email="dev@bytesentinel.io",
     description="A library for simple logging",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bytesentinel-io/fibertrace.py",
     packages=find_packages(where="src"),
```

### Comparing `fibertrace-0.1.0/src/fibertrace/log.py` & `fibertrace-0.1.1/src/fibertrace/log.py`

 * *Files identical despite different names*

### Comparing `fibertrace-0.1.0/src/fibertrace.egg-info/PKG-INFO` & `fibertrace-0.1.1/src/fibertrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibertrace
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library for simple logging
 Home-page: https://github.com/bytesentinel-io/fibertrace.py
 Author: ByteSentinel.io
 Author-email: dev@bytesentinel.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

