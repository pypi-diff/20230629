# Comparing `tmp/django-utilitas-1.3.8.tar.gz` & `tmp/django-utilitas-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-utilitas-1.3.8.tar", last modified: Tue May 16 13:17:17 2023, max compression
+gzip compressed data, was "django-utilitas-1.3.9.tar", last modified: Tue May 16 13:19:16 2023, max compression
```

## Comparing `django-utilitas-1.3.8.tar` & `django-utilitas-1.3.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:17:17.725072 django-utilitas-1.3.8/
--rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.8/LICENSE
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4941 2023-05-16 13:17:17.725363 django-utilitas-1.3.8/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4696 2023-05-16 13:17:04.000000 django-utilitas-1.3.8/README.md
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:17:17.709892 django-utilitas-1.3.8/django_utilitas.egg-info/
--rw-r--r--   0 jamesthiha   (501) staff       (20)     4941 2023-05-16 13:17:17.000000 django-utilitas-1.3.8/django_utilitas.egg-info/PKG-INFO
--rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-05-16 13:17:17.000000 django-utilitas-1.3.8/django_utilitas.egg-info/SOURCES.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-05-16 13:17:17.000000 django-utilitas-1.3.8/django_utilitas.egg-info/dependency_links.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-05-16 13:17:17.000000 django-utilitas-1.3.8/django_utilitas.egg-info/requires.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-05-16 13:17:17.000000 django-utilitas-1.3.8/django_utilitas.egg-info/top_level.txt
--rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-05-16 13:17:17.726453 django-utilitas-1.3.8/setup.cfg
--rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.8/setup.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:17:17.723045 django-utilitas-1.3.8/utilitas/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.8/utilitas/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.8/utilitas/admin.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.8/utilitas/apps.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.8/utilitas/exception_handler.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.8/utilitas/exceptions.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.8/utilitas/managers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.8/utilitas/metadata.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.8/utilitas/middlewares.py
-drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:17:17.724543 django-utilitas-1.3.8/utilitas/migrations/
--rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.8/utilitas/migrations/__init__.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     2481 2023-05-16 13:16:42.000000 django-utilitas-1.3.8/utilitas/models.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.8/utilitas/pagination.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.8/utilitas/renderer.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.8/utilitas/serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.8/utilitas/swagger_query_params.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.8/utilitas/swagger_serializers.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.8/utilitas/tests.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.8/utilitas/urls.py
--rw-r--r--   0 jamesthiha   (501) staff       (20)    17268 2023-05-16 13:11:12.000000 django-utilitas-1.3.8/utilitas/views.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:19:16.533434 django-utilitas-1.3.9/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    35149 2022-12-05 07:45:37.000000 django-utilitas-1.3.9/LICENSE
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4965 2023-05-16 13:19:16.533697 django-utilitas-1.3.9/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4720 2023-05-16 13:19:00.000000 django-utilitas-1.3.9/README.md
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:19:16.518703 django-utilitas-1.3.9/django_utilitas.egg-info/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     4965 2023-05-16 13:19:16.000000 django-utilitas-1.3.9/django_utilitas.egg-info/PKG-INFO
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      642 2023-05-16 13:19:16.000000 django-utilitas-1.3.9/django_utilitas.egg-info/SOURCES.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        1 2023-05-16 13:19:16.000000 django-utilitas-1.3.9/django_utilitas.egg-info/dependency_links.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       80 2023-05-16 13:19:16.000000 django-utilitas-1.3.9/django_utilitas.egg-info/requires.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        9 2023-05-16 13:19:16.000000 django-utilitas-1.3.9/django_utilitas.egg-info/top_level.txt
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      428 2023-05-16 13:19:16.534792 django-utilitas-1.3.9/setup.cfg
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      263 2022-12-05 08:04:03.000000 django-utilitas-1.3.9/setup.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:19:16.532275 django-utilitas-1.3.9/utilitas/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.9/utilitas/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       63 2022-11-28 18:11:49.000000 django-utilitas-1.3.9/utilitas/admin.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      148 2022-11-28 18:11:50.000000 django-utilitas-1.3.9/utilitas/apps.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      349 2022-12-05 07:27:09.000000 django-utilitas-1.3.9/utilitas/exception_handler.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 19:38:13.000000 django-utilitas-1.3.9/utilitas/exceptions.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       76 2022-12-05 07:26:41.000000 django-utilitas-1.3.9/utilitas/managers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      778 2022-12-05 03:43:29.000000 django-utilitas-1.3.9/utilitas/metadata.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      591 2023-01-25 15:05:12.000000 django-utilitas-1.3.9/utilitas/middlewares.py
+drwxr-xr-x   0 jamesthiha   (501) staff       (20)        0 2023-05-16 13:19:16.532986 django-utilitas-1.3.9/utilitas/migrations/
+-rw-r--r--   0 jamesthiha   (501) staff       (20)        0 2022-11-28 18:11:49.000000 django-utilitas-1.3.9/utilitas/migrations/__init__.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     2481 2023-05-16 13:16:42.000000 django-utilitas-1.3.9/utilitas/models.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1031 2023-02-22 06:50:16.000000 django-utilitas-1.3.9/utilitas/pagination.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      366 2022-11-28 19:43:27.000000 django-utilitas-1.3.9/utilitas/renderer.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)     1450 2023-02-19 23:16:44.000000 django-utilitas-1.3.9/utilitas/serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      945 2022-12-05 08:14:19.000000 django-utilitas-1.3.9/utilitas/swagger_query_params.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)      347 2022-11-28 19:35:23.000000 django-utilitas-1.3.9/utilitas/swagger_serializers.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       60 2022-11-28 18:11:49.000000 django-utilitas-1.3.9/utilitas/tests.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)       18 2022-11-28 18:28:32.000000 django-utilitas-1.3.9/utilitas/urls.py
+-rw-r--r--   0 jamesthiha   (501) staff       (20)    17278 2023-05-16 13:18:45.000000 django-utilitas-1.3.9/utilitas/views.py
```

### Comparing `django-utilitas-1.3.8/LICENSE` & `django-utilitas-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/PKG-INFO` & `django-utilitas-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.3.8
+Version: 1.3.9
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -116,14 +116,16 @@
 
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
+- 1.3.9
+    - bug fixes
 - 1.3.8
     - bug fixes
 - 1.3.7
     - bug fixes
 - 1.3.6
     - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
