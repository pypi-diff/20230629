# Comparing `tmp/django-entity-history-1.3.0.tar.gz` & `tmp/django-entity-history-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-entity-history-1.3.0.tar", last modified: Mon Nov 29 04:30:24 2021, max compression
+gzip compressed data, was "django-entity-history-2.0.0.tar", last modified: Thu Jun 29 18:22:54 2023, max compression
```

## Comparing `django-entity-history-1.3.0.tar` & `django-entity-history-2.0.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/
--rw-rw-r--   0 jared     (1000) jared     (1000)     1075 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/LICENSE
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/django_entity_history.egg-info/
--rw-rw-r--   0 jared     (1000) jared     (1000)     1911 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/SOURCES.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)        1 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/dependency_links.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)        1 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/not-zip-safe
--rw-rw-r--   0 jared     (1000) jared     (1000)       15 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/top_level.txt
--rw-rw-r--   0 jared     (1000) jared     (1000)     2209 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/PKG-INFO
--rw-rw-r--   0 jared     (1000) jared     (1000)       42 2021-11-29 04:30:23.000000 django-entity-history-1.3.0/django_entity_history.egg-info/requires.txt
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/entity_history/
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/entity_history/tests/
--rw-rw-r--   0 jared     (1000) jared     (1000)     2338 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/trigger_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)    24493 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/entity_history_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     5682 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/entity_relationship_activation_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     4871 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/entity_activation_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     3548 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/cascade_tests.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/tests/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/entity_history/sql/
--rw-rw-r--   0 jared     (1000) jared     (1000)      371 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/foreign_keys.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2094 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/triggers.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      613 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_trigger_create.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)     2285 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/foreign_keys_cascade_delete.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)       73 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_procedure_delete.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)      568 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_activation_trigger_create.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)     3423 2021-11-27 00:50:15.000000 django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_procedure_create.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)     3732 2021-11-27 00:56:57.000000 django-entity-history-1.3.0/entity_history/sql/entity_activation_procedure_create.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)      618 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_trigger_immediate_create.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/__init__.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/entity_history/sql/__pycache__/
--rw-r--r--   0 jared     (1000) jared     (1000)     2600 2021-11-27 00:52:30.000000 django-entity-history-1.3.0/entity_history/sql/__pycache__/triggers.cpython-36.pyc
--rw-r--r--   0 jared     (1000) jared     (1000)      155 2021-11-27 00:52:30.000000 django-entity-history-1.3.0/entity_history/sql/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 jared     (1000) jared     (1000)      859 2021-11-27 00:52:30.000000 django-entity-history-1.3.0/entity_history/sql/__pycache__/foreign_keys.cpython-36.pyc
--rw-rw-r--   0 jared     (1000) jared     (1000)       99 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_trigger_delete.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)       60 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_activation_procedure_delete.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)       74 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/sql/entity_activation_trigger_delete.sql
--rw-rw-r--   0 jared     (1000) jared     (1000)      145 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/apps.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     6332 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/models.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       37 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/urls.py
--rw-rw-r--   0 jared     (1000) jared     (1000)       22 2021-11-29 04:25:26.000000 django-entity-history-1.3.0/entity_history/version.py
-drwxrwxr-x   0 jared     (1000) jared     (1000)        0 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/entity_history/migrations/
--rw-rw-r--   0 jared     (1000) jared     (1000)      240 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/0002_auto_20150406_1605.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      251 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/0003_update_triggers.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     1148 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/0004_update_triggers_and_foreign_keys.py
--rw-rw-r--   0 jared     (1000) jared     (1000)        0 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/__init__.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2820 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/0005_auto_20180108_2021.py
--rw-rw-r--   0 jared     (1000) jared     (1000)     2222 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/migrations/0001_initial.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      113 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/entity_history/__init__.py
--rwxrwxr-x   0 jared     (1000) jared     (1000)     1710 2021-11-27 00:48:08.000000 django-entity-history-1.3.0/setup.py
--rw-rw-r--   0 jared     (1000) jared     (1000)      264 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/setup.cfg
--rw-rw-r--   0 jared     (1000) jared     (1000)     1192 2021-11-27 00:48:08.000000 django-entity-history-1.3.0/README.rst
--rw-rw-r--   0 jared     (1000) jared     (1000)       74 2021-11-27 00:47:44.000000 django-entity-history-1.3.0/MANIFEST.in
--rw-rw-r--   0 jared     (1000) jared     (1000)     2209 2021-11-29 04:30:24.000000 django-entity-history-1.3.0/PKG-INFO
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)      107 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1978 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1192 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/README.rst
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.836037 django-entity-history-2.0.0/django_entity_history.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1978 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1832 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)       41 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       15 2023-06-29 18:22:54.000000 django-entity-history-2.0.0/django_entity_history.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.836037 django-entity-history-2.0.0/entity_history/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       50 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      145 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/apps.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.836037 django-entity-history-2.0.0/entity_history/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2182 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      200 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/migrations/0002_auto_20150406_1605.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      211 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/migrations/0003_update_triggers.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1108 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/migrations/0004_update_triggers_and_foreign_keys.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2780 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/migrations/0005_auto_20180108_2021.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6332 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/entity_history/sql/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3732 2023-01-25 13:41:39.000000 django-entity-history-2.0.0/entity_history/sql/entity_activation_procedure_create.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)       60 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_activation_procedure_delete.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)      568 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_activation_trigger_create.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)       74 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_activation_trigger_delete.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3423 2023-01-25 13:41:39.000000 django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_procedure_create.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)       73 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_procedure_delete.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)      613 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_trigger_create.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)       99 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_trigger_delete.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)      618 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_trigger_immediate_create.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)      371 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/foreign_keys.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2285 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/foreign_keys_cascade_delete.sql
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2094 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/sql/triggers.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/entity_history/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     3548 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/cascade_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4871 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/entity_activation_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    24493 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/entity_history_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5682 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/entity_relationship_activation_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2338 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/tests/trigger_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/entity_history/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/entity_history/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       31 2023-01-09 15:25:40.000000 django-entity-history-2.0.0/requirements/docs.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       60 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       41 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      264 2023-06-29 18:22:54.840037 django-entity-history-2.0.0/setup.cfg
+-rwxrwxr-x   0 wes       (1000) wes       (1000)     1834 2023-06-29 18:18:27.000000 django-entity-history-2.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-entity-history-1.3.0/LICENSE` & `django-entity-history-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/django_entity_history.egg-info/SOURCES.txt` & `django-entity-history-2.0.0/django_entity_history.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 entity_history/sql/entity_relationship_activation_procedure_delete.sql
 entity_history/sql/entity_relationship_activation_trigger_create.sql
 entity_history/sql/entity_relationship_activation_trigger_delete.sql
 entity_history/sql/entity_relationship_activation_trigger_immediate_create.sql
 entity_history/sql/foreign_keys.py
 entity_history/sql/foreign_keys_cascade_delete.sql
 entity_history/sql/triggers.py
