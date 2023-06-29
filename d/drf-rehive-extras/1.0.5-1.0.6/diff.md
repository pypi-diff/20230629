# Comparing `tmp/drf-rehive-extras-1.0.5.tar.gz` & `tmp/drf-rehive-extras-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drf-rehive-extras-1.0.5.tar", last modified: Thu Feb 16 20:40:29 2023, max compression
+gzip compressed data, was "dist/drf-rehive-extras-1.0.6.tar", last modified: Thu Jun 29 14:13:15 2023, max compression
```

## Comparing `drf-rehive-extras-1.0.5.tar` & `drf-rehive-extras-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/dependency_links.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-1.0.5/README.md
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/setup.cfg
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/serializers.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     7121 2023-02-16 20:38:10.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/mixins.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/pagination.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     4403 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/generics.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/apps.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-1.0.5/drf_rehive_extras/fields.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-02-16 20:25:02.000000 drf-rehive-extras-1.0.5/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/MANIFEST.in
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.5/LICENSE
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-02-16 20:40:29.000000 drf-rehive-extras-1.0.5/PKG-INFO
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/top_level.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      108 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/requires.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      459 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/PKG-INFO
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      753 2022-09-20 12:21:57.000000 drf-rehive-extras-1.0.6/README.md
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/setup.cfg
+drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      256 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/serializers.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       61 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/__init__.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     7486 2023-06-29 14:10:41.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/mixins.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1183 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/pagination.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     6049 2023-06-29 13:57:52.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/generics.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)      131 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/apps.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     2678 2022-09-20 21:52:23.000000 drf-rehive-extras-1.0.6/drf_rehive_extras/fields.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1741 2023-06-29 14:11:53.000000 drf-rehive-extras-1.0.6/setup.py
+-rw-r--r--   0 joshua    (1000) joshua    (1000)       18 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/MANIFEST.in
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1063 2022-01-20 20:14:53.000000 drf-rehive-extras-1.0.6/LICENSE
+-rw-r--r--   0 joshua    (1000) joshua    (1000)     1860 2023-06-29 14:13:15.000000 drf-rehive-extras-1.0.6/PKG-INFO
```

### Comparing `drf-rehive-extras-1.0.5/drf_rehive_extras.egg-info/PKG-INFO` & `drf-rehive-extras-1.0.6/drf_rehive_extras.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.5
+Version: 1.0.6
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.5.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.6.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

### Comparing `drf-rehive-extras-1.0.5/README.md` & `drf-rehive-extras-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.5/drf_rehive_extras/mixins.py` & `drf-rehive-extras-1.0.6/drf_rehive_extras/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,35 +43,35 @@
     """
 
     def create(self, request, *args, **kwargs):
         """
         Handle object creation on the view.
         """
 
-        # Handle serialization and update.
+        # Handle the request serialization and creation.
         serializer = self.get_serializer(data=request.data)
         serializer.is_valid(raise_exception=True)
         self.perform_create(serializer)
 
         # Inject resource data into the request.
         add_resource_data(request, serializer.instance)
 
         # Attach creation success headers.
         headers = self.get_success_headers(serializer.data)
 
         # Handle the response serialization. Sometimes the serialization of
-        # responses should be different from the create serialization.
-        _return_serializer = kwargs.get('return_serializer')
-        data = _return_serializer(
+        # responses should be different from the request serialization.
+        response_serializer = self.get_response_serializer()
+        data = response_serializer(
             serializer.instance, context=self.get_serializer_context()
-        ).data if _return_serializer else serializer.data
+        ).data if response_serializer else serializer.data
 
         return Response(
-            {'status': 'success', 'data': data},
-            status=kwargs.get('return_status_code', status.HTTP_201_CREATED),
+            data={'status': 'success', 'data': data},
+            status=self.get_response_status_code(status.HTTP_201_CREATED),
             headers=headers
         )
 
     def perform_create(self, serializer):
         """
         Perform creation using the serializer.
         """
@@ -140,15 +140,18 @@
         if page is not None:
             serializer = self.get_serializer(page, many=True)
             return self.get_paginated_response(serializer.data)
 
         # Handle serialization.
         serializer = self.get_serializer(queryset, many=True)
 
-        return Response({'status': 'success', 'data': serializer.data})
+        return Response(
+            data={'status': 'success', 'data': serializer.data},
+            status=self.get_response_status_code(status.HTTP_200_OK)
+        )
 
 
 class RetrieveModelMixin:
     """
     Retrieve a model instance.
     """
 
@@ -162,25 +165,28 @@
 
         # Inject resource data into the request.
         add_resource_data(request, instance)
 
         # Handle serialization.
         serializer = self.get_serializer(instance)
 
-        return Response({'status': 'success', 'data': serializer.data})
+        return Response(
+            data={'status': 'success', 'data': serializer.data},
+            status=self.get_response_status_code(status.HTTP_200_OK)
+        )
 
 
 class UpdateModelMixin:
     """
     Update a model instance.
     """
 
     def update(self, request, *args, **kwargs):
         """
