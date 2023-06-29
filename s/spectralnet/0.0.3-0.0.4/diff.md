# Comparing `tmp/spectralnet-0.0.3.tar.gz` & `tmp/spectralnet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.3.tar", last modified: Tue Jun 27 12:06:39 2023, max compression
+gzip compressed data, was "spectralnet-0.0.4.tar", last modified: Thu Jun 29 14:34:23 2023, max compression
```

## Comparing `spectralnet-0.0.3.tar` & `spectralnet-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.273912 spectralnet-0.0.3/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-25 12:12:14.000000 spectralnet-0.0.3/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-27 12:06:39.273998 spectralnet-0.0.3/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-27 12:05:58.000000 spectralnet-0.0.3/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-27 10:10:06.000000 spectralnet-0.0.3/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-27 12:06:39.274305 spectralnet-0.0.3/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-27 11:38:50.000000 spectralnet-0.0.3/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.269049 spectralnet-0.0.3/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.270830 spectralnet-0.0.3/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      114 2023-06-27 09:56:19.000000 spectralnet-0.0.3/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.271770 spectralnet-0.0.3/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-25 13:45:07.000000 spectralnet-0.0.3/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-25 17:02:04.000000 spectralnet-0.0.3/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-25 13:27:35.000000 spectralnet-0.0.3/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-25 17:05:52.000000 spectralnet-0.0.3/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.272797 spectralnet-0.0.3/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-25 13:44:44.000000 spectralnet-0.0.3/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-27 09:25:21.000000 spectralnet-0.0.3/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-25 17:56:01.000000 spectralnet-0.0.3/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2897 2023-06-25 18:01:13.000000 spectralnet-0.0.3/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-26 12:24:44.000000 spectralnet-0.0.3/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.273767 spectralnet-0.0.3/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-25 17:49:01.000000 spectralnet-0.0.3/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3733 2023-06-25 18:43:37.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9437 2023-06-25 18:58:20.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7892 2023-06-27 11:52:09.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-25 17:43:03.000000 spectralnet-0.0.3/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-25 17:04:22.000000 spectralnet-0.0.3/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-27 12:06:39.271409 spectralnet-0.0.3/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      823 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       12 2023-06-27 12:06:39.000000 spectralnet-0.0.3/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.901244 spectralnet-0.0.4/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-25 12:12:14.000000 spectralnet-0.0.4/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 14:34:23.901350 spectralnet-0.0.4/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-27 16:30:09.000000 spectralnet-0.0.4/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-27 10:10:06.000000 spectralnet-0.0.4/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-29 14:34:23.901660 spectralnet-0.0.4/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-27 11:38:50.000000 spectralnet-0.0.4/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.891526 spectralnet-0.0.4/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.893991 spectralnet-0.0.4/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-27 12:26:31.000000 spectralnet-0.0.4/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.895449 spectralnet-0.0.4/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-25 13:45:07.000000 spectralnet-0.0.4/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-25 17:02:04.000000 spectralnet-0.0.4/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-25 13:27:35.000000 spectralnet-0.0.4/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-25 17:05:52.000000 spectralnet-0.0.4/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.897030 spectralnet-0.0.4/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-25 13:44:44.000000 spectralnet-0.0.4/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-27 09:25:21.000000 spectralnet-0.0.4/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-25 17:56:01.000000 spectralnet-0.0.4/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:15:11.000000 spectralnet-0.0.4/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-26 12:24:44.000000 spectralnet-0.0.4/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.899206 spectralnet-0.0.4/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-25 17:49:01.000000 spectralnet-0.0.4/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:23:29.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:23:36.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     8022 2023-06-29 14:22:49.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-25 17:43:03.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-25 17:04:22.000000 spectralnet-0.0.4/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.894751 spectralnet-0.0.4/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      872 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       18 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.900835 spectralnet-0.0.4/src/tests/
+-rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 04:54:02.000000 spectralnet-0.0.4/src/tests/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 09:34:12.000000 spectralnet-0.0.4/src/tests/test_twomoons.py
```

### Comparing `spectralnet-0.0.3/LICENSE.md` & `spectralnet-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/PKG-INFO` & `spectralnet-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,28 @@
 License-File: LICENSE.md
 
 # SpectralNet
 
 <p align="center">
     <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
 
