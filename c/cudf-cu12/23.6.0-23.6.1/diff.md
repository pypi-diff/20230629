# Comparing `tmp/cudf-cu12-23.6.0.tar.gz` & `tmp/cudf-cu12-23.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudf-cu12-23.6.0.tar", last modified: Tue Jun 13 15:57:43 2023, max compression
+gzip compressed data, was "cudf-cu12-23.6.1.tar", last modified: Thu Jun 29 16:58:15 2023, max compression
```

## Comparing `cudf-cu12-23.6.0.tar` & `cudf-cu12-23.6.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-13 15:57:43.463798 cudf-cu12-23.6.0/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-13 15:37:00.000000 cudf-cu12-23.6.0/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-13 15:57:43.462798 cudf-cu12-23.6.0/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-13 15:57:43.461798 cudf-cu12-23.6.0/cudf_cu12.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/cudf_cu12.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/cudf_cu12.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/cudf_cu12.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-13 15:57:43.000000 cudf-cu12-23.6.0/cudf_cu12.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-13 15:57:43.463798 cudf-cu12-23.6.0/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-13 15:37:00.000000 cudf-cu12-23.6.0/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 16:58:15.114101 cudf-cu12-23.6.1/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      441 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 14:12:21.000000 cudf-cu12-23.6.1/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        9 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-29 16:58:15.114101 cudf-cu12-23.6.1/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      232 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 16:58:15.114101 cudf-cu12-23.6.1/cudf_cu12.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1584 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/cudf_cu12.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      185 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/cudf_cu12.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/cudf_cu12.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-29 16:58:15.000000 cudf-cu12-23.6.1/cudf_cu12.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-29 16:58:15.114101 cudf-cu12-23.6.1/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 14:12:21.000000 cudf-cu12-23.6.1/setup.py
```

### Comparing `cudf-cu12-23.6.0/LICENSE.md` & `cudf-cu12-23.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cudf-cu12-23.6.0/PKG-INFO` & `cudf-cu12-23.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf-cu12
-Version: 23.6.0
+Version: 23.6.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf-cu12-23.6.0/cudf_cu12.egg-info/PKG-INFO` & `cudf-cu12-23.6.1/cudf_cu12.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cudf-cu12
-Version: 23.6.0
+Version: 23.6.1
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `cudf-cu12-23.6.0/setup.py` & `cudf-cu12-23.6.1/setup.py`

 * *Files identical despite different names*

