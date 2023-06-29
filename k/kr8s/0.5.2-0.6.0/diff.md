# Comparing `tmp/kr8s-0.5.2.tar.gz` & `tmp/kr8s-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kr8s-0.5.2.tar", max compression
+gzip compressed data, was "kr8s-0.6.0.tar", max compression
```

## Comparing `kr8s-0.5.2.tar` & `kr8s-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,32 @@
--rw-r--r--   0        0        0     1549 2023-06-11 20:49:47.175779 kr8s-0.5.2/LICENSE
--rw-r--r--   0        0        0     2308 2023-06-11 20:49:47.175779 kr8s-0.5.2/README.md
--rw-r--r--   0        0        0      551 2023-06-11 20:50:18.911588 kr8s-0.5.2/kr8s/__init__.py
--rw-r--r--   0        0        0    10470 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_api.py
--rw-r--r--   0        0        0     5250 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_asyncio.py
--rw-r--r--   0        0        0     5854 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_auth.py
--rw-r--r--   0        0        0     1553 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_data_utils.py
--rw-r--r--   0        0        0      163 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_exceptions.py
--rw-r--r--   0        0        0    28114 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_objects.py
--rw-r--r--   0        0        0     7764 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_portforward.py
--rw-r--r--   0        0        0      680 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/_testutils.py
--rw-r--r--   0        0        0       30 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/asyncio/__init__.py
--rw-r--r--   0        0        0      992 2023-06-11 20:49:47.199779 kr8s-0.5.2/kr8s/asyncio/_api.py
--rw-r--r--   0        0        0      685 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/asyncio/objects.py
--rw-r--r--   0        0        0       50 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/asyncio/portforward.py
--rw-r--r--   0        0        0     5575 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/conftest.py
--rw-r--r--   0        0        0     5893 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/objects.py
--rw-r--r--   0        0        0      157 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/portforward.py
--rw-r--r--   0        0        0       61 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/resources/serviceaccount.yaml
--rwxr-xr-x   0        0        0      614 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/scripts/envexec.py
--rw-r--r--   0        0        0     4385 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_api.py
--rw-r--r--   0        0        0     3144 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_auth.py
--rw-r--r--   0        0        0      639 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_data_utils.py
--rw-r--r--   0        0        0    14477 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_objects.py
--rw-r--r--   0        0        0      622 2023-06-11 20:49:47.203779 kr8s-0.5.2/kr8s/tests/test_testutils.py
--rw-r--r--   0        0        0     2576 2023-06-11 20:50:18.911588 kr8s-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     3102 1970-01-01 00:00:00.000000 kr8s-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1549 2023-06-29 08:25:21.067652 kr8s-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2571 2023-06-29 08:25:21.067652 kr8s-0.6.0/README.md
+-rw-r--r--   0        0        0      541 2023-06-29 08:25:44.343775 kr8s-0.6.0/kr8s/__init__.py
+-rw-r--r--   0        0        0    10470 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_api.py
+-rw-r--r--   0        0        0     5879 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_auth.py
+-rw-r--r--   0        0        0     1920 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_data_utils.py
+-rw-r--r--   0        0        0      163 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_exceptions.py
+-rw-r--r--   0        0        0     4294 2023-06-29 08:25:21.087653 kr8s-0.6.0/kr8s/_io.py
+-rw-r--r--   0        0        0    30540 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_objects.py
+-rw-r--r--   0        0        0     7764 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_portforward.py
+-rw-r--r--   0        0        0      680 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/_testutils.py
+-rw-r--r--   0        0        0       30 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/__init__.py
+-rw-r--r--   0        0        0      992 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/_api.py
+-rw-r--r--   0        0        0      709 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/objects.py
+-rw-r--r--   0        0        0       50 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/asyncio/portforward.py
+-rw-r--r--   0        0        0     5575 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/conftest.py
+-rw-r--r--   0        0        0     6001 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/objects.py
+-rw-r--r--   0        0        0      152 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/portforward.py
+-rw-r--r--   0        0        0       78 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/custom/evc.yaml
+-rw-r--r--   0        0        0       61 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/serviceaccount.yaml
+-rw-r--r--   0        0        0      369 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nested/nginx_ingress.yaml
+-rw-r--r--   0        0        0      144 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nginx_pod.yaml
+-rw-r--r--   0        0        0      435 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/resources/simple/nginx_pod_service.yaml
+-rwxr-xr-x   0        0        0      614 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/scripts/envexec.py
+-rw-r--r--   0        0        0     4385 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_api.py
+-rw-r--r--   0        0        0     3402 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_auth.py
+-rw-r--r--   0        0        0      824 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_data_utils.py
+-rw-r--r--   0        0        0      643 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_io.py
+-rw-r--r--   0        0        0    15968 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_objects.py
+-rw-r--r--   0        0        0      622 2023-06-29 08:25:21.091653 kr8s-0.6.0/kr8s/tests/test_testutils.py
+-rw-r--r--   0        0        0     2564 2023-06-29 08:25:44.343775 kr8s-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3314 1970-01-01 00:00:00.000000 kr8s-0.6.0/PKG-INFO
```

### Comparing `kr8s-0.5.2/LICENSE` & `kr8s-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/README.md` & `kr8s-0.6.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,19 +6,57 @@
 [![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
 [![Kubernetes Version Support](https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue)](https://docs.kr8s.org/en/latest/installation.html#supported-kubernetes-versions)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
-> **Warning**
-> This is beta software and might not be ready for prime time.
+A simple, extensible Python client library for Kubernetes that feels familiar for folks who already know how to use `kubectl`.
 
-A Kubernetes API for Python
+## Highlights
 
-### History
+- API inspired by `kubectl` to reduce developer learning curve.
+- [Sensible defaults](https://docs.kr8s.org/en/latest/authentication.html) to reduce boiler plate.
+- No swagger generated code, human readable code only.
+- Supports both [async/await](https://docs.kr8s.org/en/latest/asyncio.html) and sync APIs.
+- [Client caching](https://docs.kr8s.org/en/latest/client.html#client-caching) to reduce passing API objects around.
+- Batteries included by providing useful utilities and methods inspired by `kubectl`.
 
-This project was originally spun out from [dask-kubernetes](https://github.com/dask/dask-kubernetes) which provides utilities for deploying [Dask](https://www.dask.org/) clusters on Kubernetes.
+## Quickstart
 
-The `dask-kubernetes` project used a mix of [kubernetes](https://github.com/kubernetes-client/python), [kubernetes-asyncio](https://github.com/tomplus/kubernetes_asyncio) and [pykube-ng](https://codeberg.org/hjacobs/pykube-ng) (and some subprocess calls to [kubectl](https://kubernetes.io/docs/reference/kubectl/)) to interact with the Kubernetes API. It also contained a whole load of glue code to work around missing features and get everything working together.
+### Installation
 
-To improve maintenance and code reuse `kr8s` was born to extract the Kubernetes library code in `dask-kubernetes` and replace it with something simpler and more complete. Thank you to everyone who contributed to `dask-kubernetes` and we hope you contribute to `kr8s` too.
+```console
+$ pip install kr8s
+```
+
+### Client API
+
+```python
+import kr8s
+
+api = kr8s.api()
+pods = api.get("pods")
+```
+
+See the [Client API docs](https://docs.kr8s.org/en/latest/client.html) for more examples.
+
+### Object API
+
+```python
+from kr8s.objects import Pod
+
+pod = Pod({
+        "apiVersion": "v1",
+        "kind": "Pod",
+        "metadata": {
+            "name": "my-pod",
+        },
+        "spec": {
+            "containers": [{"name": "pause", "image": "gcr.io/google_containers/pause",}]
+        },
+    })
+
+pod.create()
+```
+
+See the [Object API docs](https://docs.kr8s.org/en/latest/object.html) for more examples.
```

### Comparing `kr8s-0.5.2/kr8s/__init__.py` & `kr8s-0.6.0/kr8s/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 from functools import partial
 
 from ._api import ALL  # noqa
 from ._api import Api as _AsyncApi
-from ._asyncio import run_sync as _run_sync
-from ._asyncio import sync as _sync  # noqa
 from ._exceptions import NotFoundError  # noqa
+from ._io import run_sync as _run_sync
+from ._io import sync as _sync  # noqa
 from .asyncio import api as _api  # noqa
 
-__version__ = "0.5.2"
+__version__ = "0.6.0"
 
 
 @_sync
 class Api(_AsyncApi):
     __doc__ = _AsyncApi.__doc__
```

### Comparing `kr8s-0.5.2/kr8s/_api.py` & `kr8s-0.6.0/kr8s/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/_auth.py` & `kr8s-0.6.0/kr8s/_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import base64
 import json
 import os
 
-import aiofiles
-import aiofiles.os
+import anyio
 import yaml
 
-from ._asyncio import check_output
+from ._io import NamedTemporaryFile, check_output
 
 
 class KubeAuth:
     """Load kubernetes auth from kubeconfig, service account, or url."""
 
     def __init__(
         self,
         kubeconfig=None,
         url=None,
-        serviceaccount="/var/run/secrets/kubernetes.io/serviceaccount",
+        serviceaccount=None,
         namespace=None,
     ) -> None:
         self.server = None
         self.client_cert_file = None
         self.client_key_file = None
         self.server_ca_file = None
         self.token = None
         self.username = None
         self.password = None
         self.namespace = namespace
         self._context = None
         self._cluster = None
         self._user = None
-        self._serviceaccount = serviceaccount
-        self._kubeconfig = os.path.expanduser(
-            kubeconfig or os.environ.get("KUBECONFIG", "~/.kube/config")
+        self._serviceaccount = (
+            serviceaccount
+            if serviceaccount is not None
+            else "/var/run/secrets/kubernetes.io/serviceaccount"
         )
+        self._kubeconfig = kubeconfig or os.environ.get("KUBECONFIG", "~/.kube/config")
+
         if url:
             self.server = url
 
     def __await__(self):
         async def f():
             await self.reauthenticate()
             return self
@@ -53,17 +55,18 @@
         if self._kubeconfig is not False and not self.server:
             await self._load_kubeconfig()
         if not self.server:
             raise ValueError("Unable to find valid credentials")
 
     async def _load_kubeconfig(self) -> None:
         """Load kubernetes auth from kubeconfig."""
-        if not await aiofiles.os.path.isfile(self._kubeconfig):
+        self._kubeconfig = os.path.expanduser(self._kubeconfig)
+        if not os.path.exists(self._kubeconfig):
             return
-        async with aiofiles.open(self._kubeconfig, mode="r") as f:
+        async with await anyio.open_file(self._kubeconfig) as f:
             config = yaml.safe_load(await f.read())
         if "current-context" in config:
             [self._context] = [
                 c["context"]
                 for c in config["contexts"]
                 if c["name"] == config["current-context"]
             ]
@@ -101,52 +104,52 @@
             elif "clientCertificateData" in data and "clientKeyData" in data:
                 self._user["client-certificate-data"] = data["clientCertificateData"]
                 self._user["client-key-data"] = data["clientKeyData"]
             else:
                 raise KeyError(f"Did not find credentials in {command} output.")
 
         if "client-key-data" in self._user:
-            async with aiofiles.tempfile.NamedTemporaryFile(delete=False) as key_file:
-                await key_file.write(base64.b64decode(self._user["client-key-data"]))
-                await key_file.flush()
-                self.client_key_file = key_file.name
+            async with NamedTemporaryFile(delete=False) as key_file:
+                await key_file.write_bytes(
+                    base64.b64decode(self._user["client-key-data"])
+                )
+                self.client_key_file = str(key_file)
         if "client-certificate-data" in self._user:
-            async with aiofiles.tempfile.NamedTemporaryFile(delete=False) as cert_file:
-                await cert_file.write(
+            async with NamedTemporaryFile(delete=False) as cert_file:
+                await cert_file.write_bytes(
                     base64.b64decode(self._user["client-certificate-data"])
                 )
-                await cert_file.flush()
-                self.client_cert_file = cert_file.name
+                self.client_cert_file = str(cert_file)
         if "certificate-authority-data" in self._cluster:
-            async with aiofiles.tempfile.NamedTemporaryFile(delete=False) as ca_file:
-                await ca_file.write(
+            async with NamedTemporaryFile(delete=False) as ca_file:
+                await ca_file.write_bytes(
                     base64.b64decode(self._cluster["certificate-authority-data"])
                 )
-                await ca_file.flush()
-                self.server_ca_file = ca_file.name
+                self.server_ca_file = str(ca_file)
         if "token" in self._user:
             self.token = self._user["token"]
         if "username" in self._user:
             self.username = self._user["username"]
         if "password" in self._user:
             self.password = self._user["password"]
         if self.namespace is None:
             self.namespace = self._context.get("namespace", "default")
         # TODO: Handle auth-provider oidc auth
 
     async def _load_service_account(self) -> None:
         """Load credentials from service account."""
-        if not await aiofiles.os.path.isdir(self._serviceaccount):
+        self._serviceaccount = os.path.expanduser(self._serviceaccount)
+        if not os.path.isdir(self._serviceaccount):
             return
         host = os.environ["KUBERNETES_SERVICE_HOST"]
         port = os.environ["KUBERNETES_SERVICE_PORT"]
         self.server = f"https://{host}:{port}"
-        async with aiofiles.open(
-            os.path.join(self._serviceaccount, "token"), mode="r"
+        async with await anyio.open_file(
+            os.path.join(self._serviceaccount, "token")
         ) as f:
             self.token = await f.read()
         self.server_ca_file = os.path.join(self._serviceaccount, "ca.crt")
         if self.namespace is None:
-            async with aiofiles.open(
-                os.path.join(self._serviceaccount, "namespace"), mode="r"
+            async with await anyio.open_file(
+                os.path.join(self._serviceaccount, "namespace")
             ) as f:
                 self.namespace = await f.read()
```

### Comparing `kr8s-0.5.2/kr8s/_data_utils.py` & `kr8s-0.6.0/kr8s/_data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,7 +46,23 @@
     nested_dict = {}
     for key in reversed(keys):
         if not nested_dict:
             nested_dict[key] = value
         else:
             nested_dict = {key: nested_dict}
     return nested_dict
+
+
+def dict_to_selector(selector_dict: Dict) -> str:
+    """Convert a dictionary to a Kubernetes selector.
+
+    Parameters
+    ----------
+    selector_dict : Dict
+        The dictionary to convert to a Kubernetes selector.
+
+    Returns
+    -------
+    str
+        A Kubernetes selector string.
+    """
+    return ",".join(f"{k}={v}" for k, v in selector_dict.items())
```

### Comparing `kr8s-0.5.2/kr8s/_objects.py` & `kr8s-0.6.0/kr8s/_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 from __future__ import annotations
 
 import asyncio
 import json
+import pathlib
 import re
 import time
 from typing import Any, Dict, List, Optional, Type, Union
 
 import aiohttp
+import anyio
 import jsonpath
+import yaml
 from aiohttp import ClientResponse
-from async_timeout import timeout as async_timeout
 
 import kr8s
 import kr8s.asyncio
 from kr8s._api import Api
-from kr8s._data_utils import dot_to_nested_dict, list_dict_unpack
+from kr8s._data_utils import dict_to_selector, dot_to_nested_dict, list_dict_unpack
 from kr8s._exceptions import NotFoundError
 from kr8s.asyncio.portforward import PortForward as AsyncPortForward
 from kr8s.portforward import PortForward as SyncPortForward
 
 JSONPATH_CONDITION_EXPRESSION = r"jsonpath='{(?P<expression>.*?)}'=(?P<condition>.*)"
 
 
@@ -300,15 +302,15 @@
         return True
 
     async def wait(self, conditions: Union[List[str], str], timeout: int = None):
         """Wait for conditions to be met."""
         if isinstance(conditions, str):
             conditions = [conditions]
 
-        with async_timeout(timeout):
+        with anyio.fail_after(timeout):
             try:
                 await self._refresh()
             except NotFoundError:
                 if set(conditions) == {"delete"}:
                     return
             if await self._test_conditions(conditions):
                 return
@@ -653,21 +655,24 @@
 
     async def proxy_http_delete(
         self, path: str, port: Optional[int] = None, **kwargs
     ) -> None:
         return await self._proxy_http_request("DELETE", path, port, **kwargs)
 
     async def ready_pods(self) -> List[Pod]:
-        """Return a list of ready pods for this service."""
+        """Return a list of ready Pods for this Service."""
         return await self._ready_pods()
 
     async def _ready_pods(self) -> List[Pod]:
-        """Return a list of ready pods for this service."""
-        pod_selector = ",".join([f"{k}={v}" for k, v in self.labels.items()])
-        pods = await self.api._get("pods", label_selector=pod_selector)
+        """Return a list of ready Pods for this Service."""
+        pods = await self.api._get(
+            "pods",
+            label_selector=dict_to_selector(self.spec["selector"]),
+            namespace=self.namespace,
+        )
         return [pod for pod in pods if await pod.ready()]
 
     async def ready(self) -> bool:
         """Check if the service is ready."""
         pods = await self._ready_pods()
         return len(pods) > 0
 
@@ -732,14 +737,23 @@
     endpoint = "deployments"
     kind = "Deployment"
     plural = "deployments"
     singular = "deployment"
     namespaced = True
     scalable = True
 
+    async def pods(self) -> List[Pod]:
+        """Return a list of Pods for this Deployment."""
+        pods = await self.api._get(
+            "pods",
+            label_selector=dict_to_selector(self.spec["selector"]["matchLabels"]),
+            namespace=self.namespace,
+        )
+        return pods
+
     async def ready(self):
         """Check if the deployment is ready."""
         await self._refresh()
         return (
             self.raw["status"].get("observedGeneration", 0)
             >= self.raw["metadata"]["generation"]
             and self.raw["status"].get("readyReplicas", 0) == self.replicas
@@ -954,27 +968,66 @@
             and (version is None or cls.version == version)
             and cls._asyncio == _asyncio
         ):
             return cls
     raise KeyError(f"No object registered for {version}/{kind}")
 
 
-def object_from_spec(spec: dict, api: Api = None) -> APIObject:
+def new_class(
+    kind: str, version: str = None, asyncio: bool = True, namespaced=True
+) -> Type[APIObject]:
+    """Create a new APIObject subclass.
+
+    Args:
+        kind: The Kubernetes resource kind.
+        version: The Kubernetes API version.
+        asyncio: Whether to use asyncio or not.
+        namespaced: Whether the resource is namespaced or not.
+
+    Returns:
+        A new APIObject subclass.
+    """
+    if version is None:
+        version = "v1"
+    return type(
+        kind,
+        (APIObject,),
+        {
+            "kind": kind,
+            "version": version,
+            "_asyncio": asyncio,
+            "endpoint": kind.lower() + "s",
+            "plural": kind.lower() + "s",
+            "singular": kind.lower(),
+            "namespaced": namespaced,
+        },
+    )
+
+
+def object_from_spec(
+    spec: dict, api: Api = None, allow_unknown_type: bool = False
+) -> APIObject:
     """Create an APIObject from a Kubernetes resource spec.
 
     Args:
         spec: A Kubernetes resource spec.
 
     Returns:
         A corresponding APIObject subclass instance.
 
     Raises:
         ValueError: If the resource kind or API version is not supported.
     """
-    cls = get_class(spec["kind"], spec["apiVersion"])
+    try:
+        cls = get_class(spec["kind"], spec["apiVersion"])
+    except KeyError:
+        if allow_unknown_type:
+            cls = new_class(spec["kind"], spec["apiVersion"])
+        else:
+            raise
     return cls(spec, api=api)
 
 
 async def object_from_name_type(
     name: str, namespace: str = None, api: Api = None
 ) -> APIObject:
     """Create an APIObject from a Kubernetes resource name.
@@ -995,7 +1048,40 @@
         kind = resource_type.split(".")[0]
         version = ".".join(resource_type.split(".")[1:])
     else:
         kind = resource_type
         version = None
     cls = get_class(kind, version)
     return await cls.get(name, namespace=namespace, api=api)
+
+
+async def objects_from_files(
+    path: Union[str, pathlib.Path], api: Api = None, recursive: bool = False
+) -> List[APIObject]:
+    """Create APIObjects from Kubernetes resource files.
+
+    Args:
+        path: A path to a Kubernetes resource file or directory of resource files.
+        api: An optional API instance to use.
+        recursive: Whether to recursively search for resource files in subdirectories.
+
+    Returns:
+        A list of APIObject subclass instances.
+
+    Raises:
+        ValueError: If the resource kind or API version is not supported.
+    """
+    path = pathlib.Path(path)
+    if path.is_dir():
+        pattern = "**/*.yaml" if recursive else "*.yaml"
+        files = [f for f in path.glob(pattern) if f.is_file()]
+    else:
+        files = [path]
+    objects = []
+    for file in files:
+        with open(file, "r") as f:
+            for doc in yaml.safe_load_all(f):
+                if doc is not None:
+                    objects.append(
+                        object_from_spec(doc, api=api, allow_unknown_type=True)
+                    )
+    return objects
```

### Comparing `kr8s-0.5.2/kr8s/_portforward.py` & `kr8s-0.6.0/kr8s/_portforward.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/_testutils.py` & `kr8s-0.6.0/kr8s/_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/asyncio/_api.py` & `kr8s-0.6.0/kr8s/asyncio/_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/asyncio/objects.py` & `kr8s-0.6.0/kr8s/asyncio/objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,8 +32,9 @@
     RoleBinding,
     Secret,
     Service,
     ServiceAccount,
     StatefulSet,
     Table,
     object_from_name_type,
+    objects_from_files,
 )
```

### Comparing `kr8s-0.5.2/kr8s/conftest.py` & `kr8s-0.6.0/kr8s/conftest.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/objects.py` & `kr8s-0.6.0/kr8s/objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._asyncio import run_sync, sync
+from ._io import run_sync, sync
 from ._objects import (
     APIObject as _APIObject,
 )
 from ._objects import (
     Binding as _Binding,
 )
 from ._objects import (
@@ -103,19 +103,17 @@
 )
 from ._objects import (
     StatefulSet as _StatefulSet,
 )
 from ._objects import (
     Table as _Table,
 )
-from ._objects import (  # noqa
-    get_class,
-    object_from_spec,
-)
+from ._objects import get_class, new_class, object_from_spec  # noqa
 from ._objects import object_from_name_type as _object_from_name_type
+from ._objects import objects_from_files as _objects_from_files
 
 
 @sync
 class APIObject(_APIObject):
     __doc__ = _APIObject.__doc__
     _asyncio = False
 
@@ -327,7 +325,8 @@
 @sync
 class Table(_Table):
     __doc__ = _Table.__doc__
     _asyncio = False
 
 
 object_from_name_type = run_sync(_object_from_name_type)
+objects_from_files = run_sync(_objects_from_files)
```

### Comparing `kr8s-0.5.2/kr8s/tests/scripts/envexec.py` & `kr8s-0.6.0/kr8s/tests/scripts/envexec.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/tests/test_api.py` & `kr8s-0.6.0/kr8s/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/kr8s/tests/test_auth.py` & `kr8s-0.6.0/kr8s/tests/test_auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,22 @@
 
 async def test_kubeconfig(k8s_cluster):
     kubernetes = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
     version = await kubernetes.version()
     assert "major" in version
 
 
+async def test_default_service_account(k8s_cluster):
+    kubernetes = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
+    assert (
+        str(kubernetes.auth._serviceaccount)
+        == "/var/run/secrets/kubernetes.io/serviceaccount"
+    )
+
+
 async def test_reauthenticate(k8s_cluster):
     kubernetes = await kr8s.asyncio.api(kubeconfig=k8s_cluster.kubeconfig_path)
     await kubernetes.reauthenticate()
     version = await kubernetes.version()
     assert "major" in version
```

### Comparing `kr8s-0.5.2/kr8s/tests/test_objects.py` & `kr8s-0.6.0/kr8s/tests/test_objects.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 # SPDX-FileCopyrightText: Copyright (c) 2023, Dask Developers, Yuvi Panda, Anaconda Inc, NVIDIA
 # SPDX-License-Identifier: BSD 3-Clause License
 import asyncio
+import pathlib
 import time
 
 import aiohttp
 import pytest
 
 import kr8s
 from kr8s.asyncio.objects import (
     APIObject,
     Deployment,
+    Ingress,
     PersistentVolume,
     Pod,
     Service,
     object_from_name_type,
+    objects_from_files,
 )
 from kr8s.asyncio.portforward import PortForward
 from kr8s.objects import Pod as SyncPod
 from kr8s.objects import get_class, object_from_spec
 
 DEFAULT_TIMEOUT = aiohttp.ClientTimeout(30)
+CURRENT_DIR = pathlib.Path(__file__).parent
 
 
 @pytest.fixture
 async def nginx_pod(k8s_cluster, example_pod_spec):
     example_pod_spec["metadata"]["name"] = (
         "nginx-" + example_pod_spec["metadata"]["name"]
     )
@@ -95,15 +99,15 @@
     await pod.delete()
 
 
 async def test_pod_wait_ready(example_pod_spec):
     pod = await Pod(example_pod_spec)
     await pod.create()
     await pod.wait("condition=Ready")
-    with pytest.raises(asyncio.TimeoutError):
+    with pytest.raises(TimeoutError):
         await pod.wait("jsonpath='{.status.phase}'=Foo", timeout=0.1)
     await pod.wait("condition=Ready=true")
     await pod.wait("condition=Ready=True")
     await pod.wait("jsonpath='{.status.phase}'=Running")
     with pytest.raises(ValueError):
         await pod.wait("foo=NotARealCondition")
     await pod.delete()
@@ -111,15 +115,15 @@
     await pod.wait("delete")
 
 
 def test_pod_wait_ready_sync(example_pod_spec):
     pod = SyncPod(example_pod_spec)
     pod.create()
     pod.wait("condition=Ready")
-    with pytest.raises(asyncio.TimeoutError):
+    with pytest.raises(TimeoutError):
         pod.wait("jsonpath='{.status.phase}'=Foo", timeout=0.1)
     pod.wait("condition=Ready=true")
     pod.wait("condition=Ready=True")
     pod.wait("jsonpath='{.status.phase}'=Running")
     with pytest.raises(ValueError):
         pod.wait("foo=NotARealCondition")
     pod.delete()
@@ -329,14 +333,16 @@
     deployment = await Deployment(example_deployment_spec)
     await deployment.create()
     assert deployment.replicas == 1
     await deployment.scale(2)
     assert deployment.replicas == 2
     while not await deployment.ready():
         await asyncio.sleep(0.1)
+    pods = await deployment.pods()
+    assert len(pods) == 2
     await deployment.scale(1)
     assert deployment.replicas == 1
     await deployment.delete()
 
 
 async def test_node():
     kubernetes = await kr8s.asyncio.api()
@@ -449,7 +455,50 @@
         singular = "foo"
         namespaced = True
         scalable = True
         scalable_spec = "nested.replicas"
 
     foo = await Foo({"metadata": {"name": "foo"}, "spec": {"nested": {"replicas": 1}}})
     assert foo.replicas == 1
+
+
+async def test_object_from_file():
+    api = await kr8s.asyncio.api()
+    objects = await objects_from_files(
+        CURRENT_DIR / "resources" / "simple" / "nginx_pod.yaml", api=api
+    )
+    assert len(objects) == 1
+    assert isinstance(objects[0], Pod)
+    assert objects[0].kind == "Pod"
+    assert objects[0].name == "nginx"
+    assert len(objects[0].spec["containers"]) == 1
+
+
+async def test_objects_from_file():
+    objects = await objects_from_files(
+        CURRENT_DIR / "resources" / "simple" / "nginx_pod_service.yaml"
+    )
+    assert len(objects) == 2
+    assert isinstance(objects[0], Pod)
+    assert isinstance(objects[1], Service)
+
+
+async def test_objects_from_files():
+    simple_dir = CURRENT_DIR / "resources" / "simple"
+    objects = await objects_from_files(simple_dir)
+    assert len(objects) > 1
+
+
+async def test_objects_from_files_nested():
+    simple_dir = CURRENT_DIR / "resources" / "simple"
+
+    objects = await objects_from_files(simple_dir)
+    assert not any(isinstance(o, Ingress) for o in objects)
+
+    objects = await objects_from_files(simple_dir, recursive=True)
+    assert any(isinstance(o, Ingress) for o in objects)
+
+
+async def test_custom_object_from_file():
+    simple_dir = CURRENT_DIR / "resources" / "custom" / "evc.yaml"
+    objects = await objects_from_files(simple_dir)
+    assert len(objects) == 1
```

### Comparing `kr8s-0.5.2/kr8s/tests/test_testutils.py` & `kr8s-0.6.0/kr8s/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `kr8s-0.5.2/pyproject.toml` & `kr8s-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "aiohttp",
     'importlib-metadata; python_version<"3.8"',
 ]
 dynamic = ["version"]
 
 [tool.poetry]
 name = "kr8s"
-version = "0.5.2"  # This will be populated at build time by poetry-dynamic-versioning
+version = "0.6.0"  # This will be populated at build time by poetry-dynamic-versioning
 description = "A Kubernetes API library"
 authors = ["Jacob Tomlinson <jacob@tomlinson.email>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry-dynamic-versioning]
 enable = true
@@ -33,26 +33,26 @@
 files = ["kr8s/__init__.py"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.8.4"
 pyyaml = "^6.0"
 asyncio-atexit = "^1.0.1"
-aiofiles = "^23.1.0"
 python-jsonpath = "^0.7.1"
-async-timeout = "^4.0.2"
+anyio = "^3.7.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-asyncio = "^0.20.3"
 pytest-kind = {git = "https://codeberg.org/hjacobs/pytest-kind.git"}
 pytest-timeout = "^2.1.0"
 pytest-rerunfailures = "^11.1.2"
 pytest-cov = "^4.0.0"
+trio = "^0.22.0"
 
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.3.0"
 sphinx-autobuild = "^2021.3.14"
 myst-parser = "^1.0.0"
 furo = "^2023.3.27"
@@ -61,15 +61,15 @@
 sphinxcontrib-mermaid = "^0.8.1"
 sphinx-autoapi = "^2.1.0"
 
 [tool.pytest.ini_options]
 addopts = "-v --keep-cluster --durations=10 --cov=kr8s --cov-report term-missing --cov-report xml:coverage.xml"
 timeout = 300
 xfail_strict = true
-reruns = 1
+reruns = 3
 reruns_delay = 1
 asyncio_mode = "auto"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `kr8s-0.5.2/PKG-INFO` & `kr8s-0.6.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: kr8s
-Version: 0.5.2
+Version: 0.6.0
 Summary: A Kubernetes API library
 License: BSD-3-Clause
 Author: Jacob Tomlinson
 Author-email: jacob@tomlinson.email
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiofiles (>=23.1.0,<24.0.0)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: async-timeout (>=4.0.2,<5.0.0)
+Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncio-atexit (>=1.0.1,<2.0.0)
 Requires-Dist: python-jsonpath (>=0.7.1,<0.8.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 <div style="text-align: center; width: 100%;"><img src="branding/logo-wide.png" style="max-height: 200px;" /></div>
 
@@ -28,20 +27,58 @@
 [![Read the Docs](https://img.shields.io/readthedocs/kr8s?logo=readthedocs&logoColor=white)](https://kr8s.readthedocs.io/en/latest/?badge=latest)
 [![PyPI](https://img.shields.io/pypi/v/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/kr8s)](https://pypi.org/project/kr8s/)
 [![Kubernetes Version Support](https://img.shields.io/badge/Kubernetes%20support-1.24%7C1.25%7C1.26%7C1.27-blue)](https://docs.kr8s.org/en/latest/installation.html#supported-kubernetes-versions)
 [![PyPI - Wheel](https://img.shields.io/pypi/wheel/kr8s)](https://pypi.org/project/kr8s/)
 [![PyPI - License](https://img.shields.io/pypi/l/kr8s)](https://pypi.org/project/kr8s/)
 
-> **Warning**
-> This is beta software and might not be ready for prime time.
+A simple, extensible Python client library for Kubernetes that feels familiar for folks who already know how to use `kubectl`.
 
-A Kubernetes API for Python
+## Highlights
 
-### History
+- API inspired by `kubectl` to reduce developer learning curve.
+- [Sensible defaults](https://docs.kr8s.org/en/latest/authentication.html) to reduce boiler plate.
+- No swagger generated code, human readable code only.
+- Supports both [async/await](https://docs.kr8s.org/en/latest/asyncio.html) and sync APIs.
+- [Client caching](https://docs.kr8s.org/en/latest/client.html#client-caching) to reduce passing API objects around.
+- Batteries included by providing useful utilities and methods inspired by `kubectl`.
 
-This project was originally spun out from [dask-kubernetes](https://github.com/dask/dask-kubernetes) which provides utilities for deploying [Dask](https://www.dask.org/) clusters on Kubernetes.
+## Quickstart
 
-The `dask-kubernetes` project used a mix of [kubernetes](https://github.com/kubernetes-client/python), [kubernetes-asyncio](https://github.com/tomplus/kubernetes_asyncio) and [pykube-ng](https://codeberg.org/hjacobs/pykube-ng) (and some subprocess calls to [kubectl](https://kubernetes.io/docs/reference/kubectl/)) to interact with the Kubernetes API. It also contained a whole load of glue code to work around missing features and get everything working together.
+### Installation
 
-To improve maintenance and code reuse `kr8s` was born to extract the Kubernetes library code in `dask-kubernetes` and replace it with something simpler and more complete. Thank you to everyone who contributed to `dask-kubernetes` and we hope you contribute to `kr8s` too.
+```console
+$ pip install kr8s
+```
+
+### Client API
+
+```python
+import kr8s
+
+api = kr8s.api()
+pods = api.get("pods")
+```
+
+See the [Client API docs](https://docs.kr8s.org/en/latest/client.html) for more examples.
+
+### Object API
+
+```python
+from kr8s.objects import Pod
+
+pod = Pod({
+        "apiVersion": "v1",
+        "kind": "Pod",
+        "metadata": {
+            "name": "my-pod",
+        },
+        "spec": {
+            "containers": [{"name": "pause", "image": "gcr.io/google_containers/pause",}]
+        },
+    })
+
+pod.create()
+```
+
+See the [Object API docs](https://docs.kr8s.org/en/latest/object.html) for more examples.
```

