# Comparing `tmp/spectralnet-0.0.4.tar.gz` & `tmp/spectralnet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.4.tar", last modified: Thu Jun 29 14:34:23 2023, max compression
+gzip compressed data, was "spectralnet-0.0.5.tar", last modified: Thu Jun 29 18:49:42 2023, max compression
```

## Comparing `spectralnet-0.0.4.tar` & `spectralnet-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,33 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.901244 spectralnet-0.0.4/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-25 12:12:14.000000 spectralnet-0.0.4/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 14:34:23.901350 spectralnet-0.0.4/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-27 16:30:09.000000 spectralnet-0.0.4/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-27 10:10:06.000000 spectralnet-0.0.4/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-29 14:34:23.901660 spectralnet-0.0.4/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-27 11:38:50.000000 spectralnet-0.0.4/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.891526 spectralnet-0.0.4/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.893991 spectralnet-0.0.4/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-27 12:26:31.000000 spectralnet-0.0.4/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.895449 spectralnet-0.0.4/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-25 13:45:07.000000 spectralnet-0.0.4/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-25 17:02:04.000000 spectralnet-0.0.4/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-25 13:27:35.000000 spectralnet-0.0.4/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-25 17:05:52.000000 spectralnet-0.0.4/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.897030 spectralnet-0.0.4/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-25 13:44:44.000000 spectralnet-0.0.4/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-27 09:25:21.000000 spectralnet-0.0.4/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-25 17:56:01.000000 spectralnet-0.0.4/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:15:11.000000 spectralnet-0.0.4/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-26 12:24:44.000000 spectralnet-0.0.4/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.899206 spectralnet-0.0.4/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-25 17:49:01.000000 spectralnet-0.0.4/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:23:29.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:23:36.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     8022 2023-06-29 14:22:49.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-25 17:43:03.000000 spectralnet-0.0.4/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-25 17:04:22.000000 spectralnet-0.0.4/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.894751 spectralnet-0.0.4/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      872 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       18 2023-06-29 14:34:23.000000 spectralnet-0.0.4/src/spectralnet.egg-info/top_level.txt
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 14:34:23.900835 spectralnet-0.0.4/src/tests/
--rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 04:54:02.000000 spectralnet-0.0.4/src/tests/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 09:34:12.000000 spectralnet-0.0.4/src/tests/test_twomoons.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.433954 spectralnet-0.0.5/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.5/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 18:49:42.434099 spectralnet-0.0.5/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-29 14:42:02.000000 spectralnet-0.0.5/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.5/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-29 18:49:42.434462 spectralnet-0.0.5/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.5/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.427976 spectralnet-0.0.5/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.430116 spectralnet-0.0.5/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.431636 spectralnet-0.0.5/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.432524 spectralnet-0.0.5/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.433742 spectralnet-0.0.5/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.430997 spectralnet-0.0.5/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      823 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       12 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/top_level.txt
```

### Comparing `spectralnet-0.0.4/LICENSE.md` & `spectralnet-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/PKG-INFO` & `spectralnet-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spectralnet-0.0.4/README.md` & `spectralnet-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/setup.cfg` & `spectralnet-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = spectralnet
-version = 0.0.4
+version = 0.0.5
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/AmitaiYacobi/SpectralNet.git
 project_urls = 
 	Bug Tracker = https://github.com/AmitaiYacobi/SpectralNet/issues
```

### Comparing `spectralnet-0.0.4/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.5/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.5/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_metrics.py` & `spectralnet-0.0.5/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.5/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.5/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.5/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_spectral.py` & `spectralnet-0.0.5/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.5/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.5/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.5/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,14 @@
 
                 W = self._get_affinity_matrix(X)
 
                 loss = self.criterion(W, Y)
                 valid_loss += loss.item()
 
         self.counter += 1
-        if self.counter % 10 == 0:
-            plot_laplacian_eigenvectors(Y, y)
 
         valid_loss /= len(valid_loader)
         return valid_loss
 
     def _get_affinity_matrix(self, X: torch.Tensor) -> torch.Tensor:
         """
         This function computes the affinity matrix W using the Gaussian kernel.
```

### Comparing `spectralnet-0.0.4/src/spectralnet/_utils.py` & `spectralnet-0.0.5/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.4/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.0.5/src/spectralnet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Spectral Clustering Using Deep Neural Networks
 Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
 Author: Amitai
 Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `spectralnet-0.0.4/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.5/src/spectralnet.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -18,10 +18,8 @@
 src/spectralnet/_models/_ae_model.py
 src/spectralnet/_models/_siamesenet_model.py
 src/spectralnet/_models/_spectralnet_model.py
 src/spectralnet/_trainers/__init__.py
 src/spectralnet/_trainers/_ae_trainer.py
 src/spectralnet/_trainers/_siamesenet_trainer.py
 src/spectralnet/_trainers/_spectralnet_trainer.py
-src/spectralnet/_trainers/_trainer.py
-src/tests/__init__.py
-src/tests/test_twomoons.py
+src/spectralnet/_trainers/_trainer.py
```

