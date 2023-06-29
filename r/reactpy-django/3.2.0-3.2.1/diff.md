# Comparing `tmp/reactpy_django-3.2.0.tar.gz` & `tmp/reactpy_django-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reactpy_django-3.2.0.tar", last modified: Fri Jun 23 22:41:39 2023, max compression
+gzip compressed data, was "reactpy_django-3.2.1.tar", last modified: Thu Jun 29 20:01:08 2023, max compression
```

## Comparing `reactpy_django-3.2.0.tar` & `reactpy_django-3.2.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-23 22:41:39.994863 reactpy_django-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10356 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/http/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/reactpy_django/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/
--rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.986863 reactpy_django-3.2.0/src/reactpy_django/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/templates/reactpy/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templates/reactpy/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/templatetags/reactpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13908 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-23 22:41:08.000000 reactpy_django-3.2.0/src/reactpy_django/websocket/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 22:41:39.990862 reactpy_django-3.2.0/src/reactpy_django.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 22:41:33.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 22:41:39.000000 reactpy_django-3.2.0/src/reactpy_django.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10305 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/http/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0002_rename_created_at_componentparams_last_accessed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/
+-rw-r--r--   0 runner    (1001) docker     (123)   166388 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.881083 reactpy_django-3.2.1/src/reactpy_django/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/templates/reactpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templates/reactpy/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/templatetags/reactpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-29 20:00:33.000000 reactpy_django-3.2.1/src/reactpy_django/websocket/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:01:08.885084 reactpy_django-3.2.1/src/reactpy_django.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:01:01.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 20:01:08.000000 reactpy_django-3.2.1/src/reactpy_django.egg-info/top_level.txt
```

### Comparing `reactpy_django-3.2.0/LICENSE` & `reactpy_django-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/PKG-INFO` & `reactpy_django-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy_django
-Version: 3.2.0
+Version: 3.2.1
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy_django Version: 3.2.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy_django Version: 3.2.1 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.2.0/README.md` & `reactpy_django-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/pyproject.toml` & `reactpy_django-3.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/setup.py` & `reactpy_django-3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/components.py` & `reactpy_django-3.2.1/src/reactpy_django/components.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/config.py` & `reactpy_django-3.2.1/src/reactpy_django/config.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/decorators.py` & `reactpy_django-3.2.1/src/reactpy_django/decorators.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/hooks.py` & `reactpy_django-3.2.1/src/reactpy_django/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,17 +153,15 @@
                     )(new_data, **query_options.postprocessor_kwargs)
 
         # Log any errors and set the error state
         except Exception as e:
             set_data(None)
             set_loading(False)
             set_error(e)
-            _logger.exception(
-                f"Failed to execute query: {generate_obj_name(query) or query}"
-            )
+            _logger.exception(f"Failed to execute query: {generate_obj_name(query)}")
             return
 
         # Query was successful
         else:
             set_data(new_data)
             set_loading(False)
             set_error(None)
@@ -248,15 +246,15 @@
                 )(*exec_args, **exec_kwargs)
 
         # Log any errors and set the error state
         except Exception as e:
             set_loading(False)
             set_error(e)
             _logger.exception(
-                f"Failed to execute mutation: {generate_obj_name(mutation) or mutation}"
+                f"Failed to execute mutation: {generate_obj_name(mutation)}"
             )
 
         # Mutation was successful
         else:
             set_loading(False)
             set_error(None)
