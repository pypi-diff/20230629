# Comparing `tmp/spear-tts-pytorch-0.0.3.tar.gz` & `tmp/spear-tts-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.3.tar", last modified: Thu Jun 29 18:16:12 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.4.tar", last modified: Thu Jun 29 19:32:30 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.3.tar` & `spear-tts-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:16:12.883972 spear-tts-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 18:16:02.000000 spear-tts-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 18:16:12.883972 spear-tts-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 18:16:02.000000 spear-tts-pytorch-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:16:12.883972 spear-tts-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 18:16:02.000000 spear-tts-pytorch-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:16:12.883972 spear-tts-pytorch-0.0.3/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 18:16:02.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-29 18:16:02.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:16:12.883972 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 18:16:12.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 18:16:12.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:16:12.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 18:16:12.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 18:16:12.000000 spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.3/LICENSE` & `spear-tts-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.3/PKG-INFO` & `spear-tts-pytorch-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.3/README.md` & `spear-tts-pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.3/setup.py` & `spear-tts-pytorch-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
```

### Comparing `spear-tts-pytorch-0.0.3/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.4/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,14 +21,24 @@
 
 def default(val, d):
     return val if exists(val) else d
 
 def empty(t: Tensor):
     return t.numel() == 0
 
+def set_eos_id(t: Tensor, eos_id: int, pad_id: int):
+    eos_indices = ((t == pad_id).cumsum(dim = -1) == 0).sum(dim = -1, keepdim = True).long()
+
+    batch_range = torch.arange(t.shape[0], device = t.device, dtype = torch.long)
+    batch_range = rearrange(batch_range, '... -> ... 1')
+
+    t = F.pad(t, (0, 1), value = pad_id)
+    t[batch_range, eos_indices] = eos_id
+    return t
+
 # t5 relative positional bias
 
 class RelativePositionBias(nn.Module):
     def __init__(
         self,
         *,
         heads,
@@ -255,15 +265,17 @@
         tokenizer_encode: Optional[Callable] = None,
         use_openai_tokenizer = False,
         wav2vec: Optional[Union[FairseqVQWav2Vec, HubertWithKmeans]] = None,
         num_semantic_token_ids = None,
         dim_head = 64,
         heads = 8,
         semantic_pad_id = -1,
-        text_pad_id = 0
+        text_pad_id = 0,
+        autoset_semantic_eos_id = True,
+        autoset_text_eos_id = True,
     ):
         super().__init__()
         self.dim = dim
         self.wav2vec = wav2vec
 
         self.tokenizer_encode = tokenizer_encode
 
@@ -282,18 +294,30 @@
         text_pad_id = text_pad_id
 
         self.pad_id = dict(
             speech = semantic_pad_id,
             text = text_pad_id
         )
 
+        # eos id
+
+        self.autoset_eos_id = dict(
+            speech = autoset_semantic_eos_id,
+            text = autoset_text_eos_id
+        )
+
+        self.eos_id = dict(
+            speech = num_semantic_token_ids,
+            text = num_text_token_ids
+        )
+
         # embedding
 
-        semantic_token_emb = nn.Embedding(num_semantic_token_ids, dim)
-        text_token_emb = nn.Embedding(num_text_token_ids, dim)
+        semantic_token_emb = nn.Embedding(num_semantic_token_ids + int(autoset_semantic_eos_id), dim)
+        text_token_emb = nn.Embedding(num_text_token_ids + int(autoset_text_eos_id), dim)
 
         self.semantic_token_emb = semantic_token_emb
 
         self.token_emb = nn.ModuleDict(dict(
             speech = semantic_token_emb,
             text = text_token_emb
         ))
@@ -358,27 +382,37 @@
 
         assert source.shape[0] == target.shape[0]
         batch = source.shape[0]
 
         source_token_emb = self.token_emb[source_type]
         source_pad_id = self.pad_id[source_type]
 
-        # if source mask is not passed in
-        # automatically derive by the padding id of the modality
-
-        if not exists(source_mask) and source.dtype == torch.long:
-            source_mask = source != source_pad_id
-
         # all target modules and parameters
 
         target_token_emb = self.token_emb[target_type]
         target_start_token = self.start_token[target_type]
         target_to_logit = self.to_logits[target_type]
         target_pad_id = self.pad_id[target_type]
 
+        # auto set eos id
+
+        if self.autoset_eos_id[source_type]:
+            source_eos_id = self.eos_id[source_type]
+            source = set_eos_id(source, source_eos_id, pad_id = source_pad_id)
+
+        if self.autoset_eos_id[target_type] and return_loss:
+            target_eos_id = self.eos_id[target_type]
+            target = set_eos_id(target, target_eos_id, pad_id = target_pad_id)
+
+        # if source mask is not passed in
+        # automatically derive by the padding id of the modality
+
+        if not exists(source_mask) and source.dtype == torch.long:
+            source_mask = source != source_pad_id
+
         # embedding
 
         source_emb = source_token_emb(source)
 
         target_emb = target_token_emb(target)
         start_token = repeat(target_start_token, 'd -> b 1 d', b = batch)
```

### Comparing `spear-tts-pytorch-0.0.3/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

