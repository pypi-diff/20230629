# Comparing `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230627.tar.gz` & `tmp/nvidia-dali-nightly-cuda120-1.28.0.dev20230628.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230627.tar", last modified: Wed Jun 28 07:04:46 2023, max compression
+gzip compressed data, was "nvidia-dali-nightly-cuda120-1.28.0.dev20230628.tar", last modified: Thu Jun 29 08:04:30 2023, max compression
```

## Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230627.tar` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230628.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-28 07:04:46.729746 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-28 07:04:46.729746 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-28 07:04:46.729746 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-28 07:04:46.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-28 07:04:46.729746 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230627/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 08:04:30.141816 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      459 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       27 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-29 08:04:30.141816 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      286 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 08:04:30.141816 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1668 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      257 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-29 08:04:30.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-29 08:04:30.141816 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-nightly-cuda120-1.28.0.dev20230628/setup.py
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230627/LICENSE.md` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230628/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230627/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230628/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230627
+Version: 1.28.0.dev20230628
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.28.0.dev20230627
+Version: 1.28.0.dev20230628
 Summary: A fake package to warn the user they are not installing the correct package.
 Home-page: https://github.com/NVIDIA
 Download-URL: https://github.com/NVIDIA
 Author: Kitmaker
 Author-email: kitmaker@nvidia.com
 Maintainer: Kitmaker
 Maintainer-email: kitmaker@nvidia.com
```

### Comparing `nvidia-dali-nightly-cuda120-1.28.0.dev20230627/setup.py` & `nvidia-dali-nightly-cuda120-1.28.0.dev20230628/setup.py`

 * *Files identical despite different names*