-entity_history/sql/__pycache__/__init__.cpython-36.pyc
-entity_history/sql/__pycache__/foreign_keys.cpython-36.pyc
-entity_history/sql/__pycache__/triggers.cpython-36.pyc
 entity_history/tests/__init__.py
 entity_history/tests/cascade_tests.py
 entity_history/tests/entity_activation_tests.py
 entity_history/tests/entity_history_tests.py
 entity_history/tests/entity_relationship_activation_tests.py
-entity_history/tests/trigger_tests.py
+entity_history/tests/trigger_tests.py
+requirements/docs.txt
+requirements/requirements-testing.txt
+requirements/requirements.txt
```

### Comparing `django-entity-history-1.3.0/django_entity_history.egg-info/PKG-INFO` & `django-entity-history-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-entity-history
-Version: 1.3.0
+Version: 2.0.0
 Summary: History about Django Entities
 Home-page: https://github.com/ambitioninc/django-entity-history
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-entity-history.png
-           :target: https://travis-ci.org/ambitioninc/django-entity-history
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/django-entity-history/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/django-entity-history?branch=develop
-        
-        .. image:: https://img.shields.io/pypi/v/django-entity-history.svg
-            :target: https://crate.io/packages/django-entity-history/
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-entity-history.svg
-            :target: https://crate.io/packages/django-entity-history/
-            :alt: Number of PyPI downloads
-        
-        
-        django-entity-history
-        =====================
-        
-        
-        I have failed to provide a good README.rst in my project, and you should shun
-        me if I do any pull requests
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-entity-history
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-entity-history.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-entity-history.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-entity-history.png
+   :target: https://travis-ci.org/ambitioninc/django-entity-history
+
+.. image:: https://coveralls.io/repos/ambitioninc/django-entity-history/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/django-entity-history?branch=develop
+
+.. image:: https://img.shields.io/pypi/v/django-entity-history.svg
+    :target: https://crate.io/packages/django-entity-history/
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-entity-history.svg
+    :target: https://crate.io/packages/django-entity-history/
+    :alt: Number of PyPI downloads
+
+
+django-entity-history
+=====================
+
+
+I have failed to provide a good README.rst in my project, and you should shun
+me if I do any pull requests
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-entity-history
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-entity-history.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-entity-history.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

