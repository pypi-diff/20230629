# Comparing `tmp/drf-rehive-extras-1.0.7.tar.gz` & `tmp/drf-rehive-extras-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-1.0.7.tar", last modified: Thu Jun 29 14:43:51 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-2.0.0.tar", last modified: Thu Jun 29 20:19:18 2023, max compression
```

## Comparing `drf-rehive-extras-1.0.7.tar` & `drf-rehive-extras-2.0.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-1.0.7/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7172 2023-06-29 14:40:40.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-29 14:42:37.000000 drf-rehive-extras-1.0.7/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-2.0.0/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7164 2023-06-29 20:18:25.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-2.0.0/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-29 20:18:35.000000 drf-rehive-extras-2.0.0/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-2.0.0/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 20:19:18.000000 drf-rehive-extras-2.0.0/PKG-INFO
```

### Comparing `drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-2.0.0/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.7
+Version: 2.0.0
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.7.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.0.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-1.0.7/README.md` & `drf-rehive-extras-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.7/drf_rehive_extras/mixins.py` & `drf-rehive-extras-2.0.0/drf_rehive_extras/mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
         # Handle serialization and destroy.
         serializer = self.get_serializer(instance, data=request.data)
         self.perform_destroy(serializer)
 
         return Response(
             data={'status': 'success'},
-            status=self.get_response_status_code(status.HTTP_204_NO_CONTENT)
+            status=self.get_response_status_code(status.HTTP_200_OK)
         )
 
     def perform_destroy(self, serializer):
         """
         Perform destroy using the serializer.
         """
```

### Comparing `drf-rehive-extras-1.0.7/drf_rehive_extras/pagination.py` & `drf-rehive-extras-2.0.0/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.7/drf_rehive_extras/generics.py` & `drf-rehive-extras-2.0.0/drf_rehive_extras/generics.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.7/drf_rehive_extras/fields.py` & `drf-rehive-extras-2.0.0/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.7/setup.py` & `drf-rehive-extras-2.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '1.0.7'
+VERSION = '2.0.0'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-1.0.7/LICENSE` & `drf-rehive-extras-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.7/PKG-INFO` & `drf-rehive-extras-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.7
+Version: 2.0.0
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.7.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/2.0.0.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

