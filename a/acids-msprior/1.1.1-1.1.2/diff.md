# Comparing `tmp/acids-msprior-1.1.1.tar.gz` & `tmp/acids-msprior-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acids-msprior-1.1.1.tar", last modified: Wed Jun  7 12:55:12 2023, max compression
+gzip compressed data, was "acids-msprior-1.1.2.tar", last modified: Thu Jun 29 14:56:01 2023, max compression
```

## Comparing `acids-msprior-1.1.1.tar` & `acids-msprior-1.1.2.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.879970 acids-msprior-1.1.1/acids_msprior.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 12:55:12.000000 acids-msprior-1.1.1/acids_msprior.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.879970 acids-msprior-1.1.1/msprior/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20823 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/decoder_only.gin
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/encoder_decoder.gin
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/encoder_decoder_continuous.gin
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/flattened.gin
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/recurrent.gin
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/rwkv.gin
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/configs/rwkv_semantic.gin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/cuda/wkv_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/cuda/wkv_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (123)    11112 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/scripted.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.883970 acids-msprior-1.1.1/msprior_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/compact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/export.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/main_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/msprior_scripts/train.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:55:12.887970 acids-msprior-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-07 12:51:51.000000 acids-msprior-1.1.1/tests/test_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.692353 acids-msprior-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-29 14:56:01.692353 acids-msprior-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.684353 acids-msprior-1.1.2/acids_msprior.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-29 14:56:01.000000 acids-msprior-1.1.2/acids_msprior.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.684353 acids-msprior-1.1.2/msprior/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22737 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.688353 acids-msprior-1.1.2/msprior/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/decoder_only.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/flattened.gin
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/modulated_alibi.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/recurrent.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/rwkv.gin
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/configs/rwkv_semantic.gin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.688353 acids-msprior-1.1.2/msprior/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/cuda/wkv_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/cuda/wkv_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12734 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/scripted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.688353 acids-msprior-1.1.2/msprior_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/compact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/main_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6808 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/msprior_scripts/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:56:01.692353 acids-msprior-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:56:01.688353 acids-msprior-1.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-29 14:53:08.000000 acids-msprior-1.1.2/tests/test_configs.py
```

### Comparing `acids-msprior-1.1.1/PKG-INFO` & `acids-msprior-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.1.1
+Version: 1.1.2
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.1 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.2 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.1.1/README.md` & `acids-msprior-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/acids_msprior.egg-info/PKG-INFO` & `acids-msprior-1.1.2/acids_msprior.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acids-msprior
-Version: 1.1.1
+Version: 1.1.2
 Summary: MSPRIOR: A multiscale prior model for realtime temporal learning
 Author: Antoine CAILLON
 Author-email: caillon@ircam.fr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.1 Summary: MSPRIOR: A
+Metadata-Version: 2.1 Name: acids-msprior Version: 1.1.2 Summary: MSPRIOR: A
 multiscale prior model for realtime temporal learning Author: Antoine CAILLON
 Author-email: caillon@ircam.fr Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
 markdown # MSPrior ### A multi(scale/stream) prior model for realtime temporal
 learning ## Disclaimer This is an experimental project that *will* be subject
 to lots of changes. ## Installation ```bash pip install acids-msprior ``` ##
```

### Comparing `acids-msprior-1.1.1/acids_msprior.egg-info/SOURCES.txt` & `acids-msprior-1.1.2/acids_msprior.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -13,17 +13,16 @@
 msprior/dataset.py
 msprior/preprocessor.py
 msprior/rwkv.py
 msprior/scripted.py
 msprior/task.py
 msprior/utils.py
 msprior/configs/decoder_only.gin
-msprior/configs/encoder_decoder.gin
-msprior/configs/encoder_decoder_continuous.gin
 msprior/configs/flattened.gin
+msprior/configs/modulated_alibi.gin
 msprior/configs/recurrent.gin
 msprior/configs/rwkv.gin
 msprior/configs/rwkv_semantic.gin
 msprior/cuda/wkv_cuda.cu
 msprior/cuda/wkv_op.cpp
 msprior_scripts/__init__.py
 msprior_scripts/combine.py
```

### Comparing `acids-msprior-1.1.1/msprior/attention.py` & `acids-msprior-1.1.2/msprior/attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import cached_conv as cc
 import gin
 import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 
 import msprior
