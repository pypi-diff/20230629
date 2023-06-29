# Comparing `tmp/czmodel-5.0.0.tar.gz` & `tmp/czmodel-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "czmodel-5.0.0.tar", last modified: Thu Sep 15 14:11:25 2022, max compression
+gzip compressed data, was "czmodel-5.1.0.tar", last modified: Thu Jun 29 16:27:00 2023, max compression
```

## Comparing `czmodel-5.0.0.tar` & `czmodel-5.1.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/
--rw-rw-rw-   0        0        0    11558 2022-09-15 14:10:44.000000 czmodel-5.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0       26 2022-09-15 14:10:44.000000 czmodel-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0      193 2022-09-15 14:10:44.000000 czmodel-5.0.0/NOTICE.txt
--rw-rw-rw-   0        0        0    20822 2022-09-15 14:11:25.897092 czmodel-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    19830 2022-09-15 14:10:44.000000 czmodel-5.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.881463 czmodel-5.0.0/czmodel/
--rw-rw-rw-   0        0        0     1055 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.881463 czmodel-5.0.0/czmodel/core/
--rw-rw-rw-   0        0        0      980 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/__init__.py
--rw-rw-rw-   0        0        0     2762 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/convert.py
--rw-rw-rw-   0        0        0    12389 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/legacy_model_metadata.py
--rw-rw-rw-   0        0        0     1969 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/legacy_model_spec.py
--rw-rw-rw-   0        0        0     7251 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/model_metadata.py
--rw-rw-rw-   0        0        0     2276 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/model_spec.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/czmodel/core/util/
--rw-rw-rw-   0        0        0      842 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/__init__.py
--rw-rw-rw-   0        0        0     4037 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/_extract_model.py
--rw-rw-rw-   0        0        0     1741 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/argument_parsing.py
--rw-rw-rw-   0        0        0     2281 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/base_convert.py
--rw-rw-rw-   0        0        0     3178 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/color_generation.py
--rw-rw-rw-   0        0        0     3842 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/common.py
--rw-rw-rw-   0        0        0     4851 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/model_packing.py
--rw-rw-rw-   0        0        0     4658 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/core/util/onnx_export.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/czmodel/pytorch/
--rw-rw-rw-   0        0        0     1029 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/__init__.py
--rw-rw-rw-   0        0        0     6960 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/convert.py
--rw-rw-rw-   0        0        0     1458 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/legacy_model_spec.py
--rw-rw-rw-   0        0        0     1651 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/model_spec.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/czmodel/pytorch/util/
--rw-rw-rw-   0        0        0      843 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/util/__init__.py
--rw-rw-rw-   0        0        0     9872 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/pytorch/util/torch_export.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/czmodel/tensorflow/
--rw-rw-rw-   0        0        0     1041 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/__init__.py
--rw-rw-rw-   0        0        0     8497 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/convert.py
--rw-rw-rw-   0        0        0     1470 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/legacy_model_spec.py
--rw-rw-rw-   0        0        0     1674 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/model_spec.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.897092 czmodel-5.0.0/czmodel/tensorflow/util/
--rw-rw-rw-   0        0        0      846 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/util/__init__.py
--rw-rw-rw-   0        0        0     7545 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/util/keras_export.py
--rw-rw-rw-   0        0        0     9959 2022-09-15 14:10:44.000000 czmodel-5.0.0/czmodel/tensorflow/util/transforms.py
-drwxrwxrwx   0        0        0        0 2022-09-15 14:11:25.881463 czmodel-5.0.0/czmodel.egg-info/
--rw-rw-rw-   0        0        0    20822 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1162 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-15 14:11:25.000000 czmodel-5.0.0/czmodel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1777 2022-09-15 14:11:25.897092 czmodel-5.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4007 2022-09-15 14:10:44.000000 czmodel-5.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.480723 czmodel-5.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-06-29 16:25:49.000000 czmodel-5.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       26 2023-06-29 16:25:49.000000 czmodel-5.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      193 2023-06-29 16:25:49.000000 czmodel-5.1.0/NOTICE.txt
+-rw-rw-rw-   0        0        0    20865 2023-06-29 16:27:00.480723 czmodel-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    19830 2023-06-29 16:25:49.000000 czmodel-5.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.449473 czmodel-5.1.0/czmodel/
+-rw-rw-rw-   0        0        0     1055 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.465098 czmodel-5.1.0/czmodel/core/
+-rw-rw-rw-   0        0        0      980 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/convert.py
+-rw-rw-rw-   0        0        0    12389 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/legacy_model_metadata.py
+-rw-rw-rw-   0        0        0     1969 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/legacy_model_spec.py
+-rw-rw-rw-   0        0        0     7251 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/model_metadata.py
+-rw-rw-rw-   0        0        0     2276 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/model_spec.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.465098 czmodel-5.1.0/czmodel/core/util/
+-rw-rw-rw-   0        0        0      842 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/__init__.py
+-rw-rw-rw-   0        0        0     4037 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/_extract_model.py
+-rw-rw-rw-   0        0        0     1741 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/argument_parsing.py
+-rw-rw-rw-   0        0        0     2281 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/base_convert.py
+-rw-rw-rw-   0        0        0     3178 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/color_generation.py
+-rw-rw-rw-   0        0        0     3842 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/common.py
+-rw-rw-rw-   0        0        0     4851 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/model_packing.py
+-rw-rw-rw-   0        0        0     4658 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/core/util/onnx_export.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.465098 czmodel-5.1.0/czmodel/pytorch/
+-rw-rw-rw-   0        0        0     1029 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     6960 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/convert.py
+-rw-rw-rw-   0        0        0     1458 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/legacy_model_spec.py
+-rw-rw-rw-   0        0        0     1651 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/model_spec.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.465098 czmodel-5.1.0/czmodel/pytorch/util/
+-rw-rw-rw-   0        0        0      843 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/util/__init__.py
+-rw-rw-rw-   0        0        0     9872 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/pytorch/util/torch_export.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.480723 czmodel-5.1.0/czmodel/tensorflow/
+-rw-rw-rw-   0        0        0     1041 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/__init__.py
+-rw-rw-rw-   0        0        0     8497 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/convert.py
+-rw-rw-rw-   0        0        0     1470 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/legacy_model_spec.py
+-rw-rw-rw-   0        0        0     1674 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/model_spec.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.480723 czmodel-5.1.0/czmodel/tensorflow/util/
+-rw-rw-rw-   0        0        0      846 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/util/__init__.py
+-rw-rw-rw-   0        0        0     7545 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/util/keras_export.py
+-rw-rw-rw-   0        0        0     9959 2023-06-29 16:25:49.000000 czmodel-5.1.0/czmodel/tensorflow/util/transforms.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:27:00.449473 czmodel-5.1.0/czmodel.egg-info/
+-rw-rw-rw-   0        0        0    20865 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1162 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 16:27:00.000000 czmodel-5.1.0/czmodel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1782 2023-06-29 16:27:00.480723 czmodel-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3902 2023-06-29 16:25:49.000000 czmodel-5.1.0/setup.py
```

### Comparing `czmodel-5.0.0/LICENSE.txt` & `czmodel-5.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/PKG-INFO` & `czmodel-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: czmodel
-Version: 5.0.0
+Version: 5.1.0
 Summary: A conversion tool for TensorFlow or ONNX ANNs to CZANN
