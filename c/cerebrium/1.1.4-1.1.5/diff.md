# Comparing `tmp/cerebrium-1.1.4.tar.gz` & `tmp/cerebrium-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.4.tar", max compression
+gzip compressed data, was "cerebrium-1.1.5.tar", max compression
```

## Comparing `cerebrium-1.1.4.tar` & `cerebrium-1.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    34594 2023-06-28 15:08:02.800964 cerebrium-1.1.4/LICENSE
--rw-r--r--   0        0        0     3473 2023-06-28 15:08:02.800964 cerebrium-1.1.4/README.md
--rw-r--r--   0        0        0      381 2023-06-28 15:12:01.841640 cerebrium-1.1.4/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    21379 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/cli.py
--rw-r--r--   0        0        0    31606 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/conduit.py
--rw-r--r--   0        0        0     5050 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/errors.py
--rw-r--r--   0        0        0    11300 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/flow.py
--rw-r--r--   0        0        0     2777 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3798 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      914 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/base.py
--rw-r--r--   0        0        0      447 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      419 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1118 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      150 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      344 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8753 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/requests.py
--rw-r--r--   0        0        0     5297 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/README.md
--rw-r--r--   0        0        0        0 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/__init__.py
--rw-r--r--   0        0        0     9013 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/fine_tuner.py
--rw-r--r--   0        0        0     1520 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/finetuning_model.py
--rw-r--r--   0        0        0        0 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/__init__.py
--rw-r--r--   0        0        0     2703 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/base_dataset.py
--rw-r--r--   0        0        0     3750 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/data_validator.py
--rw-r--r--   0        0        0     2007 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/README.md
--rw-r--r--   0        0        0      530 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/alpaca.json
--rw-r--r--   0        0        0      269 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/alpaca_short.json
--rw-r--r--   0        0        0      597 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/vigogne.json
--rw-r--r--   0        0        0      466 2023-06-28 15:08:02.800964 cerebrium-1.1.4/cerebrium/utils.py
--rw-r--r--   0        0        0     2611 2023-06-28 15:12:01.837640 cerebrium-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 cerebrium-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-29 19:53:05.814995 cerebrium-1.1.5/LICENSE
+-rw-r--r--   0        0        0     3473 2023-06-29 19:53:05.814995 cerebrium-1.1.5/README.md
+-rw-r--r--   0        0        0      381 2023-06-29 19:58:27.716272 cerebrium-1.1.5/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    21379 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/cli.py
+-rw-r--r--   0        0        0    31606 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5050 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/errors.py
+-rw-r--r--   0        0        0    11300 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/flow.py
+-rw-r--r--   0        0        0     2777 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3798 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      914 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/base.py
+-rw-r--r--   0        0        0      447 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      419 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1118 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      150 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      344 2023-06-29 19:53:05.814995 cerebrium-1.1.5/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8753 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/requests.py
+-rw-r--r--   0        0        0     5297 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/__init__.py
+-rw-r--r--   0        0        0     9013 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/fine_tuner.py
+-rw-r--r--   0        0        0     1520 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/finetuning_model.py
+-rw-r--r--   0        0        0        0 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/__init__.py
+-rw-r--r--   0        0        0     2703 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/base_dataset.py
+-rw-r--r--   0        0        0     3750 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/data_validator.py
+-rw-r--r--   0        0        0     2007 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/README.md
+-rw-r--r--   0        0        0      530 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/alpaca.json
+-rw-r--r--   0        0        0      269 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/alpaca_short.json
+-rw-r--r--   0        0        0      597 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/vigogne.json
+-rw-r--r--   0        0        0      466 2023-06-29 19:53:05.818995 cerebrium-1.1.5/cerebrium/utils.py
+-rw-r--r--   0        0        0     2634 2023-06-29 19:58:27.712272 cerebrium-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     5661 1970-01-01 00:00:00.000000 cerebrium-1.1.5/PKG-INFO
```

### Comparing `cerebrium-1.1.4/LICENSE` & `cerebrium-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/README.md` & `cerebrium-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/cli.py` & `cerebrium-1.1.5/cerebrium/cli.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/conduit.py` & `cerebrium-1.1.5/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/core.py` & `cerebrium-1.1.5/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/errors.py` & `cerebrium-1.1.5/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/flow.py` & `cerebrium-1.1.5/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/logging/arize.py` & `cerebrium-1.1.5/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/logging/base.py` & `cerebrium-1.1.5/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/logging/censius.py` & `cerebrium-1.1.5/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/models/base.py` & `cerebrium-1.1.5/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/models/sklearn.py` & `cerebrium-1.1.5/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/requests.py` & `cerebrium-1.1.5/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/README.md` & `cerebrium-1.1.5/cerebrium/trainer/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/fine_tuner.py` & `cerebrium-1.1.5/cerebrium/trainer/fine_tuner.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/finetuning_model.py` & `cerebrium-1.1.5/cerebrium/trainer/finetuning_model.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/userDataset/base_dataset.py` & `cerebrium-1.1.5/cerebrium/trainer/userDataset/base_dataset.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/userDataset/data_validator.py` & `cerebrium-1.1.5/cerebrium/trainer/userDataset/data_validator.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/README.md` & `cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/alpaca.json` & `cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/alpaca.json`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/cerebrium/trainer/userDataset/templates/vigogne.json` & `cerebrium-1.1.5/cerebrium/trainer/userDataset/templates/vigogne.json`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.4/pyproject.toml` & `cerebrium-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.4"
+version = "1.1.5"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "webhook/*", "builder/*", "prebuilt/*", "common/*", "examples/*", "trainer/*"]
 
 [tool.poetry.urls]
