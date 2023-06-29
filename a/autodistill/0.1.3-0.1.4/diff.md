# Comparing `tmp/autodistill-0.1.3.tar.gz` & `tmp/autodistill-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-0.1.3.tar", last modified: Wed Jun 21 10:36:10 2023, max compression
+gzip compressed data, was "autodistill-0.1.4.tar", last modified: Thu Jun 29 11:27:29 2023, max compression
```

## Comparing `autodistill-0.1.3.tar` & `autodistill-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.149181 autodistill-0.1.3/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-21 10:32:32.000000 autodistill-0.1.3/LICENSE
--rw-r--r--   0 james      (501) staff       (20)    15193 2023-06-21 10:36:10.148941 autodistill-0.1.3/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    14669 2023-06-21 10:32:32.000000 autodistill-0.1.3/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.145667 autodistill-0.1.3/autodistill/
--rw-r--r--   0 james      (501) staff       (20)       22 2023-06-21 10:32:54.000000 autodistill-0.1.3/autodistill/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.147340 autodistill-0.1.3/autodistill/core/
--rw-r--r--   0 james      (501) staff       (20)      151 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      516 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/base_model.py
--rw-r--r--   0 james      (501) staff       (20)      114 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/ontology.py
--rw-r--r--   0 james      (501) staff       (20)      236 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/core/target_model.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.148337 autodistill-0.1.3/autodistill/detection/
--rw-r--r--   0 james      (501) staff       (20)      290 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      580 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/caption_ontology.py
--rw-r--r--   0 james      (501) staff       (20)     1760 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_base_model.py
--rw-r--r--   0 james      (501) staff       (20)      769 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_ontology.py
--rw-r--r--   0 james      (501) staff       (20)      366 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/detection/detection_target_model.py
--rw-r--r--   0 james      (501) staff       (20)     3258 2023-06-21 10:32:32.000000 autodistill-0.1.3/autodistill/helpers.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.146617 autodistill-0.1.3/autodistill.egg-info/
--rw-r--r--   0 james      (501) staff       (20)    15193 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      602 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      142 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       12 2023-06-21 10:36:10.000000 autodistill-0.1.3/autodistill.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-21 10:36:10.149228 autodistill-0.1.3/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1273 2023-06-21 10:36:06.000000 autodistill-0.1.3/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-21 10:36:10.148529 autodistill-0.1.3/test/
--rw-r--r--   0 james      (501) staff       (20)       41 2023-06-21 10:32:32.000000 autodistill-0.1.3/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.591657 autodistill-0.1.4/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-07 11:34:42.000000 autodistill-0.1.4/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:27:29.590795 autodistill-0.1.4/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    15196 2023-06-29 10:08:16.000000 autodistill-0.1.4/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.586595 autodistill-0.1.4/autodistill/
+-rw-r--r--   0 james      (501) staff       (20)       22 2023-06-29 11:27:11.000000 autodistill-0.1.4/autodistill/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.588397 autodistill-0.1.4/autodistill/classification/
+-rw-r--r--   0 james      (501) staff       (20)      191 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1903 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/classification_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      380 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/classification/classification_target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.589160 autodistill-0.1.4/autodistill/core/
+-rw-r--r--   0 james      (501) staff       (20)      151 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      532 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      116 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      237 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/core/target_model.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.590224 autodistill-0.1.4/autodistill/detection/
+-rw-r--r--   0 james      (501) staff       (20)      290 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      577 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/caption_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)     1761 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_base_model.py
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_ontology.py
+-rw-r--r--   0 james      (501) staff       (20)      370 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/detection/detection_target_model.py
+-rw-r--r--   0 james      (501) staff       (20)     3259 2023-06-29 11:03:41.000000 autodistill-0.1.4/autodistill/helpers.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.587694 autodistill-0.1.4/autodistill.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)    15720 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      755 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      142 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       12 2023-06-29 11:27:29.000000 autodistill-0.1.4/autodistill.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 11:27:29.591852 autodistill-0.1.4/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1273 2023-06-29 11:18:18.000000 autodistill-0.1.4/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 11:27:29.590414 autodistill-0.1.4/test/
+-rw-r--r--   0 james      (501) staff       (20)       41 2023-06-07 11:34:42.000000 autodistill-0.1.4/test/test_hello.py
```

### Comparing `autodistill-0.1.3/LICENSE` & `autodistill-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-0.1.3/PKG-INFO` & `autodistill-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.3
+Version: 0.1.4
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
         width="850"
         src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.jpg?2"
       >
     </a>
   </p>
 </div>
 
