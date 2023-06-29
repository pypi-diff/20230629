# Comparing `tmp/nomic-1.1.9.tar.gz` & `tmp/nomic-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomic-1.1.9.tar", last modified: Thu Jun  8 20:02:34 2023, max compression
+gzip compressed data, was "nomic-2.0.0.tar", last modified: Wed Jun 28 21:59:30 2023, max compression
```

## Comparing `nomic-1.1.9.tar` & `nomic-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.593768 nomic-1.1.9/
--rw-r--r--   0 andriy     (501) staff       (20)      409 2023-06-08 20:02:34.593371 nomic-1.1.9/PKG-INFO
--rw-r--r--   0 andriy     (501) staff       (20)     1419 2023-05-18 03:34:02.000000 nomic-1.1.9/README.md
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.588679 nomic-1.1.9/nomic/
--rw-r--r--   0 andriy     (501) staff       (20)      105 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/__init__.py
--rw-r--r--   0 andriy     (501) staff       (20)    10318 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/atlas.py
--rw-r--r--   0 andriy     (501) staff       (20)     4542 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/cli.py
--rw-r--r--   0 andriy     (501) staff       (20)     1982 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/data_inference.py
--rw-r--r--   0 andriy     (501) staff       (20)     2028 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/embedders.py
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.591003 nomic-1.1.9/nomic/gpt4all/
--rw-r--r--   0 andriy     (501) staff       (20)       49 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/gpt4all/__init__.py
--rw-r--r--   0 andriy     (501) staff       (20)     8102 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/gpt4all/gpt4all.py
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.592814 nomic-1.1.9/nomic/pl_callbacks/
--rw-r--r--   0 andriy     (501) staff       (20)       47 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/pl_callbacks/__init__.py
--rw-r--r--   0 andriy     (501) staff       (20)     6875 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/pl_callbacks/pl_callback.py
--rw-r--r--   0 andriy     (501) staff       (20)    72218 2023-06-08 19:59:08.000000 nomic-1.1.9/nomic/project.py
--rw-r--r--   0 andriy     (501) staff       (20)      521 2023-06-08 19:56:46.000000 nomic-1.1.9/nomic/settings.py
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.593126 nomic-1.1.9/nomic/tests/
--rw-r--r--   0 andriy     (501) staff       (20)        0 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/tests/__init__.py
--rw-r--r--   0 andriy     (501) staff       (20)    10418 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/tests/test_atlas_client.py
--rw-r--r--   0 andriy     (501) staff       (20)     1284 2023-05-18 03:34:02.000000 nomic-1.1.9/nomic/utils.py
-drwxr-xr-x   0 andriy     (501) staff       (20)        0 2023-06-08 20:02:34.590590 nomic-1.1.9/nomic.egg-info/
--rw-r--r--   0 andriy     (501) staff       (20)      409 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/PKG-INFO
--rw-r--r--   0 andriy     (501) staff       (20)      506 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/SOURCES.txt
--rw-r--r--   0 andriy     (501) staff       (20)        1 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/dependency_links.txt
--rw-r--r--   0 andriy     (501) staff       (20)       41 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/entry_points.txt
--rw-r--r--   0 andriy     (501) staff       (20)      468 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/requires.txt
--rw-r--r--   0 andriy     (501) staff       (20)        6 2023-06-08 20:02:34.000000 nomic-1.1.9/nomic.egg-info/top_level.txt
--rw-r--r--   0 andriy     (501) staff       (20)       38 2023-06-08 20:02:34.593823 nomic-1.1.9/setup.cfg
--rw-r--r--   0 andriy     (501) staff       (20)     1722 2023-06-08 19:56:46.000000 nomic-1.1.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:30.481928 nomic-2.0.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      409 2023-06-28 21:59:30.481928 nomic-2.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2023-06-28 21:59:21.000000 nomic-2.0.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:30.477928 nomic-2.0.0/nomic/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      106 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10917 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/atlas.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4531 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/cli.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/data_inference.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    27888 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/data_operations.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2028 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/embedders.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:30.477928 nomic-2.0.0/nomic/pl_callbacks/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       48 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/pl_callbacks/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6975 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/pl_callbacks/pl_callback.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    57666 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/project.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      521 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/settings.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:30.477928 nomic-2.0.0/nomic/tests/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/tests/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10483 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/tests/test_atlas_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2023-06-28 21:59:21.000000 nomic-2.0.0/nomic/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-28 21:59:30.477928 nomic-2.0.0/nomic.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      409 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      480 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      437 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2023-06-28 21:59:30.000000 nomic-2.0.0/nomic.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-28 21:59:30.481928 nomic-2.0.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1740 2023-06-28 21:59:21.000000 nomic-2.0.0/setup.py
```

### Comparing `nomic-1.1.9/README.md` & `nomic-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `nomic-1.1.9/nomic/atlas.py` & `nomic-2.0.0/nomic/atlas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 """
 This class allows for programmatic interactions with Atlas - Nomic's neural database. Initialize AtlasClient in any Python context such as a script
 or in a Jupyter Notebook to organize and interact with your unstructured data.
 """
 
+import uuid
 from typing import Dict, List, Optional
 
 import numpy as np
 from loguru import logger
 from tqdm import tqdm
-import uuid
 
 from .project import AtlasProject
 from .settings import *
-from .utils import get_random_name
+from .utils import b64int, get_random_name
+
 
 def map_embeddings(
     embeddings: np.array,
     data: List[Dict] = None,
     id_field: str = None,
     name: str = None,
     description: str = None,
@@ -72,32 +73,38 @@
 
     if name:
         project_name = name
         index_name = name
     if description:
         description = description
 
+    added_id_field = False
     if data is None:
-        data = [{
-            ATLAS_DEFAULT_ID_FIELD: str(uuid.uuid4())
-        } for _ in range(len(embeddings))]
+        data = [{ATLAS_DEFAULT_ID_FIELD: b64int(i)} for i in range(len(embeddings))]
+        added_id_field = True
+
+    if id_field == ATLAS_DEFAULT_ID_FIELD and id_field not in data[0]:
+        added_id_field = True
+        for i in range(len(data)):
+            data[i][id_field] = b64int(i)
+
+    if added_id_field:
+        logger.warning("An ID field was not specified in your data so one was generated for you in insertion order.")
 
     project = AtlasProject(
         name=project_name,
         description=description,
         unique_id_field=id_field,
         modality='embedding',
         is_public=is_public,
         organization_name=organization_name,
         reset_project_if_exists=reset_project_if_exists,
         add_datums_if_exists=add_datums_if_exists,
     )
 
-    # project._validate_map_data_inputs(colorable_fields=colorable_fields, id_field=id_field, data=data)
-
     number_of_datums_before_upload = project.total_datums
 
     # sends several requests to allow for threadpool refreshing. Threadpool hogs memory and new ones need to be created.
     logger.info("Uploading embeddings to Atlas.")
 
     embeddings = embeddings.astype(np.float16)
     if shard_size is not None:
@@ -153,15 +160,15 @@
     reset_project_if_exists: bool = False,
     add_datums_if_exists: bool = False,
     shard_size: None = None,
     projection_n_neighbors: int = DEFAULT_PROJECTION_N_NEIGHBORS,
     projection_epochs: int = DEFAULT_PROJECTION_EPOCHS,
     projection_spread: float = DEFAULT_PROJECTION_SPREAD,
     duplicate_detection: bool = False,
-    duplicate_threshold: float = DEFAULT_DUPLICATE_THRESHOLD, 
+    duplicate_threshold: float = DEFAULT_DUPLICATE_THRESHOLD,
 ) -> AtlasProject:
     '''
     Generates or updates a map of the given text.
 
     Args:
         data: An [N,] element list of dictionaries containing metadata for each embedding.
         indexed_field: The name the data field containing the text your want to map.
@@ -203,14 +210,24 @@
         modality='text',
         is_public=is_public,
         organization_name=organization_name,
         reset_project_if_exists=reset_project_if_exists,
         add_datums_if_exists=add_datums_if_exists,
     )
 
+    added_id_field = False
+
+    if id_field == ATLAS_DEFAULT_ID_FIELD and id_field not in data[0]:
+        added_id_field = True
+        for i in range(len(data)):
+            data[i][id_field] = b64int(i)
+
+    if added_id_field:
+        logger.warning("An ID field was not specified in your data so one was generated for you in insertion order.")
+
     project._validate_map_data_inputs(colorable_fields=colorable_fields, id_field=id_field, data=data)
 
     number_of_datums_before_upload = project.total_datums
 
     logger.info("Uploading text to Atlas.")
     if shard_size is not None:
         logger.warning("Passing 'shard_size' is deprecated and will be removed in a future release.")
```

### Comparing `nomic-1.1.9/nomic/cli.py` & `nomic-2.0.0/nomic/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     'staging': {'frontend_domain': 'staging-atlas.nomic.ai', 'api_domain': 'staging-api-atlas.nomic.ai'},
     'production': {'frontend_domain': 'atlas.nomic.ai', 'api_domain': 'api-atlas.nomic.ai'},
 }
 
 nomic_base_path = Path.home() / '.nomic'
 
 
-
 def validate_api_http_response(response):
     if response.status_code >= 500 and response.status_code < 600:
         raise Exception("Cannot contact establish a connection with Nomic services.")
 
     return response
 
 
@@ -82,14 +81,15 @@
 
         bearer_token = response.json()['access_token']
         credentials['token'] = bearer_token
         with open(os.path.join(nomic_base_path, 'credentials'), 'w') as file:
             json.dump(credentials, file)
     return credentials
 
+
 def switch(tenant):
     assert tenant in ['staging', 'production', None]
     credentials = get_api_credentials()
     current_tenant = credentials['tenant']
     if tenant is None:
         print(f'Current tenant: {current_tenant}')
         return
@@ -101,15 +101,15 @@
         print(f'Switching from {current_tenant} to {tenant}.')
         if current_loc.exists():
             current_loc.rename(new_loc)
         if (nomic_base_path / f'credentials_{tenant}').exists():
             (nomic_base_path / f'credentials_{tenant}').rename(current_loc)
         else:
             login(token=None, tenant=tenant)
-        
+
 
 @click.command()
 @click.argument('command', nargs=1, default='')
 @click.argument('params', nargs=-1)
 def cli(command, params):
     if command == 'login':
         if len(params) == 0:
@@ -123,10 +123,11 @@
     elif command == 'switch':
         if len(params) == 0:
             switch(tenant=None)
         if len(params) == 1:
             switch(tenant=params[0])
     else:
         raise ValueError(f"Command {command} not found.")
-    
+
+
 if __name__ == "__main__":
     cli()
```

### Comparing `nomic-1.1.9/nomic/data_inference.py` & `nomic-2.0.0/nomic/data_inference.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,53 +1,54 @@
+from typing import Any, Dict, List, Union
+
 import pyarrow as pa
