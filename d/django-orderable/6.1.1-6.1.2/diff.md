# Comparing `tmp/django-orderable-6.1.1.tar.gz` & `tmp/django-orderable-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-orderable-6.1.1.tar", last modified: Fri Oct 23 14:25:31 2020, max compression
+gzip compressed data, was "dist/django-orderable-6.1.2.tar", last modified: Thu Jun 29 19:28:25 2023, max compression
```

## Comparing `django-orderable-6.1.1.tar` & `django-orderable-6.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/
--rw-r--r--   0 max        (502) staff       (20)       76 2012-10-06 17:28:33.000000 django-orderable-6.1.1/MANIFEST.in
--rw-r--r--   0 max        (502) staff       (20)     4269 2020-10-23 14:25:31.000000 django-orderable-6.1.1/PKG-INFO
--rw-r--r--   0 max        (502) staff       (20)     2598 2020-06-20 12:06:11.000000 django-orderable-6.1.1/README.md
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/django_orderable.egg-info/
--rw-r--r--   0 max        (502) staff       (20)     4269 2020-10-23 14:25:30.000000 django-orderable-6.1.1/django_orderable.egg-info/PKG-INFO
--rw-r--r--   0 max        (502) staff       (20)      667 2020-10-23 14:25:30.000000 django-orderable-6.1.1/django_orderable.egg-info/SOURCES.txt
--rw-r--r--   0 max        (502) staff       (20)        1 2020-10-23 14:25:30.000000 django-orderable-6.1.1/django_orderable.egg-info/dependency_links.txt
--rw-r--r--   0 max        (502) staff       (20)       10 2020-10-23 14:25:30.000000 django-orderable-6.1.1/django_orderable.egg-info/top_level.txt
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/
--rw-r--r--   0 max        (502) staff       (20)        0 2014-05-16 11:58:11.000000 django-orderable-6.1.1/orderable/__init__.py
--rw-r--r--   0 max        (502) staff       (20)     2439 2019-03-07 08:41:14.000000 django-orderable-6.1.1/orderable/admin.py
--rw-r--r--   0 max        (502) staff       (20)      344 2019-03-06 11:37:02.000000 django-orderable-6.1.1/orderable/managers.py
--rw-r--r--   0 max        (502) staff       (20)     6710 2020-10-23 14:16:39.000000 django-orderable-6.1.1/orderable/models.py
--rw-r--r--   0 max        (502) staff       (20)     2885 2019-03-06 11:37:02.000000 django-orderable-6.1.1/orderable/querysets.py
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/static/
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/static/admin/
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/static/admin/img/
--rw-r--r--   0 max        (502) staff       (20)       76 2012-10-06 17:28:33.000000 django-orderable-6.1.1/orderable/static/admin/img/drag_handle.gif
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/templates/
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/templates/admin/
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/templates/admin/edit_inline/
--rw-r--r--   0 max        (502) staff       (20)     2709 2020-06-19 17:08:42.000000 django-orderable-6.1.1/orderable/templates/admin/edit_inline/orderable_tabular.html
--rw-r--r--   0 max        (502) staff       (20)     2844 2020-10-23 14:16:39.000000 django-orderable-6.1.1/orderable/templates/admin/orderable_change_list.html
-drwxr-xr-x   0 max        (502) staff       (20)        0 2020-10-23 14:25:31.000000 django-orderable-6.1.1/orderable/tests/
--rw-r--r--   0 max        (502) staff       (20)        0 2014-05-16 11:58:11.000000 django-orderable-6.1.1/orderable/tests/__init__.py
--rw-r--r--   0 max        (502) staff       (20)      478 2019-03-07 15:37:23.000000 django-orderable-6.1.1/orderable/tests/models.py
--rw-r--r--   0 max        (502) staff       (20)     2104 2019-03-07 08:41:14.000000 django-orderable-6.1.1/orderable/tests/run.py
--rw-r--r--   0 max        (502) staff       (20)      438 2014-05-16 11:58:11.000000 django-orderable-6.1.1/orderable/tests/test_admin.py
--rw-r--r--   0 max        (502) staff       (20)     1893 2019-03-06 11:37:02.000000 django-orderable-6.1.1/orderable/tests/test_manager.py
--rw-r--r--   0 max        (502) staff       (20)     9767 2020-06-19 17:08:42.000000 django-orderable-6.1.1/orderable/tests/test_models.py
--rw-r--r--   0 max        (502) staff       (20)     2784 2019-03-06 11:37:02.000000 django-orderable-6.1.1/orderable/tests/test_querysets.py
--rw-r--r--   0 max        (502) staff       (20)      195 2020-10-23 14:25:31.000000 django-orderable-6.1.1/setup.cfg
--rw-r--r--   0 max        (502) staff       (20)     1056 2020-10-23 14:23:52.000000 django-orderable-6.1.1/setup.py
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/
+-rw-r--r--   0 max        (502) staff       (20)       76 2012-10-06 17:28:33.000000 django-orderable-6.1.2/MANIFEST.in
+-rw-r--r--   0 max        (502) staff       (20)     4269 2023-06-29 19:28:25.000000 django-orderable-6.1.2/PKG-INFO
+-rw-r--r--   0 max        (502) staff       (20)     2598 2020-06-20 12:06:11.000000 django-orderable-6.1.2/README.md
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/django_orderable.egg-info/
+-rw-r--r--   0 max        (502) staff       (20)     4269 2023-06-29 19:28:25.000000 django-orderable-6.1.2/django_orderable.egg-info/PKG-INFO
+-rw-r--r--   0 max        (502) staff       (20)      667 2023-06-29 19:28:25.000000 django-orderable-6.1.2/django_orderable.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (502) staff       (20)        1 2023-06-29 19:28:25.000000 django-orderable-6.1.2/django_orderable.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (502) staff       (20)       10 2023-06-29 19:28:25.000000 django-orderable-6.1.2/django_orderable.egg-info/top_level.txt
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/
+-rw-r--r--   0 max        (502) staff       (20)        0 2014-05-16 11:58:11.000000 django-orderable-6.1.2/orderable/__init__.py
+-rw-r--r--   0 max        (502) staff       (20)     2325 2023-06-29 19:25:00.000000 django-orderable-6.1.2/orderable/admin.py
+-rw-r--r--   0 max        (502) staff       (20)      344 2019-03-06 11:37:02.000000 django-orderable-6.1.2/orderable/managers.py
+-rw-r--r--   0 max        (502) staff       (20)     6710 2020-10-23 14:16:39.000000 django-orderable-6.1.2/orderable/models.py
+-rw-r--r--   0 max        (502) staff       (20)     2885 2019-03-06 11:37:02.000000 django-orderable-6.1.2/orderable/querysets.py
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/static/
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/static/admin/
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/static/admin/img/
+-rw-r--r--   0 max        (502) staff       (20)       76 2012-10-06 17:28:33.000000 django-orderable-6.1.2/orderable/static/admin/img/drag_handle.gif
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/templates/
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/templates/admin/
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/templates/admin/edit_inline/
+-rw-r--r--   0 max        (502) staff       (20)     2709 2020-06-19 17:08:42.000000 django-orderable-6.1.2/orderable/templates/admin/edit_inline/orderable_tabular.html
+-rw-r--r--   0 max        (502) staff       (20)     2844 2020-10-23 14:16:39.000000 django-orderable-6.1.2/orderable/templates/admin/orderable_change_list.html
+drwxr-xr-x   0 max        (502) staff       (20)        0 2023-06-29 19:28:25.000000 django-orderable-6.1.2/orderable/tests/
+-rw-r--r--   0 max        (502) staff       (20)        0 2014-05-16 11:58:11.000000 django-orderable-6.1.2/orderable/tests/__init__.py
+-rw-r--r--   0 max        (502) staff       (20)      478 2019-03-07 15:37:23.000000 django-orderable-6.1.2/orderable/tests/models.py
+-rw-r--r--   0 max        (502) staff       (20)     2104 2019-03-07 08:41:14.000000 django-orderable-6.1.2/orderable/tests/run.py
+-rw-r--r--   0 max        (502) staff       (20)      438 2014-05-16 11:58:11.000000 django-orderable-6.1.2/orderable/tests/test_admin.py
+-rw-r--r--   0 max        (502) staff       (20)     1893 2019-03-06 11:37:02.000000 django-orderable-6.1.2/orderable/tests/test_manager.py
+-rw-r--r--   0 max        (502) staff       (20)     9767 2020-06-19 17:08:42.000000 django-orderable-6.1.2/orderable/tests/test_models.py
+-rw-r--r--   0 max        (502) staff       (20)     2784 2019-03-06 11:37:02.000000 django-orderable-6.1.2/orderable/tests/test_querysets.py
+-rw-r--r--   0 max        (502) staff       (20)      195 2023-06-29 19:28:25.000000 django-orderable-6.1.2/setup.cfg
+-rw-r--r--   0 max        (502) staff       (20)     1056 2023-06-29 19:27:33.000000 django-orderable-6.1.2/setup.py
```

### Comparing `django-orderable-6.1.1/PKG-INFO` & `django-orderable-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-orderable
-Version: 6.1.1
+Version: 6.1.2
 Summary: Add manual sort order to Django objects via an abstract base class and admin classes.
 Home-page: https://github.com/incuna/django-orderable
 Author: Incuna Ltd
 Author-email: admin@incuna.com
 License: BSD
 Description: # Django Orderable
