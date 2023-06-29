# Comparing `tmp/gispandas-0.1.1.tar.gz` & `tmp/gispandas-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gispandas-0.1.1.tar", last modified: Thu Jun 29 08:01:07 2023, max compression
+gzip compressed data, was "gispandas-0.1.2.tar", last modified: Thu Jun 29 08:14:52 2023, max compression
```

## Comparing `gispandas-0.1.1.tar` & `gispandas-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,10 @@
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
+drwxrwxrwx   0        0        0        0 2023-06-29 08:14:52.116768 gispandas-0.1.2/
+-rw-rw-rw-   0        0        0      236 2023-06-29 08:14:52.115771 gispandas-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 08:14:52.114773 gispandas-0.1.2/gispandas.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-06-29 08:14:51.000000 gispandas-0.1.2/gispandas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-29 08:14:51.000000 gispandas-0.1.2/gispandas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:14:51.000000 gispandas-0.1.2/gispandas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 08:01:06.000000 gispandas-0.1.2/gispandas.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:14:51.000000 gispandas-0.1.2/gispandas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:14:52.116768 gispandas-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      621 2023-06-29 08:14:33.000000 gispandas-0.1.2/setup.py
```

### Comparing `gispandas-0.1.1/setup.py` & `gispandas-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 setup(
     name='gispandas',  # package name
     version=VERSION,  # package version
     author="HMX",
     author_email="kzdhb8023@163.com",
     description='gispandas',  # package description
```