-from typing import List, Union, Dict, Any
 
 
-def from_list(values: Dict[str, Any], schema = None) -> pa.Table:
-  tb = pa.Table.from_pylist(values, schema=schema)
-  return tb
+def from_list(values: Dict[str, Any], schema=None) -> pa.Table:
+    tb = pa.Table.from_pylist(values, schema=schema)
+    return tb
+
 
 permitted_types = {
     'integer': pa.int32(),
     'float': pa.float32(),
     'date': pa.timestamp('ms'),
     'string': pa.string(),
     'categorical': pa.string(),
 }
 
-def convert_pyarrow_schema_for_atlas(schema : pa.Schema) -> pa.Schema:
-  """
-  Convert a pyarrow schema to one with types that match the subset of types supported by Atlas for upload.
-  """
-  types = {}
-  whitelist = {}
-  for field in schema:      
-      if field.name.startswith('_'):
-          # Underscore fields are private to Atlas and will be handled with their own logic.
-          if not field.name in {"_embeddings"}:
-            raise ValueError(f"Underscore fields are reserved for Atlas internal use: {field.name}")
-          whitelist[field.name] = field.type
-      elif pa.types.is_boolean(field.type):
-          raise TypeError(f"Boolean type not supported: {field.name}")
-      elif pa.types.is_list(field.type):
-          raise TypeError(f"List types not supported: {field.name}")
-      elif pa.types.is_struct(field.type):
-          raise TypeError(f"Struct types not supported: {field.name}")
-      elif pa.types.is_dictionary(field.type):
-          types[field.name] = 'categorical'
-      elif pa.types.is_string(field.type):
-          types[field.name] = 'string'
-      elif pa.types.is_integer(field.type):
-          types[field.name] = 'integer'
-      elif pa.types.is_floating(field.type):
-          types[field.name] = 'float'
-      elif pa.types.is_timestamp(field.type):
-          types[field.name] = 'date'
-      elif pa.types.is_temporal(field.type):
-          types[field.name] = 'date'
-      else:
-          raise TypeError(f"Unknown type: {field.name} {field.type}")
-  usertypes = {
-    k: permitted_types[v] for k, v in types.items()
-  }
 
-  return pa.schema({**usertypes, **whitelist})
+def convert_pyarrow_schema_for_atlas(schema: pa.Schema) -> pa.Schema:
+    """
+    Convert a pyarrow schema to one with types that match the subset of types supported by Atlas for upload.
+    """
+    types = {}
+    whitelist = {}
+    for field in schema:
+        if field.name.startswith('_'):
+            # Underscore fields are private to Atlas and will be handled with their own logic.
+            if not field.name in {"_embeddings"}:
+                raise ValueError(f"Underscore fields are reserved for Atlas internal use: {field.name}")
+            whitelist[field.name] = field.type
+        elif pa.types.is_boolean(field.type):
+            raise TypeError(f"Boolean type not supported: {field.name}")
+        elif pa.types.is_list(field.type):
+            raise TypeError(f"List types not supported: {field.name}")
+        elif pa.types.is_struct(field.type):
+            raise TypeError(f"Struct types not supported: {field.name}")
+        elif pa.types.is_dictionary(field.type):
+            types[field.name] = 'categorical'
+        elif pa.types.is_string(field.type):
+            types[field.name] = 'string'
+        elif pa.types.is_integer(field.type):
+            types[field.name] = 'integer'
+        elif pa.types.is_floating(field.type):
+            types[field.name] = 'float'
+        elif pa.types.is_timestamp(field.type):
+            types[field.name] = 'date'
+        elif pa.types.is_temporal(field.type):
+            types[field.name] = 'date'
+        else:
+            raise TypeError(f"Unknown type: {field.name} {field.type}")
+    usertypes = {k: permitted_types[v] for k, v in types.items()}
+
+    return pa.schema({**usertypes, **whitelist})
```

### Comparing `nomic-1.1.9/nomic/embedders.py` & `nomic-2.0.0/nomic/embedders.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.9/nomic/pl_callbacks/pl_callback.py` & `nomic-2.0.0/nomic/pl_callbacks/pl_callback.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,76 @@
-import torch
-from pytorch_lightning.callbacks import Callback
-from nomic import atlas, AtlasUser
-from loguru import logger
-from typing import List, Dict
 from collections import defaultdict
 from datetime import datetime
+from typing import Dict, List
 
 import numpy as np
+import torch
+from loguru import logger
+from pytorch_lightning.callbacks import Callback
+
+from nomic import AtlasUser, atlas
+
 
 class AtlasLightningContainer:
     def __init__(self):
         self.embeddings = []
         self.metadata = defaultdict(list)
 
     def log(self, embeddings: torch.Tensor, metadata: Dict[str, List] = {}):
         '''Log a batch of embeddings and corresponding metadata for each embedding.'''
         assert isinstance(embeddings, torch.Tensor), 'You must log a torch Tensor'
 
-        #ensure passed in embeddings are a tensor with shape (batch_size, dimension)
+        # ensure passed in embeddings are a tensor with shape (batch_size, dimension)
         if len(embeddings.shape) != 2:
             raise ValueError("Your logged embedding tensor must have shape (N,d)")
 
-        #sanity check the inputs
+        # sanity check the inputs
         for key in metadata:
             if isinstance(metadata[key], torch.Tensor):
                 metadata[key] = metadata[key].flatten().cpu().tolist()
             elif isinstance(metadata[key], np.ndarray):
                 metadata[key] = metadata[key].flatten().tolist()
             else:
                 if not isinstance(metadata[key], list):
-                    if isinstance(metadata[key], float) or isinstance(metadata[key], int) or isinstance(metadata[key], str):
+                    if (
+                        isinstance(metadata[key], float)
+                        or isinstance(metadata[key], int)
+                        or isinstance(metadata[key], str)
+                    ):
                         metadata[key] = [metadata[key]]
 
-
             if embeddings.shape[0] != len(metadata[key]):
-                raise ValueError(f"Your metadata has invalid shape. You have {embeddings.shape[0]} embeddings but len(metadata['{key}']) = {len(metadata[key])}")
+                raise ValueError(
+                    f"Your metadata has invalid shape. You have {embeddings.shape[0]} embeddings but len(metadata['{key}']) = {len(metadata[key])}"
+                )
 
         self.embeddings.append(embeddings)
         for key in metadata:
             self.metadata[key] = self.metadata[key] + metadata[key]
 
     def clear(self):
         '''Clears all embeddings and metadata from the final produced map.'''
         self.embeddings = []
         self.metadata = defaultdict(list)
 
+
 class AtlasEmbeddingExplorer(Callback):
-    def __init__(self, max_points=-1, rebuild_time_delay=600, name=None, description=None, is_public=True, overwrite_on_validation=False):
+    def __init__(
+        self,
+        max_points=-1,
+        rebuild_time_delay=600,
+        name=None,
+        description=None,
+        is_public=True,
+        overwrite_on_validation=False,
+    ):
         '''
 
         Args:
-            max_points: The maximum points to visualize.
+            max_points: The maximum points to visualize. -1 will visualize all points.
             rebuild_time_delay: Only rebuilds the embedding explorer if 'rebuild_time_delay' seconds have passed since the last rebuild.
             name: The name for your embedding explorer.
             description: A description for your embedding explorer.
             is_public: Should your embedding explorer be public
             overwrite_on_validation: Re-creates your validation set viewer on every validation run.
         '''
         self.max_points = max_points
@@ -66,22 +82,21 @@
         self.map = None
         self.atlas = AtlasLightningContainer()
         self.rebuild_time_delay = rebuild_time_delay
         self.last_rebuild_timestamp = datetime.min
 
     def on_train_start(self, trainer, pl_module):
         '''Verify that atlas is configured and set up variables'''