```

### Comparing `django-utilitas-1.3.8/README.md` & `django-utilitas-1.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
 
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
+- 1.3.9
+    - bug fixes
 - 1.3.8
     - bug fixes
 - 1.3.7
     - bug fixes
 - 1.3.6
     - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
```

### Comparing `django-utilitas-1.3.8/django_utilitas.egg-info/PKG-INFO` & `django-utilitas-1.3.9/django_utilitas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-utilitas
-Version: 1.3.8
+Version: 1.3.9
 Summary: Django package with useful utility classes
 Home-page: https://github.com/ninnroot/utilitas
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Django Utilitas
@@ -116,14 +116,16 @@
 
 requests.get("api/books?csv=true")
 ```
 
 
 ## Changelog
 
+- 1.3.9
+    - bug fixes
 - 1.3.8
     - bug fixes
 - 1.3.7
     - bug fixes
 - 1.3.6
     - added an alias option for model fields. (user_friendly_field attribute)
 - 1.3.5
```

### Comparing `django-utilitas-1.3.8/django_utilitas.egg-info/SOURCES.txt` & `django-utilitas-1.3.9/django_utilitas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/metadata.py` & `django-utilitas-1.3.9/utilitas/metadata.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/middlewares.py` & `django-utilitas-1.3.9/utilitas/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/models.py` & `django-utilitas-1.3.9/utilitas/models.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/pagination.py` & `django-utilitas-1.3.9/utilitas/pagination.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/serializers.py` & `django-utilitas-1.3.9/utilitas/serializers.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/swagger_query_params.py` & `django-utilitas-1.3.9/utilitas/swagger_query_params.py`

 * *Files identical despite different names*

### Comparing `django-utilitas-1.3.8/utilitas/views.py` & `django-utilitas-1.3.9/utilitas/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,30 +307,32 @@
     # )
     def get(self, request: Request):
         self.description = self.model.__doc__
 
         # if meta query_param is present, return metadata of the current endpoint
         if request.GET.get("meta"):
             return self.send_metadata(request)
+        
+        try:
+            query_params = self.get_query_params(request)
+        except BadRequest as e:
+            return self.send_response(
+                True, "bad_request", {"details": str(e)}, status=400
+            )
 
         if request.query_params.get("csv"):
             return self.send_csv(
                 request,
                 self.get_queryset(
                     request, None, None, True, **query_params
                 ),
                 fields=query_params["fields"],
             )
 
-        try:
-            query_params = self.get_query_params(request)
-        except BadRequest as e:
-            return self.send_response(
-                True, "bad_request", {"details": str(e)}, status=400
-            )
+
 
         serialized_data = self.get_queryset(request, **query_params)
 
         # return the serialized queryset in a standardized manner
         return self.send_response(
             False,
             "success",
```