### Comparing `django-entity-history-1.3.0/entity_history/tests/trigger_tests.py` & `django-entity-history-2.0.0/entity_history/tests/trigger_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/tests/entity_history_tests.py` & `django-entity-history-2.0.0/entity_history/tests/entity_history_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/tests/entity_relationship_activation_tests.py` & `django-entity-history-2.0.0/entity_history/tests/entity_relationship_activation_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/tests/entity_activation_tests.py` & `django-entity-history-2.0.0/entity_history/tests/entity_activation_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/tests/cascade_tests.py` & `django-entity-history-2.0.0/entity_history/tests/cascade_tests.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/triggers.py` & `django-entity-history-2.0.0/entity_history/sql/triggers.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_trigger_create.sql` & `django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_trigger_create.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/foreign_keys_cascade_delete.sql` & `django-entity-history-2.0.0/entity_history/sql/foreign_keys_cascade_delete.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/entity_activation_trigger_create.sql` & `django-entity-history-2.0.0/entity_history/sql/entity_activation_trigger_create.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_procedure_create.sql` & `django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_procedure_create.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/entity_activation_procedure_create.sql` & `django-entity-history-2.0.0/entity_history/sql/entity_activation_procedure_create.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/sql/entity_relationship_activation_trigger_immediate_create.sql` & `django-entity-history-2.0.0/entity_history/sql/entity_relationship_activation_trigger_immediate_create.sql`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/models.py` & `django-entity-history-2.0.0/entity_history/models.py`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/entity_history/migrations/0004_update_triggers_and_foreign_keys.py` & `django-entity-history-2.0.0/entity_history/migrations/0004_update_triggers_and_foreign_keys.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 
 from entity_history.sql.foreign_keys import EntityHistoryForeignKeys
 from entity_history.sql.triggers import (
     EntityActivationTrigger,
     EntityRelationshipActivationImmediateTrigger
```

### Comparing `django-entity-history-1.3.0/entity_history/migrations/0005_auto_20180108_2021.py` & `django-entity-history-2.0.0/entity_history/migrations/0005_auto_20180108_2021.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.11.9 on 2018-01-08 20:21
-from __future__ import unicode_literals
 
 import datetime
 from django.db import migrations, models
 from entity_history.sql.foreign_keys import EntityHistoryForeignKeys
 
 from entity_history.sql.triggers import EntityActivationTrigger, EntityRelationshipActivationImmediateTrigger
```

### Comparing `django-entity-history-1.3.0/entity_history/migrations/0001_initial.py` & `django-entity-history-2.0.0/entity_history/migrations/0001_initial.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-entity-history-1.3.0/setup.py` & `django-entity-history-2.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-import re
-from setuptools import setup, find_packages
-
 # import multiprocessing to avoid this bug (http://bugs.python.org/issue15881#msg170215)
 import multiprocessing
 assert multiprocessing
+import re
+from setuptools import setup, find_packages
 
 
 def get_version():
     """
     Extracts the version number from the version.py file.
     """
     VERSION_FILE = 'entity_history/version.py'
     mo = re.search(r'^__version__ = [\'"]([^\'"]*)[\'"]', open(VERSION_FILE, 'rt').read(), re.M)
     if mo:
         return mo.group(1)
     else:
         raise RuntimeError('Unable to find version string in {0}.'.format(VERSION_FILE))
 
 
+def get_lines(file_path):
+    return open(file_path, 'r').read().split('\n')
+
+
+install_requires = get_lines('requirements/requirements.txt')
+tests_require = get_lines('requirements/requirements-testing.txt')
+
 setup(
     name='django-entity-history',
     version=get_version(),
     description='History about Django Entities',
     long_description=open('README.rst').read(),
     url='https://github.com/ambitioninc/django-entity-history',
     author='Wes Kendall',
     author_email='opensource@ambition.com',
     keywords='',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Framework :: Django',
-        'Framework :: Django :: 2.0',
-        'Framework :: Django :: 2.1',
-        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Framework :: Django :: 4.1',
+        'Framework :: Django :: 4.2',
     ],
     license='MIT',
-    install_requires=[
-        'Django>=2.0',
-        'django-entity>=4.2.0',
-        'psycopg2'
-    ],
-    tests_require=[
-        'django-nose>=1.4',
-        'mock>=1.0.1',
-        'coverage>=3.7.1',
-        'django-dynamic-fixture',
-    ],
+    install_requires=install_requires,
+    tests_require=tests_require,
     test_suite='run_tests.run',
     include_package_data=True,
     zip_safe=False,
 )