-        AtlasUser() #verify logged in.
+        AtlasUser()  # verify logged in.
         pl_module.atlas = self.atlas
 
     def on_sanity_check_start(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
         AtlasUser()  # verify logged in.
         pl_module.atlas = AtlasLightningContainer()
 
-
     def on_train_epoch_start(self, *args, **kwargs):
         self.atlas.clear()
 
     def on_validation_start(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
         self.atlas.clear()
 
     def on_train_end(self, trainer: "pl.Trainer", pl_module: "pl.LightningModule") -> None:
@@ -91,60 +106,67 @@
         self._create_map()
 
     def _create_map(self):
         seconds_since_last_build = int((datetime.now() - self.last_rebuild_timestamp).total_seconds())
         if seconds_since_last_build < self.rebuild_time_delay:
             logger.info(
                 f"Skipping regenerating embedding explorer for this validation epoch as its been {seconds_since_last_build} seconds since the last rebuild and `rebuild_time_delay={self.rebuild_time_delay}`"
-                f" See your previous validation embedding space at: {self.map.map_link}")
+                f" See your previous validation embedding space at: {self.map.map_link}"
+            )
             return
         if not self.atlas.embeddings:
-            logger.info("Pytorch module does not have logits recorded in _atlas_logits property, AtlasEmbeddingExplorer will not generate a map.")
+            logger.info(
+                "Pytorch module does not have logits recorded in _atlas_logits property, AtlasEmbeddingExplorer will not generate a map."
+            )
             return
         embeddings = torch.cat(self.atlas.embeddings).detach().cpu().numpy()
 
         lengths = map(len, self.atlas.metadata.values())
         assert set(lengths) != 1, 'Error in logging metadata, it is not all the same length'
 
         if self.max_points > 0:
-            embeddings = embeddings[:self.max_points, :]
+            embeddings = embeddings[: self.max_points, :]
             for key in self.atlas.metadata:
-                self.atlas.metadata[key] = self.atlas.metadata[key][:self.max_points]
+                self.atlas.metadata[key] = self.atlas.metadata[key][: self.max_points]
 
-                #convert all uniqish values to strings prior to insertion into Atlas so
+                # convert all uniqish values to strings prior to insertion into Atlas so
                 if len(set(self.atlas.metadata[key])) <= 10:
                     self.atlas.metadata[key] = [str(x) for x in self.atlas.metadata[key]]
 
         keys = list(self.atlas.metadata.keys())
         if 'id' not in self.atlas.metadata:
             self.atlas.metadata['id'] = [i for i in range(embeddings.shape[0])]
             keys.append('id')
 
         metadata = [dict(zip(keys, vals)) for vals in zip(*(self.atlas.metadata[k] for k in keys))]
 
         colorable_fields = []
         for key in keys:
             if key == 'id':
                 continue
-            if isinstance(metadata[0][key], float) or \
-                    isinstance(metadata[0][key], int) or \
-                    key in ('class', 'label', 'target') or \
-                    len(set(self.atlas.metadata[key])) <= 10:
+            if (
+                isinstance(metadata[0][key], float)
+                or isinstance(metadata[0][key], int)
+                or key in ('class', 'label', 'target')
+                or len(set(self.atlas.metadata[key])) <= 10
+            ):
                 colorable_fields.append(key)
 
         try:
-            project = atlas.map_embeddings(embeddings=embeddings,
-                                            data=metadata,
-                                            id_field='id',
-                                            colorable_fields=colorable_fields,
-                                            is_public=self.is_public,
-                                            name=self.name,
-                                            description=self.description,
-                                            reset_project_if_exists=self.overwrite,
-                                            build_topic_model=False)
+            project = atlas.map_embeddings(
+                embeddings=embeddings,
+                data=metadata,
+                id_field='id',
+                colorable_fields=colorable_fields,
+                is_public=self.is_public,
+                name=self.name,
+                description=self.description,
+                reset_project_if_exists=self.overwrite,
+                build_topic_model=False,
+            )
         except BaseException as e:
             logger.info(e)
             logger.info("Failed to update your map on this validation epoch.")
             return
         self.project = project
         self.map = project.maps[0]
-        self.last_rebuild_timestamp = datetime.now()
+        self.last_rebuild_timestamp = datetime.now()
```

### Comparing `nomic-1.1.9/nomic/project.py` & `nomic-2.0.0/nomic/project.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,51 +4,44 @@
 import io
 import json
 import os
 import pickle
 import time
 import uuid
 from collections import defaultdict
+from contextlib import contextmanager
 from datetime import date, datetime
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Iterable, Union
-from typing import TYPE_CHECKING
-
-from contextlib import contextmanager
+from typing import TYPE_CHECKING, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy as np
+import pandas as pd
 import pyarrow as pa
-from pyarrow import compute as pc
 import requests
 from loguru import logger
+from pandas import DataFrame
 from pyarrow import compute as pc
 from pyarrow import feather, ipc
 from pydantic import BaseModel, Field
 from tqdm import tqdm
 
-
-# Mainly for type checking
-try:
-    from pandas import DataFrame
-    import pandas as pd
-except ImportError:
-    pd = None
-    DataFrame = None
-
 import nomic
 
 from .cli import refresh_bearer_token, validate_api_http_response
+from .data_inference import convert_pyarrow_schema_for_atlas
+from .data_operations import AtlasMapDuplicates, AtlasMapEmbeddings, AtlasMapTags, AtlasMapTopics
 from .settings import *
 from .utils import assert_valid_project_id, get_object_size_in_bytes
-from .data_inference import convert_pyarrow_schema_for_atlas
+
 
 class AtlasUser:
     def __init__(self):
         self.credentials = refresh_bearer_token()
 
+
 class AtlasClass(object):
     def __init__(self):
         '''
         Initializes the Atlas client.
         '''
 
         if self.credentials['tenant'] == 'staging':
@@ -58,15 +51,20 @@
             api_hostname = 'api-atlas.nomic.ai'
             web_hostname = 'atlas.nomic.ai'
         else:
             raise ValueError("Invalid tenant.")
 
         self.atlas_api_path = f"https://{api_hostname}"
         self.web_path = f"https://{web_hostname}"
-        override_api_path = os.environ['ATLAS_API_PATH']
+
+        try:
+            override_api_path = os.environ['ATLAS_API_PATH']
+        except KeyError:
+            override_api_path = None
+
         if override_api_path:
             self.atlas_api_path = override_api_path
 
         token = self.credentials['token']
         self.token = token
 
         self.header = {"Authorization": f"Bearer {token}"}
@@ -111,15 +109,15 @@
             raise ValueError("colorable_fields must be a list of fields")
 
         if id_field in colorable_fields:
             raise Exception(f'Cannot color by unique id field: {id_field}')
 
         for field in colorable_fields:
             if field not in data[0]:
-                raise Exception(f"Cannot color by field `{field}` as it is not present in the meta-data.")
+                raise Exception(f"Cannot color by field `{field}` as it is not present in the metadata.")
 
     def _get_current_users_main_organization(self):
         '''
         Retrieves the ID of the current users default organization.
 
         **Returns:** The ID of the current users default organization
 
@@ -175,21 +173,19 @@
         )
 
         if response.status_code != 200:
             raise Exception(f'Could not access job state: {response.text}')
 
         return response.json()
 
-    def _validate_and_correct_arrow_upload(
-        self, data: pa.Table, project: "AtlasProject"
-    ) -> pa.Table:
+    def _validate_and_correct_arrow_upload(self, data: pa.Table, project: "AtlasProject") -> pa.Table:
         '''
         Private method. validates upload data against the project arrow schema, and associated other checks.
 
-        1. If unique_id_field is specified, validates that each datum has that field. If not, adds it and then notifies the user that it was added.        
+        1. If unique_id_field is specified, validates that each datum has that field. If not, adds it and then notifies the user that it was added.
 
         Args:
             data: an arrow table.
             project: the atlas project you are validating the data for.
 
         Returns:
 
@@ -202,90 +198,97 @@
                 msg = "Can't add embeddings to a text project."
                 raise ValueError(msg)
         if project.meta['modality'] == 'embedding':
             if "_embeddings" not in data.column_names:
                 msg = "Must include embeddings in embedding project upload."
                 raise ValueError(msg)
 
-        if project.id_field == ATLAS_DEFAULT_ID_FIELD and not ATLAS_DEFAULT_ID_FIELD in data.column_names:
-            # Generate random ids.
-            data = data.append_column(ATLAS_DEFAULT_ID_FIELD, pa.array([base64.b64encode(uuid.uuid4().bytes[:8]).decode('utf-8').rstrip('=') for _ in range(len(data))]))
+        if project.id_field not in data.column_names:
+            raise ValueError(f'Data must contain the ID column `{project.id_field}`')
 
         if project.schema is None:
             project._schema = convert_pyarrow_schema_for_atlas(data.schema)
         # Reformat to match the schema of the project.
         # This includes shuffling the order around if necessary,
         # filling in nulls, etc.
         reformatted = {}
-    
-        if data[project.id_field].null_count > 0:            
-            raise ValueError(f"{project.id_field} must not contain null values, but {data[project.id_field].null_count} found.")
 
+        if data[project.id_field].null_count > 0:
+            raise ValueError(
+                f"{project.id_field} must not contain null values, but {data[project.id_field].null_count} found."
+            )
 
         for field in project.schema:
-            if field.name in data.column_names:                
+            if field.name in data.column_names:
                 # Allow loss of precision in dates and ints, etc.
                 reformatted[field.name] = data[field.name].cast(field.type, safe=False)
-            else:                
-                raise KeyError(f"Field {field.name} present in table schema not found in data. Present fields: {data.column_names}")
+            else:
+                raise KeyError(
+                    f"Field {field.name} present in table schema not found in data. Present fields: {data.column_names}"
+                )
             if pa.types.is_string(field.type):
                 # Ugly temporary measures
                 if data[field.name].null_count > 0:
-                    logger.warning(f"Replacing {data[field.name].null_count} null values for field {field.name} with string 'null'. This behavior will change in a future version.")
+                    logger.warning(
+                        f"Replacing {data[field.name].null_count} null values for field {field.name} with string 'null'. This behavior will change in a future version."
+                    )
                     reformatted[field.name] = pc.fill_null(reformatted[field.name], "null")
                 if pc.any(pc.equal(pc.binary_length(reformatted[field.name]), 0)):
                     mask = pc.equal(pc.binary_length(reformatted[field.name]), 0).combine_chunks()
                     assert pa.types.is_boolean(mask.type)
                     reformatted[field.name] = pc.replace_with_mask(reformatted[field.name], mask, "null")
         for field in data.schema:
             if not field.name in reformatted:
                 if field.name == "_embeddings":
                     reformatted['_embeddings'] = data['_embeddings']
                 else:
                     logger.warning(f"Field {field.name} present in data, but not found in table schema. Ignoring.")
         data = pa.Table.from_pydict(reformatted, schema=project.schema)
-        
+
         if project.meta['insert_update_delete_lock']:
             raise Exception("Project is currently indexing and cannot ingest new datums. Try again later.")
 
         # The following two conditions should never occur given the above, but just in case...
         assert project.id_field in data.column_names, f"Upload does not contain your specified id_field"
 
         if not pa.types.is_string(data[project.id_field].type):
             logger.warning(f"id_field is not a string. Converting to string from {data[project.id_field].type}")
-            data = data.drop([project.id_field]).append_column(project.id_field, data[project.id_field].cast(pa.string()))
+            data = data.drop([project.id_field]).append_column(
+                project.id_field, data[project.id_field].cast(pa.string())
+            )
 
-        
         for key in data.column_names:
             if key.startswith('_'):
                 if key == '_embeddings':
                     continue
                 raise ValueError('Metadata fields cannot start with _')
         if pc.max(pc.utf8_length(data[project.id_field])).as_py() > 36:
-            first_match = data.filter(pc.greater(pc.utf8_length(data[project.id_field]), 36)).to_pylist()[0][project.id_field]
+            first_match = data.filter(pc.greater(pc.utf8_length(data[project.id_field]), 36)).to_pylist()[0][
+                project.id_field
+            ]
             raise ValueError(
                 f"The id_field {first_match} is greater than 36 characters. Atlas does not support id_fields longer than 36 characters."
             )
         return data
-    
+
     def _get_organization(self, organization_name=None, organization_id=None) -> Tuple[str, str]:
         '''
         Gets an organization by either it's name or id.
 
         Args:
             organization_name: the name of the organization
             organization_id: the id of the organization
 
         Returns:
             The organization_name and organization_id if one was found.
 
         '''
 
         if organization_name is None:
-            if organization_id is None: #default to current users organization (the one with their name)
+            if organization_id is None:  # default to current users organization (the one with their name)
                 organization = self._get_current_users_main_organization()
                 organization_name = organization['nickname']
                 organization_id = organization['organization_id']
             else:
                 raise NotImplementedError("Getting organization by a specific ID is not yet implemented.")
 
         else:
@@ -298,17 +301,14 @@
                 raise Exception(
                     f"No such organization exists: {organization_name}. You have access to the following organizations: {users_organizations}"
                 )
             organization_id = organization_id_request.json()['organization_id']
 
         return organization_name, organization_id
 
-
-
-
     def _get_existing_project_by_name(self, project_name, organization_name) -> Dict:
         '''
         Utility method for instantiating an AtlasProject.
         Retrieves an existing project by name in a given organization. Fail
         Args:
             project_name: the project name
             organization_name: the organization name
@@ -336,14 +336,15 @@
                 'project_id': existing_project_id,
                 'organization_name': existing_project['owner'],
             }
 
         organization_name, organization_id = self._get_organization(organization_name=organization_name)
         return {'organization_id': organization_id, 'organization_name': organization_name}
 
+
 class AtlasIndex:
     """
     An AtlasIndex represents a single view of an Atlas Project at a point in time.
 
     An AtlasIndex typically contains one or more *projections* which are 2D representations of
     the points in the index that you can browse online.
     """
@@ -354,32 +355,37 @@
         self.name = name
         self.indexed_field = indexed_field
         self.projections = projections
 
     def _repr_html_(self):
         return '<br>'.join([d._repr_html_() for d in self.projections])
 
+
 class AtlasProjection:
     '''
-    Manages operations on maps such as text/vector search.
+    Interact and access state of an Atlas Map including text/vector search.
     This class should not be instantiated directly.
-    Instead instantiate an AtlasProject and use the project.indices or get_map method to retrieve an AtlasProjection.
-    '''
 
+    Instead instantiate an AtlasProject and use the project.maps attribute to retrieve an AtlasProjection.
+    '''
 
-    def __init__(self, project : "AtlasProject", atlas_index_id: str, projection_id: str, name):
+    def __init__(self, project: "AtlasProject", atlas_index_id: str, projection_id: str, name):
         """
         Creates an AtlasProjection.
         """
         self.project = project
         self.id = projection_id
         self.atlas_index_id = atlas_index_id
         self.projection_id = projection_id
         self.name = name
-        self.tile_data = None
+        self._duplicates = None
+        self._embeddings = None
+        self._topics = None
+        self._tags = None
+        self._tile_data = None
 
     @property
     def map_link(self):
         '''
         Retrieves a map link.
         '''
         return f"{self.project.web_path}/map/{self.project.id}/{self.id}"
@@ -411,15 +417,15 @@
             .iframe {{
                 /* vh can be **very** large in vscode ipynb. */
                 height: min(75vh, 66vw);
                 width: 100%;
             }}
         </style>
         """
-    
+
     def _embed_html(self):
         return f"""<script>
             destroy = function() {{
                 document.getElementById("iframe{self.id}").remove()
             }}
         </script>
         <div class="actions">
@@ -455,74 +461,102 @@
         state = self._status['index_build_stage']
         if state != 'Completed':
             return f"""Atlas Projection {self.name}. Status {state}. <a target="_blank" href="{self.map_link}">view online</a>"""
         return f"""
             <h3>Project: {self.name}</h3>
             {self._embed_html()}
             """
-    
-    def web_tile_data(self, tile_destination=None):
+
+    @property
+    def duplicates(self):
+        """Duplicate detection state"""
+        if self._duplicates is None:
+            self._duplicates = AtlasMapDuplicates(self)
+        return self._duplicates
+
+    @property
+    def topics(self):
+        """Topic state"""
+        if self.project.is_locked:
+            raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
+        if self._topics is None:
+            self._topics = AtlasMapTopics(self)
+        return self._topics
+
+    @property
+    def embeddings(self):
+        """Embedding state"""
+        if self._embeddings is None:
+            self._embeddings = AtlasMapEmbeddings(self)
+        return self._embeddings
+
+    @property
+    def tags(self):
+        """Embedding state"""
+        if self._tags is None:
+            self._tags = AtlasMapTags(self)
+        return self._tags
+
+    def _fetch_tiles(self, overwrite: bool = True):
         """
         Downloads all web data for the projection to the specified directory and returns it as a memmapped arrow table.
 
         Args:
-            tile_destination: The directory to download the tiles to. Defaults to "web_tiles".
+            overwrite: If True then overwrite web tile files.
+
+        Returns:
+            An Arrow table containing information for all data points in the index.
         """
-        if tile_destination is None:
-            # Default download directory is ~/.nomic/cache/
-            home_dir = os.path.expanduser("~")
-            tile_destination = os.path.join(home_dir, ".nomic", "cache")
-        self._download_feather(tile_destination, overwrite=True)
+        if self._tile_data is not None:
+            return self._tile_data
+        self._download_feather(overwrite=overwrite)
         tbs = []
-        root = feather.read_table(f"{tile_destination}/0/0/0.feather")
+        root = feather.read_table(self.tile_destination / "0/0/0.feather")
         try:
             sidecars = set([v for k, v in json.loads(root.schema.metadata[b'sidecars']).items()])
         except KeyError:
             sidecars = []
-        for path in Path(tile_destination).glob('**/*.feather'):
+        for path in self.tile_destination.glob('**/*.feather'):
             if len(path.stem.split(".")) > 1:
-                # Sidecars are loaded alonside
+                # Sidecars are loaded alongside
                 continue
             tb = pa.feather.read_table(path)
             for sidecar_file in sidecars:
                 carfile = pa.feather.read_table(path.parent / f"{path.stem}.{sidecar_file}.feather")
                 for col in carfile.column_names:
                     tb = tb.append_column(col, carfile[col])
             tbs.append(tb)
-        self.tile_data = pa.concat_tables(tbs)
+        self._tile_data = pa.concat_tables(tbs)
+
+        return self._tile_data
 
-        return self.tile_data
-                
+    @property
+    def tile_destination(self):
+        return Path("~/.nomic/cache", self.id).expanduser()
 
-    def _download_feather(self, dest: str = None, overwrite: bool = True):
+    def _download_feather(self, dest: Optional[Union[str, Path]] = None, overwrite: bool = True):
         '''
         Downloads the feather tree.
         Args:
-            dest: the destination to download the quadtree.
             overwrite: if True then overwrite existing feather files.
 
         Returns:
             A list containing all quadtiles downloads
         '''
-        if dest is None:
-            # Default download directory is ~/.nomic/cache/
-            home_dir = os.path.expanduser("~")
-            dest = os.path.join(home_dir, ".nomic", "cache")
-            if not os.path.exists(dest):
-                os.mkdir(dest)
-        dest = Path(dest)
+
+        self.tile_destination.mkdir(parents=True, exist_ok=True)
         root = f'{self.project.atlas_api_path}/v1/project/public/{self.project.id}/index/projection/{self.id}/quadtree/'
         quads = [f'0/0/0']
         all_quads = []
         sidecars = None
         while len(quads) > 0:
             rawquad = quads.pop(0)
             quad = rawquad + ".feather"
-            all_quads.append(quad)            
-            path = dest / quad
+            all_quads.append(quad)
+            path = self.tile_destination / quad
             if not path.exists() or overwrite:
                 data = requests.get(root + quad)
                 readable = io.BytesIO(data.content)
                 readable.seek(0)
                 tb = feather.read_table(readable)
                 path.parent.mkdir(parents=True, exist_ok=True)
                 feather.write_feather(tb, path)
@@ -540,312 +574,17 @@
                 # Sidecars don't have children.
                 continue
             kids = schema.metadata.get(b'children')
             children = json.loads(kids)
             quads.extend(children)
         return all_quads
 
-    def download_embeddings(self, save_directory: str, num_workers: int = 10) -> bool:
-        '''
-        Downloads a mapping from datum_id to embedding in shards to the provided directory
-
-        Args:
-            save_directory: The directory to save your embeddings.
-        Returns:
-            True on success
-
-
-        '''
-        self.project._latest_project_state()
-
-        total_datums = self.project.total_datums
-        if self.project.is_locked:
-            raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
-
-        offset = 0
-        limit = EMBEDDING_PAGINATION_LIMIT
-
-        def download_shard(offset, check_access=False):
-            response = requests.get(
-                self.project.atlas_api_path + f"/v1/project/data/get/embedding/{self.project.id}/{self.atlas_index_id}/{offset}/{limit}",
-                headers=self.project.header,
-            )
-
-            if response.status_code != 200:
-                raise Exception(response.text)
-
-            if check_access:
-                return
-            try:
-                content = response.json()
-
-                shard_name = '{}_{}_{}.pkl'.format(self.atlas_index_id, offset, offset + limit)
-                shard_path = os.path.join(save_directory, shard_name)
-                with open(shard_path, 'wb') as f:
-                    pickle.dump(content, f)
-
-            except Exception as e:
-                logger.error('Shard {} download failed with error: {}'.format(shard_name, e))
-
-        download_shard(0, check_access=True)
-
-        with tqdm(total=total_datums // limit) as pbar:
-            with concurrent.futures.ThreadPoolExecutor(max_workers=num_workers) as executor:
-                futures = {
-                    executor.submit(download_shard, cur_offset): cur_offset
-                    for cur_offset in range(0, total_datums, limit)
-                }
-                for future in concurrent.futures.as_completed(futures):
-                    _ = future.result()
-                    pbar.update(1)
-
-        return True
-
-
-    def get_embedding_iterator(self) -> Iterable[Tuple[str, str]]:
-        '''
-        Iterate through embeddings of your datums.
-
-        Returns:
-            A iterable mapping datum ids to their embeddings.
-
-        '''
-
-        if self.is_locked:
-            raise Exception('Project is locked! Please wait until the project is unlocked to download embeddings')
-
-        offset = 0
-        limit = EMBEDDING_PAGINATION_LIMIT
-        while True:
-            response = requests.get(
-                self.atlas_api_path + f"/v1/project/data/get/embedding/{self.id}/{self.atlas_index_id}/{offset}/{limit}",
-                headers=self.header,
-            )
-            if response.status_code != 200:
-                raise Exception(response.text)
-
-            content = response.json()
-            if len(content['datum_ids']) == 0:
-                break
-            offset += len(content['datum_ids'])
-
-            yield content['datum_ids'], content['embeddings']
-
-    def vector_search(self, queries: np.array = None, ids: List[str] = None, k: int = 5) -> Dict[str, List]:
-        '''
-        Performs vector similarity search over data points on your map.
-        If ids is specified, receive back the most similar data ids in vector space to your input ids.
-        If queries is specified, receive back the data ids with representations most similar to the query vectors.
-
-        You should not specify both queries and ids.
-
-        Args:
-            queries: a 2d numpy array where each row corresponds to a query vector
-            ids: a list of
-            k: the number of closest data points (neighbors) to return for each input query/data id
-        Returns:
-            A tuple with two elements containing the following information:
-                neighbors: A set of ids corresponding to the nearest neighbors of each query
-                distances: A set of distances between each query and its neighbors
-        '''
-
-        if queries is None and ids is None:
-            raise ValueError('You must specify either a list of datum `ids` or numpy array of `queries` but not both.')
-
-        max_k = 128
-        max_queries = 256
-        if k > max_k:
-            raise Exception(f"Cannot query for more than {max_k} nearest neighbors. Set `k` to {max_k} or lower")
-
-        if ids is not None:
-            if len(ids) > max_queries:
-                raise Exception(f"Max ids per query is {max_queries}. You sent {len(ids)}.")
-        if queries is not None:
-            if not isinstance(queries, np.ndarray):
-                raise Exception("`queries` must be an instance of np.array.")
-            if queries.shape[0] > max_queries:
-                raise Exception(f"Max vectors per query is {max_queries}. You sent {queries.shape[0]}.")
-
-        if queries is not None:
-            if queries.ndim != 2:
-                raise ValueError('Expected a 2 dimensional array. If you have a single query, we expect an array of shape (1, d).')
-
-            bytesio = io.BytesIO()
-            np.save(bytesio, queries)
-
-        if queries is not None:
-            response = requests.post(
-                self.project.atlas_api_path + "/v1/project/data/get/nearest_neighbors/by_embedding",
-                headers=self.project.header,
-                json={'atlas_index_id': self.atlas_index_id,
-                      'queries': base64.b64encode(bytesio.getvalue()).decode('utf-8'),
-                      'k': k},
-            )
-        else:
-            response = requests.post(
-                self.project.atlas_api_path + "/v1/project/data/get/nearest_neighbors/by_id",
-                headers=self.project.header,
-                json={'atlas_index_id': self.atlas_index_id,
-                      'datum_ids': ids,
-                      'k': k},
-            )
-
-
-        if response.status_code == 500:
-            raise Exception('Cannot perform vector search on your map at this time. Try again later.')
-
-        if response.status_code != 200:
-            raise Exception(response.text)
-
-        response = response.json()
-
-        return response['neighbors'], response['distances']
-
-    def group_by_topic(self, topic_depth = 1):
-        """
-        Group datums by topic at a set topic depth.
-
-        Args:
-            topic_depth: Topic depth to group datums by. Acceptable values
-            currently are (1, 2, 3). Default is 1.
-        Returns:
-            List of dictionaries where each dictionary contains
-                next depth subtopics, topic_id, topic_short_description, topic_long_description,
-                and list of datum_ids.
-        """
-        if not self.tile_data:
-            self.web_tile_data()
-
-        topic_cols = []
-        # TODO: This will need to be changed once topic depths becomes dynamic and not hard-coded
-        if topic_depth not in (1, 2, 3):
-            raise ValueError("Topic depth out of range.")
-
-        # Unique datum id column to aggregate
-        datum_id_col = self.project.meta["unique_id_field"]
-
-        cols = [datum_id_col, f"_topic_depth_{topic_depth}"]
-
-        df = self.tile_data.select(cols).to_pandas()
-        topic_datum_dict = df.groupby(f"_topic_depth_{topic_depth}")[datum_id_col].apply(set).to_dict()
-
-        topic_data = self.get_topic_data()
-        topic_df, hierarchy = self._get_topic_artifacts(topic_data)
-
-        result = []
-
-        for topic, datum_ids in topic_datum_dict.items():
-            # Encountered topic with zero datums
-            if len(datum_ids) == 0:
-                continue
-            
-            result_dict = {}
-            topic_metadata = topic_df[topic_df["topic_short_description"] == topic]
-
-            result_dict["subtopics"] = hierarchy[topic]
-            result_dict["topic_id"] = topic_metadata["topic_id"]
-            result_dict["topic_short_description"] = topic_metadata["topic_short_description"]
-            result_dict["topic_long_description"] = topic_metadata["topic_description"]
-            result_dict["datum_ids"] = datum_ids
-            result.append(result_dict)
-        return result
-
-    @staticmethod
-    def _get_topic_artifacts(topic_data):
-        topic_df = pd.DataFrame(topic_data)
-        topic_df = topic_df.rename(columns={"topic": "topic_id"})
-
-        topic_hierarchy = defaultdict(list)
-        cols = ["topic_id", "_topic_depth_1", "_topic_depth_2", "_topic_depth_3"]
-
-        for i, row in topic_df[cols].iterrows():
-            # Only consider the non-null values for each row
-            topics = [topic for topic in row if pd.notna(topic)]
-            
-            # Iterate over the topics in each row, adding each topic to the
-            # list of subtopics for the topic at the previous depth
-            for i in range(1, len(topics) - 1):
-                if topics[i + 1] not in topic_hierarchy[topics[i]]:
-                    topic_hierarchy[topics[i]].append(topics[i + 1]) 
-        return topic_df, dict(topic_hierarchy)
-
-    def get_topic_data(self) -> List:
-        '''
-        Retrieves metadata about a maps pre-computed topics
-
-        Returns:
-            A dictionary of metadata for each topic in the model
-
-        '''
-        response = requests.get(
-            self.project.atlas_api_path + "/v1/project/{}/index/projection/{}".format(self.project.meta['id'], self.projection_id),
-            headers=self.project.header,
-        )
-        topics = json.loads(response.text)['topic_models'][0]['features']
-        topic_data = [e['properties'] for e in topics]
-        return topic_data
-
-    def get_topic_density(self, time_field: str, start: datetime, end: datetime):
-        '''
-        Counts the number of datums in each topic within a window
-
-        Args:
-            time_field: Your metadata field containing isoformat timestamps
-            start: A datetime object for the window start
-            end: A datetime object for the window end
-
-        Returns:
-            List[{topic: str, count: int}] - A list of {topic, count} dictionaries, sorted from largest count to smallest count
-        '''
-        response = requests.post(
-            self.project.atlas_api_path + "/v1/project/{}/topic_density".format(self.atlas_index_id),
-            headers=self.project.header,
-            json={'start': start.isoformat(),
-                  'end': end.isoformat(),
-                  'time_field': time_field},
-        )
-        if response.status_code != 200:
-            raise Exception(response.text)
-
-        return response.json()
-
-
-    def vector_search_topics(self, queries: np.array, k: int = 32, depth: int = 3) -> Dict:
-        '''
-        Returns the topics best associated with each vector query
-
-        Args:
-            queries: a 2d numpy array where each row corresponds to a query vector
-            k: (Default 32) the number of neighbors to use when estimating the posterior
-            depth: (Default 3) the topic depth at which you want to search
-
-        Returns:
-            A dict of {topic: posterior probability} for each query
-        '''
-
-        if queries.ndim != 2:
-            raise ValueError('Expected a 2 dimensional array. If you have a single query, we expect an array of shape (1, d).')
-
-        bytesio = io.BytesIO()
-        np.save(bytesio, queries)
-
-        response = requests.post(
-            self.project.atlas_api_path + "/v1/project/data/get/embedding/topic",
-            headers=self.project.header,
-            json={'atlas_index_id': self.atlas_index_id,
-                  'queries': base64.b64encode(bytesio.getvalue()).decode('utf-8'),
-                  'k': k,
-                  'depth': depth},
-        )
-
-        if response.status_code != 200:
-            raise Exception(response.text)
-
-        return response.json()
-
+    @property
+    def datum_id_field(self):
+        return self.project.meta["unique_id_field"]
 
     def _get_atoms(self, ids: List[str]) -> List[Dict]:
         '''
         Retrieves atoms by id
 
         Args:
             ids: list of atom ids
@@ -865,107 +604,28 @@
         )
 
         if response.status_code == 200:
             return response.json()['atoms']
         else:
             raise Exception(response.text)
 
-    def get_tags(self) -> Dict[str, List[str]]:
-        '''
-        Retrieves back all tags made in the web browser for a specific project and map.
-
-        Returns:
-            A dictionary mapping datum ids to tags.
-        '''
-        # now get the tags
-        datums_and_tags = requests.post(
-            self.project.atlas_api_path + '/v1/project/tag/read/all_by_datum',
-            headers=self.project.header,
-            json={
-                'project_id': self.project.id,
-            },
-        ).json()['results']
-
-        label_to_datums = {}
-        for item in datums_and_tags:
-            for label in item['labels']:
-                if label not in label_to_datums:
-                    label_to_datums[label] = []
-                label_to_datums[label].append(item['datum_id'])
-        return label_to_datums
-
-    def tag(self, ids: List[str], tags: List[str]):
-        '''
-
-        Args:
-            ids: The datum ids you want to tag
-            tags: A list containing the tags you want to apply to these data points.
-
-        '''
-        assert isinstance(ids, list), 'ids must be a list of strings'
-        assert isinstance(tags, list), 'tags must be a list of strings'
-
-        colname = json.dumps({'project_id': self.project.id, 'atlas_index_id': self.atlas_index_id, 'type': 'datum_id', 'tags': tags})
-        payload_table = pa.table([pa.array(ids, type=pa.string())], [colname])
-        buffer = io.BytesIO()
-        writer = ipc.new_file(buffer, payload_table.schema, options=ipc.IpcWriteOptions(compression='zstd'))
-        writer.write_table(payload_table)
-        writer.close()
-        payload = buffer.getvalue()
-
-        headers = self.project.header.copy()
-        headers['Content-Type'] = 'application/octet-stream'
-        response = requests.post(self.project.atlas_api_path + "/v1/project/tag/add", headers=headers, data=payload)
-        if response.status_code != 200:
-            raise Exception("Failed to add tags")
-
-    def remove_tags(self, ids: List[str], tags: List[str], delete_all: bool = False) -> bool:
-        '''
-        Deletes the specified tags from the given datum_ids.
-
-        Args:
-            ids: The datum_ids to delete tags from.
-            tags: The list of tags to delete from the data points. Each tag will be applied to all data points in `ids`.
-            delete_all: If true, ignores datum_ids and deletes all specified tags from all data points.
-
-        Returns:
-            True on success
-
-        '''
-        assert isinstance(ids, list), 'datum_ids must be a list of strings'
-        assert isinstance(tags, list), 'tags must be a list of strings'
-
-        colname = json.dumps({'project_id': self.project.id, 'atlas_index_id': self.atlas_index_id, 'type': 'datum_id', 'tags': tags, 'delete_all': delete_all})
-        payload_table = pa.table([pa.array(ids, type=pa.string())], [colname])
-        buffer = io.BytesIO()
-        writer = ipc.new_file(buffer, payload_table.schema, options=ipc.IpcWriteOptions(compression='zstd'))
-        writer.write_table(payload_table)
-        writer.close()
-        payload = buffer.getvalue()
-
-        headers = self.project.header.copy()
-        headers['Content-Type'] = 'application/octet-stream'
-        response = requests.post(self.project.atlas_api_path + "/v1/project/tag/delete", headers=headers, data=payload)
-        if response.status_code != 200:
-            raise Exception("Failed to delete tags")
 
 class AtlasProject(AtlasClass):
     def __init__(
         self,
         name: Optional[str] = None,
         description: Optional[str] = 'A description for your map.',
         unique_id_field: Optional[str] = None,
         modality: Optional[str] = None,
         organization_name: Optional[str] = None,
         is_public: bool = True,
         project_id=None,
         reset_project_if_exists=False,
         add_datums_if_exists=True,
     ):
-
         """
         Creates or loads an Atlas project.
         Atlas projects store data (text, embeddings, etc) that you can organize by building indices.
         If the organization already contains a project with this name, it will be returned instead.
 
         **Parameters:**
 
@@ -990,35 +650,32 @@
             return
 
         if organization_name is None:
             organization_name = self._get_current_users_main_organization()['nickname']
 
         results = self._get_existing_project_by_name(project_name=name, organization_name=organization_name)
 
-        if 'project_id' in results: #project already exists
+        if 'project_id' in results:  # project already exists
             organization_name = results['organization_name']
             project_id = results['project_id']
-            if reset_project_if_exists: #reset the project
+            if reset_project_if_exists:  # reset the project
                 logger.info(
                     f"Found existing project `{name}` in organization `{organization_name}`. Clearing it of data by request."
                 )
                 self._delete_project_by_id(project_id=project_id)
                 project_id = None
-            elif not add_datums_if_exists: #prevent adding datums to existing project explicitly
+            elif not add_datums_if_exists:  # prevent adding datums to existing project explicitly
                 raise ValueError(
                     f"Project already exists with the name `{name}` in organization `{organization_name}`. "
                     f"You can add datums to it by settings `add_datums_if_exists = True` or reset it by specifying `reset_project_if_exists=True` on a new upload."
                 )
             else:
-                logger.info(
-                    f"Loading existing project `{name}` from organization `{organization_name}`."
-                )
-
-        if project_id is None: #if there is no existing project, make a new one.
+                logger.info(f"Loading existing project `{name}` from organization `{organization_name}`.")
 
+        if project_id is None:  # if there is no existing project, make a new one.
             if unique_id_field is None:
                 unique_id_field = ATLAS_DEFAULT_ID_FIELD
 
                 raise ValueError("You must specify a unique_id_field when creating a new project.")
 
             if modality is None:
                 raise ValueError("You must specify a modality when creating a new project.")
@@ -1028,23 +685,20 @@
 
             project_id = self._create_project(
                 project_name=name,
                 description=description,
                 unique_id_field=unique_id_field,
                 modality=modality,
                 organization_name=organization_name,
-                is_public=is_public
+                is_public=is_public,
             )
 
-
         self.meta = self._get_project_by_id(project_id=project_id)
         self._schema = None
 
-
-
     def delete(self):
         '''
         Deletes an atlas project with all associated metadata.
         '''
         organization = self._get_current_users_main_organization()
         organization_name = organization['nickname']
 
@@ -1057,15 +711,15 @@
     def _create_project(
         self,
         project_name: str,
         description: Optional[str],
         unique_id_field: str,
         modality: str,
         organization_name: Optional[str] = None,
-        is_public: bool = True
+        is_public: bool = True,
     ):
         '''
         Creates an Atlas project.
         Atlas projects store data (text, embeddings, etc) that you can organize by building indices.
         If the organization already contains a project with this name, it will be returned instead.
 
         **Parameters:**
@@ -1094,28 +748,27 @@
             raise ValueError("You must specify a unique id field")
         logger.info(f"Creating project `{project_name}` in organization `{organization_name}`")
         if description is None:
             description = ""
         response = requests.post(
             self.atlas_api_path + "/v1/project/create",
             headers=self.header,
-            json = {
+            json={
                 'organization_id': organization_id,
                 'project_name': project_name,
                 'description': description,
                 'unique_id_field': unique_id_field,
                 'modality': modality,
                 'is_public': is_public,
             },
         )
         if response.status_code != 201:
             raise Exception(f"Failed to create project: {response.json()}")
-        
-        return response.json()['project_id']
 
+        return response.json()['project_id']
 
     def _latest_project_state(self):
         '''
         Refreshes the project's state. Try to call this sparingly but use it when you need it.
         '''
 
         self.meta = self._get_project_by_id(self.id)
@@ -1128,15 +781,20 @@
         for index in self.meta['atlas_indices']:
             projections = []
             for projection in index['projections']:
                 projection = AtlasProjection(
                     project=self, projection_id=projection['id'], atlas_index_id=index['id'], name=index['index_name']
                 )
                 projections.append(projection)
-            index = AtlasIndex(atlas_index_id=index['id'], name=index['index_name'], indexed_field=index['indexed_field'], projections=projections)
+            index = AtlasIndex(
+                atlas_index_id=index['id'],
+                name=index['index_name'],
+                indexed_field=index['indexed_field'],
+                projections=projections,
+            )
             output.append(index)
 
         return output
 
     @property
     def projections(self) -> List[AtlasProjection]:
         output = []
@@ -1180,21 +838,21 @@
     def project_fields(self):
         return self.meta['project_fields']
 
     @property
     def is_locked(self) -> bool:
         self._latest_project_state()
         return self.meta['insert_update_delete_lock']
-    
+
     @property
     def schema(self) -> Optional[pa.Schema]:
         if self._schema is not None:
             return self._schema
         if 'schema' in self.meta and self.meta['schema'] is not None:
-            self._schema : pa.Schema = ipc.read_schema(io.BytesIO(base64.b64decode(self.meta['schema'])))
+            self._schema: pa.Schema = ipc.read_schema(io.BytesIO(base64.b64decode(self.meta['schema'])))
             return self._schema
         return None
 
     @property
     def is_accepting_data(self) -> bool:
         '''
         Checks if the project can accept data. Projects cannot accept data when they are being indexed.
@@ -1287,15 +945,15 @@
             multilingual: Should the map take language into account? If true, points from different languages but semantically similar text are close together.
             build_topic_model: Should a topic model be built?
             projection_n_neighbors: A projection hyperparameter
             projection_epochs: A projection hyperparameter
             projection_spread: A projection hyperparameter
             topic_label_field: A text field in your metadata to estimate topic labels from. Defaults to the indexed_field for text projects if not specified.
             reuse_embeddings_from_index: the name of the index to reuse embeddings from.
-            duplicate_detection: A boolean whether to run duplicate detection 
+            duplicate_detection: A boolean whether to run duplicate detection
             duplicate_threshold: At which threshold to consider points to be duplicates
 
         Returns:
             The projection this index has built.
 
         '''
 
@@ -1330,25 +988,26 @@
                 ),
                 'topic_model_hyperparameters': json.dumps(
                     {'build_topic_model': build_topic_model, 'community_description_target_field': topic_label_field}
                 ),
             }
 
         elif self.modality == 'text':
-
-            #find the index id of the index with name reuse_embeddings_from_index
+            # find the index id of the index with name reuse_embeddings_from_index
             reuse_embedding_from_index_id = None
             indices = self.indices
             if reuse_embeddings_from_index is not None:
                 for index in indices:
                     if index.name == reuse_embeddings_from_index:
                         reuse_embedding_from_index_id = index.id
                         break
                 if reuse_embedding_from_index_id is None:
-                    raise Exception(f"Could not find the index '{reuse_embeddings_from_index}' to re-use from. Possible options are {[index.name for index in indices]}")
+                    raise Exception(
+                        f"Could not find the index '{reuse_embeddings_from_index}' to re-use from. Possible options are {[index.name for index in indices]}"
+                    )
 
             if indexed_field is None:
                 raise Exception("You did not specify a field to index. Specify an 'indexed_field'.")
 
             if indexed_field not in self.project_fields:
                 raise Exception(f"Indexing on {indexed_field} not allowed. Valid options are: {self.project_fields}")
 
@@ -1379,15 +1038,15 @@
                     {'n_neighbors': projection_n_neighbors, 'n_epochs': projection_epochs, 'spread': projection_spread}
                 ),
                 'topic_model_hyperparameters': json.dumps(
                     {'build_topic_model': build_topic_model, 'community_description_target_field': indexed_field}
                 ),
                 'duplicate_detection_hyperparameters': json.dumps(
                     {'tag_duplicates': duplicate_detection, 'duplicate_cutoff': duplicate_threshold}
-                )
+                ),
             }
 
         response = requests.post(
             self.atlas_api_path + "/v1/project/index/create",
             headers=self.header,
             json=build_template,
         )
