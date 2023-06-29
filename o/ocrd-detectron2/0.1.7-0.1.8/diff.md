# Comparing `tmp/ocrd_detectron2-0.1.7.tar.gz` & `tmp/ocrd_detectron2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_detectron2-0.1.7.tar", last modified: Mon Mar 20 10:45:45 2023, max compression
+gzip compressed data, was "/home/xbert/unsortiert/arbeit/heyer/tools/ocrd_detectron2/dist/.tmp-y84t0869/ocrd_detectron2-0.1.8.tar", last modified: Thu Jun 29 12:58:17 2023, max compression
```

## Comparing `ocrd_detectron2-0.1.7.tar` & `ocrd_detectron2-0.1.8.tar`

### file list

```diff
@@ -1,31 +1,34 @@
-drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-03-20 10:45:45.676878 ocrd_detectron2-0.1.7/
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    17124 2023-03-20 10:45:45.676878 ocrd_detectron2-0.1.7/PKG-INFO
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    16783 2023-03-20 10:39:21.000000 ocrd_detectron2-0.1.7/README.md
-drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-03-20 10:45:45.676878 ocrd_detectron2-0.1.7/ocrd_detectron2/
--rw-rw-r--   0 xbert     (1000) xbert     (1000)        0 2022-01-19 08:49:47.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/__init__.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)      276 2022-01-19 08:49:28.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/cli.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2022-01-19 08:36:51.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/config.py
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    11547 2023-03-20 10:45:02.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/ocrd-tool.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      476 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_DocBank_X101.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      480 2022-12-02 22:54:42.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_DocBank_X101_page.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      289 2023-03-19 02:29:37.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_Jambo-sudo_X101.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      153 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_Math_R50.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      357 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_NewspaperNavigator_R50.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      286 2023-03-19 20:22:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PRImALayout_R50.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      273 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PubLayNet_R101.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      289 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PubLayNet_R101_JPLeoRX.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      271 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PubLayNet_R50.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      287 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PubLayNet_R50_JPLeoRX.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      285 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_PubLayNet_X101.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      137 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_TableBank_X152.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      154 2023-03-10 21:08:28.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/presets_TableBank_X152_Psarpei.json
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    36421 2023-03-19 18:20:09.000000 ocrd_detectron2-0.1.7/ocrd_detectron2/segment.py
-drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-03-20 10:45:45.676878 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    17124 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/PKG-INFO
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      988 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/SOURCES.txt
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      302 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/dependency_links.txt
--rw-rw-r--   0 xbert     (1000) xbert     (1000)       88 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/entry_points.txt
--rw-rw-r--   0 xbert     (1000) xbert     (1000)      153 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/requires.txt
--rw-rw-r--   0 xbert     (1000) xbert     (1000)       16 2023-03-20 10:45:45.000000 ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/top_level.txt
--rw-rw-r--   0 xbert     (1000) xbert     (1000)       38 2023-03-20 10:45:45.676878 ocrd_detectron2-0.1.7/setup.cfg
--rw-rw-r--   0 xbert     (1000) xbert     (1000)     1539 2022-01-20 16:51:36.000000 ocrd_detectron2-0.1.7/setup.py
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-29 12:58:17.536027 ocrd_detectron2-0.1.8/
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       66 2023-06-29 12:58:08.000000 ocrd_detectron2-0.1.8/MANIFEST.in
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    19014 2023-06-29 12:58:17.536027 ocrd_detectron2-0.1.8/PKG-INFO
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    18673 2023-06-24 12:19:11.000000 ocrd_detectron2-0.1.8/README.md
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    11462 2023-06-29 12:53:46.000000 ocrd_detectron2-0.1.8/ocrd-tool.json
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-29 12:58:17.532026 ocrd_detectron2-0.1.8/ocrd_detectron2/
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)        0 2022-01-19 08:49:47.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/__init__.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      276 2022-01-19 08:49:28.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/cli.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2022-01-19 08:36:51.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/config.py
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    11462 2023-06-29 12:53:46.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/ocrd-tool.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      476 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_DocBank_X101.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      480 2022-12-02 22:54:42.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_DocBank_X101_page.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      289 2023-03-19 02:29:37.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_Jambo-sudo_X101.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      153 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_Math_R50.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      357 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_NewspaperNavigator_R50.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      286 2023-03-19 20:22:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PRImALayout_R50.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      273 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PubLayNet_R101.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      289 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PubLayNet_R101_JPLeoRX.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      271 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PubLayNet_R50.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      287 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PubLayNet_R50_JPLeoRX.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      285 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_PubLayNet_X101.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      137 2022-10-28 11:55:34.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_TableBank_X152.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      154 2023-03-10 21:08:28.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/presets_TableBank_X152_Psarpei.json
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    36810 2023-06-29 12:50:56.000000 ocrd_detectron2-0.1.8/ocrd_detectron2/segment.py
+drwxrwxr-x   0 xbert     (1000) xbert     (1000)        0 2023-06-29 12:58:17.532026 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)    19014 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/PKG-INFO
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     1032 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/SOURCES.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      302 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/dependency_links.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       88 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/entry_points.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      171 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/requires.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       16 2023-06-29 12:58:17.000000 ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/top_level.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)      235 2023-06-27 22:32:44.000000 ocrd_detectron2-0.1.8/requirements.txt
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)       38 2023-06-29 12:58:17.536027 ocrd_detectron2-0.1.8/setup.cfg
+-rw-rw-r--   0 xbert     (1000) xbert     (1000)     1539 2022-01-20 16:51:36.000000 ocrd_detectron2-0.1.8/setup.py
```

### Comparing `ocrd_detectron2-0.1.7/PKG-INFO` & `ocrd_detectron2-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: ocrd_detectron2
-Version: 0.1.7
+Version: 0.1.8
 Summary: OCR-D wrapper for detectron2 based segmentation models
 Home-page: https://github.com/bertsky/ocrd_detectron2
 Author: Robert Sachunsky, Julian Balling
 Author-email: sachunsky@informatik.uni-leipzig.de, balling@infai.org
 License: MIT
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/ocrd-detectron2.svg)](https://badge.fury.io/py/ocrd-detectron2)
+[![Python test](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml)
+[![Docker Automated build via Github Container Registry](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml)
+[![Docker Automated build via Dockerhub](https://img.shields.io/docker/automated/bertsky/ocrd_detectron2.svg)](https://hub.docker.com/r/bertsky/ocrd_detectron2/tags/)
 
 # ocrd_detectron2
 
     OCR-D wrapper for detectron2 based segmentation models
 
   * [Introduction](#introduction)
   * [Installation](#installation)
@@ -21,14 +24,15 @@
   * [Models](#models)
      * [TableBank](#tablebank)
      * [PubLayNet](#publaynet)
      * [PubLayNet](#publaynet-1)
      * [LayoutParser](#layoutparser)
      * [DocBank](#docbank)
   * [Testing](#testing)
+     * [Test results](#test-results)
 
 ## Introduction
 
 This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for document layout analysis with models trained on [Detectron2](https://github.com/facebookresearch/detectron2), which implements [Faster R-CNN](https://arxiv.org/abs/1506.01497), [Mask R-CNN](https://arxiv.org/abs/1703.06870), [Cascade R-CNN](https://arxiv.org/abs/1712.00726), [Feature Pyramid Networks](https://arxiv.org/abs/1612.03144) and [Panoptic Segmentation](https://arxiv.org/abs/1801.00868), among others.
 
 In trying to cover a broad range of third-party models, a few sacrifices have to be made: Deployment of [models](#models) may be difficult, and needs configuration. Class labels (really [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) region types) must be provided. The code itself tries to cope with panoptic and instance segmentation models (with or without masks).
 
@@ -51,14 +55,21 @@
 
     make install
 
 Which is the equivalent of:
 
     pip install .
 
+**Alternatively**, you can use the provided **Docker image** (either from [Github Container Registry](https://github.com/users/bertsky/packages/container/package/ocrd_detectron2) or from [Dockerhub](https://hub.docker.com/r/bertsky/ocrd_detectron2)):
+
+    docker pull bertsky/ocrd_detectron2
+    # or
+    docker pull ghcr.io/bertsky/ocrd_detectron2
+
+
 ## Usage
 
 ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-detectron2-segment`
 
 To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
 
 ```
@@ -162,14 +173,28 @@
     # run it (setting model_config, model_weights and categories):
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -P categories '["TableRegion"]' -P model_config TableBank_X152.yaml -P model_weights TableBank_X152.pth -P min_confidence 0.1
     # run it (equivalent, with presets file)
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -p presets_TableBank_X152.json -P min_confidence 0.1 
     # download all preconfigured models
     ocrd resmgr download ocrd-detectron2-segment "*"
 
+For installation **via Docker**, usage is bascially the same as above – with some modifications:
+
+    # For data persistency, decide which host-side directories you want to mount in Docker:
+    DATADIR=/host-side/path/to/data
+    MODELDIR=/host-side/path/to/models
+    # Either you "log in" to a container first:
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources -it bertsky/ocrd_detectron2 bash
+    # and then can use the above commands verbatim
+    ...
+    # Or you spin up a new container each time,
+    # which means prefixing the above commands with
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources bertsky/ocrd_detectron2 ...
+
+
 #### Debugging
 
 If you mistrust your model, and/or this tool's additional postprocessing,
 try playing with the runtime parameters:
 
 - Set `debug_img` to some value other than `none`, e.g. `instance_colors_only`.
   This will generate an image which overlays the raw predictions with the raw image
@@ -308,7 +333,11 @@
 
 You can inspect the results under `test/assets/*/data` under various new `OCR-D-SEG-*` fileGrps.
 (Again, it is recommended to use [OCR-D Browser](https://github.com/hnesk/browse-ocrd).)
 
 Finally, to remove the test data, do:
 
     make clean
+
+### Test results
+
+These tests are integrated as a [Github Action](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml). Its results can be viewed [here](https://bertsky.github.io/ocrd_detectron2/test-results).
```

### Comparing `ocrd_detectron2-0.1.7/README.md` & `ocrd_detectron2-0.1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 [![PyPI version](https://badge.fury.io/py/ocrd-detectron2.svg)](https://badge.fury.io/py/ocrd-detectron2)
+[![Python test](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml)
+[![Docker Automated build via Github Container Registry](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml)
+[![Docker Automated build via Dockerhub](https://img.shields.io/docker/automated/bertsky/ocrd_detectron2.svg)](https://hub.docker.com/r/bertsky/ocrd_detectron2/tags/)
 
 # ocrd_detectron2
 
     OCR-D wrapper for detectron2 based segmentation models
 
   * [Introduction](#introduction)
   * [Installation](#installation)
@@ -11,14 +14,15 @@
   * [Models](#models)
      * [TableBank](#tablebank)
      * [PubLayNet](#publaynet)
      * [PubLayNet](#publaynet-1)
      * [LayoutParser](#layoutparser)
      * [DocBank](#docbank)
   * [Testing](#testing)
+     * [Test results](#test-results)
 
 ## Introduction
 
 This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for document layout analysis with models trained on [Detectron2](https://github.com/facebookresearch/detectron2), which implements [Faster R-CNN](https://arxiv.org/abs/1506.01497), [Mask R-CNN](https://arxiv.org/abs/1703.06870), [Cascade R-CNN](https://arxiv.org/abs/1712.00726), [Feature Pyramid Networks](https://arxiv.org/abs/1612.03144) and [Panoptic Segmentation](https://arxiv.org/abs/1801.00868), among others.
 
 In trying to cover a broad range of third-party models, a few sacrifices have to be made: Deployment of [models](#models) may be difficult, and needs configuration. Class labels (really [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) region types) must be provided. The code itself tries to cope with panoptic and instance segmentation models (with or without masks).
 
@@ -41,14 +45,21 @@
 
     make install
 
 Which is the equivalent of:
 
     pip install .
 
+**Alternatively**, you can use the provided **Docker image** (either from [Github Container Registry](https://github.com/users/bertsky/packages/container/package/ocrd_detectron2) or from [Dockerhub](https://hub.docker.com/r/bertsky/ocrd_detectron2)):
+
+    docker pull bertsky/ocrd_detectron2
+    # or
+    docker pull ghcr.io/bertsky/ocrd_detectron2
+
+
 ## Usage
 
 ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-detectron2-segment`
 
 To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
 
 ```
@@ -152,14 +163,28 @@
     # run it (setting model_config, model_weights and categories):
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -P categories '["TableRegion"]' -P model_config TableBank_X152.yaml -P model_weights TableBank_X152.pth -P min_confidence 0.1
     # run it (equivalent, with presets file)
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -p presets_TableBank_X152.json -P min_confidence 0.1 
     # download all preconfigured models
     ocrd resmgr download ocrd-detectron2-segment "*"
 
+For installation **via Docker**, usage is bascially the same as above – with some modifications:
+
+    # For data persistency, decide which host-side directories you want to mount in Docker:
+    DATADIR=/host-side/path/to/data
+    MODELDIR=/host-side/path/to/models
+    # Either you "log in" to a container first:
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources -it bertsky/ocrd_detectron2 bash
+    # and then can use the above commands verbatim
+    ...
+    # Or you spin up a new container each time,
+    # which means prefixing the above commands with
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources bertsky/ocrd_detectron2 ...
+
+
 #### Debugging
 
 If you mistrust your model, and/or this tool's additional postprocessing,
 try playing with the runtime parameters:
 
 - Set `debug_img` to some value other than `none`, e.g. `instance_colors_only`.
   This will generate an image which overlays the raw predictions with the raw image
@@ -298,7 +323,11 @@
 
 You can inspect the results under `test/assets/*/data` under various new `OCR-D-SEG-*` fileGrps.
 (Again, it is recommended to use [OCR-D Browser](https://github.com/hnesk/browse-ocrd).)
 
 Finally, to remove the test data, do:
 
     make clean
+
+### Test results
+
+These tests are integrated as a [Github Action](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml). Its results can be viewed [here](https://bertsky.github.io/ocrd_detectron2/test-results).
```

### Comparing `ocrd_detectron2-0.1.7/ocrd_detectron2/ocrd-tool.json` & `ocrd_detectron2-0.1.8/ocrd-tool.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.832275390625%*

 * *Differences: {"'tools'": "{'ocrd-detectron2-segment': {'resources': {0: {'url': "*

 * *            "'https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152.yaml'}, "*

 * *            "1: {'url': "*

 * *            "'https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152.pth'}, "*

 * *            "2: {'url': "*

 * *            "'https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152_Psarpei.yaml'}, "*

 * *            "3: {'url': "*

 * *            "'https://github.com/bert […]*

```diff
@@ -77,165 +77,155 @@
                 }
             },
             "resources": [
                 {
                     "description": "TableBank via LayoutLM X152-FPN config",
                     "name": "TableBank_X152.yaml",
                     "size": 536,
-                    "url": "https://layoutlm.blob.core.windows.net/tablebank/model_zoo/detection/All_X152/All_X152.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152.yaml"
                 },
                 {
                     "description": "TableBank via LayoutLM X152-FPN weights",
                     "name": "TableBank_X152.pth",
                     "size": 1103832675,
-                    "url": "https://layoutlm.blob.core.windows.net/tablebank/model_zoo/detection/All_X152/model_final.pth"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152.pth"
                 },
                 {
                     "description": "TableBank via Psarpei X152-FPN config",
                     "name": "TableBank_X152_Psarpei.yaml",
                     "size": 534,
-                    "url": "https://drive.google.com/uc?id=1WBk6kHHyvyEzoPBsRr2BvFY51zURjd4R"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152_Psarpei.yaml"
                 },
                 {
                     "description": "TableBank via Psarpei X152-FPN weights",
                     "name": "TableBank_X152_Psarpei.pth",
                     "size": 1103832675,
-                    "url": "https://drive.google.com/uc?id=11FgFTy0MyVUMGd00T_InEDaarB4qAlP8"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/TableBank_X152_Psarpei.pth"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 R50-FPN config",
                     "name": "PubLayNet_R_50_FPN_3x.yaml",
                     "size": 388,
-                    "url": "https://github.com/hpanwar08/detectron2/raw/master/configs/DLA_mask_rcnn_R_50_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_50_FPN_3x.yaml"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 R50-FPN weights",
                     "name": "PubLayNet_R_50_FPN_3x.pth",
-                    "path_in_archive": "model_final_trimmed.pth",
-                    "size": 176249992,
-                    "type": "archive",
-                    "url": "https://www.dropbox.com/sh/44ez171b2qaocd2/AAB0huidzzOXeo99QdplZRjua"
+                    "size": 176249718,
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_50_FPN_3x.pth"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 R101-FPN config",
                     "name": "PubLayNet_R_101_FPN_3x.yaml",
                     "size": 392,
-                    "url": "https://github.com/hpanwar08/detectron2/raw/master/configs/DLA_mask_rcnn_R_101_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_101_FPN_3x.yaml"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 R101-FPN weights",
                     "name": "PubLayNet_R_101_FPN_3x.pth",
-                    "path_in_archive": "model_final.pth",
-                    "size": 254055290,
-                    "type": "archive",
-                    "url": "https://www.dropbox.com/sh/wgt9skz67usliei/AAD9n6qbsyMz1Y3CwpZpHXCpa"
+                    "size": 503147199,
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_101_FPN_3x.pth"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 X101-FPN config",
                     "name": "PubLayNet_X_101_32x8d_FPN_3x.yaml",
                     "size": 592,
-                    "url": "https://github.com/hpanwar08/detectron2/raw/master/configs/DLA_mask_rcnn_X_101_32x8d_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_X_101_32x8d_FPN_3x.yaml"
                 },
                 {
                     "description": "PubLayNet via hpanwar08 X101-FPN weights",
                     "name": "PubLayNet_X_101_32x8d_FPN_3x.pth",
-                    "path_in_archive": "model_final_trimmed.pth",
-                    "size": 431414189,
-                    "type": "archive",
-                    "url": "https://www.dropbox.com/sh/1098ym6vhad4zi6/AABe16eSdY_34KGp52W0ruwha"
+                    "size": 429840864,
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_X_101_32x8d_FPN_3x.pth"
                 },
                 {
                     "description": "PubLayNet via JPLeoRX R50-FPN config",
                     "name": "PubLayNet_R_50_FPN_3x_JPLeoRX.yaml",
                     "size": 388,
-                    "url": "https://github.com/hpanwar08/detectron2/raw/master/configs/DLA_mask_rcnn_R_50_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_50_FPN_3x_JPLeoRX.yaml"
                 },
                 {
                     "description": "PubLayNet via JPLeoRX R50-FPN weights",
                     "name": "PubLayNet_R_50_FPN_3x_JPLeoRX.pth",
                     "size": 176299422,
-                    "url": "https://drive.google.com/file/d/1IbxaRd82hIrxPT4a1U61_g2vvE3zcRLO/view?usp=sharing"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_50_FPN_3x_JPLeoRX.pth"
                 },
                 {
                     "description": "PubLayNet via JPLeoRX R101-FPN config",
                     "name": "PubLayNet_R_101_FPN_3x_JPLeoRX.yaml",
                     "size": 392,
-                    "url": "https://github.com/hpanwar08/detectron2/raw/master/configs/DLA_mask_rcnn_R_101_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_101_FPN_3x_JPLeoRX.yaml"
                 },
                 {
                     "description": "PubLayNet via JPLeoRX R101-FPN weights",
                     "name": "PubLayNet_R_101_FPN_3x_JPLeoRX.pth",
                     "size": 252572745,
-                    "url": "https://drive.google.com/file/d/17MD-FegQtFRNn4GeHqKCLaQZ6FiFrzLg/view?usp=sharing"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PubLayNet_R_101_FPN_3x_JPLeoRX.pth"
                 },
                 {
                     "description": "Modern Magazines via Jambo-sudo X101-FPN (pre-trained on PubLayNet, fine-tuned on 500 p. 20th cent. magazines) config",
                     "name": "Jambo-sudo_X101.yaml",
                     "size": 592,
-                    "url": "https://github.com/Jambo-sudo/Historical-document-layout-analysis/raw/main/historical-document-analysis/DLA_mask_rcnn_X_101_32x8d_FPN_3x.yaml"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/Jambo-sudo_X101.yaml"
                 },
                 {
                     "description": "Modern Magazines via Jambo-sudo X101-FPN (pre-trained on PubLayNet, fine-tuned on 500 p. 20th cent. magazines) weights",
                     "name": "Jambo-sudo_X101.pth",
                     "size": 856430002,
-                    "url": "https://www.dropbox.com/s/hfhsdpvg7jesd4g/pub_model_final.pth?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/Jambo-sudo_X101.pth"
                 },
                 {
                     "description": "PRImALayout via LayoutLM R50-FPN config",
                     "name": "PRImALayout_R50.yaml",
                     "size": 934,
-                    "url": "https://www.dropbox.com/s/yc92x97k50abynt/config.yaml?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PRImALayout_R50.yaml"
                 },
                 {
                     "description": "PRImALayout via LayoutLM R50-FPN weights",
                     "name": "PRImALayout_R50.pth",
                     "size": 351229486,
-                    "url": "https://www.dropbox.com/s/h7th27jfv19rxiy/model_final.pth?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/PRImALayout_R50.pth"
                 },
                 {
                     "description": "DocBank via LayoutLM X101-FPN config",
                     "name": "DocBank_X101.yaml",
-                    "path_in_archive": "X101/X101.yaml",
-                    "size": 783884362,
-                    "type": "archive",
-                    "url": "https://layoutlm.blob.core.windows.net/docbank/model_zoo/X101.zip"
+                    "size": 523,
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/DocBank_X101.yaml"
                 },
                 {
                     "description": "DocBank via LayoutLM X101-FPN config",
                     "name": "DocBank_X101.pth",
-                    "path_in_archive": "X101/model.pth",
-                    "size": 783884362,
-                    "type": "archive",
-                    "url": "https://layoutlm.blob.core.windows.net/docbank/model_zoo/X101.zip"
+                    "size": 835606605,
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/DocBank_X101.pth"
                 },
                 {
                     "description": "NewspaperNavigator via LayoutParser R50-PanopticFPN config",
                     "name": "NewspaperNavigator_R_50_PFPN_3x.yaml",
                     "size": 330226761,
-                    "url": "https://www.dropbox.com/s/wnido8pk4oubyzr/config.yml?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/NewspaperNavigator_R_50_PFPN_3x.yaml"
                 },
                 {
                     "description": "NewspaperNavigator via LayoutParser R50-PanopticFPN weights",
                     "name": "NewspaperNavigator_R_50_PFPN_3x.pth",
                     "size": 330226761,
-                    "url": "https://www.dropbox.com/s/6ewh6g8rqt2ev3a/model_final.pth?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/NewspaperNavigator_R_50_PFPN_3x.pth"
                 },
                 {
                     "description": "MathFormulaDetection via LayoutParser R50-FPN config",
                     "name": "Math_R_50_FPN_3x.yaml",
                     "size": 5632,
-                    "url": "https://www.dropbox.com/s/ld9izb95f19369w/config.yaml?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/Math_R_50_FPN_3x.yaml"
                 },
                 {
                     "description": "MathFormulaDetection via LayoutParser R50-FPN weights",
                     "name": "Math_R_50_FPN_3x.pth",
                     "size": 330084629,
-                    "url": "https://www.dropbox.com/s/7xel0i3iqpm2p8y/model_final.pth?dl=1"
+                    "url": "https://github.com/bertsky/ocrd_detectron2/releases/download/v0.1.7/Math_R_50_FPN_3x.pth"
                 }
             ],
             "steps": [
                 "layout/segmentation/region"
             ]
         }
     },
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `ocrd_detectron2-0.1.7/ocrd_detectron2/segment.py` & `ocrd_detectron2-0.1.8/ocrd_detectron2/segment.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,18 +115,22 @@
             shutil.copyfile(model_config, temp_config)
             with pushd_popd(tmpdir):
                 # repair broken config files that make deviating assumptions on model_zoo files
                 with fileinput.input(temp_config, inplace=True) as temp_config_file:
                     for line in temp_config_file:
                         if fileinput.isfirstline():
                             PREFIXES = ['/content/',
+                                        '../../configs/',
                                         '../configs/',
                                         '../']
                             line = next((line.replace(pref, '') for pref in PREFIXES
                                          if line.startswith('_BASE_: "' + pref)), line)
+                        if os.path.basename(model_config) == 'Jambo-sudo_X101.yaml' and 'NUM_CLASSES: 5' in line:
+                            # workaround for Jambo-sudo/Historical-document-layout-analysis#1
+                            line = line.replace('NUM_CLASSES: 5', 'NUM_CLASSES: 6')
                         print(line, end='')
                 cfg = get_cfg()
                 cfg.merge_from_file(temp_config)
         model_weights = self.resolve_resource(self.parameter['model_weights'])
         cfg.merge_from_list([
             # set threshold for this model
             "MODEL.ROI_HEADS.SCORE_THRESH_TEST", self.parameter['min_confidence'],
@@ -193,14 +197,15 @@
 
         # pylint: disable=attribute-defined-outside-init
         for n, input_file in enumerate(self.input_files):
             file_id = make_file_id(input_file, self.output_file_grp)
             page_id = input_file.pageId or input_file.ID
             LOG.info("INPUT FILE %i / %s", n, page_id)
             pcgts = page_from_file(self.workspace.download_file(input_file))
+            pcgts.set_pcGtsId(file_id)
             self.add_metadata(pcgts)
 
             page = pcgts.get_Page()
             page_image_raw, page_coords, page_image_info = self.workspace.image_from_page(
                 page, page_id, feature_filter='binarized')
             # for morphological post-processing, we will need the binarized image, too
             if self.parameter['postprocessing'] != 'none':
```

### Comparing `ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/PKG-INFO` & `ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: ocrd-detectron2
-Version: 0.1.7
+Version: 0.1.8
 Summary: OCR-D wrapper for detectron2 based segmentation models
 Home-page: https://github.com/bertsky/ocrd_detectron2
 Author: Robert Sachunsky, Julian Balling
 Author-email: sachunsky@informatik.uni-leipzig.de, balling@infai.org
 License: MIT
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/ocrd-detectron2.svg)](https://badge.fury.io/py/ocrd-detectron2)
+[![Python test](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml)
+[![Docker Automated build via Github Container Registry](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml/badge.svg)](https://github.com/bertsky/ocrd_detectron2/actions/workflows/docker-image.yml)
+[![Docker Automated build via Dockerhub](https://img.shields.io/docker/automated/bertsky/ocrd_detectron2.svg)](https://hub.docker.com/r/bertsky/ocrd_detectron2/tags/)
 
 # ocrd_detectron2
 
     OCR-D wrapper for detectron2 based segmentation models
 
   * [Introduction](#introduction)
   * [Installation](#installation)
@@ -21,14 +24,15 @@
   * [Models](#models)
      * [TableBank](#tablebank)
      * [PubLayNet](#publaynet)
      * [PubLayNet](#publaynet-1)
      * [LayoutParser](#layoutparser)
      * [DocBank](#docbank)
   * [Testing](#testing)
+     * [Test results](#test-results)
 
 ## Introduction
 
 This offers [OCR-D](https://ocr-d.de) compliant [workspace processors](https://ocr-d.de/en/spec/cli) for document layout analysis with models trained on [Detectron2](https://github.com/facebookresearch/detectron2), which implements [Faster R-CNN](https://arxiv.org/abs/1506.01497), [Mask R-CNN](https://arxiv.org/abs/1703.06870), [Cascade R-CNN](https://arxiv.org/abs/1712.00726), [Feature Pyramid Networks](https://arxiv.org/abs/1612.03144) and [Panoptic Segmentation](https://arxiv.org/abs/1801.00868), among others.
 
 In trying to cover a broad range of third-party models, a few sacrifices have to be made: Deployment of [models](#models) may be difficult, and needs configuration. Class labels (really [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) region types) must be provided. The code itself tries to cope with panoptic and instance segmentation models (with or without masks).
 
@@ -51,14 +55,21 @@
 
     make install
 
 Which is the equivalent of:
 
     pip install .
 
+**Alternatively**, you can use the provided **Docker image** (either from [Github Container Registry](https://github.com/users/bertsky/packages/container/package/ocrd_detectron2) or from [Dockerhub](https://hub.docker.com/r/bertsky/ocrd_detectron2)):
+
+    docker pull bertsky/ocrd_detectron2
+    # or
+    docker pull ghcr.io/bertsky/ocrd_detectron2
+
+
 ## Usage
 
 ### [OCR-D processor](https://ocr-d.de/en/spec/cli) interface `ocrd-detectron2-segment`
 
 To be used with [PAGE-XML](https://github.com/PRImA-Research-Lab/PAGE-XML) documents in an [OCR-D](https://ocr-d.de/en/about) annotation workflow.
 
 ```
@@ -162,14 +173,28 @@
     # run it (setting model_config, model_weights and categories):
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -P categories '["TableRegion"]' -P model_config TableBank_X152.yaml -P model_weights TableBank_X152.pth -P min_confidence 0.1
     # run it (equivalent, with presets file)
     ocrd-detectron2-segment -I OCR-D-BIN -O OCR-D-SEG-TAB -p presets_TableBank_X152.json -P min_confidence 0.1 
     # download all preconfigured models
     ocrd resmgr download ocrd-detectron2-segment "*"
 
+For installation **via Docker**, usage is bascially the same as above – with some modifications:
+
+    # For data persistency, decide which host-side directories you want to mount in Docker:
+    DATADIR=/host-side/path/to/data
+    MODELDIR=/host-side/path/to/models
+    # Either you "log in" to a container first:
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources -it bertsky/ocrd_detectron2 bash
+    # and then can use the above commands verbatim
+    ...
+    # Or you spin up a new container each time,
+    # which means prefixing the above commands with
+    docker run -v $DATADIR:/data -v $MODELDIR:/usr/local/share/ocrd-resources bertsky/ocrd_detectron2 ...
+
+
 #### Debugging
 
 If you mistrust your model, and/or this tool's additional postprocessing,
 try playing with the runtime parameters:
 
 - Set `debug_img` to some value other than `none`, e.g. `instance_colors_only`.
   This will generate an image which overlays the raw predictions with the raw image
@@ -308,7 +333,11 @@
 
 You can inspect the results under `test/assets/*/data` under various new `OCR-D-SEG-*` fileGrps.
 (Again, it is recommended to use [OCR-D Browser](https://github.com/hnesk/browse-ocrd).)
 
 Finally, to remove the test data, do:
 
     make clean
+
+### Test results
+
+These tests are integrated as a [Github Action](https://github.com/bertsky/ocrd_detectron2/actions/workflows/python-app.yml). Its results can be viewed [here](https://bertsky.github.io/ocrd_detectron2/test-results).
```

### Comparing `ocrd_detectron2-0.1.7/ocrd_detectron2.egg-info/SOURCES.txt` & `ocrd_detectron2-0.1.8/ocrd_detectron2.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+MANIFEST.in
 README.md
+ocrd-tool.json
+requirements.txt
 setup.py
 ocrd_detectron2/__init__.py
 ocrd_detectron2/cli.py
 ocrd_detectron2/config.py
 ocrd_detectron2/ocrd-tool.json
 ocrd_detectron2/presets_DocBank_X101.json
 ocrd_detectron2/presets_DocBank_X101_page.json
```

### Comparing `ocrd_detectron2-0.1.7/setup.py` & `ocrd_detectron2-0.1.8/setup.py`

 * *Files identical despite different names*

