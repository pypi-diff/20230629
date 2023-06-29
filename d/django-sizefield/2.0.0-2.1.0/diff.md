# Comparing `tmp/django-sizefield-2.0.0.tar.gz` & `tmp/django-sizefield-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sizefield-2.0.0.tar", last modified: Wed Sep  8 10:23:21 2021, max compression
+gzip compressed data, was "django-sizefield-2.1.0.tar", last modified: Thu Jun 29 12:00:56 2023, max compression
```

## Comparing `django-sizefield-2.0.0.tar` & `django-sizefield-2.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     1235 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/CHANGES
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     7651 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/LICENSE
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       35 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/MANIFEST.in
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     4488 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/PKG-INFO
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     1132 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/README.rst
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/django_sizefield.egg-info/
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     4488 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/PKG-INFO
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      461 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/SOURCES.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        1 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/dependency_links.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        1 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/not-zip-safe
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        7 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/requires.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       10 2021-09-08 10:23:21.000000 django-sizefield-2.0.0/django_sizefield.egg-info/top_level.txt
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)       38 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/setup.cfg
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     1464 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/setup.py
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/sizefield/
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/__init__.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      954 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/models.py
-drwxrwxr-x   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:21.199153 django-sizefield-2.0.0/sizefield/templatetags/
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)        0 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/templatetags/__init__.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      256 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/templatetags/sizefieldtags.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     4032 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/tests.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)     2104 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/utils.py
--rw-rw-r--   0 mathieu   (1000) mathieu   (1000)      922 2021-09-08 10:23:20.000000 django-sizefield-2.0.0/sizefield/widgets.py
+drwxr-xr-x   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.759898 django-sizefield-2.1.0/
+-rw-r--r--   0 mathieu    (503) staff       (20)     1349 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/CHANGES
+-rw-r--r--   0 mathieu    (503) staff       (20)     7651 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/LICENSE
+-rw-r--r--   0 mathieu    (503) staff       (20)       35 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/MANIFEST.in
+-rw-r--r--   0 mathieu    (503) staff       (20)     3385 2023-06-29 12:00:56.759774 django-sizefield-2.1.0/PKG-INFO
+-rw-r--r--   0 mathieu    (503) staff       (20)     1132 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/README.rst
+drwxr-xr-x   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.758829 django-sizefield-2.1.0/django_sizefield.egg-info/
+-rw-r--r--   0 mathieu    (503) staff       (20)     3385 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/PKG-INFO
+-rw-r--r--   0 mathieu    (503) staff       (20)      461 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/SOURCES.txt
+-rw-r--r--   0 mathieu    (503) staff       (20)        1 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/dependency_links.txt
+-rw-r--r--   0 mathieu    (503) staff       (20)        1 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/not-zip-safe
+-rw-r--r--   0 mathieu    (503) staff       (20)        7 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/requires.txt
+-rw-r--r--   0 mathieu    (503) staff       (20)       10 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/django_sizefield.egg-info/top_level.txt
+-rw-r--r--   0 mathieu    (503) staff       (20)       38 2023-06-29 12:00:56.759932 django-sizefield-2.1.0/setup.cfg
+-rw-r--r--   0 mathieu    (503) staff       (20)     1464 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/setup.py
+drwxr-xr-x   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.759389 django-sizefield-2.1.0/sizefield/
+-rw-r--r--   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/__init__.py
+-rw-r--r--   0 mathieu    (503) staff       (20)      953 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/models.py
+drwxr-xr-x   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.759603 django-sizefield-2.1.0/sizefield/templatetags/
+-rw-r--r--   0 mathieu    (503) staff       (20)        0 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/templatetags/__init__.py
+-rw-r--r--   0 mathieu    (503) staff       (20)      256 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/templatetags/sizefieldtags.py
+-rw-r--r--   0 mathieu    (503) staff       (20)     4032 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/tests.py
+-rw-r--r--   0 mathieu    (503) staff       (20)     2103 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/utils.py
+-rw-r--r--   0 mathieu    (503) staff       (20)      922 2023-06-29 12:00:56.000000 django-sizefield-2.1.0/sizefield/widgets.py
```

### Comparing `django-sizefield-2.0.0/CHANGES` & `django-sizefield-2.1.0/CHANGES`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 =========
 CHANGELOG
 =========
 
+2.1.0 (2023-06-29)
+==================
+
+- Remove usage of removed functions in Django 4 (thanks @hagbarddenstore)
+
 2.0.0 (2020-08-13)
 ==================
 
 - Dropped support for python 2
 - Dropped support for Django <2
 - Moved testing to GitHub Actions and tox
```

### Comparing `django-sizefield-2.0.0/LICENSE` & `django-sizefield-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sizefield-2.0.0/README.rst` & `django-sizefield-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-sizefield-2.0.0/setup.py` & `django-sizefield-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup(
     name='django-sizefield',
-    version='2.0.0',
+    version='2.1.0',
     author='Mathieu Leplatre',
     author_email='contact@mathieu-leplatre.info',
     url='https://github.com/leplatrem/django-sizefield',
     download_url="http://pypi.python.org/pypi/django-sizefield/",
     description="A model field to store a file size, whose edition and display shows units.",
     long_description=open(os.path.join(here, 'README.rst')).read() + '\n\n' +
                      open(os.path.join(here, 'CHANGES')).read(),
```

### Comparing `django-sizefield-2.0.0/sizefield/models.py` & `django-sizefield-2.1.0/sizefield/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.db import models
 from django.core import exceptions
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from sizefield.utils import parse_size
 from sizefield.widgets import FileSizeWidget
 
 
 class FileSizeField(models.BigIntegerField):
     default_error_messages = {
```

### Comparing `django-sizefield-2.0.0/sizefield/tests.py` & `django-sizefield-2.1.0/sizefield/tests.py`

 * *Files identical despite different names*

### Comparing `django-sizefield-2.0.0/sizefield/utils.py` & `django-sizefield-2.1.0/sizefield/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import unicode_literals
 
 import sys
 import re
 import operator
 
 from django.utils import formats
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.conf import settings
 
 
 if sys.version_info >= (3, 0):
     xrange = range
 
 SIZEFIELD_FORMAT = getattr(settings, 'SIZEFIELD_FORMAT', '{value}{unit}')
```

### Comparing `django-sizefield-2.0.0/sizefield/widgets.py` & `django-sizefield-2.1.0/sizefield/widgets.py`

 * *Files identical despite different names*

