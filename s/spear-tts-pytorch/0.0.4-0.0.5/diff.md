# Comparing `tmp/spear-tts-pytorch-0.0.4.tar.gz` & `tmp/spear-tts-pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spear-tts-pytorch-0.0.4.tar", last modified: Thu Jun 29 19:32:30 2023, max compression
+gzip compressed data, was "spear-tts-pytorch-0.0.5.tar", last modified: Thu Jun 29 20:17:08 2023, max compression
```

## Comparing `spear-tts-pytorch-0.0.4.tar` & `spear-tts-pytorch-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/spear_tts_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12370 2023-06-29 19:32:20.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch/spear_tts_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:32:30.501274 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 19:32:30.000000 spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/spear_tts_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-06-29 20:16:57.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch/spear_tts_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 20:17:08.300353 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 20:17:08.000000 spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/top_level.txt
```

### Comparing `spear-tts-pytorch-0.0.4/LICENSE` & `spear-tts-pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.4/PKG-INFO` & `spear-tts-pytorch-0.0.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `spear-tts-pytorch-0.0.4/README.md` & `spear-tts-pytorch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spear-tts-pytorch-0.0.4/setup.py` & `spear-tts-pytorch-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'spear-tts-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Spear-TTS - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/spear-tts-pytorch',
   keywords = [
@@ -18,14 +18,15 @@
     'text-to-speech'
   ],
   install_requires=[
     'audiolm-pytorch>=1.2.8',
     'beartype',
     'einops>=0.6.1',
     'torch>=1.6',
+    'tqdm',
     'x-clip>=0.12.2'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
```

### Comparing `spear-tts-pytorch-0.0.4/spear_tts_pytorch/spear_tts_pytorch.py` & `spear-tts-pytorch-0.0.5/spear_tts_pytorch/spear_tts_pytorch.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import math
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn, einsum
 from torch.nn import Module, ModuleList
 
-from einops import rearrange, repeat
+from einops import rearrange, repeat, pack
 
 from audiolm_pytorch import FairseqVQWav2Vec, HubertWithKmeans
 
 from beartype import beartype
 from beartype.door import is_bearable
 from beartype.typing import Optional, Union, Callable, Literal, Tuple, List
 
 from x_clip.tokenizer import tokenizer
 
+from tqdm import tqdm
+
 # helpers
 
 def exists(val):
     return val is not None
 
 def default(val, d):
     return val if exists(val) else d
@@ -31,14 +33,53 @@
     batch_range = torch.arange(t.shape[0], device = t.device, dtype = torch.long)
     batch_range = rearrange(batch_range, '... -> ... 1')
 
     t = F.pad(t, (0, 1), value = pad_id)
     t[batch_range, eos_indices] = eos_id
     return t
 
+# sampling helpers
+
+def eval_decorator(fn):
+    def inner(self, *args, **kwargs):
+        was_training = self.training
+        self.eval()
+        out = fn(self, *args, **kwargs)
+        self.train(was_training)
+        return out
+    return inner
+
+def log(t, eps = 1e-20):
+    return torch.log(t.clamp(min = eps))
+
+def gumbel_noise(t):
+    noise = torch.zeros_like(t).uniform_(0, 1)
+    return -log(-log(noise))
+
+def gumbel_sample(t, temperature = 1., dim = -1):
+    return ((t / max(temperature, 1e-10)) + gumbel_noise(t)).argmax(dim = dim)
+
+def top_p(logits, thres = 0.9):
+    sorted_logits, sorted_indices = torch.sort(logits, descending=True)
+    cum_probs = torch.cumsum(F.softmax(sorted_logits, dim=-1), dim=-1)
+
+    sorted_indices_to_remove = cum_probs > (1 - thres)
+    sorted_indices_to_remove[:, 1:] = sorted_indices_to_remove[:, :-1].clone()
+    sorted_indices_to_remove[:, 0] = 0
+
+    sorted_logits[sorted_indices_to_remove] = float('-inf')
+    return sorted_logits.scatter(1, sorted_indices, sorted_logits)
+
+def top_k(logits, thres = 0.9):
+    k = math.ceil((1 - thres) * logits.shape[-1])
+    val, ind = torch.topk(logits, k)
+    probs = torch.full_like(logits, float('-inf'))
+    probs.scatter_(1, ind, val)
+    return probs
+
 # t5 relative positional bias
 
 class RelativePositionBias(nn.Module):
     def __init__(
         self,
         *,
         heads,
@@ -357,32 +398,128 @@
             dim_head = dim_head,
             heads = heads,
             depth = source_depth,
             causal = True,
             cross_attend = True
         )
 
