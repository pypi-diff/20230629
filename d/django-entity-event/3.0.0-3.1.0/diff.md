# Comparing `tmp/django-entity-event-3.0.0.tar.gz` & `tmp/django-entity-event-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-entity-event-3.0.0.tar", last modified: Wed Jan 25 13:26:14 2023, max compression
+gzip compressed data, was "django-entity-event-3.1.0.tar", last modified: Thu Jun 29 16:21:54 2023, max compression
```

## Comparing `django-entity-event-3.0.0.tar` & `django-entity-event-3.1.0.tar`

### file list

```diff
@@ -1,44 +1,40 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       68 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     2218 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1311 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/README.rst
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/django_entity_event.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2218 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1185 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/not-zip-safe
--rw-rw-r--   0 wes       (1000) wes       (1000)       66 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       13 2023-01-25 13:26:14.000000 django-entity-event-3.0.0/django_entity_event.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/entity_event/
--rw-rw-r--   0 wes       (1000) wes       (1000)      109 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2909 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/admin.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      139 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     9384 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/context_loader.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3864 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/context_serializer.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/entity_event/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     8617 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      568 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/0002_medium_creation_time.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      469 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/0003_auto_20170830_1321.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1126 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/0004_auto_20180403_1655.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1750 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/0005_auto_20200409_1612.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    56822 2023-01-25 13:25:57.000000 django-entity-event-3.0.0/entity_event/models.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/entity_event/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      877 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/admin_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    30529 2023-01-25 13:25:57.000000 django-entity-event-3.0.0/entity_event/tests/context_loader_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     7091 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/context_serializer_tests.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/entity_event/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1627 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    40244 2023-01-24 21:40:16.000000 django-entity-event-3.0.0/entity_event/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      610 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/entity_event/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-01-25 13:25:57.000000 django-entity-event-3.0.0/entity_event/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       31 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/requirements/docs.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       75 2023-01-25 13:25:57.000000 django-entity-event-3.0.0/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       66 2021-04-06 17:21:24.000000 django-entity-event-3.0.0/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      276 2023-01-25 13:26:14.661713 django-entity-event-3.0.0/setup.cfg
--rwxrwxr-x   0 wes       (1000) wes       (1000)     1954 2023-01-25 13:25:57.000000 django-entity-event-3.0.0/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       68 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2140 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1311 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/django_entity_event.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2140 2023-06-29 16:21:54.000000 django-entity-event-3.1.0/django_entity_event.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      985 2023-06-29 16:21:54.000000 django-entity-event-3.1.0/django_entity_event.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 16:21:54.000000 django-entity-event-3.1.0/django_entity_event.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-25 13:26:14.000000 django-entity-event-3.1.0/django_entity_event.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       44 2023-06-29 16:21:54.000000 django-entity-event-3.1.0/django_entity_event.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       13 2023-06-29 16:21:54.000000 django-entity-event-3.1.0/django_entity_event.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/entity_event/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2909 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/admin.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      139 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     9226 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/context_loader.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3840 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/context_serializer.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/entity_event/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     8963 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/migrations/0001_0005_squashed.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    56808 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/entity_event/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      877 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/tests/admin_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    30473 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/tests/context_loader_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7100 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/tests/context_serializer_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/entity_event/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1587 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    40241 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      610 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/entity_event/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/entity_event/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2021-04-06 17:21:24.000000 django-entity-event-3.1.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       75 2023-01-25 13:25:57.000000 django-entity-event-3.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       44 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      276 2023-06-29 16:21:54.767369 django-entity-event-3.1.0/setup.cfg
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1878 2023-06-29 16:21:06.000000 django-entity-event-3.1.0/setup.py
```

### Comparing `django-entity-event-3.0.0/LICENSE` & `django-entity-event-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-entity-event-3.0.0/PKG-INFO` & `django-entity-event-3.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: django-entity-event
-Version: 3.0.0
+Version: 3.1.0
 Summary: Newsfeed-style event tracking and subscription management for django-entity.
 Home-page: https://github.com/ambitioninc/django-entity-event
 Author: Erik Swanson
 Author-email: opensource@ambition.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 .. image:: https://travis-ci.org/ambitioninc/django-entity-event.png
    :target: https://travis-ci.org/ambitioninc/django-entity-event
 
 .. image:: https://pypip.in/v/django-entity-event/badge.png
     :target: https://crate.io/packages/django-entity-event/
```

### Comparing `django-entity-event-3.0.0/README.rst` & `django-entity-event-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-entity-event-3.0.0/django_entity_event.egg-info/PKG-INFO` & `django-entity-event-3.1.0/django_entity_event.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: django-entity-event
-Version: 3.0.0
+Version: 3.1.0
 Summary: Newsfeed-style event tracking and subscription management for django-entity.
 Home-page: https://github.com/ambitioninc/django-entity-event
 Author: Erik Swanson
 Author-email: opensource@ambition.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 License-File: LICENSE
 
 .. image:: https://travis-ci.org/ambitioninc/django-entity-event.png
    :target: https://travis-ci.org/ambitioninc/django-entity-event
 
 .. image:: https://pypip.in/v/django-entity-event/badge.png
     :target: https://crate.io/packages/django-entity-event/
```

### Comparing `django-entity-event-3.0.0/django_entity_event.egg-info/SOURCES.txt` & `django-entity-event-3.1.0/django_entity_event.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,19 +13,15 @@
 entity_event/admin.py
 entity_event/apps.py
 entity_event/context_loader.py
 entity_event/context_serializer.py
 entity_event/models.py
 entity_event/urls.py
 entity_event/version.py
-entity_event/migrations/0001_initial.py
-entity_event/migrations/0002_medium_creation_time.py
-entity_event/migrations/0003_auto_20170830_1321.py
-entity_event/migrations/0004_auto_20180403_1655.py
-entity_event/migrations/0005_auto_20200409_1612.py
+entity_event/migrations/0001_0005_squashed.py
 entity_event/migrations/__init__.py
 entity_event/tests/__init__.py
 entity_event/tests/admin_tests.py
 entity_event/tests/context_loader_tests.py
 entity_event/tests/context_serializer_tests.py
 entity_event/tests/model_tests.py
 entity_event/tests/models.py
