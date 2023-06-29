# Comparing `tmp/grai_schemas-0.1.9.tar.gz` & `tmp/grai_schemas-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_schemas-0.1.9.tar", max compression
+gzip compressed data, was "grai_schemas-0.2.0a1.tar", max compression
```

## Comparing `grai_schemas-0.1.9.tar` & `grai_schemas-0.2.0a1.tar`

### file list

```diff
@@ -1,21 +1,27 @@
--rw-r--r--   0        0        0     3793 2023-01-10 22:34:25.293196 grai_schemas-0.1.9/LICENSE
--rw-r--r--   0        0        0        0 2023-01-10 22:34:25.293226 grai_schemas-0.1.9/README.md
--rw-r--r--   0        0        0      558 2023-02-01 16:25:14.091601 grai_schemas-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      180 2023-01-27 01:14:06.497464 grai_schemas-0.1.9/src/grai_schemas/__init__.py
--rw-r--r--   0        0        0      345 2023-01-27 01:14:06.497536 grai_schemas-0.1.9/src/grai_schemas/base.py
--rw-r--r--   0        0        0     2798 2023-01-29 22:48:26.179628 grai_schemas-0.1.9/src/grai_schemas/generics.py
--rw-r--r--   0        0        0      162 2023-01-29 22:48:26.179850 grai_schemas-0.1.9/src/grai_schemas/package_definitions.py
--rw-r--r--   0        0        0        0 2023-01-18 14:35:11.049253 grai_schemas-0.1.9/src/grai_schemas/py.typed
--rw-r--r--   0        0        0      500 2023-01-29 22:48:26.180085 grai_schemas-0.1.9/src/grai_schemas/schema.py
--rw-r--r--   0        0        0      795 2023-01-31 02:14:01.658847 grai_schemas-0.1.9/src/grai_schemas/utilities.py
--rw-r--r--   0        0        0      139 2023-01-27 01:14:06.497746 grai_schemas-0.1.9/src/grai_schemas/v1/__init__.py
--rw-r--r--   0        0        0     1277 2023-01-31 02:14:01.659066 grai_schemas-0.1.9/src/grai_schemas/v1/edge.py
--rw-r--r--   0        0        0      790 2023-01-31 02:14:01.659316 grai_schemas-0.1.9/src/grai_schemas/v1/generics.py
--rw-r--r--   0        0        0      269 2023-01-27 01:14:06.497906 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/__init__.py
--rw-r--r--   0        0        0     1251 2023-02-01 16:24:41.545223 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/edges.py
--rw-r--r--   0        0        0      289 2023-01-27 01:14:06.497998 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/metadata.py
--rw-r--r--   0        0        0     1086 2023-01-27 01:14:06.498045 grai_schemas-0.1.9/src/grai_schemas/v1/metadata/nodes.py
--rw-r--r--   0        0        0     1096 2023-01-29 22:48:26.180432 grai_schemas-0.1.9/src/grai_schemas/v1/node.py
--rw-r--r--   0        0        0        0 2023-01-27 01:14:06.498108 grai_schemas-0.1.9/src/grai_schemas/v1/workspace.py
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 grai_schemas-0.1.9/setup.py
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 grai_schemas-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3793 2023-02-14 12:06:39.096892 grai_schemas-0.2.0a1/LICENSE
+-rw-r--r--   0        0        0      322 2023-05-02 08:01:59.697152 grai_schemas-0.2.0a1/README.md
+-rw-r--r--   0        0        0      834 2023-06-29 09:52:52.322058 grai_schemas-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      203 2023-06-29 08:12:22.804283 grai_schemas-0.2.0a1/src/grai_schemas/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-29 08:12:22.804823 grai_schemas-0.2.0a1/src/grai_schemas/base.py
+-rw-r--r--   0        0        0     3715 2023-06-29 08:12:22.804993 grai_schemas-0.2.0a1/src/grai_schemas/generics.py
+-rw-r--r--   0        0        0    41788 2023-06-08 08:40:20.862352 grai_schemas-0.2.0a1/src/grai_schemas/human_ids.py
+-rw-r--r--   0        0        0      175 2023-06-06 17:35:16.829056 grai_schemas-0.2.0a1/src/grai_schemas/package_definitions.py
+-rw-r--r--   0        0        0        0 2023-02-14 12:06:39.097597 grai_schemas-0.2.0a1/src/grai_schemas/py.typed
+-rw-r--r--   0        0        0      701 2023-06-06 17:35:16.829170 grai_schemas-0.2.0a1/src/grai_schemas/schema.py
+-rw-r--r--   0        0        0     2568 2023-06-16 16:15:18.436927 grai_schemas-0.2.0a1/src/grai_schemas/utilities.py
+-rw-r--r--   0        0        0      440 2023-06-29 08:12:22.805122 grai_schemas-0.2.0a1/src/grai_schemas/v1/__init__.py
+-rw-r--r--   0        0        0     2786 2023-06-29 08:12:22.805233 grai_schemas-0.2.0a1/src/grai_schemas/v1/edge.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:12:22.805263 grai_schemas-0.2.0a1/src/grai_schemas/v1/events
+-rw-r--r--   0        0        0      845 2023-06-29 08:12:22.805491 grai_schemas-0.2.0a1/src/grai_schemas/v1/events.py
+-rw-r--r--   0        0        0      858 2023-06-29 08:12:22.805602 grai_schemas-0.2.0a1/src/grai_schemas/v1/generics.py
+-rw-r--r--   0        0        0      279 2023-06-16 16:15:18.437295 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/__init__.py
+-rw-r--r--   0        0        0     2067 2023-06-29 08:12:22.805723 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/edges.py
+-rw-r--r--   0        0        0      321 2023-06-16 16:15:18.437462 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/generics.py
+-rw-r--r--   0        0        0      779 2023-06-29 08:12:22.805839 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/metadata.py
+-rw-r--r--   0        0        0     1873 2023-06-29 08:12:22.805942 grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/nodes.py
+-rw-r--r--   0        0        0     6925 2023-06-29 08:12:22.806053 grai_schemas-0.2.0a1/src/grai_schemas/v1/mock.py
+-rw-r--r--   0        0        0     2776 2023-06-29 08:12:22.806146 grai_schemas-0.2.0a1/src/grai_schemas/v1/node.py
+-rw-r--r--   0        0        0      940 2023-06-29 08:12:22.806213 grai_schemas-0.2.0a1/src/grai_schemas/v1/organization.py
+-rw-r--r--   0        0        0     1325 2023-06-29 08:12:22.806285 grai_schemas-0.2.0a1/src/grai_schemas/v1/source.py
+-rw-r--r--   0        0        0     3686 2023-06-29 08:12:22.806382 grai_schemas-0.2.0a1/src/grai_schemas/v1/workspace.py
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 grai_schemas-0.2.0a1/PKG-INFO
```

### Comparing `grai_schemas-0.1.9/LICENSE` & `grai_schemas-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `grai_schemas-0.1.9/pyproject.toml` & `grai_schemas-0.2.0a1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [tool.poetry]
 name = "grai_schemas"
-version = "0.1.9"
+version = "0.2.0-alpha1"
 description = ""
-authors = ["Ian Eaves <ian@grai.io>"]
-readme = "README.md"
+authors = ["Ian Eaves <ian@grai.io>", "Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [{ include = "grai_schemas", from = "src" },]
+readme = "README.md"
+homepage = "https://www.grai.io/"
+repository = "https://github.com/grai-io/grai-core/tree/master/grai-schemas"
+documentation = "https://docs.grai.io/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.10.4"
-
+multimethod = "^1.9.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.11.4"
 pre-commit = "^2.21.0"
 pytest = "^7.2.0"
 mypy = "^0.991"
@@ -24,7 +27,9 @@
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry_bumpversion.file."src/grai_schemas/__init__.py"]
```

