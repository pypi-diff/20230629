# Comparing `tmp/drf-rehive-extras-1.0.6.tar.gz` & `tmp/drf-rehive-extras-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-1.0.6.tar", last modified: Thu Jun 29 14:13:15 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-1.0.7.tar", last modified: Thu Jun 29 14:43:51 2023, max compression
```

## Comparing `drf-rehive-extras-1.0.6.tar` & `drf-rehive-extras-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-1.0.6/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7486 2023-06-29 14:10:41.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-29 14:11:53.000000 drf-rehive-extras-1.0.6/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-1.0.7/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7172 2023-06-29 14:40:40.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-1.0.7/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-29 14:42:37.000000 drf-rehive-extras-1.0.7/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.7/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:43:51.000000 drf-rehive-extras-1.0.7/PKG-INFO
```

### Comparing `drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-1.0.7/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.6.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.7.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-1.0.6/README.md` & `drf-rehive-extras-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.6/drf_rehive_extras/mixins.py` & `drf-rehive-extras-1.0.7/drf_rehive_extras/mixins.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,18 +56,15 @@
         add_resource_data(request, serializer.instance)
 
         # Attach creation success headers.
         headers = self.get_success_headers(serializer.data)
 
         # Handle the response serialization. Sometimes the serialization of
         # responses should be different from the request serialization.
-        response_serializer = self.get_response_serializer()
-        data = response_serializer(
-            serializer.instance, context=self.get_serializer_context()
-        ).data if response_serializer else serializer.data
+        data = self.get_response_serializer(serializer.instance).data
 
         return Response(
             data={'status': 'success', 'data': data},
             status=self.get_response_status_code(status.HTTP_201_CREATED),
             headers=headers
         )
 
@@ -199,18 +196,15 @@
             instance, data=request.data, partial=partial
         )
         serializer.is_valid(raise_exception=True)
         self.perform_update(serializer)
 
         # Handle the response serialization. Sometimes the serialization of
         # responses should be different from the request serialization.
-        response_serializer = self.get_response_serializer()
-        data = response_serializer(
-            serializer.instance, context=self.get_serializer_context()
-        ).data if response_serializer else serializer.data
+        data = self.get_response_serializer(serializer.instance).data
 
         return Response(
             data={'status': 'success', 'data': data},
             status=self.get_response_status_code(status.HTTP_200_OK),
         )
 
     def perform_update(self, serializer):
```

### Comparing `drf-rehive-extras-1.0.6/drf_rehive_extras/pagination.py` & `drf-rehive-extras-1.0.7/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.6/drf_rehive_extras/generics.py` & `drf-rehive-extras-1.0.7/drf_rehive_extras/generics.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.6/drf_rehive_extras/fields.py` & `drf-rehive-extras-1.0.7/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.6/setup.py` & `drf-rehive-extras-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '1.0.6'
+VERSION = '1.0.7'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-1.0.6/LICENSE` & `drf-rehive-extras-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.6/PKG-INFO` & `drf-rehive-extras-1.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.6
+Version: 1.0.7
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.6.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.7.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

