# Comparing `tmp/makolator-2.0.0.tar.gz` & `tmp/makolator-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-2.0.0.tar", max compression
+gzip compressed data, was "makolator-2.0.1.tar", max compression
```

## Comparing `makolator-2.0.0.tar` & `makolator-2.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-2.0.0/LICENSE
--rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-2.0.0/README.md
--rw-r--r--   0        0        0     5006 2023-06-23 15:54:24.125144 makolator-2.0.0/makolator/__init__.py
--rw-r--r--   0        0        0     1182 2023-06-23 20:30:05.045375 makolator-2.0.0/makolator/__main__.py
--rw-r--r--   0        0        0     8305 2023-06-23 20:51:04.188011 makolator-2.0.0/makolator/_inplace.py
--rw-r--r--   0        0        0     4189 2023-06-23 20:33:51.637383 makolator-2.0.0/makolator/cli.py
--rw-r--r--   0        0        0     2209 2023-06-23 19:03:41.601501 makolator-2.0.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-2.0.0/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-2.0.0/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-2.0.0/makolator/exceptions.py
--rw-r--r--   0        0        0     7662 2023-06-23 20:50:50.723768 makolator-2.0.0/makolator/makolator.py
--rw-r--r--   0        0        0     2290 2023-06-23 20:54:37.851855 makolator-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 13:28:30.852384 makolator-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1140 2023-06-29 13:28:30.852384 makolator-2.0.1/README.md
+-rw-r--r--   0        0        0     5006 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/__init__.py
+-rw-r--r--   0        0        0     1182 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/__main__.py
+-rw-r--r--   0        0        0     8305 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/_inplace.py
+-rw-r--r--   0        0        0     4189 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/cli.py
+-rw-r--r--   0        0        0     2209 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/datamodel.py
+-rw-r--r--   0        0        0      897 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/escape.py
+-rw-r--r--   0        0        0      106 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/exceptions.py
+-rw-r--r--   0        0        0     7662 2023-06-29 13:28:30.852384 makolator-2.0.1/makolator/makolator.py
+-rw-r--r--   0        0        0     2290 2023-06-29 13:28:30.856384 makolator-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-2.0.1/PKG-INFO
```

### Comparing `makolator-2.0.0/LICENSE` & `makolator-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/README.md` & `makolator-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/__init__.py` & `makolator-2.0.1/makolator/__init__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/__main__.py` & `makolator-2.0.1/makolator/__main__.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/_inplace.py` & `makolator-2.0.1/makolator/_inplace.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/cli.py` & `makolator-2.0.1/makolator/cli.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/config.py` & `makolator-2.0.1/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/datamodel.py` & `makolator-2.0.1/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/escape.py` & `makolator-2.0.1/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/makolator/makolator.py` & `makolator-2.0.1/makolator/makolator.py`

 * *Files identical despite different names*

### Comparing `makolator-2.0.0/pyproject.toml` & `makolator-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "2.0.0"
+version = "2.0.1"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-2.0.0/PKG-INFO` & `makolator-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 2.0.0
+Version: 2.0.1
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

