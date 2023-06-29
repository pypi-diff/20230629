# Comparing `tmp/nlp_service-1.4.3.tar.gz` & `tmp/nlp_service-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp_service-1.4.3.tar", max compression
+gzip compressed data, was "nlp_service-1.4.4.tar", max compression
```

## Comparing `nlp_service-1.4.3.tar` & `nlp_service-1.4.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1067 2023-06-07 09:28:54.184637 nlp_service-1.4.3/LICENSE
--rw-r--r--   0        0        0     8218 2023-06-07 09:28:54.184637 nlp_service-1.4.3/README.md
--rw-r--r--   0        0        0      226 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/__init__.py
--rw-r--r--   0        0        0       42 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/__main__.py
--rw-r--r--   0        0        0     2259 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/client.py
--rw-r--r--   0        0        0    10441 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/infersent.py
--rw-r--r--   0        0        0        0 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/py.typed
--rw-r--r--   0        0        0    15668 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/server.py
--rw-r--r--   0        0        0     9147 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/similarity.py
--rw-r--r--   0        0        0      344 2023-06-07 09:28:54.188637 nlp_service-1.4.3/nlp_service/typing.py
--rw-r--r--   0        0        0     1519 2023-06-07 09:29:21.228982 nlp_service-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     9983 1970-01-01 00:00:00.000000 nlp_service-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-29 13:28:53.760156 nlp_service-1.4.4/LICENSE
+-rw-r--r--   0        0        0     7699 2023-06-29 13:28:53.760156 nlp_service-1.4.4/README.md
+-rw-r--r--   0        0        0      226 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/__init__.py
+-rw-r--r--   0        0        0       42 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/__main__.py
+-rw-r--r--   0        0        0     2259 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/client.py
+-rw-r--r--   0        0        0    10441 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/infersent.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/py.typed
+-rw-r--r--   0        0        0    17139 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/server.py
+-rw-r--r--   0        0        0     9147 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/similarity.py
+-rw-r--r--   0        0        0      344 2023-06-29 13:28:53.760156 nlp_service-1.4.4/nlp_service/typing.py
+-rw-r--r--   0        0        0     1361 2023-06-29 13:29:21.196484 nlp_service-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0     9329 1970-01-01 00:00:00.000000 nlp_service-1.4.4/PKG-INFO
```

### Comparing `nlp_service-1.4.3/LICENSE` & `nlp_service-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.3/README.md` & `nlp_service-1.4.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,40 +10,30 @@
 
 In addition to the server, we also provide a client containing convenience functions.
 This makes it easier for python applications to interact with the gRPC server.
 We will discuss the client at the end of this README.
 
 ## Installation and Setup
 
