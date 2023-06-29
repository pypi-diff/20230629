# Comparing `tmp/grai_client-0.2.9.tar.gz` & `tmp/grai_client-0.3.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.2.9.tar", max compression
+gzip compressed data, was "grai_client-0.3.0a1.tar", max compression
```

## Comparing `grai_client-0.2.9.tar` & `grai_client-0.3.0a1.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0      168 2023-04-29 00:58:02.888509 grai_client-0.2.9/README.md
--rw-r--r--   0        0        0      944 2023-04-30 17:35:35.960665 grai_client-0.2.9/pyproject.toml
--rw-r--r--   0        0        0       78 2023-02-13 20:16:22.660883 grai_client-0.2.9/src/grai_client/__init__.py
--rw-r--r--   0        0        0      445 2023-04-29 00:19:10.353763 grai_client-0.2.9/src/grai_client/authentication.py
--rw-r--r--   0        0        0      210 2023-02-13 20:16:22.661271 grai_client-0.2.9/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0     8706 2023-04-17 19:21:38.334922 grai_client-0.2.9/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0      286 2023-04-17 19:21:38.335020 grai_client-0.2.9/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     2640 2023-04-17 19:21:38.335218 grai_client-0.2.9/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-13 20:16:22.661588 grai_client-0.2.9/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     2514 2023-04-17 19:21:38.335366 grai_client-0.2.9/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0      931 2023-04-17 19:21:38.335480 grai_client-0.2.9/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0     7796 2023-04-17 19:21:38.335700 grai_client-0.2.9/src/grai_client/endpoints/v1/get.py
--rw-r--r--   0        0        0     1780 2023-04-17 19:21:38.335803 grai_client-0.2.9/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     1338 2023-04-17 19:21:38.335909 grai_client-0.2.9/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0      976 2023-03-13 20:23:41.240223 grai_client-0.2.9/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0      948 2023-04-17 19:21:38.336104 grai_client-0.2.9/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0        0 2023-02-13 20:16:22.662418 grai_client-0.2.9/src/grai_client/py.typed
--rw-r--r--   0        0        0       58 2023-02-13 20:16:22.662870 grai_client-0.2.9/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0      218 2023-02-13 20:16:22.662940 grai_client-0.2.9/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      329 2023-02-13 20:16:22.663042 grai_client-0.2.9/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0      111 2023-02-13 20:16:22.663106 grai_client-0.2.9/src/grai_client/schemas/workspace.py
--rw-r--r--   0        0        0       39 2023-02-13 20:16:22.663186 grai_client-0.2.9/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     2907 2023-02-13 20:16:22.663262 grai_client-0.2.9/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     1375 2023-04-29 00:19:10.354101 grai_client-0.2.9/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-13 20:16:22.663408 grai_client-0.2.9/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      529 2023-04-26 00:38:08.539486 grai_client-0.2.9/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1147 1970-01-01 00:00:00.000000 grai_client-0.2.9/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 grai_client-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a1/README.md
+-rw-r--r--   0        0        0     1238 2023-06-29 09:46:51.630799 grai_client-0.3.0a1/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-29 08:12:22.777016 grai_client-0.3.0a1/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a1/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a1/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a1/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a1/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a1/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a1/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a1/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a1/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a1/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a1/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a1/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a1/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a1/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a1/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a1/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     2262 2023-06-29 09:37:24.601652 grai_client-0.3.0a1/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a1/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a1/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a1/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a1/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a1/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a1/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a1/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a1/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a1/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 grai_client-0.3.0a1/PKG-INFO
```

### Comparing `grai_client-0.2.9/pyproject.toml` & `grai_client-0.3.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.2.9"
+version = "0.3.0-alpha1"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
@@ -15,30 +15,41 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.1"
 requests = "^2.28.1"
 multimethod = "^1.9"
 orjson = "^3.8.3"
 pyyaml = "^6.0"
-grai-schemas = "^0.1.11"
-httpx = "^0.23.3"
+grai-schemas = "^0.1.15"
+httpx = {extras = ["http2"], version = "^0.24.0"}
 brotli = "^1.0.9"
+tqdm = "^4.65.0"
+more-itertools = "^9.1.0"
+furl = "^2.1.3"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^0.971"
 isort = "^5.10.1"
 black = "^22.6.0"
 pytest = "^7.2.0"
 types-requests = "^2.28.11.5"
 types-pyyaml = "^6.0.12.2"
 pre-commit = "^2.20.0"