@@ -1440,22 +1099,22 @@
         if len(self.projections) >= 1:
             html += "<br><strong>Projections</strong>\n"
             html += "<ul>\n"
             for projection in self.projections:
                 state = projection._status['index_build_stage']
                 if state == 'Completed':
                     complete_projections.append(projection)
-                html += f"""<li>{projection.name}. Status {state}. <a target="_blank" href="{projection.map_link}">view online</a></li>"""   
+                html += f"""<li>{projection.name}. Status {state}. <a target="_blank" href="{projection.map_link}">view online</a></li>"""
             html += "</ul>"
         if len(complete_projections) >= 1:
             # Display most recent complete projection.
             html += "<hr>"
             html += complete_projections[-1]._embed_html()
         return html
-    
+
     def __str__(self):
         return "\n".join([str(projection) for index in self.indices for projection in index.projections])
 
     def get_data(self, ids: List[str]) -> List[Dict]:
         '''
         Retrieve the contents of the data given ids
 
@@ -1503,21 +1162,15 @@
         )
 
         if response.status_code == 200:
             return True
         else:
             raise Exception(response.text)
 
-    def add_text(
-        self,
-        data = Union[DataFrame, List[Dict], pa.Table],
-        pbar=None,
-        shard_size=None,
-        num_workers=None
-    ):
+    def add_text(self, data=Union[DataFrame, List[Dict], pa.Table], pbar=None, shard_size=None, num_workers=None):
         """
         Add text data to the project.
         data: A pandas DataFrame, a list of python dictionaries, or a pyarrow Table matching the project schema.
         pbar: (Optional). A tqdm progress bar to display progress.
         """
         if shard_size is not None or num_workers is not None:
             raise DeprecationWarning("shard_size and num_workers are deprecated.")
@@ -1526,53 +1179,56 @@
         elif isinstance(data, list):
             data = pa.Table.from_pylist(data)
         elif not isinstance(data, pa.Table):
             raise ValueError("Data must be a pandas DataFrame, list of dictionaries, or a pyarrow Table.")
         self._add_data(data, pbar=pbar)
 
     def add_embeddings(
-            self,
-            data : Union[DataFrame, List[Dict], pa.Table, None],
-            embeddings: np.array,
-            pbar = None,
-            shard_size=None, num_workers=None
+        self,
+        data: Union[DataFrame, List[Dict], pa.Table, None],
+        embeddings: np.array,
+        pbar=None,
+        shard_size=None,
+        num_workers=None,
     ):
         """
         Add data, with associated embeddings, to the project.
-        
+
         Args:
             data: A pandas DataFrame, list of dictionaries, or pyarrow Table matching the project schema.
             embeddings: A numpy array of embeddings: each row corresponds to a row in the table.
             pbar: (Optional). A tqdm progress bar to update.
         """
-        
+
         """
         # TODO: validate embedding size.
         assert embeddings.shape[1] == self.embedding_size, "Embedding size must match the embedding size of the project."
         """
         if shard_size is not None:
             raise DeprecationWarning("shard_size is deprecated and no longer has any effect")
         if num_workers is not None:
             raise DeprecationWarning("num_workers is deprecated and no longer has any effect")
         assert type(embeddings) == np.ndarray, "Embeddings must be a numpy array."
         assert len(embeddings.shape) == 2, "Embeddings must be a 2D numpy array."
         assert len(data) == embeddings.shape[0], "Data and embeddings must have the same number of rows."
         assert len(data) > 0, "Data must have at least one row."
-        
+
         tb: pa.Table
 
         if DataFrame is not None and isinstance(data, DataFrame):
             tb = pa.Table.from_pandas(data)
         elif isinstance(data, list):
             tb = pa.Table.from_pylist(data)
         elif isinstance(data, pa.Table):
             tb = data
         else:
-            raise ValueError(f"Data must be a pandas DataFrame, list of dictionaries, or a pyarrow Table, not {type(data)}")
-        
+            raise ValueError(
+                f"Data must be a pandas DataFrame, list of dictionaries, or a pyarrow Table, not {type(data)}"
+            )
+
         del data
 
         # Add embeddings to the data.
         embeddings = embeddings.astype(np.float16)
 
         # Fail if any embeddings are NaN or Inf.
         assert not np.isnan(embeddings).any(), "Embeddings must not contain NaN values."
@@ -1612,36 +1268,34 @@
         nrow = len(data)
 
         shard_size = 5000
         n_chunks = int(np.ceil(nrow / shard_size))
         # Chunk into 4MB pieces. These will probably compress down a bit.
         if bytesize / n_chunks > 4_000_000:
             shard_size = int(np.ceil(nrow / (bytesize / 4_000_000)))
-        
 
         data = self._validate_and_correct_arrow_upload(
-                data=data,
-                project=self
-            )
+            data=data,
+            project=self,
+        )
 
         upload_endpoint = "/v1/project/data/add/arrow"
 
         # Actually do the upload
         def send_request(i):
             data_shard = data.slice(i, shard_size)
             with io.BytesIO() as buffer:
                 data_shard = data_shard.replace_schema_metadata({'project_id': self.id})
-                feather.write_feather(data_shard, buffer, compression = 'zstd', compression_level = 6)
+                feather.write_feather(data_shard, buffer, compression='zstd', compression_level=6)
                 buffer.seek(0)
 
                 response = requests.post(
                     self.atlas_api_path + upload_endpoint,
                     headers=self.header,
-                    data = buffer,
-                    json={'project_id': self.id},
+                    data=buffer,
                 )
                 return response
 
         # if this method is being called internally, we pass a global progress bar
         close_pbar = False
         if pbar is None:
             close_pbar = True
@@ -1712,19 +1366,17 @@
             logger.warning(f"Failed to upload {failed} datums")
         if close_pbar:
             if failed:
                 logger.warning("Upload partially succeeded.")
             else:
                 logger.info("Upload succeeded.")
 
-    def update_maps(self,
-                    data: List[Dict],
-                    embeddings: Optional[np.array]=None,
-                    shard_size: int = 1000,
-                    num_workers: int = 10):
+    def update_maps(
+        self, data: List[Dict], embeddings: Optional[np.array] = None, shard_size: int = 1000, num_workers: int = 10
+    ):
         '''
         Utility method to update a projects maps by adding the given data.
 
         Args:
             data: An [N,] element list of dictionaries containing metadata for each embedding.
             embeddings: An [N, d] matrix of embeddings for updating embedding projects. Leave as None to update text projects.
             shard_size: Data is uploaded in parallel by many threads. Adjust the number of datums to upload by each worker.
