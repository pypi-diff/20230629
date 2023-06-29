# Comparing `tmp/x-clip-0.8.4.tar.gz` & `tmp/x-clip-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-clip-0.8.4.tar", last modified: Fri Aug  5 14:57:56 2022, max compression
+gzip compressed data, was "x-clip-0.9.0.tar", last modified: Wed Aug 17 03:53:28 2022, max compression
```

## Comparing `x-clip-0.8.4.tar` & `x-clip-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 14:57:56.688338 x-clip-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-05 14:57:45.000000 x-clip-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-05 14:57:45.000000 x-clip-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-05 14:57:56.688338 x-clip-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10754 2022-08-05 14:57:45.000000 x-clip-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-05 14:57:56.688338 x-clip-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-05 14:57:45.000000 x-clip-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 14:57:56.684338 x-clip-0.8.4/x_clip/
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 14:57:56.684338 x-clip-0.8.4/x_clip/data/
--rw-r--r--   0 runner    (1001) docker     (121)  3194984 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/data/bpe_simple_vocab_16e6.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/mlm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5155 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9208 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/visual_ssl.py
--rw-r--r--   0 runner    (1001) docker     (121)    25679 2022-08-05 14:57:45.000000 x-clip-0.8.4/x_clip/x_clip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-05 14:57:56.684338 x-clip-0.8.4/x_clip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-05 14:57:56.000000 x-clip-0.8.4/x_clip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-05 14:57:56.000000 x-clip-0.8.4/x_clip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-05 14:57:56.000000 x-clip-0.8.4/x_clip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-05 14:57:56.000000 x-clip-0.8.4/x_clip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-05 14:57:56.000000 x-clip-0.8.4/x_clip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 03:53:28.314635 x-clip-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-17 03:53:19.000000 x-clip-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-08-17 03:53:19.000000 x-clip-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-17 03:53:28.314635 x-clip-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    10754 2022-08-17 03:53:19.000000 x-clip-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-17 03:53:28.314635 x-clip-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-08-17 03:53:19.000000 x-clip-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 03:53:28.310635 x-clip-0.9.0/x_clip/
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 03:53:28.310635 x-clip-0.9.0/x_clip/data/
+-rw-r--r--   0 runner    (1001) docker     (121)  3194984 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/data/bpe_simple_vocab_16e6.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3888 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/mlm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5155 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9208 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/visual_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27436 2022-08-17 03:53:19.000000 x-clip-0.9.0/x_clip/x_clip.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-17 03:53:28.310635 x-clip-0.9.0/x_clip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-17 03:53:28.000000 x-clip-0.9.0/x_clip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-17 03:53:28.000000 x-clip-0.9.0/x_clip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-17 03:53:28.000000 x-clip-0.9.0/x_clip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-08-17 03:53:28.000000 x-clip-0.9.0/x_clip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-08-17 03:53:28.000000 x-clip-0.9.0/x_clip.egg-info/top_level.txt
```

### Comparing `x-clip-0.8.4/LICENSE` & `x-clip-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/PKG-INFO` & `x-clip-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-clip
-Version: 0.8.4
+Version: 0.9.0
 Summary: X-CLIP
 Home-page: https://github.com/lucidrains/x-clip
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,contrastive learning,CLIP
 Classifier: Development Status :: 4 - Beta
```

### Comparing `x-clip-0.8.4/README.md` & `x-clip-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/setup.py` & `x-clip-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'x-clip',
   packages = find_packages(exclude=[]),
   include_package_data = True,