```

### Comparing `django-entity-event-3.0.0/entity_event/admin.py` & `django-entity-event-3.1.0/entity_event/admin.py`

 * *Files identical despite different names*

### Comparing `django-entity-event-3.0.0/entity_event/context_loader.py` & `django-entity-event-3.1.0/entity_event/context_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """
 A module for loading contexts using context hints.
 """
 from collections import defaultdict
-import six
 
 from django.conf import settings
 from django.db.models import Q
-try:
-    # Django 1.9
-    from django.apps import apps
-    get_model = apps.get_model
-except ImportError:  # pragma: no cover
-    # Django < 1.9
-    from django.db.models import get_model
+from django.apps import apps
+get_model = apps.get_model
 from manager_utils import id_dict
 
 from entity_event.models import ContextRenderer
 
 
 def get_context_hints_per_source(context_renderers):
     """
@@ -100,15 +94,15 @@
     point to sets of ids that need to be fetched. Return output is as follows:
 
     {
         model: [id1, id2, ...],
         ...
     }
     """
-    number_types = (complex, float) + six.integer_types
+    number_types = (complex, float, int)
     model_ids_to_fetch = defaultdict(set)
 
     for event in events:
         context_hints = context_hints_per_source.get(event.source, {})
         for context_key, hints in context_hints.items():
             for d, value in dict_find(event.context, context_key):
                 values = value if isinstance(value, list) else [value]
```

### Comparing `django-entity-event-3.0.0/entity_event/context_serializer.py` & `django-entity-event-3.1.0/entity_event/context_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from django.db import models
 from django.forms import model_to_dict
-import six
 
 
 class DefaultContextSerializer(object):
     """
     Default class for serializing context data
     """
 
@@ -82,15 +81,15 @@
         """
         Tries to load an encoded json string back into an object
         :param json_string:
         :return:
         """
 
         # Check if the value might be a json string
-        if not isinstance(value, six.string_types):
+        if not isinstance(value, str):
             return value
 
         # Make sure it starts with a brace
         if not value.startswith('{') or value.startswith('['):
             return value
 
         # Try to load the string
```

### Comparing `django-entity-event-3.0.0/entity_event/migrations/0001_initial.py` & `django-entity-event-3.1.0/entity_event/migrations/0001_0005_squashed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,200 +1,188 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals
+# Generated by Django 3.2.19 on 2023-05-31 20:54
 
-from django.db import models, migrations
-import django.db.models.deletion
 import datetime
-import jsonfield.fields
+import django.core.serializers.json
+from django.db import migrations, models
+import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
+    replaces = [('entity_event', '0001_initial'), ('entity_event', '0002_medium_creation_time'),
+                ('entity_event', '0003_auto_20170830_1321'), ('entity_event', '0004_auto_20180403_1655'),
+                ('entity_event', '0005_auto_20200409_1612')]
 
     dependencies = [
         ('entity', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
-            name='ContextRenderer',
-            fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('name', models.CharField(max_length=64, unique=True)),
-                ('text_template_path', models.CharField(max_length=256, default='')),
-                ('html_template_path', models.CharField(max_length=256, default='')),
-                ('text_template', models.TextField(default='')),
-                ('html_template', models.TextField(default='')),
-                ('context_hints', jsonfield.fields.JSONField(null=True, default=None)),
-            ],
-            options={
-            },
-            bases=(models.Model,),
-        ),
-        migrations.CreateModel(
             name='Event',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('context', jsonfield.fields.JSONField()),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('context', models.JSONField()),
                 ('time', models.DateTimeField(auto_now_add=True, db_index=True)),
                 ('time_expires', models.DateTimeField(db_index=True, default=datetime.datetime(9999, 12, 31, 23, 59, 59, 999999))),
                 ('uuid', models.CharField(max_length=128, unique=True)),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='EventActor',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity.Entity')),
-                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Event')),
-            ],
-            options={
-            },
-            bases=(models.Model,),
-        ),
-        migrations.CreateModel(
-            name='EventSeen',
-            fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('time_seen', models.DateTimeField(default=datetime.datetime.utcnow)),
-                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Event')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity.entity')),
+                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.event')),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='Medium',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=64, unique=True)),
                 ('display_name', models.CharField(max_length=64)),
                 ('description', models.TextField()),
-                ('additional_context', jsonfield.fields.JSONField(null=True, default=None)),
+                ('additional_context', models.JSONField(default=None, null=True)),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='RenderingStyle',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('name', models.CharField(max_length=64, unique=True)),
-                ('display_name', models.CharField(max_length=64, default='')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=256, unique=True)),
+                ('display_name', models.CharField(default='', max_length=256)),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='Source',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=64, unique=True)),
                 ('display_name', models.CharField(max_length=64)),
                 ('description', models.TextField()),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='SourceGroup',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('name', models.CharField(max_length=64, unique=True)),
-                ('display_name', models.CharField(max_length=64)),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=256, unique=True)),
+                ('display_name', models.CharField(max_length=256)),
                 ('description', models.TextField()),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='Subscription',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('only_following', models.BooleanField(default=True)),
