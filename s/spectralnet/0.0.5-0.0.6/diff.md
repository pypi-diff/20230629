# Comparing `tmp/spectralnet-0.0.5.tar.gz` & `tmp/spectralnet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectralnet-0.0.5.tar", last modified: Thu Jun 29 18:49:42 2023, max compression
+gzip compressed data, was "spectralnet-0.0.6.tar", last modified: Thu Jun 29 19:01:27 2023, max compression
```

## Comparing `spectralnet-0.0.5.tar` & `spectralnet-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.433954 spectralnet-0.0.5/
--rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.5/LICENSE.md
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 18:49:42.434099 spectralnet-0.0.5/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-29 14:42:02.000000 spectralnet-0.0.5/README.md
--rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.5/pyproject.toml
--rw-r--r--   0 amitai     (501) staff       (20)      619 2023-06-29 18:49:42.434462 spectralnet-0.0.5/setup.cfg
--rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.5/setup.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.427976 spectralnet-0.0.5/src/
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.430116 spectralnet-0.0.5/src/spectralnet/
--rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/__init__.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.431636 spectralnet-0.0.5/src/spectralnet/_losses/
--rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/_siamese_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_losses/_spectralnet_loss.py
--rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_metrics.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.432524 spectralnet-0.0.5/src/spectralnet/_models/
--rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_ae_model.py
--rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_siamesenet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_models/_spectralnet_model.py
--rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_spectral.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.433742 spectralnet-0.0.5/src/spectralnet/_trainers/
--rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/__init__.py
--rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_ae_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_siamesenet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_spectralnet_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_trainers/_trainer.py
--rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.5/src/spectralnet/_utils.py
-drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 18:49:42.430997 spectralnet-0.0.5/src/spectralnet.egg-info/
--rw-r--r--   0 amitai     (501) staff       (20)     2270 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/PKG-INFO
--rw-r--r--   0 amitai     (501) staff       (20)      823 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/SOURCES.txt
--rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/dependency_links.txt
--rw-r--r--   0 amitai     (501) staff       (20)       12 2023-06-29 18:49:42.000000 spectralnet-0.0.5/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.995085 spectralnet-0.0.6/
+-rw-r--r--   0 amitai     (501) staff       (20)     1082 2023-06-29 14:40:19.000000 spectralnet-0.0.6/LICENSE.md
+-rw-r--r--   0 amitai     (501) staff       (20)     2266 2023-06-29 19:01:27.995193 spectralnet-0.0.6/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)     1772 2023-06-29 14:42:02.000000 spectralnet-0.0.6/README.md
+-rw-r--r--   0 amitai     (501) staff       (20)      342 2023-06-29 14:42:18.000000 spectralnet-0.0.6/pyproject.toml
+-rw-r--r--   0 amitai     (501) staff       (20)      615 2023-06-29 19:01:27.995505 spectralnet-0.0.6/setup.cfg
+-rw-r--r--   0 amitai     (501) staff       (20)       38 2023-06-29 14:42:12.000000 spectralnet-0.0.6/setup.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.987843 spectralnet-0.0.6/src/
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.990848 spectralnet-0.0.6/src/spectralnet/
+-rw-r--r--   0 amitai     (501) staff       (20)      136 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/__init__.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.992757 spectralnet-0.0.6/src/spectralnet/_losses/
+-rw-r--r--   0 amitai     (501) staff       (20)       89 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1574 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/_siamese_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)      989 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_losses/_spectralnet_loss.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2795 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_metrics.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.993615 spectralnet-0.0.6/src/spectralnet/_models/
+-rw-r--r--   0 amitai     (501) staff       (20)      126 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     1522 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_ae_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)      835 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_siamesenet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     2603 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_models/_spectralnet_model.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9930 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_spectral.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.994753 spectralnet-0.0.6/src/spectralnet/_trainers/
+-rw-r--r--   0 amitai     (501) staff       (20)      133 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/__init__.py
+-rw-r--r--   0 amitai     (501) staff       (20)     3783 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_ae_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     9485 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_siamesenet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)     7941 2023-06-29 18:46:31.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_spectralnet_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)       52 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_trainers/_trainer.py
+-rw-r--r--   0 amitai     (501) staff       (20)    11012 2023-06-29 14:41:56.000000 spectralnet-0.0.6/src/spectralnet/_utils.py
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.992062 spectralnet-0.0.6/src/spectralnet.egg-info/
+-rw-r--r--   0 amitai     (501) staff       (20)     2266 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/PKG-INFO
+-rw-r--r--   0 amitai     (501) staff       (20)      845 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/SOURCES.txt
+-rw-r--r--   0 amitai     (501) staff       (20)        1 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/dependency_links.txt
+-rw-r--r--   0 amitai     (501) staff       (20)       18 2023-06-29 19:01:27.000000 spectralnet-0.0.6/src/spectralnet.egg-info/top_level.txt
+drwxr-xr-x   0 amitai     (501) staff       (20)        0 2023-06-29 19:01:27.994962 spectralnet-0.0.6/src/tests/
+-rw-r--r--   0 amitai     (501) staff       (20)        0 2023-06-29 18:58:30.000000 spectralnet-0.0.6/src/tests/__init__.py
```

### Comparing `spectralnet-0.0.5/LICENSE.md` & `spectralnet-0.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/PKG-INFO` & `spectralnet-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spectral Clustering Using Deep Neural Networks
-Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
+Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
-Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
+Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `spectralnet-0.0.5/README.md` & `spectralnet-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/setup.cfg` & `spectralnet-0.0.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = spectralnet
-version = 0.0.5
+version = 0.0.6
 author = Amitai
 description = Spectral Clustering Using Deep Neural Networks
 long_description = file: README.md
 long_description_content_type = text/markdown
-url = https://github.com/AmitaiYacobi/SpectralNet.git
+url = https://github.com/shaham-lab/SpectralNet.git
 project_urls = 
-	Bug Tracker = https://github.com/AmitaiYacobi/SpectralNet/issues
+	Bug Tracker = https://github.com/shaham-lab/SpectralNet/issues
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir =
```

