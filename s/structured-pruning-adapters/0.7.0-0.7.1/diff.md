# Comparing `tmp/structured-pruning-adapters-0.7.0.tar.gz` & `tmp/structured-pruning-adapters-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structured-pruning-adapters-0.7.0.tar", last modified: Wed Jun 21 13:28:17 2023, max compression
+gzip compressed data, was "structured-pruning-adapters-0.7.1.tar", last modified: Thu Jun 29 09:34:33 2023, max compression
```

## Comparing `structured-pruning-adapters-0.7.0.tar` & `structured-pruning-adapters-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,28 @@
-drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.193543 structured-pruning-adapters-0.7.0/
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    11357 2022-06-15 08:39:30.000000 structured-pruning-adapters-0.7.0/LICENSE
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7752 2023-06-21 13:28:17.193279 structured-pruning-adapters-0.7.0/PKG-INFO
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     6515 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/README.md
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)       38 2023-06-21 13:28:17.193644 structured-pruning-adapters-0.7.0/setup.cfg
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     2565 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/setup.py
-drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.191247 structured-pruning-adapters-0.7.0/sp_adapters/
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      599 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/__init__.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      116 2022-06-15 13:38:30.000000 structured-pruning-adapters-0.7.0/sp_adapters/base.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     1445 2022-11-17 10:31:11.000000 structured-pruning-adapters-0.7.0/sp_adapters/lora.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7089 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/splopa.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    31521 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/splora.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     9919 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/sppara.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)    13244 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/torch_pruning.py
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     2076 2023-06-21 13:28:07.000000 structured-pruning-adapters-0.7.0/sp_adapters/utils.py
-drwxr-xr-x   0 au478108 (794351465) UNI\Domain Users (357318537)        0 2023-06-21 13:28:17.192829 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)     7752 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/PKG-INFO
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      460 2023-06-21 13:28:17.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/SOURCES.txt
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)        1 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/dependency_links.txt
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)      119 2023-06-21 13:28:16.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/requires.txt
--rw-r--r--   0 au478108 (794351465) UNI\Domain Users (357318537)       12 2023-06-21 13:28:17.000000 structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:34:33.293434 structured-pruning-adapters-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-29 09:34:33.293434 structured-pruning-adapters-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:34:33.293434 structured-pruning-adapters-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:34:33.289434 structured-pruning-adapters-0.7.1/sp_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31616 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/sppara.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13244 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/torch_pruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/sp_adapters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:34:33.289434 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-29 09:34:33.000000 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 09:34:33.000000 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:34:33.000000 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 09:34:33.000000 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 09:34:33.000000 structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:34:33.293434 structured-pruning-adapters-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_lin_as_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_splopa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17924 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_splora.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_sppara.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_torchpruning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-29 09:32:35.000000 structured-pruning-adapters-0.7.1/tests/test_utils.py
```

### Comparing `structured-pruning-adapters-0.7.0/LICENSE` & `structured-pruning-adapters-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/PKG-INFO` & `structured-pruning-adapters-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.7.0
+Version: 0.7.1
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.1 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `structured-pruning-adapters-0.7.0/README.md` & `structured-pruning-adapters-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/setup.py` & `structured-pruning-adapters-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/__init__.py` & `structured-pruning-adapters-0.7.1/sp_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/lora.py` & `structured-pruning-adapters-0.7.1/sp_adapters/lora.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/splopa.py` & `structured-pruning-adapters-0.7.1/sp_adapters/splopa.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/splora.py` & `structured-pruning-adapters-0.7.1/sp_adapters/splora.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,24 +101,25 @@
 class _SPLoRAConvNd:
     def __init__(
         self,
         ConvCls: Union[nn.Conv1d, nn.Conv2d, nn.Conv3d],
         in_channels: int,
         out_channels: int,
         bias: bool = True,
+        groups: int = 1,
         # rank (int) or fraction of output_channels
         rank: Union[int, float] = _DEFAULT_RANK,
         init_range: float = _DEFAULT_INIT_RANGE,
         device=None,
         dtype=None,
     ):
         self._nd = int(ConvCls.__name__[-2])
         self._ConvCls = ConvCls
         self.adapter = LowRankMatrix(
-            1, in_channels, out_channels, rank, init_range=init_range
+            1, in_channels // groups, out_channels, rank, init_range=init_range
         )
 
     def forward(self, input: Tensor) -> Tensor:
         return self._conv_forward(input, self.adapted_weight, self.bias)
 
     @property
     def adapted_weight(self) -> nn.Parameter:
@@ -188,14 +189,15 @@
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPLoRAConvNd.__init__(
             self,
             nn.Conv1d,
             in_channels,
             out_channels,
             bias,
+            groups,
             rank,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
@@ -261,14 +263,15 @@
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPLoRAConvNd.__init__(
             self,
             nn.Conv2d,
             in_channels,
             out_channels,
             bias,
+            groups,
             rank,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
@@ -334,14 +337,15 @@
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPLoRAConvNd.__init__(
             self,
             nn.Conv3d,
             in_channels,
             out_channels,
             bias,
+            groups,
             rank,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
```

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/sppara.py` & `structured-pruning-adapters-0.7.1/sp_adapters/sppara.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,24 +17,25 @@
     """Base class for Convolutional {S}tructured {P}runing {Pa}rallel {Re}sidual {A}dapters"""
 
     def __init__(
         self,
         ConvCls: Union[nn.Conv1d, nn.Conv2d, nn.Conv3d],
         in_channels: int,
         out_channels: int,
-        bias: bool = True,
-        # rank (int) or fraction of output_channels
+        groups: int = 1,
         init_range: float = _DEFAULT_INIT_RANGE,
         device=None,
         dtype=None,
+        *args,
+        **kwargs,
     ):
         self._nd = int(ConvCls.__name__[-2])
         self._ConvCls = ConvCls
         self.adapter = nn.Parameter(
-            torch.empty((in_channels, out_channels), device=device, dtype=dtype)
+            torch.empty(out_channels, in_channels // groups, device=device, dtype=dtype)
         )
         nn.init.uniform_(self.adapter, -init_range, init_range)
 
     def forward(self, input: Tensor) -> Tensor:
         return self._conv_forward(input, self.adapted_weight, self.bias)
 
     @property
@@ -42,15 +43,15 @@
         if self.weight.requires_grad:
             self.weight.requires_grad = False
         w_diag = torch.zeros_like(self.weight)
         kdx = self.kernel_size[0] // 2
         center_inds = [kdx for _ in range(self._nd)]
         # w_diag[:, :, *center_inds] += self.adapter # Python 3.11+
         wdx = [slice(None), slice(None)] + center_inds
-        w_diag.__setitem__(wdx, w_diag.__getitem__(wdx) + self.adapter.T)
+        w_diag.__setitem__(wdx, w_diag.__getitem__(wdx) + self.adapter)
         return self.weight + w_diag
 
     def to_module(self) -> torch.nn.modules.conv._ConvNd:
         instance = self._ConvCls(
             self.in_channels,
             self.out_channels,
             self.kernel_size,
@@ -104,15 +105,15 @@
         assert len(set(self.kernel_size)) == 1, "All dimensions of kernel_size equal."
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPPaRAConvNd.__init__(
             self,
             nn.Conv1d,
             in_channels,
             out_channels,
-            bias,
+            groups,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
     def from_module(
@@ -173,15 +174,15 @@
         assert len(set(self.kernel_size)) == 1, "All dimensions of kernel_size equal."
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPPaRAConvNd.__init__(
             self,
             nn.Conv2d,
             in_channels,
             out_channels,
-            bias,
+            groups,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
     def from_module(
@@ -242,15 +243,15 @@
         assert len(set(self.kernel_size)) == 1, "All dimensions of kernel_size equal."
         assert self.kernel_size[0] % 2 == 1, "kernel_size should be odd."
         _SPPaRAConvNd.__init__(
             self,
             nn.Conv3d,
             in_channels,
             out_channels,
-            bias,
+            groups,
             init_range,
             device,
             dtype,
         )
 
     @classmethod
     def from_module(
@@ -309,17 +310,17 @@
     out_features_mask: torch.BoolTensor = None,
 ) -> Iterator[Tuple[str, nn.Parameter]]:
     for name, param in module.named_parameters(
         prefix=prefix, recurse=recurse, remove_duplicate=True
     ):
         if name == "adapter":
             if in_features_mask is not None:
-                param = param[in_features_mask]
+                param = param[:, in_features_mask]
             if out_features_mask is not None:
-                param = param[:, out_features_mask]
+                param = param[out_features_mask]
         elif name == "bias" and out_features_mask is not None:
             param = param[out_features_mask]
         elif name == "weight" and not adapter_weights_only:
             if out_features_mask is not None:
                 param = param[out_features_mask]
             if in_features_mask is not None:
                 param = param[:, in_features_mask]
```

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/torch_pruning.py` & `structured-pruning-adapters-0.7.1/sp_adapters/torch_pruning.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/sp_adapters/utils.py` & `structured-pruning-adapters-0.7.1/sp_adapters/utils.py`

 * *Files identical despite different names*

### Comparing `structured-pruning-adapters-0.7.0/structured_pruning_adapters.egg-info/PKG-INFO` & `structured-pruning-adapters-0.7.1/structured_pruning_adapters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structured-pruning-adapters
-Version: 0.7.0
+Version: 0.7.1
 Summary: Structured Pruning Adapters for PyTorch
 Home-page: https://github.com/lukashedegaard/structured-pruning-adapters
 Author: Lukas Hedegaard
 Author-email: lukasxhedegaard@gmail.com
 License: UNKNOWN
 Keywords: deep learning,pytorch,AI,adapters,pruning,inference
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.0 Summary:
+Metadata-Version: 2.1 Name: structured-pruning-adapters Version: 0.7.1 Summary:
 Structured Pruning Adapters for PyTorch Home-page: https://github.com/
 lukashedegaard/structured-pruning-adapters Author: Lukas Hedegaard Author-
 email: lukasxhedegaard@gmail.com License: UNKNOWN Keywords: deep
 learning,pytorch,AI,adapters,pruning,inference Platform: UNKNOWN Classifier:
 Environment :: Console Classifier: Natural Language :: English Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

