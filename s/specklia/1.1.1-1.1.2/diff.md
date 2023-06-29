# Comparing `tmp/specklia-1.1.1.tar.gz` & `tmp/specklia-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specklia-1.1.1.tar", last modified: Thu Jun 29 08:38:20 2023, max compression
+gzip compressed data, was "specklia-1.1.2.tar", last modified: Thu Jun 29 08:50:40 2023, max compression
```

## Comparing `specklia-1.1.1.tar` & `specklia-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:38:20.791806 specklia-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 08:34:52.000000 specklia-1.1.1/LICENCE
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 08:38:20.791806 specklia-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 08:34:52.000000 specklia-1.1.1/README.md
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 08:38:20.791806 specklia-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1499 2023-06-29 08:34:52.000000 specklia-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:38:20.787806 specklia-1.1.1/specklia/
--rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 08:34:52.000000 specklia-1.1.1/specklia/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24282 2023-06-29 08:34:52.000000 specklia-1.1.1/specklia/client.py
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 08:34:52.000000 specklia-1.1.1/specklia/websocket_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:38:20.787806 specklia-1.1.1/specklia.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 08:38:20.000000 specklia-1.1.1/specklia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 08:38:20.000000 specklia-1.1.1/specklia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:38:20.000000 specklia-1.1.1/specklia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-29 08:38:20.000000 specklia-1.1.1/specklia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 08:38:20.000000 specklia-1.1.1/specklia.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:38:20.791806 specklia-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)    10065 2023-06-29 08:34:52.000000 specklia-1.1.1/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 08:34:52.000000 specklia-1.1.1/tests/test_websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:50:40.031768 specklia-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-06-29 08:36:21.000000 specklia-1.1.2/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 08:50:40.031768 specklia-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-29 08:36:21.000000 specklia-1.1.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 08:50:40.031768 specklia-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-29 08:36:21.000000 specklia-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:50:40.031768 specklia-1.1.2/specklia/
+-rw-r--r--   0 root         (0) root         (0)       51 2023-06-29 08:36:21.000000 specklia-1.1.2/specklia/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24282 2023-06-29 08:36:21.000000 specklia-1.1.2/specklia/client.py
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-29 08:36:21.000000 specklia-1.1.2/specklia/websocket_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:50:40.031768 specklia-1.1.2/specklia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3467 2023-06-29 08:50:39.000000 specklia-1.1.2/specklia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 08:50:39.000000 specklia-1.1.2/specklia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 08:50:39.000000 specklia-1.1.2/specklia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-29 08:50:39.000000 specklia-1.1.2/specklia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 08:50:39.000000 specklia-1.1.2/specklia.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 08:50:40.031768 specklia-1.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)    10065 2023-06-29 08:36:21.000000 specklia-1.1.2/tests/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     6631 2023-06-29 08:36:21.000000 specklia-1.1.2/tests/test_websocket_helpers.py
```

### Comparing `specklia-1.1.1/LICENCE` & `specklia-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/PKG-INFO` & `specklia-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.1/README.md` & `specklia-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/setup.py` & `specklia-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/specklia/client.py` & `specklia-1.1.2/specklia/client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/specklia/websocket_helpers.py` & `specklia-1.1.2/specklia/websocket_helpers.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/specklia.egg-info/PKG-INFO` & `specklia-1.1.2/specklia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specklia
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python client for Specklia, a geospatial point cloud database by Earthwave.
 Home-page: https://specklia.earthwave.co.uk/
 Author: Earthwave Ltd
 Author-email: info@earthwave.co.uk
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `specklia-1.1.1/tests/test_client.py` & `specklia-1.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `specklia-1.1.1/tests/test_websocket_helpers.py` & `specklia-1.1.2/tests/test_websocket_helpers.py`

 * *Files identical despite different names*