```

### Comparing `reactpy_django-3.2.0/src/reactpy_django/http/views.py` & `reactpy_django-3.2.1/src/reactpy_django/http/views.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/migrations/0001_initial.py` & `reactpy_django-3.2.1/src/reactpy_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py` & `reactpy_django-3.2.1/src/reactpy_django/migrations/0003_componentsession_delete_componentparams.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/static/reactpy_django/client.js` & `reactpy_django-3.2.1/src/reactpy_django/static/reactpy_django/client.js`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/templatetags/reactpy.py` & `reactpy_django-3.2.1/src/reactpy_django/templatetags/reactpy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+from logging import getLogger
 from uuid import uuid4
 
 import dill as pickle
 from django import template
 from django.urls import reverse
 
 from reactpy_django import models
 from reactpy_django.config import (
     REACTPY_DATABASE,
+    REACTPY_DEBUG_MODE,
     REACTPY_RECONNECT_MAX,
     REACTPY_WEBSOCKET_URL,
 )
+from reactpy_django.exceptions import ComponentDoesNotExistError, ComponentParamError
 from reactpy_django.types import ComponentParamData
-from reactpy_django.utils import _register_component, func_has_params
+from reactpy_django.utils import (
+    _register_component,
+    check_component_args,
+    func_has_args,
+)
 
 
 REACTPY_WEB_MODULES_URL = reverse("reactpy:web_modules", args=["x"])[:-1][1:]
 register = template.Library()
+_logger = getLogger(__name__)
 
 
 @register.inclusion_tag("reactpy/component.html")
 def component(dotted_path: str, *args, **kwargs):
     """This tag is used to embed an existing ReactPy component into your HTML template.
 
     Args:
@@ -35,33 +43,63 @@
         <!DOCTYPE html>
         <html>
         <body>
             {% component "example_project.my_app.components.hello_world" recipient="World" %}
         </body>
         </html>
     """
-    component = _register_component(dotted_path)
-    uuid = uuid4().hex
-    class_ = kwargs.pop("class", "")
-    kwargs.pop("key", "")  # `key` is effectively useless for the root node
+
+    # Register the component if needed
+    try:
+        component = _register_component(dotted_path)
+        uuid = uuid4().hex
+        class_ = kwargs.pop("class", "")
+        kwargs.pop("key", "")  # `key` is effectively useless for the root node
+
+    except Exception as e:
+        if isinstance(e, ComponentDoesNotExistError):
+            _logger.error(str(e))
+        else:
+            _logger.exception(
+                "An unknown error has occurred while registering component '%s'.",
+                dotted_path,
+            )
+        return failure_context(dotted_path, e)
 
     # Store the component's args/kwargs in the database if needed
     # This will be fetched by the websocket consumer later
     try:
-        if func_has_params(component, *args, **kwargs):
+        check_component_args(component, *args, **kwargs)
+        if func_has_args(component):
             params = ComponentParamData(args, kwargs)
             model = models.ComponentSession(uuid=uuid, params=pickle.dumps(params))
             model.full_clean()
             model.save(using=REACTPY_DATABASE)
-    except TypeError as e:
-        raise TypeError(
-            f"The provided parameters are incompatible with component '{dotted_path}'."
-        ) from e
 
+    except Exception as e:
+        if isinstance(e, ComponentParamError):
+            _logger.error(str(e))
+        else:
+            _logger.exception(
+                "An unknown error has occurred while saving component params for '%s'.",
+                dotted_path,
+            )
+        return failure_context(dotted_path, e)
+
+    # Return the template rendering context
     return {
         "class": class_,
         "reactpy_websocket_url": REACTPY_WEBSOCKET_URL,
         "reactpy_web_modules_url": REACTPY_WEB_MODULES_URL,
         "reactpy_reconnect_max": REACTPY_RECONNECT_MAX,
         "reactpy_mount_uuid": uuid,
         "reactpy_component_path": f"{dotted_path}/{uuid}/",
     }
+
+
+def failure_context(dotted_path: str, error: Exception):
+    return {
+        "reactpy_failure": True,
+        "reactpy_debug_mode": REACTPY_DEBUG_MODE,
+        "reactpy_dotted_path": dotted_path,
+        "reactpy_error": type(error).__name__,
+    }
```

### Comparing `reactpy_django-3.2.0/src/reactpy_django/types.py` & `reactpy_django-3.2.1/src/reactpy_django/types.py`

 * *Files identical despite different names*

### Comparing `reactpy_django-3.2.0/src/reactpy_django/utils.py` & `reactpy_django-3.2.1/src/reactpy_django/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 from django.db.models.query import QuerySet
 from django.http import HttpRequest, HttpResponse
 from django.template import engines
 from django.utils import timezone
 from django.utils.encoding import smart_str
 from django.views import View
 
+from reactpy_django.exceptions import ComponentDoesNotExistError, ComponentParamError
+
 
 _logger = logging.getLogger(__name__)
 _component_tag = r"(?P<tag>component)"