-Home-page: UNKNOWN
 Author: Sebastian Soyer
 Author-email: sebastian.soyer@zeiss.com
-License: UNKNOWN
 Project-URL: ZEN Intellesis, https://www.zeiss.com/microscopy/int/products/microscope-software/zen-intellesis-image-segmentation-by-deep-learning.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tensorflow
 Provides-Extra: pytorch
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
@@ -400,9 +399,7 @@
 {
   "Id": "064587eb-d5a1-4434-82fc-2fbc9f5871f9",
   "Type": "Regression",
   "InputShape": [1024, 1024, 3],
   "OutputShape": [1024, 1024, 3]
 }
 ```
-
-
```

### Comparing `czmodel-5.0.0/README.md` & `czmodel-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/__init__.py` & `czmodel-5.1.0/czmodel/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/__init__.py` & `czmodel-5.1.0/czmodel/core/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/convert.py` & `czmodel-5.1.0/czmodel/core/convert.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/legacy_model_metadata.py` & `czmodel-5.1.0/czmodel/core/legacy_model_metadata.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/legacy_model_spec.py` & `czmodel-5.1.0/czmodel/core/legacy_model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/model_metadata.py` & `czmodel-5.1.0/czmodel/core/model_metadata.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/model_spec.py` & `czmodel-5.1.0/czmodel/core/model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/__init__.py` & `czmodel-5.1.0/czmodel/core/util/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/_extract_model.py` & `czmodel-5.1.0/czmodel/core/util/_extract_model.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/argument_parsing.py` & `czmodel-5.1.0/czmodel/core/util/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/base_convert.py` & `czmodel-5.1.0/czmodel/core/util/base_convert.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/color_generation.py` & `czmodel-5.1.0/czmodel/core/util/color_generation.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/common.py` & `czmodel-5.1.0/czmodel/core/util/common.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/model_packing.py` & `czmodel-5.1.0/czmodel/core/util/model_packing.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/core/util/onnx_export.py` & `czmodel-5.1.0/czmodel/core/util/onnx_export.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/__init__.py` & `czmodel-5.1.0/czmodel/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/convert.py` & `czmodel-5.1.0/czmodel/pytorch/convert.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/legacy_model_spec.py` & `czmodel-5.1.0/czmodel/pytorch/legacy_model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/model_spec.py` & `czmodel-5.1.0/czmodel/pytorch/model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/util/__init__.py` & `czmodel-5.1.0/czmodel/pytorch/util/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/pytorch/util/torch_export.py` & `czmodel-5.1.0/czmodel/pytorch/util/torch_export.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/__init__.py` & `czmodel-5.1.0/czmodel/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/convert.py` & `czmodel-5.1.0/czmodel/tensorflow/convert.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/legacy_model_spec.py` & `czmodel-5.1.0/czmodel/tensorflow/legacy_model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/model_spec.py` & `czmodel-5.1.0/czmodel/tensorflow/model_spec.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/util/__init__.py` & `czmodel-5.1.0/czmodel/tensorflow/util/__init__.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/util/keras_export.py` & `czmodel-5.1.0/czmodel/tensorflow/util/keras_export.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel/tensorflow/util/transforms.py` & `czmodel-5.1.0/czmodel/tensorflow/util/transforms.py`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/czmodel.egg-info/PKG-INFO` & `czmodel-5.1.0/czmodel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: czmodel
-Version: 5.0.0
+Version: 5.1.0
 Summary: A conversion tool for TensorFlow or ONNX ANNs to CZANN