```

### Comparing `django-entity-history-1.3.0/README.rst` & `django-entity-history-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-entity-history-1.3.0/PKG-INFO` & `django-entity-history-2.0.0/django_entity_history.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-entity-history
-Version: 1.3.0
+Version: 2.0.0
 Summary: History about Django Entities
 Home-page: https://github.com/ambitioninc/django-entity-history
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
-Description: .. image:: https://travis-ci.org/ambitioninc/django-entity-history.png
-           :target: https://travis-ci.org/ambitioninc/django-entity-history
-        
-        .. image:: https://coveralls.io/repos/ambitioninc/django-entity-history/badge.png?branch=develop
-            :target: https://coveralls.io/r/ambitioninc/django-entity-history?branch=develop
-        
-        .. image:: https://img.shields.io/pypi/v/django-entity-history.svg
-            :target: https://crate.io/packages/django-entity-history/
-            :alt: Latest PyPI version
-        
-        .. image:: https://img.shields.io/pypi/dm/django-entity-history.svg
-            :target: https://crate.io/packages/django-entity-history/
-            :alt: Number of PyPI downloads
-        
-        
-        django-entity-history
-        =====================
-        
-        
-        I have failed to provide a good README.rst in my project, and you should shun
-        me if I do any pull requests
-        
-        Installation
-        ------------
-        To install the latest release, type::
-        
-            pip install django-entity-history
-        
-        To install the latest code directly from source, type::
-        
-            pip install git+git://github.com/ambitioninc/django-entity-history.git
-        
-        Documentation
-        -------------
-        
-        Full documentation is available at http://django-entity-history.readthedocs.org
-        
-        License
-        -------
-        MIT License (see LICENSE)
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+License-File: LICENSE
+
+.. image:: https://travis-ci.org/ambitioninc/django-entity-history.png
+   :target: https://travis-ci.org/ambitioninc/django-entity-history
+
+.. image:: https://coveralls.io/repos/ambitioninc/django-entity-history/badge.png?branch=develop
+    :target: https://coveralls.io/r/ambitioninc/django-entity-history?branch=develop
+
+.. image:: https://img.shields.io/pypi/v/django-entity-history.svg
+    :target: https://crate.io/packages/django-entity-history/
+    :alt: Latest PyPI version
+
+.. image:: https://img.shields.io/pypi/dm/django-entity-history.svg
+    :target: https://crate.io/packages/django-entity-history/
+    :alt: Number of PyPI downloads
+
+
+django-entity-history
+=====================
+
+
+I have failed to provide a good README.rst in my project, and you should shun
+me if I do any pull requests
+
+Installation
+------------
+To install the latest release, type::
+
+    pip install django-entity-history
+
+To install the latest code directly from source, type::
+
+    pip install git+git://github.com/ambitioninc/django-entity-history.git
+
+Documentation
+-------------
+
+Full documentation is available at http://django-entity-history.readthedocs.org
+
+License
+-------
+MIT License (see LICENSE)
```