-from msprior import utils
+from msprior import rwkv, utils
 
 TensorDict = Dict[str, torch.Tensor]
 
 
 class MultiHeadAlibiAttention(nn.Module):
 
     def __init__(self,
@@ -278,14 +278,72 @@
         x = self.feed_forward_dropout(x)
         x = x + x_res
         x = self.feed_forward_norm(x)
 
         return x
 
 
+class ModulatedTransformerLayer(nn.Module):
+
+    def __init__(self, attention_factory: Callable[[],
+                                                   MultiHeadAlibiAttention],
+                 feed_forward_factory: Callable[[], FeedForward],
+                 dropout_rate: float, model_dim: int, head_dim: int,
+                 num_heads: int, film: Callable[[], rwkv.Film]) -> None:
+        super().__init__()
+
+        self.attention_norm = nn.LayerNorm(model_dim)
+        self.q_linear = nn.Linear(model_dim, head_dim * num_heads)
+        self.kv_linear = nn.Linear(model_dim, 2 * head_dim * num_heads)
+        self.attention = attention_factory()
+        self.post_attention_linear = nn.Linear(head_dim * num_heads, model_dim)
+        self.attention_dropout = nn.Dropout(dropout_rate)
+
+        self.feed_forward_norm = nn.LayerNorm(model_dim)
+        self.feed_forward = feed_forward_factory()
+        self.feed_forward_dropout = nn.Dropout(dropout_rate)
+
+        self.film_norm = nn.LayerNorm(model_dim)
+        self.film = film()
+        self.film_dropout = nn.Dropout(dropout_rate)
+
+    def forward(self,
+                x: torch.Tensor,
+                y: Optional[torch.Tensor] = None) -> torch.Tensor:
+
+        assert y is not None
+
+        # SELF ATTENTION
+        x_res = x.clone()
+        x = self.attention_norm(x)
+        q = self.q_linear(x)
+        k, v = self.kv_linear(x).chunk(2, -1)
+        x = self.attention(q, k, v)
+        x = self.post_attention_linear(x)
+        x = self.attention_dropout(x)
+        x = x + x_res
+
+        # FEED FORWARD
+        x_res = x.clone()
+        x = self.feed_forward_norm(x)
+        x = self.feed_forward(x)
+        x = self.feed_forward_dropout(x)
+        x = x + x_res
+
+        # MODULATION
+
+        x_res = x.clone()
+        x = self.film_norm(x)
+        x = self.film(x, y)
+        x = self.film_dropout(x)
+        x = x + x_res
+
+        return x
+
+
 class MultivariateEmbedding(nn.Module):
 
     def __init__(self,
                  num_tokens: int,
                  num_features: int,
                  num_quantizers: int,
                  from_pretrained: Optional[str] = None) -> None:
```

### Comparing `acids-msprior-1.1.1/msprior/configs/decoder_only.gin` & `acids-msprior-1.1.2/msprior/configs/decoder_only.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/configs/flattened.gin` & `acids-msprior-1.1.2/msprior/configs/flattened.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/configs/rwkv.gin` & `acids-msprior-1.1.2/msprior/configs/rwkv.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/configs/rwkv_semantic.gin` & `acids-msprior-1.1.2/msprior/configs/rwkv_semantic.gin`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/cuda/wkv_cuda.cu` & `acids-msprior-1.1.2/msprior/cuda/wkv_cuda.cu`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/cuda/wkv_op.cpp` & `acids-msprior-1.1.2/msprior/cuda/wkv_op.cpp`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/dataset.py` & `acids-msprior-1.1.2/msprior/dataset.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/preprocessor.py` & `acids-msprior-1.1.2/msprior/preprocessor.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/rwkv.py` & `acids-msprior-1.1.2/msprior/rwkv.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/scripted.py` & `acids-msprior-1.1.2/msprior/scripted.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     def __init__(
         self,
         run: Optional[str] = None,
         temporal_ratio: int = 1024,
         from_continuous: bool = False,
         vae_path: Optional[str] = None,
         initial_listen: bool = True,
+        ema_weights: bool = False,
     ) -> None:
         super().__init__()
         print("streaming mode is set to", cc.USE_BUFFER_CONV)
 
         if run is not None:
             config = os.path.join(run, "config.gin")
 
@@ -36,15 +37,19 @@
         model = Prior()
 
         if run is not None:
             ckpts = pathlib.Path(run).rglob("*.ckpt")
             ckpts = map(str, ckpts)
             ckpts = sorted(ckpts, key=lambda x: "last" in x, reverse=True)
             ckpt = next(iter(ckpts))
-            ckpt = torch.load(ckpt, map_location="cpu")["state_dict"]
+            ckpt = torch.load(ckpt, map_location="cpu")
+            if ema_weights and "EMA" in ckpt["callbacks"]:
+                ckpt = ckpt["callbacks"]["EMA"],
+            else:
+                ckpt = ckpt["state_dict"]
             if isinstance(model.decoder.net[0], RWKV):
                 for k, v in ckpt.items():
                     if ".time" in k:
                         ckpt[k] = v.reshape(-1)
             model.load_state_dict(ckpt, strict=False)
 
         model.eval()
```

### Comparing `acids-msprior-1.1.1/msprior/task.py` & `acids-msprior-1.1.2/msprior/task.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior/utils.py` & `acids-msprior-1.1.2/msprior/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pathlib
 import subprocess
 from itertools import repeat
 from typing import Any, Callable, Dict, Iterable, Optional, Sequence, Tuple
 
 import gin
 import numpy as np
+import pytorch_lightning as pl
 import torch
 import torch.nn as nn
 
 # GIN UTILS
 
 TensorDict = Dict[str, torch.Tensor]
 
@@ -274,7 +275,49 @@
         )
 
         inputs["encoder_inputs"] = reconstruction
 
         return inputs
 
     return vae_processing
