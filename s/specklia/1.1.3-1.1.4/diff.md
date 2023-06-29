# Comparing `tmp/specklia-1.1.3.tar.gz` & `tmp/specklia-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.3.tar", last modified: Thu Jun 29 09:11:28 2023, max compression
+gzip compressed data, was "specklia-1.1.4.tar", last modified: Thu Jun 29 10:17:31 2023, max compression
```

## Comparing `specklia-1.1.3.tar` & `specklia-1.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:11:28.014274 specklia-1.1.3/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 09:11:15.000000 specklia-1.1.3/LICENCE
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 09:11:28.014274 specklia-1.1.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 09:11:15.000000 specklia-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 09:11:28.014274 specklia-1.1.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-29 09:11:15.000000 specklia-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:11:28.014274 specklia-1.1.3/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 09:11:15.000000 specklia-1.1.3/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24282 2023-06-29 09:11:15.000000 specklia-1.1.3/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 09:11:15.000000 specklia-1.1.3/specklia/websocket_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:11:28.014274 specklia-1.1.3/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 09:11:27.000000 specklia-1.1.3/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 09:11:27.000000 specklia-1.1.3/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 09:11:27.000000 specklia-1.1.3/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-29 09:11:27.000000 specklia-1.1.3/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 09:11:27.000000 specklia-1.1.3/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:11:28.014274 specklia-1.1.3/tests/
--rw-r--r--   0 root         (0) root         (0)    10065 2023-06-29 09:11:15.000000 specklia-1.1.3/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 09:11:15.000000 specklia-1.1.3/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 09:58:06.000000 specklia-1.1.4/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 10:17:31.108687 specklia-1.1.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 09:58:06.000000 specklia-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 10:17:31.108687 specklia-1.1.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1527 2023-06-29 09:58:06.000000 specklia-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 09:58:06.000000 specklia-1.1.4/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24283 2023-06-29 10:17:28.000000 specklia-1.1.4/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 09:58:06.000000 specklia-1.1.4/specklia/websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 10:17:31.000000 specklia-1.1.4/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:17:31.108687 specklia-1.1.4/tests/
+-rw-r--r--   0 root         (0) root         (0)    10065 2023-06-29 10:17:28.000000 specklia-1.1.4/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 09:58:06.000000 specklia-1.1.4/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.3/LICENCE` & `specklia-1.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.3/PKG-INFO` & `specklia-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.3/README.md` & `specklia-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.3/setup.py` & `specklia-1.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,10 +36,11 @@
     install_requires=[
         'blosc',
         'flask',
         'geopandas',
         'pandas',
         'requests',
         'shapely',
-        'simple-websocket'
+        'simple-websocket',
+        'sphinx_rtd_theme'
     ],
 )
```

### Comparing `specklia-1.1.3/specklia/client.py` & `specklia-1.1.4/specklia/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,14 +496,15 @@
             A list of columns should follow the format:
                 [{'name': 'elevation', 'type': 'float', 'description': 'elevation', 'unit': 'metres'},
                  {'name': 'remarks', 'type': 'str', 'description': 'per-row remarks', 'unit': 'NA'}]
             Where valid values for 'type' are 'string', 'float' and 'int' and the other three fields are strings,
             which must contain alphanumeric characters, spaces, underscores and hyphens only.
             Please do not create explicit EPSG:4326 columns (e.g. 'lat', 'lon') or POSIX timestamp columns
             as these are unnecessary repetitions of Specklia default columns.
+
         Returns
         -------
         str
             The unique ID of the newly created dataset.
         """
         if columns and any(x in ['lat', 'lon', 'long', 'latitude', 'longitude', 'timestamp', 'posix']
                            for x in [col['name'].lower() for col in columns]):
```

### Comparing `specklia-1.1.3/specklia/websocket_helpers.py` & `specklia-1.1.4/specklia/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.3/specklia.egg-info/PKG-INFO` & `specklia-1.1.4/specklia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.3/tests/test_client.py` & `specklia-1.1.4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.3/tests/test_websocket_helpers.py` & `specklia-1.1.4/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

