# Comparing `tmp/spaces-0.3.0.tar.gz` & `tmp/spaces-0.4b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.3.0.tar", max compression
+gzip compressed data, was "spaces-0.4b1.tar", max compression
```

## Comparing `spaces-0.3.0.tar` & `spaces-0.4b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.3.0/README.md
--rw-r--r--   0        0        0     1490 2023-06-19 14:28:05.760905 spaces-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.3.0/spaces/__init__.py
--rw-r--r--   0        0        0      453 2023-06-19 14:01:43.384427 spaces-0.3.0/spaces/config.py
--rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.3.0/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     1589 2023-06-19 13:46:27.461593 spaces-0.3.0/spaces/gpu/client.py
--rw-r--r--   0        0        0      662 2023-06-19 13:47:01.122285 spaces-0.3.0/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3555 2023-06-02 18:22:00.557437 spaces-0.3.0/spaces/gpu/torch.py
--rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.3.0/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0      690 2023-06-01 15:35:22.446266 spaces-0.3.0/spaces/gradio.py
--rw-r--r--   0        0        0     1332 2023-06-19 14:10:55.323758 spaces-0.3.0/spaces/utils.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.3.0/setup.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.4b1/README.md
+-rw-r--r--   0        0        0     1489 2023-06-29 15:26:22.992172 spaces-0.4b1/pyproject.toml
+-rw-r--r--   0        0        0      168 2023-05-23 16:06:07.578194 spaces-0.4b1/spaces/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-19 14:01:43.384427 spaces-0.4b1/spaces/config.py
+-rw-r--r--   0        0        0      259 2023-05-30 12:29:38.149333 spaces-0.4b1/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-29 12:42:06.802062 spaces-0.4b1/spaces/gpu/client.py
+-rw-r--r--   0        0        0      711 2023-06-29 12:39:51.539671 spaces-0.4b1/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3581 2023-06-29 12:16:02.996586 spaces-0.4b1/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     6753 2023-06-02 18:54:45.252087 spaces-0.4b1/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0      690 2023-06-01 15:35:22.446266 spaces-0.4b1/spaces/gradio.py
+-rw-r--r--   0        0        0     1332 2023-06-19 14:10:55.323758 spaces-0.4b1/spaces/utils.py
+-rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 spaces-0.4b1/setup.py
+-rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 spaces-0.4b1/PKG-INFO
```

### Comparing `spaces-0.3.0/pyproject.toml` & `spaces-0.4b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.3.0"
+version = "0.4b1"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
 
@@ -19,16 +19,16 @@
 pytest = "^7.3.1"
 pytest-dotenv = "^0.5.2"
 pytest-mock = "^3.10.0"
 requests-mock = "^1.10.0"
 pytest-timeout = "^2.1.0"
 poethepoet = "^0.20.0"
 coverage = "^7.2.6"
-pytest-ordering = "^0.6"
 pyright = "^1.1.311"
+pytest-order = "^1.1.0"
 
 [tool.poetry.group.test.dependencies]
 diffusers = "^0.16.1"
 transformers = "^4.29.1"
 accelerate = "^0.19.0"
 xformers = "^0.0.19"
```

### Comparing `spaces-0.3.0/spaces/gpu/client.py` & `spaces-0.4b1/spaces/gpu/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 """
+from __future__ import annotations
 
 from http import HTTPStatus
 
 import requests
 from pydantic import BaseModel
 
 from .. import utils
@@ -27,16 +28,22 @@
 
 
 def base_url() -> str:
     assert Config.zero_device_api_url is not None
     return Config.zero_device_api_url
 
 
-def post(path: str, params: BaseModel) -> requests.Response:
-    return requests.post(base_url() + path, params=params.dict())
+def post(path: str, params: BaseModel | None = None) -> requests.Response:
+    return requests.post(base_url() + path, params=params.dict() if params else None)
+
+
+def startup_report():
+    res = post('/startup-report')
+    if res.status_code != HTTPStatus.OK: # pragma: no cover
+        raise RuntimeError("Error while initializing ZeroGPU")
 
 
 def schedule() -> ScheduleResponse:
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
     ))
```

### Comparing `spaces-0.3.0/spaces/gpu/decorator.py` & `spaces-0.4b1/spaces/gpu/decorator.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """
 from __future__ import annotations
 
 import inspect
 from typing import Callable
 
 from ..utils import CallableT
+from . import client
 from .wrappers import regular_function_wrapper
 from .wrappers import generator_function_wrapper
 
 
 already_decorated: set[Callable] = set()
 
 
@@ -22,10 +23,11 @@
         raise NotImplementedError
 
     if inspect.isgeneratorfunction(task):
         decorated = generator_function_wrapper(task)
     else:
         decorated = regular_function_wrapper(task)
 
+    client.startup_report()
     already_decorated.add(decorated)
 
     return decorated # type: ignore
```

### Comparing `spaces-0.3.0/spaces/gpu/torch.py` & `spaces-0.4b1/spaces/gpu/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                 device='cuda',
                 dtype=dtype,
                 memory_format=memory_format,
             ) # type: ignore
         for op in cuda_ops:
             tensor = op
             tensor.data = _tensor_cuda(tensor)
+        torch.cuda.init()
 
     def _is_in_bad_fork():
         with ProcessPoolExecutor(mp_context=multiprocessing.get_context('fork')) as e:
             f = e.submit(torch.cuda._is_in_bad_fork)
             return f.result()
 
     def _disable_cuda_intercept():
```

### Comparing `spaces-0.3.0/spaces/gpu/wrappers.py` & `spaces-0.4b1/spaces/gpu/wrappers.py`

 * *Files identical despite different names*

### Comparing `spaces-0.3.0/spaces/gradio.py` & `spaces-0.4b1/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.3.0/spaces/utils.py` & `spaces-0.4b1/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.3.0/setup.py` & `spaces-0.4b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.3.0',
+    'version': '0.4b1',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.3.0/PKG-INFO` & `spaces-0.4b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.3.0
+Version: 0.4b1
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

