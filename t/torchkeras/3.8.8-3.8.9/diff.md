# Comparing `tmp/torchkeras-3.8.8.tar.gz` & `tmp/torchkeras-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchkeras-3.8.8.tar", last modified: Mon Jun 12 02:41:26 2023, max compression
+gzip compressed data, was "dist/torchkeras-3.8.9.tar", last modified: Thu Jun 29 13:43:04 2023, max compression
```

## Comparing `torchkeras-3.8.8.tar` & `torchkeras-3.8.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.388811 torchkeras-3.8.8/
--rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.8.8/LICENSE
--rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.8.8/MANIFEST.in
--rw-r--r--   0 liangyun2   (502) staff       (20)     5897 2023-06-12 02:41:26.388184 torchkeras-3.8.8/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)     9005 2023-06-06 09:33:44.000000 torchkeras-3.8.8/README.md
--rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-06-12 02:41:26.388934 torchkeras-3.8.8/setup.cfg
--rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-01 01:30:50.000000 torchkeras-3.8.8/setup.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.360227 torchkeras-3.8.8/torchkeras/
--rw-r--r--   0 liangyun2   (502) staff       (20)      232 2023-06-06 02:38:42.000000 torchkeras-3.8.8/torchkeras/__init__.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.383382 torchkeras-3.8.8/torchkeras/assets/
--rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.8.8/torchkeras/assets/SimHei.ttf
--rw-r--r--   0 liangyun2   (502) staff       (20)   487438 2023-02-09 16:00:16.000000 torchkeras-3.8.8/torchkeras/assets/bus.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.8.8/torchkeras/assets/park.jpg
--rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.8.8/torchkeras/assets/zidane.jpg
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.384701 torchkeras-3.8.8/torchkeras/chatgpt/
--rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.8.8/torchkeras/chatgpt/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     8640 2023-06-09 14:44:53.000000 torchkeras-3.8.8/torchkeras/data.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.8.8/torchkeras/eda.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.8.8/torchkeras/email.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    11507 2023-06-10 08:24:05.000000 torchkeras-3.8.8/torchkeras/hugmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10634 2023-06-06 02:38:43.000000 torchkeras-3.8.8/torchkeras/kerascallbacks.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    12128 2023-06-12 02:38:33.000000 torchkeras-3.8.8/torchkeras/kerasmodel.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.8.8/torchkeras/metrics.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.387673 torchkeras-3.8.8/torchkeras/models/
--rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.8.8/torchkeras/models/__init__.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.8.8/torchkeras/models/resnet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.8.8/torchkeras/models/ssd.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.8.8/torchkeras/models/unet.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.8.8/torchkeras/pbar.py
--rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.8.8/torchkeras/plots.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.8.8/torchkeras/soup.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.8.8/torchkeras/summary.py
--rw-r--r--   0 liangyun2   (502) staff       (20)     3694 2023-05-29 05:43:40.000000 torchkeras-3.8.8/torchkeras/utils.py
-drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-12 02:41:26.365427 torchkeras-3.8.8/torchkeras.egg-info/
--rw-r--r--   0 liangyun2   (502) staff       (20)     5897 2023-06-12 02:41:26.000000 torchkeras-3.8.8/torchkeras.egg-info/PKG-INFO
--rw-r--r--   0 liangyun2   (502) staff       (20)      737 2023-06-12 02:41:26.000000 torchkeras-3.8.8/torchkeras.egg-info/SOURCES.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-06-12 02:41:26.000000 torchkeras-3.8.8/torchkeras.egg-info/dependency_links.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-06-12 02:41:26.000000 torchkeras-3.8.8/torchkeras.egg-info/requires.txt
--rw-r--r--   0 liangyun2   (502) staff       (20)       26 2023-06-12 02:41:26.000000 torchkeras-3.8.8/torchkeras.egg-info/top_level.txt
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.536709 torchkeras-3.8.9/
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11325 2023-02-09 16:00:16.000000 torchkeras-3.8.9/LICENSE
+-rw-r--r--   0 liangyun2   (502) staff       (20)      357 2023-02-09 16:55:42.000000 torchkeras-3.8.9/MANIFEST.in
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-29 13:43:04.536179 torchkeras-3.8.9/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)    12396 2023-06-25 16:00:42.000000 torchkeras-3.8.9/README.md
+-rw-r--r--   0 liangyun2   (502) staff       (20)       38 2023-06-29 13:43:04.536936 torchkeras-3.8.9/setup.cfg
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1273 2023-06-01 01:30:50.000000 torchkeras-3.8.9/setup.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.509811 torchkeras-3.8.9/torchkeras/
+-rw-r--r--   0 liangyun2   (502) staff       (20)      246 2023-06-12 11:39:16.000000 torchkeras-3.8.9/torchkeras/__init__.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.530976 torchkeras-3.8.9/torchkeras/assets/
+-rw-r--r--   0 liangyun2   (502) staff       (20) 10043912 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/SimHei.ttf
+-rw-r--r--   0 liangyun2   (502) staff       (20)   487438 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/bus.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)  1012077 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/park.jpg
+-rw-r--r--   0 liangyun2   (502) staff       (20)   168949 2023-02-09 16:00:16.000000 torchkeras-3.8.9/torchkeras/assets/zidane.jpg
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.532099 torchkeras-3.8.9/torchkeras/chatgpt/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4178 2023-05-14 01:50:00.000000 torchkeras-3.8.9/torchkeras/chatgpt/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     8640 2023-06-09 14:44:53.000000 torchkeras-3.8.9/torchkeras/data.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5222 2023-04-13 09:25:41.000000 torchkeras-3.8.9/torchkeras/eda.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     1628 2023-04-13 07:46:39.000000 torchkeras-3.8.9/torchkeras/email.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    11531 2023-06-25 03:42:54.000000 torchkeras-3.8.9/torchkeras/hugmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10468 2023-06-14 13:45:41.000000 torchkeras-3.8.9/torchkeras/kerascallbacks.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    12601 2023-06-29 09:06:38.000000 torchkeras-3.8.9/torchkeras/kerasmodel.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     7316 2023-02-22 02:34:47.000000 torchkeras-3.8.9/torchkeras/metrics.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.535769 torchkeras-3.8.9/torchkeras/models/
+-rw-r--r--   0 liangyun2   (502) staff       (20)       75 2023-03-10 08:21:36.000000 torchkeras-3.8.9/torchkeras/models/__init__.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     4088 2023-02-24 04:01:48.000000 torchkeras-3.8.9/torchkeras/models/resnet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    31333 2023-05-20 15:18:08.000000 torchkeras-3.8.9/torchkeras/models/ssd.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3374 2023-02-21 12:33:54.000000 torchkeras-3.8.9/torchkeras/models/unet.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5444 2023-06-04 08:48:25.000000 torchkeras-3.8.9/torchkeras/pbar.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)    10676 2023-06-10 15:29:22.000000 torchkeras-3.8.9/torchkeras/plots.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5737 2023-05-12 10:11:52.000000 torchkeras-3.8.9/torchkeras/soup.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     5256 2023-05-28 13:14:40.000000 torchkeras-3.8.9/torchkeras/summary.py
+-rw-r--r--   0 liangyun2   (502) staff       (20)     3843 2023-06-12 11:38:27.000000 torchkeras-3.8.9/torchkeras/utils.py
+drwxr-xr-x   0 liangyun2   (502) staff       (20)        0 2023-06-29 13:43:04.512226 torchkeras-3.8.9/torchkeras.egg-info/
+-rw-r--r--   0 liangyun2   (502) staff       (20)     6252 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/PKG-INFO
+-rw-r--r--   0 liangyun2   (502) staff       (20)      737 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/SOURCES.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)        1 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/dependency_links.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       16 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/requires.txt
+-rw-r--r--   0 liangyun2   (502) staff       (20)       37 2023-06-29 13:43:04.000000 torchkeras-3.8.9/torchkeras.egg-info/top_level.txt
```

### Comparing `torchkeras-3.8.8/LICENSE` & `torchkeras-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/PKG-INFO` & `torchkeras-3.8.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.8
+Version: 3.8.9
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -121,20 +121,23 @@
 
 |example|model library  |notebook |
 |:----|:-----------|:-----------:|
 |ImageClassification——Resnet|  -  | [Resnet](./examples/ResNet.ipynb) |
 |ImageSegmentation——UNet|  - | [UNet](./examples/UNet.ipynb) |
 |ObjectDetection——SSD| -  | [SSD](./examples/SSD.ipynb) |
 |OCR——CRNN 🔥🔥| -  | [CRNN-CTC](./examples/CRNN_CTC.ipynb) |