+    @property
+    def device(self):
+        return next(self.parameters()).device
+
+    @torch.no_grad()
+    @eval_decorator
+    @beartype
+    def generate(
+        self,
+        source: Union[List[str], Tensor],
+        *,
+        source_type: SpeechOrTextLiteral,
+        target_type: SpeechOrTextLiteral,
+        temperature = 1.,
+        filter_logits_fn = top_k,
+        filter_thres = 0.9,
+        source_mask: Optional[Tensor] = None,
+        max_length = 2048
+    ):
+        if is_bearable(source, List[str]):
+            assert exists(self.tokenizer_encode)
+            source = self.tokenizer_encode(source)
+            source = source.to(self.device)
+
+        batch = source.shape[0]
+
+        source_token_emb = self.token_emb[source_type]
+        source_pad_id = self.pad_id[source_type]
+
+        # all target modules and parameters
+
+        target_token_emb = self.token_emb[target_type]
+        target_start_token = self.start_token[target_type]
+        target_to_logit = self.to_logits[target_type]
+        target_pad_id = self.pad_id[target_type]
+        target_eos_id = self.eos_id[target_type]
+
+        # auto set eos id
+
+        if self.autoset_eos_id[source_type]:
+            source_eos_id = self.eos_id[source_type]
+            source = set_eos_id(source, source_eos_id, pad_id = source_pad_id)
+
+        # if source mask is not passed in
+        # automatically derive by the padding id of the modality
+
+        if not exists(source_mask) and source.dtype == torch.long:
+            source_mask = source != source_pad_id
+
+        # source embedding
+
+        source_emb = source_token_emb(source)
+
+        source_emb = self.source_transformer(source_emb, mask = source_mask)
+
+        # decode target
+
+        target = torch.empty((batch, 0), dtype = torch.long, device = self.device)
+        start_token = repeat(target_start_token, 'd -> b 1 d', b = batch)
+
+        # loop to decode
+
+        for _ in tqdm(range(max_length)):
+            target_emb = target_token_emb(target)
+            target_emb = torch.cat((start_token, target_emb), dim = 1)
+
+            # target attention
+
+            target_emb = self.target_transformer(target_emb, context = source_emb, context_mask = source_mask)
+
+            # decoder logits
+
+            logits = target_to_logit(target_emb)
+
+            logits = logits[:, -1]
+            logits = filter_logits_fn(logits, thres = filter_thres)
+
+            sampled = gumbel_sample(logits, temperature = temperature)
+            target, _ = pack((target, sampled), 'b *')
+
+            if not self.autoset_eos_id[target_type]:
+                continue
+
+            is_eos = target == target_eos_id
+
+            if not is_eos.any(dim = -1).all():
+                continue
+
+            mask = is_eos.cumsum(dim = -1) == 0
+            target = target.masked_fill(~mask, target_pad_id)
+            break
+
+        return target
+
     @beartype
     def forward(
         self,
         source: Union[List[str], Tensor],
         target: Union[List[str], Tensor],
         *,
         source_type: SpeechOrTextLiteral,
         target_type: SpeechOrTextLiteral,
         source_mask: Optional[Tensor] = None,
         return_loss = False
     ):
         if is_bearable(source, List[str]):
             assert exists(self.tokenizer_encode)
             source = self.tokenizer_encode(source)
+            source = source.to(self.device)
 
         if is_bearable(target, List[str]):
             assert exists(self.tokenizer_encode)
             target = self.tokenizer_encode(target)
+            target = target.to(self.device)
 
         assert source.shape[0] == target.shape[0]
         batch = source.shape[0]
 
         source_token_emb = self.token_emb[source_type]
         source_pad_id = self.pad_id[source_type]
```

### Comparing `spear-tts-pytorch-0.0.4/spear_tts_pytorch.egg-info/PKG-INFO` & `spear-tts-pytorch-0.0.5/spear_tts_pytorch.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spear-tts-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spear-TTS - Pytorch
 Home-page: https://github.com/lucidrains/spear-tts-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-speech
 Classifier: Development Status :: 4 - Beta
```

