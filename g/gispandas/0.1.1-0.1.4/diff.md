# Comparing `tmp/gispandas-0.1.1.tar.gz` & `tmp/gispandas-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.1.tar", last modified: Thu Jun 29 08:01:07 2023, max compression
+gzip compressed data, was "gispandas-0.1.4.tar", last modified: Thu Jun 29 09:28:25 2023, max compression
```

## Comparing `gispandas-0.1.1.tar` & `gispandas-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:01:07.097169 gispandas-0.1.1/
--rw-rw-rw-   0        0        0      236 2023-06-29 08:01:07.096163 gispandas-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 08:01:07.089131 gispandas-0.1.1/gispandas.egg-info/
--rw-rw-rw-   0        0        0      236 2023-06-29 08:01:06.000000 gispandas-0.1.1/gispandas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-29 08:01:06.000000 gispandas-0.1.1/gispandas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:01:06.000000 gispandas-0.1.1/gispandas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 08:01:06.000000 gispandas-0.1.1/gispandas.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-06-29 08:01:06.000000 gispandas-0.1.1/gispandas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 08:01:07.097169 gispandas-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      621 2023-06-29 08:00:02.000000 gispandas-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:01:07.091126 gispandas-0.1.1/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 07:49:45.000000 gispandas-0.1.1/src/__init__.py
--rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.1/src/gispandas.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.067198 gispandas-0.1.4/
+-rw-rw-rw-   0        0        0      236 2023-06-29 09:28:25.065196 gispandas-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2023-06-29 09:25:50.000000 gispandas-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.059181 gispandas-0.1.4/gispandas/
+-rw-rw-rw-   0        0        0        0 2023-06-29 07:49:45.000000 gispandas-0.1.4/gispandas/__init__.py
+-rw-rw-rw-   0        0        0     2652 2023-06-29 06:54:45.000000 gispandas-0.1.4/gispandas/gispandas.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:28:25.064199 gispandas-0.1.4/gispandas.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-29 09:28:24.000000 gispandas-0.1.4/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:28:25.067198 gispandas-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      748 2023-06-29 09:27:27.000000 gispandas-0.1.4/setup.py
```

### Comparing `gispandas-0.1.1/setup.py` & `gispandas-0.1.4/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
-import os
-
-VERSION = '0.1.1'
-
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+filepath = path.join(this_directory, 'README.md')
+VERSION = '0.1.4'
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
     packages=find_packages(),
     url="https://github.com/mxhou/gispandas/",
     zip_safe=False,
     # What packages are required for this module to be executed?
-    REQUIRED = ['geopandas', 'numpy', 'geopandas','json','rasterio','rasterstats'],
+    REQUIRED = ['geopandas', 'numpy','json','rasterio','rasterstats'],
     license='MIT',
     python_requires=">=3.6",
-    keywords=['gis','geo','tif','json']
+    keywords=['gis','geo','tif','json'],
+    data_files=[filepath]
 )
```

### Comparing `gispandas-0.1.1/src/gispandas.py` & `gispandas-0.1.4/gispandas/gispandas.py`

 * *Files identical despite different names*

