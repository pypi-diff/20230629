# Comparing `tmp/autodistill-0.1.4.tar.gz` & `tmp/autodistill-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-0.1.4.tar", last modified: Thu Jun 29 11:27:29 2023, max compression
+gzip compressed data, was "autodistill-0.1.5.tar", last modified: Thu Jun 29 11:57:26 2023, max compression
```

## Comparing `autodistill-0.1.4.tar` & `autodistill-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.591657 autodistill-0.1.4/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-07 11:34:42.000000 autodistill-0.1.4/LICENSE
--rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:27:29.590795 autodistill-0.1.4/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    15196 2023-06-29 10:08:16.000000 autodistill-0.1.4/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.586595 autodistill-0.1.4/autodistill/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-29 11:27:11.000000 autodistill-0.1.4/autodistill/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.588397 autodistill-0.1.4/autodistill/classification/
--rw-r--r--   0 james      (501) staff       (20)      191 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1903 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/classification_base_model.py
--rw-r--r--   0 james      (501) staff       (20)      380 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/classification_target_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.589160 autodistill-0.1.4/autodistill/core/
--rw-r--r--   0 james      (501) staff       (20)      151 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      532 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/base_model.py
--rw-r--r--   0 james      (501) staff       (20)      116 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/ontology.py
--rw-r--r--   0 james      (501) staff       (20)      237 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/target_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.590224 autodistill-0.1.4/autodistill/detection/
--rw-r--r--   0 james      (501) staff       (20)      290 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      577 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/caption_ontology.py
--rw-r--r--   0 james      (501) staff       (20)     1761 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_base_model.py
--rw-r--r--   0 james      (501) staff       (20)      763 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_ontology.py
--rw-r--r--   0 james      (501) staff       (20)      370 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_target_model.py
--rw-r--r--   0 james      (501) staff       (20)     3259 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.587694 autodistill-0.1.4/autodistill.egg-info/
--rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      755 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      142 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 11:27:29.591852 autodistill-0.1.4/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1273 2023-06-29 11:18:18.000000 autodistill-0.1.4/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.590414 autodistill-0.1.4/test/
--rw-r--r--   0 james      (501) staff       (20)       41 2023-06-07 11:34:42.000000 autodistill-0.1.4/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.477157 autodistill-0.1.5/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-07 11:34:42.000000 autodistill-0.1.5/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:57:26.476912 autodistill-0.1.5/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    15196 2023-06-29 10:08:16.000000 autodistill-0.1.5/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.473653 autodistill-0.1.5/autodistill/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-06-29 11:57:12.000000 autodistill-0.1.5/autodistill/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.474979 autodistill-0.1.5/autodistill/classification/
+-rw-r--r--   0 james      (501) staff       (20)      191 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/classification/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1903 2023-06-29 11:50:30.000000 autodistill-0.1.5/autodistill/classification/classification_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      375 2023-06-29 11:50:45.000000 autodistill-0.1.5/autodistill/classification/classification_target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.475831 autodistill-0.1.5/autodistill/core/
+-rw-r--r--   0 james      (501) staff       (20)      151 2023-06-29 11:56:59.000000 autodistill-0.1.5/autodistill/core/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      532 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/core/base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      116 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/core/ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      237 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/core/target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.476565 autodistill-0.1.5/autodistill/detection/
+-rw-r--r--   0 james      (501) staff       (20)      290 2023-06-29 11:55:08.000000 autodistill-0.1.5/autodistill/detection/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      577 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/detection/caption_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)     1761 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/detection/detection_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/detection/detection_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      370 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/detection/detection_target_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3259 2023-06-29 11:03:41.000000 autodistill-0.1.5/autodistill/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.474450 autodistill-0.1.5/autodistill.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:57:26.000000 autodistill-0.1.5/autodistill.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      755 2023-06-29 11:57:26.000000 autodistill-0.1.5/autodistill.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 11:57:26.000000 autodistill-0.1.5/autodistill.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      142 2023-06-29 11:57:26.000000 autodistill-0.1.5/autodistill.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-06-29 11:57:26.000000 autodistill-0.1.5/autodistill.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 11:57:26.477204 autodistill-0.1.5/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1273 2023-06-29 11:18:18.000000 autodistill-0.1.5/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:57:26.476704 autodistill-0.1.5/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-07 11:34:42.000000 autodistill-0.1.5/test/test_hello.py
```

### Comparing `autodistill-0.1.4/LICENSE` & `autodistill-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/PKG-INFO` & `autodistill-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.4
+Version: 0.1.5
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-0.1.4/README.md` & `autodistill-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/classification/classification_base_model.py` & `autodistill-0.1.5/autodistill/classification/classification_base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/core/base_model.py` & `autodistill-0.1.5/autodistill/core/base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/detection/caption_ontology.py` & `autodistill-0.1.5/autodistill/detection/caption_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/detection/detection_base_model.py` & `autodistill-0.1.5/autodistill/detection/detection_base_model.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/detection/detection_ontology.py` & `autodistill-0.1.5/autodistill/detection/detection_ontology.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill/helpers.py` & `autodistill-0.1.5/autodistill/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/autodistill.egg-info/PKG-INFO` & `autodistill-0.1.5/autodistill.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.4
+Version: 0.1.5
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill-0.1.4/autodistill.egg-info/SOURCES.txt` & `autodistill-0.1.5/autodistill.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.4/setup.py` & `autodistill-0.1.5/setup.py`

 * *Files identical despite different names*