@@ -1738,40 +1390,41 @@
             raise ValueError(msg)
 
         if self.modality == 'text' and embeddings is not None:
             msg = 'Please dont specify embeddings for updating a text project'
             raise ValueError(msg)
 
         if embeddings is not None and len(data) != embeddings.shape[0]:
-            msg = 'Expected data and embeddings to be the same length but found lengths {} and {} respectively.'.format()
+            msg = (
+                'Expected data and embeddings to be the same length but found lengths {} and {} respectively.'.format()
+            )
             raise ValueError(msg)
 
-
         # Add new data
         logger.info("Uploading data to Nomic's neural database Atlas.")
         with tqdm(total=len(data) // shard_size) as pbar:
             for i in range(0, len(data), MAX_MEMORY_CHUNK):
                 if self.modality == 'embedding':
                     self.add_embeddings(
-                        embeddings=embeddings[i: i + MAX_MEMORY_CHUNK, :],
-                        data=data[i: i + MAX_MEMORY_CHUNK],
+                        embeddings=embeddings[i : i + MAX_MEMORY_CHUNK, :],
+                        data=data[i : i + MAX_MEMORY_CHUNK],
                         shard_size=shard_size,
                         num_workers=num_workers,
                         pbar=pbar,
                     )
                 else:
                     self.add_text(
-                        data=data[i: i + MAX_MEMORY_CHUNK],
+                        data=data[i : i + MAX_MEMORY_CHUNK],
                         shard_size=shard_size,
                         num_workers=num_workers,
                         pbar=pbar,
                     )
         logger.info("Upload succeeded.")
 
-        #Update maps
+        # Update maps
         # finally, update all the indices
         return self.rebuild_maps()
 
     def rebuild_maps(self, rebuild_topic_models: bool = False):
         '''
         Rebuilds all maps in a project with the latest state project data state. Maps will not be rebuilt to
         reflect the additions, deletions or updates you have made to your data until this method is called.
@@ -1779,14 +1432,11 @@
         Args:
             rebuild_topic_models: (Default False) - If true, will create new topic models when updating these indices
         '''
 
         response = requests.post(
             self.atlas_api_path + "/v1/project/update_indices",
             headers=self.header,
-            json={
-                'project_id': self.id,
-                'rebuild_topic_models': rebuild_topic_models
-            },
+            json={'project_id': self.id, 'rebuild_topic_models': rebuild_topic_models},
         )
 
         logger.info(f"Updating maps in project `{self.name}`")
```

### Comparing `nomic-1.1.9/nomic/settings.py` & `nomic-2.0.0/nomic/settings.py`

 * *Files identical despite different names*

### Comparing `nomic-1.1.9/nomic/tests/test_atlas_client.py` & `nomic-2.0.0/nomic/tests/test_atlas_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import os
 import random
 import tempfile
 import time
 import uuid
 from datetime import datetime, timedelta
 import numpy as np
 import pytest
@@ -13,19 +14,20 @@
 def gen_random_datetime(min_year=1900, max_year=datetime.now().year):
     # generate a datetime in format yyyy-mm-dd hh:mm:ss.000000
     start = datetime(min_year, 1, 1, 00, 00, 00)
     years = max_year - min_year + 1
     end = start + timedelta(days=365 * years)
     return start + (end - start) * random.random()
 
+
 def test_map_idless_embeddings():
     num_embeddings = 50
     embeddings = np.random.rand(num_embeddings, 512)
 
-    response = atlas.map_embeddings(name="test1", embeddings=embeddings, reset_project_if_exists = True)
+    response = atlas.map_embeddings(name="test1", embeddings=embeddings, reset_project_if_exists=True)
 
     AtlasProject(name="test1").delete()
 
 
 def test_map_embeddings_with_errors():
     num_embeddings = 20
     embeddings = np.random.rand(num_embeddings, 10)
@@ -53,63 +55,35 @@
             name='UNITTEST1',
             id_field='id',
             is_public=True,
             reset_project_if_exists=True,
         )
 
 