-SpectralNet is a python package that performs spectral clustering with deep neural networks.<br><br>
+SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
 
 ```bash
 pip install spectralnet
 ```
 
 ## Usage
 
-The basic functionlaity is quite intuitive and easy to use, e.g.,
+The basic functionality is quite intuitive and easy to use, e.g.,
 
 ```python
 from spectralnet import SpectralNet
 
 spectralnet = SpectralNet(n_clusters=10)
 spectralnet.fit(X) # X is the dataset and it should be a torch.Tensor
 cluster_assignments = spectralnet.predict(X) # Get the final assignments to clusters
```

### Comparing `spectralnet-0.0.3/README.md` & `spectralnet-0.0.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SpectralNet
 
 <p align="center">
     <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
 
-SpectralNet is a python package that performs spectral clustering with deep neural networks.<br><br>
+SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
 
 ```bash
 pip install spectralnet
 ```
 
 ## Usage
 
-The basic functionlaity is quite intuitive and easy to use, e.g.,
+The basic functionality is quite intuitive and easy to use, e.g.,
 
 ```python
 from spectralnet import SpectralNet
 
 spectralnet = SpectralNet(n_clusters=10)
 spectralnet.fit(X) # X is the dataset and it should be a torch.Tensor
 cluster_assignments = spectralnet.predict(X) # Get the final assignments to clusters
```

### Comparing `spectralnet-0.0.3/setup.cfg` & `spectralnet-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.0.3
+version = 0.0.4
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AmitaiYacobi/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/AmitaiYacobi/SpectralNet/issues
```

### Comparing `spectralnet-0.0.3/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.4/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.4/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_metrics.py` & `spectralnet-0.0.4/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.4/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.4/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.4/src/spectralnet/_models/_spectralnet_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,29 +35,21 @@
         Returns
         -------
         torch.Tensor
             The orthonormalized output.
 
         Notes
         -----
-        This function applies the Cholesky decomposition to orthonormalize the output (`Y`) of the network.
-        The orthonormalized output is returned as a tensor.
+        This function applies QR decomposition to orthonormalize the output (`Y`) of the network.
+        The inverse of the R matrix is returned as the orthonormalization weights.
         """
 
         m = Y.shape[0]
-        to_factorize = torch.mm(Y.t(), Y)
-
-        try:
-            L = torch.linalg.cholesky(to_factorize, upper=False)
-        except torch._C._LinAlgError:
-            to_factorize += 0.1 * torch.eye(to_factorize.shape[0])
-            L = torch.linalg.cholesky(to_factorize, upper=False)
-
-        L_inverse = torch.inverse(L)
-        orthonorm_weights = np.sqrt(m) * L_inverse.t()
+        _, R = torch.linalg.qr(Y)
+        orthonorm_weights = np.sqrt(m) * torch.inverse(R)
         return orthonorm_weights
 
     def forward(
         self, x: torch.Tensor, should_update_orth_weights: bool = True
     ) -> torch.Tensor:
         """
         Perform the forward pass of the model.
@@ -74,19 +66,19 @@
         torch.Tensor
             The output tensor.
 
         Notes
         -----
         This function takes an input tensor `x` and computes the forward pass of the model.
         If `should_update_orth_weights` is set to True, the orthonormalization weights are updated
