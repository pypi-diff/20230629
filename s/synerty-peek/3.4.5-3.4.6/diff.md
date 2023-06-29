# Comparing `tmp/synerty-peek-3.4.5.tar.gz` & `tmp/synerty-peek-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synerty-peek-3.4.5.tar", last modified: Wed Jun 28 07:27:33 2023, max compression
+gzip compressed data, was "synerty-peek-3.4.6.tar", last modified: Thu Jun 29 10:21:21 2023, max compression
```

## Comparing `synerty-peek-3.4.5.tar` & `synerty-peek-3.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:33.371096 synerty-peek-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-28 07:27:33.371096 synerty-peek-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2984 2023-06-28 07:25:25.000000 synerty-peek-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:33.371096 synerty-peek-3.4.5/peek/
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-28 07:25:25.000000 synerty-peek-3.4.5/peek/__init__.py
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-28 07:27:33.371096 synerty-peek-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2051 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:33.371096 synerty-peek-3.4.5/synerty_peek.egg-info/
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      260 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      802 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-28 07:27:33.000000 synerty-peek-3.4.5/synerty_peek.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:21.263518 synerty-peek-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-29 10:21:21.263518 synerty-peek-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-29 10:19:16.000000 synerty-peek-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:21.263518 synerty-peek-3.4.6/peek/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-29 10:19:16.000000 synerty-peek-3.4.6/peek/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 10:21:21.264519 synerty-peek-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2051 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:21.263518 synerty-peek-3.4.6/synerty_peek.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      260 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-29 10:21:21.000000 synerty-peek-3.4.6/synerty_peek.egg-info/top_level.txt
```

### Comparing `synerty-peek-3.4.5/README.rst` & `synerty-peek-3.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `synerty-peek-3.4.5/setup.py` & `synerty-peek-3.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from setuptools import find_packages, setup
 
 pip_package_name = "synerty-peek"
-package_version = "3.4.5"
+package_version = "3.4.6"
 
 egg_info = "%s.egg-info" % pip_package_name
 if os.path.isdir(egg_info):
     shutil.rmtree(egg_info)
 
 if os.path.isfile("MANIFEST"):
     os.remove("MANIFEST")
```

### Comparing `synerty-peek-3.4.5/synerty_peek.egg-info/requires.txt` & `synerty-peek-3.4.6/synerty_peek.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-peek-admin-doc==3.4.*,>=3.4.5
-peek-admin-app==3.4.*,>=3.4.5
-peek-agent-service==3.4.*,>=3.4.5
-peek-core-device==3.4.*,>=3.4.5
-peek-core-docdb==3.4.*,>=3.4.5
-peek-core-email==3.4.*,>=3.4.5
-peek-core-search==3.4.*,>=3.4.5
-peek-core-user==3.4.*,>=3.4.5
-peek-core-screen==3.4.*,>=3.4.5
-peek-field-doc==3.4.*,>=3.4.5
-peek-field-app==3.4.*,>=3.4.5
-peek-field-service==3.4.*,>=3.4.5
-peek-logic-service==3.4.*,>=3.4.5
-peek-office-doc==3.4.*,>=3.4.5
-peek-office-app==3.4.*,>=3.4.5
-peek-office-service==3.4.*,>=3.4.5
-peek-platform==3.4.*,>=3.4.5
-peek-plugin-base==3.4.*,>=3.4.5
-peek-storage-service==3.4.*,>=3.4.5
-peek-worker-service==3.4.*,>=3.4.5
-peek-abstract-chunked-index==3.4.*,>=3.4.5
-peek-abstract-chunked-data-loader==3.4.*,>=3.4.5
+peek-admin-doc==3.4.*,>=3.4.6
+peek-admin-app==3.4.*,>=3.4.6
+peek-agent-service==3.4.*,>=3.4.6
+peek-core-device==3.4.*,>=3.4.6
+peek-core-docdb==3.4.*,>=3.4.6
+peek-core-email==3.4.*,>=3.4.6
+peek-core-search==3.4.*,>=3.4.6
+peek-core-user==3.4.*,>=3.4.6
+peek-core-screen==3.4.*,>=3.4.6
+peek-field-doc==3.4.*,>=3.4.6
+peek-field-app==3.4.*,>=3.4.6
+peek-field-service==3.4.*,>=3.4.6
+peek-logic-service==3.4.*,>=3.4.6
+peek-office-doc==3.4.*,>=3.4.6
+peek-office-app==3.4.*,>=3.4.6
+peek-office-service==3.4.*,>=3.4.6
+peek-platform==3.4.*,>=3.4.6
+peek-plugin-base==3.4.*,>=3.4.6
+peek-storage-service==3.4.*,>=3.4.6
+peek-worker-service==3.4.*,>=3.4.6
+peek-abstract-chunked-index==3.4.*,>=3.4.6
+peek-abstract-chunked-data-loader==3.4.*,>=3.4.6
 sphinx
 sphinx-rtd-theme
 sphinx-autobuild
 pytmpdir<1.1.0,>=1.0.2
 py-spy
```