-def test_map_embeddings():
-    num_embeddings = 20
-    embeddings = np.random.rand(num_embeddings, 10)
-    data = [{'field': str(uuid.uuid4()), 'id': str(uuid.uuid4())} for i in range(len(embeddings))]
-
-    project = atlas.map_embeddings(
-        embeddings=embeddings,
-        name='UNITTEST1',
-        id_field='id',
-        data=data,
-        is_public=True,
-        reset_project_if_exists=True,
-    )
-
-    map = project.get_map(name='UNITTEST1')
-
-    time.sleep(10)
-    with tempfile.TemporaryDirectory() as td:
-        retrieved_embeddings = map.download_embeddings(td)
-
-    assert project.total_datums == num_embeddings
-
-    project = AtlasProject(name='UNITTEST1')
-    map = project.get_map(name='UNITTEST1')
-
-    project.create_index(name='My new index')
-    with project.wait_for_project_lock():
-        neighbors, _ = map.vector_search(queries=np.random.rand(1, 10), k=2)
-        assert len(neighbors[0]) == 2
-
-    for map in project.projections:
-        assert map.map_link
-
-    map.tag(ids=[data[0]['id']], tags=['my_tag'])
-
-    assert len(map.get_tags()['my_tag']) == 1
-
-    map.remove_tags(ids=[data[0]['id']], tags=['my_tag'])
-
-    assert 'my_tag' not in map.get_tags()
-
-    project.delete()
+def test_map_text_errors():
+    # no indexed field
+    with pytest.raises(Exception):
+        project = atlas.map_text(
+            data=[{'key': 'a'}],
+            indexed_field='text',
+            is_public=True,
+            name='test_map_text_errors',
+            description='test map description',
+            reset_project_if_exists=True,
+        )
+    AtlasProject(name='test_map_text_errors').delete()
 
 
 def test_date_metadata():
     num_embeddings = 20
     embeddings = np.random.rand(num_embeddings, 10)
