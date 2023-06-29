# Comparing `tmp/google-cloud-network-management-1.8.2.tar.gz` & `tmp/google-cloud-network-management-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-network-management-1.8.2.tar", last modified: Tue Apr 18 13:54:20 2023, max compression
+gzip compressed data, was "google-cloud-network-management-1.9.0.tar", last modified: Thu Jun 29 16:29:49 2023, max compression
```

## Comparing `google-cloud-network-management-1.8.2.tar` & `google-cloud-network-management-1.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4733 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3784 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/network_management/
--rw-rw-r--   0 root         (0)     1003     2621 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.856801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/
--rw-rw-r--   0 root         (0)     1003     2370 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3205 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/
--rw-rw-r--   0 root         (0)     1003      789 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41915 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51661 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/client.py
--rw-rw-r--   0 root         (0)     1003     6105 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/
--rw-rw-r--   0 root         (0)     1003     1478 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8803 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    21371 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    21772 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42143 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/
--rw-rw-r--   0 root         (0)     1003     2042 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    12903 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/connectivity_test.py
--rw-rw-r--   0 root         (0)     1003     8907 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/reachability.py
--rw-rw-r--   0 root         (0)     1003    51873 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/trace.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/
--rw-r--r--   0 root         (0)     1003     4733 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1980 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-18 13:54:20.000000 google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2971 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.860801 google-cloud-network-management-1.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-18 13:54:20.864801 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   216829 2023-04-18 13:51:54.000000 google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/test_reachability_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4691 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3748 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.811269 google-cloud-network-management-1.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.811269 google-cloud-network-management-1.9.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management/
+-rw-rw-r--   0 root         (0)     1003     2621 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003     2370 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3205 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.815269 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/
+-rw-rw-r--   0 root         (0)     1003      789 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41915 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51661 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6105 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1478 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8803 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    21371 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    21772 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42143 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2042 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13540 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/connectivity_test.py
+-rw-rw-r--   0 root         (0)     1003     8907 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/reachability.py
+-rw-rw-r--   0 root         (0)     1003    51873 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/trace.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/
+-rw-r--r--   0 root         (0)     1003     4691 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1980 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-29 16:29:49.000000 google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-29 16:29:49.823268 google-cloud-network-management-1.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-29 16:29:49.819268 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   217053 2023-06-29 16:26:38.000000 google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/test_reachability_service.py
```

### Comparing `google-cloud-network-management-1.8.2/LICENSE` & `google-cloud-network-management-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/MANIFEST.in` & `google-cloud-network-management-1.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/PKG-INFO` & `google-cloud-network-management-1.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Network Management API client library
-Home-page: https://github.com/googleapis/python-network-management
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Network Management API
-========================================
+Python Client for Network Management
+====================================
 
 |stable| |pypi| |versions|
 
-`Network Management API`_: provides a collection of network performance monitoring and diagnostic capabilities.
+`Network Management`_: provides a collection of network performance monitoring and diagnostic capabilities.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
-.. _Network Management API: https://cloud.google.com/network-management
+.. _Network Management: https://cloud.google.com/network-management
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkmanagement/latest
 .. _Product Documentation:  https://cloud.google.com/network-management
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Management API.`_
+3. `Enable the Network Management.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Management API.:  https://cloud.google.com/network-management
+.. _Enable the Network Management.:  https://cloud.google.com/network-management
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-management
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Management API
+-  Read the `Client Library Documentation`_ for Network Management
    to see other available methods on the client.
--  Read the `Network Management API Product documentation`_ to learn
+-  Read the `Network Management Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Management API Product documentation:  https://cloud.google.com/network-management
+.. _Network Management Product documentation:  https://cloud.google.com/network-management
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-management-1.8.2/README.rst` & `google-cloud-network-management-1.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Network Management API
-========================================
+Python Client for Network Management
+====================================
 
 |stable| |pypi| |versions|
 
-`Network Management API`_: provides a collection of network performance monitoring and diagnostic capabilities.
+`Network Management`_: provides a collection of network performance monitoring and diagnostic capabilities.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
-.. _Network Management API: https://cloud.google.com/network-management
+.. _Network Management: https://cloud.google.com/network-management
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkmanagement/latest
 .. _Product Documentation:  https://cloud.google.com/network-management
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Management API.`_
+3. `Enable the Network Management.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Management API.:  https://cloud.google.com/network-management
+.. _Enable the Network Management.:  https://cloud.google.com/network-management
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-management
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Management API
+-  Read the `Client Library Documentation`_ for Network Management
    to see other available methods on the client.
--  Read the `Network Management API Product documentation`_ to learn
+-  Read the `Network Management Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Management API Product documentation:  https://cloud.google.com/network-management
+.. _Network Management Product documentation:  https://cloud.google.com/network-management
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management/gapic_version.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_metadata.json` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/gapic_version.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.8.2"  # {x-release-please-version}
+__version__ = "1.9.0"  # {x-release-please-version}
```

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/async_client.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/client.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/pagers.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/base.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/services/reachability_service/transports/rest.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/services/reachability_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/__init__.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/connectivity_test.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/connectivity_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,25 @@
             destination is a `global load balancer
             VIP </load-balancing/docs/load-balancing-overview>`__.
         port (int):
             The IP protocol port of the endpoint.
             Only applicable when protocol is TCP or UDP.
         instance (str):
             A Compute Engine instance URI.
