# Comparing `tmp/large-image-source-dicom-1.23.1.dev6.tar.gz` & `tmp/large-image-source-dicom-1.23.1.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.23.1.dev6.tar", last modified: Tue Jun 27 14:26:40 2023, max compression
+gzip compressed data, was "large-image-source-dicom-1.23.1.dev8.tar", last modified: Tue Jun 27 17:24:26 2023, max compression
```

## Comparing `large-image-source-dicom-1.23.1.dev6.tar` & `large-image-source-dicom-1.23.1.dev8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:26:40.610122 large-image-source-dicom-1.23.1.dev6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-06-27 14:26:40.606122 large-image-source-dicom-1.23.1.dev6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:26:40.606122 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10125 2023-06-27 14:25:57.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-06-27 14:25:57.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 14:26:40.606122 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-27 14:26:40.000000 large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-27 14:26:40.610122 large-image-source-dicom-1.23.1.dev6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-06-27 14:25:57.000000 large-image-source-dicom-1.23.1.dev6/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:24:26.590877 large-image-source-dicom-1.23.1.dev8/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-06-27 17:24:26.590877 large-image-source-dicom-1.23.1.dev8/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:24:26.590877 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10125 2023-06-27 17:23:37.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-06-27 17:23:37.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-27 17:24:26.590877 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-27 17:24:26.000000 large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-27 17:24:26.590877 large-image-source-dicom-1.23.1.dev8/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-06-27 17:23:37.000000 large-image-source-dicom-1.23.1.dev8/setup.py
```

### Comparing `large-image-source-dicom-1.23.1.dev6/LICENSE` & `large-image-source-dicom-1.23.1.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.1.dev6/PKG-INFO` & `large-image-source-dicom-1.23.1.dev8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.23.1.dev6
+Version: 1.23.1.dev8
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.23.1.dev6/README.rst` & `large-image-source-dicom-1.23.1.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.1.dev6/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.23.1.dev8/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.1.dev6/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.23.1.dev8/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.1.dev6/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.23.1.dev8/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.23.1.dev6
+Version: 1.23.1.dev8
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.23.1.dev6/setup.py` & `large-image-source-dicom-1.23.1.dev8/setup.py`

 * *Files identical despite different names*

