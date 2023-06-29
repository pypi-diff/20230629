# Comparing `tmp/vectortile-1.4.0.tar.gz` & `tmp/vectortile-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectortile-1.4.0.tar", last modified: Thu Jun 29 14:48:02 2023, max compression
+gzip compressed data, was "vectortile-1.4.1.tar", last modified: Thu Jun 29 15:07:23 2023, max compression
```

## Comparing `vectortile-1.4.0.tar` & `vectortile-1.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1075 2023-06-29 14:09:24.000000 vectortile-1.4.0/LICENSE
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       43 2023-06-29 14:09:24.000000 vectortile-1.4.0/MANIFEST.in
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 14:48:02.081652 vectortile-1.4.0/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     4321 2023-06-29 14:09:24.000000 vectortile-1.4.0/README.md
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 14:09:24.000000 vectortile-1.4.0/requirements.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-29 14:48:02.081652 vectortile-1.4.0/setup.cfg
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      975 2023-06-29 14:47:50.000000 vectortile-1.4.0/setup.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2041 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/Bbox.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1903 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/Tile.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3083 2023-06-29 14:13:22.000000 vectortile-1.4.0/vectortile/TileBounds.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     6202 2023-06-29 14:42:56.000000 vectortile-1.4.0/vectortile/TypedMatrix.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      195 2023-06-29 14:13:09.000000 vectortile-1.4.0/vectortile/__init__.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile/tests/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/__init__.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      411 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_Bbox.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      685 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_Tile.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     2110 2023-06-29 14:09:24.000000 vectortile-1.4.0/vectortile/tests/test_TileBounds.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     3873 2023-06-29 14:42:21.000000 vectortile-1.4.0/vectortile/tests/test_TypedMatrix.py
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     1276 2023-06-29 14:46:00.000000 vectortile-1.4.0/vectortile/version.py
-drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:48:02.081652 vectortile-1.4.0/vectortile.egg-info/
--rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/PKG-INFO
--rw-rw-r--   0 redhog    (1000) redhog    (1000)      520 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/SOURCES.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/dependency_links.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/requires.txt
--rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2023-06-29 14:48:02.000000 vectortile-1.4.0/vectortile.egg-info/top_level.txt
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 15:07:23.509858 vectortile-1.4.1/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1075 2023-06-29 14:09:24.000000 vectortile-1.4.1/LICENSE
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       43 2023-06-29 14:09:24.000000 vectortile-1.4.1/MANIFEST.in
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 15:07:23.509858 vectortile-1.4.1/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     4321 2023-06-29 14:09:24.000000 vectortile-1.4.1/README.md
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 14:09:24.000000 vectortile-1.4.1/requirements.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       38 2023-06-29 15:07:23.509858 vectortile-1.4.1/setup.cfg
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      975 2023-06-29 14:47:50.000000 vectortile-1.4.1/setup.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 15:07:23.509858 vectortile-1.4.1/vectortile/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2041 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/Bbox.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1903 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/Tile.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3083 2023-06-29 14:13:22.000000 vectortile-1.4.1/vectortile/TileBounds.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     6381 2023-06-29 15:04:15.000000 vectortile-1.4.1/vectortile/TypedMatrix.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      195 2023-06-29 14:13:09.000000 vectortile-1.4.1/vectortile/__init__.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 15:07:23.509858 vectortile-1.4.1/vectortile/tests/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        0 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/tests/__init__.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      411 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/tests/test_Bbox.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      685 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/tests/test_Tile.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     2110 2023-06-29 14:09:24.000000 vectortile-1.4.1/vectortile/tests/test_TileBounds.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     3873 2023-06-29 14:42:21.000000 vectortile-1.4.1/vectortile/tests/test_TypedMatrix.py
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     1276 2023-06-29 15:07:03.000000 vectortile-1.4.1/vectortile/version.py
+drwxrwxr-x   0 redhog    (1000) redhog    (1000)        0 2023-06-29 15:07:23.509858 vectortile-1.4.1/vectortile.egg-info/
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)     5902 2023-06-29 15:07:23.000000 vectortile-1.4.1/vectortile.egg-info/PKG-INFO
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)      520 2023-06-29 15:07:23.000000 vectortile-1.4.1/vectortile.egg-info/SOURCES.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)        1 2023-06-29 15:07:23.000000 vectortile-1.4.1/vectortile.egg-info/dependency_links.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       37 2023-06-29 15:07:23.000000 vectortile-1.4.1/vectortile.egg-info/requires.txt
+-rw-rw-r--   0 redhog    (1000) redhog    (1000)       11 2023-06-29 15:07:23.000000 vectortile-1.4.1/vectortile.egg-info/top_level.txt
```

### Comparing `vectortile-1.4.0/LICENSE` & `vectortile-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/PKG-INFO` & `vectortile-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectortile
-Version: 1.4.0
+Version: 1.4.1
 Summary: A set of classes for managing tiles of geospatial vector data
 Home-page: https://github.com/emerald-geomodelling/vectortile
 Author: Paul Woods, Egil Moeller
 Author-email: paul@skytruth.org, em@emrld.no
 License: The MIT License (MIT)
         
         Copyright (c) 2014 SkyTruth
