# Comparing `tmp/django_hawk-1.2.0.tar.gz` & `tmp/django_hawk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hawk-1.2.0.tar", max compression
+gzip compressed data, was "django_hawk-1.2.1.tar", max compression
```

## Comparing `django_hawk-1.2.0.tar` & `django_hawk-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1091 2022-11-15 16:57:39.615067 django_hawk-1.2.0/LICENSE
--rw-r--r--   0        0        0     2632 2023-04-19 10:07:40.848963 django_hawk-1.2.0/README.md
--rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615449 django_hawk-1.2.0/django_hawk/__init__.py
--rw-r--r--   0        0        0     1992 2022-11-15 16:58:07.593679 django_hawk-1.2.0/django_hawk/authentication.py
--rw-r--r--   0        0        0     1494 2023-02-28 10:16:42.657151 django_hawk-1.2.0/django_hawk/middleware.py
--rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615710 django_hawk-1.2.0/django_hawk/py.typed
--rw-r--r--   0        0        0     1014 2022-11-15 16:58:07.593989 django_hawk-1.2.0/django_hawk/settings.py
--rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615896 django_hawk-1.2.0/django_hawk/tests/__init__.py
--rw-r--r--   0        0        0     1008 2022-11-16 14:11:50.330670 django_hawk-1.2.0/django_hawk/tests/settings.py
--rw-r--r--   0        0        0     4717 2022-11-16 16:21:34.934697 django_hawk-1.2.0/django_hawk/tests/test_views.py
--rw-r--r--   0        0        0     1101 2023-02-28 10:16:42.657465 django_hawk-1.2.0/django_hawk/tests/test_views_django.py
--rw-r--r--   0        0        0      333 2023-02-28 10:16:42.657597 django_hawk-1.2.0/django_hawk/tests/urls.py
--rw-r--r--   0        0        0      936 2023-02-28 10:16:42.658072 django_hawk-1.2.0/django_hawk/tests/views.py
--rw-r--r--   0        0        0     1011 2022-11-17 13:21:23.905719 django_hawk-1.2.0/django_hawk/utils.py
--rw-r--r--   0        0        0      797 2023-04-19 10:12:06.051016 django_hawk-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 django_hawk-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-11-15 16:57:39.615067 django_hawk-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2632 2023-04-19 10:07:40.848963 django_hawk-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615449 django_hawk-1.2.1/django_hawk/__init__.py
+-rw-r--r--   0        0        0     1992 2022-11-15 16:58:07.593679 django_hawk-1.2.1/django_hawk/authentication.py
+-rw-r--r--   0        0        0     1494 2023-02-28 10:16:42.657151 django_hawk-1.2.1/django_hawk/middleware.py
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615710 django_hawk-1.2.1/django_hawk/py.typed
+-rw-r--r--   0        0        0     1014 2022-11-15 16:58:07.593989 django_hawk-1.2.1/django_hawk/settings.py
+-rw-r--r--   0        0        0        0 2022-11-15 16:57:39.615896 django_hawk-1.2.1/django_hawk/tests/__init__.py
+-rw-r--r--   0        0        0     1008 2022-11-16 14:11:50.330670 django_hawk-1.2.1/django_hawk/tests/settings.py
+-rw-r--r--   0        0        0     4717 2022-11-16 16:21:34.934697 django_hawk-1.2.1/django_hawk/tests/test_views.py
+-rw-r--r--   0        0        0     1101 2023-02-28 10:16:42.657465 django_hawk-1.2.1/django_hawk/tests/test_views_django.py
+-rw-r--r--   0        0        0      333 2023-02-28 10:16:42.657597 django_hawk-1.2.1/django_hawk/tests/urls.py
+-rw-r--r--   0        0        0      936 2023-02-28 10:16:42.658072 django_hawk-1.2.1/django_hawk/tests/views.py
+-rw-r--r--   0        0        0     1011 2022-11-17 13:21:23.905719 django_hawk-1.2.1/django_hawk/utils.py
+-rw-r--r--   0        0        0      797 2023-06-29 10:33:10.092502 django_hawk-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3375 1970-01-01 00:00:00.000000 django_hawk-1.2.1/PKG-INFO
```

### Comparing `django_hawk-1.2.0/LICENSE` & `django_hawk-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/README.md` & `django_hawk-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/authentication.py` & `django_hawk-1.2.1/django_hawk/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/middleware.py` & `django_hawk-1.2.1/django_hawk/middleware.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/settings.py` & `django_hawk-1.2.1/django_hawk/settings.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/tests/settings.py` & `django_hawk-1.2.1/django_hawk/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/tests/test_views.py` & `django_hawk-1.2.1/django_hawk/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/tests/test_views_django.py` & `django_hawk-1.2.1/django_hawk/tests/test_views_django.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/tests/views.py` & `django_hawk-1.2.1/django_hawk/tests/views.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/django_hawk/utils.py` & `django_hawk-1.2.1/django_hawk/utils.py`

 * *Files identical despite different names*

### Comparing `django_hawk-1.2.0/pyproject.toml` & `django_hawk-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "django-hawk"
-version = "1.2.0"
+version = "1.2.1"
 description = "Authenticate Django Views with HAWK"
 authors = [
     "Cameron Lamb <live.services@digital.trade.gov.uk>"
 ]
 license = "MIT"
 readme = "README.md"
 keywords = [
```

### Comparing `django_hawk-1.2.0/PKG-INFO` & `django_hawk-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hawk
-Version: 1.2.0
+Version: 1.2.1
 Summary: Authenticate Django Views with HAWK
 Home-page: https://github.com/uktrade/django-hawk
 License: MIT
 Keywords: django
 Author: Cameron Lamb
 Author-email: live.services@digital.trade.gov.uk
 Requires-Python: >=3.7,<4.0
```

