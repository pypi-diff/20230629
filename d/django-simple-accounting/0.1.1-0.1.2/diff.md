# Comparing `tmp/django_simple_accounting-0.1.1.tar.gz` & `tmp/django_simple_accounting-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_simple_accounting-0.1.1.tar", max compression
+gzip compressed data, was "django_simple_accounting-0.1.2.tar", max compression
```

## Comparing `django_simple_accounting-0.1.1.tar` & `django_simple_accounting-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1074 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/LICENSE
--rw-r--r--   0        0        0      738 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/README.md
--rw-r--r--   0        0        0      510 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-29 21:19:59.024801 django_simple_accounting-0.1.1/simple_accounting/__init__.py
--rw-r--r--   0        0        0      606 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/admin.py
--rw-r--r--   0        0        0     3302 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/models.py
--rw-r--r--   0        0        0      603 2023-06-29 21:19:59.028801 django_simple_accounting-0.1.1/simple_accounting/utils.py
--rw-r--r--   0        0        0     1291 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/README.md
+-rw-r--r--   0        0        0      510 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/simple_accounting/__init__.py
+-rw-r--r--   0        0        0      606 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/simple_accounting/admin.py
+-rw-r--r--   0        0        0     3310 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/simple_accounting/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3302 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/simple_accounting/models.py
+-rw-r--r--   0        0        0      603 2023-06-29 21:27:20.771704 django_simple_accounting-0.1.2/simple_accounting/utils.py
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 django_simple_accounting-0.1.2/PKG-INFO
```

### Comparing `django_simple_accounting-0.1.1/LICENSE` & `django_simple_accounting-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.1/README.md` & `django_simple_accounting-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.1/simple_accounting/admin.py` & `django_simple_accounting-0.1.2/simple_accounting/admin.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.1/simple_accounting/models.py` & `django_simple_accounting-0.1.2/simple_accounting/models.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.1/simple_accounting/utils.py` & `django_simple_accounting-0.1.2/simple_accounting/utils.py`

 * *Files identical despite different names*

### Comparing `django_simple_accounting-0.1.1/PKG-INFO` & `django_simple_accounting-0.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: django-simple-accounting
-Version: 0.1.1
+Version: 0.1.2
 Summary: Plain and simple accounting module for Django
 License: MIT
 Author: Šarūnas Navickas
 Author-email: sarunas@griaustinis.lt
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django (>=4.2.2,<5.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Description-Content-Type: text/markdown
 
 # django-simple-accounting
 Plain and Simple Accounting module for Django
 
 [![PyPI version fury.io](https://badge.fury.io/py/django-simple-accounting.svg)](https://pypi.python.org/pypi/django-simple-accounting/)
```