+        forwarding_rule (str):
+            A forwarding rule and its corresponding IP
+            address represent the frontend configuration of
+            a Google Cloud load balancer. Forwarding rules
+            are also used for protocol forwarding, Private
+            Service Connect and other network services to
+            provide forwarding information in the control
+            plane. Format:
+            projects/{project}/global/forwardingRules/{id}
+            or
+            projects/{project}/regions/{region}/forwardingRules/{id}
         gke_master_cluster (str):
             A cluster URI for `Google Kubernetes Engine
             master <https://cloud.google.com/kubernetes-engine/docs/concepts/cluster-architecture>`__.
         cloud_sql_instance (str):
             A `Cloud SQL <https://cloud.google.com/sql>`__ instance URI.
         network (str):
             A Compute Engine network URI.
@@ -242,14 +253,18 @@
         proto.INT32,
         number=2,
     )
     instance: str = proto.Field(
         proto.STRING,
         number=3,
     )
+    forwarding_rule: str = proto.Field(
+        proto.STRING,
+        number=13,
+    )
     gke_master_cluster: str = proto.Field(
         proto.STRING,
         number=7,
     )
     cloud_sql_instance: str = proto.Field(
         proto.STRING,
         number=8,
```

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/reachability.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/reachability.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google/cloud/network_management_v1/types/trace.py` & `google-cloud-network-management-1.9.0/google/cloud/network_management_v1/types/trace.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/PKG-INFO` & `google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-network-management
-Version: 1.8.2
+Version: 1.9.0
 Summary: Google Cloud Network Management API client library
-Home-page: https://github.com/googleapis/python-network-management
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Network Management API
-========================================
+Python Client for Network Management
+====================================
 
 |stable| |pypi| |versions|
 
-`Network Management API`_: provides a collection of network performance monitoring and diagnostic capabilities.
+`Network Management`_: provides a collection of network performance monitoring and diagnostic capabilities.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-network-management.svg
    :target: https://pypi.org/project/google-cloud-network-management/
-.. _Network Management API: https://cloud.google.com/network-management
+.. _Network Management: https://cloud.google.com/network-management
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/networkmanagement/latest
 .. _Product Documentation:  https://cloud.google.com/network-management
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Network Management API.`_
+3. `Enable the Network Management.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Network Management API.:  https://cloud.google.com/network-management
+.. _Enable the Network Management.:  https://cloud.google.com/network-management
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-network-management
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Network Management API
+-  Read the `Client Library Documentation`_ for Network Management
    to see other available methods on the client.
--  Read the `Network Management API Product documentation`_ to learn
+-  Read the `Network Management Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Network Management API Product documentation:  https://cloud.google.com/network-management
+.. _Network Management Product documentation:  https://cloud.google.com/network-management
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-network-management-1.8.2/google_cloud_network_management.egg-info/SOURCES.txt` & `google-cloud-network-management-1.9.0/google_cloud_network_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/setup.py` & `google-cloud-network-management-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-network-management"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-network-management-1.8.2/tests/__init__.py` & `google-cloud-network-management-1.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/tests/unit/__init__.py` & `google-cloud-network-management-1.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/tests/unit/gapic/__init__.py` & `google-cloud-network-management-1.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/__init__.py` & `google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-network-management-1.8.2/tests/unit/gapic/network_management_v1/test_reachability_service.py` & `google-cloud-network-management-1.9.0/tests/unit/gapic/network_management_v1/test_reachability_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -3033,14 +3033,15 @@
     request_init["resource"] = {
         "name": "name_value",
         "description": "description_value",
         "source": {
             "ip_address": "ip_address_value",
             "port": 453,
             "instance": "instance_value",
+            "forwarding_rule": "forwarding_rule_value",
             "gke_master_cluster": "gke_master_cluster_value",
             "cloud_sql_instance": "cloud_sql_instance_value",
             "network": "network_value",
             "network_type": 1,
             "project_id": "project_id_value",
         },
         "destination": {},
@@ -3418,14 +3419,15 @@
     request_init["resource"] = {
         "name": "name_value",
         "description": "description_value",
         "source": {
             "ip_address": "ip_address_value",
             "port": 453,
             "instance": "instance_value",
+            "forwarding_rule": "forwarding_rule_value",
             "gke_master_cluster": "gke_master_cluster_value",
             "cloud_sql_instance": "cloud_sql_instance_value",
             "network": "network_value",
             "network_type": 1,
             "project_id": "project_id_value",
         },
         "destination": {},
@@ -3703,14 +3705,15 @@
     request_init["resource"] = {
         "name": "projects/sample1/locations/global/connectivityTests/sample2",
         "description": "description_value",
         "source": {
             "ip_address": "ip_address_value",
             "port": 453,
             "instance": "instance_value",
+            "forwarding_rule": "forwarding_rule_value",
             "gke_master_cluster": "gke_master_cluster_value",
             "cloud_sql_instance": "cloud_sql_instance_value",
             "network": "network_value",
             "network_type": 1,
             "project_id": "project_id_value",
         },
         "destination": {},
@@ -4073,14 +4076,15 @@
     request_init["resource"] = {
         "name": "projects/sample1/locations/global/connectivityTests/sample2",
         "description": "description_value",
         "source": {
             "ip_address": "ip_address_value",
             "port": 453,
             "instance": "instance_value",
+            "forwarding_rule": "forwarding_rule_value",
             "gke_master_cluster": "gke_master_cluster_value",
             "cloud_sql_instance": "cloud_sql_instance_value",
             "network": "network_value",
             "network_type": 1,
             "project_id": "project_id_value",
         },
         "destination": {},
```