-                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='+', to='entity.Entity')),
-                ('medium', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Medium')),
-                ('source', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Source')),
-                ('sub_entity_kind', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, null=True, related_name='+', to='entity.EntityKind', default=None)),
+                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='+', to='entity.entity')),
+                ('medium', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.medium')),
+                ('source', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.source')),
+                ('sub_entity_kind', models.ForeignKey(default=None, null=True, on_delete=django.db.models.deletion.CASCADE, related_name='+', to='entity.entitykind')),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='Unsubscription',
             fields=[
-                ('id', models.AutoField(serialize=False, primary_key=True, auto_created=True, verbose_name='ID')),
-                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity.Entity')),
-                ('medium', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Medium')),
-                ('source', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Source')),
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('entity', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity.entity')),
+                ('medium', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.medium')),
+                ('source', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.source')),
             ],
-            options={
-            },
-            bases=(models.Model,),
         ),
         migrations.AddField(
             model_name='source',
             name='group',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.SourceGroup'),
-            preserve_default=True,
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.sourcegroup'),
         ),
         migrations.AddField(
             model_name='medium',
             name='rendering_style',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.RenderingStyle', null=True),
-            preserve_default=True,
+            field=models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='entity_event.renderingstyle'),
         ),
-        migrations.AddField(
-            model_name='eventseen',
-            name='medium',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Medium'),
-            preserve_default=True,
-        ),
-        migrations.AlterUniqueTogether(
-            name='eventseen',
-            unique_together=set([('event', 'medium')]),
+        migrations.CreateModel(
+            name='EventSeen',
+            fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('time_seen', models.DateTimeField(default=datetime.datetime.utcnow)),
+                ('event', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.event')),
+                ('medium', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.medium')),
+            ],
+            options={
+                'unique_together': {('event', 'medium')},
+            },
         ),
         migrations.AddField(
             model_name='event',
             name='source',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Source'),
-            preserve_default=True,
+            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.source'),
         ),
-        migrations.AddField(
-            model_name='contextrenderer',
-            name='rendering_style',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.RenderingStyle'),
-            preserve_default=True,
+        migrations.CreateModel(
+            name='AdminEvent',
+            fields=[
+            ],
+            options={
+                'proxy': True,
+            },
+            bases=('entity_event.event',),
         ),
         migrations.AddField(
-            model_name='contextrenderer',
-            name='source',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.Source', null=True),
-            preserve_default=True,
+            model_name='medium',
+            name='time_created',
+            field=models.DateTimeField(auto_now_add=True, default=datetime.datetime(2017, 5, 24, 18, 7, 45, 987701)),
+            preserve_default=False,
         ),
-        migrations.AddField(
-            model_name='contextrenderer',
-            name='source_group',
-            field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.SourceGroup', null=True),
-            preserve_default=True,
-        ),
-        migrations.AlterUniqueTogether(
-            name='contextrenderer',
-            unique_together=set([('source', 'rendering_style')]),
+        migrations.AlterField(
+            model_name='event',
+            name='uuid',
+            field=models.CharField(max_length=512, unique=True),
+        ),
+        migrations.AlterField(
+            model_name='event',
+            name='context',
+            field=models.JSONField(encoder=django.core.serializers.json.DjangoJSONEncoder),
+        ),
+        migrations.AlterField(
+            model_name='medium',
+            name='additional_context',
+            field=models.JSONField(default=None, encoder=django.core.serializers.json.DjangoJSONEncoder, null=True),
         ),
         migrations.CreateModel(
-            name='AdminEvent',
+            name='ContextRenderer',
             fields=[
+                ('id', models.AutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('name', models.CharField(max_length=256, unique=True)),
+                ('text_template_path', models.CharField(default='', max_length=256)),
+                ('html_template_path', models.CharField(default='', max_length=256)),
+                ('text_template', models.TextField(default='')),
+                ('html_template', models.TextField(default='')),
+                ('context_hints', models.JSONField(default=None, encoder=django.core.serializers.json.DjangoJSONEncoder, null=True)),
+                ('rendering_style', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='entity_event.renderingstyle')),
+                ('source', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='entity_event.source')),
+                ('source_group', models.ForeignKey(null=True, on_delete=django.db.models.deletion.CASCADE, to='entity_event.sourcegroup')),
             ],
             options={
-                'proxy': True,
+                'unique_together': {('source', 'rendering_style')},
             },
-            bases=('entity_event.event',),
+        ),
+        migrations.AlterField(
+            model_name='medium',
+            name='display_name',
+            field=models.CharField(max_length=256),
+        ),
+        migrations.AlterField(
+            model_name='medium',
+            name='name',
+            field=models.CharField(max_length=256, unique=True),
+        ),
+        migrations.AlterField(
+            model_name='source',
+            name='display_name',
+            field=models.CharField(max_length=256),
+        ),
+        migrations.AlterField(
+            model_name='source',
+            name='name',
+            field=models.CharField(max_length=256, unique=True),
         ),
     ]
```

### Comparing `django-entity-event-3.0.0/entity_event/models.py` & `django-entity-event-3.1.0/entity_event/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections import defaultdict
 from datetime import datetime
 from operator import or_
-from six.moves import reduce
+from functools import reduce
 
 from cached_property import cached_property
-from django.contrib.postgres.fields import JSONField
+from django.db.models import JSONField
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models, transaction
 from django.db.models import Q
 from django.db.models.query import QuerySet
 from django.template.loader import render_to_string
 from django.template import Context, Template
 from entity.models import Entity, EntityRelationship
```

### Comparing `django-entity-event-3.0.0/entity_event/tests/admin_tests.py` & `django-entity-event-3.1.0/entity_event/tests/admin_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-event-3.0.0/entity_event/tests/context_loader_tests.py` & `django-entity-event-3.1.0/entity_event/tests/context_loader_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from django import VERSION
 from django.test import TestCase
 from django.test.utils import override_settings
 from django_dynamic_fixture import N, G
-from mock import patch
+from unittest.mock import patch
 
 from entity_event import context_loader
 from entity_event import models
 from entity_event.tests import models as test_models
 
 
 class TestGetDefaultRenderingStyle(TestCase):
     def test_none_defined(self):
         self.assertIsNone(context_loader.get_default_rendering_style())
 
     @override_settings(DEFAULT_ENTITY_EVENT_RENDERING_STYLE='short')
     def test_defined(self):
         rs = G(models.RenderingStyle, name='short')
-        self.assertEquals(context_loader.get_default_rendering_style(), rs)
+        self.assertEqual(context_loader.get_default_rendering_style(), rs)
 
 
 class TestGetContextHintsFromSource(TestCase):
     def test_no_context_renderers(self):
         res = context_loader.get_context_hints_per_source([])
-        self.assertEquals(res, {})
+        self.assertEqual(res, {})
 
     @patch.object(models.ContextRenderer, 'get_sources', spec_set=True)
     def test_one_context_renderer(self, mock_get_sources):
         source = N(models.Source, id=1)
         mock_get_sources.return_value = [source]
         res = context_loader.get_context_hints_per_source([
             N(models.ContextRenderer, source=source, context_hints={
                 'key': {
                     'app_name': 'entity_event.tests',
                     'model_name': 'TestModel',
                     'select_related': ['fk'],
                 },
             })
         ])
-        self.assertEquals(res, {
+        self.assertEqual(res, {
             source: {
                 'key': {
                     'app_name': 'entity_event.tests',
                     'model_name': 'TestModel',
                     'select_related': set(['fk']),
                     'prefetch_related': set(),
                 }
@@ -73,15 +73,15 @@
                     'app_name': 'entity_event.tests2',
                     'model_name': 'TestModel2',
                     'select_related': ['fk2'],
                     'prefetch_related': ['prefetch5', 'prefetch6'],
                 },
             })
         ])
-        self.assertEquals(res, {
+        self.assertEqual(res, {
             source1: {
                 'key': {
                     'app_name': 'entity_event.tests',
                     'model_name': 'TestModel',
                     'select_related': set(['fk', 'fk1']),
                     'prefetch_related': set(['prefetch1', 'prefetch2', 'prefetch3']),
                 }
@@ -96,27 +96,27 @@
             },
         })
 
 
 class TestGetQuerysetsForContextHints(TestCase):
     def test_no_context_hints(self):
         qsets = context_loader.get_querysets_for_context_hints({})
-        self.assertEquals(qsets, {})
+        self.assertEqual(qsets, {})
 
     def test_one_context_hint_no_select_related(self):
         source = N(models.Source, id=1)
         qsets = context_loader.get_querysets_for_context_hints({
             source: {
                 'key': {
                     'app_name': 'tests',
                     'model_name': 'TestModel',
                 },
             },
         })
-        self.assertEquals(qsets, {
+        self.assertEqual(qsets, {
             test_models.TestModel: test_models.TestModel.objects
         })
 
     def test_one_context_hint_w_select_related(self):
         source = N(models.Source, id=1)
         qsets = context_loader.get_querysets_for_context_hints({
             source: {
@@ -135,15 +135,15 @@
             '"tests_testfkmodel" ON ("tests_testmodel"."fk_id" = "tests_testfkmodel"."id")'
         )
         actual_sql = str(qsets[test_models.TestModel].query)
 
         # Django < 1.7 and 1.8 have spaces before/after parentheses
         actual_sql = actual_sql.replace('( ', '(').replace(' )', ')')
 
-        self.assertEquals(actual_sql, expected_sql)
+        self.assertEqual(actual_sql, expected_sql)
 
     def test_multiple_context_hints_w_multiple_select_related(self):
         source = N(models.Source, id=1)
         source2 = N(models.Source, id=2)
         qsets = context_loader.get_querysets_for_context_hints({
             source: {
                 'key': {
@@ -171,15 +171,15 @@
         )
 
         actual_sql = str(qsets[test_models.TestModel].query)
 
         # Django < 1.7 and 1.8 have spaces before/after parentheses
         actual_sql = actual_sql.replace('( ', '(').replace(' )', ')')
 
-        self.assertEquals(actual_sql, expected_sql)
+        self.assertEqual(actual_sql, expected_sql)
 
     def test_multiple_context_hints_w_multiple_select_related_multiple_prefetch_related(self):
         source = N(models.Source, id=1)
         source2 = N(models.Source, id=2)
         qsets = context_loader.get_querysets_for_context_hints({
             source: {
                 'key': {
@@ -210,15 +210,15 @@
         )
 
         actual_sql = str(qsets[test_models.TestModel].query)
 
         # Django < 1.7 and 1.8 have spaces before/after parentheses
         actual_sql = actual_sql.replace('( ', '(').replace(' )', ')')
 
-        self.assertEquals(actual_sql, expected_sql)
+        self.assertEqual(actual_sql, expected_sql)
 
 
 class TestGetQuerysetsForContextHintsDbTests(TestCase):
     def test_multiple_context_hints_w_multiple_select_related_multiple_prefetch_related(self):
         source = N(models.Source, id=1)
         source2 = N(models.Source, id=2)
         qsets = context_loader.get_querysets_for_context_hints({
@@ -244,98 +244,98 @@
         fk2 = G(test_models.TestFKModel2)
         o = G(test_models.TestModel, fk=fk, fk2=fk2)
         m2ms = [G(test_models.TestFKModel), G(test_models.TestFKModel)]
         o.fk_m2m.add(*m2ms)
 
         with self.assertNumQueries(2):
             v = qsets[test_models.TestModel].get(id=o.id)
-            self.assertEquals(v.fk, fk)
-            self.assertEquals(v.fk2, fk2)
-            self.assertEquals(set(v.fk_m2m.all()), set(m2ms))
+            self.assertEqual(v.fk, fk)
+            self.assertEqual(v.fk2, fk2)
+            self.assertEqual(set(v.fk_m2m.all()), set(m2ms))
 
 
 class DictFindTest(TestCase):
     def test_dict_find_none(self):
-        self.assertEquals(list(context_loader.dict_find({}, 'key')), [])
+        self.assertEqual(list(context_loader.dict_find({}, 'key')), [])
 
     def test_dict_find_list_key(self):
         d = {'key': ['value']}
-        self.assertEquals(list(context_loader.dict_find(d, 'key')), [(d, ['value'])])
+        self.assertEqual(list(context_loader.dict_find(d, 'key')), [(d, ['value'])])
 
     def test_dict_find_nested_list_key(self):
         d = {'key': ['value']}
         larger_dict = {
             'l': [{
                 'hi': {},
             }, {
                 'hi2': d
             }]
         }
-        self.assertEquals(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value'])])
+        self.assertEqual(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value'])])
 
     def test_dict_find_double_nested_list_key(self):
         d = {'key': ['value']}
         larger_dict = {
             'l': [{
                 'hi': {},
             }, {
                 'hi2': d
             }],
             'hi3': d
         }
-        self.assertEquals(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value']), (d, ['value'])])
+        self.assertEqual(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value']), (d, ['value'])])
 
     def test_dict_find_deep_nested_list_key(self):
         d = {'key': ['value']}
         larger_dict = [[{
             'l': [{
                 'hi': {},
             }, {
                 'hi2': d
             }],
             'hi3': d
         }]]
-        self.assertEquals(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value']), (d, ['value'])])
+        self.assertEqual(list(context_loader.dict_find(larger_dict, 'key')), [(d, ['value']), (d, ['value'])])
 
 
 class GetModelIdsToFetchTest(TestCase):
     def test_no_events(self):
-        self.assertEquals(context_loader.get_model_ids_to_fetch([], {}), {})
+        self.assertEqual(context_loader.get_model_ids_to_fetch([], {}), {})
 
     def test_no_context_hints(self):
         e = N(models.Event, id=1, context={})
-        self.assertEquals(context_loader.get_model_ids_to_fetch([e], {}), {})
+        self.assertEqual(context_loader.get_model_ids_to_fetch([e], {}), {})
 
     def test_w_one_event_one_context_hint_single_pk(self):
         source = N(models.Source, id=1)
         hints = {
             source: {
                 'key': {
                     'app_name': 'tests',
                     'model_name': 'TestModel',
                 },
             },
         }
         e = N(models.Event, context={'key': 2}, source=source)
-        self.assertEquals(context_loader.get_model_ids_to_fetch([e], hints), {
+        self.assertEqual(context_loader.get_model_ids_to_fetch([e], hints), {
             test_models.TestModel: set([2])
         })
 
     def test_w_one_event_one_context_hint_list_pks(self):
         source = N(models.Source, id=1)
         hints = {
             source: {
                 'key': {
                     'app_name': 'tests',
                     'model_name': 'TestModel',
                 },
             },
         }
         e = N(models.Event, context={'key': [2, 3, 5]}, source=source)
-        self.assertEquals(context_loader.get_model_ids_to_fetch([e], hints), {
+        self.assertEqual(context_loader.get_model_ids_to_fetch([e], hints), {
             test_models.TestModel: set([2, 3, 5])
         })
 
     def test_w_multiple_events_one_context_hint_list_pks(self):
         source = N(models.Source, id=1)
         hints = {
             source: {
@@ -343,15 +343,15 @@
                     'app_name': 'tests',
                     'model_name': 'TestModel',
                 },
             },
         }
         e1 = N(models.Event, context={'key': [2, 3, 5]}, source=source)
         e2 = N(models.Event, context={'key': 88}, source=source)
-        self.assertEquals(context_loader.get_model_ids_to_fetch([e1, e2], hints), {
+        self.assertEqual(context_loader.get_model_ids_to_fetch([e1, e2], hints), {
             test_models.TestModel: set([2, 3, 5, 88])
         })
 
     def test_w_multiple_events_multiple_context_hints_list_pks(self):
         source1 = N(models.Source, id=1)
         source2 = N(models.Source, id=2)
         hints = {
@@ -372,39 +372,39 @@
                 },
             },
         }
         e1 = N(models.Event, context={'key': [2, 3, 5]}, source=source1)
         e2 = N(models.Event, context={'key': 88}, source=source1)
         e3 = N(models.Event, context={'key': 100, 'key2': [50]}, source=source2)
         e4 = N(models.Event, context={'key2': [60]}, source=source2)
-        self.assertEquals(context_loader.get_model_ids_to_fetch([e1, e2, e3, e4], hints), {
+        self.assertEqual(context_loader.get_model_ids_to_fetch([e1, e2, e3, e4], hints), {
             test_models.TestModel: set([2, 3, 5, 88, 100]),
             test_models.TestFKModel: set([50, 60])
         })
 
 
 class FetchModelDataTest(TestCase):
     def test_none(self):
-        self.assertEquals({}, context_loader.fetch_model_data({}, {}))
+        self.assertEqual({}, context_loader.fetch_model_data({}, {}))
 
     def test_one_model_one_id_to_fetch(self):
         m1 = G(test_models.TestModel)
-        self.assertEquals({
+        self.assertEqual({
             test_models.TestModel: {m1.id: m1}
         }, context_loader.fetch_model_data({
             test_models.TestModel: test_models.TestModel.objects
         }, {
             test_models.TestModel: [m1.id]
         }))
 
     def test_multiple_models_multiple_ids_to_fetch(self):
         m1 = G(test_models.TestModel)
         m2 = G(test_models.TestModel)
         m3 = G(test_models.TestFKModel)
-        self.assertEquals({
+        self.assertEqual({
             test_models.TestModel: {m1.id: m1, m2.id: m2},
             test_models.TestFKModel: {m3.id: m3}
         }, context_loader.fetch_model_data({
             test_models.TestModel: test_models.TestModel.objects,
             test_models.TestFKModel: test_models.TestFKModel.objects,
         }, {
             test_models.TestModel: [m1.id, m2.id],
@@ -415,30 +415,30 @@
 class LoadFetchedObjectsIntoContextsTest(TestCase):
     def test_none(self):
         context_loader.load_fetched_objects_into_contexts([], {}, {})
 
     def test_event_with_no_model_data(self):
         e = N(models.Event, id=1, context={'hi', 'hi'})
         context_loader.load_fetched_objects_into_contexts([e], {}, {})
-        self.assertEquals(e, e)
+        self.assertEqual(e, e)
 
     def test_one_event_w_model_data(self):
         m = N(test_models.TestModel, id=2)
         s = N(models.Source, id=1)
         hints = {
             s: {
                 'key': {
                     'model_name': 'TestModel',
                     'app_name': 'tests',
                 }
             }
         }
         e = N(models.Event, context={'key': m.id}, source=s)
         context_loader.load_fetched_objects_into_contexts([e], {test_models.TestModel: {m.id: m}}, hints)
-        self.assertEquals(e.context, {'key': m})
+        self.assertEqual(e.context, {'key': m})
 
     def test_one_event_w_list_model_data(self):
         m1 = N(test_models.TestModel, id=2)
         m2 = N(test_models.TestModel, id=3)
         s = N(models.Source, id=1)
         hints = {
             s: {
@@ -446,28 +446,28 @@
                     'model_name': 'TestModel',
                     'app_name': 'tests',
                 }
             }
         }
         e = N(models.Event, context={'key': [m1.id, m2.id]}, source=s)
         context_loader.load_fetched_objects_into_contexts([e], {test_models.TestModel: {m1.id: m1, m2.id: m2}}, hints)
-        self.assertEquals(e.context, {'key': [m1, m2]})
+        self.assertEqual(e.context, {'key': [m1, m2]})
 
 
 class TestLoadRenderersIntoEvents(TestCase):
     def test_no_mediums_or_renderers(self):
         events = [N(models.Event, context={})]
         context_loader.load_renderers_into_events(events, [], [], None)
-        self.assertEquals(events[0]._context_renderers, {})
+        self.assertEqual(events[0]._context_renderers, {})
 
     def test_mediums_and_no_renderers(self):
         events = [N(models.Event, context={})]
         mediums = [N(models.Medium)]
         context_loader.load_renderers_into_events(events, mediums, [], None)
-        self.assertEquals(events[0]._context_renderers, {})
+        self.assertEqual(events[0]._context_renderers, {})
 
     def test_mediums_w_renderers(self):
         s1 = N(models.Source, id=1)
         s2 = N(models.Source, id=2)
         e1 = N(models.Event, context={}, source=s1)
         e2 = N(models.Event, context={}, source=s2)
         rg1 = N(models.RenderingStyle, id=1)
@@ -476,19 +476,19 @@
         m2 = N(models.Medium, id=2, rendering_style=rg2)
         cr1 = N(models.ContextRenderer, source=s1, rendering_style=rg1, id=1)
         cr2 = N(models.ContextRenderer, source=s2, rendering_style=rg1, id=2)
         cr3 = N(models.ContextRenderer, source=s1, rendering_style=rg2, id=3)
 
         context_loader.load_renderers_into_events([e1, e2], [m1, m2], [cr1, cr2, cr3], None)
 
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             m1: cr1,
             m2: cr3,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             m1: cr2
         })
 
     def test_mediums_w_source_group_renderers(self):
         s1 = N(models.Source, id=1, group=N(models.SourceGroup, id=1))
         s2 = N(models.Source, id=2, group=N(models.SourceGroup, id=1))
         e1 = N(models.Event, context={}, source=s1)
@@ -498,19 +498,19 @@
         m1 = N(models.Medium, id=1, rendering_style=rs1)
         m2 = N(models.Medium, id=2, rendering_style=rs2)
         cr1 = N(models.ContextRenderer, source_group=s1.group, rendering_style=rs1, id=1)
         cr2 = N(models.ContextRenderer, source_group=s1.group, rendering_style=rs2, id=2)
 
         context_loader.load_renderers_into_events([e1, e2], [m1, m2], [cr1, cr2], None)
 
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             m1: cr1,
             m2: cr2,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             m1: cr1,
             m2: cr2,
         })
 
     def test_mediums_w_source_group_renderers_default(self):
         s1 = N(models.Source, id=1, group=N(models.SourceGroup, id=1))
         s2 = N(models.Source, id=2, group=N(models.SourceGroup, id=1))
@@ -520,19 +520,19 @@
         rs2 = N(models.RenderingStyle, id=2)
         m1 = N(models.Medium, id=1, rendering_style=rs2)
         m2 = N(models.Medium, id=2, rendering_style=rs2)
         cr1 = N(models.ContextRenderer, source_group=s1.group, rendering_style=rs1, id=1)
 
         context_loader.load_renderers_into_events([e1, e2], [m1, m2], [cr1], rs1)
 
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             m1: cr1,
             m2: cr1,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             m1: cr1,
             m2: cr1,
         })
 
     def test_mediums_w_renderers_default_source(self):
         s1 = N(models.Source, id=1)
         s2 = N(models.Source, id=2)
@@ -546,19 +546,19 @@
         cr2 = N(models.ContextRenderer, source=s2, rendering_style=rs1, id=2)
         cr3 = N(models.ContextRenderer, source=s1, rendering_style=rs2, id=3)
 
         default_style = rs1
 
         context_loader.load_renderers_into_events([e1, e2], [m1, m2], [cr1, cr2, cr3], default_style)
 
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             m1: cr1,
             m2: cr1,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             m1: cr2,
             m2: cr2,
         })
 
 
 class LoadContextsAndRenderersTest(TestCase):
     """
@@ -566,15 +566,15 @@
     """
     def test_none(self):
         context_loader.load_contexts_and_renderers([], [])
 
     def test_no_mediums(self):
         e = G(models.Event, context={})
         context_loader.load_contexts_and_renderers([e], [])
-        self.assertEquals(e.context, {})
+        self.assertEqual(e.context, {})
 
     def test_one_render_target_one_event(self):
         m1 = G(test_models.TestModel)
         s = G(models.Source)
         rg = G(models.RenderingStyle)
         e = G(models.Event, context={'key': m1.id}, source=s)
         medium = G(models.Medium, rendering_style=rg)
@@ -582,15 +582,15 @@
             'key': {
                 'model_name': 'TestModel',
                 'app_name': 'tests',
             }
         })
 
         context_loader.load_contexts_and_renderers([e], [medium])
-        self.assertEquals(e.context, {'key': m1})
+        self.assertEqual(e.context, {'key': m1})
 
     @override_settings(DEFAULT_ENTITY_EVENT_RENDERING_STYLE='short')
     def test_one_render_target_one_event_no_style_with_default(self):
         m1 = G(test_models.TestModel)
         s = G(models.Source)
         rs = G(models.RenderingStyle, name='short')
         e = G(models.Event, context={'key': m1.id}, source=s)
@@ -599,15 +599,15 @@
             'key': {
                 'model_name': 'TestModel',
                 'app_name': 'tests',
             }
         })
 
         context_loader.load_contexts_and_renderers([e], [medium])
-        self.assertEquals(e.context, {'key': m1})
+        self.assertEqual(e.context, {'key': m1})
 
     def test_multiple_render_targets_multiple_events(self):
         test_m1 = G(test_models.TestModel)
         test_m2 = G(test_models.TestModel)
         test_m3 = G(test_models.TestModel)
         test_fk_m1 = G(test_models.TestFKModel)
         test_fk_m2 = G(test_models.TestFKModel)
@@ -637,30 +637,30 @@
 
         e1 = G(models.Event, context={'key': test_m1.id, 'key2': 'haha'}, source=s1)
         e2 = G(models.Event, context={'key': [test_m2.id, test_m3.id]}, source=s1)
         e3 = G(models.Event, context={'key2': test_fk_m1.id, 'key': test_m1.id}, source=s2)
         e4 = G(models.Event, context={'key2': test_fk_m2.id}, source=s2)
 
         context_loader.load_contexts_and_renderers([e1, e2, e3, e4], [medium1, medium2])
-        self.assertEquals(e1.context, {'key': test_m1, 'key2': 'haha'})
-        self.assertEquals(e2.context, {'key': [test_m2, test_m3]})
-        self.assertEquals(e3.context, {'key2': test_fk_m1, 'key': test_m1})
-        self.assertEquals(e4.context, {'key2': test_fk_m2})
+        self.assertEqual(e1.context, {'key': test_m1, 'key2': 'haha'})
+        self.assertEqual(e2.context, {'key': [test_m2, test_m3]})
+        self.assertEqual(e3.context, {'key2': test_fk_m1, 'key': test_m1})
+        self.assertEqual(e4.context, {'key2': test_fk_m2})
 
         # Verify context renderers are put into the events properly
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             medium1: cr1,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             medium1: cr1,
         })
-        self.assertEquals(e3._context_renderers, {
+        self.assertEqual(e3._context_renderers, {
             medium2: cr2,
         })
-        self.assertEquals(e4._context_renderers, {
+        self.assertEqual(e4._context_renderers, {
             medium2: cr2,
         })
 
     @override_settings(DEFAULT_ENTITY_EVENT_RENDERING_STYLE='short')
     def test_multiple_render_targets_multiple_events_use_default(self):
         """
         Tests the case when a context renderer is not available for a rendering style
@@ -697,33 +697,33 @@
 
         e1 = G(models.Event, context={'key': test_m1.id, 'key2': 'haha'}, source=s1)
         e2 = G(models.Event, context={'key': [test_m2.id, test_m3.id]}, source=s1)
         e3 = G(models.Event, context={'key2': test_fk_m1.id, 'key': test_m1.id}, source=s2)
         e4 = G(models.Event, context={'key2': test_fk_m2.id}, source=s2)
 
         context_loader.load_contexts_and_renderers([e1, e2, e3, e4], [medium1, medium2])
-        self.assertEquals(e1.context, {'key': test_m1, 'key2': 'haha'})
-        self.assertEquals(e2.context, {'key': [test_m2, test_m3]})
-        self.assertEquals(e3.context, {'key2': test_fk_m1, 'key': test_m1})
-        self.assertEquals(e4.context, {'key2': test_fk_m2})
+        self.assertEqual(e1.context, {'key': test_m1, 'key2': 'haha'})
+        self.assertEqual(e2.context, {'key': [test_m2, test_m3]})
+        self.assertEqual(e3.context, {'key2': test_fk_m1, 'key': test_m1})
+        self.assertEqual(e4.context, {'key2': test_fk_m2})
 
         # Verify context renderers are put into the events properly
-        self.assertEquals(e1._context_renderers, {
+        self.assertEqual(e1._context_renderers, {
             medium1: cr1,
             medium2: cr1,
         })
-        self.assertEquals(e2._context_renderers, {
+        self.assertEqual(e2._context_renderers, {
             medium1: cr1,
             medium2: cr1,
         })
-        self.assertEquals(e3._context_renderers, {
+        self.assertEqual(e3._context_renderers, {
             medium1: cr2,
             medium2: cr2,
         })
-        self.assertEquals(e4._context_renderers, {
+        self.assertEqual(e4._context_renderers, {
             medium1: cr2,
             medium2: cr2,
         })
 
     def test_optimal_queries(self):
         fk1 = G(test_models.TestFKModel)
         fk11 = G(test_models.TestFKModel)
@@ -773,14 +773,14 @@
         # WHERE "entity_event_sourcegroup"."id" IN (NULL)
         num_queries = 5
         if (VERSION[0] == 3 and VERSION[1] >= 2) or VERSION[0] >= 4:  # pragma: no cover
             num_queries = 4
 
         with self.assertNumQueries(num_queries):
             context_loader.load_contexts_and_renderers([e1, e2, e3, e4], [medium1, medium2])
-            self.assertEquals(e1.context['key'].fk, fk1)
-            self.assertEquals(e2.context['key'][0].fk, fk1)
-            self.assertEquals(e1.context['key'].fk2, fk2)
-            self.assertEquals(e2.context['key'][0].fk2, fk2)
-            self.assertEquals(set(e1.context['key'].fk_m2m.all()), set([fk1, fk11]))
-            self.assertEquals(set(e2.context['key'][0].fk_m2m.all()), set([fk1, fk11]))
-            self.assertEquals(e3.context['key'].fk, fk1)
+            self.assertEqual(e1.context['key'].fk, fk1)
+            self.assertEqual(e2.context['key'][0].fk, fk1)
+            self.assertEqual(e1.context['key'].fk2, fk2)
+            self.assertEqual(e2.context['key'][0].fk2, fk2)
+            self.assertEqual(set(e1.context['key'].fk_m2m.all()), set([fk1, fk11]))
+            self.assertEqual(set(e2.context['key'][0].fk_m2m.all()), set([fk1, fk11]))
+            self.assertEqual(e3.context['key'].fk, fk1)
```

### Comparing `django-entity-event-3.0.0/entity_event/tests/context_serializer_tests.py` & `django-entity-event-3.1.0/entity_event/tests/context_serializer_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from django.test.testcases import TransactionTestCase
 from django_dynamic_fixture import G
-from mock import patch, call
+from unittest.mock import patch, call
 
 from entity_event.context_serializer import DefaultContextSerializer
 from entity_event.tests.models import TestModel
 
 
 class DefaultContextSerializerTests(TransactionTestCase):
     def setUp(self):
```

### Comparing `django-entity-event-3.0.0/entity_event/tests/migrations/0001_initial.py` & `django-entity-event-3.1.0/entity_event/tests/migrations/0001_initial.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-entity-event-3.0.0/entity_event/tests/model_tests.py` & `django-entity-event-3.1.0/entity_event/tests/model_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 from django.template import Template
 from django.test import TestCase
 from django_dynamic_fixture import N, G
 from entity.models import Entity, EntityKind, EntityRelationship
 from freezegun import freeze_time
-from mock import patch, call, Mock
+from unittest.mock import patch, call, Mock
 from six import text_type
 
 from entity_event.models import (
     Medium, Source, SourceGroup, Unsubscription, Subscription, Event, EventActor, EventSeen,
     RenderingStyle, ContextRenderer, _unseen_event_ids, SubscriptionQuerySet,
     EventQuerySet, EventManager
 )
@@ -35,16 +35,16 @@
 
         fkm = G(TestFKModel, value=100)
         G(Event, source=s, context={'fk_model': fkm.id})
 
         events = Event.objects.all().load_contexts_and_renderers(m)
         txt, html = events[0].render(m)
 
-        self.assertEquals(txt, 'Test text template with value 100')
-        self.assertEquals(html, 'Test html template with value suppressed')
+        self.assertEqual(txt, 'Test text template with value 100')
+        self.assertEqual(html, 'Test html template with value suppressed')
 
     def test_one_context_renderer_one_medium(self):
         rg = G(RenderingStyle)
         s = G(Source)
         G(
             ContextRenderer, source=s, rendering_style=rg, text_template_path='test_template.txt',
             html_template_path='test_template.html', context_hints={
@@ -57,16 +57,16 @@
 
         fkm = G(TestFKModel, value=100)
         G(Event, source=s, context={'fk_model': fkm.id})
 
         events = Event.objects.all().load_contexts_and_renderers(m)
         txt, html = events[0].render(m)
 
-        self.assertEquals(txt, 'Test text template with value 100')
-        self.assertEquals(html, 'Test html template with value 100')
+        self.assertEqual(txt, 'Test text template with value 100')
+        self.assertEqual(html, 'Test html template with value 100')
 
     def test_wo_fetching_contexts(self):
         rg = G(RenderingStyle)
         s = G(Source)
         G(
             ContextRenderer, source=s, rendering_style=rg, text_template_path='test_template.txt',
             html_template_path='test_template.html', context_hints={
@@ -288,17 +288,17 @@
         self.assertTrue(EventSeen.objects.filter(event=event, medium=medium).exists())
 
     @patch('entity_event.context_loader.load_contexts_and_renderers', spec_set=True)
     def test_load_contexts_and_renderers(self, mock_load_contexts_and_renderers):
         e = G(Event, context={})
         medium = G(Medium)
         Event.objects.load_contexts_and_renderers(medium)
-        self.assertEquals(mock_load_contexts_and_renderers.call_count, 1)
-        self.assertEquals(list(mock_load_contexts_and_renderers.call_args_list[0][0][0]), [e])
-        self.assertEquals(mock_load_contexts_and_renderers.call_args_list[0][0][1], [medium])
+        self.assertEqual(mock_load_contexts_and_renderers.call_count, 1)
+        self.assertEqual(list(mock_load_contexts_and_renderers.call_args_list[0][0][0]), [e])
+        self.assertEqual(mock_load_contexts_and_renderers.call_args_list[0][0][1], [medium])
 
     @patch.object(EventManager, 'get_queryset', autospec=True)
     def test_cache_related(self, mock_get_queryset):
         # Setup some mock return values
         mock_get_queryset.return_value = Mock(EventQuerySet(), autospec=True)
 
         # Call the method
@@ -485,15 +485,15 @@
         e1 = Mock(render=Mock(return_value=('e1.txt', 'e1.html')))
         e2 = Mock(render=Mock(return_value=('e2.txt', 'e2.html')))
 
         events = [e1, e2]
         res = medium.render(events)
 
         mock_load_contexts_and_renderers.assert_called_once_with(events, [medium])
-        self.assertEquals(res, {
+        self.assertEqual(res, {
             e1: ('e1.txt', 'e1.html'),
             e2: ('e2.txt', 'e2.html'),
         })
         e1.render.assert_called_once_with(medium)
         e2.render.assert_called_once_with(medium)
 
 
@@ -537,25 +537,25 @@
 
     def test_get_unseen_events_some_seen_some_not(self):
         seen_e = G(Event, context={}, source=self.source)
         G(EventSeen, event=seen_e, medium=self.medium)
         unseen_e = G(Event, context={}, source=self.source)
 
         events = self.medium.get_filtered_events(seen=False)
-        self.assertEquals(list(events), [unseen_e])
+        self.assertEqual(list(events), [unseen_e])
 
     def test_get_unseen_events_some_seen_from_other_mediums(self):
         seen_from_other_medium_e = G(Event, context={})
         seen_from_medium_event = G(Event, context={}, source=self.source)
         unseen_e = G(Event, context={}, source=self.source)
         G(EventSeen, event=seen_from_other_medium_e)
         G(EventSeen, event=seen_from_medium_event)
 
         events = self.medium.get_filtered_events(seen=False)
-        self.assertEquals(set(events), {unseen_e, seen_from_medium_event, seen_from_other_medium_e})
+        self.assertEqual(set(events), {unseen_e, seen_from_medium_event, seen_from_other_medium_e})
 
 
 class MediumGetEventFiltersTest(TestCase):
     def setUp(self):
         # Call the parent setup
         super(MediumGetEventFiltersTest, self).setUp()
 
@@ -998,19 +998,19 @@
         self.event = N(Event, source=self.source, context={}, id=1)
         self.event_actor = N(EventActor, event=self.event, entity=self.entity)
         self.event_seen = N(
             EventSeen, event=self.event, medium=self.medium, time_seen=datetime(2014, 1, 2))
 
     def test_RenderingStyle_formats(self):
         s = text_type(self.rendering_style)
-        self.assertEquals(s, 'Test Render Group test')
+        self.assertEqual(s, 'Test Render Group test')
 
     def test_contextrenderer_formats(self):
         s = text_type(self.context_renderer)
-        self.assertEquals(s, 'Test Context Renderer')
+        self.assertEqual(s, 'Test Context Renderer')
 
     def test_medium_formats(self):
         s = text_type(self.medium)
         self.assertEqual(s, 'Test Medium')
 
     def test_source_formats(self):
         s = text_type(self.source)
```

### Comparing `django-entity-event-3.0.0/entity_event/tests/models.py` & `django-entity-event-3.1.0/entity_event/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-entity-event-3.0.0/setup.py` & `django-entity-event-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,18 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
-        'Framework :: Django :: 3.1',
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
     install_requires=install_requires,
     tests_require=tests_require,
     test_suite='run_tests.run',
     include_package_data=True,
     zip_safe=False,
```

