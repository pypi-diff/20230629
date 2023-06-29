# Comparing `tmp/area_fig-0.0.12.tar.gz` & `tmp/area_fig-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "area_fig-0.0.12.tar", last modified: Thu Jun 29 08:09:20 2023, max compression
+gzip compressed data, was "area_fig-0.0.13.tar", last modified: Thu Jun 29 08:23:09 2023, max compression
```

## Comparing `area_fig-0.0.12.tar` & `area_fig-0.0.13.tar`

### file list

```diff
@@ -1,9 +1,12 @@
-drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 08:09:20.880755 area_fig-0.0.12/
--rw-r--r--   0 kailash    (502) staff       (20)      614 2023-06-29 08:09:20.880349 area_fig-0.0.12/PKG-INFO
-drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 08:09:20.879703 area_fig-0.0.12/area_fig.egg-info/
--rw-r--r--   0 kailash    (502) staff       (20)      614 2023-06-29 08:09:20.000000 area_fig-0.0.12/area_fig.egg-info/PKG-INFO
--rw-r--r--   0 kailash    (502) staff       (20)      136 2023-06-29 08:09:20.000000 area_fig-0.0.12/area_fig.egg-info/SOURCES.txt
--rw-r--r--   0 kailash    (502) staff       (20)        1 2023-06-29 08:09:20.000000 area_fig-0.0.12/area_fig.egg-info/dependency_links.txt
--rw-r--r--   0 kailash    (502) staff       (20)        1 2023-06-29 08:09:20.000000 area_fig-0.0.12/area_fig.egg-info/top_level.txt
--rw-r--r--   0 kailash    (502) staff       (20)       38 2023-06-29 08:09:20.880874 area_fig-0.0.12/setup.cfg
--rw-r--r--   0 kailash    (502) staff       (20)      775 2023-06-29 08:06:51.000000 area_fig-0.0.12/setup.py
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 08:23:09.302441 area_fig-0.0.13/
+-rw-r--r--   0 kailash    (502) staff       (20)      614 2023-06-29 08:23:09.301994 area_fig-0.0.13/PKG-INFO
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 08:23:09.297485 area_fig-0.0.13/area_fig/
+-rw-r--r--   0 kailash    (502) staff       (20)        0 2023-06-29 08:21:44.000000 area_fig-0.0.13/area_fig/__init__.py
+-rw-r--r--   0 kailash    (502) staff       (20)      444 2023-06-29 07:40:04.000000 area_fig-0.0.13/area_fig/area_fig.py
+drwxr-xr-x   0 kailash    (502) staff       (20)        0 2023-06-29 08:23:09.301403 area_fig-0.0.13/area_fig.egg-info/
+-rw-r--r--   0 kailash    (502) staff       (20)      614 2023-06-29 08:23:09.000000 area_fig-0.0.13/area_fig.egg-info/PKG-INFO
+-rw-r--r--   0 kailash    (502) staff       (20)      178 2023-06-29 08:23:09.000000 area_fig-0.0.13/area_fig.egg-info/SOURCES.txt
+-rw-r--r--   0 kailash    (502) staff       (20)        1 2023-06-29 08:23:09.000000 area_fig-0.0.13/area_fig.egg-info/dependency_links.txt
+-rw-r--r--   0 kailash    (502) staff       (20)        9 2023-06-29 08:23:09.000000 area_fig-0.0.13/area_fig.egg-info/top_level.txt
+-rw-r--r--   0 kailash    (502) staff       (20)       38 2023-06-29 08:23:09.302561 area_fig-0.0.13/setup.cfg
+-rw-r--r--   0 kailash    (502) staff       (20)      775 2023-06-29 08:21:56.000000 area_fig-0.0.13/setup.py
```

### Comparing `area_fig-0.0.12/PKG-INFO` & `area_fig-0.0.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: area_fig
-Version: 0.0.12
+Version: 0.0.13
 Summary: Area and Perimeter calculator
 Author: Kailash Lohar
 Author-email: kailash@aganitha.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `area_fig-0.0.12/area_fig.egg-info/PKG-INFO` & `area_fig-0.0.13/area_fig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: area-fig
-Version: 0.0.12
+Version: 0.0.13
 Summary: Area and Perimeter calculator
 Author: Kailash Lohar
 Author-email: kailash@aganitha.ai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `area_fig-0.0.12/setup.py` & `area_fig-0.0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='area_fig',
-    version='0.0.12',
+    version='0.0.13',
     author='Kailash Lohar',
     author_email='kailash@aganitha.ai',
     description='Area and Perimeter calculator',
     long_description='A package to find area of square, rectangle, triangle and circle',
     packages=find_packages(),
     install_requires=[],
     classifiers=[
```