-  version = '0.8.4',
+  version = '0.9.0',
   license='MIT',
   description = 'X-CLIP',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/x-clip',
   long_description_content_type = 'text/markdown',
   keywords = [
```

### Comparing `x-clip-0.8.4/x_clip/data/bpe_simple_vocab_16e6.txt` & `x-clip-0.9.0/x_clip/data/bpe_simple_vocab_16e6.txt`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/x_clip/mlm.py` & `x-clip-0.9.0/x_clip/mlm.py`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/x_clip/tokenizer.py` & `x-clip-0.9.0/x_clip/tokenizer.py`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/x_clip/visual_ssl.py` & `x-clip-0.9.0/x_clip/visual_ssl.py`

 * *Files identical despite different names*

### Comparing `x-clip-0.8.4/x_clip/x_clip.py` & `x-clip-0.9.0/x_clip/x_clip.py`

 * *Files 8% similar despite different names*

```diff
@@ -166,42 +166,49 @@
             nn.Linear(inner_dim, dim, bias = False)
         )
 
     def forward(self, x):
         return self.net(x)
 
 class Attention(nn.Module):
-    def __init__(self, dim, dim_head = 64, heads = 8, dropout = 0.):
+    def __init__(self, dim, dim_head = 64, heads = 8, causal = False, dropout = 0.):
         super().__init__()
         self.heads = heads
+        self.causal = causal
         self.scale = dim_head ** -0.5
         inner_dim = dim_head * heads
 
         self.to_qkv = nn.Linear(dim, inner_dim * 3, bias = False)
         self.to_out = nn.Sequential(nn.Linear(inner_dim, dim, bias = False), LayerNorm(dim))
         self.dropout = nn.Dropout(dropout)
 
     def forward(self, x, mask = None, rotary_pos_emb = None):
-        h = self.heads
+        h, device = self.heads, x.device
         q, k, v = self.to_qkv(x).chunk(3, dim = -1)
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
         q = q * self.scale
 
         if exists(rotary_pos_emb):
             apply_rotary = partial(apply_rotary_pos_emb, rotary_pos_emb)
             q, k, v = map(apply_rotary, (q, k, v))
 
         sim = einsum('b h i d, b h j d -> b h i j', q, k)
 
+        mask_value = -torch.finfo(sim.dtype).max
+
         if exists(mask):
             mask = rearrange(mask, 'b j -> b 1 1 j')
-            mask_value = -torch.finfo(sim.dtype).max
             sim = sim.masked_fill(~mask, mask_value)
 
+        if self.causal:
+            i, j = sim.shape[-2:]
+            causal_mask = torch.ones((i, j), dtype = torch.bool, device = device).triu(j - i + 1)
+            sim = sim.masked_fill(causal_mask, mask_value)
+
         attn = sim.softmax(dim = -1, dtype = torch.float32)
         attn = self.dropout(attn)
 
         out = einsum('b h i j, b h j d -> b h i d', attn, v)
         out = rearrange(out, 'b h n d -> b n (h d)')
         return self.to_out(out)
 
@@ -209,26 +216,27 @@
     def __init__(
         self,
         dim,
         *,
         depth,
         dim_head = 64,
         heads = 8,
+        causal = False,
         attn_dropout = 0.,
         ff_dropout = 0.,
         ff_mult = 4,
         checkpoint_during_training = False
     ):
         super().__init__()
         self.checkpoint_during_training = checkpoint_during_training
 
         self.layers = nn.ModuleList([])
         for _ in range(depth):
             self.layers.append(nn.ModuleList([
-                PreNorm(dim, Attention(dim = dim, dim_head = dim_head, heads = heads, dropout = attn_dropout)),
+                PreNorm(dim, Attention(dim = dim, dim_head = dim_head, heads = heads, causal = causal, dropout = attn_dropout)),
                 PreNorm(dim, FeedForward(dim = dim, mult = ff_mult)),
             ]))
 
         self.norm_in = LayerNorm(dim)
         self.norm_out = LayerNorm(dim)
 
     def forward(
@@ -257,44 +265,46 @@
         self,
         dim,
         *,
         num_tokens,
         max_seq_len,
         dim_head,
         rotary_pos_emb = None,
+        causal = False,
         **kwargs
     ):
         super().__init__()
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         self.abs_pos_emb = nn.Embedding(max_seq_len, dim) if not rotary_pos_emb else None
         self.rotary_pos_emb = RotaryEmbedding(min(dim_head, 32)) if rotary_pos_emb else None
 
-        self.cls_token = nn.Parameter(torch.randn(dim))
+        self.cls_token = nn.Parameter(torch.randn(dim)) if not causal else None
 
-        self.transformer = Transformer(dim, dim_head = dim_head, **kwargs)
+        self.transformer = Transformer(dim, dim_head = dim_head, causal = causal, **kwargs)
 
     def forward(self, x, mask = None):
         b, n, device = *x.shape, x.device
 
         x = self.token_emb(x)
 
         if exists(self.abs_pos_emb):
             pos_emb = self.abs_pos_emb(torch.arange(n, device = device))
             x = x + rearrange(pos_emb, 'n d -> 1 n d')
 
         rotary_pos_emb = None
         if exists(self.rotary_pos_emb):
             rotary_pos_emb = self.rotary_pos_emb(n + 1, device = device)
 
-        cls_tokens = repeat(self.cls_token, 'd -> b 1 d', b = b)
-        x = torch.cat((cls_tokens, x), dim = 1)
+        if exists(self.cls_token):
+            cls_tokens = repeat(self.cls_token, 'd -> b 1 d', b = b)
+            x = torch.cat((cls_tokens, x), dim = 1)
 
-        if exists(mask):
-            mask = F.pad(mask, (1, 0), value = True)
+            if exists(mask):
+                mask = F.pad(mask, (1, 0), value = True)
 
         out = self.transformer(x, mask = mask, rotary_pos_emb = rotary_pos_emb)
         return out
 
 class VisionTransformer(nn.Module):
     def __init__(
         self,
@@ -371,14 +381,16 @@
         text_enc_depth = 6,
         text_seq_len = 256,
         text_heads = 8,
         text_dim_head = 64,
         text_has_cls_token = True,
         text_pad_id = 0,
         text_rotary_pos_emb = False,
+        text_causal_mask = False,
+        text_eos_id = None,
         text_encode_without_mask = False,
         visual_enc_depth = 6,
         visual_heads = 8,
         visual_dim_head = 64,
         visual_image_size = 256,
         visual_patch_size = 32,
         visual_has_cls_token = True,
@@ -415,23 +427,29 @@
 
         self.text_pad_id = text_pad_id
         self.text_has_cls_token = text_has_cls_token
         self.text_seq_len = text_seq_len
 
         self.text_encode_without_mask = text_encode_without_mask # whether to pass in text mask to text encoder
 
+        self.text_causal_mask = text_causal_mask
+        self.text_eos_id = text_eos_id
+
+        assert not (text_causal_mask and not exists(text_eos_id)), 'text EOS token id must be given if using causal mask in text transformer'
+
         if exists(text_encoder):
             self.text_transformer = text_encoder
         else:
             self.text_transformer = TextTransformer(
                 dim = dim_text,
                 num_tokens = num_text_tokens + (1 if use_mlm else 0),
                 max_seq_len = text_seq_len,
                 depth = text_enc_depth,
                 heads = text_heads,
+                causal = text_causal_mask,
                 dim_head = text_dim_head,
                 rotary_pos_emb = text_rotary_pos_emb,
                 checkpoint_during_training = checkpoint_during_training
             )
 
         # instantiate image transformer
 
@@ -592,14 +610,33 @@
 
         enc_text = model_forward_with_context(
             fn = self.text_transformer,
             args = text_args,
             freeze = freeze_text_encoder
         )
 
+        # depending on whether text is using causal mask, post process, moving eos token to the first position
+
+        if self.text_causal_mask:
+            eos_text_mask = (text == self.text_eos_id)
+            assert torch.all(torch.any(eos_text_mask, dim = -1)), f'some of the text rows does not have the eos id {self.text_eos_id}'
+
+            text_len = text.shape[-1]
+            eos_indices = eos_text_mask.float().argmax(dim = -1, keepdim = True)
+
+            eos_text_mask = torch.zeros_like(eos_text_mask).scatter(1, eos_indices, 1.).bool()
+            eos_text_mask = rearrange(eos_text_mask, '... -> ... 1')
+
+            eos_tokens = enc_text.masked_select(eos_text_mask)
+            rest_tokens = enc_text.masked_select(~eos_text_mask)
+
+            eos_tokens = rearrange(eos_tokens, '(b d) -> b 1 d', b = b)
+            rest_tokens = rearrange(rest_tokens, '(b n d) -> b n d', b = b, n = text_len - 1)
+            enc_text = torch.cat((eos_tokens, rest_tokens), dim = 1)
+
         # whether to train image encoder, in the case that the image net was pretrained as recommended in LiT
 
         enc_image = model_forward_with_context(
             fn = self.visual_transformer,
             args = (image,),
             freeze = freeze_image_encoder
         )
```

### Comparing `x-clip-0.8.4/x_clip.egg-info/PKG-INFO` & `x-clip-0.9.0/x_clip.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-clip
-Version: 0.8.4
+Version: 0.9.0
 Summary: X-CLIP
 Home-page: https://github.com/lucidrains/x-clip
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,contrastive learning,CLIP
 Classifier: Development Status :: 4 - Beta
```