-        Hanlde object update on the view.
+        Handle object update on the view.
         """
 
         # Find out whether this is a partial (PATCH) or full (PUT) update.
         partial = kwargs.pop('partial', False)
 
         # Get a single object.
         instance = self.get_object()
@@ -192,21 +198,24 @@
         serializer = self.get_serializer(
             instance, data=request.data, partial=partial
         )
         serializer.is_valid(raise_exception=True)
         self.perform_update(serializer)
 
         # Handle the response serialization. Sometimes the serialization of
-        # responses should be different from the update serialization.
-        _return_serializer = kwargs.get('return_serializer')
-        data = _return_serializer(
+        # responses should be different from the request serialization.
+        response_serializer = self.get_response_serializer()
+        data = response_serializer(
             serializer.instance, context=self.get_serializer_context()
-        ).data if _return_serializer else serializer.data
+        ).data if response_serializer else serializer.data
 
-        return Response({'status': 'success', 'data': data})
+        return Response(
+            data={'status': 'success', 'data': data},
+            status=self.get_response_status_code(status.HTTP_200_OK),
+        )
 
     def perform_update(self, serializer):
         """
         Perform update using the serializer.
         """
 
         serializer.save()
@@ -237,15 +246,16 @@
         add_resource_data(request, instance)
 
         # Handle serialization and destroy.
         serializer = self.get_serializer(instance, data=request.data)
         self.perform_destroy(serializer)
 
         return Response(
-            data={'status': 'success'}, status=status.HTTP_200_OK
+            data={'status': 'success'},
+            status=self.get_response_status_code(status.HTTP_204_NO_CONTENT)
         )
 
     def perform_destroy(self, serializer):
         """
         Perform destroy using the serializer.
         """
```

### Comparing `drf-rehive-extras-1.0.5/drf_rehive_extras/pagination.py` & `drf-rehive-extras-1.0.6/drf_rehive_extras/pagination.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.5/drf_rehive_extras/fields.py` & `drf-rehive-extras-1.0.6/drf_rehive_extras/fields.py`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.5/setup.py` & `drf-rehive-extras-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from codecs import open
 from setuptools import find_packages, setup
 
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 
 with open(os.path.join(os.path.dirname(__file__), 'README.md')) as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
```

### Comparing `drf-rehive-extras-1.0.5/LICENSE` & `drf-rehive-extras-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-rehive-extras-1.0.5/PKG-INFO` & `drf-rehive-extras-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: drf-rehive-extras
-Version: 1.0.5
+Version: 1.0.6
 Summary: Extras for DRF
 Home-page: https://github.com/rehive/drf-rehive-extras
 Author: Rehive
 Author-email: info@rehive.com
 License: MIT
-Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.5.zip
+Download-URL: https://github.com/rehive/drf-rehive-extras/archive/1.0.6.zip
 Platform: UNKNOWN
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
```

