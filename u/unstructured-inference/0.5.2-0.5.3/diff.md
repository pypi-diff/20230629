# Comparing `tmp/unstructured_inference-0.5.2.tar.gz` & `tmp/unstructured_inference-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.2.tar", last modified: Wed Jun 21 22:26:05 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.3.tar", last modified: Thu Jun 29 17:36:14 2023, max compression
```

## Comparing `unstructured_inference-0.5.2.tar` & `unstructured_inference-0.5.3.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.416619 unstructured_inference-0.5.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.416619 unstructured_inference-0.5.2/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.420619 unstructured_inference-0.5.2/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23929 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.420619 unstructured_inference-0.5.2/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15395 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/largemodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8147 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.551451 unstructured_inference-0.5.3/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-29 17:34:13.000000 unstructured_inference-0.5.3/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:36:14.543450 unstructured_inference-0.5.3/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6817 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 17:36:14.000000 unstructured_inference-0.5.3/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.2/PKG-INFO` & `unstructured_inference-0.5.3/unstructured_inference.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unstructured_inference
-Version: 0.5.2
+Name: unstructured-inference
+Version: 0.5.3
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -40,23 +40,26 @@
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
         
         ### PaddleOCR
         
-        [PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is required for table processing for `x86_64` architectures.
-        It should not be installed under MacOS with Apple Silicon cpu.
+        [PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is suggested for table processing for `x86_64` architectures.
+        It **should not be installed under MacOS running Apple Silicon**.
         
-        PaddleOCR should be installed using the following instructions.
+        PaddleOCR may be with installed with:
         
         ```shell
+        # x86_64 only!
         pip install "unstructured.PaddleOCR"
         ```
         
+        If paddle is not available, OCR is handled by tesseract instead.
+        
         ### Repository
         
         To install the repository for development, clone the repo and run `make install` to install dependencies.
         Run `make help` for a full list of install options.
         
         ## Getting Started
```

### Comparing `unstructured_inference-0.5.2/README.md` & `unstructured_inference-0.5.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,23 +32,26 @@
 
 Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
 See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
 tips on installing Detectron2 on Windows.
 
 ### PaddleOCR
 
-[PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is required for table processing for `x86_64` architectures.
-It should not be installed under MacOS with Apple Silicon cpu.
+[PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is suggested for table processing for `x86_64` architectures.
+It **should not be installed under MacOS running Apple Silicon**.
 
-PaddleOCR should be installed using the following instructions.
+PaddleOCR may be with installed with:
 
 ```shell
+# x86_64 only!
 pip install "unstructured.PaddleOCR"
 ```
 
+If paddle is not available, OCR is handled by tesseract instead.
+
 ### Repository
 
 To install the repository for development, clone the repo and run `make install` to install dependencies.
 Run `make help` for a full list of install options.
 
 ## Getting Started
```

### Comparing `unstructured_inference-0.5.2/setup.py` & `unstructured_inference-0.5.3/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.3/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.3/unstructured_inference/inference/layout.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from __future__ import annotations
 
 import os
 import tempfile
-from typing import BinaryIO, List, Optional, Tuple, Union
+from typing import BinaryIO, Collection, List, Optional, Tuple, Union, cast
 
 import numpy as np
 import pdf2image
 from pdfminer import psparser
 from pdfminer.high_level import extract_pages
 from PIL import Image
 
 from unstructured_inference.inference.elements import (
     EmbeddedTextRegion,
     ImageTextRegion,
+    Rectangle,
     TextRegion,
 )
 from unstructured_inference.inference.layoutelement import (
     LayoutElement,
+    LocationlessLayoutElement,
     merge_inferred_layout_with_extracted_layout,
 )
 from unstructured_inference.inference.ordering import order_layout
 from unstructured_inference.logger import logger
 from unstructured_inference.models.base import get_model
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
+from unstructured_inference.models.unstructuredmodel import (
+    UnstructuredElementExtractionModel,
+    UnstructuredObjectDetectionModel,
+)
 from unstructured_inference.patches.pdfminer import parse_keyword
 from unstructured_inference.visualize import draw_bbox
 
 # NOTE(alan): Patching this to fix a bug in pdfminer.six. Submitted this PR into pdfminer.six to fix
 # the bug: https://github.com/pdfminer/pdfminer.six/pull/885
 psparser.PSBaseParser._parse_keyword = parse_keyword  # type: ignore
 
@@ -62,15 +67,16 @@
         doc_layout._pages = pages
         return doc_layout
 
     @classmethod
     def from_file(
         cls,
         filename: str,
-        model: Optional[UnstructuredModel] = None,
+        detection_model: Optional[UnstructuredObjectDetectionModel] = None,
+        element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from a pdf file."""
         logger.info(f"Reading PDF for file: {filename} ...")
@@ -84,29 +90,31 @@
             fixed_layouts = [None for _ in layouts]
         for i, (image, layout, fixed_layout) in enumerate(zip(images, layouts, fixed_layouts)):
             # NOTE(robinson) - In the future, maybe we detect the page number and default
             # to the index if it is not detected
             page = PageLayout.from_image(
                 image,
                 number=i + 1,
-                model=model,
+                detection_model=detection_model,
+                element_extraction_model=element_extraction_model,
                 layout=layout,
                 ocr_strategy=ocr_strategy,
                 ocr_languages=ocr_languages,
                 fixed_layout=fixed_layout,
                 extract_tables=extract_tables,
             )
             pages.append(page)
         return cls.from_pages(pages)
 
     @classmethod
     def from_image_file(
         cls,
         filename: str,
-        model: Optional[UnstructuredModel] = None,
+        detection_model: Optional[UnstructuredObjectDetectionModel] = None,
+        element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         fixed_layout: Optional[List[TextRegion]] = None,
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from an image file."""
         logger.info(f"Reading image file: {filename} ...")
@@ -118,15 +126,16 @@
         except Exception as e:
             if os.path.isdir(filename) or os.path.isfile(filename):
                 raise e
             else:
                 raise FileNotFoundError(f'File "{filename}" not found!') from e
         page = PageLayout.from_image(
             image,
-            model=model,
+            detection_model=detection_model,
+            element_extraction_model=element_extraction_model,
             layout=None,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             fixed_layout=fixed_layout,
             extract_tables=extract_tables,
         )
         return cls.from_pages([page])
@@ -136,49 +145,76 @@
     """Class for an individual PDF page."""
 
     def __init__(
         self,
         number: int,
         image: Image.Image,
         layout: Optional[List[TextRegion]],
-        model: Optional[UnstructuredModel] = None,
+        detection_model: Optional[UnstructuredObjectDetectionModel] = None,
+        element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
     ):
+        if detection_model is not None and element_extraction_model is not None:
+            raise ValueError("Only one of detection_model and extraction_model should be passed.")
         self.image = image
         self.image_array: Union[np.ndarray, None] = None
         self.layout = layout
         self.number = number
-        self.model = model
-        self.elements: List[LayoutElement] = []
+        self.detection_model = detection_model
+        self.element_extraction_model = element_extraction_model
+        self.elements: Collection[Union[LayoutElement, LocationlessLayoutElement]] = []
         if ocr_strategy not in VALID_OCR_STRATEGIES:
             raise ValueError(f"ocr_strategy must be one of {VALID_OCR_STRATEGIES}.")
         self.ocr_strategy = ocr_strategy
         self.ocr_languages = ocr_languages
         self.extract_tables = extract_tables
 
     def __str__(self) -> str:
         return "\n\n".join([str(element) for element in self.elements])
 
-    def get_elements_with_model(self, inplace=True) -> Optional[List[LayoutElement]]:
+    def get_elements_using_image_extraction(
+        self,
+        inplace=True,
+    ) -> Optional[List[LocationlessLayoutElement]]:
+        """Uses end-to-end text element extraction model to extract the elements on the page."""
+        if self.element_extraction_model is None:
+            raise ValueError(
+                "Cannot get elements using image extraction, no image extraction model defined",
+            )
+        elements = self.element_extraction_model(self.image)
+        if inplace:
+            self.elements = elements
+            return None
+        return elements
+
+    def get_elements_with_detection_model(self, inplace=True) -> Optional[List[LayoutElement]]:
         """Uses specified model to detect the elements on the page."""
         logger.info("Detecting page elements ...")
-        if self.model is None:
-            self.model = get_model()
+        if self.detection_model is None:
+            model = get_model()
+            if isinstance(model, UnstructuredObjectDetectionModel):
+                self.detection_model = model
+            else:
+                raise NotImplementedError("Default model should be a detection model")
 
         # NOTE(mrobinson) - We'll want make this model inference step some kind of
         # remote call in the future.
-        inferred_layout = self.model(self.image)
+        inferred_layout: List[TextRegion] = cast(List[TextRegion], self.detection_model(self.image))
         if self.layout is not None:
-            inferred_layout = merge_inferred_layout_with_extracted_layout(
-                inferred_layout=inferred_layout,
-                extracted_layout=self.layout,
+            inferred_layout = cast(
+                List[TextRegion],
+                merge_inferred_layout_with_extracted_layout(
+                    inferred_layout=cast(Collection[LayoutElement], inferred_layout),
+                    extracted_layout=self.layout,
+                ),
             )
         elements = self.get_elements_from_layout(inferred_layout)
+
         if inplace:
             self.elements = elements
             return None
         return elements
 
     def get_elements_from_layout(self, layout: List[TextRegion]) -> List[LayoutElement]:
         """Uses the given Layout to separate the page text into elements, either extracting the
@@ -211,41 +247,47 @@
             colors = [colors]
         # If there aren't enough colors, just cycle through the colors a few times
         if len(colors) < len(self.elements):
             n_copies = (len(self.elements) // len(colors)) + 1
             colors = colors * n_copies
         img = self.image.copy()
         for el, color in zip(self.elements, colors):
-            img = draw_bbox(img, el, color=color)
+            if isinstance(el, Rectangle):
+                img = draw_bbox(img, el, color=color)
         return img
 
     @classmethod
     def from_image(
         cls,
         image: Image.Image,
         number: int = 1,
-        model: Optional[UnstructuredModel] = None,
+        detection_model: Optional[UnstructuredObjectDetectionModel] = None,
+        element_extraction_model: Optional[UnstructuredElementExtractionModel] = None,
         layout: Optional[List[TextRegion]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
         fixed_layout: Optional[List[TextRegion]] = None,
     ):
         """Creates a PageLayout from an already-loaded PIL Image."""
         page = cls(
             number=number,
             image=image,
             layout=layout,
-            model=model,
+            detection_model=detection_model,
+            element_extraction_model=element_extraction_model,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             extract_tables=extract_tables,
         )
+        if page.element_extraction_model is not None:
+            page.get_elements_using_image_extraction()
+            return page
         if fixed_layout is None:
-            page.get_elements_with_model()
+            page.get_elements_with_detection_model()
         else:
             page.elements = page.get_elements_from_layout(fixed_layout)
         return page
 
 
 def process_data_with_model(
     data: BinaryIO,
@@ -281,26 +323,36 @@
     ocr_languages: str = "eng",
     fixed_layouts: Optional[List[Optional[List[TextRegion]]]] = None,
     extract_tables: bool = False,
 ) -> DocumentLayout:
     """Processes pdf file with name filename into a DocumentLayout by using a model identified by
     model_name."""
     model = get_model(model_name)
+    if isinstance(model, UnstructuredObjectDetectionModel):
+        detection_model = model
+        element_extraction_model = None
+    elif isinstance(model, UnstructuredElementExtractionModel):
+        detection_model = None
+        element_extraction_model = model
+    else:
+        raise ValueError(f"Unsupported model type: {type(model)}")
     layout = (
         DocumentLayout.from_image_file(
             filename,
-            model=model,
+            detection_model=detection_model,
+            element_extraction_model=element_extraction_model,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             extract_tables=extract_tables,
         )
         if is_image
         else DocumentLayout.from_file(
             filename,
-            model=model,
+            detection_model=detection_model,
+            element_extraction_model=element_extraction_model,
             ocr_strategy=ocr_strategy,
             ocr_languages=ocr_languages,
             fixed_layouts=fixed_layouts,
             extract_tables=extract_tables,
         )
     )
     return layout
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.5.3/unstructured_inference/inference/layoutelement.py`

 * *Files 12% similar despite different names*

```diff
@@ -136,7 +136,24 @@
         )
         for el in extracted_elements_to_add
     ]
     out_layout = categorized_extracted_elements_to_add + [
         region for region in inferred_layout if region not in inferred_regions_to_remove
     ]
     return out_layout
+
+
+# NOTE(alan): The right way to do this is probably to rewrite LayoutElement as well as the different
+# Region types to not subclass Rectangle, and instead have an optional bbox property that is a
+# Rectangle. I or someone else will have to get to that later.
+@dataclass
+class LocationlessLayoutElement:
+    text: Optional[str]
+    type: Optional[str]
+
+    def to_dict(self) -> dict:
+        """Converts the class instance to dictionary form."""
+        out_dict = {
+            "text": self.text,
+            "type": self.type,
+        }
+        return out_dict
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.3/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/base.py` & `unstructured_inference-0.5.3/unstructured_inference/models/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 )
 from unstructured_inference.models.detectron2onnx import (
     MODEL_TYPES as DETECTRON2_ONNX_MODEL_TYPES,
 )
 from unstructured_inference.models.detectron2onnx import (
     UnstructuredDetectronONNXModel,
 )
+from unstructured_inference.models.largemodel import MODEL_TYPES as LARGE_MODEL_TYPES
+from unstructured_inference.models.largemodel import UnstructuredLargeModel
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.models.yolox import (
     MODEL_TYPES as YOLOX_MODEL_TYPES,
 )
 from unstructured_inference.models.yolox import (
     UnstructuredYoloXModel,
 )
@@ -35,14 +37,17 @@
         model.initialize(**DETECTRON2_MODEL_TYPES[model_name])
     elif model_name in DETECTRON2_ONNX_MODEL_TYPES:
         model = UnstructuredDetectronONNXModel()
         model.initialize(**DETECTRON2_ONNX_MODEL_TYPES[model_name])
     elif model_name in YOLOX_MODEL_TYPES:
         model = UnstructuredYoloXModel()
         model.initialize(**YOLOX_MODEL_TYPES[model_name])
+    elif model_name in LARGE_MODEL_TYPES:
+        model = UnstructuredLargeModel()
+        model.initialize(**LARGE_MODEL_TYPES[model_name])
     else:
         raise UnknownModelException(f"Unknown model type: {model_name}")
     return model
 
 
 class UnknownModelException(Exception):
     """Exception for the case where a model is called for with an unrecognized identifier."""
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.3/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.3/unstructured_inference/models/detectron2onnx.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.3/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.3/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.3/unstructured_inference/models/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,68 +51,79 @@
             logging.critical("Failed to initialize the model.")
             logging.critical("Ensure that the model is correct")
             raise ImportError(
                 "Review the parameters to initialize a UnstructuredTableTransformerModel obj",
             )
         self.model.to(device)
 
-    def run_prediction(self, x: Image):
-        """Predict table structure"""
-        with torch.no_grad():
-            encoding = self.feature_extractor(x, return_tensors="pt").to(self.device)
-            outputs_structure = self.model(**encoding)
-
+    def get_tokens(self, x: Image):
+        """Get OCR tokens from either paddleocr or tesseract"""
         if platform.machine() == "x86_64":
-            from unstructured_inference.models import paddle_ocr
+            try:
+                from unstructured_inference.models import paddle_ocr
 
-            paddle_result = paddle_ocr.load_agent().ocr(np.array(x), cls=True)
-
-            tokens = []
-            for idx in range(len(paddle_result)):
-                res = paddle_result[idx]
-                for line in res:
-                    xmin = min([i[0] for i in line[0]])
-                    ymin = min([i[1] for i in line[0]])
-                    xmax = max([i[0] for i in line[0]])
-                    ymax = max([i[1] for i in line[0]])
-                    tokens.append({"bbox": [xmin, ymin, xmax, ymax], "text": line[1][0]})
-        else:
-            zoom = 6
-            img = cv2.resize(
-                cv2.cvtColor(np.array(x), cv2.COLOR_RGB2BGR),
-                None,
-                fx=zoom,
-                fy=zoom,
-                interpolation=cv2.INTER_CUBIC,
-            )
+                paddle_result = paddle_ocr.load_agent().ocr(np.array(x), cls=True)
 
-            kernel = np.ones((1, 1), np.uint8)
-            img = cv2.dilate(img, kernel, iterations=1)
-            img = cv2.erode(img, kernel, iterations=1)
-
-            ocr_df: pd.DataFrame = pytesseract.image_to_data(
-                Image.fromarray(img),
-                output_type="data.frame",
+                tokens = []
+                for idx in range(len(paddle_result)):
+                    res = paddle_result[idx]
+                    for line in res:
+                        xmin = min([i[0] for i in line[0]])
+                        ymin = min([i[1] for i in line[0]])
+                        xmax = max([i[0] for i in line[0]])
+                        ymax = max([i[1] for i in line[0]])
+                        tokens.append({"bbox": [xmin, ymin, xmax, ymax], "text": line[1][0]})
+                return tokens
+            except ModuleNotFoundError:
+                logging.warning(
+                    "No module named 'unstructured_paddleocr', falling back to tesseract",
+                )
+                pass
+        zoom = 6
+        img = cv2.resize(
+            cv2.cvtColor(np.array(x), cv2.COLOR_RGB2BGR),
+            None,
+            fx=zoom,
+            fy=zoom,
+            interpolation=cv2.INTER_CUBIC,
+        )
+
+        kernel = np.ones((1, 1), np.uint8)
+        img = cv2.dilate(img, kernel, iterations=1)
+        img = cv2.erode(img, kernel, iterations=1)
+
+        ocr_df: pd.DataFrame = pytesseract.image_to_data(
+            Image.fromarray(img),
+            output_type="data.frame",
+        )
+
+        ocr_df = ocr_df.dropna()
+
+        tokens = []
+        for idtx in ocr_df.itertuples():
+            tokens.append(
+                {
+                    "bbox": [
+                        idtx.left / zoom,
+                        idtx.top / zoom,
+                        (idtx.left + idtx.width) / zoom,
+                        (idtx.top + idtx.height) / zoom,
+                    ],
+                    "text": idtx.text,
+                },
             )
+        return tokens
 
-            ocr_df = ocr_df.dropna()
+    def run_prediction(self, x: Image):
+        """Predict table structure"""
+        with torch.no_grad():
+            encoding = self.feature_extractor(x, return_tensors="pt").to(self.device)
+            outputs_structure = self.model(**encoding)
 
-            tokens = []
-            for idtx in ocr_df.itertuples():
-                tokens.append(
-                    {
-                        "bbox": [
-                            idtx.left / zoom,
-                            idtx.top / zoom,
-                            (idtx.left + idtx.width) / zoom,
-                            (idtx.top + idtx.height) / zoom,
-                        ],
-                        "text": idtx.text,
-                    },
-                )
+        tokens = self.get_tokens(x=x)
 
         sorted(tokens, key=lambda x: x["bbox"][1] * 10000 + x["bbox"][0])
 
         # 'tokens' is a list of tokens
         # Need to be in a relative reading order
         # If no order is provided, use current order
         for idx, token in enumerate(tokens):
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.3/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.3/unstructured_inference/models/unstructuredmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,18 @@
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, List
 
 from PIL.Image import Image
 
 if TYPE_CHECKING:
-    from unstructured_inference.inference.layoutelement import LayoutElement
+    from unstructured_inference.inference.layoutelement import (
+        LayoutElement,
+        LocationlessLayoutElement,
+    )
 
 
 class UnstructuredModel(ABC):
     """Wrapper class for the various models used by unstructured."""
 
     def __init__(self):
         """model should support inference of some sort, either by calling or by some method.
@@ -49,9 +52,23 @@
         return []  # pragma: no cover
 
     def __call__(self, x: Image) -> List[LayoutElement]:
         """Inference using function call interface."""
         return super().__call__(x)
 
 
+class UnstructuredElementExtractionModel(UnstructuredModel):
+    """Wrapper class for object extraction models used by unstructured."""
+
+    @abstractmethod
+    def predict(self, x: Image) -> List[LocationlessLayoutElement]:
+        """Do inference using the wrapped model."""
+        super().predict(x)
+        return []  # pragma: no cover
+
+    def __call__(self, x: Image) -> List[LocationlessLayoutElement]:
+        """Inference using function call interface."""
+        return super().__call__(x)
+
+
 class ModelNotInitializedError(Exception):
     pass
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.3/unstructured_inference/models/yolox.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import cv2
 import numpy as np
 import onnxruntime
 from huggingface_hub import hf_hub_download
 from PIL import Image
 
 from unstructured_inference.inference.layoutelement import LayoutElement
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
+from unstructured_inference.models.unstructuredmodel import UnstructuredObjectDetectionModel
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 from unstructured_inference.visualize import draw_yolox_bounding_boxes
 
 YOLOX_LABEL_MAP = {
     0: "Caption",
     1: "Footnote",
     2: "Formula",
@@ -46,15 +46,15 @@
             "yolox_tiny.onnx",
         ),
         label_map=YOLOX_LABEL_MAP,
     ),
 }
 
 
-class UnstructuredYoloXModel(UnstructuredModel):
+class UnstructuredYoloXModel(UnstructuredObjectDetectionModel):
     def predict(self, x: Image):
         """Predict using YoloX model."""
         super().predict(x)
         return self.image_processing(x)
 
     def initialize(self, model_path: str, label_map: dict):
         """Start inference session for YoloX model."""
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.3/unstructured_inference/patches/pdfminer.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/utils.py` & `unstructured_inference-0.5.3/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference/visualize.py` & `unstructured_inference-0.5.3/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.2/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: unstructured-inference
-Version: 0.5.2
+Name: unstructured_inference
+Version: 0.5.3
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
@@ -40,23 +40,26 @@
         
         Windows is not officially supported by Detectron2, but some users are able to install it anyway. 
         See discussion [here](https://layout-parser.github.io/tutorials/installation#for-windows-users) for 
         tips on installing Detectron2 on Windows.
         
         ### PaddleOCR
         
-        [PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is required for table processing for `x86_64` architectures.
-        It should not be installed under MacOS with Apple Silicon cpu.
+        [PaddleOCR](https://github.com/Unstructured-IO/unstructured.PaddleOCR) is suggested for table processing for `x86_64` architectures.
+        It **should not be installed under MacOS running Apple Silicon**.
         
-        PaddleOCR should be installed using the following instructions.
+        PaddleOCR may be with installed with:
         
         ```shell
+        # x86_64 only!
         pip install "unstructured.PaddleOCR"
         ```
         
+        If paddle is not available, OCR is handled by tesseract instead.
+        
         ### Repository
         
         To install the repository for development, clone the repo and run `make install` to install dependencies.
         Run `make help` for a full list of install options.
         
         ## Getting Started
```

### Comparing `unstructured_inference-0.5.2/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.3/unstructured_inference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 unstructured_inference/inference/layoutelement.py
 unstructured_inference/inference/ordering.py
 unstructured_inference/models/__init__.py
 unstructured_inference/models/base.py
 unstructured_inference/models/detectron2.py
 unstructured_inference/models/detectron2onnx.py
 unstructured_inference/models/donut.py
+unstructured_inference/models/largemodel.py
 unstructured_inference/models/paddle_ocr.py
 unstructured_inference/models/table_postprocess.py
 unstructured_inference/models/tables.py
 unstructured_inference/models/tesseract.py
 unstructured_inference/models/unstructuredmodel.py
 unstructured_inference/models/yolox.py
 unstructured_inference/patches/__init__.py
```