+
+
+class EMA(pl.Callback):
+
+    def __init__(self, factor=.999) -> None:
+        super().__init__()
+        self.weights = {}
+        self.factor = factor
+
+    def on_train_batch_end(self, trainer, pl_module, outputs, batch,
+                           batch_idx) -> None:
+        for n, p in pl_module.named_parameters():
+            if n not in self.weights:
+                self.weights[n] = p.data.clone()
+                continue
+
+            self.weights[n] = self.weights[n] * self.factor + p.data * (
+                1 - self.factor)
+
+    def swap_weights(self, module):
+        for n, p in module.named_parameters():
+            current = p.data.clone()
+            p.data.copy_(self.weights[n])
+            self.weights[n] = current
+
+    def on_validation_epoch_start(self, trainer, pl_module) -> None:
+        if self.weights:
+            self.swap_weights(pl_module)
+        else:
+            print("no ema weights available")
+
+    def on_validation_epoch_end(self, trainer, pl_module) -> None:
+        if self.weights:
+            self.swap_weights(pl_module)
+        else:
+            print("no ema weights available")
+
+    def state_dict(self) -> Dict[str, Any]:
+        return self.weights.copy()
+
+    def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
+        self.weights.update(state_dict)
```

### Comparing `acids-msprior-1.1.1/msprior_scripts/combine.py` & `acids-msprior-1.1.2/msprior_scripts/combine.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior_scripts/compact.py` & `acids-msprior-1.1.2/msprior_scripts/compact.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior_scripts/export.py` & `acids-msprior-1.1.2/msprior_scripts/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,31 @@
     cc.use_cached_conv(True)
 
     model = ScriptedPrior(
         run=FLAGS.run,
         temporal_ratio=FLAGS.temporal_ratio,
         from_continuous=FLAGS.continuous,
         vae_path=FLAGS.vae_path,
+        ema_weights=FLAGS.ema_weights,
     )
     model.apply_full_reset()
     model_name = os.path.basename(os.path.normpath(FLAGS.run)) + '.ts'
     export_path = os.path.join(FLAGS.run, model_name)
     model.export_to_ts(export_path)
     print(f'model exported to {export_path}')
 
 
 FLAGS = flags.FLAGS
 flags.DEFINE_string('run', default=None, required=True, help='Run to export')
 flags.DEFINE_string('vae_path', default=None, help='Pretrained semantic VAE')
 flags.DEFINE_integer('batch_size', default=1, help='Maximum batch size')
+flags.DEFINE_bool('ema_weights',
+                  default=False,
+                  help='Use ema weights if available')
+
 flags.DEFINE_integer(
     'temporal_ratio',
     default=1024,
     help='Sequence temporal ratio',
 )
 flags.DEFINE_bool(
     'continuous',
```

### Comparing `acids-msprior-1.1.1/msprior_scripts/main_cli.py` & `acids-msprior-1.1.2/msprior_scripts/main_cli.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior_scripts/preprocess.py` & `acids-msprior-1.1.2/msprior_scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/msprior_scripts/train.py` & `acids-msprior-1.1.2/msprior_scripts/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import os
 
 import gin
 import pytorch_lightning as pl
 import torch
 from absl import app, flags
-from pytorch_lightning import callbacks
 from torch.utils import data
 
+import msprior.utils
 from msprior.attention import Prior
 from msprior.dataset import SequenceDataset
 
 FLAGS = flags.FLAGS
 flags.DEFINE_multi_string("config",
                           default="decoder_only",
                           help="config to parse.")
@@ -33,14 +33,17 @@
                     help="use pretrained embeddings from rave.")
 flags.DEFINE_multi_string("override",
                           default=[],
                           help="additional gin bindings.")
 flags.DEFINE_string("ckpt",
                     default=None,
                     help="checkpoint to resume training from.")
