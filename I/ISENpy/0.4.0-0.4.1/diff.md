# Comparing `tmp/ISENpy-0.4.0.tar.gz` & `tmp/ISENpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ISENpy-0.4.0.tar", last modified: Wed Jun 28 13:58:53 2023, max compression
+gzip compressed data, was "ISENpy-0.4.1.tar", last modified: Thu Jun 29 09:57:37 2023, max compression
```

## Comparing `ISENpy-0.4.0.tar` & `ISENpy-0.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-28 13:58:53.135733 ISENpy-0.4.0/
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-28 13:58:53.134927 ISENpy-0.4.0/ISENpy/
--rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-28 13:58:17.000000 ISENpy-0.4.0/ISENpy/__init__.py
--rwxr-xr-x   0 corentin   (501) staff       (20)     6915 2023-06-28 13:47:10.000000 ISENpy-0.4.0/ISENpy/client.py
--rwxr-xr-x   0 corentin   (501) staff       (20)    35038 2023-06-28 13:57:42.000000 ISENpy-0.4.0/ISENpy/dataClasses.py
-drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-28 13:58:53.135463 ISENpy-0.4.0/ISENpy.egg-info/
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-28 13:58:53.000000 ISENpy-0.4.0/ISENpy.egg-info/PKG-INFO
--rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-28 13:58:53.000000 ISENpy-0.4.0/ISENpy.egg-info/SOURCES.txt
--rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-28 13:58:53.000000 ISENpy-0.4.0/ISENpy.egg-info/dependency_links.txt
--rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-28 13:58:53.000000 ISENpy-0.4.0/ISENpy.egg-info/requires.txt
--rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-28 13:58:53.000000 ISENpy-0.4.0/ISENpy.egg-info/top_level.txt
--rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.0/LICENSE
--rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-28 13:58:53.135614 ISENpy-0.4.0/PKG-INFO
--rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.0/README.md
--rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-28 13:58:53.135772 ISENpy-0.4.0/setup.cfg
--rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-28 13:58:09.000000 ISENpy-0.4.0/setup.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 09:57:37.543637 ISENpy-0.4.1/
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 09:57:37.542231 ISENpy-0.4.1/ISENpy/
+-rwxr-xr-x   0 corentin   (501) staff       (20)     1343 2023-06-29 09:56:14.000000 ISENpy-0.4.1/ISENpy/__init__.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)     6915 2023-06-28 13:47:10.000000 ISENpy-0.4.1/ISENpy/client.py
+-rwxr-xr-x   0 corentin   (501) staff       (20)    35152 2023-06-29 09:54:05.000000 ISENpy-0.4.1/ISENpy/dataClasses.py
+drwxr-xr-x   0 corentin   (501) staff       (20)        0 2023-06-29 09:57:37.543342 ISENpy-0.4.1/ISENpy.egg-info/
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 09:57:37.000000 ISENpy-0.4.1/ISENpy.egg-info/PKG-INFO
+-rw-r--r--   0 corentin   (501) staff       (20)      233 2023-06-29 09:57:37.000000 ISENpy-0.4.1/ISENpy.egg-info/SOURCES.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        1 2023-06-29 09:57:37.000000 ISENpy-0.4.1/ISENpy.egg-info/dependency_links.txt
+-rw-r--r--   0 corentin   (501) staff       (20)       18 2023-06-29 09:57:37.000000 ISENpy-0.4.1/ISENpy.egg-info/requires.txt
+-rw-r--r--   0 corentin   (501) staff       (20)        7 2023-06-29 09:57:37.000000 ISENpy-0.4.1/ISENpy.egg-info/top_level.txt
+-rwxrwxrwx   0 corentin   (501) staff       (20)     1068 2022-08-01 16:04:58.000000 ISENpy-0.4.1/LICENSE
+-rw-r--r--   0 corentin   (501) staff       (20)     5427 2023-06-29 09:57:37.543519 ISENpy-0.4.1/PKG-INFO
+-rwxr-xr-x   0 corentin   (501) staff       (20)     4991 2023-06-28 13:43:43.000000 ISENpy-0.4.1/README.md
+-rw-r--r--   0 corentin   (501) staff       (20)       38 2023-06-29 09:57:37.543670 ISENpy-0.4.1/setup.cfg
+-rw-r--r--   0 corentin   (501) staff       (20)      848 2023-06-29 09:56:17.000000 ISENpy-0.4.1/setup.py
```

### Comparing `ISENpy-0.4.0/ISENpy/__init__.py` & `ISENpy-0.4.1/ISENpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,12 +19,12 @@
 """
 
 
 __title__ = "ISENpy"
 __author__ = "CorentinMre"
 __license__ = "MIT"
 __copyright__ = "Copyright (c) CorentinMre"
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 
 from .dataClasses import *
 from .client import *
```

### Comparing `ISENpy-0.4.0/ISENpy/client.py` & `ISENpy-0.4.1/ISENpy/client.py`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.0/ISENpy/dataClasses.py` & `ISENpy-0.4.1/ISENpy/dataClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -686,14 +686,17 @@
                 
 
             if self.infoReport["nbReport"] == 0:
                 raise Exception("The user not have any report")
             
             if self.infoReport["nbReport"] > 1 and path != None:
                 raise Exception("The user have more than one report, please choose no one path or no path")
+
+            if path == None and idReport != None:
+                path = list(self.infoReport["data"].keys())[0]
             
             if idReport == None:
                 for i in self.infoReport["data"].keys():
                     if path == None:
                         path = i
                     self.downloadReport(path, self.infoReport["data"][i])
                     return
```

### Comparing `ISENpy-0.4.0/ISENpy.egg-info/PKG-INFO` & `ISENpy-0.4.1/ISENpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.0/LICENSE` & `ISENpy-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.0/PKG-INFO` & `ISENpy-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ISENpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: A python API wrapper for ISEN-OUEST
 Home-page: https://github.com/CorentinMre/ISENpy
 Author: CorentinMre
 Author-email: corentin.marie@isen-ouest.yncrea.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ISENpy-0.4.0/README.md` & `ISENpy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ISENpy-0.4.0/setup.py` & `ISENpy-0.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='ISENpy',
-    version='0.4.0',    
+    version='0.4.1',    
     description='A python API wrapper for ISEN-OUEST',
     long_description_content_type = "text/markdown",
     long_description=long_description,
     url='https://github.com/CorentinMre/ISENpy',
     author='CorentinMre',
     author_email='corentin.marie@isen-ouest.yncrea.fr',
     license='MIT',
```