### Comparing `grai_schemas-0.1.9/src/grai_schemas/v1/generics.py` & `grai_schemas-0.2.0a1/src/grai_schemas/v1/generics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 from typing import Literal, Optional, Union
 from uuid import UUID
 
 from grai_schemas.generics import GraiBaseModel
+from pydantic import BaseModel
 
 
-class V1Mixin(GraiBaseModel):
+class V1Mixin(BaseModel):
+    """ """
+
     version: Literal["v1"] = "v1"
 
 
 class BaseID(GraiBaseModel):
+    """ """
+
     id: Optional[UUID]
     name: Optional[str]
     namespace: Optional[str]
 
     def __hash__(self):
         if self.name is None or self.namespace is None:
             raise NotImplementedError(
                 f"Computing a hash for {self} requires both name and namespace for compatibility reasons."
             )
-        return hash(hash(self.name) + hash(self.namespace))
+        return hash((self.name, self.namespace))
 
 
 class NamedID(BaseID):
+    """ """
+
     name: str
     namespace: str
     id: Optional[UUID]
 
 
 class UuidID(BaseID):
+    """ """
+
     id: UUID
     name: Optional[str]
     namespace: Optional[str]
 
 
 ID = Union[UuidID, NamedID]
```

### Comparing `grai_schemas-0.1.9/src/grai_schemas/v1/metadata/nodes.py` & `grai_schemas-0.2.0a1/src/grai_schemas/v1/metadata/nodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,77 @@
 from enum import Enum