-Home-page: UNKNOWN
 Author: Sebastian Soyer
 Author-email: sebastian.soyer@zeiss.com
-License: UNKNOWN
 Project-URL: ZEN Intellesis, https://www.zeiss.com/microscopy/int/products/microscope-software/zen-intellesis-image-segmentation-by-deep-learning.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7,<3.10
+Requires-Python: >=3.7,<3.12
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: tensorflow
 Provides-Extra: pytorch
 License-File: LICENSE.txt
 License-File: NOTICE.txt
 
@@ -400,9 +399,7 @@
 {
   "Id": "064587eb-d5a1-4434-82fc-2fbc9f5871f9",
   "Type": "Regression",
   "InputShape": [1024, 1024, 3],
   "OutputShape": [1024, 1024, 3]
 }
 ```
-
-
```

### Comparing `czmodel-5.0.0/czmodel.egg-info/SOURCES.txt` & `czmodel-5.1.0/czmodel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `czmodel-5.0.0/setup.cfg` & `czmodel-5.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,112 +1,112 @@
 00000000: 5b66 6c61 6b65 385d 0d0a 646f 6373 7472  [flake8]..docstr
 00000010: 696e 672d 636f 6e76 656e 7469 6f6e 203d  ing-convention =
 00000020: 2067 6f6f 676c 650d 0a6d 6178 2d6c 696e   google..max-lin
 00000030: 652d 6c65 6e67 7468 203d 2031 3230 0d0a  e-length = 120..
 00000040: 6578 7465 6e64 2d69 676e 6f72 6520 3d20  extend-ignore = 
 00000050: 4432 3035 2c44 3431 352c 4532 3033 2c46  D205,D415,E203,F
