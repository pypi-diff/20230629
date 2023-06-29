# Comparing `tmp/szh_toolbox-0.0.5.tar.gz` & `tmp/szh_toolbox-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szh_toolbox-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "szh_toolbox-0.0.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `szh_toolbox-0.0.5.tar` & `szh_toolbox-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       12 2023-06-29 04:49:53.240161 szh_toolbox-0.0.5/README.md
--rw-r--r--   0        0        0      664 2023-06-29 06:36:36.292429 szh_toolbox-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1862 2023-06-29 06:35:42.398384 szh_toolbox-0.0.5/src/szh_toolbox/__init__.py
--rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.5/src/szh_toolbox/commond.py
--rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.5/src/szh_toolbox/namelist.py
--rw-r--r--   0        0        0     2786 2023-06-29 06:33:25.154818 szh_toolbox-0.0.5/src/szh_toolbox/namelistwps.py
--rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.5/src/szh_toolbox/test.py
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 szh_toolbox-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-29 04:49:53.240161 szh_toolbox-0.0.6/README.md
+-rw-r--r--   0        0        0      664 2023-06-29 06:39:45.708070 szh_toolbox-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1862 2023-06-29 06:35:42.398384 szh_toolbox-0.0.6/src/szh_toolbox/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-29 02:31:19.795188 szh_toolbox-0.0.6/src/szh_toolbox/commond.py
+-rw-r--r--   0        0        0     4563 2023-05-15 06:26:45.362456 szh_toolbox-0.0.6/src/szh_toolbox/namelist.py
+-rw-r--r--   0        0        0     2793 2023-06-29 06:39:39.421182 szh_toolbox-0.0.6/src/szh_toolbox/namelistwps.py
+-rw-r--r--   0        0        0       67 2023-06-28 07:18:07.747348 szh_toolbox-0.0.6/src/szh_toolbox/test.py
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 szh_toolbox-0.0.6/PKG-INFO
```

### Comparing `szh_toolbox-0.0.5/pyproject.toml` & `szh_toolbox-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.9"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "szh_toolbox"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `szh_toolbox-0.0.5/src/szh_toolbox/__init__.py` & `szh_toolbox-0.0.6/src/szh_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.5/src/szh_toolbox/namelist.py` & `szh_toolbox-0.0.6/src/szh_toolbox/namelist.py`

 * *Files identical despite different names*

### Comparing `szh_toolbox-0.0.5/src/szh_toolbox/namelistwps.py` & `szh_toolbox-0.0.6/src/szh_toolbox/namelistwps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyproj import Transformer
-import namelist as nl
+from . import namelist as nl
 from math import ceil, floor
 import argparse
 import os
 
 
 def mercator_in_wps(rlat, rlon, tlat, delta, e_we, e_sn):
     '''
```