-        using the Cholesky decomposition. The output tensor is returned.
+        using the QR decomposition. The output tensor is returned.
         """
 
         for layer in self.layers:
             x = layer(x)
 
         Y_tilde = x
         if should_update_orth_weights:
             self.orthonorm_weights = self._make_orthonorm_weights(Y_tilde)
 
-        Y = torch.mm(Y_tilde, self.orthonorm_weights)
+        Y = Y_tilde @ self.orthonorm_weights
         return Y
```

### Comparing `spectralnet-0.0.3/src/spectralnet/_spectral.py` & `spectralnet-0.0.4/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.4/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import torch
 import torch.nn as nn
 import torch.optim as optim
 
+from tqdm import trange
 from ._trainer import Trainer
 from .._models import AEModel
 from torch.utils.data import DataLoader, random_split
 
 
 class AETrainer:
     def __init__(self, config: dict, device: torch.device):
@@ -38,15 +39,16 @@
         if os.path.exists(self.weights_path):
             self.ae_net.load_state_dict(torch.load(self.weights_path))
             return self.ae_net
 
         train_loader, valid_loader = self._get_data_loader()
 
         print("Training Autoencoder:")
-        for epoch in range(self.epochs):
+        t = trange(self.epochs, leave=True)
+        for epoch in t:
             train_loss = 0.0
             for batch_x in train_loader:
                 batch_x = batch_x.to(self.device)
                 batch_x = batch_x.view(batch_x.size(0), -1)
                 self.optimizer.zero_grad()
                 output = self.ae_net(batch_x)
                 loss = self.criterion(output, batch_x)
@@ -57,19 +59,21 @@
             train_loss /= len(train_loader)
             valid_loss = self.validate(valid_loader)
             self.scheduler.step(valid_loss)
             current_lr = self.optimizer.param_groups[0]["lr"]
 
             if current_lr <= self.min_lr:
                 break
-            print(
-                "Epoch: {}/{}, Train Loss: {:.4f}, Valid Loss: {:.4f}, LR: {:.6f}".format(
-                    epoch + 1, self.epochs, train_loss, valid_loss, current_lr
+
+            t.set_description(
+                "Train Loss: {:.7f}, Valid Loss: {:.7f}, LR: {:.6f}".format(
+                    train_loss, valid_loss, current_lr
                 )
             )
+            t.refresh()
 
         return self.ae_net
 
     def validate(self, valid_loader: DataLoader) -> float:
         self.ae_net.eval()
         valid_loss = 0.0
         with torch.no_grad():
```

### Comparing `spectralnet-0.0.3/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.4/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import torch
 import numpy as np
 import torch.optim as optim
 
-
+from tqdm import trange
 from annoy import AnnoyIndex
 from sklearn.neighbors import NearestNeighbors
 from torch.utils.data import DataLoader, random_split
 
 from ._trainer import Trainer
 from .._models import SiameseNetModel
 from .._losses import ContrastiveLoss
@@ -69,16 +69,17 @@
         if os.path.exists(self.weights_path):
             self.siamese_net.load_state_dict(torch.load(self.weights_path))
             return self.siamese_net
 
         train_loader, valid_loader = self._get_data_loader()
 
         print("Training Siamese Network:")
+        t = trange(self.epochs, leave=True)
         self.siamese_net.train()
-        for epoch in range(self.epochs):
+        for epoch in t:
             train_loss = 0.0
             for x1, x2, label in train_loader:
                 x1 = x1.to(self.device)
                 x1 = x1.view(x1.size(0), -1)
                 x2 = x2.to(self.device)
                 x2 = x2.view(x2.size(0), -1)
                 label = label.to(self.device)
@@ -92,19 +93,20 @@
             train_loss /= len(train_loader)
             valid_loss = self.validate(valid_loader)
             self.scheduler.step(valid_loss)
             current_lr = self.optimizer.param_groups[0]["lr"]
 
             if current_lr <= self.min_lr:
                 break
-            print(
-                "Epoch: {}/{}, Train Loss: {:.4f}, Valid Loss: {:.4f}, LR: {:.6f}".format(
-                    epoch + 1, self.epochs, train_loss, valid_loss, current_lr
+            t.set_description(
+                "Train Loss: {:.7f}, Valid Loss: {:.7f}, LR: {:.6f}".format(
+                    train_loss, valid_loss, current_lr
                 )
             )
+            t.refresh()
 
         return self.siamese_net
 
     def validate(self, valid_loader: DataLoader) -> float:
         valid_loss = 0.0
         self.siamese_net.eval()
         with torch.no_grad():
```

### Comparing `spectralnet-0.0.3/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.4/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 import torch.nn as nn
 import torch.optim as optim
 from torch.utils.data import DataLoader, random_split, TensorDataset
 
+from tqdm import trange
 from spectralnet._utils import *
 from ._trainer import Trainer
 from .._losses import SpectralNetLoss
 from .._models import SpectralNetModel
 
 
 class SpectralTrainer:
@@ -89,15 +90,16 @@
         self.scheduler = optim.lr_scheduler.ReduceLROnPlateau(
             self.optimizer, mode="min", factor=self.lr_decay, patience=self.patience
         )
 
         train_loader, ortho_loader, valid_loader = self._get_data_loader()
 
         print("Training SpectralNet:")
-        for epoch in range(self.epochs):
+        t = trange(self.epochs, leave=True)
+        for epoch in t:
             train_loss = 0.0
             for (X_grad, _), (X_orth, _) in zip(train_loader, ortho_loader):
                 X_grad = X_grad.to(device=self.device)
                 X_grad = X_grad.view(X_grad.size(0), -1)
                 X_orth = X_orth.to(device=self.device)
                 X_orth = X_orth.view(X_orth.size(0), -1)
 
@@ -130,19 +132,20 @@
             # Validation step
             valid_loss = self.validate(valid_loader)
             self.scheduler.step(valid_loss)
 
             current_lr = self.optimizer.param_groups[0]["lr"]
             if current_lr <= self.spectral_config["min_lr"]:
                 break
-            print(
-                "Epoch: {}/{}, Train Loss: {:.7f}, Valid Loss: {:.7f}, LR: {:.6f}".format(
-                    epoch + 1, self.epochs, train_loss, valid_loss, current_lr
+            t.set_description(
+                "Train Loss: {:.7f}, Valid Loss: {:.7f}, LR: {:.6f}".format(
+                    train_loss, valid_loss, current_lr
                 )
             )
+            t.refresh()
 
         return self.spectral_net
 
     def validate(self, valid_loader: DataLoader) -> float:
         valid_loss = 0.0
         self.spectral_net.eval()
         with torch.no_grad():
@@ -160,14 +163,16 @@
 
                 W = self._get_affinity_matrix(X)
 
                 loss = self.criterion(W, Y)
                 valid_loss += loss.item()
 
         self.counter += 1
+        if self.counter % 10 == 0:
+            plot_laplacian_eigenvectors(Y, y)
 
         valid_loss /= len(valid_loader)
         return valid_loss
 
     def _get_affinity_matrix(self, X: torch.Tensor) -> torch.Tensor:
         """
         This function computes the affinity matrix W using the Gaussian kernel.
