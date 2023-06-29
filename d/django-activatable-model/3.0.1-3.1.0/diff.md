# Comparing `tmp/django-activatable-model-3.0.1.tar.gz` & `tmp/django-activatable-model-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-activatable-model-3.0.1.tar", last modified: Tue Jan 24 19:01:17 2023, max compression
+gzip compressed data, was "django-activatable-model-3.1.0.tar", last modified: Thu Jun 29 14:46:22 2023, max compression
```

## Comparing `django-activatable-model-3.0.1.tar` & `django-activatable-model-3.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/LICENSE
--rw-rw-r--   0 wes       (1000) wes       (1000)       67 2023-01-24 18:59:26.000000 django-activatable-model-3.0.1/MANIFEST.in
--rw-rw-r--   0 wes       (1000) wes       (1000)     7921 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     6962 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/activatable_model/
--rw-rw-r--   0 wes       (1000) wes       (1000)      192 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      291 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/apps.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     5254 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      206 2023-01-24 18:39:49.000000 django-activatable-model-3.0.1/activatable_model/signals.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/activatable_model/tests/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/__init__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/activatable_model/tests/migrations/
--rw-rw-r--   0 wes       (1000) wes       (1000)     2056 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/migrations/0001_initial.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      810 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/migrations/0002_activatablemodelwrelandcascade.py
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/migrations/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      940 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/models.py
--rw-rw-r--   0 wes       (1000) wes       (1000)    22321 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/tests/tests.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/urls.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     2222 2023-01-09 15:24:09.000000 django-activatable-model-3.0.1/activatable_model/validation.py
--rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-01-24 19:00:35.000000 django-activatable-model-3.0.1/activatable_model/version.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/django_activatable_model.egg-info/
--rw-rw-r--   0 wes       (1000) wes       (1000)     7921 2023-01-24 19:01:17.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)      877 2023-01-24 19:01:17.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 19:01:17.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 18:58:31.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/not-zip-safe
--rw-rw-r--   0 wes       (1000) wes       (1000)      112 2023-01-24 19:01:17.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       18 2023-01-24 19:01:17.000000 django-activatable-model-3.0.1/django_activatable_model.egg-info/top_level.txt
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/requirements/
--rw-rw-r--   0 wes       (1000) wes       (1000)       76 2023-01-24 17:58:36.000000 django-activatable-model-3.0.1/requirements/requirements-testing.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-01-24 17:46:13.000000 django-activatable-model-3.0.1/requirements/requirements.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)      197 2023-01-24 19:01:17.143408 django-activatable-model-3.0.1/setup.cfg
--rw-rw-r--   0 wes       (1000) wes       (1000)     2040 2023-01-24 17:46:13.000000 django-activatable-model-3.0.1/setup.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1075 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/LICENSE
+-rw-rw-r--   0 wes       (1000) wes       (1000)       67 2023-06-29 14:45:43.000000 django-activatable-model-3.1.0/MANIFEST.in
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7843 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6962 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/activatable_model/
+-rw-rw-r--   0 wes       (1000) wes       (1000)      123 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/activatable_model/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      291 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/apps.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     5254 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      206 2023-01-24 18:39:49.000000 django-activatable-model-3.1.0/activatable_model/signals.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/activatable_model/tests/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/tests/__init__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/activatable_model/tests/migrations/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2016 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/activatable_model/tests/migrations/0001_initial.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      770 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/activatable_model/tests/migrations/0002_activatablemodelwrelandcascade.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/tests/migrations/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      940 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/tests/models.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)    22321 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/tests/tests.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       37 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/urls.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     2222 2023-01-09 15:24:09.000000 django-activatable-model-3.1.0/activatable_model/validation.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)       22 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/activatable_model/version.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/django_activatable_model.egg-info/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     7843 2023-06-29 14:46:22.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)      877 2023-06-29 14:46:22.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-06-29 14:46:22.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2023-01-24 18:58:31.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/not-zip-safe
+-rw-rw-r--   0 wes       (1000) wes       (1000)      112 2023-06-29 14:46:22.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       18 2023-06-29 14:46:22.000000 django-activatable-model-3.1.0/django_activatable_model.egg-info/top_level.txt
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/requirements/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       76 2023-01-24 17:58:36.000000 django-activatable-model-3.1.0/requirements/requirements-testing.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       40 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/requirements/requirements.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)      197 2023-06-29 14:46:22.496614 django-activatable-model-3.1.0/setup.cfg
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1964 2023-06-29 14:45:49.000000 django-activatable-model-3.1.0/setup.py
```

### Comparing `django-activatable-model-3.0.1/LICENSE` & `django-activatable-model-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/PKG-INFO` & `django-activatable-model-3.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: django-activatable-model
-Version: 3.0.1
+Version: 3.1.0
 Summary: Django Activatable Model
 Home-page: https://github.com/ambitioninc/django-activatable-model
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
 Keywords: Django,Model,Activatable
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
 
 [![Build Status](https://travis-ci.org/ambitioninc/django-activatable-model.png)](https://travis-ci.org/ambitioninc/django-activatable-model)
 # Django Activatable Model
```

### Comparing `django-activatable-model-3.0.1/README.md` & `django-activatable-model-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/activatable_model/models.py` & `django-activatable-model-3.1.0/activatable_model/models.py`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/activatable_model/tests/migrations/0001_initial.py` & `django-activatable-model-3.1.0/activatable_model/tests/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from django.db import models, migrations
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-activatable-model-3.0.1/activatable_model/tests/migrations/0002_activatablemodelwrelandcascade.py` & `django-activatable-model-3.1.0/activatable_model/tests/migrations/0002_activatablemodelwrelandcascade.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.9 on 2017-06-28 17:24
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `django-activatable-model-3.0.1/activatable_model/tests/models.py` & `django-activatable-model-3.1.0/activatable_model/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/activatable_model/tests/tests.py` & `django-activatable-model-3.1.0/activatable_model/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/activatable_model/validation.py` & `django-activatable-model-3.1.0/activatable_model/validation.py`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/django_activatable_model.egg-info/PKG-INFO` & `django-activatable-model-3.1.0/django_activatable_model.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 Metadata-Version: 2.1
 Name: django-activatable-model
-Version: 3.0.1
+Version: 3.1.0
 Summary: Django Activatable Model
 Home-page: https://github.com/ambitioninc/django-activatable-model
 Author: Wes Kendall
 Author-email: opensource@ambition.com
 License: MIT
 Keywords: Django,Model,Activatable
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
 
 [![Build Status](https://travis-ci.org/ambitioninc/django-activatable-model.png)](https://travis-ci.org/ambitioninc/django-activatable-model)
 # Django Activatable Model
```

### Comparing `django-activatable-model-3.0.1/django_activatable_model.egg-info/SOURCES.txt` & `django-activatable-model-3.1.0/django_activatable_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-activatable-model-3.0.1/setup.py` & `django-activatable-model-3.1.0/setup.py`

 * *Files 10% similar despite different names*

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
     extras_require={'dev': tests_require},
     test_suite='run_tests.run_tests',
     include_package_data=True,
```