-_component_path = r"(?P<path>(\"[^\"'\s]+\")|('[^\"'\s]+'))"
-_component_kwargs = r"(?P<kwargs>(.*?|\s*?)*)"
-COMMENT_REGEX = re.compile(r"(<!--)(.|\s)*?(-->)")
+_component_path = r"(?P<path>\"[^\"'\s]+\"|'[^\"'\s]+')"
+_component_kwargs = r"(?P<kwargs>[\s\S]*?)"
+COMMENT_REGEX = re.compile(r"<!--[\s\S]*?-->")
 COMPONENT_REGEX = re.compile(
     r"{%\s*"
     + _component_tag
     + r"\s*"
     + _component_path
     + r"\s*"
     + _component_kwargs
@@ -87,15 +89,20 @@
     This should only be called on startup to maintain synchronization during mulitprocessing.
     """
     from reactpy_django.config import REACTPY_REGISTERED_COMPONENTS
 
     if dotted_path in REACTPY_REGISTERED_COMPONENTS:
         return REACTPY_REGISTERED_COMPONENTS[dotted_path]
 
-    REACTPY_REGISTERED_COMPONENTS[dotted_path] = import_dotted_path(dotted_path)
+    try:
+        REACTPY_REGISTERED_COMPONENTS[dotted_path] = import_dotted_path(dotted_path)
+    except AttributeError as e:
+        raise ComponentDoesNotExistError(
+            f"Error while fetching '{dotted_path}'. {(str(e).capitalize())}."
+        ) from e
     _logger.debug("ReactPy has registered component %s", dotted_path)
     return REACTPY_REGISTERED_COMPONENTS[dotted_path]
 
 
 def import_dotted_path(dotted_path: str) -> Callable:
     """Imports a dotted path and returns the callable."""
     module_name, component_name = dotted_path.rsplit(".", 1)
@@ -206,23 +213,26 @@
                     "This component path may not be valid, "
                     "or an exception may have occurred while importing."
                     "\033[0m",
                     component,
                 )
 
 
-def generate_obj_name(object: Any) -> str | None:
+def generate_obj_name(object: Any) -> str:
     """Makes a best effort to create a name for an object.
     Useful for JSON serialization of Python objects."""
     if hasattr(object, "__module__"):
         if hasattr(object, "__name__"):
             return f"{object.__module__}.{object.__name__}"
         if hasattr(object, "__class__"):
             return f"{object.__module__}.{object.__class__.__name__}"
-    return None
+
+    with contextlib.suppress(Exception):
+        return str(object)
+    return ""
 
 
 def django_query_postprocessor(
     data: QuerySet | Model, many_to_many: bool = True, many_to_one: bool = True
 ) -> QuerySet | Model:
     """Recursively fetch all fields within a `Model` or `QuerySet` to ensure they are not performed lazily.
 
@@ -280,28 +290,37 @@
             "  - You are attempting to use `use_query` to fetch non-ORM data.\n\n"
             "If these situations seem correct, you may want to consider disabling the postprocessor via `QueryOptions`."
         )
 
     return data
 
 
-def func_has_params(func: Callable, *args, **kwargs) -> bool:
-    """Checks if a function has any args or kwarg parameters.
-
-    Can optionally validate whether a set of args/kwargs would work on the given function.
-    """
+def func_has_args(func: Callable) -> bool:
+    """Checks if a function has any args or kwarg."""
     signature = inspect.signature(func)
 
     # Check if the function has any args/kwargs
-    if not args and not kwargs:
-        return str(signature) != "()"
+    return str(signature) != "()"
+
 
-    # Check if the function has the given args/kwargs
-    signature.bind(*args, **kwargs)
-    return True
+def check_component_args(func: Callable, *args, **kwargs):
+    """
+    Validate whether a set of args/kwargs would work on the given function.
+
+    Raises `ComponentParamError` if the args/kwargs are invalid.
+    """
+    signature = inspect.signature(func)
+
+    try:
+        signature.bind(*args, **kwargs)
+    except TypeError as e:
+        name = generate_obj_name(func)
+        raise ComponentParamError(
+            f"Invalid args for '{name}'. {str(e).capitalize()}."
+        ) from e
 
 
 def create_cache_key(*args):
     """Creates a cache key string that starts with `reactpy_django` contains
     all *args separated by `:`."""
 
     if not args:
```

### Comparing `reactpy_django-3.2.0/src/reactpy_django/websocket/consumer.py` & `reactpy_django-3.2.1/src/reactpy_django/websocket/consumer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from django.utils import timezone
 from reactpy.backend.hooks import ConnectionContext
 from reactpy.backend.types import Connection, Location
 from reactpy.core.layout import Layout
 from reactpy.core.serve import serve_layout
 
 from reactpy_django.types import ComponentParamData, ComponentWebsocket
-from reactpy_django.utils import db_cleanup, func_has_params
+from reactpy_django.utils import db_cleanup, func_has_args
 
 
 _logger = logging.getLogger(__name__)
 
 
 class ReactpyAsyncWebsocketConsumer(AsyncJsonWebsocketConsumer):
     """Communicates with the browser to perform actions on-demand."""
@@ -107,15 +107,15 @@
             _logger.warning(
                 f"Attempt to access invalid ReactPy component: {dotted_path!r}"
             )
             return
 
         # Fetch the component's args/kwargs from the database, if needed
         try:
-            if func_has_params(component_constructor):
+            if func_has_args(component_constructor):
                 try:
                     # Always clean up expired entries first
                     await database_sync_to_async(db_cleanup, thread_sensitive=False)()
 
                     # Get the queries from a DB
                     params_query = await models.ComponentSession.objects.using(
                         REACTPY_DATABASE
@@ -126,17 +126,16 @@
                     )
                     params_query.last_accessed = timezone.now()
                     await database_sync_to_async(
                         params_query.save, thread_sensitive=False
                     )()
                 except models.ComponentSession.DoesNotExist:
                     _logger.warning(
-                        f"Browser has attempted to access '{dotted_path}', "
-                        f"but the component has already expired beyond REACTPY_RECONNECT_MAX. "
-                        "If this was expected, this warning can be ignored."
+                        f"Component session for '{dotted_path}:{uuid}' not found. The "
+                        "session may have already expired beyond REACTPY_RECONNECT_MAX."
                     )
                     return
                 component_params: ComponentParamData = pickle.loads(params_query.params)
                 component_args = component_params.args
                 component_kwargs = component_params.kwargs
 
             # Generate the initial component instance
```

### Comparing `reactpy_django-3.2.0/src/reactpy_django.egg-info/PKG-INFO` & `reactpy_django-3.2.1/src/reactpy_django.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reactpy-django
-Version: 3.2.0
+Version: 3.2.1
 Summary: Control the web with Python
 Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead
 Author-email: ryan.morshead@gmail.com
 License: MIT
 Keywords: interactive,widgets,DOM,React
 Platform: Linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: reactpy-django Version: 3.2.0 Summary: Control the
+Metadata-Version: 2.1 Name: reactpy-django Version: 3.2.1 Summary: Control the
 web with Python Home-page: https://github.com/reactive-python/reactpy-django
 Author: Ryan Morshead Author-email: ryan.morshead@gmail.com License: MIT
 Keywords: interactive,widgets,DOM,React Platform: Linux Platform: Mac OS X
 Platform: Windows Classifier: Framework :: Django Classifier: Framework ::
 Django :: 4.0 Classifier: Operating System :: OS Independent Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: Topic :: Multimedia :: Graphics Classifier: Programming
```

### Comparing `reactpy_django-3.2.0/src/reactpy_django.egg-info/SOURCES.txt` & `reactpy_django-3.2.1/src/reactpy_django.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 setup.cfg
 setup.py
 src/reactpy_django/__init__.py
 src/reactpy_django/apps.py
 src/reactpy_django/components.py
 src/reactpy_django/config.py
 src/reactpy_django/decorators.py
+src/reactpy_django/exceptions.py
 src/reactpy_django/hooks.py
 src/reactpy_django/models.py
 src/reactpy_django/py.typed
 src/reactpy_django/types.py
 src/reactpy_django/utils.py
 src/reactpy_django.egg-info/PKG-INFO
 src/reactpy_django.egg-info/SOURCES.txt
```

