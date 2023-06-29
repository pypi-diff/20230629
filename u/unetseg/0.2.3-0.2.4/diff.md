# Comparing `tmp/unetseg-0.2.3.tar.gz` & `tmp/unetseg-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unetseg-0.2.3.tar", max compression
+gzip compressed data, was "unetseg-0.2.4.tar", max compression
```

## Comparing `unetseg-0.2.3.tar` & `unetseg-0.2.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-04-11 14:43:39.872672 unetseg-0.2.3/LICENSE.txt
--rw-r--r--   0        0        0      876 2023-04-11 14:50:20.255825 unetseg-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      363 2023-04-11 14:43:39.885340 unetseg-0.2.3/unetseg/__init__.py
--rw-r--r--   0        0        0     3537 2023-04-11 14:43:39.885514 unetseg-0.2.3/unetseg/console/predict.py
--rw-r--r--   0        0        0     4998 2023-04-11 14:43:39.885650 unetseg-0.2.3/unetseg/console/train.py
--rw-r--r--   0        0        0     3861 2023-04-11 14:43:39.885769 unetseg-0.2.3/unetseg/evaluate.py
--rw-r--r--   0        0        0     3662 2023-04-11 14:43:39.885918 unetseg-0.2.3/unetseg/postprocess.py
--rw-r--r--   0        0        0     3810 2023-04-11 14:43:39.886056 unetseg-0.2.3/unetseg/predict.py
--rw-r--r--   0        0        0    22083 2023-04-11 14:43:39.886268 unetseg-0.2.3/unetseg/train.py
--rw-r--r--   0        0        0      842 2023-04-11 14:43:39.886391 unetseg-0.2.3/unetseg/utils.py
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 unetseg-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-11 14:43:39.872672 unetseg-0.2.4/LICENSE.txt
+-rw-r--r--   0        0        0      876 2023-06-29 12:31:41.710487 unetseg-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      363 2023-04-11 14:43:39.885340 unetseg-0.2.4/unetseg/__init__.py
+-rw-r--r--   0        0        0     3537 2023-04-11 14:43:39.885514 unetseg-0.2.4/unetseg/console/predict.py
+-rw-r--r--   0        0        0     4998 2023-04-11 14:43:39.885650 unetseg-0.2.4/unetseg/console/train.py
+-rw-r--r--   0        0        0     3861 2023-04-11 14:43:39.885769 unetseg-0.2.4/unetseg/evaluate.py
+-rw-r--r--   0        0        0     3662 2023-04-11 14:43:39.885918 unetseg-0.2.4/unetseg/postprocess.py
+-rw-r--r--   0        0        0     3842 2023-06-28 18:17:28.741172 unetseg-0.2.4/unetseg/predict.py
+-rw-r--r--   0        0        0    22114 2023-06-28 18:17:28.741393 unetseg-0.2.4/unetseg/train.py
+-rw-r--r--   0        0        0      842 2023-04-11 14:43:39.886391 unetseg-0.2.4/unetseg/utils.py
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 unetseg-0.2.4/PKG-INFO
```

### Comparing `unetseg-0.2.3/LICENSE.txt` & `unetseg-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/pyproject.toml` & `unetseg-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unetseg"
-version = "0.2.3"
+version = "0.2.4"
 description = "U-Net semantic segmentation for satellite imagery"
 authors = ["Damián Silvani <munshkr@gmail.com>"]
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 albumentations = "^1.1.0"
```

### Comparing `unetseg-0.2.3/unetseg/console/predict.py` & `unetseg-0.2.4/unetseg/console/predict.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/unetseg/console/train.py` & `unetseg-0.2.4/unetseg/console/train.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/unetseg/evaluate.py` & `unetseg-0.2.4/unetseg/evaluate.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/unetseg/postprocess.py` & `unetseg-0.2.4/unetseg/postprocess.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/unetseg/predict.py` & `unetseg-0.2.4/unetseg/predict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import warnings
-from dataclasses import dataclass
+from dataclasses import dataclass,field
 from glob import glob
 from typing import List
 
 import numpy as np
 import rasterio
 from sklearn.preprocessing import minmax_scale
 from tqdm import tqdm
@@ -22,15 +22,16 @@
     batch_size: int = 32
     model_architecture: str = "unet"
     model_path: str = "unet.h5"
     height: int = 320
     width: int = 320
     n_channels: int = 3
     n_classes: int = 1
-    class_weights: List[float] = []
+    class_weights: List[float] = field(default_factory=list)
+
 
 
 def predict(cfg: PredictConfig):
     """
     Performs inference based on a configuration object
 
     Parameters
```

### Comparing `unetseg-0.2.3/unetseg/train.py` & `unetseg-0.2.4/unetseg/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import math
 import os
 import random
 import warnings
-from dataclasses import dataclass
+from dataclasses import dataclass,field
 from glob import glob
 from typing import List, Tuple
 from datetime import datetime
 import albumentations as A
 import numpy as np
 import rasterio
 import tensorflow as tf
@@ -46,15 +46,15 @@
     test_split: float = 0.1
     epochs: int = 15
     steps_per_epoch: int = 2000
     early_stopping_patience: int = 3
     batch_size: int = 32
     seed: int = None
     evaluate: bool = True
-    class_weights: List[float] = []
+    class_weights: List[float] = field(default_factory=list)
 
 
 def build_model_unetplusplus(cfg: TrainConfig) -> Model:
     """
     Builds a U-Net++ model.
 
     Parameters
```

### Comparing `unetseg-0.2.3/unetseg/utils.py` & `unetseg-0.2.4/unetseg/utils.py`

 * *Files identical despite different names*

### Comparing `unetseg-0.2.3/PKG-INFO` & `unetseg-0.2.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unetseg
-Version: 0.2.3
+Version: 0.2.4
 Summary: U-Net semantic segmentation for satellite imagery
 License: Apache-2.0
 Author: Damián Silvani
 Author-email: munshkr@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

