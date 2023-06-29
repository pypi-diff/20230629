# Comparing `tmp/aof-0.0.8.tar.gz` & `tmp/aof-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aof-0.0.8.tar", last modified: Thu Jun 29 07:31:38 2023, max compression
+gzip compressed data, was "aof-0.0.9.tar", last modified: Thu Jun 29 07:47:47 2023, max compression
```

## Comparing `aof-0.0.8.tar` & `aof-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:31:38.199154 aof-0.0.8/
--rw-r--r--   0 kailash    (502) staff       (20)      608 2023-06-29 07:31:38.198492 aof-0.0.8/PKG-INFO
-drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:31:38.191400 aof-0.0.8/aof.egg-info/
--rw-r--r--   0 kailash    (502) staff       (20)      608 2023-06-29 07:31:38.000000 aof-0.0.8/aof.egg-info/PKG-INFO
--rw-r--r--   0 kailash    (502) staff       (20)      154 2023-06-29 07:31:38.000000 aof-0.0.8/aof.egg-info/SOURCES.txt
--rw-r--r--   0 kailash    (502) staff       (20)        1 2023-06-29 07:31:38.000000 aof-0.0.8/aof.egg-info/dependency_links.txt
--rw-r--r--   0 kailash    (502) staff       (20)        7 2023-06-29 07:31:38.000000 aof-0.0.8/aof.egg-info/top_level.txt
-drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:31:38.192475 aof-0.0.8/mypckg/
--rw-r--r--   0 kailash    (502) staff       (20)        0 2023-06-29 03:39:35.000000 aof-0.0.8/mypckg/__init__.py
--rw-r--r--   0 kailash    (502) staff       (20)      442 2023-06-29 07:02:49.000000 aof-0.0.8/mypckg/area_fig.py
--rw-r--r--   0 kailash    (502) staff       (20)       38 2023-06-29 07:31:38.199632 aof-0.0.8/setup.cfg
--rw-r--r--   0 kailash    (502) staff       (20)      769 2023-06-29 07:31:03.000000 aof-0.0.8/setup.py
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:47:47.882243 aof-0.0.9/
+-rw-r--r--   0 kailash    (502) staff       (20)      608 2023-06-29 07:47:47.881613 aof-0.0.9/PKG-INFO
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:47:47.869551 aof-0.0.9/aof.egg-info/
+-rw-r--r--   0 kailash    (502) staff       (20)      608 2023-06-29 07:47:47.000000 aof-0.0.9/aof.egg-info/PKG-INFO
+-rw-r--r--   0 kailash    (502) staff       (20)      172 2023-06-29 07:47:47.000000 aof-0.0.9/aof.egg-info/SOURCES.txt
+-rw-r--r--   0 kailash    (502) staff       (20)        1 2023-06-29 07:47:47.000000 aof-0.0.9/aof.egg-info/dependency_links.txt
+-rw-r--r--   0 kailash    (502) staff       (20)        9 2023-06-29 07:47:47.000000 aof-0.0.9/aof.egg-info/top_level.txt
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 07:47:47.878854 aof-0.0.9/area_fig/
+-rw-r--r--   0 kailash    (502) staff       (20)        0 2023-06-29 03:39:35.000000 aof-0.0.9/area_fig/__init__.py
+-rw-r--r--   0 kailash    (502) staff       (20)      444 2023-06-29 07:40:04.000000 aof-0.0.9/area_fig/area_fig.py
+-rw-r--r--   0 kailash    (502) staff       (20)       38 2023-06-29 07:42:10.000000 aof-0.0.9/area_fig/t.py
+-rw-r--r--   0 kailash    (502) staff       (20)       38 2023-06-29 07:47:47.882394 aof-0.0.9/setup.cfg
+-rw-r--r--   0 kailash    (502) staff       (20)      769 2023-06-29 07:46:24.000000 aof-0.0.9/setup.py
```

### Comparing `aof-0.0.8/PKG-INFO` & `aof-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aof
-Version: 0.0.8
+Version: 0.0.9
 Summary: Area and Perimeter calculator
 Author: Kailash Lohar
 Author-email: kailash@aganitha.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aof-0.0.8/aof.egg-info/PKG-INFO` & `aof-0.0.9/aof.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aof
-Version: 0.0.8
+Version: 0.0.9
 Summary: Area and Perimeter calculator
 Author: Kailash Lohar
 Author-email: kailash@aganitha.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aof-0.0.8/setup.py` & `aof-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aof',
-    version='0.0.8',
+    version='0.0.9',
     author='Kailash Lohar',
     author_email='kailash@aganitha.ai',
     description='Area and Perimeter calculator',
     long_description='A package to find area of square, rectangle, triangle and circle',
     packages=find_packages(),
     install_requires=[],
     classifiers=[
```

