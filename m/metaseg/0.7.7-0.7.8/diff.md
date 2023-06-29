# Comparing `tmp/metaseg-0.7.7.tar.gz` & `tmp/metaseg-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaseg-0.7.7.tar", max compression
+gzip compressed data, was "metaseg-0.7.8.tar", max compression
```

## Comparing `metaseg-0.7.7.tar` & `metaseg-0.7.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11357 2023-06-27 15:33:14.661577 metaseg-0.7.7/LICENSE
--rw-r--r--   0        0        0     4804 2023-06-27 15:33:14.661577 metaseg-0.7.7/README.md
--rw-r--r--   0        0        0      771 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/__init__.py
--rw-r--r--   0        0        0     2874 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/falai_demo.py
--rw-r--r--   0        0        0      438 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/__init__.py
--rw-r--r--   0        0        0    15292 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/automatic_mask_generator.py
--rw-r--r--   0        0        0     3094 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/build_sam.py
--rw-r--r--   0        0        0    11890 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/generator/predictor.py
--rw-r--r--   0        0        0     8395 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/mask_predictor.py
--rw-r--r--   0        0        0      749 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/__init__.py
--rw-r--r--   0        0        0     1479 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/common.py
--rw-r--r--   0        0        0    14851 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/image_encoder.py
--rw-r--r--   0        0        0     6800 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/mask_decoder.py
--rw-r--r--   0        0        0     8733 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/prompt_encoder.py
--rw-r--r--   0        0        0     7363 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/sam.py
--rw-r--r--   0        0        0     8436 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/modeling/transformer.py
--rw-r--r--   0        0        0     3548 2023-06-27 15:33:14.661577 metaseg-0.7.7/metaseg/sahi_predict.py
--rw-r--r--   0        0        0      924 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/__init__.py
--rw-r--r--   0        0        0    12711 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/amg.py
--rw-r--r--   0        0        0     2835 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/data_utils.py
--rw-r--r--   0        0        0     1295 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/file_utils.py
--rw-r--r--   0        0        0     5932 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/onnx.py
--rw-r--r--   0        0        0     4054 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/utils/transforms.py
--rw-r--r--   0        0        0       44 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/__init__.py
--rw-r--r--   0        0        0     8595 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/app.py
--rw-r--r--   0        0        0     2541 2023-06-27 15:33:14.665577 metaseg-0.7.7/metaseg/webapp/demo.py
--rw-r--r--   0        0        0     4112 2023-06-27 15:33:14.665577 metaseg-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     7406 1970-01-01 00:00:00.000000 metaseg-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 14:39:28.146075 metaseg-0.7.8/LICENSE
+-rw-r--r--   0        0        0     5046 2023-06-29 14:39:28.146075 metaseg-0.7.8/README.md
+-rw-r--r--   0        0        0      793 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/__init__.py
+-rw-r--r--   0        0        0     2859 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/falai_predictor.py
+-rw-r--r--   0        0        0      438 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/generator/__init__.py
+-rw-r--r--   0        0        0    15292 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/generator/automatic_mask_generator.py
+-rw-r--r--   0        0        0     3094 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/generator/build_sam.py
+-rw-r--r--   0        0        0    11890 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/generator/predictor.py
+-rw-r--r--   0        0        0      749 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/modeling/__init__.py
+-rw-r--r--   0        0        0     1479 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/modeling/common.py
+-rw-r--r--   0        0        0    14851 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/modeling/image_encoder.py
+-rw-r--r--   0        0        0     6800 2023-06-29 14:39:28.146075 metaseg-0.7.8/metaseg/modeling/mask_decoder.py
+-rw-r--r--   0        0        0     8733 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/modeling/prompt_encoder.py
+-rw-r--r--   0        0        0     7363 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/modeling/sam.py
+-rw-r--r--   0        0        0     8436 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/modeling/transformer.py
+-rw-r--r--   0        0        0     3617 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/sahi_predictor.py
+-rw-r--r--   0        0        0     8411 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/sam_predictor.py
+-rw-r--r--   0        0        0      837 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/__init__.py
+-rw-r--r--   0        0        0    12670 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/amg.py
+-rw-r--r--   0        0        0     2915 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/data_utils.py
+-rw-r--r--   0        0        0     3237 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/model_file_downloader.py
+-rw-r--r--   0        0        0     5932 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/onnx.py
+-rw-r--r--   0        0        0     4054 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/utils/transforms.py
+-rw-r--r--   0        0        0       44 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/webapp/__init__.py
+-rw-r--r--   0        0        0     8595 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/webapp/app.py
+-rw-r--r--   0        0        0     2547 2023-06-29 14:39:28.150075 metaseg-0.7.8/metaseg/webapp/demo.py
+-rw-r--r--   0        0        0     4133 2023-06-29 14:39:28.150075 metaseg-0.7.8/pyproject.toml
+-rw-r--r--   0        0        0     7690 1970-01-01 00:00:00.000000 metaseg-0.7.8/PKG-INFO
```

### Comparing `metaseg-0.7.7/LICENSE` & `metaseg-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/README.md` & `metaseg-0.7.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 </a>
 <a href="https://pypi.org/project/metaseg" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/metaseg.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 <a href="https://pypi.org/project/metaseg" target="_blank">
     <img src="https://img.shields.io/pypi/status/metaseg?color=orange" alt="Project Status">
 </a>
