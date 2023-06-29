# Comparing `tmp/adaptivecard-0.0.8.tar.gz` & `tmp/adaptivecard-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptivecard-0.0.8.tar", last modified: Thu Jun 29 21:27:43 2023, max compression
+gzip compressed data, was "adaptivecard-0.0.9.tar", last modified: Thu Jun 29 21:32:53 2023, max compression
```

## Comparing `adaptivecard-0.0.8.tar` & `adaptivecard-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.666243 adaptivecard-0.0.8/
--rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-06-29 21:21:04.000000 adaptivecard-0.0.8/LICENSE.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)      703 2023-06-29 21:27:43.666051 adaptivecard-0.0.8/PKG-INFO
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.8/README.md
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.665170 adaptivecard-0.0.8/adaptivecard/
--rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.8/adaptivecard/__init__.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.8/adaptivecard/classes.py
--rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.8/adaptivecard/exceptions.py
--rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.8/adaptivecard/mixin.py
-drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:27:43.665813 adaptivecard-0.0.8/adaptivecard.egg-info/
--rw-r--r--   0 cabutchei   (501) staff       (20)      703 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/PKG-INFO
--rw-r--r--   0 cabutchei   (501) staff       (20)      272 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/SOURCES.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/dependency_links.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-29 21:27:43.000000 adaptivecard-0.0.8/adaptivecard.egg-info/top_level.txt
--rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-29 21:27:43.666413 adaptivecard-0.0.8/setup.cfg
--rw-r--r--   0 cabutchei   (501) staff       (20)      947 2023-06-29 21:24:26.000000 adaptivecard-0.0.8/setup.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.500735 adaptivecard-0.0.9/
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1065 2023-06-29 21:21:04.000000 adaptivecard-0.0.9/LICENSE.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-06-29 21:32:53.500540 adaptivecard-0.0.9/PKG-INFO
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       87 2023-04-12 20:17:53.000000 adaptivecard-0.0.9/README.md
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.499108 adaptivecard-0.0.9/adaptivecard/
+-rw-r--r--   0 cabutchei   (501) staff       (20)        0 2023-06-18 19:00:27.000000 adaptivecard-0.0.9/adaptivecard/__init__.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)    15621 2023-06-18 21:56:27.000000 adaptivecard-0.0.9/adaptivecard/classes.py
+-rwxr-xr-x   0 cabutchei   (501) staff       (20)       46 2023-04-12 20:17:53.000000 adaptivecard-0.0.9/adaptivecard/exceptions.py
+-rw-r--r--   0 cabutchei   (501) staff       (20)     1610 2023-06-18 21:56:27.000000 adaptivecard-0.0.9/adaptivecard/mixin.py
+drwxr-xr-x   0 cabutchei   (501) staff       (20)        0 2023-06-29 21:32:53.500242 adaptivecard-0.0.9/adaptivecard.egg-info/
+-rw-r--r--   0 cabutchei   (501) staff       (20)      683 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/PKG-INFO
+-rw-r--r--   0 cabutchei   (501) staff       (20)      307 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/SOURCES.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)        1 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/dependency_links.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       10 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/requires.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       13 2023-06-29 21:32:53.000000 adaptivecard-0.0.9/adaptivecard.egg-info/top_level.txt
+-rw-r--r--   0 cabutchei   (501) staff       (20)       38 2023-06-29 21:32:53.500802 adaptivecard-0.0.9/setup.cfg
+-rw-r--r--   0 cabutchei   (501) staff       (20)      955 2023-06-29 21:32:03.000000 adaptivecard-0.0.9/setup.py
```

### Comparing `adaptivecard-0.0.8/LICENSE.txt` & `adaptivecard-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.8/PKG-INFO` & `adaptivecard-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires: typeguard
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A package that helps you design adaptive cards in an object-oriented manner.
```

### Comparing `adaptivecard-0.0.8/adaptivecard/classes.py` & `adaptivecard-0.0.9/adaptivecard/classes.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.8/adaptivecard/mixin.py` & `adaptivecard-0.0.9/adaptivecard/mixin.py`

 * *Files identical despite different names*

### Comparing `adaptivecard-0.0.8/adaptivecard.egg-info/PKG-INFO` & `adaptivecard-0.0.9/adaptivecard.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: adaptivecard
-Version: 0.0.8
+Version: 0.0.9
 Summary: Microsoft Adaptive Cards
 Author: cabutchei (Luan Paz)
 Author-email: <luropa_paz@hotmail.com>
 Keywords: python,adaptive,card,adaptive card,microsoft
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Requires: typeguard
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 A package that helps you design adaptive cards in an object-oriented manner.
```

### Comparing `adaptivecard-0.0.8/setup.py` & `adaptivecard-0.0.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
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
-    requires=[
+    install_requires=[
         'typeguard'
     ],
     keywords=['python', 'adaptive', 'card', 'adaptive card', 'microsoft'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

