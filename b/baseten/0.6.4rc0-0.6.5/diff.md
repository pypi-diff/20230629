# Comparing `tmp/baseten-0.6.4rc0.tar.gz` & `tmp/baseten-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.6.4rc0.tar", max compression
+gzip compressed data, was "baseten-0.6.5.tar", max compression
```

## Comparing `baseten-0.6.4rc0.tar` & `baseten-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     5041 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/__init__.py
--rw-r--r--   0        0        0    29519 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/lib_support.py
--rw-r--r--   0        0        0    18670 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2847 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-06-07 21:52:49.966710 baseten-0.6.4rc0/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-06-07 21:52:49.970711 baseten-0.6.4rc0/pypi_readme.md
--rw-r--r--   0        0        0     1964 2023-06-07 21:54:36.531871 baseten-0.6.4rc0/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 baseten-0.6.4rc0/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/__init__.py
+-rw-r--r--   0        0        0    12867 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/common/__init__.py
+-rw-r--r--   0        0        0    29519 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-06-28 15:48:06.297290 baseten-0.6.5/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    18701 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2847 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-06-28 15:48:06.301290 baseten-0.6.5/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-06-28 15:48:06.305291 baseten-0.6.5/pypi_readme.md
+-rw-r--r--   0        0        0     1960 2023-06-28 15:48:56.101690 baseten-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 baseten-0.6.5/PKG-INFO
```

### Comparing `baseten-0.6.4rc0/baseten/__init__.py` & `baseten-0.6.5/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/baseten_deployed_model.py` & `baseten-0.6.5/baseten/baseten_deployed_model.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/cli.py` & `baseten-0.6.5/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/client_commands/baseten_cli.py` & `baseten-0.6.5/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/client_commands/dataset_cli.py` & `baseten-0.6.5/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/client_commands/finetuning_cli.py` & `baseten-0.6.5/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/client_commands/models_cli.py` & `baseten-0.6.5/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/client_commands/pretrained_cli.py` & `baseten-0.6.5/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/api.py` & `baseten-0.6.5/baseten/common/api.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/core.py` & `baseten-0.6.5/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/error_handler.py` & `baseten-0.6.5/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/files.py` & `baseten-0.6.5/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/lib_support.py` & `baseten-0.6.5/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/model_deployer.py` & `baseten-0.6.5/baseten/common/model_deployer.py`

 * *Files 0% similar despite different names*

```diff
@@ -265,14 +265,15 @@
         )
 
     if model_deployment_status not in [
         "MODEL_READY",
         "SCALED_TO_ZERO",
         "SCALING_FROM_ZERO",
         "MODEL_LOADING",
+        "MODEL_DEPLOY_FAILED",
     ]:
         return TryPatchDraftTrussResponse(
             succeeded=False,
             needs_full_deploy=True,
             model_version_info=dev_model_version_info,
             error_message=f"model {model_name} is not ready for patching.",
         )
```

### Comparing `baseten-0.6.4rc0/baseten/common/settings.py` & `baseten-0.6.5/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/tar.py` & `baseten-0.6.5/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/types.py` & `baseten-0.6.5/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/common/util.py` & `baseten-0.6.5/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/models/flan_t5.py` & `baseten-0.6.5/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/models/llama.py` & `baseten-0.6.5/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/models/stable_diffusion.py` & `baseten-0.6.5/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/models/util.py` & `baseten-0.6.5/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/models/whisper.py` & `baseten-0.6.5/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/training/datasets.py` & `baseten-0.6.5/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/training/finetuning.py` & `baseten-0.6.5/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/baseten/training/logs.py` & `baseten-0.6.5/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/pypi_readme.md` & `baseten-0.6.5/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.6.4rc0/pyproject.toml` & `baseten-0.6.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.6.4rc0"
+version = "0.6.5"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
@@ -25,15 +25,15 @@
 coolname = ">=1.1.0"
 pyyaml = ">=5.1"
 tqdm = "^4.62.1"
 requests-toolbelt = "^0.9.1"
 tenacity = "^8.0.1"
 single-source = "^0.3.0"
 semantic-version = "^2.10.0"
-truss = "^0.4.8"
+truss = "0.4.9"
 Pillow = "^9.3.0"
 types-requests = "^2.28.11.7"
 types-setuptools = "^65.6.0.2"
 types-pillow = "^9.3.0.4"
 types-pyyaml = "^6.0.12.2"
 halo = "^0.0.31"
 types-pytz = "^2022.7.1.0"
```

### Comparing `baseten-0.6.4rc0/PKG-INFO` & `baseten-0.6.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.6.4rc0
+Version: 0.6.5
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -23,15 +23,15 @@
 Requires-Dist: pyyaml (>=5.1)
 Requires-Dist: requests (>=2.22)
 Requires-Dist: requests-toolbelt (>=0.9.1,<0.10.0)
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
 Requires-Dist: single-source (>=0.3.0,<0.4.0)
 Requires-Dist: tenacity (>=8.0.1,<9.0.0)
 Requires-Dist: tqdm (>=4.62.1,<5.0.0)
-Requires-Dist: truss (>=0.4.8,<0.5.0)
+Requires-Dist: truss (==0.4.9)
 Requires-Dist: types-pillow (>=9.3.0.4,<10.0.0.0)
 Requires-Dist: types-pytz (>=2022.7.1.0,<2023.0.0.0)
 Requires-Dist: types-pyyaml (>=6.0.12.2,<7.0.0.0)
 Requires-Dist: types-requests (>=2.28.11.7,<3.0.0.0)
 Requires-Dist: types-setuptools (>=65.6.0.2,<66.0.0.0)
 Project-URL: Documentation, https://docs.baseten.co
 Project-URL: Homepage, https://baseten.co
```