+|ReinforcementLearning——Q-Learning🔥🔥|- |[Q-learning](./examples/Q-learning.ipynb)|
+|ReinforcementLearning——DQN|- |[DQN](./examples/DQN.ipynb)|
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
-|ImageSegmentation——DeepLabV3++ 🔥| segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
-|InstanceSegmentation——MaskRCNN 🔥🔥| detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
+|ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
+|InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
-|TextClassification——BERT 🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
-
+|TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
+|TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
+|ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 
 **If you want to understand or modify some details of this project, feel free to read and change the source code!!!**
 
 Any other questions, you can contact the author form the wechat official account below:
 
 **算法美食屋**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.8 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.8.9 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -56,19 +56,25 @@
 | ### 4, Advanced Examples In some using cases, because of the differences of
 the model input types, you need to rewrite the StepRunner of KerasModel. Here
 are some examples. |example|model library |notebook | |:----|:-----------|:----
 -------:| |ImageClassificationââResnet| - | [Resnet](./examples/
 ResNet.ipynb) | |ImageSegmentationââUNet| - | [UNet](./examples/UNet.ipynb)
 | |ObjectDetectionââSSD| - | [SSD](./examples/SSD.ipynb) | |OCRââCRNN
 ð¥ð¥| - | [CRNN-CTC](./examples/CRNN_CTC.ipynb) |