```

### Comparing `vectortile-1.4.0/README.md` & `vectortile-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/setup.py` & `vectortile-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/Bbox.py` & `vectortile-1.4.1/vectortile/Bbox.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/Tile.py` & `vectortile-1.4.1/vectortile/Tile.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/TileBounds.py` & `vectortile-1.4.1/vectortile/TileBounds.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/TypedMatrix.py` & `vectortile-1.4.1/vectortile/TypedMatrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 version = 2
 
 import io
 import struct
 import json
 import calendar
 from datetime import datetime
+try:
+    import pandas
+except:
+    pandas = None
 
 # Header Structure
 # {
 #   length: count of rows of data
 #   version: format version
 #   cols: array of column definitions
 #       [{}
@@ -21,14 +25,16 @@
 # }
 
 typemap = {
     int: 'Float32',
     float: 'Float32',
     datetime: 'Float32',
 }
+if pandas:
+    typemap[pandas.Timestamp] = 'Float32'
 typeformatmap = {
     'Float32': 'f',
 }
 typedefaultmap = {
     'Float32': 0.0,
 }
 
@@ -84,14 +90,17 @@
     If a list of columns is not given, the columns are derived from the data using get_columns()
     extra_header_fields can supply an optional dict with additional fields to be included in the packed header
 
     orientation can be 'rowwise' or 'columnwise'.   For row-wise orientation, the typedmatrix will stored as a list of rows.
     for column-wise oreintation it is stored as a list of columns.
     """
 
+    if hasattr(data, "to_dict"):
+        data = data.to_dict('records')
+    
     # make data iterable
     if type(data) is dict:
         data = [data]
 
     if extra_header_fields:
         header = dict(extra_header_fields)
     else:
```

### Comparing `vectortile-1.4.0/vectortile/tests/test_Tile.py` & `vectortile-1.4.1/vectortile/tests/test_Tile.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/tests/test_TileBounds.py` & `vectortile-1.4.1/vectortile/tests/test_TileBounds.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/tests/test_TypedMatrix.py` & `vectortile-1.4.1/vectortile/tests/test_TypedMatrix.py`

 * *Files identical despite different names*

### Comparing `vectortile-1.4.0/vectortile/version.py` & `vectortile-1.4.1/vectortile/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.4.0'
+__version__ = '1.4.1'
 __author__ = 'Paul Woods, Egil Moeller'
 __author_email__ = 'paul@skytruth.org, em@emrld.no'
 __source__ = 'https://github.com/emerald-geomodelling/vectortile'
 __license__ = """The MIT License (MIT)
 
 Copyright (c) 2014 SkyTruth
```

### Comparing `vectortile-1.4.0/vectortile.egg-info/PKG-INFO` & `vectortile-1.4.1/vectortile.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectortile
-Version: 1.4.0
+Version: 1.4.1
 Summary: A set of classes for managing tiles of geospatial vector data
 Home-page: https://github.com/emerald-geomodelling/vectortile
 Author: Paul Woods, Egil Moeller
 Author-email: paul@skytruth.org, em@emrld.no
 License: The MIT License (MIT)
         
         Copyright (c) 2014 SkyTruth
```

### Comparing `vectortile-1.4.0/vectortile.egg-info/SOURCES.txt` & `vectortile-1.4.1/vectortile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