-from typing import Any, Literal, Optional, Union
+from typing import Any, List, Literal, Optional, Union
 
-from grai_schemas.generics import DefaultValue, HashableBaseModel
+from grai_schemas.generics import DefaultValue, HashableBaseModel, MalformedMetadata
 from grai_schemas.v1.generics import GraiBaseModel, V1Mixin
+from grai_schemas.v1.metadata.generics import GenericAttributes
 
 
-class NodeTypeLabels(Enum):
-    generic = "Node"
-    table = "Table"
-    column = "Column"
+class NodeMetadataTypeLabels(Enum):
+    """ """
+
+    generic: Literal["Generic"] = "Generic"
+    table: Literal["Table"] = "Table"
+    column: Literal["Column"] = "Column"
+
+
+NodeMetadataTypeLabelLiterals = Literal["Generic", "Table", "Column"]
 
 
 class SourceType(Enum):
+    """ """
+
     database = "SQL"
 
 
-class GenericNodeMetadataV1(V1Mixin):
-    node_type: Literal["Node"]
-    node_attributes: dict = {}
+class BaseNodeMetadataV1(V1Mixin):
+    """ """
+
+    type: Literal["NodeV1"] = "NodeV1"
+    node_type: NodeMetadataTypeLabelLiterals
+    node_attributes: GenericAttributes
+    tags: Optional[List[str]]
+
+
+class MalformedNodeMetadataV1(MalformedMetadata, BaseNodeMetadataV1):
+    """ """
 
+    node_type: Optional[str] = "Malformed"  # type: ignore
+    node_attributes: Optional[Any] = GenericAttributes()  # type: ignore
+
+
+class GenericNodeMetadataV1(BaseNodeMetadataV1):
+    node_type: Literal["Generic"]
+    node_attributes: GenericAttributes = GenericAttributes()
+
+
+class ColumnAttributes(V1Mixin, GenericAttributes):
+    """ """
 
-class ColumnAttributes(GraiBaseModel):
     data_type: Optional[str]  # This will need to be standardized
     default_value: Optional[DefaultValue]
     is_nullable: Optional[bool]
     is_unique: Optional[bool]
     is_primary_key: Optional[bool]
 
 
-class ColumnMetadata(GenericNodeMetadataV1):
+class ColumnMetadata(BaseNodeMetadataV1):
+    """ """
+
     node_type: Literal["Column"]
     node_attributes: ColumnAttributes = ColumnAttributes()
 
 
-class TableAttributes(HashableBaseModel):
+class TableAttributes(V1Mixin, GenericAttributes):
+    """ """
+
     pass
 
 
-class TableMetadata(GenericNodeMetadataV1):
+class TableMetadata(BaseNodeMetadataV1):
+    """ """
+
     node_type: Literal["Table"]
     node_attributes: TableAttributes = TableAttributes()
 
 
 Metadata = Union[ColumnMetadata, TableMetadata, GenericNodeMetadataV1]
```