### Comparing `spectralnet-0.0.5/src/spectralnet/_losses/_siamese_loss.py` & `spectralnet-0.0.6/src/spectralnet/_losses/_siamese_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_losses/_spectralnet_loss.py` & `spectralnet-0.0.6/src/spectralnet/_losses/_spectralnet_loss.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_metrics.py` & `spectralnet-0.0.6/src/spectralnet/_metrics.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_models/_ae_model.py` & `spectralnet-0.0.6/src/spectralnet/_models/_ae_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_models/_siamesenet_model.py` & `spectralnet-0.0.6/src/spectralnet/_models/_siamesenet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_models/_spectralnet_model.py` & `spectralnet-0.0.6/src/spectralnet/_models/_spectralnet_model.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_spectral.py` & `spectralnet-0.0.6/src/spectralnet/_spectral.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_trainers/_ae_trainer.py` & `spectralnet-0.0.6/src/spectralnet/_trainers/_ae_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_trainers/_siamesenet_trainer.py` & `spectralnet-0.0.6/src/spectralnet/_trainers/_siamesenet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_trainers/_spectralnet_trainer.py` & `spectralnet-0.0.6/src/spectralnet/_trainers/_spectralnet_trainer.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet/_utils.py` & `spectralnet-0.0.6/src/spectralnet/_utils.py`

 * *Files identical despite different names*

### Comparing `spectralnet-0.0.5/src/spectralnet.egg-info/PKG-INFO` & `spectralnet-0.0.6/src/spectralnet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: spectralnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spectral Clustering Using Deep Neural Networks
-Home-page: https://github.com/AmitaiYacobi/SpectralNet.git
+Home-page: https://github.com/shaham-lab/SpectralNet.git
 Author: Amitai
-Project-URL: Bug Tracker, https://github.com/AmitaiYacobi/SpectralNet/issues
+Project-URL: Bug Tracker, https://github.com/shaham-lab/SpectralNet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `spectralnet-0.0.5/src/spectralnet.egg-info/SOURCES.txt` & `spectralnet-0.0.6/src/spectralnet.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,8 +18,9 @@
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
```

