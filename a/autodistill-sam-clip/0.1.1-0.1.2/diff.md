# Comparing `tmp/autodistill-sam-clip-0.1.1.tar.gz` & `tmp/autodistill-sam-clip-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill-sam-clip-0.1.1.tar", last modified: Mon Jun 12 08:32:57 2023, max compression
+gzip compressed data, was "autodistill-sam-clip-0.1.2.tar", last modified: Thu Jun 29 13:46:33 2023, max compression
```

## Comparing `autodistill-sam-clip-0.1.1.tar` & `autodistill-sam-clip-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.401580 autodistill-sam-clip-0.1.1/
--rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 18:33:41.000000 autodistill-sam-clip-0.1.1/LICENSE
--rw-r--r--   0 james      (501) staff       (20)      479 2023-06-12 08:32:57.401338 autodistill-sam-clip-0.1.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1884 2023-06-09 18:57:56.000000 autodistill-sam-clip-0.1.1/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.399587 autodistill-sam-clip-0.1.1/autodistill_sam_clip/
--rw-r--r--   0 james      (501) staff       (20)       73 2023-06-09 18:45:16.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     2798 2023-06-12 08:32:31.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/helpers.py
--rw-r--r--   0 james      (501) staff       (20)     5206 2023-06-12 08:29:22.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip/sam_clip.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-12 08:32:57.401024 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/
--rw-r--r--   0 james      (501) staff       (20)      479 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      343 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      138 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       21 2023-06-12 08:32:57.000000 autodistill-sam-clip-0.1.1/autodistill_sam_clip.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-12 08:32:57.401656 autodistill-sam-clip-0.1.1/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1469 2023-06-12 08:32:01.000000 autodistill-sam-clip-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.570834 autodistill-sam-clip-0.1.2/
+-rw-r--r--   0 james      (501) staff       (20)    11356 2023-06-09 18:33:41.000000 autodistill-sam-clip-0.1.2/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)      491 2023-06-29 13:46:33.570680 autodistill-sam-clip-0.1.2/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1903 2023-06-29 13:44:02.000000 autodistill-sam-clip-0.1.2/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.569340 autodistill-sam-clip-0.1.2/autodistill_sam_clip/
+-rw-r--r--   0 james      (501) staff       (20)       73 2023-06-29 13:46:14.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     2798 2023-06-12 08:32:31.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/helpers.py
+-rw-r--r--   0 james      (501) staff       (20)     4528 2023-06-28 10:56:59.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip/sam_clip.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-29 13:46:33.570475 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)      491 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      343 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      138 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       21 2023-06-29 13:46:33.000000 autodistill-sam-clip-0.1.2/autodistill_sam_clip.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-29 13:46:33.570895 autodistill-sam-clip-0.1.2/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1481 2023-06-29 13:43:39.000000 autodistill-sam-clip-0.1.2/setup.py
```

### Comparing `autodistill-sam-clip-0.1.1/LICENSE` & `autodistill-sam-clip-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill-sam-clip-0.1.1/README.md` & `autodistill-sam-clip-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 Read the full [Autodistill documentation](https://autodistill.github.io/autodistill/).
 
 Read the [SAM-CLIP Autodistill documentation](https://autodistill.github.io/autodistill/base_models/sam-clip/).
 
 ## Installation
 
-To use the Grounded SAM base model, you will need to install the following dependency:
+To use the SAM-CLIP base model, you will need to install the following dependency:
 
 ```bash
 pip3 install autodistill-sam-clip
 ```
 
 ## Quickstart
 
@@ -43,12 +43,12 @@
 
 # label all images in a folder called `context_images`
 base_model.label("./context_images", extension=".jpeg")
 ```
 
 ## License
 
-The code in this repository is licensed under an [Apache 2.0 license](LICENSE).
+SAM licensed under an [Apache 2.0 license](LICENSE). CLIP is licensed under an [MIT license](LICENSE).
 
 ## 🏆 Contributing
 
 We love your input! Please see the core Autodistill [contributing guide](https://github.com/autodistill/autodistill/blob/main/CONTRIBUTING.md) to get started. Thank you 🙏 to all our contributors!
```

### Comparing `autodistill-sam-clip-0.1.1/autodistill_sam_clip/helpers.py` & `autodistill-sam-clip-0.1.2/autodistill_sam_clip/helpers.py`

 * *Files identical despite different names*

### Comparing `autodistill-sam-clip-0.1.1/autodistill_sam_clip/sam_clip.py` & `autodistill-sam-clip-0.1.2/autodistill_sam_clip/sam_clip.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 torch.use_deterministic_algorithms(False)
 
 import numpy as np
 import supervision as sv
 from autodistill.detection import CaptionOntology, DetectionBaseModel
 from segment_anything import SamAutomaticMaskGenerator
 
-from helpers import combine_detections, load_SAM
+from .helpers import combine_detections, load_SAM
 
 HOME = os.path.expanduser("~")
 DEVICE = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
 @dataclass
 class SAMCLIP(DetectionBaseModel):
@@ -38,134 +38,116 @@
             os.makedirs(f"{HOME}/.cache/autodistill/clip")
 
             os.system("pip install ftfy regex tqdm")
             os.system(
                 f"cd {HOME}/.cache/autodistill/clip && pip install git+https://github.com/openai/CLIP.git"
             )
 
-        # add clip path to path
+        # add clip path to user path
         sys.path.insert(0, f"{HOME}/.cache/autodistill/clip/CLIP")
 
         import clip
 
         model, preprocess = clip.load("ViT-B/32", device=DEVICE)
 
         self.clip_model = model
         self.clip_preprocess = preprocess
         self.tokenize = clip.tokenize
 
     def predict(self, input: str, confidence: int = 0.5) -> sv.Detections:
         image_bgr = cv2.imread(input)
         image_rgb = cv2.cvtColor(image_bgr, cv2.COLOR_BGR2RGB)
 
-        # SAM Predictions
         sam_result = self.sam_predictor.generate(image_rgb)
 
         valid_detections = []
 
         labels = self.ontology.prompts()
 
         nms_data = []
 
         if len(sam_result) == 0:
             return sv.Detections.empty()
 
+        if "background" not in [l.lower() for l in labels]:
+            labels.append("background")
+
         for mask in sam_result:
             mask_item = mask["segmentation"]
 
             image = image_rgb.copy()
 
-            # image[mask_item == 0] = 0
+            bbox = mask["bbox"]
+
+            xyxy = [bbox[0], bbox[1], bbox[0] + bbox[2], bbox[1] + bbox[3]]
 
-            # transform box from xywh to xyxy
-            mask["bbox"] = [
-                mask["bbox"][0],
-                mask["bbox"][1],
-                mask["bbox"][0] + mask["bbox"][2],
-                mask["bbox"][1] + mask["bbox"][3],
-            ]
-
-            # cut out bbox
-            image = image[
-                int(mask["bbox"][1]) : int(mask["bbox"][3]),
-                int(mask["bbox"][0]) : int(mask["bbox"][2]),
-            ]
+            # cut out mask from image using numpy indexing
+            image[mask_item == 0] = 0
 
             # fix ValueError: tile cannot extend outside image
             if image.shape[0] == 0 or image.shape[1] == 0:
                 continue
 
             # show me the bbox
             image = Image.fromarray(image)
 
             image = self.clip_preprocess(image).unsqueeze(0).to(DEVICE)
 
-            cosime_sims = []
-
             with torch.no_grad():
                 image_features = self.clip_model.encode_image(image)
 
                 image_features /= image_features.norm(dim=-1, keepdim=True)
 
-                for label in labels:
-                    text = self.tokenize([label]).to(DEVICE)
+                text = self.tokenize(labels)
 
-                    text_features = self.clip_model.encode_text(text)
+                text_features = self.clip_model.encode_text(text)
 
-                    text_features /= text_features.norm(dim=-1, keepdim=True)
-                    # get cosine similarity between image and text features
+                text_features /= text_features.norm(dim=-1, keepdim=True)
 
-                    cosine_sim = cosine_similarity(
-                        image_features.cpu().numpy(), text_features.cpu().numpy()
-                    )
+                similarity = (100.0 * image_features @ text_features.T).softmax(dim=-1)
 
-                    cosime_sims.append(cosine_sim[0][0])
+                if similarity.shape[0] == 0:
+                    continue
 
-            max_prob = None
-            max_idx = None
+                max_prob, max_idx = similarity[0].max(dim=0)
 
-            values, indices = torch.topk(torch.tensor(cosime_sims), 1)
+                if max_prob < confidence:
+                    continue
 
-            max_prob = values[0].item()
-            max_idx = indices[0].item()
+                if labels[max_idx] == "background":
+                    continue
 
-            if max_prob > confidence:
                 valid_detections.append(
                     sv.Detections(
-                        xyxy=np.array([mask["bbox"]]),
+                        xyxy=np.array([xyxy]),
                         confidence=np.array([max_prob]),
                         mask=np.array([mask_item]),
                         class_id=np.array([max_idx]),
                     )
                 )
+
                 # (x_min, y_min, x_max, y_max, score, class)
                 nms_data.append(
                     (
                         mask["bbox"][0],
                         mask["bbox"][1],
                         mask["bbox"][2],
                         mask["bbox"][3],
                         max_prob,
                         max_idx,
                     )
                 )
 
-                annotator = sv.BoxAnnotator()
-
-                annotated_image = annotator.annotate(
-                    scene=image_bgr,
-                    detections=sv.Detections(
-                        xyxy=np.array([mask["bbox"]]), class_id=np.array([1])
-                    ),
-                )
-
-                cv2.imshow("image", annotated_image)
+        nms = sv.non_max_suppression(np.array(nms_data), 0.5)
 
-                cv2.waitKey(0)
+        print(nms)
 
-        # nms = sv.non_max_suppression(np.array(nms_data), 0.5)
+        final_detections = []
+        ids = []
 
-        # valid_detections = [valid_detections[i] for i in nms if i == True]
+        # nms is list of bools
+        for idx, is_valid in enumerate(nms):
+            if is_valid:
+                final_detections.append(valid_detections[idx])
+                ids.append(valid_detections[idx].class_id[0])
 
-        return combine_detections(
-            valid_detections, overwrite_class_ids=len(valid_detections) * [1]
-        )
+        return combine_detections(final_detections, overwrite_class_ids=ids)
```

### Comparing `autodistill-sam-clip-0.1.1/setup.py` & `autodistill-sam-clip-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,12 +38,12 @@
     ],
     packages=find_packages(exclude=("tests",)),
     extras_require={
         "dev": ["flake8", "black==22.3.0", "isort", "twine", "pytest", "wheel"],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
+        "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
 )
```

