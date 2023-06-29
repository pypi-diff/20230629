# Comparing `tmp/loopia_of_fury-1.2.1.tar.gz` & `tmp/loopia_of_fury-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopia_of_fury-1.2.1.tar", max compression
+gzip compressed data, was "loopia_of_fury-1.3.0.tar", max compression
```

## Comparing `loopia_of_fury-1.2.1.tar` & `loopia_of_fury-1.3.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     5630 2021-11-20 09:47:55.286610 loopia_of_fury-1.2.1/loopia_of_fury/__init__.py
--rw-r--r--   0        0        0       45 2021-11-20 09:47:55.286610 loopia_of_fury-1.2.1/loopia_of_fury/__main__.py
--rw-r--r--   0        0        0      620 2021-11-20 09:47:55.286610 loopia_of_fury-1.2.1/pyproject.toml
--rw-r--r--   0        0        0      850 2021-11-20 09:48:01.327359 loopia_of_fury-1.2.1/setup.py
--rw-r--r--   0        0        0      591 2021-11-20 09:48:01.327591 loopia_of_fury-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5630 2023-06-29 19:37:46.907977 loopia_of_fury-1.3.0/loopia_of_fury/__init__.py
+-rw-r--r--   0        0        0       45 2023-06-29 19:37:46.907977 loopia_of_fury-1.3.0/loopia_of_fury/__main__.py
+-rw-r--r--   0        0        0      615 2023-06-29 19:37:46.907977 loopia_of_fury-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 loopia_of_fury-1.3.0/PKG-INFO
```

### Comparing `loopia_of_fury-1.2.1/loopia_of_fury/__init__.py` & `loopia_of_fury-1.3.0/loopia_of_fury/__init__.py`

 * *Files identical despite different names*

### Comparing `loopia_of_fury-1.2.1/pyproject.toml` & `loopia_of_fury-1.3.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "loopia_of_fury"
-version = "1.2.1"
+version = "1.3.0"
 description = 'Loopia of Fury - A "DynDNS" client for Loopia when you have MFA/BankID enabled '
 authors = ["Simon Lundström <github-commits@soy.se>"]
 homepage = "https://github.com/simmel/loopia_of_fury"
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7.2"
 su-logging = {extras = ["structured"], version = "^0.3.0"}
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
-mypy = "^0.800"
-pytest = "^6.2.2"
-pylint = "^2.6.0"
+black = "^23.3"
+mypy = "^1.4"
+pytest = "^7.4"
+pylint = "^2.17"
 
 [tool.poetry.scripts]
 loopia_of_fury = 'loopia_of_fury:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `loopia_of_fury-1.2.1/PKG-INFO` & `loopia_of_fury-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: loopia-of-fury
-Version: 1.2.1
+Version: 1.3.0
 Summary: Loopia of Fury - A "DynDNS" client for Loopia when you have MFA/BankID enabled 
 Home-page: https://github.com/simmel/loopia_of_fury
 Author: Simon Lundström
 Author-email: github-commits@soy.se
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7.2,<4.0.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: su-logging[structured] (>=0.3.0,<0.4.0)
```