-|ObjectDetectionââFasterRCNN| torchvision | [FasterRCNN](./examples/
-FasterRCNNââvision.ipynb) | |ImageSegmentationââDeepLabV3++ ð¥|
+|ReinforcementLearningââQ-Learningð¥ð¥|- |[Q-learning](./examples/Q-
+learning.ipynb)| |ReinforcementLearningââDQN|- |[DQN](./examples/
+DQN.ipynb)| |ObjectDetectionââFasterRCNN| torchvision | [FasterRCNN](./
+examples/FasterRCNNââvision.ipynb) | |ImageSegmentationââDeepLabV3++ |
 segmentation_models_pytorch | [Deeplabv3++](./examples/
-Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN ð¥ð¥|
+Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
-YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥|
-transformers | [BERT](./examples/BERTââtransformers.ipynb) | **If you want
-to understand or modify some details of this project, feel free to read and
-change the source code!!!** Any other questions, you can contact the author
-form the wechat official account below: **ç®æ³ç¾é£å±** ![](https://
-tva1.sinaimg.cn/large/e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
+YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥ð¥|
+transformers | [BERT](./examples/BERTââtransformers.ipynb) |
+|TokenClassificationââBERT | transformers | [BERT_NER](./examples/
+BERT_NERââtransformers.ipynb) |
+|ImageClassificationââSwinTransformer|timm| [Swin](./examples/
+SwinTransformerââtimm.ipynb)| **If you want to understand or modify some
+details of this project, feel free to read and change the source code!!!** Any
+other questions, you can contact the author form the wechat official account
+below: **ç®æ³ç¾é£å±** ![](https://tva1.sinaimg.cn/large/
+e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
```

### Comparing `torchkeras-3.8.8/setup.py` & `torchkeras-3.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/assets/SimHei.ttf` & `torchkeras-3.8.9/torchkeras/assets/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/assets/bus.jpg` & `torchkeras-3.8.9/torchkeras/assets/bus.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/assets/park.jpg` & `torchkeras-3.8.9/torchkeras/assets/park.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/assets/zidane.jpg` & `torchkeras-3.8.9/torchkeras/assets/zidane.jpg`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/chatgpt/__init__.py` & `torchkeras-3.8.9/torchkeras/chatgpt/__init__.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/data.py` & `torchkeras-3.8.9/torchkeras/data.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/eda.py` & `torchkeras-3.8.9/torchkeras/eda.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/email.py` & `torchkeras-3.8.9/torchkeras/email.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/hugmodel.py` & `torchkeras-3.8.9/torchkeras/hugmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         for k,m in self.metrics_dict.items():
             m.reset()
         return result 
     
     def get_collate_fn(self, default_fn):
         def collate_fn(examples):
             batch = default_fn(examples)
-            if isinstance(batch,dict):
+            if hasattr(batch,'keys') and hasattr(batch,'pop'):
                 return batch
             elif isinstance(batch, (list,tuple)):
                 if len(batch)==2:
                     return {'features':batch[0],'labels':batch[1]}
             else:
                 raise Exception('dataset format error!')
         return collate_fn
```

### Comparing `torchkeras-3.8.8/torchkeras/kerascallbacks.py` & `torchkeras-3.8.9/torchkeras/kerascallbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os 
 import sys
 import datetime 
 from copy import deepcopy
 import numpy as np 
 import pandas as pd 
 from argparse import Namespace 
-from .plots import plot_metric
 
 class TensorBoardCallback:
     def __init__(self, save_dir= "runs", model_name="model", 
                  log_weight=False, log_weight_freq=5):
         from torch.utils.tensorboard import SummaryWriter 
         self.__dict__.update(locals())
         nowtime = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
@@ -118,19 +117,15 @@
         dfhistory.to_csv(os.path.join(self.wb.run.dir,'dfhistory.csv'),index=None) 
         
         #save ckpt
         if self.save_ckpt:
             arti_model = self.wb.Artifact('checkpoint', type='model')
             arti_model.add_file(model.ckpt_path)
             self.wb.log_artifact(arti_model)
-                 
-        #plotly metrics
-        metrics = [x.replace('train_','').replace('val_','') for x in dfhistory.columns if 'train_' in x] 
-        metric_fig = {m+'_curve':plot_metric(dfhistory,m) for m in metrics}
-        self.wb.log(metric_fig)
+
         run_dir = self.wb.run.dir
         self.wb.finish()
 
         #local save
         import shutil
         shutil.copy(model.ckpt_path,os.path.join(run_dir,os.path.basename(model.ckpt_path)))
     
@@ -210,15 +205,15 @@
         m2 = 'val_'+self.metric
         if m2 in dfhistory.columns:
             val_metrics = dfhistory[m2]
             self.graph_ax.plot(epochs,val_metrics,'ro-',label =m2)
 
         if self.metric in dfhistory.columns:
             metric_values = dfhistory[self.metric]
-            self.graph_ax.plot(epochs, metric_values,'go-', label = self.metric)
+            self.graph_ax.plot(epochs, metric_values,'ro-', label = self.metric)
 
         self.graph_ax.set_xlabel("epoch")
         self.graph_ax.set_ylabel(self.metric)  
         if title:
              self.graph_ax.set_title(title)
         if m1 in dfhistory.columns or m2 in dfhistory.columns or self.metric in dfhistory.columns:
             self.graph_ax.legend(loc='best')
@@ -226,18 +221,19 @@
         if x_bounds is not None: self.graph_ax.set_xlim(*x_bounds)
         if y_bounds is not None: self.graph_ax.set_ylim(*y_bounds)
         self.graph_out.update(self.graph_ax.figure)
         self.plt.close();
         
 
 class VisDisplay:
-    def __init__(self,display_fn,model=None,init_display=True):
+    def __init__(self,display_fn,model=None,init_display=True,dis_period=1):
         from ipywidgets import Output 
         self.display_fn = display_fn
         self.init_display = init_display
+        self.dis_period = dis_period
         self.out = Output()
         
         if self.init_display:
             display(self.out)
             with self.out:
                 self.display_fn(model)
         
@@ -245,17 +241,18 @@
         if not self.init_display:
             display(self.out)
 
     def on_train_epoch_end(self,model:'KerasModel'):
         pass
     
     def on_validation_epoch_end(self, model:"KerasModel"):
-        self.out.clear_output()
-        with self.out:
-            self.display_fn(model)
+        if len(model.history['epoch'])%self.dis_period==0:
+            self.out.clear_output()
+            with self.out:
+                self.display_fn(model)
            
     def on_fit_end(self,  model:"KerasModel"):
         pass
         
         
 class EpochCheckpoint:
     def __init__(self, ckpt_dir= "weights",
```

### Comparing `torchkeras-3.8.8/torchkeras/kerasmodel.py` & `torchkeras-3.8.9/torchkeras/kerasmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import sys,datetime
 from tqdm import tqdm
 from copy import deepcopy
 import numpy as np
 import pandas as pd
 import torch
 from accelerate import Accelerator
-from .utils import colorful,is_jupyter
 
 class StepRunner:
-    def __init__(self, net, loss_fn, accelerator, stage = "train", metrics_dict = None, 
+    def __init__(self, net, loss_fn, accelerator=None, stage = "train", metrics_dict = None, 
                  optimizer = None, lr_scheduler = None
                  ):
         self.net,self.loss_fn,self.metrics_dict,self.stage = net,loss_fn,metrics_dict,stage
         self.optimizer,self.lr_scheduler = optimizer,lr_scheduler
-        self.accelerator = accelerator
+        self.accelerator = accelerator if accelerator is not None else Accelerator() 
         if self.stage=='train':
             self.net.train() 
         else:
             self.net.eval()
     
     def __call__(self, batch):
         features,labels = batch 
@@ -33,22 +32,22 @@
             if self.accelerator.sync_gradients:
                 self.accelerator.clip_grad_norm_(self.net.parameters(), 1.0)
             self.optimizer.step()
             if self.lr_scheduler is not None:
                 self.lr_scheduler.step()
             self.optimizer.zero_grad()
             
+        all_loss = self.accelerator.gather(loss).sum()
         all_preds = self.accelerator.gather(preds)
         all_labels = self.accelerator.gather(labels)
-        all_loss = self.accelerator.gather(loss).sum()
         
-        #losses (plain metrics)
+        #losses (or plain metrics that can be averaged)
         step_losses = {self.stage+"_loss":all_loss.item()}
         
-        #metrics (state metrics)
+        #metrics (stateful metrics)
         step_metrics = {self.stage+"_"+name:metric_fn(all_preds, all_labels).item() 
                         for name,metric_fn in self.metrics_dict.items()}
         
         if self.stage=="train":
             if self.optimizer is not None:
                 step_metrics['lr'] = self.optimizer.state_dict()['param_groups'][0]['lr']
             else:
@@ -82,89 +81,96 @@
                 if step<n:
                     loop.set_postfix(**step_log)
             
                     if hasattr(self,'progress') and self.accelerator.is_local_main_process:
                         post_log = dict(**{'i':step,'n':n},**step_log)
                         self.progress.set_postfix(**post_log)
 
-                        
                 elif step==n:
                     epoch_metrics = step_metrics
                     epoch_metrics.update({self.stage+"_"+name:metric_fn.compute().item() 
                                      for name,metric_fn in self.steprunner.metrics_dict.items()})
                     epoch_losses = {k:v/step for k,v in epoch_losses.items()}
                     epoch_log = dict(epoch_losses,**epoch_metrics)
                     loop.set_postfix(**epoch_log)
                     
                     if hasattr(self,'progress') and self.accelerator.is_local_main_process:
                         post_log = dict(**{'i':step,'n':n},**epoch_log)
                         self.progress.set_postfix(**post_log)
                     
                     for name,metric_fn in self.steprunner.metrics_dict.items():
-                        metric_fn.reset()
+                        metric_fn.reset()  
                 else:
                     break
         return epoch_log
 
 class KerasModel(torch.nn.Module):
     
     StepRunner,EpochRunner = StepRunner,EpochRunner
     
     def __init__(self,net,loss_fn,metrics_dict=None,optimizer=None,lr_scheduler = None):
         super().__init__()
         self.net,self.loss_fn,self.metrics_dict = net, loss_fn, torch.nn.ModuleDict(metrics_dict) 
         self.optimizer = optimizer if optimizer is not None else torch.optim.Adam(
-            self.net.parameters(), lr=1e-3)
+            self.net.parameters(), lr=3e-4)
         self.lr_scheduler = lr_scheduler
         self.from_scratch = True
         
+    def save_ckpt(self, ckpt_path='checkpoint.pt'):
+        net_dict = self.accelerator.get_state_dict(self.net)
+        self.accelerator.save(net_dict,ckpt_path)
+      
     def load_ckpt(self, ckpt_path='checkpoint.pt'):
         self.net.load_state_dict(torch.load(ckpt_path))
         self.from_scratch = False
 
     def forward(self, x):
         return self.net.forward(x)
     
     def fit(self, train_data, val_data=None, epochs=10, ckpt_path='checkpoint.pt',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
-            plot=True, wandb=False, quiet=None, 
+            plot=True,  wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1):
         
+        from torchkeras.utils import colorful,is_jupyter
+        
         self.__dict__.update(locals())
         self.accelerator = Accelerator(mixed_precision=mixed_precision,cpu=cpu,
             gradient_accumulation_steps=gradient_accumulation_steps)
         device = str(self.accelerator.device)
-        device_type = '🐌'  if 'cpu' in device else '⚡️'
+        device_type = '🐌'  if 'cpu' in device else ('⚡️' if 'cuda' in device else '🚀')
         self.accelerator.print(
             colorful("<<<<<< "+device_type +" "+ device +" is used >>>>>>"))
     
         self.net,self.loss_fn,self.metrics_dict,self.optimizer,self.lr_scheduler= self.accelerator.prepare(
             self.net,self.loss_fn,self.metrics_dict,self.optimizer,self.lr_scheduler)
         
         train_dataloader,val_dataloader = self.accelerator.prepare(train_data,val_data)
+        train_dataloader.size = train_data.size if hasattr(train_data,'size') else len(train_data)
+        if val_data:
+            val_dataloader.size = val_data.size if hasattr(val_data,'size') else len(val_data)
+        
         
         self.history = {}
         callbacks = callbacks if callbacks is not None else []
         
-        if bool(plot)!=False:
-            if is_jupyter():
-                from .kerascallbacks import VisMetric,VisProgress
-                callbacks = [VisMetric(),VisProgress()]+callbacks
+        if bool(plot) and is_jupyter():
+            from torchkeras.kerascallbacks import VisMetric,VisProgress
+            callbacks = [VisMetric(),VisProgress()]+callbacks
                 
         if wandb!=False:
-            from .kerascallbacks import WandbCallback
+            from torchkeras.kerascallbacks import WandbCallback
             project = wandb if isinstance(wandb,str) else 'torchkeras'
             callbacks.append(WandbCallback(project=project))
             
         self.callbacks = [self.accelerator.prepare(x) for x in callbacks]
         
         if self.accelerator.is_local_main_process:
-            for callback_obj in self.callbacks:
-                callback_obj.on_fit_start(model = self)
-        
+            [cb.on_fit_start(model = self) for cb in self.callbacks if hasattr(cb,'on_fit_start')]
+                
         start_epoch = 1 if self.from_scratch else 0
         
         if quiet is None:
             if is_jupyter():
                 quiet = True
             else:
                 quiet = False
@@ -196,17 +202,17 @@
             train_metrics = {'epoch':epoch}
             train_metrics.update(train_epoch_runner(train_dataloader))
 
             for name, metric in train_metrics.items():
                 self.history[name] = self.history.get(name, []) + [metric]
 
             if self.accelerator.is_local_main_process:
-                for callback_obj in self.callbacks:
-                    callback_obj.on_train_epoch_end(model = self)
-
+                [cb.on_train_epoch_end(model = self) for cb in self.callbacks 
+                 if hasattr(cb,'on_train_epoch_end')]
+                
             # 2，validate -------------------------------------------------
             if val_dataloader is not None:
                 val_step_runner = self.StepRunner(
                     net = self.net,
                     loss_fn = self.loss_fn,
                     accelerator = self.accelerator,
                     stage="val",
@@ -215,43 +221,42 @@
                 val_epoch_runner = self.EpochRunner(val_step_runner,should_quiet)
                 with torch.no_grad():
                     val_metrics = val_epoch_runner(val_dataloader)
 
                 for name, metric in val_metrics.items():
                     self.history[name] = self.history.get(name, []) + [metric]
                 
-                if self.accelerator.is_local_main_process:
-                    for callback_obj in self.callbacks:
-                        callback_obj.on_validation_epoch_end(model = self)
+            if self.accelerator.is_local_main_process:
+                [cb.on_validation_epoch_end(model = self) for cb in self.callbacks 
+                 if hasattr(cb,'on_validation_epoch_end')]
 
             # 3，early-stopping -------------------------------------------------
             self.accelerator.wait_for_everyone()
             arr_scores = self.history[monitor]
             best_score_idx = np.argmax(arr_scores) if mode=="max" else np.argmin(arr_scores)
 
             if best_score_idx==len(arr_scores)-1:
-                net_dict = self.accelerator.get_state_dict(self.net)
-                self.accelerator.save(net_dict,ckpt_path)
+                self.save_ckpt(ckpt_path)
                 if not should_quiet:
                     self.accelerator.print(colorful("<<<<<< reach best {0} : {1} >>>>>>".format(
                         monitor,arr_scores[best_score_idx])))
 
             if len(arr_scores)-best_score_idx>patience:
                 self.accelerator.print(colorful(
                     "<<<<<< {} without improvement in {} epoch,""early stopping >>>>>>"
                 ).format(monitor,patience))
                 break; 
                 
         if self.accelerator.is_local_main_process:   
             dfhistory = pd.DataFrame(self.history)
-            for callback_obj in self.callbacks:
-                callback_obj.on_fit_end(model = self)
-        
+            [cb.on_fit_end(model = self) for cb in self.callbacks 
+                 if hasattr(cb,'on_fit_end')]
             self.net = self.accelerator.unwrap_model(self.net)
-            self.net.load_state_dict(torch.load(ckpt_path))
+            self.net.cpu()
+            self.load_ckpt(ckpt_path)
             return dfhistory
     
     @torch.no_grad()
     def evaluate(self, val_data, quiet=False):
         accelerator = Accelerator() if not hasattr(self,'accelerator') else self.accelerator
         self.net,self.loss_fn,self.metrics_dict = accelerator.prepare(self.net,self.loss_fn,self.metrics_dict)
         val_data = accelerator.prepare(val_data)
@@ -266,11 +271,11 @@
             val_data=None, epochs=10, ckpt_path='checkpoint.pt',
             patience=5, monitor="val_loss", mode="min", callbacks=None, 
             plot=True, wandb=False, quiet=None, 
             mixed_precision='no', cpu=False, gradient_accumulation_steps=1
            ):
         args = (train_data,val_data,epochs,ckpt_path,patience,monitor,mode,
             callbacks,plot,wandb,quiet,mixed_precision,cpu,gradient_accumulation_steps)
-    
+        
         from accelerate import notebook_launcher
         notebook_launcher(self.fit, args, num_processes=num_processes)
```

### Comparing `torchkeras-3.8.8/torchkeras/metrics.py` & `torchkeras-3.8.9/torchkeras/metrics.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/models/resnet.py` & `torchkeras-3.8.9/torchkeras/models/resnet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/models/ssd.py` & `torchkeras-3.8.9/torchkeras/models/ssd.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/models/unet.py` & `torchkeras-3.8.9/torchkeras/models/unet.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/pbar.py` & `torchkeras-3.8.9/torchkeras/pbar.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/plots.py` & `torchkeras-3.8.9/torchkeras/plots.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/soup.py` & `torchkeras-3.8.9/torchkeras/soup.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/summary.py` & `torchkeras-3.8.9/torchkeras/summary.py`

 * *Files identical despite different names*

### Comparing `torchkeras-3.8.8/torchkeras/utils.py` & `torchkeras-3.8.9/torchkeras/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,22 @@
     random.seed(seed)
     os.environ['PYTHONHASHSEED'] = str(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
     return seed
 
-
+def delete_object(obj):
+    import gc
+    obj = None
+    gc.collect()
+    del obj
+    with torch.no_grad():
+        torch.cuda.empty_cache()
+        
 def colorful(obj,color="red", display_type="plain"):
     # 彩色输出格式：
     # 设置颜色开始 ：\033[显示方式;前景色;背景色m
     # 说明：
     # 前景色            背景色           颜色
     # ---------------------------------------
     # 30                40              黑色
```

### Comparing `torchkeras-3.8.8/torchkeras.egg-info/PKG-INFO` & `torchkeras-3.8.9/torchkeras.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchkeras
-Version: 3.8.8
+Version: 3.8.9
 Summary: pytorch❤️keras
 Home-page: https://github.com/lyhue1991/torchkeras
 Author: PythonAiRoad, Laugh
 Author-email: lyhue1991@163.com
 Keywords: machine-learning,deep-learning,ML,DL,pytorch,torch,keras
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -121,20 +121,23 @@
 
 |example|model library  |notebook |
 |:----|:-----------|:-----------:|
 |ImageClassification——Resnet|  -  | [Resnet](./examples/ResNet.ipynb) |
 |ImageSegmentation——UNet|  - | [UNet](./examples/UNet.ipynb) |
 |ObjectDetection——SSD| -  | [SSD](./examples/SSD.ipynb) |
 |OCR——CRNN 🔥🔥| -  | [CRNN-CTC](./examples/CRNN_CTC.ipynb) |
+|ReinforcementLearning——Q-Learning🔥🔥|- |[Q-learning](./examples/Q-learning.ipynb)|
+|ReinforcementLearning——DQN|- |[DQN](./examples/DQN.ipynb)|
 |ObjectDetection——FasterRCNN| torchvision  |  [FasterRCNN](./examples/FasterRCNN——vision.ipynb) | 
-|ImageSegmentation——DeepLabV3++ 🔥| segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
-|InstanceSegmentation——MaskRCNN 🔥🔥| detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
+|ImageSegmentation——DeepLabV3++ | segmentation_models_pytorch |  [Deeplabv3++](./examples/Deeplabv3plus——smp.ipynb) |
+|InstanceSegmentation——MaskRCNN | detectron2 |  [MaskRCNN](./examples/MaskRCNN——detectron2.ipynb) |
 |ObjectDetection——YOLOv8 🔥🔥| ultralytics |  [YOLOv8](./examples/YOLOv8——ultralytics.ipynb) |
-|TextClassification——BERT 🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
-
+|TextClassification——BERT 🔥🔥| transformers |  [BERT](./examples/BERT——transformers.ipynb) |
+|TokenClassification——BERT | transformers |  [BERT_NER](./examples/BERT_NER——transformers.ipynb) |
+|ImageClassification——SwinTransformer|timm| [Swin](./examples/SwinTransformer——timm.ipynb)|
 
 **If you want to understand or modify some details of this project, feel free to read and change the source code!!!**
 
 Any other questions, you can contact the author form the wechat official account below:
 
 **算法美食屋**
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchkeras Version: 3.8.8 Summary:
+Metadata-Version: 2.1 Name: torchkeras Version: 3.8.9 Summary:
 pytorchâ¤ï¸keras Home-page: https://github.com/lyhue1991/torchkeras Author:
 PythonAiRoad, Laugh Author-email: lyhue1991@163.com Keywords: machine-
 learning,deep-learning,ML,DL,pytorch,torch,keras Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.5
 Description-Content-Type: text/markdown License-File: LICENSE #
 Pytorchâ¤ï¸Keras English | [ç®ä½ä¸­æ](README.md) The torchkeras library
@@ -56,19 +56,25 @@
 | ### 4, Advanced Examples In some using cases, because of the differences of
 the model input types, you need to rewrite the StepRunner of KerasModel. Here
 are some examples. |example|model library |notebook | |:----|:-----------|:----
 -------:| |ImageClassificationââResnet| - | [Resnet](./examples/
 ResNet.ipynb) | |ImageSegmentationââUNet| - | [UNet](./examples/UNet.ipynb)
 | |ObjectDetectionââSSD| - | [SSD](./examples/SSD.ipynb) | |OCRââCRNN
 ð¥ð¥| - | [CRNN-CTC](./examples/CRNN_CTC.ipynb) |
-|ObjectDetectionââFasterRCNN| torchvision | [FasterRCNN](./examples/
-FasterRCNNââvision.ipynb) | |ImageSegmentationââDeepLabV3++ ð¥|
+|ReinforcementLearningââQ-Learningð¥ð¥|- |[Q-learning](./examples/Q-
+learning.ipynb)| |ReinforcementLearningââDQN|- |[DQN](./examples/
+DQN.ipynb)| |ObjectDetectionââFasterRCNN| torchvision | [FasterRCNN](./
+examples/FasterRCNNââvision.ipynb) | |ImageSegmentationââDeepLabV3++ |
 segmentation_models_pytorch | [Deeplabv3++](./examples/
-Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN ð¥ð¥|
+Deeplabv3plusââsmp.ipynb) | |InstanceSegmentationââMaskRCNN |
 detectron2 | [MaskRCNN](./examples/MaskRCNNââdetectron2.ipynb) |
 |ObjectDetectionââYOLOv8 ð¥ð¥| ultralytics | [YOLOv8](./examples/
-YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥|
-transformers | [BERT](./examples/BERTââtransformers.ipynb) | **If you want
-to understand or modify some details of this project, feel free to read and
-change the source code!!!** Any other questions, you can contact the author
-form the wechat official account below: **ç®æ³ç¾é£å±** ![](https://
-tva1.sinaimg.cn/large/e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
+YOLOv8ââultralytics.ipynb) | |TextClassificationââBERT ð¥ð¥|
+transformers | [BERT](./examples/BERTââtransformers.ipynb) |
+|TokenClassificationââBERT | transformers | [BERT_NER](./examples/
+BERT_NERââtransformers.ipynb) |
+|ImageClassificationââSwinTransformer|timm| [Swin](./examples/
+SwinTransformerââtimm.ipynb)| **If you want to understand or modify some
+details of this project, feel free to read and change the source code!!!** Any
+other questions, you can contact the author form the wechat official account
+below: **ç®æ³ç¾é£å±** ![](https://tva1.sinaimg.cn/large/
+e6c9d24egy1h41m2zugguj20k00b9q46.jpg)
```

### Comparing `torchkeras-3.8.8/torchkeras.egg-info/SOURCES.txt` & `torchkeras-3.8.9/torchkeras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

