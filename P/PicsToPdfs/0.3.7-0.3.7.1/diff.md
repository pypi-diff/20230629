# Comparing `tmp/PicsToPdfs-0.3.7.tar.gz` & `tmp/PicsToPdfs-0.3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.3.7.tar", last modified: Thu May 11 09:19:31 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.7.1.tar", last modified: Thu Jun 29 09:50:52 2023, max compression
```

## Comparing `PicsToPdfs-0.3.7.tar` & `PicsToPdfs-0.3.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 09:19:31.614936 PicsToPdfs-0.3.7/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0      387 2023-05-11 09:19:31.614936 PicsToPdfs-0.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-11 09:19:31.598937 PicsToPdfs-0.3.7/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-05-11 09:19:31.608937 PicsToPdfs-0.3.7/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7/PicsToPdfs/Function/__init__.py
--rw-rw-rw-   0        0        0    59904 2023-04-28 06:28:34.000000 PicsToPdfs-0.3.7/PicsToPdfs/Function/imgToPdf.pyd
--rw-rw-rw-   0        0        0   110592 2023-05-11 09:17:48.000000 PicsToPdfs-0.3.7/PicsToPdfs/PicsToPdfs.pyd
-drwxrwxrwx   0        0        0        0 2023-05-11 09:19:31.612937 PicsToPdfs-0.3.7/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0    79872 2023-05-11 09:17:53.000000 PicsToPdfs-0.3.7/PicsToPdfs/Ui/PicToPdfUi.pyd
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 09:19:31.605941 PicsToPdfs-0.3.7/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      387 2023-05-11 09:19:31.000000 PicsToPdfs-0.3.7/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-11 09:19:31.000000 PicsToPdfs-0.3.7/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 09:19:31.000000 PicsToPdfs-0.3.7/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-11 09:19:31.000000 PicsToPdfs-0.3.7/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.7/README.md
--rw-rw-rw-   0        0        0      136 2023-05-11 09:19:31.615939 PicsToPdfs-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0      959 2023-05-11 09:11:32.000000 PicsToPdfs-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:50:52.851892 PicsToPdfs-0.3.7.1/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      389 2023-06-29 09:50:52.851892 PicsToPdfs-0.3.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 09:50:52.838895 PicsToPdfs-0.3.7.1/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-06-29 09:50:52.846892 PicsToPdfs-0.3.7.1/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/Function/__init__.py
+-rw-rw-rw-   0        0        0    66048 2023-06-29 09:49:36.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/Function/imgToPdf.pyd
+-rw-rw-rw-   0        0        0   120320 2023-06-29 09:49:41.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/PicsToPdfs.pyd
+drwxrwxrwx   0        0        0        0 2023-06-29 09:50:52.849893 PicsToPdfs-0.3.7.1/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0    81920 2023-06-29 09:49:46.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/Ui/PicToPdfUi.pyd
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.7.1/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:50:52.844892 PicsToPdfs-0.3.7.1/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      389 2023-06-29 09:50:52.000000 PicsToPdfs-0.3.7.1/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-29 09:50:52.000000 PicsToPdfs-0.3.7.1/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:50:52.000000 PicsToPdfs-0.3.7.1/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 09:50:52.000000 PicsToPdfs-0.3.7.1/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.7.1/README.md
+-rw-rw-rw-   0        0        0      136 2023-06-29 09:50:52.853900 PicsToPdfs-0.3.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      961 2023-06-29 09:48:34.000000 PicsToPdfs-0.3.7.1/setup.py
```

### Comparing `PicsToPdfs-0.3.7/LICENSE.txt` & `PicsToPdfs-0.3.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.3.7/setup.py` & `PicsToPdfs-0.3.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 3
 PATCH = 7
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.1"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "PicsToPdfs",
     version=VERSION,
```

