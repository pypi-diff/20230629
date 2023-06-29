# Comparing `tmp/spear-tts-pytorch-0.0.5.tar.gz` & `tmp/spear-tts-pytorch-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.5.tar", last modified: Thu Jun 29 20:17:08 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.6.tar", last modified: Thu Jun 29 20:59:23 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.5.tar` & `spear-tts-pytorch-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16834 2023-06-29 20:59:12.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:59:23.782541 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 20:59:23.000000 spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.5/LICENSE` & `spear-tts-pytorch-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.5/PKG-INFO` & `spear-tts-pytorch-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.5/README.md` & `spear-tts-pytorch-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.5/setup.py` & `spear-tts-pytorch-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.5',
+  version = '0.0.6',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
```

### Comparing `spear-tts-pytorch-0.0.5/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.6/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+from pathlib import Path
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn, einsum
 from torch.nn import Module, ModuleList
 
 from einops import rearrange, repeat, pack
 
@@ -398,14 +399,20 @@
             dim_head = dim_head,
             heads = heads,
             depth = source_depth,
             causal = True,
             cross_attend = True
         )
 
+    def load(self, path, strict = True):
+        path = Path(path)
+        assert path.exists()
+        pkg = torch.load(str(path), map_location = 'cpu')
+        self.load_state_dict(pkg, strict = strict)
+
     @property
     def device(self):
         return next(self.parameters()).device
 
     @torch.no_grad()
     @eval_decorator
     @beartype
```

### Comparing `spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.6/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

