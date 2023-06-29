# Comparing `tmp/scReGAT-0.0.0.tar.gz` & `tmp/scReGAT-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scReGAT-0.0.0.tar", last modified: Tue Jun  6 06:48:39 2023, max compression
+gzip compressed data, was "dist/scReGAT-0.0.1.tar", last modified: Thu Jun 29 13:49:17 2023, max compression
```

## Comparing `scReGAT-0.0.0.tar` & `scReGAT-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:48:39.004176 scReGAT-0.0.0/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-06 06:48:39.004176 scReGAT-0.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-05 08:08:33.000000 scReGAT-0.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:48:39.004176 scReGAT-0.0.0/example/
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-04 09:41:22.000000 scReGAT-0.0.0/example/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 06:48:39.004176 scReGAT-0.0.0/scReGAT.egg-info/
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-06 06:48:38.000000 scReGAT-0.0.0/scReGAT.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      192 2023-06-06 06:48:39.000000 scReGAT-0.0.0/scReGAT.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 06:48:38.000000 scReGAT-0.0.0/scReGAT.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-06-06 06:48:38.000000 scReGAT-0.0.0/scReGAT.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-06 06:48:38.000000 scReGAT-0.0.0/scReGAT.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 06:48:39.004176 scReGAT-0.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1054 2023-06-06 03:20:58.000000 scReGAT-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:49:17.938343 scReGAT-0.0.1/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-29 13:49:17.938343 scReGAT-0.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-05 08:08:33.000000 scReGAT-0.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:49:17.938343 scReGAT-0.0.1/example/
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-04 09:41:22.000000 scReGAT-0.0.1/example/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:49:17.938343 scReGAT-0.0.1/scReGAT.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-29 13:49:17.000000 scReGAT-0.0.1/scReGAT.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-29 13:49:17.000000 scReGAT-0.0.1/scReGAT.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 13:49:17.000000 scReGAT-0.0.1/scReGAT.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      120 2023-06-29 13:49:17.000000 scReGAT-0.0.1/scReGAT.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 13:49:17.000000 scReGAT-0.0.1/scReGAT.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 13:49:17.938343 scReGAT-0.0.1/scregat/
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 13:17:07.000000 scReGAT-0.0.1/scregat/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    25982 2023-06-29 11:45:18.000000 scReGAT-0.0.1/scregat/data_process.py
+-rwxr-xr-x   0 root         (0) root         (0)    23602 2023-04-03 07:03:21.000000 scReGAT-0.0.1/scregat/data_process_1.py
+-rwxr-xr-x   0 root         (0) root         (0)    27891 2023-04-03 11:48:59.000000 scReGAT-0.0.1/scregat/data_process_2.py
+-rwxr-xr-x   0 root         (0) root         (0)    22374 2023-06-08 06:29:07.000000 scReGAT-0.0.1/scregat/model.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 13:49:17.938343 scReGAT-0.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-06-29 13:41:35.000000 scReGAT-0.0.1/setup.py
```

### Comparing `scReGAT-0.0.0/setup.py` & `scReGAT-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 NAME = 'scReGAT'
 DESCRIPTION = \
     'A GAT-based computational framework to predict long-range gene regulatory relationships'
 URL = 'https://github.com/Drizzle-Zhang/scReGAT'
 EMAIL = 'zhang_yu18@fudan.edu.cn'
 AUTHOR = 'Yu Zhang'
 REQUIRES_PYTHON = '>=3.8.3'
-VERSION = '0.0.0'
+VERSION = '0.0.1'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "numpy", "pandas", "sklearn", "scipy", "statsmodels", "anndata", "scanpy", "episcanpy", "cosg",
     "torch", "torch_geometric", "captum", "audtorch", "torch_sparse",
 ]
```

