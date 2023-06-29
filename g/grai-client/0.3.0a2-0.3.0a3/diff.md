# Comparing `tmp/grai_client-0.3.0a2.tar.gz` & `tmp/grai_client-0.3.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_client-0.3.0a2.tar", max compression
+gzip compressed data, was "grai_client-0.3.0a3.tar", max compression
```

## Comparing `grai_client-0.3.0a2.tar` & `grai_client-0.3.0a3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a2/README.md
--rw-r--r--   0        0        0     1239 2023-06-29 09:55:35.729289 grai_client-0.3.0a2/pyproject.toml
--rw-r--r--   0        0        0      156 2023-06-29 08:12:22.777016 grai_client-0.3.0a2/src/grai_client/__init__.py
--rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a2/src/grai_client/authentication.py
--rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a2/src/grai_client/endpoints/__init__.py
--rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a2/src/grai_client/endpoints/client.py
--rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a2/src/grai_client/endpoints/rest.py
--rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a2/src/grai_client/endpoints/utilities.py
--rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a2/src/grai_client/endpoints/v1/__init__.py
--rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a2/src/grai_client/endpoints/v1/client.py
--rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a2/src/grai_client/endpoints/v1/delete.py
--rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/__init__.py
--rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/edge.py
--rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/node.py
--rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/organisation.py
--rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/source.py
--rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/utils.py
--rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/workspace.py
--rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a2/src/grai_client/endpoints/v1/patch.py
--rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a2/src/grai_client/endpoints/v1/post.py
--rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a2/src/grai_client/endpoints/v1/url.py
--rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a2/src/grai_client/endpoints/v1/utils.py
--rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a2/src/grai_client/errors.py
--rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a2/src/grai_client/integrations/__init__.py
--rw-r--r--   0        0        0     2262 2023-06-29 09:37:24.601652 grai_client-0.3.0a2/src/grai_client/integrations/base.py
--rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a2/src/grai_client/py.typed
--rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a2/src/grai_client/schemas/__init__.py
--rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a2/src/grai_client/schemas/labels.py
--rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a2/src/grai_client/schemas/schema.py
--rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a2/src/grai_client/testing/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a2/src/grai_client/testing/schema.py
--rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a2/src/grai_client/update.py
--rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a2/src/grai_client/utilities/__init__.py
--rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a2/src/grai_client/utilities/tests.py
--rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-05-02 08:01:59.660150 grai_client-0.3.0a3/README.md
+-rw-r--r--   0        0        0     1239 2023-06-29 10:21:40.167754 grai_client-0.3.0a3/pyproject.toml
+-rw-r--r--   0        0        0      156 2023-06-29 08:12:22.777016 grai_client-0.3.0a3/src/grai_client/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 17:35:16.716176 grai_client-0.3.0a3/src/grai_client/authentication.py
+-rw-r--r--   0        0        0      265 2023-06-06 17:35:16.716588 grai_client-0.3.0a3/src/grai_client/endpoints/__init__.py
+-rw-r--r--   0        0        0    24172 2023-06-16 20:34:04.867796 grai_client-0.3.0a3/src/grai_client/endpoints/client.py
+-rw-r--r--   0        0        0     1011 2023-06-29 08:12:22.777282 grai_client-0.3.0a3/src/grai_client/endpoints/rest.py
+-rw-r--r--   0        0        0     7282 2023-06-29 08:12:22.777420 grai_client-0.3.0a3/src/grai_client/endpoints/utilities.py
+-rw-r--r--   0        0        0       82 2023-02-14 12:06:39.058550 grai_client-0.3.0a3/src/grai_client/endpoints/v1/__init__.py
+-rw-r--r--   0        0        0     3947 2023-06-29 08:12:22.777559 grai_client-0.3.0a3/src/grai_client/endpoints/v1/client.py
+-rw-r--r--   0        0        0     5369 2023-06-29 08:12:22.777848 grai_client-0.3.0a3/src/grai_client/endpoints/v1/delete.py
+-rw-r--r--   0        0        0      121 2023-06-29 08:12:22.777953 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/__init__.py
+-rw-r--r--   0        0        0     5904 2023-06-29 08:12:22.778062 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/edge.py
+-rw-r--r--   0        0        0     4895 2023-06-29 08:12:22.778126 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/node.py
+-rw-r--r--   0        0        0      838 2023-06-29 08:12:22.778210 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/organisation.py
+-rw-r--r--   0        0        0     2501 2023-06-29 08:12:22.778290 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/source.py
+-rw-r--r--   0        0        0     1953 2023-06-29 08:12:22.778367 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/utils.py
+-rw-r--r--   0        0        0     2622 2023-06-29 08:12:22.778433 grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/workspace.py
+-rw-r--r--   0        0        0     6704 2023-06-29 08:12:22.778569 grai_client-0.3.0a3/src/grai_client/endpoints/v1/patch.py
+-rw-r--r--   0        0        0     8301 2023-06-29 08:12:22.778680 grai_client-0.3.0a3/src/grai_client/endpoints/v1/post.py
+-rw-r--r--   0        0        0     3167 2023-06-29 08:12:22.778795 grai_client-0.3.0a3/src/grai_client/endpoints/v1/url.py
+-rw-r--r--   0        0        0     1102 2023-06-06 17:35:16.717987 grai_client-0.3.0a3/src/grai_client/endpoints/v1/utils.py
+-rw-r--r--   0        0        0      307 2023-06-29 08:12:22.778860 grai_client-0.3.0a3/src/grai_client/errors.py
+-rw-r--r--   0        0        0       42 2023-06-29 08:12:22.779159 grai_client-0.3.0a3/src/grai_client/integrations/__init__.py
+-rw-r--r--   0        0        0     2149 2023-06-29 10:21:30.925245 grai_client-0.3.0a3/src/grai_client/integrations/base.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.059014 grai_client-0.3.0a3/src/grai_client/py.typed
+-rw-r--r--   0        0        0       47 2023-06-29 08:12:22.779751 grai_client-0.3.0a3/src/grai_client/schemas/__init__.py
+-rw-r--r--   0        0        0     1116 2023-06-29 08:12:22.779918 grai_client-0.3.0a3/src/grai_client/schemas/labels.py
+-rw-r--r--   0        0        0      417 2023-06-06 17:35:16.718112 grai_client-0.3.0a3/src/grai_client/schemas/schema.py
+-rw-r--r--   0        0        0       39 2023-02-14 12:06:39.059327 grai_client-0.3.0a3/src/grai_client/testing/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-16 16:15:18.411510 grai_client-0.3.0a3/src/grai_client/testing/schema.py
+-rw-r--r--   0        0        0     3516 2023-06-29 08:12:22.780091 grai_client-0.3.0a3/src/grai_client/update.py
+-rw-r--r--   0        0        0       40 2023-02-14 12:06:39.059522 grai_client-0.3.0a3/src/grai_client/utilities/__init__.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:35:16.718665 grai_client-0.3.0a3/src/grai_client/utilities/tests.py
+-rw-r--r--   0        0        0     1290 1970-01-01 00:00:00.000000 grai_client-0.3.0a3/PKG-INFO
```

### Comparing `grai_client-0.3.0a2/pyproject.toml` & `grai_client-0.3.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai-client"
-version = "0.3.0-alpha2"
+version = "0.3.0-alpha3"
 description = ""
 authors = ["Ian Eaves <ian@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_client", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_client-0.3.0a2/src/grai_client/authentication.py` & `grai_client-0.3.0a3/src/grai_client/authentication.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/client.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/rest.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/rest.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/utilities.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/utilities.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/client.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/client.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/delete.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/delete.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/edge.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/edge.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/node.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/node.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/organisation.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/organisation.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/source.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/source.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/utils.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/get/workspace.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/get/workspace.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/patch.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/patch.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/post.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/post.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/url.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/url.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/endpoints/v1/utils.py` & `grai_client-0.3.0a3/src/grai_client/endpoints/v1/utils.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/integrations/base.py` & `grai_client-0.3.0a3/src/grai_client/integrations/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
 from grai_schemas.base import Event, SourcedEdge, SourcedNode
 from grai_schemas.v1.source import SourceV1
-from grai_source_mysql.adapters import adapt_to_client
 
 from grai_client.endpoints.v1.client import ClientV1
 from grai_client.update import update
 
 
 class EventMixin(ABC):
     def __init__(self):
@@ -70,10 +69,10 @@
 
 
 class ConnectorMixin(CombinedNodesAndEdgesMixin):
     def get_nodes_and_edges(self) -> Tuple[List[SourcedNode], List[SourcedEdge]]:
         with self.connector.connect() as conn:
             nodes, edges = conn.get_nodes_and_edges()
 
-        nodes = adapt_to_client(nodes, self.source, self.client.version)
-        edges = adapt_to_client(edges, self.source, self.client.version)
+        nodes = self.adapt_to_client(nodes)
+        edges = self.adapt_to_client(edges)
         return nodes, edges
```

### Comparing `grai_client-0.3.0a2/src/grai_client/schemas/labels.py` & `grai_client-0.3.0a3/src/grai_client/schemas/labels.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/testing/schema.py` & `grai_client-0.3.0a3/src/grai_client/testing/schema.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/update.py` & `grai_client-0.3.0a3/src/grai_client/update.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/src/grai_client/utilities/tests.py` & `grai_client-0.3.0a3/src/grai_client/utilities/tests.py`

 * *Files identical despite different names*

### Comparing `grai_client-0.3.0a2/PKG-INFO` & `grai_client-0.3.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-client
-Version: 0.3.0a2
+Version: 0.3.0a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Ian Eaves
 Author-email: ian@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