-00000060: 3430 310d 0a70 6572 2d66 696c 652d 6967  401..per-file-ig
-00000070: 6e6f 7265 7320 3d20 0d0a 0973 6574 7570  nores = ...setup
-00000080: 2e70 793a 2045 3530 310d 0a0d 0a5b 4d41  .py: E501....[MA
-00000090: 5354 4552 5d0d 0a69 676e 6f72 6520 3d20  STER]..ignore = 
-000000a0: 0d0a 6c6f 6164 2d70 6c75 6769 6e73 203d  ..load-plugins =
-000000b0: 2070 796c 696e 742e 6578 7465 6e73 696f   pylint.extensio
-000000c0: 6e73 2e64 6f63 7061 7261 6d73 0d0a 0d0a  ns.docparams....
-000000d0: 5b70 796c 696e 745d 0d0a 6163 6365 7074  [pylint]..accept
-000000e0: 2d6e 6f2d 7061 7261 6d2d 646f 6320 3d20  -no-param-doc = 
-000000f0: 6e6f 0d0a 6465 6661 756c 742d 646f 6373  no..default-docs
-00000100: 7472 696e 672d 7479 7065 203d 2067 6f6f  tring-type = goo
-00000110: 676c 650d 0a63 6f6e 7465 7874 6d61 6e61  gle..contextmana
-00000120: 6765 722d 6465 636f 7261 746f 7273 203d  ger-decorators =
-00000130: 2063 6f6e 7465 7874 6c69 622e 636f 6e74   contextlib.cont
-00000140: 6578 746d 616e 6167 6572 2c20 7465 6e73  extmanager, tens
-00000150: 6f72 666c 6f77 2e70 7974 686f 6e2e 7574  orflow.python.ut
-00000160: 696c 2e74 665f 636f 6e74 6578 746c 6962  il.tf_contextlib
-00000170: 2e63 6f6e 7465 7874 6d61 6e61 6765 720d  .contextmanager.
-00000180: 0a6c 6f67 6769 6e67 2d66 6f72 6d61 742d  .logging-format-
-00000190: 7374 796c 6520 3d20 6e65 770d 0a6d 6178  style = new..max
-000001a0: 2d6c 696e 652d 6c65 6e67 7468 203d 2031  -line-length = 1
-000001b0: 3230 0d0a 6a6f 6273 203d 2031 0d0a 6469  20..jobs = 1..di
-000001c0: 7361 626c 6520 3d20 6272 6f61 642d 6578  sable = broad-ex
-000001d0: 6365 7074 2c0d 0a09 696e 7661 6c69 642d  cept,...invalid-
-000001e0: 6e61 6d65 2c0d 0a09 6e6f 2d6d 656d 6265  name,...no-membe
-000001f0: 722c 0d0a 096e 6f2d 6e61 6d65 2d69 6e2d  r,...no-name-in-
-00000200: 6d6f 6475 6c65 2c0d 0a09 746f 6f2d 6665  module,...too-fe
-00000210: 772d 7075 626c 6963 2d6d 6574 686f 6473  w-public-methods
-00000220: 2c0d 0a09 746f 6f2d 6d61 6e79 2d70 7562  ,...too-many-pub
-00000230: 6c69 632d 6d65 7468 6f64 732c 0d0a 0974  lic-methods,...t
-00000240: 6f6f 2d6d 616e 792d 6172 6775 6d65 6e74  oo-many-argument
-00000250: 732c 0d0a 0974 6f6f 2d6d 616e 792d 6272  s,...too-many-br
-00000260: 616e 6368 6573 2c0d 0a09 746f 6f2d 6d61  anches,...too-ma
-00000270: 6e79 2d6c 696e 6573 2c0d 0a09 746f 6f2d  ny-lines,...too-
-00000280: 6d61 6e79 2d6c 6f63 616c 732c 0d0a 0974  many-locals,...t
-00000290: 6f6f 2d6d 616e 792d 696e 7374 616e 6365  oo-many-instance
-000002a0: 2d61 7474 7269 6275 7465 732c 0d0a 0974  -attributes,...t
-000002b0: 6f6f 2d6d 616e 792d 7374 6174 656d 656e  oo-many-statemen
-000002c0: 7473 2c0d 0a09 676c 6f62 616c 2d73 7461  ts,...global-sta
-000002d0: 7465 6d65 6e74 2c0d 0a09 7072 6f74 6563  tement,...protec
-000002e0: 7465 642d 6163 6365 7373 2c0d 0a09 7573  ted-access,...us
-000002f0: 652d 612d 6765 6e65 7261 746f 722c 0d0a  e-a-generator,..
-00000300: 0975 7365 6c65 7373 2d70 6172 616d 2d64  .useless-param-d
-00000310: 6f63 2c0d 0a09 7573 656c 6573 732d 7479  oc,...useless-ty
-00000320: 7065 2d64 6f63 2c0d 0a09 6d69 7373 696e  pe-doc,...missin
-00000330: 672d 7265 7475 726e 2d74 7970 652d 646f  g-return-type-do
-00000340: 632c 0d0a 096d 6973 7369 6e67 2d79 6965  c,...missing-yie
-00000350: 6c64 2d74 7970 652d 646f 632c 0d0a 096d  ld-type-doc,...m
-00000360: 6973 7369 6e67 2d74 7970 652d 646f 632c  issing-type-doc,
-00000370: 0d0a 096d 6973 7369 6e67 2d79 6965 6c64  ...missing-yield
-00000380: 2d64 6f63 2c0d 0a09 6d69 7373 696e 672d  -doc,...missing-
-00000390: 7265 7475 726e 2d64 6f63 2c0d 0a09 756e  return-doc,...un
-000003a0: 7370 6563 6966 6965 642d 656e 636f 6469  specified-encodi
-000003b0: 6e67 2c0d 0a09 6475 706c 6963 6174 652d  ng,...duplicate-
-000003c0: 636f 6465 2c0d 0a09 696d 706f 7274 2d65  code,...import-e
-000003d0: 7272 6f72 0d0a 0d0a 5b70 796c 696e 742e  rror....[pylint.
-000003e0: 6d65 7373 6167 6573 5f63 6f6e 7472 6f6c  messages_control
-000003f0: 5d0d 0a64 6973 6162 6c65 203d 2052 3034  ]..disable = R04
-00000400: 3032 0d0a 7661 7269 6162 6c65 2d72 6778  02..variable-rgx
-00000410: 203d 205e 283f 212e 2a28 5b5f 5d29 5c31   = ^(?!.*([_])\1
-00000420: 295e 283f 3d2e 7b31 2c33 307d 2429 5b61  )^(?=.{1,30}$)[a
-00000430: 2d7a 5f5d 5b61 2d7a 302d 395f 5d7b 302c  -z_][a-z0-9_]{0,
-00000440: 7d24 0d0a 0d0a 5b6d 7970 795d 0d0a 6469  }$....[mypy]..di
-00000450: 7361 6c6c 6f77 5f75 6e74 7970 6564 5f64  sallow_untyped_d
-00000460: 6566 7320 3d20 5472 7565 0d0a 6469 7361  efs = True..disa
-00000470: 6c6c 6f77 5f69 6e63 6f6d 706c 6574 655f  llow_incomplete_
-00000480: 6465 6673 203d 2054 7275 650d 0a63 6865  defs = True..che
-00000490: 636b 5f75 6e74 7970 6564 5f64 6566 7320  ck_untyped_defs 
-000004a0: 3d20 5472 7565 0d0a 6e6f 5f69 6d70 6c69  = True..no_impli
-000004b0: 6369 745f 6f70 7469 6f6e 616c 203d 2054  cit_optional = T
-000004c0: 7275 650d 0a73 7472 6963 745f 6f70 7469  rue..strict_opti
-000004d0: 6f6e 616c 203d 2054 7275 650d 0a73 7472  onal = True..str
-000004e0: 6963 745f 6571 7561 6c69 7479 203d 2054  ict_equality = T
-000004f0: 7275 650d 0a77 6172 6e5f 7265 6475 6e64  rue..warn_redund
-00000500: 616e 745f 6361 7374 7320 3d20 5472 7565  ant_casts = True
-00000510: 0d0a 7761 726e 5f75 6e75 7365 645f 6967  ..warn_unused_ig
-00000520: 6e6f 7265 7320 3d20 5472 7565 0d0a 7761  nores = True..wa
-00000530: 726e 5f72 6574 7572 6e5f 616e 7920 3d20  rn_return_any = 
-00000540: 5472 7565 0d0a 7761 726e 5f75 6e75 7365  True..warn_unuse
-00000550: 645f 636f 6e66 6967 7320 3d20 5472 7565  d_configs = True
-00000560: 0d0a 7761 726e 5f75 6e72 6561 6368 6162  ..warn_unreachab
-00000570: 6c65 203d 2054 7275 650d 0a6e 6f5f 696d  le = True..no_im
-00000580: 706c 6963 6974 5f72 6565 7870 6f72 7420  plicit_reexport 
-00000590: 3d20 5472 7565 0d0a 0d0a 5b6d 7970 792d  = True....[mypy-
-000005a0: 7465 6e73 6f72 666c 6f77 2e2a 5d0d 0a69  tensorflow.*]..i
-000005b0: 676e 6f72 655f 6d69 7373 696e 675f 696d  gnore_missing_im
-000005c0: 706f 7274 7320 3d20 5472 7565 0d0a 0d0a  ports = True....
-000005d0: 5b6d 7970 792d 746f 7263 682e 2a5d 0d0a  [mypy-torch.*]..
-000005e0: 6967 6e6f 7265 5f6d 6973 7369 6e67 5f69  ignore_missing_i
-000005f0: 6d70 6f72 7473 203d 2054 7275 650d 0a0d  mports = True...
-00000600: 0a5b 6d79 7079 2d73 6574 7570 746f 6f6c  .[mypy-setuptool
-00000610: 735d 0d0a 6967 6e6f 7265 5f6d 6973 7369  s]..ignore_missi
-00000620: 6e67 5f69 6d70 6f72 7473 203d 2054 7275  ng_imports = Tru
-00000630: 650d 0a0d 0a5b 6d79 7079 2d6e 756d 7079  e....[mypy-numpy
-00000640: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-00000650: 675f 696d 706f 7274 7320 3d20 5472 7565  g_imports = True
-00000660: 0d0a 0d0a 5b6d 7970 792d 6f6e 6e78 2e2a  ....[mypy-onnx.*
-00000670: 5d0d 0a69 676e 6f72 655f 6d69 7373 696e  ]..ignore_missin
-00000680: 675f 696d 706f 7274 7320 3d20 5472 7565  g_imports = True
-00000690: 0d0a 0d0a 5b6d 7970 792d 7466 326f 6e6e  ....[mypy-tf2onn
-000006a0: 782e 2a5d 0d0a 6967 6e6f 7265 5f6d 6973  x.*]..ignore_mis
-000006b0: 7369 6e67 5f69 6d70 6f72 7473 203d 2054  sing_imports = T
-000006c0: 7275 650d 0a0d 0a5b 6567 675f 696e 666f  rue....[egg_info
-000006d0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000006e0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000006f0: 0a                                       .
+00000060: 3430 312c 4230 3238 0d0a 7065 722d 6669  401,B028..per-fi
+00000070: 6c65 2d69 676e 6f72 6573 203d 200d 0a09  le-ignores = ...
+00000080: 7365 7475 702e 7079 3a20 4535 3031 0d0a  setup.py: E501..
+00000090: 0d0a 5b4d 4153 5445 525d 0d0a 6967 6e6f  ..[MASTER]..igno
+000000a0: 7265 203d 200d 0a6c 6f61 642d 706c 7567  re = ..load-plug
+000000b0: 696e 7320 3d20 7079 6c69 6e74 2e65 7874  ins = pylint.ext
+000000c0: 656e 7369 6f6e 732e 646f 6370 6172 616d  ensions.docparam
+000000d0: 730d 0a0d 0a5b 7079 6c69 6e74 5d0d 0a61  s....[pylint]..a
+000000e0: 6363 6570 742d 6e6f 2d70 6172 616d 2d64  ccept-no-param-d
+000000f0: 6f63 203d 206e 6f0d 0a64 6566 6175 6c74  oc = no..default
+00000100: 2d64 6f63 7374 7269 6e67 2d74 7970 6520  -docstring-type 
+00000110: 3d20 676f 6f67 6c65 0d0a 636f 6e74 6578  = google..contex
+00000120: 746d 616e 6167 6572 2d64 6563 6f72 6174  tmanager-decorat
+00000130: 6f72 7320 3d20 636f 6e74 6578 746c 6962  ors = contextlib
+00000140: 2e63 6f6e 7465 7874 6d61 6e61 6765 722c  .contextmanager,
+00000150: 2074 656e 736f 7266 6c6f 772e 7079 7468   tensorflow.pyth
+00000160: 6f6e 2e75 7469 6c2e 7466 5f63 6f6e 7465  on.util.tf_conte
+00000170: 7874 6c69 622e 636f 6e74 6578 746d 616e  xtlib.contextman
+00000180: 6167 6572 0d0a 6c6f 6767 696e 672d 666f  ager..logging-fo
+00000190: 726d 6174 2d73 7479 6c65 203d 206e 6577  rmat-style = new
+000001a0: 0d0a 6d61 782d 6c69 6e65 2d6c 656e 6774  ..max-line-lengt
+000001b0: 6820 3d20 3132 300d 0a6a 6f62 7320 3d20  h = 120..jobs = 
+000001c0: 310d 0a64 6973 6162 6c65 203d 2062 726f  1..disable = bro
+000001d0: 6164 2d65 7863 6570 742c 0d0a 0969 6e76  ad-except,...inv
+000001e0: 616c 6964 2d6e 616d 652c 0d0a 096e 6f2d  alid-name,...no-
+000001f0: 6d65 6d62 6572 2c0d 0a09 6e6f 2d6e 616d  member,...no-nam
+00000200: 652d 696e 2d6d 6f64 756c 652c 0d0a 0974  e-in-module,...t
+00000210: 6f6f 2d66 6577 2d70 7562 6c69 632d 6d65  oo-few-public-me
+00000220: 7468 6f64 732c 0d0a 0974 6f6f 2d6d 616e  thods,...too-man
+00000230: 792d 7075 626c 6963 2d6d 6574 686f 6473  y-public-methods
+00000240: 2c0d 0a09 746f 6f2d 6d61 6e79 2d61 7267  ,...too-many-arg
+00000250: 756d 656e 7473 2c0d 0a09 746f 6f2d 6d61  uments,...too-ma
+00000260: 6e79 2d62 7261 6e63 6865 732c 0d0a 0974  ny-branches,...t
+00000270: 6f6f 2d6d 616e 792d 6c69 6e65 732c 0d0a  oo-many-lines,..
+00000280: 0974 6f6f 2d6d 616e 792d 6c6f 6361 6c73  .too-many-locals
+00000290: 2c0d 0a09 746f 6f2d 6d61 6e79 2d69 6e73  ,...too-many-ins
+000002a0: 7461 6e63 652d 6174 7472 6962 7574 6573  tance-attributes
+000002b0: 2c0d 0a09 746f 6f2d 6d61 6e79 2d73 7461  ,...too-many-sta
+000002c0: 7465 6d65 6e74 732c 0d0a 0967 6c6f 6261  tements,...globa
+000002d0: 6c2d 7374 6174 656d 656e 742c 0d0a 0970  l-statement,...p
+000002e0: 726f 7465 6374 6564 2d61 6363 6573 732c  rotected-access,
+000002f0: 0d0a 0975 7365 2d61 2d67 656e 6572 6174  ...use-a-generat
+00000300: 6f72 2c0d 0a09 7573 656c 6573 732d 7061  or,...useless-pa
+00000310: 7261 6d2d 646f 632c 0d0a 0975 7365 6c65  ram-doc,...usele
+00000320: 7373 2d74 7970 652d 646f 632c 0d0a 096d  ss-type-doc,...m
+00000330: 6973 7369 6e67 2d72 6574 7572 6e2d 7479  issing-return-ty
+00000340: 7065 2d64 6f63 2c0d 0a09 6d69 7373 696e  pe-doc,...missin
+00000350: 672d 7969 656c 642d 7479 7065 2d64 6f63  g-yield-type-doc
+00000360: 2c0d 0a09 6d69 7373 696e 672d 7479 7065  ,...missing-type
+00000370: 2d64 6f63 2c0d 0a09 6d69 7373 696e 672d  -doc,...missing-
+00000380: 7969 656c 642d 646f 632c 0d0a 096d 6973  yield-doc,...mis
+00000390: 7369 6e67 2d72 6574 7572 6e2d 646f 632c  sing-return-doc,
+000003a0: 0d0a 0975 6e73 7065 6369 6669 6564 2d65  ...unspecified-e
+000003b0: 6e63 6f64 696e 672c 0d0a 0964 7570 6c69  ncoding,...dupli
+000003c0: 6361 7465 2d63 6f64 652c 0d0a 0969 6d70  cate-code,...imp
+000003d0: 6f72 742d 6572 726f 720d 0a0d 0a5b 7079  ort-error....[py
+000003e0: 6c69 6e74 2e6d 6573 7361 6765 735f 636f  lint.messages_co
+000003f0: 6e74 726f 6c5d 0d0a 6469 7361 626c 6520  ntrol]..disable 
+00000400: 3d20 5230 3430 320d 0a76 6172 6961 626c  = R0402..variabl
+00000410: 652d 7267 7820 3d20 5e28 3f21 2e2a 285b  e-rgx = ^(?!.*([
+00000420: 5f5d 295c 3129 5e28 3f3d 2e7b 312c 3330  _])\1)^(?=.{1,30
+00000430: 7d24 295b 612d 7a5f 5d5b 612d 7a30 2d39  }$)[a-z_][a-z0-9
+00000440: 5f5d 7b30 2c7d 240d 0a0d 0a5b 6d79 7079  _]{0,}$....[mypy
+00000450: 5d0d 0a64 6973 616c 6c6f 775f 756e 7479  ]..disallow_unty
+00000460: 7065 645f 6465 6673 203d 2054 7275 650d  ped_defs = True.
+00000470: 0a64 6973 616c 6c6f 775f 696e 636f 6d70  .disallow_incomp
+00000480: 6c65 7465 5f64 6566 7320 3d20 5472 7565  lete_defs = True
+00000490: 0d0a 6368 6563 6b5f 756e 7479 7065 645f  ..check_untyped_
+000004a0: 6465 6673 203d 2054 7275 650d 0a6e 6f5f  defs = True..no_
+000004b0: 696d 706c 6963 6974 5f6f 7074 696f 6e61  implicit_optiona
+000004c0: 6c20 3d20 5472 7565 0d0a 7374 7269 6374  l = True..strict
+000004d0: 5f6f 7074 696f 6e61 6c20 3d20 5472 7565  _optional = True
+000004e0: 0d0a 7374 7269 6374 5f65 7175 616c 6974  ..strict_equalit
+000004f0: 7920 3d20 5472 7565 0d0a 7761 726e 5f72  y = True..warn_r
+00000500: 6564 756e 6461 6e74 5f63 6173 7473 203d  edundant_casts =
+00000510: 2054 7275 650d 0a77 6172 6e5f 756e 7573   True..warn_unus
+00000520: 6564 5f69 676e 6f72 6573 203d 2054 7275  ed_ignores = Tru
+00000530: 650d 0a77 6172 6e5f 7265 7475 726e 5f61  e..warn_return_a
+00000540: 6e79 203d 2054 7275 650d 0a77 6172 6e5f  ny = True..warn_
+00000550: 756e 7573 6564 5f63 6f6e 6669 6773 203d  unused_configs =
+00000560: 2054 7275 650d 0a77 6172 6e5f 756e 7265   True..warn_unre
+00000570: 6163 6861 626c 6520 3d20 5472 7565 0d0a  achable = True..
+00000580: 6e6f 5f69 6d70 6c69 6369 745f 7265 6578  no_implicit_reex
+00000590: 706f 7274 203d 2054 7275 650d 0a0d 0a5b  port = True....[
+000005a0: 6d79 7079 2d74 656e 736f 7266 6c6f 772e  mypy-tensorflow.
+000005b0: 2a5d 0d0a 6967 6e6f 7265 5f6d 6973 7369  *]..ignore_missi
+000005c0: 6e67 5f69 6d70 6f72 7473 203d 2054 7275  ng_imports = Tru
+000005d0: 650d 0a0d 0a5b 6d79 7079 2d74 6f72 6368  e....[mypy-torch
+000005e0: 2e2a 5d0d 0a69 676e 6f72 655f 6d69 7373  .*]..ignore_miss
+000005f0: 696e 675f 696d 706f 7274 7320 3d20 5472  ing_imports = Tr
+00000600: 7565 0d0a 0d0a 5b6d 7970 792d 7365 7475  ue....[mypy-setu
+00000610: 7074 6f6f 6c73 5d0d 0a69 676e 6f72 655f  ptools]..ignore_
+00000620: 6d69 7373 696e 675f 696d 706f 7274 7320  missing_imports 
+00000630: 3d20 5472 7565 0d0a 0d0a 5b6d 7970 792d  = True....[mypy-
+00000640: 6e75 6d70 795d 0d0a 6967 6e6f 7265 5f6d  numpy]..ignore_m
+00000650: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+00000660: 2054 7275 650d 0a0d 0a5b 6d79 7079 2d6f   True....[mypy-o
+00000670: 6e6e 782e 2a5d 0d0a 6967 6e6f 7265 5f6d  nnx.*]..ignore_m
+00000680: 6973 7369 6e67 5f69 6d70 6f72 7473 203d  issing_imports =
+00000690: 2054 7275 650d 0a0d 0a5b 6d79 7079 2d74   True....[mypy-t
+000006a0: 6632 6f6e 6e78 2e2a 5d0d 0a69 676e 6f72  f2onnx.*]..ignor
+000006b0: 655f 6d69 7373 696e 675f 696d 706f 7274  e_missing_import
+000006c0: 7320 3d20 5472 7565 0d0a 0d0a 5b65 6767  s = True....[egg
+000006d0: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+000006e0: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+000006f0: 2030 0d0a 0d0a                            0....
```

### Comparing `czmodel-5.0.0/setup.py` & `czmodel-5.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     ],
     "pytorch": [
         *requirements,
         *pytorch_requirements,
     ],
 }
 
-VERSION = "5.0.0"
+VERSION = "5.1.0"
 
 # pylint: disable=line-too-long
 with open("README.md", "r", encoding="utf-8") as fh_read:
     long_description = fh_read.read()
 setuptools.setup(
     name="czmodel",
     version=VERSION,
@@ -60,27 +60,26 @@
     # For a list of valid classifiers, see https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     # Make required Python version compliant with official TF docs (https://www.tensorflow.org/install)
     # It follows: We build a pure Python wheel
     # Note that Python used to build the sources specifies the Python version of the dist (relevant during build only)
     # See https://packaging.python.org/guides/distributing-packages-using-setuptools/#pure-python-wheels for more info
     # We also restrict the code to >=3.6 to fully benefit from type annotations
     # See https://realpython.com/python-type-checking/ for more info
-    # No source distribution support for 3.10 yet
-    # See https://stackoverflow.com/questions/69458399/numpy-1-21-2-may-not-yet-support-python-3-10
-    # See https://github.com/numpy/numpy/issues/17044
-    python_requires=">=3.7,<3.10",
+    python_requires=">=3.7,<3.12",
     install_requires=[requirements],
     extras_require=extra_requirements,
     # List additional URLs that are relevant to your project as a dict.
     # The key is what's used to render the link text on PyPI.
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
     project_urls={
```