-We are using [poetry](https://python-poetry.org) to manage the dependencies.
-For easier setup, we also provide a `Dockerfile` and a `docker-compose` specification.
+We are using `nix` and `poetry` to manage the dependencies.
+We will soon provide a pre-built docker image for simplify usage of the NLP service.
 
-### Docker-Compose (recommended)
-
-You first need to pull this repository.
-Then execute the following in the project directory:
+### Nix (recommended)
 
 ```sh
-docker-compose build cpu
-# OR, if you need extras:
-docker-compose build --build-arg EXTRAS="levenshtein transformers" cpu
-# Start the CPU-only container
-docker-compose up cpu
+nix run . -- "127.0.0.1:50100"
+# or alternatively
+nix develop -c poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
-In case you have a **CUDA-enabled GPU**, you can replace `cpu` with `cuda` in the above commands and make full use of your card for advanced models like BERT.
-
 ### Poetry (advanced)
 
 ```sh
 # The server dependencies are optional, thus they have to be installed explicitly.
-poetry install --extras server
-# To get startet, we recommend to use the default spacy model.
-# In case you are dealing with English texts, you can run.
-poetry run python -m spacy download core_en_web_lg
+poetry install --extras all
 # To run the server, you need to specify the address it should listen on.
 # In this example, it should liston on port 5678 on localhost.
 poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
 ## General Usage
```

### Comparing `nlp_service-1.4.3/nlp_service/client.py` & `nlp_service-1.4.4/nlp_service/client.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.3/nlp_service/infersent.py` & `nlp_service-1.4.4/nlp_service/infersent.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.3/nlp_service/server.py` & `nlp_service-1.4.4/nlp_service/server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,54 @@
 from __future__ import annotations
 
 import itertools
 import logging
+import tarfile
 import typing as t
+import urllib.request
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
+from pathlib import Path
 
 import arg_services
 import grpc
 import numpy as np
 import scipy.stats
 import spacy
 import typer
 from arg_services.nlp.v1 import nlp_pb2, nlp_pb2_grpc
 from mashumaro.mixins.dict import DataClassDictMixin
-from spacy.cli.download import download as spacy_download
+from rich.progress import Progress
+from spacy import about as spacy_about
+from spacy.cli.download import (
+    get_latest_version as spacy_get_latest_version,
+)
+from spacy.cli.download import (
+    get_model_filename as spacy_get_model_filename,
+)
 from spacy.language import Language as SpacyLanguage
 from spacy.tokens import Doc, DocBin
 from thinc.types import Floats1d as SpacyVector
 
 from nlp_service.similarity import SimilarityFactory as SimilarityFactory
 from nlp_service.typing import ArrayLike, NumpyMatrix, NumpyVector
 
 log = logging.getLogger(__name__)
 
+
+torch_device = "cpu"
+
+try:
+    from torch.cuda import is_available as is_cuda_available
+
+    torch_device = "cuda" if is_cuda_available() else "cpu"
+    print(f"Using torch device '{torch_device}'.")
+except ModuleNotFoundError:
+    log.info("'torch' not installed.")
+
 # https://spacy.io/usage/processing-pipelines#built-in
 spacy_components = (
     "tagger",
     "parser",
     "ner",
     "entity_linker",
     "entity_ruler",
@@ -106,19 +127,16 @@
 ] = {
     nlp_pb2.EmbeddingType.EMBEDDING_TYPE_SPACY: SpacyModel,
 }
 
 
 try:
     import torch
-    from torch.cuda import is_available as is_cuda_available
     from transformers import AutoModel, AutoTokenizer
 
-    torch_device = "cuda" if is_cuda_available() else "cpu"
-
     class TransformersModel(ModelBase):
         def __init__(self, model: EmbeddingModel):
             # Load model from HuggingFace Hub
             try:
                 self.tokenizer = AutoTokenizer.from_pretrained(
                     model.model_name, use_fast=True
                 )
@@ -159,15 +177,14 @@
 
 except ModuleNotFoundError:
     log.info("'transformers' not installed.")
 
 
 try:
     from sentence_transformers import SentenceTransformer
-    from torch.cuda import is_available as is_cuda_available
 
     class SentenceTransformersModel(ModelBase):
         def __init__(self, model: EmbeddingModel):
             self.model = SentenceTransformer(model.model_name, device=torch_device)
 
         def vector(self, text: str) -> SpacyVector:
             embeddings = t.cast(
@@ -181,34 +198,14 @@
     )
 
 except ModuleNotFoundError:
     log.info("'sentence-transformers' not installed.")
 
 
 try:
-    import tensorflow_hub as hub
-
-    class TensorflowHubModel(ModelBase):
-        def __init__(self, model: EmbeddingModel):
-            self.model: t.Any = hub.load(model.model_name)
-
-        def vector(self, text: str) -> SpacyVector:
-            embeddings: t.Sequence[t.Any] = self.model([text])
-
-            return embeddings[0].numpy()
-
-    embedding_map[nlp_pb2.EmbeddingType.EMBEDDING_TYPE_TENSORFLOW_HUB] = (
-        TensorflowHubModel
-    )
-
-except ModuleNotFoundError:
-    log.info("'tensorflow-hub' not installed.")
-
-
-try:
     import openai
 
     openai.api_key_path = "./openai_api_key.txt"
 
     class OpenaiModel(ModelBase):
         def __init__(self, model: EmbeddingModel):
             self.model_name: str = model.model_name
@@ -260,23 +257,72 @@
 
 SpacyKey = tuple[str, str, tuple[EmbeddingModel, ...]]
 SpacyCache = t.Tuple[SpacyLanguage, dict[str, Doc]]
 spacy_cache: dict[SpacyKey, SpacyCache] = {}
 model_cache: dict[EmbeddingModel, ModelBase] = {}
 
 
+class UrlReportHook:
+    def __init__(self, progress: Progress, name: str):
+        self.task = None
+        self.progress = progress
+        self.name = name
+
+    def __call__(self, block_num: int, block_size: int, total_size: int):
+        if self.task is None:
+            self.task = self.progress.add_task(
+                f"Downloading {self.name}...", total=total_size
+            )
+
+        downloaded = block_num * block_size
+
+        if downloaded < total_size:
+            self.progress.update(self.task, completed=downloaded)
+
+        if self.progress.finished:
+            self.task = None
+
+
+def get_tarfile_members(
+    tf: tarfile.TarFile, prefix: str
+) -> t.Generator[tarfile.TarInfo, None, None]:
+    prefix_len = len(prefix)
+
+    for member in tf.getmembers():
+        if member.path.startswith(prefix):
+            member.path = member.path[prefix_len:]
+            yield member
+
+
 def _load_spacy_model(name: t.Optional[str]) -> SpacyLanguage:
     if not name:
         return spacy.blank("en")
 
-    try:
-        return spacy.load(name)
-    except OSError:
-        spacy_download(name)
-        return spacy.load(name)
+    version = spacy_get_latest_version(name)
+    filename = spacy_get_model_filename(name, version, sdist=True)
+    versioned_name = f"{name}-{version}"
+    path = Path.home() / ".cache" / "nlp-service" / "spacy" / versioned_name
+    tmpfile = path.with_suffix(".tar.gz")
+
+    if not path.exists():
+        path.parent.mkdir(parents=True, exist_ok=True)
+        download_url = f"{spacy_about.__download_url__}/{filename}"
+        with Progress() as progress:
+            urllib.request.urlretrieve(
+                download_url, tmpfile, UrlReportHook(progress, versioned_name)
+            )
+
+        with tarfile.open(tmpfile, mode="r:gz") as tf:
+            member_prefix = f"{versioned_name}/{name}/{versioned_name}/"
+            members = get_tarfile_members(tf, member_prefix)
+            tf.extractall(path=path, members=members)
+
+        tmpfile.unlink()
+
+    return spacy.load(path)
 
 
 def _load_spacy(config: nlp_pb2.NlpConfig) -> SpacyCache:
     models = tuple(
         EmbeddingModel.from_protobuf(model) for model in config.embedding_models
     )
     key: SpacyKey = (
```

### Comparing `nlp_service-1.4.3/nlp_service/similarity.py` & `nlp_service-1.4.4/nlp_service/similarity.py`

 * *Files identical despite different names*

### Comparing `nlp_service-1.4.3/pyproject.toml` & `nlp_service-1.4.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlp-service"
-version = "1.4.3"
+version = "1.4.4"
 description = "Microservice for NLP tasks using gRPC"
 authors = ["Mirko Lenz <info@mirko-lenz.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://recap.uni-trier.de"
 repository = "https://github.com/recap-utr/nlp-service"
 packages = [{ include = "nlp_service" }]
@@ -12,42 +12,39 @@
 [tool.poetry.scripts]
 nlp-service = "nlp_service.server:app"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 numpy = "^1.23.5"
 scipy = "^1.10.1"
-spacy = "^3.5.3"
-arg-services = "^1.3.1"
+spacy = "^3.5.4"
+arg-services = "^1.4.0"
 nltk = "^3.8.1"
 nptyping = "^2.5.0"
-mashumaro = "^3.7"
-typer = ">=0.7.0, <1.0.0"
+mashumaro = "^3.8.1"
+typer = "^0.9.0"
 gensim = { version = "^4.3.1", optional = true }
-python-Levenshtein = { version = "^0.21.0", optional = true }
+python-Levenshtein = { version = "^0.21.1", optional = true }
 sentence-transformers = { version = "^2.2.2", optional = true }
-torch = { version = ">=1.13.1, <3.0", optional = true }
-transformers = { version = "^4.29.2", optional = true }
-tensorflow = { version = "^2.12.0", optional = true }
-tensorflow-hub = { version = "^0.13.0", optional = true }
+torch = { version = ">=2.0.0, !=2.0.1, <3.0", optional = true }
+transformers = { version = "^4.30.2", optional = true }
 openai = { version = "^0.27.8", optional = true }
+rich = "^13.4.2"
 
 [tool.poetry.extras]
 wmd = ["gensim"]
 levenshtein = ["python-Levenshtein"]
 sentence-transformers = ["sentence-transformers", "torch"]
 transformers = ["transformers", "torch"]
-tensorflow = ["tensorflow", "tensorflow-hub"]
 openai = ["openai"]
 all = [
     "gensim",
     "python-Levenshtein",
     "sentence-transformers",
     "transformers",
     "torch",
-    "tensorflow",
     "openai",
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nlp_service-1.4.3/PKG-INFO` & `nlp_service-1.4.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 Metadata-Version: 2.1
 Name: nlp-service
-Version: 1.4.3
+Version: 1.4.4
 Summary: Microservice for NLP tasks using gRPC
 Home-page: http://recap.uni-trier.de
 License: MIT
 Author: Mirko Lenz
 Author-email: info@mirko-lenz.de
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: levenshtein
 Provides-Extra: openai
 Provides-Extra: sentence-transformers
-Provides-Extra: tensorflow
 Provides-Extra: transformers
 Provides-Extra: wmd
-Requires-Dist: arg-services (>=1.3.1,<2.0.0)
+Requires-Dist: arg-services (>=1.4.0,<2.0.0)
 Requires-Dist: gensim (>=4.3.1,<5.0.0) ; extra == "wmd" or extra == "all"
-Requires-Dist: mashumaro (>=3.7,<4.0)
+Requires-Dist: mashumaro (>=3.8.1,<4.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0) ; extra == "openai" or extra == "all"
-Requires-Dist: python-Levenshtein (>=0.21.0,<0.22.0) ; extra == "levenshtein" or extra == "all"
+Requires-Dist: python-Levenshtein (>=0.21.1,<0.22.0) ; extra == "levenshtein" or extra == "all"
+Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "sentence-transformers" or extra == "all"
-Requires-Dist: spacy (>=3.5.3,<4.0.0)
-Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; extra == "tensorflow" or extra == "all"
-Requires-Dist: tensorflow-hub (>=0.13.0,<0.14.0) ; extra == "tensorflow"
-Requires-Dist: torch (>=1.13.1,<3.0) ; extra == "sentence-transformers" or extra == "transformers" or extra == "all"
-Requires-Dist: transformers (>=4.29.2,<5.0.0) ; extra == "transformers" or extra == "all"
-Requires-Dist: typer (>=0.7.0,<1.0.0)
+Requires-Dist: spacy (>=3.5.4,<4.0.0)
+Requires-Dist: torch (>=2.0.0,!=2.0.1,<3.0) ; extra == "sentence-transformers" or extra == "transformers" or extra == "all"
+Requires-Dist: transformers (>=4.30.2,<5.0.0) ; extra == "transformers" or extra == "all"
+Requires-Dist: typer (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/recap-utr/nlp-service
 Description-Content-Type: text/markdown
 
 # NLP Microservice
 
 The goal of this project is to provide a [gRPC](https://grpc.io) server for resource-heavy NLP tasks&mdash;for instance, computing vectors/embeddings for words or sentences.
 By using [protobuf](https://developers.google.com/protocol-buffers) internally, our NLP server provides native and strongly typed interfaces for many programming languages.
@@ -49,40 +47,30 @@
 
 In addition to the server, we also provide a client containing convenience functions.
 This makes it easier for python applications to interact with the gRPC server.
 We will discuss the client at the end of this README.
 
 ## Installation and Setup
 
-We are using [poetry](https://python-poetry.org) to manage the dependencies.
-For easier setup, we also provide a `Dockerfile` and a `docker-compose` specification.
+We are using `nix` and `poetry` to manage the dependencies.
+We will soon provide a pre-built docker image for simplify usage of the NLP service.
 
-### Docker-Compose (recommended)
-
-You first need to pull this repository.
-Then execute the following in the project directory:
+### Nix (recommended)
 
 ```sh
-docker-compose build cpu
-# OR, if you need extras:
-docker-compose build --build-arg EXTRAS="levenshtein transformers" cpu
-# Start the CPU-only container
-docker-compose up cpu
+nix run . -- "127.0.0.1:50100"
+# or alternatively
+nix develop -c poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
-In case you have a **CUDA-enabled GPU**, you can replace `cpu` with `cuda` in the above commands and make full use of your card for advanced models like BERT.
-
 ### Poetry (advanced)
 
 ```sh
 # The server dependencies are optional, thus they have to be installed explicitly.
-poetry install --extras server
-# To get startet, we recommend to use the default spacy model.
-# In case you are dealing with English texts, you can run.
-poetry run python -m spacy download core_en_web_lg
+poetry install --extras all
 # To run the server, you need to specify the address it should listen on.
 # In this example, it should liston on port 5678 on localhost.
 poetry run python -m nlp_service "127.0.0.1:50100"
 ```
 
 ## General Usage
```

