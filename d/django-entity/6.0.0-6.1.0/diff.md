# Comparing `tmp/django-entity-6.0.0.tar.gz` & `tmp/django-entity-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-entity-6.0.0.tar", last modified: Tue Jan 24 20:30:15 2023, max compression
+gzip compressed data, was "django-entity-6.1.0.tar", last modified: Thu Jun 29 15:30:35 2023, max compression
```

## Comparing `django-entity-6.0.0.tar` & `django-entity-6.1.0.tar`

### file list

```diff
@@ -1,53 +1,44 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-06-21 20:30:36.000000 django-entity-6.0.0/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       67 2021-07-22 19:05:21.000000 django-entity-6.0.0/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)    21901 2023-01-24 20:30:15.901990 django-entity-6.0.0/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)    20995 2021-07-22 19:05:21.000000 django-entity-6.0.0/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.897990 django-entity-6.0.0/django_entity.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)    21901 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1307 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/not-zip-safe
--rw-rw-r--   0 wes       (1000) wes       (1000)      195 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        7 2023-01-24 20:30:15.000000 django-entity-6.0.0/django_entity.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/
--rw-rw-r--   0 wes       (1000) wes       (1000)       97 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      204 2023-01-24 20:29:11.000000 django-entity-6.0.0/entity/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4465 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/management/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/management/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/management/commands/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/management/commands/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      304 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/management/commands/sync_entities.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2594 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      432 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/migrations/0002_entitykind_is_active.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1504 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0003_auto_20150813_2234.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      511 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0004_auto_20150915_1747.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      358 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/migrations/0005_remove_entitygroup_entities.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2420 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/migrations/0006_entity_relationship_unique.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      517 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/migrations/0007_allentityproxy.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      514 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0008_auto_20180329_1934.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      610 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0009_auto_20180402_2145.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      421 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/migrations/0010_auto_20181213_1817.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    24939 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3919 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/signal_handlers.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    23317 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/sync.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/tests/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/entity/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     5497 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    47144 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/tests/model_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     6950 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     3180 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/tests/registry_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    44201 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/tests/sync_tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1263 2021-06-21 20:30:36.000000 django-entity-6.0.0/entity/tests/utils.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       37 2021-07-22 19:05:21.000000 django-entity-6.0.0/entity/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-01-24 20:29:11.000000 django-entity-6.0.0/entity/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 20:30:15.901990 django-entity-6.0.0/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       65 2023-01-24 20:29:11.000000 django-entity-6.0.0/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      123 2021-07-22 19:05:21.000000 django-entity-6.0.0/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      207 2023-01-24 20:30:15.901990 django-entity-6.0.0/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     1957 2023-01-24 20:29:11.000000 django-entity-6.0.0/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-06-21 20:30:36.000000 django-entity-6.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       67 2021-07-22 19:05:21.000000 django-entity-6.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)    21823 2023-06-29 15:30:35.727623 django-entity-6.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)    20995 2021-07-22 19:05:21.000000 django-entity-6.1.0/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/django_entity.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    21823 2023-06-29 15:30:35.000000 django-entity-6.1.0/django_entity.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      893 2023-06-29 15:30:35.000000 django-entity-6.1.0/django_entity.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 15:30:35.000000 django-entity-6.1.0/django_entity.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 20:30:15.000000 django-entity-6.1.0/django_entity.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)      172 2023-06-29 15:30:35.000000 django-entity-6.1.0/django_entity.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        7 2023-06-29 15:30:35.000000 django-entity-6.1.0/django_entity.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       48 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      204 2023-01-24 20:29:11.000000 django-entity-6.1.0/entity/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4465 2021-07-22 19:05:21.000000 django-entity-6.1.0/entity/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/management/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/management/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/management/commands/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/management/commands/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      304 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/management/commands/sync_entities.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4926 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/migrations/0001_0010_squashed.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    24897 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3919 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/signal_handlers.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    23317 2021-07-22 19:05:21.000000 django-entity-6.1.0/entity/sync.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/tests/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/entity/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5457 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    47102 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/tests/model_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6950 2021-07-22 19:05:21.000000 django-entity-6.1.0/entity/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3189 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/tests/registry_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    44099 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/tests/sync_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1263 2021-06-21 20:30:36.000000 django-entity-6.1.0/entity/tests/utils.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2021-07-22 19:05:21.000000 django-entity-6.1.0/entity/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 15:20:34.000000 django-entity-6.1.0/entity/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 15:30:35.727623 django-entity-6.1.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       60 2023-06-29 15:20:34.000000 django-entity-6.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      105 2023-06-29 15:20:34.000000 django-entity-6.1.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      207 2023-06-29 15:30:35.727623 django-entity-6.1.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1881 2023-06-29 15:20:34.000000 django-entity-6.1.0/setup.py
```

### Comparing `django-entity-6.0.0/LICENSE` & `django-entity-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/PKG-INFO` & `django-entity-6.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: django-entity
-Version: 6.0.0
+Version: 6.1.0
 Summary: Entity relationship management for Django
 Home-page: http://github.com/ambitioninc/django-entity/
 Author: Wes Kendall
 Author-email: wesleykendall@gmail.com
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
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.org/ambitioninc/django-entity.svg)](https://travis-ci.org/ambitioninc/django-entity)
 # Django Entity - [Release Notes](release_notes.md)
```

### Comparing `django-entity-6.0.0/README.md` & `django-entity-6.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/django_entity.egg-info/PKG-INFO` & `django-entity-6.1.0/django_entity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: django-entity
-Version: 6.0.0
+Version: 6.1.0
 Summary: Entity relationship management for Django
 Home-page: http://github.com/ambitioninc/django-entity/
 Author: Wes Kendall
 Author-email: wesleykendall@gmail.com
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
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 [![Build Status](https://travis-ci.org/ambitioninc/django-entity.svg)](https://travis-ci.org/ambitioninc/django-entity)
 # Django Entity - [Release Notes](release_notes.md)
```

### Comparing `django-entity-6.0.0/django_entity.egg-info/SOURCES.txt` & `django-entity-6.1.0/django_entity.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,24 +16,15 @@
 entity/signal_handlers.py
 entity/sync.py
 entity/urls.py
 entity/version.py
 entity/management/__init__.py
 entity/management/commands/__init__.py
 entity/management/commands/sync_entities.py
-entity/migrations/0001_initial.py
-entity/migrations/0002_entitykind_is_active.py
-entity/migrations/0003_auto_20150813_2234.py
-entity/migrations/0004_auto_20150915_1747.py
-entity/migrations/0005_remove_entitygroup_entities.py
-entity/migrations/0006_entity_relationship_unique.py
-entity/migrations/0007_allentityproxy.py
-entity/migrations/0008_auto_20180329_1934.py
-entity/migrations/0009_auto_20180402_2145.py
-entity/migrations/0010_auto_20181213_1817.py
+entity/migrations/0001_0010_squashed.py
 entity/migrations/__init__.py
 entity/tests/__init__.py
 entity/tests/model_tests.py
 entity/tests/models.py
 entity/tests/registry_tests.py
 entity/tests/sync_tests.py
 entity/tests/utils.py
```

### Comparing `django-entity-6.0.0/entity/config.py` & `django-entity-6.1.0/entity/config.py`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/entity/models.py` & `django-entity-6.1.0/entity/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from itertools import compress
 
 from activatable_model.models import BaseActivatableModel, ActivatableManager, ActivatableQuerySet
 from django.contrib.contenttypes.fields import GenericForeignKey
 from django.contrib.contenttypes.models import ContentType
-from django.contrib.postgres.fields import JSONField
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import models
-from django.db.models import Count, Q
+from django.db.models import Count, Q, JSONField
 from python3_utils import compare_on_attr
-from six.moves import reduce
+from functools import reduce
 
 
 class AllEntityKindManager(ActivatableManager):
     """
     Provides additional filtering for entity kinds.
     """
     pass
```

### Comparing `django-entity-6.0.0/entity/signal_handlers.py` & `django-entity-6.1.0/entity/signal_handlers.py`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/entity/sync.py` & `django-entity-6.1.0/entity/sync.py`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/entity/tests/migrations/0001_initial.py` & `django-entity-6.1.0/entity/tests/migrations/0001_initial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-entity-6.0.0/entity/tests/model_tests.py` & `django-entity-6.1.0/entity/tests/model_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,29 +16,29 @@
 class EntityKindManagerTest(EntityTestCase):
     """
     Tests the active and all entity kind managers.
     """
     def test_only_active(self):
         G(EntityKind, is_active=False)
         active_ek = G(EntityKind, is_active=True)
-        self.assertEquals([active_ek], list(EntityKind.objects.all()))
+        self.assertEqual([active_ek], list(EntityKind.objects.all()))
 
     def test_all_objects(self):
         inactive_ek = G(EntityKind, is_active=False)
         active_ek = G(EntityKind, is_active=True)
-        self.assertEquals(set([active_ek, inactive_ek]), set(EntityKind.all_objects.all()))
+        self.assertEqual(set([active_ek, inactive_ek]), set(EntityKind.all_objects.all()))
 
 
 class EntityKindTest(EntityTestCase):
     """
     Tests the EntityKind model.
     """
     def test_unicode(self):
         ek = N(EntityKind, display_name='hello')
-        self.assertEquals(u'{0}'.format(ek), u'hello')
+        self.assertEqual(u'{0}'.format(ek), u'hello')
 
     def test_regular_delete(self):
         """
         Regular deletion should deactivate the entity kind.
         """
         ek = G(EntityKind, is_active=True)
         ek.delete()
@@ -48,15 +48,15 @@
 class TestActiveEntityManager(EntityTestCase):
     def test_filters_active_by_default(self):
         """
         Tests that active entities are returned by default when accessing Entity.objects
         """
         e = G(Entity, is_active=True)
         G(Entity, is_active=False)
-        self.assertEquals([e], list(Entity.objects.all()))
+        self.assertEqual([e], list(Entity.objects.all()))
 
 
 class TestAllEntityManager(EntityTestCase):
     """
     Tests custom function in the AllEntityManager class.
     """
     def setUp(self):
@@ -82,15 +82,15 @@
         # Five queries should happen here - one for all entities, two for EntityRelationships,
         # and two more for entities in the relationships
         with self.assertNumQueries(5):
             entities = Entity.objects.cache_relationships()
             for entity in entities:
                 self.assertTrue(len(list(entity.get_super_entities())) >= 0)
                 self.assertTrue(len(list(entity.get_sub_entities())) >= 0)
-        self.assertEquals(entities.count(), 6)
+        self.assertEqual(entities.count(), 6)
 
     def test_manager_cache_relationships_only_sub(self):
         """
         Tests a retrieval of cache relationships on the manager and verifies it results in the smallest amount of
         queries when only caching sub entities.
         """
         team = Team.objects.create()
@@ -99,15 +99,15 @@
 
         # Five queries should happen here - one for all entities, two for EntityRelationships,
         # and two more for entities in the relationships
         with self.assertNumQueries(3):
             entities = Entity.objects.cache_relationships(cache_super=False)
             for entity in entities:
                 self.assertTrue(len(list(entity.get_sub_entities())) >= 0)
-        self.assertEquals(entities.count(), 6)
+        self.assertEqual(entities.count(), 6)
 
     def test_manager_cache_relationships_only_super(self):
         """
         Tests a retrieval of cache relationships on the manager and verifies it results in the smallest amount of
         queries when only caching super entities.
         """
         team = Team.objects.create()
@@ -116,15 +116,15 @@
 
         # Five queries should happen here - one for all entities, two for EntityRelationships,
         # and two more for entities in the relationships
         with self.assertNumQueries(3):
             entities = Entity.objects.cache_relationships(cache_sub=False)
             for entity in entities:
                 self.assertTrue(len(list(entity.get_super_entities())) >= 0)
-        self.assertEquals(entities.count(), 6)
+        self.assertEqual(entities.count(), 6)
 
     def test_manager_cache_relationships_none(self):
         """
         Tests a retrieval of cache relationships on the manager and verifies it results in the smallest amount of
         queries when super and sub are set to false
         """
         team = Team.objects.create()
@@ -132,15 +132,15 @@
             Account.objects.create(team=team)
 
         # Five queries should happen here - one for all entities, two for EntityRelationships,
         # and two more for entities in the relationships
         with self.assertNumQueries(1):
             entities = Entity.objects.cache_relationships(cache_sub=False, cache_super=False)
             self.assertTrue(len(entities) > 0)
-        self.assertEquals(entities.count(), 6)
+        self.assertEqual(entities.count(), 6)
 
     def test_queryset_cache_relationships(self):
         """
         Tests a retrieval of cache relationships on the queryset and verifies it results in the smallest amount of
         queries
         """
         team = Team.objects.create()
@@ -151,15 +151,15 @@
         # Five queries should happen here - 1 for the Entity filter, two for EntityRelationships, and two more
         # for entities in those relationships
         with self.assertNumQueries(5):
             entities = Entity.objects.filter(id__in=entity_ids).cache_relationships()
             for entity in entities:
                 self.assertTrue(len(list(entity.get_super_entities())) >= 0)
                 self.assertTrue(len(list(entity.get_sub_entities())) >= 0)
-        self.assertEquals(entities.count(), 6)
+        self.assertEqual(entities.count(), 6)
 
     def test_cache_subset(self):
         """
         Tests that caching still operates the same on an entity subset call.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
@@ -169,105 +169,105 @@
         # Five queries should happen here - 1 for the Entity filter, two for EntityRelationships, and one more
         # for entities in those relationships (since no sub relationships exist)
         with self.assertNumQueries(4):
             entities = Entity.objects.is_sub_to_all(team_entity).cache_relationships()
             for entity in entities:
                 self.assertTrue(len(list(entity.get_super_entities())) == 1)
                 self.assertTrue(len(list(entity.get_sub_entities())) == 0)
-            self.assertEquals(len(entities), 5)
+            self.assertEqual(len(entities), 5)
 
     def test_get_for_obj(self):
         """
         Test retrieving an entity associated with an object.
         """
         # Create an account with no team
         account = Account.objects.create()
         # Get its resulting entity
         entity = Entity.objects.get(entity_type=ContentType.objects.get_for_model(account), entity_id=account.id)
-        self.assertEquals(entity, Entity.objects.get_for_obj(account))
+        self.assertEqual(entity, Entity.objects.get_for_obj(account))
 
     def test_filter_manager_active(self):
         """
         Test filtering active entities directly from the manager.
         """
         # Create an active and inactive account
         account = Account.objects.create()
         Account.objects.create(is_active=False)
         # Get its resulting entity
         entity = Entity.objects.get_for_obj(account)
-        self.assertEquals([entity], list(Entity.objects.active()))
+        self.assertEqual([entity], list(Entity.objects.active()))
 
     def test_filter_manager_inactive(self):
         """
         Test filtering inactive entities directly from the manager.
         """
         # Create an active and inactive account
         account = Account.objects.create()
         account = Account.objects.create(is_active=False)
         # Get its resulting entity
         entity = Entity.all_objects.get_for_obj(account)
-        self.assertEquals([entity], list(Entity.all_objects.inactive()))
+        self.assertEqual([entity], list(Entity.all_objects.inactive()))
 
     def test_filter_queryset_active(self):
         """
         Test filtering active entities from a queryset.
         """
         # Create an active and inactive account
         active_entity = Entity.objects.get_for_obj(Account.objects.create())
         inactive_entity = Entity.all_objects.get_for_obj(Account.objects.create(is_active=False))
-        self.assertEquals(
+        self.assertEqual(
             [active_entity], list(Entity.objects.filter(id__in=[active_entity.id, inactive_entity.id]).active()))
 
     def test_filter_queryset_inactive(self):
         """
         Test filtering inactive entities from a queryset.
         """
         # Create an active and inactive account
         active_entity = Entity.objects.get_for_obj(Account.objects.create())
         inactive_entity = Entity.all_objects.get_for_obj(Account.objects.create(is_active=False))
-        self.assertEquals(
+        self.assertEqual(
             [inactive_entity],
             list(Entity.all_objects.filter(id__in=[active_entity.id, inactive_entity.id]).inactive()))
 
     def test_filter_manager_is_kind_none(self):
         """
         Tests filtering by entity kind when no kind is given.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = [
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         ]
-        self.assertEquals(set([team_entity] + account_entities), set(Entity.objects.is_any_kind()))
+        self.assertEqual(set([team_entity] + account_entities), set(Entity.objects.is_any_kind()))
 
     def test_filter_manager_one_kind(self):
         """
         Tests filtering by entity kind when one kind is given.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals([team_entity], list(Entity.objects.is_any_kind(self.team_kind)))
-        self.assertEquals(account_entities, set(Entity.objects.is_any_kind(self.account_kind)))
+        self.assertEqual([team_entity], list(Entity.objects.is_any_kind(self.team_kind)))
+        self.assertEqual(account_entities, set(Entity.objects.is_any_kind(self.account_kind)))
 
     def test_filter_manager_two_kinds(self):
         """
         Tests filtering by entity kind when two kinds are given.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals(
+        self.assertEqual(
             account_entities.union([team_entity]), set(Entity.objects.is_any_kind(self.account_kind, self.team_kind)))
 
     def test_is_sub_to_all_kinds_none(self):
         # set up teams, groups and competitors
         team = Team.objects.create()
         group = TeamGroup.objects.create(name='group')
         competitor = Competitor.objects.create(name='competitor')
@@ -400,67 +400,67 @@
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals(
+        self.assertEqual(
             account_entities.union([team_entity]),
             set(
                 Entity.objects.filter(id__in=(i.id for i in account_entities.union([team_entity]))).is_any_kind(
                     self.account_kind, self.team_kind)
             ))
 
     def test_filter_manager_is_not_kind_two(self):
         """
         Tests filtering by entity kind when two kinds are given.
         """
         team = Team.objects.create()
         for i in range(5):
             Account.objects.create(team=team)
-        self.assertEquals([], list(Entity.objects.is_not_any_kind(self.team_kind, self.account_kind)))
+        self.assertEqual([], list(Entity.objects.is_not_any_kind(self.team_kind, self.account_kind)))
 
     def test_filter_manager_is_not_kind_one(self):
         """
         Tests filtering by entity kind when one kind is given.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals([team_entity], list(Entity.objects.is_not_any_kind(self.account_kind)))
-        self.assertEquals(account_entities, set(Entity.objects.is_not_any_kind(self.team_kind)))
+        self.assertEqual([team_entity], list(Entity.objects.is_not_any_kind(self.account_kind)))
+        self.assertEqual(account_entities, set(Entity.objects.is_not_any_kind(self.team_kind)))
 
     def test_filter_manager_is_not_kind_none(self):
         """
         Tests filtering by entity kind when no kinds are given.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals(
+        self.assertEqual(
             account_entities.union([team_entity]), set(Entity.objects.is_not_any_kind()))
 
     def test_filter_queryset_two_is_not_kinds(self):
         """
         Tests filtering by entity type when two kinds are given on a queryset.
         """
         team = Team.objects.create()
         team_entity = Entity.objects.get_for_obj(team)
         account_entities = set(
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
-        self.assertEquals(
+        self.assertEqual(
             [],
             list(Entity.objects.filter(id__in=(i.id for i in account_entities.union([team_entity]))).is_not_any_kind(
                 self.account_kind, self.team_kind))
         )
 
     def test_is_sub_to_all_none(self):
         """
@@ -476,15 +476,15 @@
         for i in range(5):
             Account.objects.create(competitor=competitor, team=team, team2=team2, team_group=team_group)
 
         # Create accounts that have no super entities
         for i in range(5):
             Entity.objects.get_for_obj(Account.objects.create())
 
-        self.assertEquals(
+        self.assertEqual(
             set(Entity.objects.all()), set(Entity.objects.is_sub_to_all()))
 
     def test_is_sub_to_all_none_is_any_kind(self):
         """
         Tests the base case of is_sub_to_all on no super entities with a kind specified.
         """
         # Create test accounts that have three types of super entities
@@ -497,15 +497,15 @@
         for i in range(5):
             Account.objects.create(competitor=competitor, team=team, team2=team2, team_group=team_group)
 
         # Create accounts that have no super entities
         for i in range(5):
             Entity.objects.get_for_obj(Account.objects.create())
 
-        self.assertEquals(
+        self.assertEqual(
             set(Entity.objects.filter(entity_type=self.account_type)),
             set(Entity.objects.is_sub_to_all().is_any_kind(self.account_kind)))
 
     def test_is_sub_to_all_manager(self):
         """
         Tests the is_sub_to_all for an entity directly from the entity manager.
         """
@@ -533,24 +533,24 @@
         entities_2se2 = set(
             Entity.objects.get_for_obj(Account.objects.create(competitor=competitor, team=team)) for i in range(5)
         )
         # Create test accounts that have one super entity
         entities_1se = set(Entity.objects.get_for_obj(Account.objects.create(team=team)) for i in range(5))
 
         # Test various subset results
-        self.assertEquals(
+        self.assertEqual(
             entities_4se, set(Entity.objects.is_sub_to_all(
                 team_entity, team2_entity, team_group_entity, competitor_entity)))
-        self.assertEquals(
+        self.assertEqual(
             entities_1se | entities_2se2 | entities_4se, set(Entity.objects.is_sub_to_all(team_entity)))
-        self.assertEquals(
+        self.assertEqual(
             entities_4se | entities_2se2, set(Entity.objects.is_sub_to_all(team_entity, competitor_entity)))
-        self.assertEquals(
+        self.assertEqual(
             entities_4se | entities_2se1, set(Entity.objects.is_sub_to_all(team_group_entity)))
-        self.assertEquals(
+        self.assertEqual(
             entities_4se | entities_2se1 | entities_2se2,
             set(Entity.objects.is_sub_to_all(competitor_entity)))
 
     def test_is_sub_to_all_queryset(self):
         """
         Tests the subset of super entity types for an entity from a queryset.
         """
@@ -568,15 +568,15 @@
         entities_4se = list(
             Entity.objects.get_for_obj(
                 Account.objects.create(competitor=competitor, team=team, team2=team2, team_group=team_group))
             for i in range(5)
         )
 
         # Test subset results
-        self.assertEquals(
+        self.assertEqual(
             set(entities_4se).difference([entities_4se[0]]),
             set(Entity.objects.exclude(id=entities_4se[0].id).is_sub_to_all(
                 team_entity, team2_entity, team_group_entity, competitor_entity)))
 
     def test_is_sub_to_all_queryset_num_queries(self):
         """
         Tests that is_sub_to_all only results in one query.
@@ -599,15 +599,15 @@
         )
 
         with self.assertNumQueries(1):
             entities = set(Entity.objects.exclude(id=entities_4se[0].id).is_sub_to_all(
                 team_entity, team2_entity, team_group_entity, competitor_entity))
 
         # Test subset results
-        self.assertEquals(set(entities_4se).difference([entities_4se[0]]), entities)
+        self.assertEqual(set(entities_4se).difference([entities_4se[0]]), entities)
 
     def test_is_sub_to_any_none(self):
         """
         Tests the base case of is_sub_to_any on no super entities.
         """
         # Create test accounts that have three types of super entities
         team = Team.objects.create()
@@ -619,15 +619,15 @@
         for i in range(5):
             Account.objects.create(competitor=competitor, team=team, team2=team2, team_group=team_group)
 
         # Create accounts that have no super entities
         for i in range(5):
             Entity.objects.get_for_obj(Account.objects.create())
 
-        self.assertEquals(
+        self.assertEqual(
             set(Entity.objects.all()), set(Entity.objects.is_sub_to_any()))
 
     def test_is_sub_to_any_queryset(self):
         """
         Tests the is_sub_to_any for an entity from a queryset.
         """
         # Create test accounts that have three types of super entities
@@ -644,15 +644,15 @@
         entities_4se = list(
             Entity.objects.get_for_obj(
                 Account.objects.create(competitor=competitor, team=team, team2=team2, team_group=team_group))
             for i in range(5)
         )
 
         # Test subset results
-        self.assertEquals(
+        self.assertEqual(
             set(entities_4se).difference([entities_4se[0]]),
             set(Entity.objects.exclude(id=entities_4se[0].id).is_sub_to_any(
                 team_entity, team2_entity, team_group_entity, competitor_entity)))
 
     def test_is_sub_to_any_limited_results(self):
         """
         Tests the is_sub_to_any for an entity from a queryset where the is_sub_to_any returns less than all
@@ -668,15 +668,15 @@
             Entity.objects.get_for_obj(Account.objects.create(team=team))
             for i in range(5)
         )
         for i in range(5):
             Account.objects.create(team=team2)
 
         # Test subset results
-        self.assertEquals(set(entities_w_team), set(Entity.objects.is_sub_to_any(team_entity)))
+        self.assertEqual(set(entities_w_team), set(Entity.objects.is_sub_to_any(team_entity)))
 
 
 class TestEntityModel(EntityTestCase):
     """
     Tests custom functionality in the Entity model.
     """
     def test_get_super_entities_none(self):
@@ -685,61 +685,61 @@
         have no super entities
         """
         # Create an account with no team
         account = Account.objects.create()
         # Get its resulting entity
         entity = Entity.objects.get_for_obj(account)
         # Get its super entities. It should be an empty list
-        self.assertEquals(list(entity.get_super_entities()), [])
+        self.assertEqual(list(entity.get_super_entities()), [])
 
     def test_get_super_entities_one(self):
         """
         Tests retrieval of super entities when an entity has exactly one.
         """
         # Create a team and an account with the team as a super entity.
         team = Team.objects.create()
         account = Account.objects.create(team=team)
         # Get the entity of the account and the team
         account_entity = Entity.objects.get_for_obj(account)
         team_entity = Entity.objects.get_for_obj(team)
         # Verify that the super entities of the account is the team
-        self.assertEquals(list(account_entity.get_super_entities()), [team_entity])
+        self.assertEqual(list(account_entity.get_super_entities()), [team_entity])
 
     def test_get_sub_entities_none(self):
         """
         Tests retrieval of sub entities when an entity has none.
         """
         # Create a team
         team = Team.objects.create()
         # Get the entity of the team
         team_entity = Entity.objects.get_for_obj(team)
         # Verify that the sub entities of the team is an empty list
-        self.assertEquals(list(team_entity.get_super_entities()), [])
+        self.assertEqual(list(team_entity.get_super_entities()), [])
 
     def test_get_sub_entities_one(self):
         """
         Tests retrieval of sub entities when an entity has exactly one.
         """
         # Create a team and an account with the team as a super entity.
         team = Team.objects.create()
         account = Account.objects.create(team=team)
         # Get the entity of the account and the team
         account_entity = Entity.objects.get_for_obj(account)
         team_entity = Entity.objects.get_for_obj(team)
         # Verify that the sub entities of the team is the account
-        self.assertEquals(list(team_entity.get_sub_entities()), [account_entity])
+        self.assertEqual(list(team_entity.get_sub_entities()), [account_entity])
 
     def test_unicode(self):
         """
         Tests that the unicode method returns the display name of the entity.
         """
         account = Account.objects.create(email='hi')
         entity = Entity.objects.get_for_obj(account)
         entity_unicode = entity.__str__()
-        self.assertEquals(entity_unicode, 'hi')
+        self.assertEqual(entity_unicode, 'hi')
 
 
 class EntityGroupAllEntitiesTest(EntityTestCase):
     def setUp(self):
         super(EntityGroupAllEntitiesTest, self).setUp()
         # Create three super entities, each with two sub
         # entities. THere are two entity kinds. Super entity 1 has two
```

### Comparing `django-entity-6.0.0/entity/tests/models.py` & `django-entity-6.1.0/entity/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/entity/tests/registry_tests.py` & `django-entity-6.1.0/entity/tests/registry_tests.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db.models import Model
 from django.test import TestCase
-from mock import patch
+from unittest.mock import patch
 
 from entity.config import EntityConfig, entity_registry, EntityRegistry, register_entity
 
 
 class EntityRegistryTest(TestCase):
     """
     Tests the EntityRegistry class.
```

### Comparing `django-entity-6.0.0/entity/tests/sync_tests.py` & `django-entity-6.1.0/entity/tests/sync_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from entity.config import EntityRegistry
 from entity.models import Entity, EntityRelationship, EntityKind
 from entity.sync import (
     sync_entities, defer_entity_syncing, transaction_atomic_with_retry, _get_super_entities_by_ctype,
     suppress_entity_syncing,
 )
 from entity.signal_handlers import turn_on_syncing, turn_off_syncing
-from mock import patch, MagicMock, call
+from unittest.mock import patch, MagicMock, call
 
 from entity.tests.models import (
     Account, Team, EntityPointer, DummyModel, MultiInheritEntity, AccountConfig, TeamConfig, TeamGroup,
     M2mEntity, PointsToM2mEntity, PointsToAccount, Competitor
 )
 from entity.tests.utils import EntityTestCase
 
@@ -87,15 +87,15 @@
         """
         Tests that delete signals are connected by default.
         """
         a = Account.objects.create()
         with patch('entity.models.Entity.all_objects.delete_for_obj') as mock_handler:
             # Delete the object. The signal should be called
             a.delete()
-            self.assertEquals(mock_handler.call_count, 1)
+            self.assertEqual(mock_handler.call_count, 1)
 
     def test_bulk_operation_turned_off_by_default(self):
         """
         Tests that bulk operations are turned off by default.
         """
         with patch('entity.signal_handlers.sync_entities') as mock_handler:
             Account.objects.bulk_create([Account() for i in range(5)])
@@ -145,15 +145,15 @@
         Tests turning on syncing for the delete signal.
         """
         turn_off_syncing()
         turn_on_syncing()
         with patch('entity.models.Entity.all_objects.delete_for_obj') as mock_handler:
             a = Account.objects.create()
             a.delete()
-            self.assertEquals(mock_handler.call_count, 1)
+            self.assertEqual(mock_handler.call_count, 1)
 
     def test_turn_on_bulk(self):
         """
         Tests turning on syncing for bulk operations.
         """
         turn_off_syncing()
         turn_on_syncing(for_post_bulk_operation=True)
@@ -174,62 +174,62 @@
         # Create five test accounts
         turn_off_syncing()
         for i in range(5):
             Account.objects.create()
         turn_on_syncing()
 
         # Test that the management command syncs all five entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
         call_command('sync_entities')
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
 
     def test_sync_dummy_data(self):
         """
         Tests that dummy data (i.e data that does not inherit EntityModelMixin) doesn't
         get synced.
         """
         # Create dummy data
         DummyModel.objects.create()
         # Sync all entities and verify that none were created
         sync_entities()
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
     def test_sync_multi_inherited_data(self):
         """
         Test when models are synced that don't directly inherit EntityModelMixin.
         """
         # Create an entity that does not directly inherit EntityModelMixin
         MultiInheritEntity.objects.create()
         # Sync all entities and verify that one was created
         sync_entities()
-        self.assertEquals(Entity.objects.all().count(), 1)
+        self.assertEqual(Entity.objects.all().count(), 1)
 
     def test_sync_all_account_no_teams(self):
         """
         Tests syncing all accounts with no super entities.
         """
         turn_off_syncing()
         # Create five test accounts
         accounts = [Account.objects.create() for i in range(5)]
         turn_on_syncing()
 
         # Sync all of the entities and verify that five Entity models were created for the Account model
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
         sync_entities()
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
 
         # Delete an account. When all entities are synced again,
         # there should only be four accounts
         turn_off_syncing()
         accounts[0].delete()
         turn_on_syncing()
 
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
         sync_entities()
-        self.assertEquals(Entity.objects.all().count(), 4)
+        self.assertEqual(Entity.objects.all().count(), 4)
 
     def test_sync_all_accounts_teams(self):
         """
         Tests syncing of all accounts when they have super entities.
         """
         # Create five test accounts
         accounts = [Account.objects.create() for i in range(5)]
@@ -242,20 +242,20 @@
         accounts[2].team = teams[1]
         accounts[2].save()
         accounts[3].team = teams[1]
         accounts[3].save()
 
         # Sync all the entities. There should be 7 (5 accounts 2 teams)
         sync_entities()
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
-        self.assertEquals(Entity.objects.all().count(), 7)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 7)
 
         # There should be four entity relationships since four accounts have teams
-        self.assertEquals(EntityRelationship.objects.all().count(), 4)
+        self.assertEqual(EntityRelationship.objects.all().count(), 4)
 
     def test_sync_all_accounts_teams_new_account_during_sync(self):
         """
         Tests the scenario of a new account being created after account ids are fetched but before the super
         entities are fetched
         """
         # Create five test accounts
@@ -281,20 +281,20 @@
 
             return _get_super_entities_by_ctype(*args, **kwargs)
 
         # Sync all the entities. There should be 8 (6 accounts 2 teams)
         with patch('entity.sync._get_super_entities_by_ctype', wraps=wrapped_super_entities):
             sync_entities()
 
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 6)
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
-        self.assertEquals(Entity.objects.all().count(), 8)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 6)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 8)
 
         # There should be six entity relationships
-        self.assertEquals(EntityRelationship.objects.all().count(), 6)
+        self.assertEqual(EntityRelationship.objects.all().count(), 6)
 
     def test_sync_all_accounts_teams_deleted_account_during_sync(self):
         """
         Tests the scenario of an account being deleted after account ids are fetched but before the super
         entities are fetched
         """
         # Create five test accounts
@@ -330,20 +330,20 @@
         with patch('entity.sync._get_super_entities_by_ctype', wraps=wrapped_super_entities):
             accounts = Account.objects.all()
             sync_entities(*accounts)
             account = Account.objects.get(email='fake@fake.com')
             entity = Entity.all_objects.get_for_obj(account)
             self.assertEqual(entity.is_active, False)
 
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 4)
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
-        self.assertEquals(Entity.objects.all().count(), 6)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 4)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 6)
 
         # There should be six entity relationships
-        self.assertEquals(EntityRelationship.objects.all().count(), 4)
+        self.assertEqual(EntityRelationship.objects.all().count(), 4)
 
     def test_sync_all_accounts_teams_inactive_entity_kind(self):
         """
         Tests syncing of all accounts when they have super entities and the entity kind is inactive
         """
         # Create five test accounts
         accounts = [Account.objects.create() for i in range(5)]
@@ -359,20 +359,20 @@
         accounts[3].save()
 
         team_ek = EntityKind.objects.get(name='tests.team')
         team_ek.delete()
 
         # Sync all the entities. There should be 7 (5 accounts 2 teams)
         sync_entities()
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
-        self.assertEquals(Entity.objects.all().count(), 7)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 7)
 
         # There should be four entity relationships since four accounts have teams
-        self.assertEquals(EntityRelationship.objects.all().count(), 4)
+        self.assertEqual(EntityRelationship.objects.all().count(), 4)
 
 
 class SyncSignalTests(EntityTestCase):
     """
     Test that when we are syncing we are calling the proper signals
     """
 
@@ -386,17 +386,17 @@
         turn_off_syncing()
         initial_accounts = []
         for i in range(5):
             initial_accounts.append(Account.objects.create())
         turn_on_syncing()
 
         # Test that the management command syncs all five entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
         sync_entities()
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
         initial_entity_ids = list(Entity.objects.all().values_list('id', flat=True))
         mock_model_activations_changed.send.assert_called_once_with(
             sender=Entity,
             instance_ids=sorted(initial_entity_ids),
             is_active=True
         )
 
@@ -450,36 +450,36 @@
         """
         Tests that entities can have bulk creates applied to them and still be synced.
         """
         # Bulk create five accounts
         accounts = [Account() for i in range(5)]
         Account.objects.bulk_create(accounts)
         # Verify that there are 5 entities
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
 
     def test_post_bulk_update(self):
         """
         Calls a bulk update on a list of entities. Verifies that the models are appropriately
         synced.
         """
         # Create five accounts
         for i in range(5):
             Account.objects.create(email='test1@test.com')
         # Verify that there are five entities all with the 'test1@test.com' email
         for entity in Entity.objects.all():
-            self.assertEquals(entity.entity_meta['email'], 'test1@test.com')
-        self.assertEquals(Entity.objects.all().count(), 5)
+            self.assertEqual(entity.entity_meta['email'], 'test1@test.com')
+        self.assertEqual(Entity.objects.all().count(), 5)
 
         # Bulk update the account emails to a different one
         Account.objects.all().update(email='test2@test.com')
 
         # Verify that the email was updated properly in all entities
         for entity in Entity.objects.all():
-            self.assertEquals(entity.entity_meta['email'], 'test2@test.com')
-        self.assertEquals(Entity.objects.all().count(), 5)
+            self.assertEqual(entity.entity_meta['email'], 'test2@test.com')
+        self.assertEqual(Entity.objects.all().count(), 5)
 
     def test_invalid_entity_model(self):
         """
         Tests that an invalid entity model is not synced on bulk update.
         """
         DummyModel.objects.bulk_create([DummyModel()])
         self.assertFalse(Entity.objects.exists())
@@ -488,37 +488,37 @@
         """
         Tests that even if the dummy model is using the special model manager for bulk
         updates, it still does not get synced since it doesn't inherit EntityModelMixin.
         """
         # Create five dummy models with a bulk update
         DummyModel.objects.bulk_create([DummyModel() for i in range(5)])
         # There should be no synced entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
 
 class TestWatching(EntityTestCase):
     """
     Tests when an entity is watching another model for changes.
     """
     def test_m2m_changed_of_another_model(self):
         """
         Tests when an entity model is listening for a change of an m2m of another model.
         """
         m2m_entity = G(M2mEntity)
         team = G(Team)
         points_to_m2m_entity = G(PointsToM2mEntity, m2m_entity=m2m_entity)
         # Three entities should be synced and there should not yet be any relationships
-        self.assertEquals(Entity.objects.count(), 3)
+        self.assertEqual(Entity.objects.count(), 3)
         self.assertFalse(EntityRelationship.objects.exists())
 
         # When a team is added to the m2m entity, it should be a super entity to the points_to_m2m_entity and
         # of m2m_entity
         m2m_entity.teams.add(team)
-        self.assertEquals(Entity.objects.count(), 3)
-        self.assertEquals(EntityRelationship.objects.count(), 2)
+        self.assertEqual(Entity.objects.count(), 3)
+        self.assertEqual(EntityRelationship.objects.count(), 2)
 
         points_to_m2m_entity = Entity.objects.get_for_obj(points_to_m2m_entity)
         team_entity = Entity.objects.get_for_obj(team)
         m2m_entity = Entity.objects.get_for_obj(m2m_entity)
         self.assertTrue(EntityRelationship.objects.filter(
             sub_entity=points_to_m2m_entity, super_entity=team_entity).exists())
         self.assertTrue(EntityRelationship.objects.filter(sub_entity=m2m_entity, super_entity=team_entity).exists())
@@ -526,47 +526,47 @@
     def test_points_to_account_config_competitor_updated(self):
         """
         Tests that a PointsToAccount model is updated when the competitor of its account is updated.
         """
         account = G(Account)
         pta = G(PointsToAccount, account=account)
         pta_entity = Entity.objects.get_for_obj(pta)
-        self.assertEquals(pta_entity.entity_meta, {
+        self.assertEqual(pta_entity.entity_meta, {
             'team_name': 'None',
             'competitor_name': 'None',
         })
 
         team = G(Team, name='team1')
         competitor = G(Competitor, name='competitor1')
         account.team = team
         account.competitor = competitor
         account.save()
 
         # Nothing should have been updated on the entity. This is because it is watching the competitor
         # and team models for changes. Since these models were changed before they were linked to the
         # account, the changes are not propagated.
         pta_entity = Entity.objects.get_for_obj(pta)
-        self.assertEquals(pta_entity.entity_meta, {
+        self.assertEqual(pta_entity.entity_meta, {
             'team_name': 'None',
             'competitor_name': 'None',
         })
 
         # Now change names of the competitors and teams. Things will be propagated.
         team.name = 'team2'
         team.save()
         pta_entity = Entity.objects.get_for_obj(pta)
-        self.assertEquals(pta_entity.entity_meta, {
+        self.assertEqual(pta_entity.entity_meta, {
             'team_name': 'team2',
             'competitor_name': 'competitor1',
         })
 
         competitor.name = 'competitor2'
         competitor.save()
         pta_entity = Entity.objects.get_for_obj(pta)
-        self.assertEquals(pta_entity.entity_meta, {
+        self.assertEqual(pta_entity.entity_meta, {
             'team_name': 'team2',
             'competitor_name': 'competitor2',
         })
 
         # The power of django entity compels you...
 
 
@@ -580,53 +580,53 @@
         """
         turn_off_syncing()
         m = G(M2mEntity)
         m.teams.add(G(Team))
         turn_on_syncing()
 
         m.save()
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 1)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 1)
 
     def test_sync_when_m2m_add(self):
         """
         Verifies an entity is synced properly when and m2m field is added.
         """
         m = G(M2mEntity)
-        self.assertEquals(Entity.objects.count(), 1)
-        self.assertEquals(EntityRelationship.objects.count(), 0)
+        self.assertEqual(Entity.objects.count(), 1)
+        self.assertEqual(EntityRelationship.objects.count(), 0)
         m.teams.add(G(Team))
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 1)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 1)
 
     def test_sync_when_m2m_delete(self):
         """
         Verifies an entity is synced properly when and m2m field is deleted.
         """
         m = G(M2mEntity)
         team = G(Team)
         m.teams.add(team)
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 1)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 1)
         m.teams.remove(team)
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 0)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 0)
 
     def test_sync_when_m2m_clear(self):
         """
         Verifies an entity is synced properly when and m2m field is cleared.
         """
         m = G(M2mEntity)
         team = G(Team)
         m.teams.add(team)
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 1)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 1)
         m.teams.clear()
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 0)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 0)
 
 
 class TestEntityPostSavePostDeleteSignalSync(EntityTestCase):
     """
     Tests that entities (from the test models) are properly synced upon post_save
     and post_delete signals.
     """
@@ -652,63 +652,63 @@
     def test_display_name_mirrored_default(self):
         """
         Tests that the display name is mirrored to the __unicode__ of the models. This
         is the default behavior.
         """
         a = Account.objects.create(email='test_email')
         e = Entity.objects.get_for_obj(a)
-        self.assertEquals(e.display_name, 'test_email')
+        self.assertEqual(e.display_name, 'test_email')
 
     def test_display_name_mirrored_custom(self):
         """
         Tests that the display name is mirrored properly when a custom get_display_name
         function is defined. In this case, the function for Teams returns 'team'
         """
         t = G(Team)
         e = Entity.objects.get_for_obj(t)
-        self.assertEquals(e.display_name, 'team')
+        self.assertEqual(e.display_name, 'team')
 
     def test_post_save_dummy_data(self):
         """
         Tests that dummy data that does not inherit from EntityModelMixin is not synced
         when saved.
         """
         DummyModel.objects.create()
         # Verify that no entities were created
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
     def test_post_save_multi_inherit_model(self):
         """
         Tests that a model that does not directly inherit EntityModelMixin is still synced.
         """
         MultiInheritEntity.objects.create()
         # Verify that one entity was synced
-        self.assertEquals(Entity.objects.all().count(), 1)
+        self.assertEqual(Entity.objects.all().count(), 1)
 
     def test_post_delete_inactive_entity(self):
         """
         Tests deleting an entity that was already inactive.
         """
         account = Account.objects.create(is_active=False)
         account.delete()
-        self.assertEquals(Entity.all_objects.all().count(), 0)
+        self.assertEqual(Entity.all_objects.all().count(), 0)
 
     def test_post_delete_no_entity(self):
         """
         Tests a post_delete on an account that has no current mirrored entity.
         """
         # Create an account
         account = Account.objects.create()
         # Clear out the Entity table since post_save will create an entry for it
         Entity.objects.all().delete()
 
         # Delete the created model. No errors should occur and nothing should
         # be in the entity table
         account.delete()
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
     def test_post_delete_account(self):
         """
         Tests a post_delete on an account that has a current mirrored entity.
         """
         # Create accounts for the test
         main_account = Account.objects.create()
@@ -719,99 +719,99 @@
         # Create entity entries for the account object and for another account
         self.create_entity(main_account)
         self.create_entity(other_account)
 
         # Delete the created model. No errors should occur and the other account
         # should still be an entity in the Entity table.
         main_account.delete()
-        self.assertEquals(Entity.objects.all().count(), 1)
-        self.assertEquals(Entity.objects.filter(entity_id=other_account.id).count(), 1)
+        self.assertEqual(Entity.objects.all().count(), 1)
+        self.assertEqual(Entity.objects.filter(entity_id=other_account.id).count(), 1)
 
     def test_post_delete_account_under_team(self):
         """
         Tests the deletion of an account that had a relationship with a team.
         """
         # Create a team
         team = Team.objects.create(name='Team')
         # Create an account under that team
         account = Account.objects.create(email='test@test.com', team=team)
 
         # There should be two entities and a relationship between them.
-        self.assertEquals(Entity.objects.all().count(), 2)
-        self.assertEquals(EntityRelationship.objects.all().count(), 1)
+        self.assertEqual(Entity.objects.all().count(), 2)
+        self.assertEqual(EntityRelationship.objects.all().count(), 1)
 
         # Delete the account. The team entity should still exist
         account.delete()
-        self.assertEquals(Entity.objects.all().count(), 1)
-        self.assertEquals(EntityRelationship.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 1)
+        self.assertEqual(EntityRelationship.objects.all().count(), 0)
         Entity.objects.get_for_obj(team)
 
     def test_post_create_account_no_relationships_active(self):
         """
         Tests that an Entity is created when the appropriate EntityModelMixin model is
         created. Tests the case where the entity has no relationships.
         """
         # Verify that there are no entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
         # Create an account. An entity with no relationships should be created
         account = Account.objects.create(email='test@test.com')
         entity = Entity.objects.get_for_obj(account)
         # Check that the metadata and is_active fields were set properly
-        self.assertEquals(entity.entity_meta, {
+        self.assertEqual(entity.entity_meta, {
             'email': 'test@test.com',
             'is_captain': False,
             'team': None,
             'team_is_active': None,
         })
-        self.assertEquals(entity.is_active, True)
+        self.assertEqual(entity.is_active, True)
 
-        self.assertEquals(entity.sub_relationships.all().count(), 0)
-        self.assertEquals(entity.super_relationships.all().count(), 0)
+        self.assertEqual(entity.sub_relationships.all().count(), 0)
+        self.assertEqual(entity.super_relationships.all().count(), 0)
 
     def test_post_create_account_relationships(self):
         """
         Creates an account that has super relationships. Verifies that the entity table is updated
         properly.
         """
         # Verify that there are no entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
         # Create a team
         team = Team.objects.create(name='Team')
         # Create an account under that team
         account = Account.objects.create(email='test@test.com', team=team)
 
         # There should be two entities. Test their existence and values
-        self.assertEquals(Entity.objects.all().count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 2)
         account_entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(account_entity.entity_meta, {
+        self.assertEqual(account_entity.entity_meta, {
             'email': 'test@test.com',
             'is_captain': False,
             'team': 'Team',
             'team_is_active': True,
         })
         team_entity = Entity.objects.get_for_obj(team)
-        self.assertEquals(team_entity.entity_meta, None)
+        self.assertEqual(team_entity.entity_meta, None)
 
         # Check that the appropriate entity relationship was created
-        self.assertEquals(EntityRelationship.objects.all().count(), 1)
+        self.assertEqual(EntityRelationship.objects.all().count(), 1)
         relationship = EntityRelationship.objects.first()
-        self.assertEquals(relationship.sub_entity, account_entity)
-        self.assertEquals(relationship.super_entity, team_entity)
+        self.assertEqual(relationship.sub_entity, account_entity)
+        self.assertEqual(relationship.super_entity, team_entity)
 
     def test_post_updated_entity_no_cascade(self):
         """
         Verify that updating a mirrored entity does not cause the entity to be deleted (which
         results in a cascading delete for all pointers.
         """
         # Create a test account
         account = Account.objects.create(email='test@test.com')
         entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(entity.entity_meta, {
+        self.assertEqual(entity.entity_meta, {
             'email': 'test@test.com',
             'is_captain': False,
             'team': None,
             'team_is_active': None,
         })
         old_entity_id = entity.id
 
@@ -820,119 +820,119 @@
         test_pointer = EntityPointer.objects.create(entity=entity)
 
         # Now update the account
         account.email = 'newemail@test.com'
         account.save()
         # Verify that the mirrored entity has the same ID
         entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(entity.entity_meta, {
+        self.assertEqual(entity.entity_meta, {
             'email': 'newemail@test.com',
             'is_captain': False,
             'team': None,
             'team_is_active': None,
         })
-        self.assertEquals(old_entity_id, entity.id)
+        self.assertEqual(old_entity_id, entity.id)
 
         # Verify that the pointer still exists and wasn't cascade deleted
         test_pointer = EntityPointer.objects.get(id=test_pointer.id)
-        self.assertEquals(test_pointer.entity, entity)
+        self.assertEqual(test_pointer.entity, entity)
 
     def test_post_update_account_meta(self):
         """
         Verifies that an account's metadata is updated properly in the mirrored tables.
         """
         # Create an account and check it's mirrored metadata
         account = Account.objects.create(email='test@test.com')
         entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(entity.entity_meta, {
+        self.assertEqual(entity.entity_meta, {
             'email': 'test@test.com',
             'is_captain': False,
             'team': None,
             'team_is_active': None,
         })
 
         # Update the account's metadata and check that it is mirrored
         account.email = 'newemail@test.com'
         account.save()
         entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(entity.entity_meta, {
+        self.assertEqual(entity.entity_meta, {
             'email': 'newemail@test.com',
             'is_captain': False,
             'team': None,
             'team_is_active': None,
         })
 
     def test_post_update_account_relationship_activity(self):
         """
         Creates an account that has super relationships. Verifies that the entity table is updated
         properly when changing the activity of a relationship.
         """
         # Verify that there are no entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
         # Create a team
         team = Team.objects.create(name='Team')
         # Create an account under that team
         account = Account.objects.create(email='test@test.com', team=team)
 
         # There should be two entities. Test their existence and values
-        self.assertEquals(Entity.objects.all().count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 2)
         account_entity = Entity.objects.get_for_obj(account)
-        self.assertEquals(account_entity.entity_meta, {
+        self.assertEqual(account_entity.entity_meta, {
             'email': 'test@test.com',
             'is_captain': False,
             'team': 'Team',
             'team_is_active': True,
         })
         team_entity = Entity.objects.get_for_obj(team)
-        self.assertEquals(team_entity.entity_meta, None)
+        self.assertEqual(team_entity.entity_meta, None)
 
         # Check that the appropriate entity relationship was created
-        self.assertEquals(EntityRelationship.objects.all().count(), 1)
+        self.assertEqual(EntityRelationship.objects.all().count(), 1)
         relationship = EntityRelationship.objects.first()
-        self.assertEquals(relationship.sub_entity, account_entity)
-        self.assertEquals(relationship.super_entity, team_entity)
+        self.assertEqual(relationship.sub_entity, account_entity)
+        self.assertEqual(relationship.super_entity, team_entity)
 
         # Update the account to be a team captain. According to our test project, this
         # means it no longer has an active relationship to a team
         account.is_captain = True
         account.save()
 
         # Verify that it no longer has an active relationship
-        self.assertEquals(EntityRelationship.objects.all().count(), 1)
+        self.assertEqual(EntityRelationship.objects.all().count(), 1)
         relationship = EntityRelationship.objects.first()
-        self.assertEquals(relationship.sub_entity, account_entity)
-        self.assertEquals(relationship.super_entity, team_entity)
+        self.assertEqual(relationship.sub_entity, account_entity)
+        self.assertEqual(relationship.super_entity, team_entity)
 
 
 class TestSyncingMultipleEntities(EntityTestCase):
     """
     Tests syncing multiple entities at once of different types.
     """
     def test_sync_two_accounts(self):
         turn_off_syncing()
         team = G(Team)
         account1 = G(Account, team=team)
         account2 = G(Account, team=team)
         G(TeamGroup)
         sync_entities(account1, account2)
 
-        self.assertEquals(Entity.objects.count(), 3)
-        self.assertEquals(EntityRelationship.objects.count(), 2)
+        self.assertEqual(Entity.objects.count(), 3)
+        self.assertEqual(EntityRelationship.objects.count(), 2)
 
     def test_sync_two_accounts_one_team_group(self):
         turn_off_syncing()
         team = G(Team)
         account1 = G(Account, team=team)
         account2 = G(Account, team=team)
         team_group = G(TeamGroup)
         sync_entities(account1, account2, team_group)
 
-        self.assertEquals(Entity.objects.count(), 4)
-        self.assertEquals(EntityRelationship.objects.count(), 2)
+        self.assertEqual(Entity.objects.count(), 4)
+        self.assertEqual(EntityRelationship.objects.count(), 2)
 
 
 class TestCachingAndCascading(EntityTestCase):
     """
     Tests caching, cascade syncing, and optimal queries when syncing single, multiple, or all entities.
     """
     def test_cascade_sync_super_entities(self):
@@ -942,16 +942,16 @@
         """
         turn_off_syncing()
         team = G(Team)
         turn_on_syncing()
 
         self.assertFalse(Entity.objects.exists())
         G(Account, team=team)
-        self.assertEquals(Entity.objects.count(), 2)
-        self.assertEquals(EntityRelationship.objects.count(), 1)
+        self.assertEqual(Entity.objects.count(), 2)
+        self.assertEqual(EntityRelationship.objects.count(), 1)
 
     def test_optimal_queries_registered_entity_with_no_qset(self):
         """
         Tests that the optimal number of queries are performed when syncing a single entity that
         did not register a queryset.
         """
         team_group = G(TeamGroup)
@@ -995,20 +995,20 @@
 
         with patch('entity.sync.entity_registry') as mock_entity_registry:
             mock_entity_registry.entity_registry = new_registry.entity_registry
             ContentType.objects.clear_cache()
             with self.assertNumQueries(20):
                 sync_entities()
 
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
-        self.assertEquals(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
-        self.assertEquals(Entity.objects.all().count(), 7)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Account)).count(), 5)
+        self.assertEqual(Entity.objects.filter(entity_type=ContentType.objects.get_for_model(Team)).count(), 2)
+        self.assertEqual(Entity.objects.all().count(), 7)
 
         # There should be four entity relationships since four accounts have teams
-        self.assertEquals(EntityRelationship.objects.all().count(), 4)
+        self.assertEqual(EntityRelationship.objects.all().count(), 4)
 
 
 class DeferEntitySyncingTests(EntityTestCase):
     """
     Tests the defer entity syncing decorator
     """
 
@@ -1019,30 +1019,30 @@
             for i in range(count):
                 Account.objects.create()
 
             if sync_all:
                 sync_entities()
 
             # Assert that we do not have any entities
-            test.assertEquals(Entity.objects.all().count(), 0)
+            test.assertEqual(Entity.objects.all().count(), 0)
 
         # Call the test method
         test_method(self, count=5)
 
         # Assert that after the method was run we did sync the entities
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
 
         # Delete all entities
         Entity.all_objects.all()._raw_delete(Entity.objects.db)
 
         # Call the method again syncing all
         test_method(self, count=0, sync_all=True)
 
         # Assert that after the method was run we did sync the entities
-        self.assertEquals(Entity.objects.all().count(), 5)
+        self.assertEqual(Entity.objects.all().count(), 5)
 
         # Assert that we restored the defer flag
         self.assertFalse(sync_entities.defer)
 
         # Assert that we cleared the buffer
         self.assertEqual(sync_entities.buffer, {})
 
@@ -1050,15 +1050,15 @@
         """
         Test the defer decorator when nothing is synced
         """
 
         @defer_entity_syncing
         def test_method(test):
             # Assert that we do not have any entities
-            test.assertEquals(Entity.objects.all().count(), 0)
+            test.assertEqual(Entity.objects.all().count(), 0)
 
         # Call the test method
         with patch('entity.sync.sync_entities') as mock_sync_entities:
             # Call the method that does no syncing
             test_method(self)
 
             # Ensure that we did not call sync entities
@@ -1074,21 +1074,21 @@
         @suppress_entity_syncing
         def test_method(test, count):
             # Create some entities
             for i in range(count):
                 Account.objects.create()
 
             # Assert that we do not have any entities
-            test.assertEquals(Entity.objects.all().count(), 0)
+            test.assertEqual(Entity.objects.all().count(), 0)
 
         # Call the test method
         test_method(self, count=5)
 
         # Assert that after the method was run we did sync the entities
-        self.assertEquals(Entity.objects.all().count(), 0)
+        self.assertEqual(Entity.objects.all().count(), 0)
 
         # Assert that we restored the suppress flag
         self.assertFalse(sync_entities.suppress)
 
 
 class TransactionAtomicWithRetryTests(EntityTestCase):
     """
```

### Comparing `django-entity-6.0.0/entity/tests/utils.py` & `django-entity-6.1.0/entity/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-entity-6.0.0/setup.py` & `django-entity-6.1.0/setup.py`

 * *Files 14% similar despite different names*

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
     install_requires=install_requires,
     tests_require=tests_require,
     extras_require={'dev': tests_require},
     test_suite='run_tests.run',
     include_package_data=True,
     zip_safe=False,
```