+flags.DEFINE_float('ema',
+                   default=None,
+                   help='Exponential weight averaging factor (optional)')
 flags.DEFINE_integer("val_every",
                      default=1000,
                      help="validate training every n step.")
 
 
 def add_ext(config: str):
     if config[-4:] != ".gin":
@@ -59,14 +62,20 @@
     gin.parse_config_files_and_bindings(
         configs,
         overrides,
     )
 
     logging.info("loading dataset")
     dataset = SequenceDataset(db_path=FLAGS.db_path)
+
+    if FLAGS.val_size > len(dataset):
+        logging.warn(
+            r"Dataset too small, using 5% of the train set as the val set")
+        FLAGS.val_size = len(dataset) // 20
+
     train, val = data.random_split(
         dataset,
         (len(dataset) - FLAGS.val_size, FLAGS.val_size),
         generator=torch.Generator().manual_seed(42),
     )
     if not any(map(lambda x: "flattened" in x, FLAGS.config)):
         logging.info("quantizer number retrieval")
@@ -100,29 +109,34 @@
     val_check = {}
     if len(train_loader) >= FLAGS.val_every:
         val_check["val_check_interval"] = FLAGS.val_every
     else:
         nepoch = FLAGS.val_every // len(train_loader)
         val_check["check_val_every_n_epoch"] = nepoch
 
+    callbacks = [
+        pl.callbacks.LearningRateMonitor(logging_interval='step'),
+        pl.callbacks.ModelCheckpoint(monitor="val_cross_entropy",
+                                     filename='best'),
+        pl.callbacks.ModelCheckpoint(filename='last'),
+        pl.callbacks.EarlyStopping(
+            "val_cross_entropy",
+            patience=20,
+        )
+    ]
+
+    if FLAGS.ema is not None:
+        callbacks.append(msprior.utils.EMA(FLAGS.ema))
+
     logging.info("creating trainer")
     trainer = pl.Trainer(
         logger=pl.loggers.TensorBoardLogger('runs', name=FLAGS.name),
         accelerator='gpu',
         devices=[FLAGS.gpu],
-        callbacks=[
-            callbacks.LearningRateMonitor(logging_interval='step'),
-            callbacks.ModelCheckpoint(monitor="val_cross_entropy",
-                                      filename='best'),
-            callbacks.ModelCheckpoint(filename='last'),
-            callbacks.EarlyStopping(
-                "val_cross_entropy",
-                patience=20,
-            )
-        ],
+        callbacks=callbacks,
         log_every_n_steps=10,
         **val_check,
     )
 
     torch.backends.cudnn.benchmark = True
     torch.set_float32_matmul_precision('high')
```

### Comparing `acids-msprior-1.1.1/setup.py` & `acids-msprior-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/tests/test_attention.py` & `acids-msprior-1.1.2/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `acids-msprior-1.1.1/tests/test_cache.py` & `acids-msprior-1.1.2/tests/test_cache.py`

 * *Files 26% similar despite different names*