```

### Comparing `spectralnet-0.0.3/src/spectralnet/_utils.py` & `spectralnet-0.0.4/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.3/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.0.4/src/spectralnet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,28 +13,28 @@
 License-File: LICENSE.md
 
 # SpectralNet
 
 <p align="center">
     <img src="https://github.com/AmitaiYacobi/SpectralNet01/blob/main/figures/twomoons.png">
 
-SpectralNet is a python package that performs spectral clustering with deep neural networks.<br><br>
+SpectralNet is a Python package that performs spectral clustering with deep neural networks.<br><br>
 This package is based on the following paper - [SpectralNet](https://openreview.net/pdf?id=HJ_aoCyRZ)
 
 ## Installation
 
 You can install the latest package version via
 
 ```bash
 pip install spectralnet
 ```
 
 ## Usage
 
-The basic functionlaity is quite intuitive and easy to use, e.g.,
+The basic functionality is quite intuitive and easy to use, e.g.,
 
 ```python
 from spectralnet import SpectralNet
 
 spectralnet = SpectralNet(n_clusters=10)
 spectralnet.fit(X) # X is the dataset and it should be a torch.Tensor
 cluster_assignments = spectralnet.predict(X) # Get the final assignments to clusters
```

### Comparing `spectralnet-0.0.3/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.4/src/spectralnet.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -18,8 +18,10 @@
 src/spectralnet/_models/_ae_model.py
 src/spectralnet/_models/_siamesenet_model.py
 src/spectralnet/_models/_spectralnet_model.py
 src/spectralnet/_trainers/__init__.py
 src/spectralnet/_trainers/_ae_trainer.py
 src/spectralnet/_trainers/_siamesenet_trainer.py
 src/spectralnet/_trainers/_spectralnet_trainer.py
-src/spectralnet/_trainers/_trainer.py
+src/spectralnet/_trainers/_trainer.py
+src/tests/__init__.py
+src/tests/test_twomoons.py
```