```

### Comparing `django-orderable-6.1.1/README.md` & `django-orderable-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/django_orderable.egg-info/PKG-INFO` & `django-orderable-6.1.2/django_orderable.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-orderable
-Version: 6.1.1
+Version: 6.1.2
 Summary: Add manual sort order to Django objects via an abstract base class and admin classes.
 Home-page: https://github.com/incuna/django-orderable
 Author: Incuna Ltd
 Author-email: admin@incuna.com
 License: BSD
 Description: # Django Orderable
```

### Comparing `django-orderable-6.1.1/django_orderable.egg-info/SOURCES.txt` & `django-orderable-6.1.2/django_orderable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/admin.py` & `django-orderable-6.1.2/orderable/admin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib import admin
 from django.core.exceptions import PermissionDenied
 from django.http import HttpResponse
+from django.urls import path
 from django.utils.decorators import method_decorator
 from django.views.decorators.csrf import csrf_protect
 
 
 csrf_protect_m = method_decorator(csrf_protect)
 
 
@@ -16,26 +17,21 @@
     want to add sort_order_display to list_display.
     """
     list_display = ('__str__', 'sort_order_display')
 
     change_list_template = "admin/orderable_change_list.html"
 
     def get_urls(self):
-        try:
-            from django.conf.urls.defaults import url
-        except ImportError:
-            from django.conf.urls import url
-
         patterns = super(OrderableAdmin, self).get_urls()
         patterns.insert(
             # insert just before (.+) rule
             # (see django.contrib.admin.options.ModelAdmin.get_urls)
             -1,
-            url(
-                r'^reorder/$',
+            path(
+                'reorder/',
                 self.reorder_view,
                 name=self.get_url_name()
             )
         )
         return patterns
 
     def get_url_name(self):
```

### Comparing `django-orderable-6.1.1/orderable/models.py` & `django-orderable-6.1.2/orderable/models.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/querysets.py` & `django-orderable-6.1.2/orderable/querysets.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/templates/admin/edit_inline/orderable_tabular.html` & `django-orderable-6.1.2/orderable/templates/admin/edit_inline/orderable_tabular.html`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/templates/admin/orderable_change_list.html` & `django-orderable-6.1.2/orderable/templates/admin/orderable_change_list.html`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/tests/run.py` & `django-orderable-6.1.2/orderable/tests/run.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/tests/test_manager.py` & `django-orderable-6.1.2/orderable/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/tests/test_models.py` & `django-orderable-6.1.2/orderable/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/orderable/tests/test_querysets.py` & `django-orderable-6.1.2/orderable/tests/test_querysets.py`

 * *Files identical despite different names*

### Comparing `django-orderable-6.1.1/setup.py` & `django-orderable-6.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 
 setup(
     name='django-orderable',
     packages=find_packages(),
     include_package_data=True,
-    version='6.1.1',
+    version='6.1.2',
     description='Add manual sort order to Django objects via an abstract base '
                 'class and admin classes.',
     author='Incuna Ltd',
     author_email='admin@incuna.com',
     url='https://github.com/incuna/django-orderable',
     long_description_content_type='text/markdown',
     long_description=open('README.md').read(),
```

