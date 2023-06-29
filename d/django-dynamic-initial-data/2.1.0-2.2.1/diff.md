# Comparing `tmp/django-dynamic-initial-data-2.1.0.tar.gz` & `tmp/django-dynamic-initial-data-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-dynamic-initial-data-2.1.0.tar", last modified: Thu Jul 11 21:11:35 2019, max compression
+gzip compressed data, was "django-dynamic-initial-data-2.2.1.tar", last modified: Thu Jun 29 13:40:33 2023, max compression
```

## Comparing `django-dynamic-initial-data-2.1.0.tar` & `django-dynamic-initial-data-2.2.1.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/
--rwxr-xr-x   0 root         (0) root         (0)        1 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/dependency_links.txt
--rwxr-xr-x   0 root         (0) root         (0)     7267 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)       40 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/requires.txt
--rwxr-xr-x   0 root         (0) root         (0)     1326 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/SOURCES.txt
--rwxr-xr-x   0 root         (0) root         (0)       21 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/
--rwxr-xr-x   0 root         (0) root         (0)      168 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/apps.py
--rwxr-xr-x   0 root         (0) root         (0)    10684 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/base.py
--rwxr-xr-x   0 root         (0) root         (0)      891 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/commands/
--rwxr-xr-x   0 root         (0) root         (0)      834 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/commands/update_initial_data.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/commands/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/migrations/
--rwxr-xr-x   0 root         (0) root         (0)     1048 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      940 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/models.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/
--rwxr-xr-x   0 root         (0) root         (0)    14799 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/base_tests.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_1/
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_1/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_2/
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_2/fixtures/
--rwxr-xr-x   0 root         (0) root         (0)       62 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_2/fixtures/initial_data.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_2/fixtures/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/fake_app_2/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10862 2019-07-10 23:56:49.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/integration_tests.py
--rwxr-xr-x   0 root         (0) root         (0)     1026 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/management_command_tests.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2019-07-11 21:11:34.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/migrations/
--rwxr-xr-x   0 root         (0) root         (0)     1450 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      405 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/mocks.py
--rwxr-xr-x   0 root         (0) root         (0)      442 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/models.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       22 2019-07-10 23:56:55.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/version.py
--rwxr-xr-x   0 root         (0) root         (0)      127 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/dynamic_initial_data/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1095 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)       36 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/MANIFEST.in
--rwxr-xr-x   0 root         (0) root         (0)     7267 2019-07-11 21:11:35.000000 django-dynamic-initial-data-2.1.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     5660 2019-01-22 18:28:53.000000 django-dynamic-initial-data-2.1.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)      197 2019-07-11 21:11:35.000000 django-dynamic-initial-data-2.1.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1778 2019-07-11 18:47:13.000000 django-dynamic-initial-data-2.1.0/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       67 2023-06-29 13:37:35.000000 django-dynamic-initial-data-2.2.1/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6412 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5543 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6412 2023-06-29 13:40:33.000000 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1423 2023-06-29 13:40:33.000000 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 13:40:33.000000 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-29 13:40:33.000000 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       21 2023-06-29 13:40:33.000000 django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       49 2023-06-28 22:41:39.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      162 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    10684 2021-05-03 22:29:54.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/base.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      866 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/exceptions.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/commands/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/commands/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      811 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/commands/update_initial_data.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      977 2023-06-28 22:41:39.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      916 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/models.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    14767 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/base_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_1/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_1/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.428846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_2/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_2/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_2/fixtures/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_2/fixtures/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       61 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/fake_app_2/fixtures/initial_data.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    10843 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/integration_tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1009 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/management_command_tests.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1363 2023-06-28 22:41:39.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      381 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/mocks.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      418 2021-05-03 22:00:12.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 13:37:35.000000 django-dynamic-initial-data-2.2.1/dynamic_initial_data/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       70 2023-06-28 22:38:44.000000 django-dynamic-initial-data-2.2.1/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       63 2023-06-28 22:39:12.000000 django-dynamic-initial-data-2.2.1/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      197 2023-06-29 13:40:33.432846 django-dynamic-initial-data-2.2.1/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1909 2023-06-28 22:43:42.000000 django-dynamic-initial-data-2.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/PKG-INFO` & `django-dynamic-initial-data-2.2.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,142 @@
 Metadata-Version: 2.1
 Name: django-dynamic-initial-data
-Version: 2.1.0
+Version: 2.2.1
 Summary: Dynamic initial data fixtures for Django apps
 Home-page: https://github.com/ambitioninc/django-dynamic-initial-data
 Author: 
 Author-email: opensource@ambition.com
 License: MIT