+<a href="https://results.pre-commit.ci/latest/github/kadirnar/segment-anything-video/main" target="_blank">
+    <img src="https://results.pre-commit.ci/badge/github/kadirnar/segment-anything-video/main.svg" alt="pre-commit.ci">
+</a>
 </p>
 
+
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 ### Installation
 ```bash
 pip install metaseg
 ```
 
@@ -97,25 +101,25 @@
 
 ```python
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
 image_path = "image.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
-    detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
+    detection_model_type="yolov5",  # yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
     slice_width=256,
     overlap_height_ratio=0.2,
     overlap_width_ratio=0.2,
 )
 
-SahiAutoSegmentation().predict(
+SahiAutoSegmentation().image_predict(
     source=image_path,
     model_type="vit_b",
     input_box=boxes,
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                        [downloads] [HuggingFace_Spaces]
 [Package_version] [Download_Count] [Supported_Python_versions] [Project_Status]
+                                [pre-commit.ci]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
@@ -20,27 +21,27 @@
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
 0, 100, 100], input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
 github.com/obss/sahi) + Segment Anything ```bash pip install sahi metaseg ```
 ```python from metaseg.sahi_predict import SahiAutoSegmentation,
 sahi_sliced_predict image_path = "image.jpg" boxes = sahi_sliced_predict
-( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+( image_path=image_path, detection_model_type="yolov5", # yolov8, detectron2,
 mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
 image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
-overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
-model_type="vit_b", input_box=boxes, multimask_output=False,
-random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
-GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install metaseg fal_serverless fal-serverless auth login ``` ```python #
-For Auto Mask from metaseg import falai_automask_image image =
-falai_automask_image( image_path="image.jpg", model_type="vit_b",
-points_per_side=16, points_per_batch=32, min_area=0, ) image.show() # Show
-image image.save("output.jpg") # Save image # For Manual Mask from metaseg
-import falai_manuelmask_image image = falai_manualmask_image
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().image_predict
+( source=image_path, model_type="vit_b", input_box=boxes,
+multimask_output=False, random_color=False, show=True, save=False, ) ```
+[teaser] ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart)
++ Segment Anything ```bash pip install metaseg fal_serverless fal-serverless
+auth login ``` ```python # For Auto Mask from metaseg import
+falai_automask_image image = falai_automask_image( image_path="image.jpg",
+model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
+image.show() # Show image image.save("output.jpg") # Save image # For Manual
+Mask from metaseg import falai_manuelmask_image image = falai_manualmask_image
 ( image_path="image.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
 200, 200], [100, 100, 200, 200]], multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
```

### Comparing `metaseg-0.7.7/metaseg/falai_demo.py` & `metaseg-0.7.8/metaseg/falai_predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from io import BytesIO
 
 from PIL import Image
 
-from metaseg.mask_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
-from metaseg.utils.data_utils import load_server_image
+from .sam_predictor import SegAutoMaskPredictor, SegManualMaskPredictor
+from .utils.data_utils import load_server_image
 
 try:
     from fal_serverless import isolated
 except ImportError:
     raise ImportError(
         "Please install FalAI library using 'pip install fal_serverless'."
     )
```

### Comparing `metaseg-0.7.7/metaseg/generator/automatic_mask_generator.py` & `metaseg-0.7.8/metaseg/generator/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/generator/build_sam.py` & `metaseg-0.7.8/metaseg/generator/build_sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/generator/predictor.py` & `metaseg-0.7.8/metaseg/generator/predictor.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/mask_predictor.py` & `metaseg-0.7.8/metaseg/sam_predictor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+from typing import Union
+
 import cv2
 import numpy as np
 import torch
+from cv2 import Mat
 from tqdm import tqdm
 
 from metaseg.generator.automatic_mask_generator import SamAutomaticMaskGenerator
 from metaseg.generator.build_sam import sam_model_registry
 from metaseg.generator.predictor import SamPredictor
 from metaseg.utils import (
     download_model,
     load_box,
     load_image,
     load_mask,
     load_video,
     multi_boxes,
-    save_image,
     show_image,
 )
 
 
 class SegAutoMaskPredictor:
     def __init__(self):
         self.model = None
@@ -29,15 +31,15 @@
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
     def image_predict(
         self,
-        source,
+        source: Union[str, Mat],
         model_type,
         points_per_side,
         points_per_batch,
         min_area,
         output_path="output.png",
         show=False,
         save=False,
@@ -73,15 +75,15 @@
 
         combined_mask = cv2.add(read_image, mask_image)
         self.combined_mask = combined_mask
         if show:
             show_image(combined_mask)
 
         if save:
-            save_image(output_path=output_path, output_image=combined_mask)
+            cv2.imwrite(output_path, combined_mask)
 
         return masks
 
     def video_predict(
         self,
         source,
         model_type,
@@ -153,15 +155,15 @@
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
     def image_predict(
         self,
-        source,
+        source: Union[str, Mat],
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
         output_path="output.png",
         random_color=False,
@@ -198,15 +200,15 @@
                 multimask_output=multimask_output,
             )
             mask_image = load_mask(masks, random_color)
             image = load_box(input_box, image)
 
         combined_mask = cv2.add(image, mask_image)
         if save:
-            save_image(output_path=output_path, output_image=combined_mask)
+            cv2.imwrite(output_path, combined_mask)
 
         if show:
             show_image(combined_mask)
 
         return masks
 
     def video_predict(
```

### Comparing `metaseg-0.7.7/metaseg/modeling/__init__.py` & `metaseg-0.7.8/metaseg/modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/common.py` & `metaseg-0.7.8/metaseg/modeling/common.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/image_encoder.py` & `metaseg-0.7.8/metaseg/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/mask_decoder.py` & `metaseg-0.7.8/metaseg/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/prompt_encoder.py` & `metaseg-0.7.8/metaseg/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/sam.py` & `metaseg-0.7.8/metaseg/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/modeling/transformer.py` & `metaseg-0.7.8/metaseg/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/sahi_predict.py` & `metaseg-0.7.8/metaseg/sahi_predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import Union
+
 import cv2
 import matplotlib.pyplot as plt
 import numpy as np
 import torch
+from cv2 import Mat
 from PIL import Image
 
 from metaseg.generator import SamPredictor, sam_model_registry
 from metaseg.utils import (
     download_model,
     load_image,
     multi_boxes,
@@ -67,17 +70,17 @@
         if self.model is None:
             self.model_path = download_model(model_type)
             self.model = sam_model_registry[model_type](checkpoint=self.model_path)
             self.model.to(device=self.device)
 
         return self.model
 
-    def predict(
+    def image_predict(
         self,
-        source,
+        source: Union[str, Mat],
         model_type,
         input_box=None,
         input_point=None,
         input_label=None,
         multimask_output=False,
         random_color=False,
         show=False,
```

### Comparing `metaseg-0.7.7/metaseg/utils/amg.py` & `metaseg-0.7.8/metaseg/utils/amg.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # LICENSE file in the root directory of this source tree.
 
 import math
 from copy import deepcopy
 from itertools import product
 from typing import Any, Dict, Generator, ItemsView, List, Tuple
 
+import cv2
 import numpy as np
 import torch
+from pycocotools import mask as mask_utils
 
 
 class MaskData:
     """
     A structure for storing masks and their related data in batched format.
     Implements basic filtering and concatenation.
     """
@@ -267,15 +269,14 @@
 def remove_small_regions(
     mask: np.ndarray, area_thresh: float, mode: str
 ) -> Tuple[np.ndarray, bool]:
     """
     Removes small disconnected regions and holes in a mask. Returns the
     mask and an indicator of if the mask has been modified.
     """
-    import cv2  # type: ignore
 
     assert mode in ["holes", "islands"]
     correct_holes = mode == "holes"
     working_mask = (correct_holes ^ mask).astype(np.uint8)
     n_labels, regions, stats, _ = cv2.connectedComponentsWithStats(working_mask, 8)
     sizes = stats[:, -1][1:]  # Row 0 is background label
     small_regions = [i + 1 for i, s in enumerate(sizes) if s < area_thresh]
@@ -288,16 +289,14 @@
         if len(fill_labels) == 0:
             fill_labels = [int(np.argmax(sizes)) + 1]
     mask = np.isin(regions, fill_labels)
     return mask, True
 
 
 def coco_encode_rle(uncompressed_rle: Dict[str, Any]) -> Dict[str, Any]:
-    from pycocotools import mask as mask_utils  # type: ignore
-
     h, w = uncompressed_rle["size"]
     rle = mask_utils.frPyObjects(uncompressed_rle, h, w)
     rle["counts"] = rle["counts"].decode("utf-8")  # Necessary to serialize with json
     return rle
 
 
 def batched_mask_to_box(masks: torch.Tensor) -> torch.Tensor:
```

### Comparing `metaseg-0.7.7/metaseg/utils/onnx.py` & `metaseg-0.7.8/metaseg/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/utils/transforms.py` & `metaseg-0.7.8/metaseg/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/webapp/app.py` & `metaseg-0.7.8/metaseg/webapp/app.py`

 * *Files identical despite different names*

### Comparing `metaseg-0.7.7/metaseg/webapp/demo.py` & `metaseg-0.7.8/metaseg/webapp/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         image_size=image_size,
         slice_height=slice_height,
         slice_width=slice_width,
         overlap_height_ratio=overlap_height_ratio,
         overlap_width_ratio=overlap_width_ratio,
     )
 
-    SahiAutoSegmentation().predict(
+    SahiAutoSegmentation().image_predict(
         source=image_path,
         model_type=sam_model_type,
         input_box=boxes,
         multimask_output=False,
         random_color=False,
         show=False,
         save=True,
```

### Comparing `metaseg-0.7.7/pyproject.toml` & `metaseg-0.7.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metaseg"
-version = "0.7.7"
+version = "0.7.8"
 description = "MetaSeg: Packaged version of the Segment Anything repository"
 authors = ["Kadir Nar <kadir.nar@hotmail.com>"]
 maintainers = ["Kadir Nar <kadir.nar@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "metaseg"}]
 homepage = "https://github.com/kadirnar/segment-anything-video"
 repository = "https://github.com/kadirnar/segment-anything-video"
@@ -49,14 +49,15 @@
 pycocotools = "^2.0.6"
 fal-serverless = "^0.6.35"
 sahi = "^0.11.14"
 onnx = { version = "^1.14.0", optional = true }
 onnxruntime =  { version ="^1.15.1", optional = true }
 ultralytics = { version = "^8.0.123", optional = true }
 yolov5 = { version ="^7.0.12", optional = true }
+requests = "^2.31.0"
 
 
 [tool.poetry.extras]
 full = ["onnxruntime","onnx","yolov5","ultralytics"]
 yolov5 = ["yolov5"]
 yolov8 = ["ultralytics"]
```

### Comparing `metaseg-0.7.7/PKG-INFO` & `metaseg-0.7.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaseg
-Version: 0.7.7
+Version: 0.7.8
 Summary: MetaSeg: Packaged version of the Segment Anything repository
 Home-page: https://github.com/kadirnar/segment-anything-video
 License: Apache-2.0
 Keywords: pytorch,segment-anything-video,metaseg
 Author: Kadir Nar
 Author-email: kadir.nar@hotmail.com
 Maintainer: Kadir Nar
@@ -39,14 +39,15 @@
 Requires-Dist: fal-serverless (>=0.6.35,<0.7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: onnx (>=1.14.0,<2.0.0) ; extra == "full"
 Requires-Dist: onnxruntime (>=1.15.1,<2.0.0) ; extra == "full"
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: pillow (>=9.5.0,<10.0.0)
 Requires-Dist: pycocotools (>=2.0.6,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sahi (>=0.11.14,<0.12.0)
 Requires-Dist: torch (>=2.0.1,<3.0.0)
 Requires-Dist: torchvision (>=0.15.2,<0.16.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: ultralytics (>=8.0.123,<9.0.0) ; extra == "full" or extra == "yolov8"
 Requires-Dist: yolov5 (>=7.0.12,<8.0.0) ; extra == "full" or extra == "yolov5"
 Project-URL: Documentation, https://github.com/kadirnar/segment-anything-video/blob/main/README.md
@@ -74,16 +75,20 @@
 </a>
 <a href="https://pypi.org/project/metaseg" target="_blank">
     <img src="https://img.shields.io/pypi/pyversions/metaseg.svg?color=%2334D058" alt="Supported Python versions">
 </a>
 <a href="https://pypi.org/project/metaseg" target="_blank">
     <img src="https://img.shields.io/pypi/status/metaseg?color=orange" alt="Project Status">
 </a>
+<a href="https://results.pre-commit.ci/latest/github/kadirnar/segment-anything-video/main" target="_blank">
+    <img src="https://results.pre-commit.ci/badge/github/kadirnar/segment-anything-video/main.svg" alt="pre-commit.ci">
+</a>
 </p>
 
+
 This repo is a packaged version of the [segment-anything](https://github.com/facebookresearch/segment-anything) model.
 
 ### Installation
 ```bash
 pip install metaseg
 ```
 
@@ -152,25 +157,25 @@
 
 ```python
 from metaseg.sahi_predict import SahiAutoSegmentation, sahi_sliced_predict
 
 image_path = "image.jpg"
 boxes = sahi_sliced_predict(
     image_path=image_path,
-    detection_model_type="yolov5", #yolov8, detectron2, mmdetection, torchvision
+    detection_model_type="yolov5",  # yolov8, detectron2, mmdetection, torchvision
     detection_model_path="yolov5l6.pt",
     conf_th=0.25,
     image_size=1280,
     slice_height=256,
     slice_width=256,
     overlap_height_ratio=0.2,
     overlap_width_ratio=0.2,
 )
 
-SahiAutoSegmentation().predict(
+SahiAutoSegmentation().image_predict(
     source=image_path,
     model_type="vit_b",
     input_box=boxes,
     multimask_output=False,
     random_color=False,
     show=True,
     save=False,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: metaseg Version: 0.7.7 Summary: MetaSeg: Packaged
+Metadata-Version: 2.1 Name: metaseg Version: 0.7.8 Summary: MetaSeg: Packaged
 version of the Segment Anything repository Home-page: https://github.com/
 kadirnar/segment-anything-video License: Apache-2.0 Keywords: pytorch,segment-
 anything-video,metaseg Author: Kadir Nar Author-email: kadir.nar@hotmail.com
 Maintainer: Kadir Nar Maintainer-email: kadir.nar@hotmail.com Requires-Python:
 >=3.8.1,<3.12.0 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
@@ -21,26 +21,28 @@
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
 :: Libraries :: Python Modules Provides-Extra: full Provides-Extra: yolov5
 Provides-Extra: yolov8 Requires-Dist: fal-serverless (>=0.6.35,<0.7.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: onnx
 (>=1.14.0,<2.0.0) ; extra == "full" Requires-Dist: onnxruntime
 (>=1.15.1,<2.0.0) ; extra == "full" Requires-Dist: opencv-python
 (>=4.7.0.72,<5.0.0.0) Requires-Dist: pillow (>=9.5.0,<10.0.0) Requires-Dist:
-pycocotools (>=2.0.6,<3.0.0) Requires-Dist: sahi (>=0.11.14,<0.12.0) Requires-
-Dist: torch (>=2.0.1,<3.0.0) Requires-Dist: torchvision (>=0.15.2,<0.16.0)
-Requires-Dist: tqdm (>=4.65.0,<5.0.0) Requires-Dist: ultralytics
-(>=8.0.123,<9.0.0) ; extra == "full" or extra == "yolov8" Requires-Dist: yolov5
-(>=7.0.12,<8.0.0) ; extra == "full" or extra == "yolov5" Project-URL:
-Documentation, https://github.com/kadirnar/segment-anything-video/blob/main/
-README.md Project-URL: Repository, https://github.com/kadirnar/segment-
-anything-video Description-Content-Type: text/markdown
+pycocotools (>=2.0.6,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: sahi (>=0.11.14,<0.12.0) Requires-Dist: torch (>=2.0.1,<3.0.0)
+Requires-Dist: torchvision (>=0.15.2,<0.16.0) Requires-Dist: tqdm
+(>=4.65.0,<5.0.0) Requires-Dist: ultralytics (>=8.0.123,<9.0.0) ; extra ==
+"full" or extra == "yolov8" Requires-Dist: yolov5 (>=7.0.12,<8.0.0) ; extra ==
+"full" or extra == "yolov5" Project-URL: Documentation, https://github.com/
+kadirnar/segment-anything-video/blob/main/README.md Project-URL: Repository,
+https://github.com/kadirnar/segment-anything-video Description-Content-Type:
+text/markdown
    ***** MetaSeg: Packaged version of the Segment Anything repository *****
                                    [teaser]
                        [downloads] [HuggingFace_Spaces]
 [Package_version] [Download_Count] [Supported_Python_versions] [Project_Status]
+                                [pre-commit.ci]
 This repo is a packaged version of the [segment-anything](https://github.com/
 facebookresearch/segment-anything) model. ### Installation ```bash pip install
 metaseg ``` ### Usage ```python from metaseg import SegAutoMaskPredictor,
 SegManualMaskPredictor # If gpu memory is not enough, reduce the
 points_per_side and points_per_batch. # For image results =
 SegAutoMaskPredictor().image_predict( source="image.jpg", model_type="vit_l", #
 vit_l, vit_h, vit_b points_per_side=16, points_per_batch=64, min_area=0,
@@ -55,27 +57,27 @@
 save=False, ) # For video results = SegManualMaskPredictor().video_predict
 ( source="video.mp4", model_type="vit_l", # vit_l, vit_h, vit_b input_point=[0,
 0, 100, 100], input_label=[0, 1], input_box=None, multimask_output=False,
 random_color=False, output_path="output.mp4", ) ``` ### [SAHI](https://
 github.com/obss/sahi) + Segment Anything ```bash pip install sahi metaseg ```
 ```python from metaseg.sahi_predict import SahiAutoSegmentation,
 sahi_sliced_predict image_path = "image.jpg" boxes = sahi_sliced_predict
-( image_path=image_path, detection_model_type="yolov5", #yolov8, detectron2,
+( image_path=image_path, detection_model_type="yolov5", # yolov8, detectron2,
 mmdetection, torchvision detection_model_path="yolov5l6.pt", conf_th=0.25,
 image_size=1280, slice_height=256, slice_width=256, overlap_height_ratio=0.2,
-overlap_width_ratio=0.2, ) SahiAutoSegmentation().predict( source=image_path,
-model_type="vit_b", input_box=boxes, multimask_output=False,
-random_color=False, show=True, save=False, ) ``` [teaser] ### [FalAI(Cloud
-GPU)](https://docs.fal.ai/fal-serverless/quickstart) + Segment Anything ```bash
-pip install metaseg fal_serverless fal-serverless auth login ``` ```python #
-For Auto Mask from metaseg import falai_automask_image image =
-falai_automask_image( image_path="image.jpg", model_type="vit_b",
-points_per_side=16, points_per_batch=32, min_area=0, ) image.show() # Show
-image image.save("output.jpg") # Save image # For Manual Mask from metaseg
-import falai_manuelmask_image image = falai_manualmask_image
+overlap_width_ratio=0.2, ) SahiAutoSegmentation().image_predict
+( source=image_path, model_type="vit_b", input_box=boxes,
+multimask_output=False, random_color=False, show=True, save=False, ) ```
+[teaser] ### [FalAI(Cloud GPU)](https://docs.fal.ai/fal-serverless/quickstart)
++ Segment Anything ```bash pip install metaseg fal_serverless fal-serverless
+auth login ``` ```python # For Auto Mask from metaseg import
+falai_automask_image image = falai_automask_image( image_path="image.jpg",
+model_type="vit_b", points_per_side=16, points_per_batch=32, min_area=0, )
+image.show() # Show image image.save("output.jpg") # Save image # For Manual
+Mask from metaseg import falai_manuelmask_image image = falai_manualmask_image
 ( image_path="image.jpg", model_type="vit_b", input_point=[[100, 100], [200,
 200]], input_label=[0, 1], input_box=[100, 100, 200, 200], # or [[100, 100,
 200, 200], [100, 100, 200, 200]], multimask_output=False, random_color=False, )
 image.show() # Show image image.save("output.jpg") # Save image ``` # Extra
 Features - [x] Support for Yolov5/8, Detectron2, Mmdetection, Torchvision
 models - [x] Support for video and web application(Huggingface Spaces) - [x]
 Support for manual single multi box and point selection - [x] Support for pip
```