@@ -49,14 +49,15 @@
 celery = { version = ">=5.2.0,<5.3.0", optional= true }
 accelerate = { version = ">=0.18.0,<0.19.0", optional= true }
 bitsandbytes = { version = ">=0.38.0,<0.39.0", optional= true }
 tensorflow = { version = ">=2.12.0", optional= true }
 typer = { version = "0.7.0", extras = ["all"] }
 keras = { version = ">=2.12.0", optional= true }
 xformers = { version = ">=0.0.16", optional= true }
+jsonschema = "^4.17.3"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<23.2"
 ipython = ">=8.9,<8.10"
 ipykernel = ">=6.21,<6.22"
 poetry-dotenv = "0.3.0"
 poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21,<0.22"}
```

### Comparing `cerebrium-1.1.4/PKG-INFO` & `cerebrium-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.4
+Version: 1.1.5
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -23,14 +23,15 @@
 Requires-Dist: celery (>=5.2.0,<5.3.0) ; extra == "worker"
 Requires-Dist: censius (>=1.6,<2.0)
 Requires-Dist: chitra (>=0.2.0,<0.3.0) ; extra == "worker"
 Requires-Dist: cloudpickle (>=2.0,<2.1)
 Requires-Dist: datadog (>=0.45.0,<0.51.0) ; extra == "worker"
 Requires-Dist: datasets (>=2.10.0,<2.11.0) ; extra == "worker"
 Requires-Dist: ddtrace (>=1.10.0,<1.11.0) ; extra == "worker"
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: keras (>=2.12.0) ; extra == "tensorflow"
 Requires-Dist: loguru (>=0.6) ; extra == "worker"
 Requires-Dist: numpy (>=1.20,<2.0)
 Requires-Dist: onnxruntime (>=1.13,<2.0) ; extra == "onnxruntime"
 Requires-Dist: onnxruntime-gpu (>=1.14,<2.0) ; extra == "onnxruntime-gpu"
 Requires-Dist: pandas (>=1.5,<3.0)
 Requires-Dist: requests (>=2.28,<3.0)
```