-    data = [{'my_date': datetime(2022, 1, i),
-             'my_random_date': gen_random_datetime()} for i in range(1, len(embeddings) + 1)]
+    data = [
+        {'my_date': datetime(2022, 1, i), 'my_random_date': gen_random_datetime()}
+        for i in range(1, len(embeddings) + 1)
+    ]
 
     project = atlas.map_embeddings(
         embeddings=embeddings, name='test_date_metadata', data=data, is_public=True, reset_project_if_exists=True
     )
 
     assert project.id
 
@@ -124,27 +98,14 @@
             id_field='id',
             data=data,
             is_public=True,
             reset_project_if_exists=True,
         )
 
 
-def test_map_text_errors():
-    # no indexed field
-    with pytest.raises(Exception):
-        project = atlas.map_text(
-            data=[{'key': 'a'}],
-            indexed_field='text',
-            is_public=True,
-            name='test_map_text_errors',
-            description='test map description',
-            reset_project_if_exists=True,
-        )
-    AtlasProject(name='test_map_text_errors').delete()
-
 def test_map_embedding_progressive():
     num_embeddings = 100
     embeddings = np.random.rand(num_embeddings, 10)
     data = [{'field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 0.0} for i in range(len(embeddings))]
 
     project = atlas.map_embeddings(
         embeddings=embeddings,
@@ -171,16 +132,18 @@
             build_topic_model=False,
             is_public=True,
             add_datums_if_exists=True,
         )
     with pytest.raises(Exception):
         # Try adding a bad field.
         with current_project.wait_for_project_lock():
-            data = [{'invalid_field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 1.0} for i in
-                    range(len(embeddings))]
+            data = [
+                {'invalid_field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 1.0}
+                for i in range(len(embeddings))
+            ]
 
             current_project = AtlasProject(name=project.name)
 
             with current_project.wait_for_project_lock():
                 project = atlas.map_embeddings(
                     embeddings=embeddings,
                     name=current_project.name,
@@ -195,122 +158,139 @@
     current_project.delete()
 
 
 def test_topics():
     num_embeddings = 100
     embeddings = np.random.rand(num_embeddings, 10)
     texts = ['foo', 'bar', 'baz', 'bat']
-    data = [{'field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 0.0, 'text': texts[i % 4]}
-            for i in range(len(embeddings))]
+    data = [
+        {'field': str(uuid.uuid4()), 'id': str(uuid.uuid4()), 'upload': 0.0, 'text': texts[i % 4]}
+        for i in range(len(embeddings))
+    ]
 
-    p = atlas.map_embeddings(
+    project = atlas.map_embeddings(
         embeddings=embeddings,
         name='test_topics',
         id_field='id',
         data=data,
         is_public=True,
         build_topic_model=True,
         topic_label_field='text',
         reset_project_if_exists=True,
     )
 
-    with p.wait_for_project_lock():
-        assert len(p.maps[0].get_topic_data()) > 0
+    with project.wait_for_project_lock():
+        assert len(project.maps[0].topics.metadata) > 0
 
         q = np.random.random((3, 10))
-        assert len(p.maps[0].vector_search_topics(q, depth=1, k=3)['topics']) == 3
-        p.delete()
+        assert len(project.maps[0].topics.vector_search_topics(q, depth=1, k=3)['topics']) == 3
+
+        assert isinstance(project.maps[0].topics.group_by_topic(topic_depth=1), list)
+
+        project.delete()
 
 
 words = [
-    'foo', 'bar', 'baz', 'bat',
-    'glorp', 'gloop', 'glib', 'glub',
-    'florp', 'floop', 'flib', 'flub',
-    'blorp', 'bloop', 'blib', 'blub',
-    'slorp', 'sloop', 'slib', 'slub',
-    'clorp', 'cloop', 'clib', 'club',
-    'plorp', 'ploop', 'plib', 'plub',
-    'zlorp', 'zloop', 'zlib', 'zlub',
-    'xlorp', 'xloop', 'xlib', 'xlub',
-    'vlorp', 'vloop', 'vlib', 'vlub',
-    'nlorp', 'nloop', 'nlib', 'nlub',
-    'mlorp', 'mloop', 'mlib', 'mlub'
+    'foo',
+    'bar',
+    'baz',
+    'bat',
+    'glorp',
+    'gloop',
+    'glib',
+    'glub',
+    'florp',
+    'floop',
+    'flib',
+    'flub',
+    'blorp',
+    'bloop',
+    'blib',
+    'blub',
+    'slorp',
+    'sloop',
+    'slib',
+    'slub',
+    'clorp',
+    'cloop',
+    'clib',
+    'club',
+    'plorp',
+    'ploop',
+    'plib',
+    'plub',
+    'zlorp',
+    'zloop',
+    'zlib',
+    'zlub',
+    'xlorp',
+    'xloop',
+    'xlib',
+    'xlub',
+    'vlorp',
+    'vloop',
+    'vlib',
+    'vlub',
+    'nlorp',
+    'nloop',
+    'nlib',
+    'nlub',
+    'mlorp',
+    'mloop',
+    'mlib',
+    'mlub',
 ]
 
 
 def test_interactive_workflow():
-    p = AtlasProject(name='UNITTEST1',
-                     modality='text',
-                     unique_id_field='id',
-                     reset_project_if_exists=True
-                     )
+    p = AtlasProject(name='UNITTEST1', modality='text', unique_id_field='id', reset_project_if_exists=True)
 
     p.add_text(data=[{'text': random.choice(words), 'id': i} for i in range(100)])
 
-    p.create_index(name='UNITTEST1',
-                   indexed_field='text',
-                   build_topic_model=True
-                   )
+    p.create_index(name='UNITTEST1', indexed_field='text', build_topic_model=True)
 
     assert p.total_datums == 100
 
     # Test ability to add more data to a project and have the ids coerced.
     with p.wait_for_project_lock():
         p.add_text(data=[{'text': random.choice(words), 'id': i} for i in range(100, 200)])
-        p.create_index(name='UNITTEST1',
-                       indexed_field='text',
-                       build_topic_model=True
-                       )
+        p.create_index(name='UNITTEST1', indexed_field='text', build_topic_model=True)
         assert p.total_datums == 200
 
     with p.wait_for_project_lock():
         p.delete()
 
+
 def test_flawed_ids():
     """
     Check that null and empty strings do not block an index build.
     """
-    p = AtlasProject(
-        name='test_flawed_ids',
-        modality='text',
-        unique_id_field='id',
-        reset_project_if_exists=True
-    )
+    p = AtlasProject(name='test_flawed_ids', modality='text', unique_id_field='id', reset_project_if_exists=True)
 
     elements = []
     for i in range(10):
         if i % 3 == 0 and i % 5 == 0:
             elements.append({'text': 'fizzbuzz', 'id': str(i)})
         elif i % 3 == 0:
             elements.append({'text': 'fizz', 'id': str(i)})
         elif i % 5 == 0:
             elements.append({'text': 'buzz', 'id': str(i)})
     p.add_text(data=elements)
     with pytest.raises(ValueError):
-        p.add_text(data=[{
-            'text': 'fizzbuzz',
-            'id': None
-        }])
+        p.add_text(data=[{'text': 'fizzbuzz', 'id': None}])
     with pytest.raises(ValueError):
-        p.add_text(data=[{
-            'text': 'fizzbuzz',
-            'id': 'A' * 100
-        }])
+        p.add_text(data=[{'text': 'fizzbuzz', 'id': 'A' * 100}])
     p.delete()
 
+
 def test_weird_inputs():
     """
     Check that null and empty strings do not block an index build.
     """
-    p = AtlasProject(
-        name='test_weird_inputs',
-        modality='text',
-        unique_id_field='id',
-        reset_project_if_exists=True
-    )
+    p = AtlasProject(name='test_weird_inputs', modality='text', unique_id_field='id', reset_project_if_exists=True)
 
     elements = []
     for i in range(20):
         if i % 3 == 0 and i % 5 == 0:
             elements.append({'text': 'fizzbuzz', 'id': str(i)})
         elif i % 3 == 0:
             elements.append({'text': 'fizz', 'id': str(i)})
@@ -319,15 +299,59 @@
         elif i % 7 == 0:
             elements.append({'text': None, 'id': str(i)})
         elif i % 2 == 0:
             elements.append({'text': '', 'id': str(i)})
         else:
             elements.append({'text': 'foo', 'id': str(i)})
     p.add_text(data=elements)
-    p.create_index(
-        name='test_weird_inputs',
-        indexed_field='text',
-        build_topic_model=True
-    )
+    p.create_index(name='test_weird_inputs', indexed_field='text', build_topic_model=True)
     with p.wait_for_project_lock():
         assert True
-    p.delete()
+    p.delete()
+
+
+def test_map_embeddings():
+    num_embeddings = 20
+    embeddings = np.random.rand(num_embeddings, 10)
+    data = [{'field': str(uuid.uuid4()), 'id': str(uuid.uuid4())} for i in range(len(embeddings))]
+
+    project = atlas.map_embeddings(
+        embeddings=embeddings,
+        name='UNITTEST1',
+        id_field='id',
+        data=data,
+        is_public=True,
+        reset_project_if_exists=True,
+    )
+
+    map = project.get_map(name='UNITTEST1')
+
+    time.sleep(10)
+    with tempfile.TemporaryDirectory() as td:
+        retrieved_embeddings = map.embeddings.download_embeddings(td)
+
+    assert project.total_datums == num_embeddings
+
+    project = AtlasProject(name='UNITTEST1')
+    map = project.get_map(name='UNITTEST1')
+
+    assert len(map.topics.df) == 20
+
+    assert isinstance(map.topics.hierarchy, dict)
+
+    project.create_index(name='My new index')
+    with project.wait_for_project_lock():
+        neighbors, _ = map.embeddings.vector_search(queries=np.random.rand(1, 10), k=2)
+        assert len(neighbors[0]) == 2
+
+    for map in project.projections:
+        assert map.map_link
+
+    map.tags.add(ids=[data[0]['id']], tags=['my_tag'])
+
+    assert len(map.tags.get_tags()['my_tag']) == 1
+
+    map.tags.remove(ids=[data[0]['id']], tags=['my_tag'])
+
+    assert 'my_tag' not in map.tags.get_tags()
+
+    project.delete()
```

### Comparing `nomic-1.1.9/nomic/utils.py` & `nomic-2.0.0/nomic/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+import base64
 import gc
 import sys
 from uuid import UUID
 
 from wonderwords import RandomWord
 
 
+def b64int(i: int):
+    ibytes = int.to_bytes(i, length=8, byteorder='big').lstrip(b'\x00')
+    if ibytes == b'':
+        ibytes = b'\x00'
+    return base64.b64encode(ibytes).decode('utf8').rstrip('=')
+
+
 def get_random_name():
     random_words = RandomWord()
     return f"{random_words.word(include_parts_of_speech=['adjectives'])}-{random_words.word(include_parts_of_speech=['nouns'])}"
 
 
 def assert_valid_project_id(project_id):
     try:
```

### Comparing `nomic-1.1.9/setup.py` & `nomic-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             'sentencepiece',
             f"transformers @ file://localhost/{os.getcwd()}/bin/transformers-4.28.0.dev0-py3-none-any.whl",
             f"peft @ file://localhost/{os.getcwd()}/bin/peft-0.3.0.dev0-py3-none-any.whl"
         ]
     
 setup(
     name='nomic',
-    version='1.1.9',
+    version='2.0.0',
     url='https://github.com/nomic-ai/nomic',
     description=description,
     long_description=description,
     packages=find_packages(),
     author_email="support@nomic.ai",
     author="nomic.ai",
     classifiers=[
@@ -32,14 +32,15 @@
     install_requires=[
         "click",
         "jsonlines",
         "loguru",
         'rich',
         'requests',
         'numpy',
+        'pandas',
         'pydantic',
         'wonderwords',
         'tqdm',
         'cohere',
         'pyarrow',
     ],
     extras_require={
```