-Description: [![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
-        
-        ## Django Initial Data
-        
-        Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
-        dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
-        can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
-        deleted from initial data, a feature that Django's initial data fixture system lacks.
-        
-        ## Table of Contents
-        
-        1. [Installation] (#installation)
-        2. [A Brief Overview] (#a-brief-overview)
-        3. [Example] (#example)
-        4. [Handling Deletions](#handling-deletions)
-        
-        ## Installation
-        To install Django Dynamic Initial Data:
-        
-        ```shell
-        pip install django-dynamic-initial-data
-        ```
-        
-        Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
-        
-        settings.py
-        ```python
-        INSTALLED_APPS = (
-            'dynamic_initial_data',
-        )
-        ```
-        
-        ## A Brief Overview
-        
-        A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
-        command is intended to be called as part of the deployment process of your app. Any missing dependencies
-        will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
-        `InitialDataCircularDependency` exception.
-        
-        Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
-        directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
-        the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
-        that inherits from `BaseInitialData`.
-        
-        When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
-        If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
-        
-        Any dependencies should be included in a list called `dependencies`. Each dependency is a string
-        of the app name as defined in `INSTALLED_APPS`.
-        
-        ## Example:
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            dependencies = ['my_first_app', 'my.second.app']
-        
-            def update_initial_data(self):
-                model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
-        
-                TestModel.objects.bulk_upsert([
-                    TestModel(float_field=1.0, char_field='1', int_field=1),
-                    TestModel(float_field=2.0, char_field='2', int_field=2),
-                    TestModel(float_field=3.0, char_field='3', int_field=3),
-                ], ['int_field'], ['char_field'])
-        ```
-        In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
-        and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
-        
-        ```
-        python manage.py update_initial_data
-        ```
-        
-        Similarly, to only initialize a single app, use
-        
-        ```
-        python manage.py update_initial_data --app 'app_path'
-        ```
-        
-        Documentation on using `upsert` and `bulk_upsert` can be found below:
-        - https://github.com/ambitioninc/django-manager-utils#upsert
-        - https://github.com/ambitioninc/django-manager-utils#bulk_upsert
-        
-        ## Handling Deletions
-        One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
-        
-        Django Dynamic Initial Data fixes this problem by allowing the user to either:
-        
-        1. Return all managed initial data objects as an array from the update_initial_data function.
-        2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
-        
-        Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            def update_initial_data(self):
-                hello = Account.objects.get_or_create(name='hello')
-                world = Account.objects.get_or_create(name='world')
-                # register the accounts for deletion
-                self.register_for_deletion(hello, world)
-        ```
-        
-        After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            def update_initial_data(self):
-                world = Account.objects.get_or_create(name='world')
-                # register the accounts for deletion
-                self.register_for_deletion(world)
-        ```
-        
-        When this piece of code executes, the previous "hello" account would then be deleted since the initial data process no longer owns it. And don't worry, if it was already deleted by another process, the deletion will not throw an error.
 Keywords: Django fixtures
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
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
+
+## Django Initial Data
+
+Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
+dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
+can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
+deleted from initial data, a feature that Django's initial data fixture system lacks.
+
+## Table of Contents
+
+1. [Installation] (#installation)
+2. [A Brief Overview] (#a-brief-overview)
+3. [Example] (#example)
+4. [Handling Deletions](#handling-deletions)
+
+## Installation
+To install Django Dynamic Initial Data:
+
+```shell
+pip install django-dynamic-initial-data
+```
+
+Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
+
+settings.py
+```python
+INSTALLED_APPS = (
+    'dynamic_initial_data',
+)
+```
+
+## A Brief Overview
+
+A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
+command is intended to be called as part of the deployment process of your app. Any missing dependencies
+will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
+`InitialDataCircularDependency` exception.
+
+Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
+directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
+the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
+that inherits from `BaseInitialData`.
+
+When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
+If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
+
+Any dependencies should be included in a list called `dependencies`. Each dependency is a string
+of the app name as defined in `INSTALLED_APPS`.
+
+## Example:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    dependencies = ['my_first_app', 'my.second.app']
+
+    def update_initial_data(self):
+        model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
+
+        TestModel.objects.bulk_upsert([
+            TestModel(float_field=1.0, char_field='1', int_field=1),
+            TestModel(float_field=2.0, char_field='2', int_field=2),
+            TestModel(float_field=3.0, char_field='3', int_field=3),
+        ], ['int_field'], ['char_field'])
+```
+In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
+and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
+
+```
+python manage.py update_initial_data
+```
+
+Similarly, to only initialize a single app, use
+
+```
+python manage.py update_initial_data --app 'app_path'
+```
+
+Documentation on using `upsert` and `bulk_upsert` can be found below:
+- https://github.com/ambitioninc/django-manager-utils#upsert
+- https://github.com/ambitioninc/django-manager-utils#bulk_upsert
+
+## Handling Deletions
+One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
+
+Django Dynamic Initial Data fixes this problem by allowing the user to either:
+
+1. Return all managed initial data objects as an array from the update_initial_data function.
+2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
+
+Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        hello = Account.objects.get_or_create(name='hello')
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(hello, world)
+```
+
+After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(world)
+```
+
+When this piece of code executes, the previous "hello" account would then be deleted since the initial data process no longer owns it. And don't worry, if it was already deleted by another process, the deletion will not throw an error.
```

### Comparing `django-dynamic-initial-data-2.1.0/django_dynamic_initial_data.egg-info/SOURCES.txt` & `django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 django_dynamic_initial_data.egg-info/requires.txt
 django_dynamic_initial_data.egg-info/top_level.txt
 dynamic_initial_data/__init__.py
 dynamic_initial_data/apps.py
 dynamic_initial_data/base.py
 dynamic_initial_data/exceptions.py
 dynamic_initial_data/models.py
+dynamic_initial_data/urls.py
 dynamic_initial_data/version.py
 dynamic_initial_data/management/__init__.py
 dynamic_initial_data/management/commands/__init__.py
 dynamic_initial_data/management/commands/update_initial_data.py
 dynamic_initial_data/migrations/0001_initial.py
 dynamic_initial_data/migrations/__init__.py
 dynamic_initial_data/tests/__init__.py
@@ -26,8 +27,10 @@
 dynamic_initial_data/tests/mocks.py
 dynamic_initial_data/tests/models.py
 dynamic_initial_data/tests/fake_app_1/__init__.py
 dynamic_initial_data/tests/fake_app_2/__init__.py
 dynamic_initial_data/tests/fake_app_2/fixtures/__init__.py
 dynamic_initial_data/tests/fake_app_2/fixtures/initial_data.py
 dynamic_initial_data/tests/migrations/0001_initial.py
-dynamic_initial_data/tests/migrations/__init__.py
+dynamic_initial_data/tests/migrations/__init__.py
+requirements/requirements-testing.txt
+requirements/requirements.txt
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/base.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/base.py`

 * *Files identical despite different names*

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/exceptions.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-00000000: 0d0a 636c 6173 7320 496e 6974 6961 6c44  ..class InitialD
-00000010: 6174 6143 6972 6375 6c61 7244 6570 656e  ataCircularDepen
-00000020: 6465 6e63 7928 4578 6365 7074 696f 6e29  dency(Exception)
-00000030: 3a0d 0a20 2020 2022 2222 0d0a 2020 2020  :..    """..    
-00000040: 5261 6973 6564 2077 6865 6e20 6120 6369  Raised when a ci
-00000050: 7263 756c 6172 2064 6570 656e 6465 6e63  rcular dependenc
-00000060: 7920 6973 2064 6574 6563 7465 642e 0d0a  y is detected...
-00000070: 2020 2020 2222 220d 0a20 2020 2064 6566      """..    def
-00000080: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
-00000090: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-000000a0: 3a0d 0a20 2020 2020 2020 2064 6570 203d  :..        dep =
-000000b0: 206b 7761 7267 732e 6765 7428 2764 6570   kwargs.get('dep
-000000c0: 2729 0d0a 2020 2020 2020 2020 6361 6c6c  ')..        call
-000000d0: 5f6c 6973 7420 3d20 6b77 6172 6773 2e67  _list = kwargs.g
-000000e0: 6574 2827 6361 6c6c 5f6c 6973 7427 290d  et('call_list').
-000000f0: 0a20 2020 2020 2020 2063 616c 6c5f 6c69  .        call_li
-00000100: 7374 202b 3d20 5b64 6570 5d0d 0a20 2020  st += [dep]..   
-00000110: 2020 2020 2063 616c 6c5f 6c69 6e65 7320       call_lines 
-00000120: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-00000130: 2027 7b30 7d7b 317d 272e 666f 726d 6174   '{0}{1}'.format
-00000140: 2827 2d2d 2720 2a20 692c 2069 7465 6d29  ('--' * i, item)
-00000150: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00000160: 7220 692c 2069 7465 6d20 696e 2065 6e75  r i, item in enu
-00000170: 6d65 7261 7465 2863 616c 6c5f 6c69 7374  merate(call_list
-00000180: 290d 0a20 2020 2020 2020 205d 0d0a 2020  )..        ]..  
-00000190: 2020 2020 2020 6572 726f 725f 7374 7220        error_str 
-000001a0: 3d20 2743 6972 6375 6c61 7220 6465 7065  = 'Circular depe
-000001b0: 6e64 656e 6379 2066 6f75 6e64 5c6e 7b30  ndency found\n{0
-000001c0: 7d27 2e66 6f72 6d61 7428 275c 6e27 2e6a  }'.format('\n'.j
-000001d0: 6f69 6e28 6361 6c6c 5f6c 696e 6573 2929  oin(call_lines))
-000001e0: 0d0a 2020 2020 2020 2020 7375 7065 7228  ..        super(
-000001f0: 496e 6974 6961 6c44 6174 6143 6972 6375  InitialDataCircu
-00000200: 6c61 7244 6570 656e 6465 6e63 792c 2073  larDependency, s
-00000210: 656c 6629 2e5f 5f69 6e69 745f 5f28 6572  elf).__init__(er
-00000220: 726f 725f 7374 7229 0d0a 0d0a 0d0a 636c  ror_str)......cl
-00000230: 6173 7320 496e 6974 6961 6c44 6174 614d  ass InitialDataM
-00000240: 6973 7369 6e67 4170 7028 4578 6365 7074  issingApp(Except
-00000250: 696f 6e29 3a0d 0a20 2020 2022 2222 0d0a  ion):..    """..
-00000260: 2020 2020 5261 6973 6564 2077 6865 6e20      Raised when 
-00000270: 6120 7370 6563 6966 6965 6420 6170 7020  a specified app 
-00000280: 6361 6e6e 6f74 2062 6520 6c6f 6164 6564  cannot be loaded
-00000290: 2062 6563 6175 7365 2069 7420 646f 6573   because it does
-000002a0: 206e 6f74 2065 7869 7374 2e0d 0a20 2020   not exist...   
-000002b0: 2022 2222 0d0a 2020 2020 6465 6620 5f5f   """..    def __
-000002c0: 696e 6974 5f5f 2873 656c 662c 202a 6172  init__(self, *ar
-000002d0: 6773 2c20 2a2a 6b77 6172 6773 293a 0d0a  gs, **kwargs):..
-000002e0: 2020 2020 2020 2020 6465 7020 3d20 6b77          dep = kw
-000002f0: 6172 6773 2e67 6574 2827 6465 7027 290d  args.get('dep').
-00000300: 0a20 2020 2020 2020 2065 7272 6f72 5f73  .        error_s
-00000310: 7472 203d 2027 4d69 7373 696e 6720 6465  tr = 'Missing de
-00000320: 7065 6e64 656e 6379 207b 307d 272e 666f  pendency {0}'.fo
-00000330: 726d 6174 2864 6570 290d 0a20 2020 2020  rmat(dep)..     
-00000340: 2020 2073 7570 6572 2849 6e69 7469 616c     super(Initial
-00000350: 4461 7461 4d69 7373 696e 6741 7070 2c20  DataMissingApp, 
-00000360: 7365 6c66 292e 5f5f 696e 6974 5f5f 2865  self).__init__(e
-00000370: 7272 6f72 5f73 7472 290d 0a              rror_str)..
+00000000: 0a63 6c61 7373 2049 6e69 7469 616c 4461  .class InitialDa
+00000010: 7461 4369 7263 756c 6172 4465 7065 6e64  taCircularDepend
+00000020: 656e 6379 2845 7863 6570 7469 6f6e 293a  ency(Exception):
+00000030: 0a20 2020 2022 2222 0a20 2020 2052 6169  .    """.    Rai
+00000040: 7365 6420 7768 656e 2061 2063 6972 6375  sed when a circu
+00000050: 6c61 7220 6465 7065 6e64 656e 6379 2069  lar dependency i
+00000060: 7320 6465 7465 6374 6564 2e0a 2020 2020  s detected..    
+00000070: 2222 220a 2020 2020 6465 6620 5f5f 696e  """.    def __in
+00000080: 6974 5f5f 2873 656c 662c 202a 6172 6773  it__(self, *args
+00000090: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+000000a0: 2020 2020 2064 6570 203d 206b 7761 7267       dep = kwarg
+000000b0: 732e 6765 7428 2764 6570 2729 0a20 2020  s.get('dep').   
+000000c0: 2020 2020 2063 616c 6c5f 6c69 7374 203d       call_list =
+000000d0: 206b 7761 7267 732e 6765 7428 2763 616c   kwargs.get('cal
+000000e0: 6c5f 6c69 7374 2729 0a20 2020 2020 2020  l_list').       
+000000f0: 2063 616c 6c5f 6c69 7374 202b 3d20 5b64   call_list += [d
+00000100: 6570 5d0a 2020 2020 2020 2020 6361 6c6c  ep].        call
+00000110: 5f6c 696e 6573 203d 205b 0a20 2020 2020  _lines = [.     
+00000120: 2020 2020 2020 2027 7b30 7d7b 317d 272e         '{0}{1}'.
+00000130: 666f 726d 6174 2827 2d2d 2720 2a20 692c  format('--' * i,
+00000140: 2069 7465 6d29 0a20 2020 2020 2020 2020   item).         
+00000150: 2020 2066 6f72 2069 2c20 6974 656d 2069     for i, item i
+00000160: 6e20 656e 756d 6572 6174 6528 6361 6c6c  n enumerate(call
+00000170: 5f6c 6973 7429 0a20 2020 2020 2020 205d  _list).        ]
+00000180: 0a20 2020 2020 2020 2065 7272 6f72 5f73  .        error_s
+00000190: 7472 203d 2027 4369 7263 756c 6172 2064  tr = 'Circular d
+000001a0: 6570 656e 6465 6e63 7920 666f 756e 645c  ependency found\
+000001b0: 6e7b 307d 272e 666f 726d 6174 2827 5c6e  n{0}'.format('\n
+000001c0: 272e 6a6f 696e 2863 616c 6c5f 6c69 6e65  '.join(call_line
+000001d0: 7329 290a 2020 2020 2020 2020 7375 7065  s)).        supe
+000001e0: 7228 496e 6974 6961 6c44 6174 6143 6972  r(InitialDataCir
+000001f0: 6375 6c61 7244 6570 656e 6465 6e63 792c  cularDependency,
+00000200: 2073 656c 6629 2e5f 5f69 6e69 745f 5f28   self).__init__(
+00000210: 6572 726f 725f 7374 7229 0a0a 0a63 6c61  error_str)...cla
+00000220: 7373 2049 6e69 7469 616c 4461 7461 4d69  ss InitialDataMi
+00000230: 7373 696e 6741 7070 2845 7863 6570 7469  ssingApp(Excepti
+00000240: 6f6e 293a 0a20 2020 2022 2222 0a20 2020  on):.    """.   
+00000250: 2052 6169 7365 6420 7768 656e 2061 2073   Raised when a s
+00000260: 7065 6369 6669 6564 2061 7070 2063 616e  pecified app can
+00000270: 6e6f 7420 6265 206c 6f61 6465 6420 6265  not be loaded be
+00000280: 6361 7573 6520 6974 2064 6f65 7320 6e6f  cause it does no
+00000290: 7420 6578 6973 742e 0a20 2020 2022 2222  t exist..    """
+000002a0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000002b0: 5f28 7365 6c66 2c20 2a61 7267 732c 202a  _(self, *args, *
+000002c0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+000002d0: 2020 6465 7020 3d20 6b77 6172 6773 2e67    dep = kwargs.g
+000002e0: 6574 2827 6465 7027 290a 2020 2020 2020  et('dep').      
+000002f0: 2020 6572 726f 725f 7374 7220 3d20 274d    error_str = 'M
+00000300: 6973 7369 6e67 2064 6570 656e 6465 6e63  issing dependenc
+00000310: 7920 7b30 7d27 2e66 6f72 6d61 7428 6465  y {0}'.format(de
+00000320: 7029 0a20 2020 2020 2020 2073 7570 6572  p).        super
+00000330: 2849 6e69 7469 616c 4461 7461 4d69 7373  (InitialDataMiss
+00000340: 696e 6741 7070 2c20 7365 6c66 292e 5f5f  ingApp, self).__
+00000350: 696e 6974 5f5f 2865 7272 6f72 5f73 7472  init__(error_str
+00000360: 290a                                     ).
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/management/commands/update_initial_data.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/management/commands/update_initial_data.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from django.core.management.base import BaseCommand
-
-from dynamic_initial_data.base import InitialDataUpdater
-
-
-class Command(BaseCommand):
-    def add_arguments(self, parser):
-        parser.add_argument(
-            '--verbose', action='store_true', dest='verbose', default=False,
-            help='Determines if we should display which apps are being updated'
-        )
-        parser.add_argument(
-            '--app', dest='app', default=None, help='Updates a single app'
-        )
-
-    help = 'Call the InitialData.update_initial_data command for all apps. Use --app to update only one app.'
-
-    def handle(self, *args, **options):
-        updater = InitialDataUpdater(options)
-        if options['app']:
-            updater.update_app(options['app'])
-        else:
-            updater.update_all_apps()
+from django.core.management.base import BaseCommand
+
+from dynamic_initial_data.base import InitialDataUpdater
+
+
+class Command(BaseCommand):
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '--verbose', action='store_true', dest='verbose', default=False,
+            help='Determines if we should display which apps are being updated'
+        )
+        parser.add_argument(
+            '--app', dest='app', default=None, help='Updates a single app'
+        )
+
+    help = 'Call the InitialData.update_initial_data command for all apps. Use --app to update only one app.'
+
+    def handle(self, *args, **options):
+        updater = InitialDataUpdater(options)
+        if options['app']:
+            updater.update_app(options['app'])
+        else:
+            updater.update_all_apps()
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/models.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/models.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from django.contrib.contenttypes.fields import GenericForeignKey
-from django.contrib.contenttypes.models import ContentType
-from django.db import models
-from manager_utils import ManagerUtilsManager
-
-
-class RegisteredForDeletionReceipt(models.Model):
-    """
-    Specifies a receipt of a model object that was registered for deletion by the dynamic
-    initial data process.
-    """
-    # The model object that was registered
-    model_obj_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
-    model_obj_id = models.PositiveIntegerField()
-    model_obj = GenericForeignKey('model_obj_type', 'model_obj_id', for_concrete_model=False)
-
-    # The time at which it was registered for deletion
-    register_time = models.DateTimeField()
-
-    # Use manager utils for bulk updating capabilities
-    objects = ManagerUtilsManager()
-
-    class Meta:
-        unique_together = ('model_obj_type', 'model_obj_id')
+from django.contrib.contenttypes.fields import GenericForeignKey
+from django.contrib.contenttypes.models import ContentType
+from django.db import models
+from manager_utils import ManagerUtilsManager
+
+
+class RegisteredForDeletionReceipt(models.Model):
+    """
+    Specifies a receipt of a model object that was registered for deletion by the dynamic
+    initial data process.
+    """
+    # The model object that was registered
+    model_obj_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
+    model_obj_id = models.PositiveIntegerField()
+    model_obj = GenericForeignKey('model_obj_type', 'model_obj_id', for_concrete_model=False)
+
+    # The time at which it was registered for deletion
+    register_time = models.DateTimeField()
+
+    # Use manager utils for bulk updating capabilities
+    objects = ManagerUtilsManager()
+
+    class Meta:
+        unique_together = ('model_obj_type', 'model_obj_id')
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/base_tests.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/base_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from django.contrib.contenttypes.models import ContentType
 from django.db import transaction
 from django.test import TestCase, TransactionTestCase
 from django.test.utils import override_settings
 from django_dynamic_fixture import G
 from freezegun import freeze_time
-from mock import patch
+from unittest.mock import patch
 
 from dynamic_initial_data.base import BaseInitialData, InitialDataUpdater
 from dynamic_initial_data.exceptions import InitialDataMissingApp, InitialDataCircularDependency
 from dynamic_initial_data.models import RegisteredForDeletionReceipt
 from dynamic_initial_data.tests.mocks import MockInitialData, MockClass, MockOne, MockTwo, MockThree
 from dynamic_initial_data.tests.models import Account, ProxyAccount, CantCascadeModel, RelModel
 
@@ -27,25 +27,25 @@
     def test_register_for_deletion_one_arg(self):
         """
         Tests the register_for_deletion_function with one argument.
         """
         initial_data = BaseInitialData()
         account = G(Account)
         initial_data.register_for_deletion(account)
-        self.assertEquals(initial_data.get_model_objs_registered_for_deletion(), [account])
+        self.assertEqual(initial_data.get_model_objs_registered_for_deletion(), [account])
 
     def test_register_for_deletion_multiple_args(self):
         """
         Tests the register_for_deletion_function with multiple arguments.
         """
         initial_data = BaseInitialData()
         account1 = G(Account)
         account2 = G(Account)
         initial_data.register_for_deletion(account1, account2)
-        self.assertEquals(initial_data.get_model_objs_registered_for_deletion(), [account1, account2])
+        self.assertEqual(initial_data.get_model_objs_registered_for_deletion(), [account1, account2])
 
 
 class TestInvalidDeletions(TransactionTestCase):
     def test_cant_delete_obj_in_receipt(self):
         """
         Tests when the object in the receipt cant be deleted such as a deleted content type
         or another model that cant be cascaded.
@@ -55,18 +55,18 @@
         G(CantCascadeModel, rel_model=rel_model)
         RegisteredForDeletionReceipt.objects.create(model_obj=rel_model, register_time=datetime(2013, 4, 5))
 
         account = G(Account)
         RegisteredForDeletionReceipt.objects.create(model_obj=account, register_time=datetime(2013, 4, 5))
         initial_data_updater.model_objs_registered_for_deletion = []
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 2)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 2)
         with transaction.atomic():
             initial_data_updater.handle_deletions()
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
 
 
 class TestHandleDeletions(TestCase):
     """
     Tests the handle_deletions functionality in the InitialDataUpater class.
     """
     def setUp(self):
@@ -82,134 +82,134 @@
     def test_create_one_obj(self):
         """
         Tests creating one object to handle for deletion.
         """
         account = G(Account)
         self.initial_data_updater.model_objs_registered_for_deletion = [account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
         receipt = RegisteredForDeletionReceipt.objects.get()
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
     def test_create_dup_objs(self):
         """
         Tests creating duplicate objects for deletion.
         """
         account = G(Account)
         self.initial_data_updater.model_objs_registered_for_deletion = [account, account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
         receipt = RegisteredForDeletionReceipt.objects.get()
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
     def test_create_dup_proxy_objs(self):
         """
         Tests creating duplicate objects for deletion when one is a proxy of another.
         """
         account = G(Account)
         proxy_account = ProxyAccount.objects.get(id=account.id)
         self.initial_data_updater.model_objs_registered_for_deletion = [account, account, proxy_account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 2)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 2)
 
         receipt = RegisteredForDeletionReceipt.objects.get(model_obj_type=ContentType.objects.get_for_model(account))
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
         receipt = RegisteredForDeletionReceipt.objects.get(
             model_obj_type=ContentType.objects.get_for_model(proxy_account, for_concrete_model=False))
-        self.assertEquals(
+        self.assertEqual(
             receipt.model_obj_type, ContentType.objects.get_for_model(ProxyAccount, for_concrete_model=False))
-        self.assertEquals(receipt.model_obj_id, proxy_account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_id, proxy_account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
     def test_create_delete_one_obj(self):
         """
         Tests creating one object to handle for deletion and then deleting it.
         """
         account = G(Account)
         self.initial_data_updater.model_objs_registered_for_deletion = [account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
         receipt = RegisteredForDeletionReceipt.objects.get()
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
         # Now, don't register the object for deletion and run it again at a different time
         self.initial_data_updater.model_objs_registered_for_deletion = []
         with freeze_time('2013-04-12 05:00:00'):
             self.initial_data_updater.handle_deletions()
         # The object should be deleted, along with its receipt
-        self.assertEquals(Account.objects.count(), 0)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
 
     def test_create_update_one_obj(self):
         """
         Tests creating one object to handle for deletion and then updating it.
         """
         account = G(Account)
         self.initial_data_updater.model_objs_registered_for_deletion = [account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
         receipt = RegisteredForDeletionReceipt.objects.get()
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
         # Run the deletion handler again at a different time. It should not delete the object
         with freeze_time('2013-04-12 05:00:00'):
             self.initial_data_updater.handle_deletions()
         # The object should not be deleted, along with its receipt
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.get().register_time, datetime(2013, 4, 12, 5))
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.get().register_time, datetime(2013, 4, 12, 5))
 
     def test_delete_already_deleted_obj(self):
         """
         Tests the case when an object that was registered for deletion has already been deleted.
         """
         account = G(Account)
         self.initial_data_updater.model_objs_registered_for_deletion = [account]
 
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
         with freeze_time('2013-04-12'):
             self.initial_data_updater.handle_deletions()
         receipt = RegisteredForDeletionReceipt.objects.get()
-        self.assertEquals(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
-        self.assertEquals(receipt.model_obj_id, account.id)
-        self.assertEquals(receipt.register_time, datetime(2013, 4, 12))
+        self.assertEqual(receipt.model_obj_type, ContentType.objects.get_for_model(Account))
+        self.assertEqual(receipt.model_obj_id, account.id)
+        self.assertEqual(receipt.register_time, datetime(2013, 4, 12))
 
         # Delete the model object. The receipt should still exist
         account.delete()
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
 
         # Now, don't register the object for deletion and run it again at a different time
         self.initial_data_updater.model_objs_registered_for_deletion = []
         with freeze_time('2013-04-12 05:00:00'):
             self.initial_data_updater.handle_deletions()
         # The object should be deleted, along with its receipt
-        self.assertEquals(Account.objects.count(), 0)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
 
 
 class InitialDataUpdaterTest(TestCase):
     """
     Tests the functionality of the InitialDataUpdater
     """
     def test_verbose_option(self):
@@ -234,15 +234,15 @@
         """
         Tests that the cache is hit since import is only called once.
         """
         initial_data_updater = InitialDataUpdater()
         initial_data_updater.load_app('fake')
         initial_data_updater.load_app('fake')
         initial_data_updater.load_app('fake')
-        self.assertEquals(import_patch.call_count, 1)
+        self.assertEqual(import_patch.call_count, 1)
 
     @patch('dynamic_initial_data.base.import_string', return_value=MockClass)
     def test_load_app_doesnt_exist(self, import_patch):
         """
         Tests the load_app method on an app that doesnt exist
         """
         self.assertIsNone(InitialDataUpdater().load_app('fake'))
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/integration_tests.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/integration_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from django.test import TestCase
 from django.core.management import call_command
-from mock import patch
+from unittest.mock import patch
 
 from dynamic_initial_data.base import BaseInitialData, InitialDataUpdater
 from dynamic_initial_data.models import RegisteredForDeletionReceipt
 from dynamic_initial_data.tests.models import Account
 
 
 class IntegrationTest(TestCase):
@@ -17,23 +17,23 @@
         Tests creating a test account in the initial data process.
         """
         class AccountInitialData(BaseInitialData):
             def update_initial_data(self):
                 Account.objects.get_or_create()
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData) as load_app_mock:
             InitialDataUpdater().update_app('test_app')
             # It should be called twice - once for initial loading, and twice for dependency testing
-            self.assertEquals(load_app_mock.call_count, 2)
+            self.assertEqual(load_app_mock.call_count, 2)
 
         # Verify an account object was created
-        self.assertEquals(Account.objects.count(), 1)
+        self.assertEqual(Account.objects.count(), 1)
 
     def test_multiple_same_objects(self):
         """
         Tests initial data when registering the same object for deletion twice.
         """
         class AccountInitialData1(BaseInitialData):
             """
@@ -41,23 +41,23 @@
             """
             def update_initial_data(self):
                 # Return the object from update_initial_data, thus registering it for deletion
                 account = Account.objects.get_or_create()[0]
                 return [account, account, account]
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData1):
             InitialDataUpdater().update_all_apps()
             InitialDataUpdater().update_all_apps()
 
         # Verify an account object was created and is managed by a deletion receipt
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
 
     def test_handle_deletions_returned_from_update_initial_data(self):
         """
         Tests handling of deletions when they are returned from the update_initial_data function.
         """
         class AccountInitialData1(BaseInitialData):
             """
@@ -73,31 +73,31 @@
             The initial data code the second time it is called. It no longer creates the account object, so the
             previously created account object should be deleted.
             """
             def update_initial_data(self):
                 pass
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData1):
             InitialDataUpdater().update_all_apps()
 
         # Verify an account object was created and is managed by a deletion receipt
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
 
         # Run the initial data process again, this time not registering the account for
         # deletion. It should be deleted.
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData2):
             InitialDataUpdater().update_all_apps()
 
         # Verify there are no accounts or receipts
-        self.assertEquals(Account.objects.count(), 0)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
 
     def test_handle_deletions_updates_returned_from_update_initial_data(self):
         """
         Tests handling of deletions and updates when they are returned from the update_initial_data function.
         """
         class AccountInitialData1(BaseInitialData):
             """
@@ -112,31 +112,31 @@
             """
             The initial data code the second time it is called. It only manages one of the previous accounts
             """
             def update_initial_data(self):
                 return [Account.objects.get_or_create(name='hi')[0]]
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData1):
             InitialDataUpdater().update_all_apps()
 
         # Verify two account objects were created and are managed by deletion receipts
-        self.assertEquals(Account.objects.count(), 2)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 2)
+        self.assertEqual(Account.objects.count(), 2)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 2)
 
         # Run the initial data process again, this time deleting the account named 'hi2'
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData2):
             InitialDataUpdater().update_all_apps()
 
         # Verify only the 'hi' account exists
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.get().model_obj.name, 'hi')
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.get().model_obj.name, 'hi')
 
     def test_handle_deletions_registered_from_update_initial_data(self):
         """
         Tests handling of deletions when they are programmatically registered from the update_initial_data function.
         """
         class AccountInitialData1(BaseInitialData):
             """
@@ -152,31 +152,31 @@
             The initial data code the second time it is called. It no longer creates the account object, so the
             previously created account object should be deleted.
             """
             def update_initial_data(self):
                 pass
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData1):
             InitialDataUpdater().update_all_apps()
 
         # Verify an account object was created and is managed by a deletion receipt
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
 
         # Run the initial data process again, this time not registering the account for
         # deletion. It should be deleted.
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData2):
             InitialDataUpdater().update_all_apps()
 
         # Verify there are no accounts or receipts
-        self.assertEquals(Account.objects.count(), 0)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 0)
 
     def test_handle_deletions_updates_registered_from_update_initial_data(self):
         """
         Tests handling of deletions and updates when they are registered from the update_initial_data function.
         """
         class AccountInitialData1(BaseInitialData):
             """
@@ -192,31 +192,31 @@
             """
             The initial data code the second time it is called. It only manages one of the previous accounts
             """
             def update_initial_data(self):
                 self.register_for_deletion(Account.objects.get_or_create(name='hi')[0])
 
         # Verify no account objects exist
-        self.assertEquals(Account.objects.count(), 0)
+        self.assertEqual(Account.objects.count(), 0)
 
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData1):
             InitialDataUpdater().update_all_apps()
 
         # Verify two account objects were created and are managed by deletion receipts
-        self.assertEquals(Account.objects.count(), 2)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 2)
+        self.assertEqual(Account.objects.count(), 2)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 2)
 
         # Run the initial data process again, this time deleting the account named 'hi2'
         with patch.object(InitialDataUpdater, 'load_app', return_value=AccountInitialData2):
             InitialDataUpdater().update_all_apps()
 
         # Verify only the 'hi' account exists
-        self.assertEquals(Account.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.count(), 1)
-        self.assertEquals(RegisteredForDeletionReceipt.objects.get().model_obj.name, 'hi')
+        self.assertEqual(Account.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.count(), 1)
+        self.assertEqual(RegisteredForDeletionReceipt.objects.get().model_obj.name, 'hi')
 
     @patch('dynamic_initial_data.base.InitialDataUpdater.log')
     def test_missing_initial_data_file(self, mock_log):
         """
         Makes sure the log method is called when an app doesn't contain an initial_data file
         :type mock_log: mock.Mock
         """
```

### Comparing `django-dynamic-initial-data-2.1.0/dynamic_initial_data/tests/management_command_tests.py` & `django-dynamic-initial-data-2.2.1/dynamic_initial_data/tests/management_command_tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from django.core.management import call_command
-from django.test import TestCase
-from mock import patch
-
-
-class UpdateInitialDataTest(TestCase):
-    """
-    Tests each of the management commands
-    """
-    def test_no_arguments(self):
-        """
-        Makes sure the update_initial_data method gets called when the command is run
-        """
-        with patch('dynamic_initial_data.base.InitialDataUpdater.update_all_apps') as update_patch:
-            call_command('update_initial_data')
-            self.assertEqual(1, update_patch.call_count)
-
-    def test_app_argument(self):
-        """
-        Tests the management command with the --app argument. Verifies that it runs for only the
-        provided app.
-        """
-        with patch('dynamic_initial_data.base.InitialDataUpdater.update_app') as update_patch:
-            call_command('update_initial_data', app='app_path')
-            self.assertEqual(1, update_patch.call_count)
-            update_patch.assert_called_with('app_path')
+from django.core.management import call_command
+from django.test import TestCase
+from unittest.mock import patch
+
+
+class UpdateInitialDataTest(TestCase):
+    """
+    Tests each of the management commands
+    """
+    def test_no_arguments(self):
+        """
+        Makes sure the update_initial_data method gets called when the command is run
+        """
+        with patch('dynamic_initial_data.base.InitialDataUpdater.update_all_apps') as update_patch:
+            call_command('update_initial_data')
+            self.assertEqual(1, update_patch.call_count)
+
+    def test_app_argument(self):
+        """
+        Tests the management command with the --app argument. Verifies that it runs for only the
+        provided app.
+        """
+        with patch('dynamic_initial_data.base.InitialDataUpdater.update_app') as update_patch:
+            call_command('update_initial_data', app='app_path')
+            self.assertEqual(1, update_patch.call_count)
+            update_patch.assert_called_with('app_path')
```

### Comparing `django-dynamic-initial-data-2.1.0/LICENSE` & `django-dynamic-initial-data-2.2.1/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-The MIT License (MIT)
-
-Copyright (c) 2014 Ambition
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of
-this software and associated documentation files (the "Software"), to deal in
-the Software without restriction, including without limitation the rights to
-use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software is furnished to do so,
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
-FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
-COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
-IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
-CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) 2014 Ambition
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software is furnished to do so,
+subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
+FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
+COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
+IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
+CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `django-dynamic-initial-data-2.1.0/PKG-INFO` & `django-dynamic-initial-data-2.2.1/django_dynamic_initial_data.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,139 +1,142 @@
 Metadata-Version: 2.1
 Name: django-dynamic-initial-data
-Version: 2.1.0
+Version: 2.2.1
 Summary: Dynamic initial data fixtures for Django apps
 Home-page: https://github.com/ambitioninc/django-dynamic-initial-data
 Author: 
 Author-email: opensource@ambition.com
 License: MIT
-Description: [![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
-        
-        ## Django Initial Data
-        
-        Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
-        dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
-        can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
-        deleted from initial data, a feature that Django's initial data fixture system lacks.
-        
-        ## Table of Contents
-        
-        1. [Installation] (#installation)
-        2. [A Brief Overview] (#a-brief-overview)
-        3. [Example] (#example)
-        4. [Handling Deletions](#handling-deletions)
-        
-        ## Installation
-        To install Django Dynamic Initial Data:
-        
-        ```shell
-        pip install django-dynamic-initial-data
-        ```
-        
-        Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
-        
-        settings.py
-        ```python
-        INSTALLED_APPS = (
-            'dynamic_initial_data',
-        )
-        ```
-        
-        ## A Brief Overview
-        
-        A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
-        command is intended to be called as part of the deployment process of your app. Any missing dependencies
-        will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
-        `InitialDataCircularDependency` exception.
-        
-        Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
-        directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
-        the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
-        that inherits from `BaseInitialData`.
-        
-        When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
-        If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
-        
-        Any dependencies should be included in a list called `dependencies`. Each dependency is a string
-        of the app name as defined in `INSTALLED_APPS`.
-        
-        ## Example:
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            dependencies = ['my_first_app', 'my.second.app']
-        
-            def update_initial_data(self):
-                model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
-        
-                TestModel.objects.bulk_upsert([
-                    TestModel(float_field=1.0, char_field='1', int_field=1),
-                    TestModel(float_field=2.0, char_field='2', int_field=2),
-                    TestModel(float_field=3.0, char_field='3', int_field=3),
-                ], ['int_field'], ['char_field'])
-        ```
-        In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
-        and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
-        
-        ```
-        python manage.py update_initial_data
-        ```
-        
-        Similarly, to only initialize a single app, use
-        
-        ```
-        python manage.py update_initial_data --app 'app_path'
-        ```
-        
-        Documentation on using `upsert` and `bulk_upsert` can be found below:
-        - https://github.com/ambitioninc/django-manager-utils#upsert
-        - https://github.com/ambitioninc/django-manager-utils#bulk_upsert
-        
-        ## Handling Deletions
-        One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
-        
-        Django Dynamic Initial Data fixes this problem by allowing the user to either:
-        
-        1. Return all managed initial data objects as an array from the update_initial_data function.
-        2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
-        
-        Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            def update_initial_data(self):
-                hello = Account.objects.get_or_create(name='hello')
-                world = Account.objects.get_or_create(name='world')
-                # register the accounts for deletion
-                self.register_for_deletion(hello, world)
-        ```
-        
-        After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
-        
-        ```python
-        from dynamic_initial_data.base import BaseInitialData
-        
-        class InitialData(BaseInitialData):
-            def update_initial_data(self):
-                world = Account.objects.get_or_create(name='world')
-                # register the accounts for deletion
-                self.register_for_deletion(world)
-        ```
-        
-        When this piece of code executes, the previous "hello" account would then be deleted since the initial data process no longer owns it. And don't worry, if it was already deleted by another process, the deletion will not throw an error.
 Keywords: Django fixtures
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
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+[![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
+
+## Django Initial Data
+
+Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
+dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
+can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
+deleted from initial data, a feature that Django's initial data fixture system lacks.
+
+## Table of Contents
+
+1. [Installation] (#installation)
+2. [A Brief Overview] (#a-brief-overview)
+3. [Example] (#example)
+4. [Handling Deletions](#handling-deletions)
+
+## Installation
+To install Django Dynamic Initial Data:
+
+```shell
+pip install django-dynamic-initial-data
+```
+
+Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
+
+settings.py
+```python
+INSTALLED_APPS = (
+    'dynamic_initial_data',
+)
+```
+
+## A Brief Overview
+
+A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
+command is intended to be called as part of the deployment process of your app. Any missing dependencies
+will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
+`InitialDataCircularDependency` exception.
+
+Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
+directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
+the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
+that inherits from `BaseInitialData`.
+
+When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
+If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
+
+Any dependencies should be included in a list called `dependencies`. Each dependency is a string
+of the app name as defined in `INSTALLED_APPS`.
+
+## Example:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    dependencies = ['my_first_app', 'my.second.app']
+
+    def update_initial_data(self):
+        model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
+
+        TestModel.objects.bulk_upsert([
+            TestModel(float_field=1.0, char_field='1', int_field=1),
+            TestModel(float_field=2.0, char_field='2', int_field=2),
+            TestModel(float_field=3.0, char_field='3', int_field=3),
+        ], ['int_field'], ['char_field'])
+```
+In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
+and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
+
+```
+python manage.py update_initial_data
+```
+
+Similarly, to only initialize a single app, use
+
+```
+python manage.py update_initial_data --app 'app_path'
+```
+
+Documentation on using `upsert` and `bulk_upsert` can be found below:
+- https://github.com/ambitioninc/django-manager-utils#upsert
+- https://github.com/ambitioninc/django-manager-utils#bulk_upsert
+
+## Handling Deletions
+One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
+
+Django Dynamic Initial Data fixes this problem by allowing the user to either:
+
+1. Return all managed initial data objects as an array from the update_initial_data function.
+2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
+
+Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        hello = Account.objects.get_or_create(name='hello')
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(hello, world)
+```
+
+After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(world)
+```
+
+When this piece of code executes, the previous "hello" account would then be deleted since the initial data process no longer owns it. And don't worry, if it was already deleted by another process, the deletion will not throw an error.
```

### Comparing `django-dynamic-initial-data-2.1.0/README.md` & `django-dynamic-initial-data-2.2.1/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-[![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
-
-## Django Initial Data
-
-Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
-dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
-can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
-deleted from initial data, a feature that Django's initial data fixture system lacks.
-
-## Table of Contents
-
-1. [Installation] (#installation)
-2. [A Brief Overview] (#a-brief-overview)
-3. [Example] (#example)
-4. [Handling Deletions](#handling-deletions)
-
-## Installation
-To install Django Dynamic Initial Data:
-
-```shell
-pip install django-dynamic-initial-data
-```
-
-Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
-
-settings.py
-```python
-INSTALLED_APPS = (
-    'dynamic_initial_data',
-)
-```
-
-## A Brief Overview
-
-A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
-command is intended to be called as part of the deployment process of your app. Any missing dependencies
-will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
-`InitialDataCircularDependency` exception.
-
-Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
-directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
-the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
-that inherits from `BaseInitialData`.
-
-When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
-If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
-
-Any dependencies should be included in a list called `dependencies`. Each dependency is a string
-of the app name as defined in `INSTALLED_APPS`.
-
-## Example:
-
-```python
-from dynamic_initial_data.base import BaseInitialData
-
-class InitialData(BaseInitialData):
-    dependencies = ['my_first_app', 'my.second.app']
-
-    def update_initial_data(self):
-        model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
-
-        TestModel.objects.bulk_upsert([
-            TestModel(float_field=1.0, char_field='1', int_field=1),
-            TestModel(float_field=2.0, char_field='2', int_field=2),
-            TestModel(float_field=3.0, char_field='3', int_field=3),
-        ], ['int_field'], ['char_field'])
-```
-In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
-and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
-
-```
-python manage.py update_initial_data
-```
-
-Similarly, to only initialize a single app, use
-
-```
-python manage.py update_initial_data --app 'app_path'
-```
-
-Documentation on using `upsert` and `bulk_upsert` can be found below:
-- https://github.com/ambitioninc/django-manager-utils#upsert
-- https://github.com/ambitioninc/django-manager-utils#bulk_upsert
-
-## Handling Deletions
-One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
-
-Django Dynamic Initial Data fixes this problem by allowing the user to either:
-
-1. Return all managed initial data objects as an array from the update_initial_data function.
-2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
-
-Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
-
-```python
-from dynamic_initial_data.base import BaseInitialData
-
-class InitialData(BaseInitialData):
-    def update_initial_data(self):
-        hello = Account.objects.get_or_create(name='hello')
-        world = Account.objects.get_or_create(name='world')
-        # register the accounts for deletion
-        self.register_for_deletion(hello, world)
-```
-
-After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
-
-```python
-from dynamic_initial_data.base import BaseInitialData
-
-class InitialData(BaseInitialData):
-    def update_initial_data(self):
-        world = Account.objects.get_or_create(name='world')
-        # register the accounts for deletion
-        self.register_for_deletion(world)
-```
-
+[![Build Status](https://travis-ci.org/ambitioninc/django-dynamic-initial-data.png)](https://travis-ci.org/ambitioninc/django-dynamic-initial-data)
+
+## Django Initial Data
+
+Django Dynamic Initial Data is a `django>=1.6` and *postgresql* only app that helps solve the problem of initializing data for apps with
+dependencies and other conditional data. Rather than having static fixtures for each app, the initial data
+can be created and updated dynamically. Furthermore, Django Dynamic Initial Data also handles when objects are
+deleted from initial data, a feature that Django's initial data fixture system lacks.
+
+## Table of Contents
+
+1. [Installation] (#installation)
+2. [A Brief Overview] (#a-brief-overview)
+3. [Example] (#example)
+4. [Handling Deletions](#handling-deletions)
+
+## Installation
+To install Django Dynamic Initial Data:
+
+```shell
+pip install django-dynamic-initial-data
+```
+
+Add Django Dynamic Initial Data to your `INSTALLED_APPS` to get started:
+
+settings.py
+```python
+INSTALLED_APPS = (
+    'dynamic_initial_data',
+)
+```
+
+## A Brief Overview
+
+A management command `update_initial_data` is provided which will try to update all `INSTALLED_APPS`. This
+command is intended to be called as part of the deployment process of your app. Any missing dependencies
+will raise an `InitialDataMissingApp` exception and any circular dependencies will raise an
+`InitialDataCircularDependency` exception.
+
+Any app needing to define initial data needs a file called `initial_data.py` inside of a `fixtures`
+directory. This will look like `{app_name}/fixtures/initial_data.py`. Don't forget to include
+the `__init__.py` file in the fixtures directory. `initial_data.py` must define a class `InitialData`
+that inherits from `BaseInitialData`.
+
+When apps are being initialized, each `InitialData` class is instantiated and `update_initial_data` is called.
+If `update_initial_data` is not implemented, then a `NotImplementedError` will be raised.
+
+Any dependencies should be included in a list called `dependencies`. Each dependency is a string
+of the app name as defined in `INSTALLED_APPS`.
+
+## Example:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    dependencies = ['my_first_app', 'my.second.app']
+
+    def update_initial_data(self):
+        model_obj, created = TestModel.objects.upsert(int_field=5, defaults={'float_field': 2.0})
+
+        TestModel.objects.bulk_upsert([
+            TestModel(float_field=1.0, char_field='1', int_field=1),
+            TestModel(float_field=2.0, char_field='2', int_field=2),
+            TestModel(float_field=3.0, char_field='3', int_field=3),
+        ], ['int_field'], ['char_field'])
+```
+In this example, the `update_initial_data` method will be called for `my_first_app` (following any dependencies first),
+and then for `my.second.app`, before finally calling `update_initial_data` on this class. Again, this can be executed by calling
+
+```
+python manage.py update_initial_data
+```
+
+Similarly, to only initialize a single app, use
+
+```
+python manage.py update_initial_data --app 'app_path'
+```
+
+Documentation on using `upsert` and `bulk_upsert` can be found below:
+- https://github.com/ambitioninc/django-manager-utils#upsert
+- https://github.com/ambitioninc/django-manager-utils#bulk_upsert
+
+## Handling Deletions
+One difficulty when specifying initial data in Django apps is the inability to deploy initial data to your project and then subsequently remove any initial data fixtures. If one removes an object in an initial_data.json file, Django does not handle its deletion next time it is deployed, which can cause headaches with lingering objects.
+
+Django Dynamic Initial Data fixes this problem by allowing the user to either:
+
+1. Return all managed initial data objects as an array from the update_initial_data function.
+2. Explicitly register objects for deletion with the register_for_deletion(*model_objs) method.
+
+Note that it is up to the user to be responsible for always registering every object every time, regardless if the object was updated or created by the initial data process. Doing this allows Django Dynamic Initial Data to remove any objects that were previosly managed. For example, assume you have an InitialData class that manages two users with the user names "hello" and "world".
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        hello = Account.objects.get_or_create(name='hello')
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(hello, world)
+```
+
+After this code is created, the initial data process now owns the "hello" and "world" account objects. If these objects are not registered for deletion in subsequent versions of the code, they will be deleted when the initial data process executes. For example, assume the first piece of code executed and then the user executed this piece of code:
+
+```python
+from dynamic_initial_data.base import BaseInitialData
+
+class InitialData(BaseInitialData):
+    def update_initial_data(self):
+        world = Account.objects.get_or_create(name='world')
+        # register the accounts for deletion
+        self.register_for_deletion(world)
+```
+
 When this piece of code executes, the previous "hello" account would then be deleted since the initial data process no longer owns it. And don't worry, if it was already deleted by another process, the deletion will not throw an error.
```

### Comparing `django-dynamic-initial-data-2.1.0/setup.py` & `django-dynamic-initial-data-2.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,45 +13,46 @@
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
+
 setup(
     name='django-dynamic-initial-data',
     version=get_version(),
     description='Dynamic initial data fixtures for Django apps',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ambitioninc/django-dynamic-initial-data',
     author='',
     author_email='opensource@ambition.com',
     keywords='Django fixtures',
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
-        'django-manager-utils>=1.4.0',
-    ],
-    tests_require=[
-        'psycopg2',
-        'django-dynamic-fixture',
-        'django-nose>=1.4',
-        'freezegun',
-        'mock',
-    ],
+    install_requires=install_requires,
+    tests_require=tests_require,
     test_suite='run_tests.run_tests',
     include_package_data=True,
 )
```