-[![version](https://badge.fury.io/py/autodistill.svg)](https://badge.fury.io/py/autodistill)
+[![version](https://badge.fury.io/py/autodistill.svg?)](https://badge.fury.io/py/autodistill)
 [![downloads](https://img.shields.io/pypi/dm/autodistill)](https://pypistats.org/packages/autodistill)
-[![license](https://img.shields.io/pypi/l/autodistill)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
+[![license](https://img.shields.io/pypi/l/autodistill?)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
 [![python-version](https://img.shields.io/pypi/pyversions/autodistill)](https://badge.fury.io/py/autodistill)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb)
 
 Autodistill uses big, slower foundation models to train small, faster supervised models. Using `autodistill`, you can go from unlabeled images to inference on a custom model running at the edge with no human intervention in between.
 
 <div align="center">
   <p>
@@ -284,14 +284,17 @@
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p> 
 
 ## 💡 Community Resources
 
 - [Distill Large Vision Models into Smaller, Efficient Models with Autodistill](https://blog.roboflow.com/autodistill/): Announcement post with written guide on how to use Autodistill
+- [Comparing AI-Labeled Data to Human-Labeled Data](https://blog.roboflow.com/ai-vs-human-labeled-data/): A qualitative evaluation of Grounding DINO used with Autodistill across various tasks and domains.
+- [How to Evaluate Autodistill Prompts with CVevals](https://blog.roboflow.com/autodistill-prompt-evaluation/): Evaluate Autodistill prompts.
+- [Autodistill: Label and Train a Computer Vision Model in Under 20 Minutes](https://www.youtube.com/watch?v=M_QZ_Q0zT0k): Building a model to detect planes in under 20 minutes.
 - File a PR to add your own resources here!
 
 ## 🗺️ Roadmap
 
 Apart from adding new models, there are several areas we plan to explore with `autodistill` including:
 
 * 💡 Ontology creation & prompt engineering
```

### Comparing `autodistill-0.1.3/README.md` & `autodistill-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
         width="850"
         src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.jpg?2"
       >
     </a>
   </p>
 </div>
 
-[![version](https://badge.fury.io/py/autodistill.svg)](https://badge.fury.io/py/autodistill)
+[![version](https://badge.fury.io/py/autodistill.svg?)](https://badge.fury.io/py/autodistill)
 [![downloads](https://img.shields.io/pypi/dm/autodistill)](https://pypistats.org/packages/autodistill)
-[![license](https://img.shields.io/pypi/l/autodistill)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
+[![license](https://img.shields.io/pypi/l/autodistill?)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
 [![python-version](https://img.shields.io/pypi/pyversions/autodistill)](https://badge.fury.io/py/autodistill)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb)
 
 Autodistill uses big, slower foundation models to train small, faster supervised models. Using `autodistill`, you can go from unlabeled images to inference on a custom model running at the edge with no human intervention in between.
 
 <div align="center">
   <p>
@@ -269,14 +269,17 @@
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p> 
 
 ## 💡 Community Resources
 
 - [Distill Large Vision Models into Smaller, Efficient Models with Autodistill](https://blog.roboflow.com/autodistill/): Announcement post with written guide on how to use Autodistill
+- [Comparing AI-Labeled Data to Human-Labeled Data](https://blog.roboflow.com/ai-vs-human-labeled-data/): A qualitative evaluation of Grounding DINO used with Autodistill across various tasks and domains.
+- [How to Evaluate Autodistill Prompts with CVevals](https://blog.roboflow.com/autodistill-prompt-evaluation/): Evaluate Autodistill prompts.
+- [Autodistill: Label and Train a Computer Vision Model in Under 20 Minutes](https://www.youtube.com/watch?v=M_QZ_Q0zT0k): Building a model to detect planes in under 20 minutes.
 - File a PR to add your own resources here!
 
 ## 🗺️ Roadmap
 
 Apart from adding new models, there are several areas we plan to explore with `autodistill` including:
 
 * 💡 Ontology creation & prompt engineering
```

### Comparing `autodistill-0.1.3/autodistill/core/base_model.py` & `autodistill-0.1.4/autodistill/core/base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any
 
 import supervision as sv
+
 from autodistill.core import Ontology
 
+
 @dataclass
 class BaseModel(ABC):
     ontology: Ontology
 
     def set_ontology(self, ontology: Ontology):
         self.ontology = ontology
 
     @abstractmethod
     def predict(self, input: Any) -> Any:
         pass
 
     @abstractmethod
-    def label(self, input_folder: str, extension: str = ".jpg", output_folder: str = None) -> sv.BaseDataset:
+    def label(
+        self, input_folder: str, extension: str = ".jpg", output_folder: str = None
+    ) -> sv.BaseDataset:
         pass
```

### Comparing `autodistill-0.1.3/autodistill/detection/caption_ontology.py` & `autodistill-0.1.4/autodistill/detection/caption_ontology.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from dataclasses import dataclass
-from typing import List, Tuple, Dict
+from typing import Dict, List, Tuple
 
 from autodistill.detection import DetectionOntology
 
+
 @dataclass
 class CaptionOntology(DetectionOntology):
     promptMap: List[Tuple[str, str]]
 
     def __init__(self, ontology: Dict[str, str]):
         self.promptMap = [(k, v) for k, v in ontology.items()]
 
         if len(self.promptMap) == 0:
             raise ValueError("Ontology is empty")
 
     def prompts(self) -> List[str]:
         return super().prompts()
-    
+
     def classToPrompt(self, cls: str) -> str:
         return super().classToPrompt(cls)
```

### Comparing `autodistill-0.1.3/autodistill/detection/detection_base_model.py` & `autodistill-0.1.4/autodistill/detection/detection_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+import glob
+import os
 from abc import abstractmethod
 from dataclasses import dataclass
 
-import os
-import glob
-from tqdm import tqdm
 import cv2
-
 import supervision as sv
+from tqdm import tqdm
+
 from autodistill.core import BaseModel
 from autodistill.detection import DetectionOntology
-
 from autodistill.helpers import split_data
 
+
 @dataclass
 class DetectionBaseModel(BaseModel):
     ontology: DetectionOntology
 
     @abstractmethod
     def predict(self, input: str) -> sv.Detections:
         pass
 
-    def label(self, input_folder: str, extension: str = ".jpg", output_folder: str = None) -> sv.DetectionDataset:
+    def label(
+        self, input_folder: str, extension: str = ".jpg", output_folder: str = None
+    ) -> sv.DetectionDataset:
         if output_folder is None:
             output_folder = input_folder + "_labeled"
-        
+
         os.makedirs(output_folder, exist_ok=True)
 
         images_map = {}
         detections_map = {}
 
         files = glob.glob(input_folder + "/*" + extension)
         progress_bar = tqdm(files, desc="Labeling images")
@@ -50,10 +52,9 @@
             output_folder + "/annotations",
             min_image_area_percentage=0.01,
             data_yaml_path=output_folder + "/data.yaml",
         )
 
         split_data(output_folder)
 
-        print("Labeled dataset created - ready for distillation.")  
-        return dataset  
-
+        print("Labeled dataset created - ready for distillation.")
+        return dataset
```

### Comparing `autodistill-0.1.3/autodistill/detection/detection_ontology.py` & `autodistill-0.1.4/autodistill/detection/detection_ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from dataclasses import dataclass
 from typing import Any, List, Tuple
 
 from autodistill.core import Ontology
 
+
 @dataclass
 class DetectionOntology(Ontology):
     promptMap: List[Tuple[Any, str]]
 
     def prompts(self) -> List[Any]:
         return [prompt for prompt, _ in self.promptMap]
-    
+
     def classes(self) -> List[str]:
         return [cls for _, cls in self.promptMap]
 
     def promptToClass(self, prompt: Any) -> str:
         for p, cls in self.promptMap:
             if p == prompt:
                 return cls
         raise ValueError("Prompt not found in ontology")
-    
+
     def classToPrompt(self, cls: str) -> Any:
         for p, c in self.promptMap:
             if c == cls:
                 return p
-        raise ValueError("Class not found in ontology")
+        raise ValueError("Class not found in ontology")
```

### Comparing `autodistill-0.1.3/autodistill/helpers.py` & `autodistill-0.1.4/autodistill/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import random
 import shutil
 
 import yaml
 from PIL import Image
 
+
 def split_data(base_dir, split_ratio=0.8):
     images_dir = os.path.join(base_dir, "images")
     annotations_dir = os.path.join(base_dir, "annotations")
 
     # Correct the image file names if they have an extra dot before the extension
     for file in os.listdir(images_dir):
         if file.count(".") > 1:
```

### Comparing `autodistill-0.1.3/autodistill.egg-info/PKG-INFO` & `autodistill-0.1.4/autodistill.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill
-Version: 0.1.3
+Version: 0.1.4
 Summary: Distill large foundational models into smaller, domain-specific models for deployment
 Home-page: https://github.com/autodistill/autodistill
 Author: Roboflow
 Author-email: autodistill@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
         width="850"
         src="https://media.roboflow.com/open-source/autodistill/autodistill-banner.jpg?2"
       >
     </a>
   </p>
 </div>
 
-[![version](https://badge.fury.io/py/autodistill.svg)](https://badge.fury.io/py/autodistill)
+[![version](https://badge.fury.io/py/autodistill.svg?)](https://badge.fury.io/py/autodistill)
 [![downloads](https://img.shields.io/pypi/dm/autodistill)](https://pypistats.org/packages/autodistill)
-[![license](https://img.shields.io/pypi/l/autodistill)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
+[![license](https://img.shields.io/pypi/l/autodistill?)](https://github.com/autodistill/autodistill/blob/main/LICENSE)
 [![python-version](https://img.shields.io/pypi/pyversions/autodistill)](https://badge.fury.io/py/autodistill)
 [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/how-to-auto-train-yolov8-model-with-autodistill.ipynb)
 
 Autodistill uses big, slower foundation models to train small, faster supervised models. Using `autodistill`, you can go from unlabeled images to inference on a custom model running at the edge with no human intervention in between.
 
 <div align="center">
   <p>
@@ -284,14 +284,17 @@
 <a href="https://youtu.be/oEQYStnF2l8"><strong>Autodistill: Train YOLOv8 with ZERO Annotations</strong></a>
 <div><strong>Published: 8 June 2023</strong></div>
 <br/>In this video, we will show you how to use a new library to train a YOLOv8 model to detect bottles moving on a conveyor line. Yes, that's right - zero annotation hours are required! We dive deep into Autodistill's functionality, covering topics from setting up your Python environment and preparing your images, to the thrilling automatic annotation of images. </p> 
 
 ## 💡 Community Resources
 
 - [Distill Large Vision Models into Smaller, Efficient Models with Autodistill](https://blog.roboflow.com/autodistill/): Announcement post with written guide on how to use Autodistill
+- [Comparing AI-Labeled Data to Human-Labeled Data](https://blog.roboflow.com/ai-vs-human-labeled-data/): A qualitative evaluation of Grounding DINO used with Autodistill across various tasks and domains.
+- [How to Evaluate Autodistill Prompts with CVevals](https://blog.roboflow.com/autodistill-prompt-evaluation/): Evaluate Autodistill prompts.
+- [Autodistill: Label and Train a Computer Vision Model in Under 20 Minutes](https://www.youtube.com/watch?v=M_QZ_Q0zT0k): Building a model to detect planes in under 20 minutes.
 - File a PR to add your own resources here!
 
 ## 🗺️ Roadmap
 
 Apart from adding new models, there are several areas we plan to explore with `autodistill` including:
 
 * 💡 Ontology creation & prompt engineering
```

### Comparing `autodistill-0.1.3/setup.py` & `autodistill-0.1.4/setup.py`

 * *Files identical despite different names*