```diff
@@ -57,54 +57,14 @@
         outputs_streaming.append(streaming(inputs, targets=inputs))
     outputs_streaming = torch.cat(outputs_streaming, 1)
 
     assert torch.allclose(outputs_regular, outputs_streaming, 1e-4, 1e-4)
 
 
 @load_configuration(
-    path="encoder_decoder.gin",
-    overrides=["MODEL_DIM = 16", "HEAD_DIM = 2", "NUM_LAYERS = 2"],
-)
-def test_encoder_decoder():
-    cc.use_cached_conv(False)
-    regular = Prior().eval()
-
-    cc.use_cached_conv(True)
-    streaming = Prior().eval()
-
-    for p1, p2 in zip(regular.parameters(), streaming.parameters()):
-        p2.data.copy_(p1.data)
-
-    input_params = gin.get_bindings("attention.MultivariateEmbedding")
-    inputs = torch.randint(
-        0,
-        input_params["num_tokens"],
-        (1, 128, input_params["num_quantizers"]),
-    )
-
-    semantic_params = gin.get_bindings("encoder/attention.Embedding")
-    semantic = torch.randint(
-        0,
-        semantic_params["num_embeddings"],
-        (1, 32),
-    )
-
-    outputs_regular = regular(inputs, semantic, targets=inputs)
-
-    num_chunks = 4
-    outputs_streaming = []
-    for inputs, semantic in zip(inputs.chunk(num_chunks, 1),
-                                semantic.chunk(num_chunks, 1)):
-        outputs_streaming.append(streaming(inputs, semantic, targets=inputs))
-    outputs_streaming = torch.cat(outputs_streaming, 1)
-
-    assert torch.allclose(outputs_regular, outputs_streaming, 1e-4, 1e-4)
-
-
-@load_configuration(
     path="decoder_only.gin",
     overrides=["MODEL_DIM = 16", "HEAD_DIM = 2", "NUM_LAYERS = 2"],
 )
 def test_decoder_only_nn_tilde():
     cc.use_cached_conv(False)
     regular = Prior().eval()
 
@@ -137,69 +97,7 @@
 
     # AUTOREGRESSIVE SAMPLE USING NN_TILDE
     streaming.previous_step[:1].copy_(inputs)
     out = streaming(torch.zeros(1, 16, 4))[:, :-1]
     streaming_samples = torch.cat([inputs, out.permute(0, 2, 1)], 1).long()
 
     assert torch.allclose(regular_samples, streaming_samples)
-
-
-@load_configuration(
-    path="encoder_decoder.gin",
-    overrides=["MODEL_DIM = 8", "HEAD_DIM = 2", "NUM_LAYERS = 1"],
-)
-def test_encoder_decoder_nn_tilde():
-    cc.use_cached_conv(False)
-    regular = Prior().eval()
-
-    cc.use_cached_conv(True)
-    streaming = ScriptedPrior().eval()
-
-    for p1, p2 in zip(regular.parameters(), streaming.parameters()):
-        p2.data.copy_(p1.data)
-
-    input_params = gin.get_bindings("attention.MultivariateEmbedding")
-    inputs = torch.randint(
-        0,
-        input_params["num_tokens"],
-        (1, 1, input_params["num_quantizers"]),
-    )
-
-    semantic_params = gin.get_bindings("encoder/attention.Embedding")
-    semantic = torch.randint(
-        0,
-        semantic_params["num_embeddings"],
-        (1, 16),
-    )
-
-    # AUTOREGRESSIVE SAMPLE USING REGULAR MODEL
-    regular_samples = [inputs]
-
-    regular_encoder_out = regular.encoder(semantic)
-
-    for i in range(64):
-        encoder_out_in = regular_encoder_out[:, :i // 4 + 1]
-        codes_in = torch.cat(regular_samples, 1)
-        sample, _ = regular.sample(
-            codes_in,
-            encoder_out_in,
-            temperature=0,
-        )
-        regular_samples.append(sample[:, -1:])
-
-    regular_samples = torch.cat(regular_samples, 1)
-
-    # AUTOREGRESSIVE SAMPLE USING NN_TILDE
-    streaming.set_listen(False)
-    streaming.set_reset(True)
-    streaming.set_temperature(0)
-    streaming.previous_step[:1].copy_(inputs)
-
-    semantic = semantic.repeat_interleave(4, -1)
-    streaming_inputs = torch.cat([
-        torch.zeros(1, 16, 64),
-        semantic[:, :64][:, None],
-    ], 1)
-    out = streaming(streaming_inputs)[:, :-1]
-    streaming_samples = torch.cat([inputs, out.permute(0, 2, 1)], 1).long()
-
-    assert torch.allclose(regular_samples, streaming_samples)
```

### Comparing `acids-msprior-1.1.1/tests/test_configs.py` & `acids-msprior-1.1.2/tests/test_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import torch
 
 from msprior.scripted import ScriptedPrior
 
 torch.set_grad_enabled(False)
 
 configs = map(str, pathlib.Path("msprior/configs").glob("*.gin"))
-configs = filter(lambda x:"flattened" not in x, configs)
-configs = filter(lambda x:"rwkv" not in x, configs)
+configs = filter(lambda x: "flattened" not in x, configs)
+configs = filter(lambda x: "rwkv" not in x, configs)
 configs = list(configs)
 
 names = map(os.path.basename, configs)
 names = map(lambda x: os.path.splitext(x)[0], names)
 
 names = itertools.product(names, ["continuous", "discrete"],
                           ["listen", "generate"])
```

