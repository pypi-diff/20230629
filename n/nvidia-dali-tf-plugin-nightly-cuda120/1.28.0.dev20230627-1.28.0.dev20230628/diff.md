# Comparing `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627.tar.gz` & `tmp/nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627.tar", last modified: Wed Jun 28 07:03:42 2023, max compression
+gzip compressed data, was "nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628.tar", last modified: Thu Jun 29 08:03:27 2023, max compression
```

## Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627.tar` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-28 07:03:42.158458 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/ERROR.txt
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/LICENSE.md
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/PACKAGE_NAME
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-28 07:03:42.158458 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/README.rst
-drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-28 07:03:42.158458 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-28 07:03:42.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
--rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-28 07:03:42.162458 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/setup.cfg
--rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/setup.py
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 08:03:27.830496 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      469 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/ERROR.txt
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)    11336 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/LICENSE.md
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       37 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/PACKAGE_NAME
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-29 08:03:27.830496 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      316 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/README.rst
+drwxr-xr-x   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        0 2023-06-29 08:03:27.830496 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     1708 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)      297 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/SOURCES.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)        1 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/dependency_links.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       22 2023-06-29 08:03:27.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/top_level.txt
+-rw-r--r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)       38 2023-06-29 08:03:27.830496 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/setup.cfg
+-rw-rw-r--   0 svc-compute-packagin (25503) sw-cuda-installer  (2174)     4560 2023-06-14 04:38:44.000000 nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/setup.py
```

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/LICENSE.md` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/nvidia_dali_tf_plugin_nightly_cuda120.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-tf-plugin-nightly-cuda120
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

### Comparing `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230627/setup.py` & `nvidia-dali-tf-plugin-nightly-cuda120-1.28.0.dev20230628/setup.py`

 * *Files identical despite different names*

