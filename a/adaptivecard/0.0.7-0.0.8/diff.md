# Comparing `tmp/adaptivecard-0.0.7.tar.gz` & `tmp/adaptivecard-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.0.7.tar", last modified: Sun Jun 18 22:03:20 2023, max compression
+gzip compressed data, was "adaptivecard-0.0.8.tar", last modified: Thu Jun 29 21:27:43 2023, max compression
```

## Comparing `adaptivecard-0.0.7.tar` & `adaptivecard-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.233253 adaptivecard-0.0.7/
--rw-r--r--   0 cabutchei   (501) staff       (20)      600 2023-06-18 22:03:20.233014 adaptivecard-0.0.7/PKG-INFO
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.7/README.md
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.231832 adaptivecard-0.0.7/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.7/adaptivecard/__init__.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.7/adaptivecard/classes.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.7/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.7/adaptivecard/mixin.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-18 22:03:20.232748 adaptivecard-0.0.7/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      600 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      260 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-18 22:03:20.000000 adaptivecard-0.0.7/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-18 22:03:20.233318 adaptivecard-0.0.7/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)      886 2023-06-18 21:58:28.000000 adaptivecard-0.0.7/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.666243 adaptivecard-0.0.8/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-06-29 21:21:04.000000 adaptivecard-0.0.8/LICENSE.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)      703 2023-06-29 21:27:43.666051 adaptivecard-0.0.8/PKG-INFO
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.8/README.md
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.665170 adaptivecard-0.0.8/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.8/adaptivecard/__init__.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.8/adaptivecard/classes.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.8/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.8/adaptivecard/mixin.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.665813 adaptivecard-0.0.8/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      703 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      272 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-29 21:27:43.666413 adaptivecard-0.0.8/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)      947 2023-06-29 21:24:26.000000 adaptivecard-0.0.8/setup.py
```

### Comparing `adaptivecard-0.0.7/adaptivecard/classes.py` & `adaptivecard-0.0.8/adaptivecard/classes.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.7/adaptivecard/mixin.py` & `adaptivecard-0.0.8/adaptivecard/mixin.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.7/setup.py` & `adaptivecard-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from re import L
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Microsoft Adaptive Cards'
 LONG_DESCRIPTION = 'A package that helps you design adaptive cards in an object-oriented manner.'
 
 setup(
     name="adaptivecard",
     version=VERSION,
     author="cabutchei (Luan Paz)",
     author_email="<luropa_paz@hotmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    keywords=['python', 'card', 'adaptive card', 'microsoft'],
+    requires=[
+        'typeguard'
+    ],
+    keywords=['python', 'adaptive', 'card', 'adaptive card', 'microsoft'],
     classifiers=[
-        "Development Status :: 1 - Planning",
+        "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
+        "License :: OSI Approved :: MIT License", 
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
 )
```