+pdoc = "^13.1.1"
+pytest-durations = "^1.2.0"
 
 [tool.isort]
 profile = "black"
 known_first_party = "grai_client"
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_client/__init__.py"]
+
+[[tool.mypy.overrides]]
+module = "tqdm.autonotebook,furl"
+ignore_missing_imports = true
```

### Comparing `grai_client-0.2.9/src/grai_client/endpoints/v1/client.py` & `grai_client-0.3.0a1/src/grai_client/endpoints/v1/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,74 +1,127 @@
-import asyncio
-from typing import Optional, Union
+from typing import Literal, Optional, Union
 from uuid import UUID, uuid4
 
+import httpx
 from httpx import Response
 
 from grai_client.endpoints.client import BaseClient
 from grai_client.endpoints.utilities import is_valid_uuid
 
 
 class ClientV1(BaseClient):
-    id = "v1"
+    """ """
+
+    id: Literal["v1"] = "v1"
     base = "/api/v1/"
     _node_endpoint = "lineage/nodes/"
     _edge_endpoint = "lineage/edges/"
+    _source_endpoint = "lineage/sources/"
     _workspace_endpoint = "workspaces/"
     _is_authenticated_endpoint = "auth/is-authenticated/"
 
     def __init__(self, *args, workspace: Optional[Union[str, UUID]] = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.api = f"{self.url}{self.base}"
         self.node_endpoint = f"{self.api}{self._node_endpoint}"
         self.edge_endpoint = f"{self.api}{self._edge_endpoint}"
+        self.source_endpoint = f"{self.api}{self._source_endpoint}"
         self.workspace_endpoint = f"{self.api}{self._workspace_endpoint}"
         self.is_authenticated_endpoint = f"{self.api}{self._is_authenticated_endpoint}"
 
-        self._workspace = str(workspace) if workspace is not None else None
+        self._workspace = str(workspace) if isinstance(workspace, (str, UUID)) else None
+
+        if self.init_auth_values.is_valid():
+            self.authenticate(**self.init_auth_values.dict())
 
     def check_authentication(self) -> Response:
-        return asyncio.run(self.session.get(self.is_authenticated_endpoint, headers=self.auth_headers))
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        return httpx.get(self.is_authenticated_endpoint, auth=self.auth)
 
     @property
     def workspace(self) -> Optional[str]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
         return self._workspace
 
     @workspace.setter
     def workspace(self, workspace: Optional[Union[str, UUID]]):
+        """
+
+        Args:
+            workspace (Optional[Union[str, UUID]]):
+
+        Returns:
+
+        Raises:
+
+        """
         if workspace is None:
             self._workspace = workspace
+            self.default_query_args.pop("workspace", None)
             self.default_payload.pop("workspace", None)
             return
 
-        if is_valid_uuid(workspace):
-            pass
+        elif is_valid_uuid(workspace):
+            result = self.get("workspace", workspace).spec
+            if result is None:
+                raise ValueError(f"No workspace found matching `{workspace}`")
         elif isinstance(workspace, str):
-            result = self.get("workspace", workspace)
+            if "/" in workspace:  # workspace ref
+                result = self.get("workspace", ref=workspace)
+            else:  # workspace name
+                result = self.get("workspace", name=workspace)
 
             if result is None:
-                raise Exception(f"No workspace matching `name={workspace}`")
-            else:
-                workspace = result.id
+                raise ValueError(f"No workspace found matching `{workspace}`")
+            elif len(result) > 1:
+                raise ValueError(f"Multiple workspaces found matching workspace ref `{workspace}`")
+            elif workspace != result[0].spec.ref:
+                message = (
+                    f"Although you specified workspace `{workspace}` in the client. We could not identify a "
+                    f"corresponding workspace for the authenticated user in the server."
+                )
+                raise Exception(message)
+
+            workspace = result[0].spec.id
         else:
             raise TypeError("Workspace must be either a string, uuid, or None.")
 
         self._workspace = str(workspace)
+        self.default_query_args["workspace"] = self._workspace
         self.default_payload["workspace"] = self._workspace
 
     def authenticate(
         self,
         username: Optional[str] = None,
         password: Optional[str] = None,
         api_key: Optional[str] = None,
     ) -> None:
+        """
+
+        Args:
+            username (Optional[str], optional):  (Default value = None)
+            password (Optional[str], optional):  (Default value = None)
+            api_key (Optional[str], optional):  (Default value = None)
+
+        Returns:
+
+        Raises:
+
+        """
         super().authenticate(username, password, api_key)
         self.workspace = self.workspace
-
-    def set_authentication_headers(
-        self,
-        username: Optional[str] = None,
-        password: Optional[str] = None,
-        api_key: Optional[str] = None,
-    ) -> None:
-        # Deprecated
-        self.authenticate(username, password, api_key)
```

### Comparing `grai_client-0.2.9/src/grai_client/testing/schema.py` & `grai_client-0.3.0a1/src/grai_client/testing/schema.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,38 @@
 import uuid
 
 from grai_schemas.v1 import EdgeV1, NodeV1
 
-BASE_NODE_METADATA = {"grai": {"node_type": "Node", "node_attributes": {}}}
-BASE_EDGE_METADATA = {"grai": {"edge_type": "Edge", "Edge_attributes": {}}}
+BASE_NODE_METADATA = {"grai": {"node_type": "Generic", "node_attributes": {}}}
+BASE_EDGE_METADATA = {"grai": {"edge_type": "Generic", "Edge_attributes": {}}}
 
 
 def mock_v1_node(
     name=None,
     namespace=None,
     data_source=None,
     display_name=None,
     is_active=True,
     metadata={},
 ):
+    """
+
+    Args:
+        name:  (Default value = None)
+        namespace:  (Default value = None)
+        data_source:  (Default value = None)
+        display_name:  (Default value = None)
+        is_active:  (Default value = True)
+        metadata:  (Default value = {})
+
+    Returns:
+
+    Raises:
+
+    """
     final_metadata = BASE_NODE_METADATA.copy()
     final_metadata.update(metadata)
     node_dict = {
         "type": "Node",
         "version": "v1",
         "spec": {
             "id": None,
@@ -29,26 +44,43 @@
             "metadata": final_metadata,
         },
     }
     return NodeV1(**node_dict)
 
 
 def mock_node_id():
+    """ """
     return {"name": str(uuid.uuid4()), "namespace": str(uuid.uuid4())}
 
 
 def mock_v1_edge(
     name=None,
     namespace=None,
     data_source=None,
     source=None,
     destination=None,
     is_active=True,
     metadata={},
 ):
+    """
+
+    Args:
+        name:  (Default value = None)
+        namespace:  (Default value = None)
+        data_source:  (Default value = None)
+        source:  (Default value = None)
+        destination:  (Default value = None)
+        is_active:  (Default value = True)
+        metadata:  (Default value = {})
+
+    Returns:
+
+    Raises:
+
+    """
     final_metadata = BASE_EDGE_METADATA.copy()
     final_metadata.update(metadata)
     edge_dict = {
         "type": "Edge",
         "version": "v1",
         "spec": {
             "id": None,
@@ -61,14 +93,28 @@
             "metadata": final_metadata,
         },
     }
     return EdgeV1(**edge_dict)
 
 
 def mock_v1_edge_and_nodes(name=None, data_source=None, is_active=True, metadata={}, namespace=None):
+    """
+
+    Args:
+        name:  (Default value = None)
+        data_source:  (Default value = None)
+        is_active:  (Default value = True)
+        metadata:  (Default value = {})
+        namespace:  (Default value = None)
+
+    Returns:
+
+    Raises:
+
+    """
     final_metadata = BASE_EDGE_METADATA.copy()
     final_metadata.update(metadata)
 
     node1 = mock_v1_node(namespace=namespace, data_source=data_source)
     node2 = mock_v1_node(namespace=namespace, data_source=data_source)
 
     edge_dict = {
```

### Comparing `grai_client-0.2.9/src/grai_client/utilities/tests.py` & `grai_client-0.3.0a1/src/grai_client/utilities/tests.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 
 def get_test_client():
+    """ """
     from grai_client.endpoints.v1.client import ClientV1
 
     host = os.environ.get("GRAI_HOST", "localhost")
     port = os.environ.get("GRAI_PORT", "8000")
     username = os.environ.get("GRAI_USERNAME", "null@grai.io")
     password = os.environ.get("GRAI_PASSWORD", "super_secret")
     workspace = os.environ.get("GRAI_WORKSPACE", "default")
 
-    client = ClientV1(host, port, workspace=workspace, insecure=True)
-    client.authenticate(username=username, password=password)
+    client = ClientV1(host, port, workspace=workspace, insecure=True, username=username, password=password)
+
     return client
```

### Comparing `grai_client-0.2.9/PKG-INFO` & `grai_client-0.3.0a1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.2.9
+Version: 0.3.0a1
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: brotli (>=1.0.9,<2.0.0)
-Requires-Dist: grai-schemas (>=0.1.11,<0.2.0)
-Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: furl (>=2.1.3,<3.0.0)
+Requires-Dist: grai-schemas (>=0.1.15,<0.2.0)
+Requires-Dist: httpx[http2] (>=0.24.0,<0.25.0)
+Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: multimethod (>=1.9,<2.0)
 Requires-Dist: orjson (>=3.8.3,<4.0.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://docs.grai.io/
 Project-URL: Repository, https://github.com/grai-io/grai-core/tree/master/grai-client
 Description-Content-Type: text/markdown
 
 # Grai Client
 
 `grai-client` is Grai's python connector for communication with the Grai server.
```

