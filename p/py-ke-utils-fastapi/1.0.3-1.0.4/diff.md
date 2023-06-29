# Comparing `tmp/py-ke-utils-fastapi-1.0.3.tar.gz` & `tmp/py-ke-utils-fastapi-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ke-utils-fastapi-1.0.3.tar", last modified: Wed Jun 28 13:53:53 2023, max compression
+gzip compressed data, was "py-ke-utils-fastapi-1.0.4.tar", last modified: Wed Jun 28 14:00:12 2023, max compression
```

## Comparing `py-ke-utils-fastapi-1.0.3.tar` & `py-ke-utils-fastapi-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 13:53:53.375651 py-ke-utils-fastapi-1.0.3/
--rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-28 13:53:53.375651 py-ke-utils-fastapi-1.0.3/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)     6383 2023-06-28 13:12:43.000000 py-ke-utils-fastapi-1.0.3/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 13:53:53.375651 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-28 13:53:53.000000 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      292 2023-06-28 13:53:53.000000 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-28 13:53:53.000000 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       42 2023-06-28 13:53:53.000000 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-06-28 13:53:53.000000 py-ke-utils-fastapi-1.0.3/py_ke_utils_fastapi.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 13:53:53.375651 py-ke-utils-fastapi-1.0.3/pykeutilsfastapi/
--rw-r--r--   0 erne      (1000) erne      (1000)       46 2023-06-28 13:32:32.000000 py-ke-utils-fastapi-1.0.3/pykeutilsfastapi/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     5072 2023-06-28 13:50:49.000000 py-ke-utils-fastapi-1.0.3/pykeutilsfastapi/_auth_deco.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-28 13:53:53.375651 py-ke-utils-fastapi-1.0.3/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      772 2023-06-28 13:51:45.000000 py-ke-utils-fastapi-1.0.3/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 14:00:12.395651 py-ke-utils-fastapi-1.0.4/
+-rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-28 14:00:12.395651 py-ke-utils-fastapi-1.0.4/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)     6383 2023-06-28 13:12:43.000000 py-ke-utils-fastapi-1.0.4/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 14:00:12.395651 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      499 2023-06-28 14:00:12.000000 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      292 2023-06-28 14:00:12.000000 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-28 14:00:12.000000 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       42 2023-06-28 14:00:12.000000 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       17 2023-06-28 14:00:12.000000 py-ke-utils-fastapi-1.0.4/py_ke_utils_fastapi.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 14:00:12.395651 py-ke-utils-fastapi-1.0.4/pykeutilsfastapi/
+-rw-r--r--   0 erne      (1000) erne      (1000)       47 2023-06-28 14:00:05.000000 py-ke-utils-fastapi-1.0.4/pykeutilsfastapi/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     5072 2023-06-28 13:50:49.000000 py-ke-utils-fastapi-1.0.4/pykeutilsfastapi/_auth_deco.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-28 14:00:12.395651 py-ke-utils-fastapi-1.0.4/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      772 2023-06-28 14:00:05.000000 py-ke-utils-fastapi-1.0.4/setup.py
```

### Comparing `py-ke-utils-fastapi-1.0.3/README.md` & `py-ke-utils-fastapi-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-1.0.3/pykeutilsfastapi/_auth_deco.py` & `py-ke-utils-fastapi-1.0.4/pykeutilsfastapi/_auth_deco.py`

 * *Files identical despite different names*

### Comparing `py-ke-utils-fastapi-1.0.3/setup.py` & `py-ke-utils-fastapi-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "Utilities with Redis and FastAPI"
 
 # Setting up
 setup(
     name="py-ke-utils-fastapi",
     version=VERSION,
     author="KE",
```

