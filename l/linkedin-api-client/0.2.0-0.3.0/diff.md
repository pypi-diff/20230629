# Comparing `tmp/linkedin_api_client-0.2.0.tar.gz` & `tmp/linkedin_api_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_api_client-0.2.0.tar", max compression
+gzip compressed data, was "linkedin_api_client-0.3.0.tar", max compression
```

## Comparing `linkedin_api_client-0.2.0.tar` & `linkedin_api_client-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0     6447 2023-02-17 18:40:47.225137 linkedin_api_client-0.2.0/LICENSE.md
--rw-r--r--   0        0        0    36444 2023-03-10 19:41:49.191801 linkedin_api_client-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-03-27 23:07:59.897197 linkedin_api_client-0.2.0/linkedin_api/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:19:19.101176 linkedin_api_client-0.2.0/linkedin_api/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-02-08 20:19:19.101372 linkedin_api_client-0.2.0/linkedin_api/clients/auth/__init__.py
--rw-r--r--   0        0        0     9015 2023-02-17 18:40:47.232931 linkedin_api_client-0.2.0/linkedin_api/clients/auth/client.py
--rw-r--r--   0        0        0     3896 2023-02-17 18:40:47.233473 linkedin_api_client-0.2.0/linkedin_api/clients/auth/response.py
--rw-r--r--   0        0        0     3245 2023-02-17 18:40:47.234030 linkedin_api_client-0.2.0/linkedin_api/clients/auth/response_formatter.py
--rw-r--r--   0        0        0        0 2023-02-17 17:32:06.508947 linkedin_api_client-0.2.0/linkedin_api/clients/auth/utils/__init__.py
--rw-r--r--   0        0        0      700 2023-02-17 18:40:47.234676 linkedin_api_client-0.2.0/linkedin_api/clients/auth/utils/oauth.py
--rw-r--r--   0        0        0        0 2023-02-08 20:19:19.103222 linkedin_api_client-0.2.0/linkedin_api/clients/common/__init__.py
--rw-r--r--   0        0        0      615 2023-03-27 23:07:59.898505 linkedin_api_client-0.2.0/linkedin_api/clients/common/response.py
--rw-r--r--   0        0        0      681 2023-02-17 18:40:47.235957 linkedin_api_client-0.2.0/linkedin_api/clients/common/response_formatter.py
--rw-r--r--   0        0        0        0 2023-02-08 20:19:19.104303 linkedin_api_client-0.2.0/linkedin_api/clients/restli/__init__.py
--rw-r--r--   0        0        0    47395 2023-02-17 18:40:47.236798 linkedin_api_client-0.2.0/linkedin_api/clients/restli/client.py
--rw-r--r--   0        0        0     8177 2023-03-27 23:07:59.899208 linkedin_api_client-0.2.0/linkedin_api/clients/restli/response.py
--rw-r--r--   0        0        0     7919 2023-02-17 18:40:47.237828 linkedin_api_client-0.2.0/linkedin_api/clients/restli/response_formatter.py
--rw-r--r--   0        0        0      166 2023-02-17 18:40:47.238263 linkedin_api_client-0.2.0/linkedin_api/clients/restli/types.py
--rw-r--r--   0        0        0        0 2023-02-17 17:32:06.509703 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/__init__.py
--rw-r--r--   0        0        0     3572 2023-03-27 23:07:59.899911 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/api.py
--rw-r--r--   0        0        0       55 2023-03-29 16:01:31.777302 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/decoder.py
--rw-r--r--   0        0        0     1345 2023-02-17 18:40:47.239996 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/encoder.py
--rw-r--r--   0        0        0     4115 2023-02-17 18:40:47.240949 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/query_tunneling.py
--rw-r--r--   0        0        0     1889 2023-02-17 18:40:47.241702 linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/restli.py
--rw-r--r--   0        0        0        0 2023-02-08 20:19:19.108572 linkedin_api_client-0.2.0/linkedin_api/common/__init__.py
--rw-r--r--   0        0        0     1659 2023-02-17 18:40:47.242298 linkedin_api_client-0.2.0/linkedin_api/common/constants.py
--rw-r--r--   0        0        0      281 2023-03-29 16:01:31.778326 linkedin_api_client-0.2.0/linkedin_api/common/errors.py
--rw-r--r--   0        0        0      981 2023-03-29 16:10:28.902818 linkedin_api_client-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    38336 1970-01-01 00:00:00.000000 linkedin_api_client-0.2.0/setup.py
--rw-r--r--   0        0        0    37515 1970-01-01 00:00:00.000000 linkedin_api_client-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6447 2023-02-17 18:40:47.225137 linkedin_api_client-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0    36530 2023-06-28 16:44:21.006756 linkedin_api_client-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 23:07:59.897197 linkedin_api_client-0.3.0/linkedin_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:19:19.101176 linkedin_api_client-0.3.0/linkedin_api/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:19:19.101372 linkedin_api_client-0.3.0/linkedin_api/clients/auth/__init__.py
+-rw-r--r--   0        0        0     9015 2023-02-17 18:40:47.232931 linkedin_api_client-0.3.0/linkedin_api/clients/auth/client.py
+-rw-r--r--   0        0        0     3896 2023-02-17 18:40:47.233473 linkedin_api_client-0.3.0/linkedin_api/clients/auth/response.py
+-rw-r--r--   0        0        0     3245 2023-02-17 18:40:47.234030 linkedin_api_client-0.3.0/linkedin_api/clients/auth/response_formatter.py
+-rw-r--r--   0        0        0        0 2023-02-17 17:32:06.508947 linkedin_api_client-0.3.0/linkedin_api/clients/auth/utils/__init__.py
+-rw-r--r--   0        0        0      700 2023-02-17 18:40:47.234676 linkedin_api_client-0.3.0/linkedin_api/clients/auth/utils/oauth.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:19:19.103222 linkedin_api_client-0.3.0/linkedin_api/clients/common/__init__.py
+-rw-r--r--   0        0        0      615 2023-03-27 23:07:59.898505 linkedin_api_client-0.3.0/linkedin_api/clients/common/response.py
+-rw-r--r--   0        0        0      681 2023-02-17 18:40:47.235957 linkedin_api_client-0.3.0/linkedin_api/clients/common/response_formatter.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:19:19.104303 linkedin_api_client-0.3.0/linkedin_api/clients/restli/__init__.py
+-rw-r--r--   0        0        0    47341 2023-06-29 15:52:52.500227 linkedin_api_client-0.3.0/linkedin_api/clients/restli/client.py
+-rw-r--r--   0        0        0     8439 2023-04-11 02:49:19.743235 linkedin_api_client-0.3.0/linkedin_api/clients/restli/response.py
+-rw-r--r--   0        0        0     8367 2023-06-29 15:52:52.502046 linkedin_api_client-0.3.0/linkedin_api/clients/restli/response_formatter.py
+-rw-r--r--   0        0        0      166 2023-02-17 18:40:47.238263 linkedin_api_client-0.3.0/linkedin_api/clients/restli/types.py
+-rw-r--r--   0        0        0        0 2023-02-17 17:32:06.509703 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-29 15:52:52.502829 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/api.py
+-rw-r--r--   0        0        0     7982 2023-06-29 15:52:52.503389 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/decoder.py
+-rw-r--r--   0        0        0     2750 2023-04-11 02:49:19.745719 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/encoder.py
+-rw-r--r--   0        0        0     4109 2023-06-29 15:52:52.503864 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/query_tunneling.py
+-rw-r--r--   0        0        0     2418 2023-04-11 02:49:19.746373 linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/restli.py
+-rw-r--r--   0        0        0        0 2023-02-08 20:19:19.108572 linkedin_api_client-0.3.0/linkedin_api/common/__init__.py
+-rw-r--r--   0        0        0     1871 2023-04-11 02:49:19.746951 linkedin_api_client-0.3.0/linkedin_api/common/constants.py
+-rw-r--r--   0        0        0      399 2023-06-29 15:52:52.504392 linkedin_api_client-0.3.0/linkedin_api/common/errors.py
+-rw-r--r--   0        0        0      981 2023-06-29 15:53:26.752134 linkedin_api_client-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    37601 1970-01-01 00:00:00.000000 linkedin_api_client-0.3.0/PKG-INFO
```

### Comparing `linkedin_api_client-0.2.0/LICENSE.md` & `linkedin_api_client-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/README.md` & `linkedin_api_client-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
   access_token=<THREE_LEGGED_ACCESS_TOKEN>
 )
 print(response.entity)
 ```
 
 ### Finder Request Example
 
-Here is a more non-trivial example to [find ad accounts](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-accounts?#search-for-accounts) by some search critiera. This requires a 3-legged access token with the "r_ads" scope, which is included with the Advertising APIs product.
+Here is a more non-trivial example to [find ad accounts](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-accounts?#search-for-accounts) by some search criteria. This requires a 3-legged access token with the "r_ads" scope, which is included with the Advertising APIs product.
 
 The "search" query parameter in this case is not a primitive, but a complex object, which we represent as a dictionary. The client will handle the correct URL-encoding. This is a versioned API call, so we also need to provide the version string in the "YYYYMM" format.
 
 ```python
 from linkedin_api.clients.restli.client import RestliClient
 
 restli_client = RestliClient()
@@ -717,15 +717,16 @@
 
 ##### `class CreateResponse`
 
 Base class: [BaseRestliResponse](#class-baserestliresponse)
 
 | Properties | Type | Description |
 |---|---|---|
-| `entity_id` | str | The encoded entity id |
+| `entity_id` | str | The reduced-encoded entity id. |
+| `decoded_entity_id` | Union[str, Dict[str,Any]] | The decoded entity id. |
 | `entity` | Dict[str,Any] | Optional created entity. Some APIs support returning the created entity to eliminate the need for a subsequent GET call. |
 
 ##### `class BatchCreateResponse`
 
 Base class: [BaseRestliResponse](#class-baserestliresponse)
 
 | Properties | Type | Description |
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/auth/client.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/auth/client.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/auth/response.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/auth/response.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/auth/response_formatter.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/auth/response_formatter.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/auth/utils/oauth.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/auth/utils/oauth.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/common/response.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/common/response.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/common/response_formatter.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/common/response_formatter.py`

 * *Files identical despite different names*

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/client.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
 import copy
 from typing import Union, Dict, Any, List, Optional, Type, Tuple, TypeVar
-from linkedin_api.clients.common.response import BaseResponse
 import linkedin_api.clients.restli.utils.api as apiutils
 import linkedin_api.clients.restli.utils.encoder as encoder
 from linkedin_api.clients.restli.utils.restli import (
     encode_query_params_for_get_requests,
 )
 from linkedin_api.clients.restli.utils.query_tunneling import (
     maybe_apply_query_tunneling_get_requests,
@@ -63,15 +62,15 @@
 
     def get(
         self,
         *,
         resource_path: str,
         access_token: str,
         path_keys: Optional[Dict[str, Any]] = None,
-        query_params: Optional[Dict[str, Any]] = {},
+        query_params: Optional[Dict[str, Any]] = None,
         version_string: Optional[str] = None
     ) -> GetResponse:
         """
         Makes a Rest.li GET request to fetch the specified entity on a resource. This method will perform query
         tunneling if necessary.
 
         Args:
@@ -504,15 +503,15 @@
         self,
         *,
         resource_path: str,
         entities: List[RestliEntity],
         ids: List[RestliEntityId],
         access_token: str,
         path_keys: Optional[Dict[str, Any]] = None,
-        query_params: Optional[Dict[str, Any]] = {},
+        query_params: Optional[Dict[str, Any]] = None,
         version_string: Optional[str] = None
     ) -> BatchUpdateResponse:
         """
         Makes a Rest.li BATCH_UPDATE request to update multiple entities in a single call.
 
         Args:
             resource_path (str): The resource path after the base URL, beginning with a forward slash. If the path contains keys, add curly-brace placeholders for the keys and specify the path key-value map in the `path_keys` argument.
@@ -685,15 +684,15 @@
 
     def delete(
         self,
         *,
         resource_path: str,
         access_token: str,
         path_keys: Optional[Dict[str, Any]] = None,
-        query_params: Optional[Dict[str, Any]] = {},
+        query_params: Optional[Dict[str, Any]] = None,
         version_string: Optional[str] = None
     ) -> BaseRestliResponse:
         """
         Makes a Rest.li DELETE request to delete an entity.
 
         Args:
             resource_path (str): The resource path after the base URL, beginning with a forward slash. If the path contains keys, add curly-brace placeholders for the keys and specify the path key-value map in the `path_keys` argument.
@@ -730,15 +729,15 @@
     def batch_delete(
         self,
         *,
         resource_path: str,
         ids: List[RestliEntityId],
         access_token: str,
         path_keys: Optional[Dict[str, Any]] = None,
-        query_params: Optional[Dict[str, Any]] = {},
+        query_params: Optional[Dict[str, Any]] = None,
         version_string: Optional[str] = None
     ) -> BatchDeleteResponse:
         """
         Makes a Rest.li BATCH_DELETE request to delete multiple entities at once.
 
         Args:
             resource_path (str): The resource path after the base URL, beginning with a forward slash. If the path contains keys, add curly-brace placeholders for the keys and specify the path key-value map in the `path_keys` argument.
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/response.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/response.py`

 * *Files 5% similar despite different names*

```diff
@@ -164,24 +164,30 @@
     def __init__(
         self,
         status_code: int,
         url: str,
         headers: Dict[str, str],
         response: Response,
         entity_id: Optional[EncodedEntityId] = None,
+        decoded_entity_id: Optional[Union[str, Dict[str, Any]]] = None,
         entity: Optional[RestliEntity] = None,
     ):
         super().__init__(
             status_code=status_code, headers=headers, url=url, response=response
         )
         self.entity_id = entity_id
         """
-    The encoded entity id of the created entity
+    The reduced-encoded entity id of the created entity (e.g. "urn%3Ali%3Aapp%3A123")
     """
 
+        self.decoded_entity_id = decoded_entity_id
+        """
+        The decoded entity id of the created entity (e.g. "urn:li:app:123")
+        """
+
         self.entity = entity
         """
     Optional created entity. Some APIs support returning the created entity to eliminate the need for a subsequent GET call.
     """
 
 
 class BatchCreateResult:
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/response_formatter.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/response_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,31 @@
+from typing import Dict
+
 from linkedin_api.clients.common.response_formatter import (
     BaseResponseFormatter,
     wrap_format_exception,
 )
-from linkedin_api.clients.restli.response import *
+from linkedin_api.clients.restli.response import (
+    GetResponse,
+    BatchGetResponse,
+    CollectionResponse,
+    Paging,
+    BatchFinderResponse,
+    BatchFinderResult,
+    CreateResponse,
+    BatchCreateResponse,
+    BatchCreateResult,
+    UpdateResponse,
+    BatchUpdateResponse,
+    BatchUpdateResult,
+    BaseRestliResponse,
+    BatchDeleteResponse,
+    BatchDeleteResult,
+    ActionResponse,
+)
 from linkedin_api.clients.restli.utils.restli import get_created_entity_id
 from requests import Response
 
 
 class GetResponseFormatter(BaseResponseFormatter[GetResponse]):
     @classmethod
     @wrap_format_exception
@@ -105,15 +124,16 @@
             json_data = None
 
         return CreateResponse(
             status_code=response.status_code,
             url=response.url,
             headers=response.headers,
             response=response,
-            entity_id=get_created_entity_id(response, True),
+            entity_id=get_created_entity_id(response, False),
+            decoded_entity_id=get_created_entity_id(response, True),
             entity=json_data if json_data else None,
         )
 
 
 class BatchCreateResponseFormatter(BaseResponseFormatter[BatchCreateResponse]):
     @classmethod
     @wrap_format_exception
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/api.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import linkedin_api.common.constants as constants
-from importlib.metadata import version
 from linkedin_api.clients.restli.utils.encoder import encode
 from typing import Dict, Any, Optional
 from linkedin_api.common.errors import InvalidArgumentError
 import re
 
+import sys
+
+if sys.version_info >= (3, 8):
+    from importlib.metadata import version
+else:
+    from importlib_metadata import version
+
+
 __version__ = version("linkedin-api-client")
 
 
 def get_rest_api_base_url(version_string):
     if version_string:
         return constants.VERSIONED_BASE_URL
     else:
@@ -65,15 +72,15 @@
 
     if version_string:
         base_url = constants.VERSIONED_BASE_URL
     else:
         base_url = constants.NON_VERSIONED_BASE_URL
 
     # Validate resource_path and path_keys
-    num_path_keys = 0 if path_keys == None else len(path_keys.keys())
+    num_path_keys = 0 if path_keys is None else len(path_keys.keys())
     if path_keys:
         encoded_path_keys = {k: encode(v) for (k, v) in path_keys.items()}
     else:
         encoded_path_keys = {}
 
     placeholders = re.findall(r"{(.*?)}", resource_path)
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/query_tunneling.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/query_tunneling.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     RESTLI_METHOD_TO_HTTP_METHOD_MAP,
     HEADERS,
 )
 import linkedin_api.clients.restli.utils.api as apiutils
 import random
 import string
 import json
-from typing import Optional, Type
+from typing import Optional
 
 MAX_QUERY_STRING_LENGTH = 4000
 
 
 def is_query_tunneling_required(encoded_query_param_string):
     return (
         encoded_query_param_string
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/clients/restli/utils/restli.py` & `linkedin_api_client-0.3.0/linkedin_api/clients/restli/utils/restli.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,34 @@
 from linkedin_api.clients.restli.utils.decoder import reduced_decode
 from linkedin_api.common.constants import HEADERS
 from typing import Dict, Any, Optional
 import copy
 from requests import Response
 
 
-def get_created_entity_id(response: Response, decode: bool = True):
+def get_created_entity_id(response: Response, decode: bool = False) -> Any:
+    """
+    Return the created entity id. This is present in the response header for
+    a CREATE request. Can optionally decode the entity id value; otherwise this will
+    return the reduced-encoded string.
+
+    Args:
+        response (Response): the response object
+        decode (bool, optional): Flag whether to decode the id. Defaults to False.
+
+    Returns:
+        Any: The created entity id
+    """
     reduced_encoded_entity_id = response.headers.get(
         HEADERS.CREATED_ENTITY_ID.value, None
     )
-    return reduced_decode(reduced_encoded_entity_id)
+    if decode and reduced_encoded_entity_id is not None:
+        return reduced_decode(reduced_encoded_entity_id)
+    else:
+        return reduced_encoded_entity_id
 
 
 def encode_query_params_for_get_requests(query_params: Optional[Dict[str, Any]]) -> str:
     """Encodes query params for HTTP GET requests
 
     This wrapper function on top of encoder.paramEncode is needed specifically to handle the
     "fields" query parameter for field projections. Although Rest.li protocol version 2.0.0 should
```

### Comparing `linkedin_api_client-0.2.0/linkedin_api/common/constants.py` & `linkedin_api_client-0.3.0/linkedin_api/common/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -60,7 +60,18 @@
     "BATCH_CREATE": "POST",
     "PARTIAL_UPDATE": "POST",
     "BATCH_PARTIAL_UPDATE": "POST",
     "ACTION": "POST",
     "DELETE": "DELETE",
     "BATCH_DELETE": "DELETE",
 }
+
+# Rest.li special characters
+LIST_PREFIX = "List("
+LIST_SUFFIX = ")"
+LIST_ITEM_SEP = ","
+OBJ_PREFIX = "("
+OBJ_SUFFIX = ")"
+OBJ_KEY_VAL_SEP = ":"
+OBJ_KEY_VAL_PAIR_SEP = ","
+LEFT_BRACKET = "("
+RIGHT_BRACKET = ")"
```

### Comparing `linkedin_api_client-0.2.0/pyproject.toml` & `linkedin_api_client-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "linkedin-api-client"
-version = "0.2.0"
+version = "0.3.0"
 packages = [
     { include = "linkedin_api" }
 ]
 authors = ["Steven Shimizu <sshimizu@linkedin.com>"]
 description = "Official Python client library for LinkedIn APIs"
 homepage = "https://github.com/linkedin-developers/linkedin-api-python-client"
 repository = "https://github.com/linkedin-developers/linkedin-api-python-client"
```

### Comparing `linkedin_api_client-0.2.0/setup.py` & `linkedin_api_client-0.3.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,980 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: linkedin-api-client
+Version: 0.3.0
+Summary: Official Python client library for LinkedIn APIs
+Home-page: https://github.com/linkedin-developers/linkedin-api-python-client
+License: Proprietary
+Keywords: linkedin,api,rest.li
+Author: Steven Shimizu
+Author-email: sshimizu@linkedin.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Requires-Dist: requests
+Project-URL: Documentation, https://github.com/linkedin-developers/linkedin-api-python-client
+Project-URL: Repository, https://github.com/linkedin-developers/linkedin-api-python-client
+Description-Content-Type: text/markdown
 
-packages = \
-['linkedin_api',
- 'linkedin_api.clients',
- 'linkedin_api.clients.auth',
- 'linkedin_api.clients.auth.utils',
- 'linkedin_api.clients.common',
- 'linkedin_api.clients.restli',
- 'linkedin_api.clients.restli.utils',
- 'linkedin_api.common']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests']
-
-setup_kwargs = {
-    'name': 'linkedin-api-client',
-    'version': '0.2.0',
-    'description': 'Official Python client library for LinkedIn APIs',
-    'long_description': '# LinkedIn API Python Client\n\n## Overview\n\nThis library provides a thin Python client for making requests to LinkedIn APIs, utilizing the Python [requests](https://pypi.org/project/requests/) HTTP client library. LinkedIn\'s APIs are built on the [Rest.li](https://linkedin.github.io/rest.li/) framework with additional LinkedIn-specific constraints, which results in a robust yet complex protocol that can be challenging to implement correctly.\n\nThis library helps reduce this complexity by formatting requests correctly, providing proper request headers, and providing interfaces to develop against for responses. The library also provides an auth client for inspecting, generating, and refreshing access tokens, along with other helpful utilities.\n\n> :warning: This API client library is currently in beta and is subject to change. It may contain bugs, errors, or other issues that we are working to resolve. Use of this library is at your own risk. Please use caution when using it in production environments and be prepared for the possibility of unexpected behavior. We welcome any feedback or reports of issues that you may encounter while using this library.\n\n### Features\n\n- Generic support for all Rest.li methods used in LinkedIn APIs\n- Supports Rest.li protocol version 2.0.0\n- Provide interfaces for request options/response payloads\n- Built-in parameter encoding\n- Utilities (e.g. URN handling, encoding)\n- Supports versioned APIs\n- Automatic query tunneling of requests\n- 2-legged and 3-legged OAuth2 support\n\n### Table of Contents\n\n- [Requirements](#requirements)\n- [Installation](#installation)\n- [Getting Started](#getting-started)\n  - [Pre-requisites](#pre-requisites)\n  - [Simple API Request Example](#simple-api-request-example)\n  - [Finder Request Example](#finder-request-example)\n  - [More Examples](#more-examples)\n- [API Reference](#api-reference)\n  - [RestliClient](#class-restliclient)\n    - [Constructor](#constructor)\n    - [Properties](#properties)\n    - [Methods](#methods)\n      - [`get()`](#get-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_get()`](#batch_get-resource_path-ids-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`get_all()`](#get_all-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`finder()`](#finder-resource_path-finder_name-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_finder()`](#batch_finder-resource_path-finder_name-finder_criteria-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`create()`](#create-resource_path-entity-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_create()`](#batch_create-resource_path-entities-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`update()`](#update-resource_path-entity-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_update()`](#batch_update-resource_path-ids-entities-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`partial_update()`](#partial_update-resource_path-patch_set_object-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_partial_update()`](#batch_partial_update-resource_path-ids-patch_set_objects-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`delete()`](#delete-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`batch_delete()`](#batch_delete-resource_path-ids-access_token-path_keysnone-query_paramsnone-version_stringnone)\n      - [`action()`](#action-resource_path-action_name-access_token-action_paramsnone-path_keysnone-query_paramsnone-version_stringnone)\n  - [AuthClient](#class-authclient)\n    - [Constructor](#constructor-1)\n    - [Properties](#properties-1)\n    - [Methods](#methods-1)\n      - [`generate_member_auth_url()`](#generate_member_auth_url-scopes-statenone)\n      - [`exchange_auth_code_for_access_token()`](#exchange_auth_code_for_access_token-code)\n      - [`exchange_refresh_token_for_access_token()`](#exchange_refresh_token_for_access_token-refresh_token)\n      - [`get_two_legged_access_token()`](#get_two_legged_access_token-)\n      - [`introspect_access_token()`](#introspect_access_token-access_token)\n- [List of dependencies](#list-of-dependencies)\n\n\n## Requirements\n\n- Python >= 3.7\n\n\n## Installation\n\n```sh\npip install linkedin-api-client\n```\n\n## Getting Started\n\n### Pre-requisites\n\n1. Create or use an existing developer application from the [LinkedIn Developer Portal](https://www.linkedin.com/developers/apps/)\n2. Request access to the Sign In With LinkedIn API product. This is a self-serve product that will be provisioned immediately to your application.\n3. Generate a 3-legged access token using the Developer Portal [token generator tool](https://www.linkedin.com/developers/tools/oauth/token-generator), selecting the r_liteprofile scope.\n\n### Simple API Request Example\n\nHere is an example of using the client to make a simple GET request to [fetch the current user\'s profile](https://learn.microsoft.com/en-us/linkedin/consumer/integrations/self-serve/sign-in-with-linkedin#retrieving-member-profiles). This requires a 3-legged access token with the "r_liteprofile" scope, which is included with the Sign In With LinkedIn API product.\n\n```python\nfrom linkedin_api.clients.restli.client import RestliClient\n\nrestli_client = RestliClient()\n\nresponse = restli_client.get(\n  resource_path="/me",\n  access_token=<THREE_LEGGED_ACCESS_TOKEN>\n)\nprint(response.entity)\n```\n\n### Finder Request Example\n\nHere is a more non-trivial example to [find ad accounts](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-accounts?#search-for-accounts) by some search critiera. This requires a 3-legged access token with the "r_ads" scope, which is included with the Advertising APIs product.\n\nThe "search" query parameter in this case is not a primitive, but a complex object, which we represent as a dictionary. The client will handle the correct URL-encoding. This is a versioned API call, so we also need to provide the version string in the "YYYYMM" format.\n\n```python\nfrom linkedin_api.clients.restli.client import RestliClient\n\nrestli_client = RestliClient()\n\nresponse = restli_client.finder(\n  resource_path="/adAccounts",\n  finder_name="search",\n  query_params={\n    "search": {\n      "status": {\n        "values": ["ACTIVE", "DRAFT"]\n      },\n      "reference": {\n        "values": ["urn:li:organization:123"]\n      },\n      "test": True\n    }\n  },\n  version_string="202212",\n  acccess_token=<THREE_LEGGED_ACCESS_TOKEN>\n)\nad_accounts = response.elements\n```\n\n### More Examples\n\nThere are more examples of using the client in [/examples](examples/) directory.\n\n\n## API Reference\n\n### `class RestliClient`\n\nThe Rest.li API client defines instance methods for all the Rest.li methods which are used by LinkedIn APIs. All calls are blocking.\n\nRest.li defines a standard set of methods that can operate on a resource, each of which maps to an HTTP method. Depending on the resource, some Rest.li methods are not applicable or not implemented. Read the API docs to determine what Rest.li method is applicable and the relevant request parameters.\n\n#### Constructor\n\nAn instance of the API client must be created before using. This creates a session object that will be used for making all subsequent requests.\n\n```python\nfrom linkedin_api.clients.restli.client import RestliClient\n\nrestli_client = RestliClient()\n```\n\nThe Requests library [session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) object is accessible to configure any additional global settings (e.g. configuring event hooks).\n\n```python\nrestli_client.session.hooks = { \'response\': [do_something_fn, do_something_2_fn] }\n```\n\n#### Properties\n\n| Property | Description |\n|---|---|\n| `session` | The session object used for making http requests. This is exposed to allow for additional configuration (e.g. adding custom request/response event hooks). |\n\n#### Methods\n\n##### Base Request Parameters\n\nAll Rest.li request methods of the API client support the following request parameters:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `resource_path` | str | Yes | <p>The resource path after the base URL, beginning with a forward slash. If the path contains keys, add curly-brace placeholders for the keys and specify the path key-value map in the `path_keys` argument.</p><p>Examples:</p><ul><li>`resource_path="/me"`</li><li>`resource_path="/adAccounts/{id}"`</li><li>`resource_path="/socialActions/{actionUrn}/comments/{commentId}"`</li><li>`resource_path="/campaignConversions/{key}`</li></ul>|\n| `access_token` | str | Yes | The access token that should provide the application access to the specified API |\n| `path_keys` | Dict[str,Any] | No | <p>If there are path keys that are part of the `resource_path` argument, the key placeholders must be specified in the provided `path_keys` map. The path key values can be strings, numbers, or objects (dictionaries), and these will be properly encoded.</p><p>Examples:</p><p><ul><li>`path_keys={"id": 123"}`</li><li>`path_keys={"actionUrn":"urn:li:share:123","commentId":987`}</li><li>`path_keys={"key": {"campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456"}}`</li></ul></p> |\n| `query_params` | Dict[str,Any] | No | A map of query parameters. The query parameter values (strings, lists, objects) will be correctly encoded by this method, so these should not be encoded. |\n| `version_string` | str | No | An optional version string of the format "YYYYMM" or "YYYYMM.RR". If specified, the version header will be passed and the request will use the versioned APIs base URL |\n\n##### `get (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li GET request to fetch the specified entity on a resource. This method will perform query tunneling if necessary.\n\n**Parameters:**\n\nThis method only uses the [base request parameters](#base-request-parameters) defined above.\n\n**Return value:**\n\nReturns [GetResponse](#class-getresponse) object\n\n**Example:**\n\n```python\nresponse = restli_client.get(\n  resource_path="/adAccounts/{id}"\n  path_keys={ "id": 123 },\n  query_params={ "fields": "id,name" }\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nad_account = response.entity\n```\n\n\n##### `batch_get (resource_path, ids, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_GET request to fetch multiple entities on a resource. This method will perform query tunneling if necessary.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to fetch on the resource. These will be encoded and added to the query parameters. |\n\n**Return value:**\n\nReturns a [BatchGetResponse](#class-batchgetresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.batch_get(\n  resource_path="/adCampaignGroups",\n  ids=[123, 456, 789],\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\ncampaign_groups = response.results.items()\n```\n\n\n##### `get_all (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li GET_ALL request to fetch all entities on a resource.\n\n**Parameters:**\n\nThis method only uses the [base request parameters](#base-request-parameters) defined above.\n\n**Return value:**\n\nReturns [CollectionResponse](#class-collectionresponse) object\n\n**Example:**\n\n```python\nresponse = restli_client.get_all(\n  resource_path="/fieldsOfStudy",\n  query_params={\n    "start": 0,\n    "count": 15\n  },\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nfields_of_study = response.elements\ntotal = response.paging.total\n```\n\n##### `finder (resource_path, finder_name, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li FINDER request to find entities by some specified criteria.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `finder_name` | str | Yes | The Rest.li finder name. This will be added to the request query parameters. |\n\n**Return value:**\n\nReturns a [CollectionResponse](#class-collectionresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.finder(\n  resource_path="/adAccounts",\n  finder_name="search",\n  query_params={\n    "search": {\n        "status": {\n            "values": ["ACTIVE", "DRAFT", "CANCELED"]\n        },\n        "reference": {\n            "values": ["urn:li:organization:123"]\n        },\n        "test": False\n    },\n    "start": 0,\n    "count": 5\n  },\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nad_accounts = response.elements\ntotal = response.paging.total\n```\n\n##### `batch_finder (resource_path, finder_name, finder_criteria, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_FINDER request to find entities by multiple sets of criteria.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `finder_name` | str | Yes | The Rest.li batch finder name (the value of the "bq" query parameter). This will be added to the request query parameters. |\n| `finder_criteria` | Tuple[str, List[Dict[str,Any]]] | Yes | The required batch finder criteria information. This is a tuple with the first value being the batch finder criteria parameter name. The second value is the list of finder param objects. The batch finder results are correspondingly ordered according to this list. The batch finder criteria will be encoded and added to the request query parameters. |\n\n**Return value:**\n\nReturns a [BatchFinderResponse](#class-batchfinderresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.batch_finder(\n  resource_path="/organizationAuthorizations",\n  finder_name="authorizationActionsAndImpersonator",\n  finder_criteria=("authorizationActions", [\n      {\n        "OrganizationRoleAuthorizationAction": {\n          actionType: "ADMINISTRATOR_READ"\n        }\n      },\n      {\n        "OrganizationContentAuthorizationAction": {\n          actionType: "ORGANIC_SHARE_DELETE"\n        }\n      }\n    ]\n  ),\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nadmin_read_authorizations = response.results[0].elements\norganic_share_delete_authorizations = response.results[1].elements\n```\n\n##### `create (resource_path, entity, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li CREATE request to create a new resource entity.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `entity` | Dict[str,Any] | Yes | A dictionary representation of the entity to create |\n\n**Return value:**\n\nReturns a [CreateResponse](#class-createresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.create(\n  resource_path="/adAccountsV2",\n  entity={\n    "name": "Test Ad Account",\n    "type": "BUSINESS",\n    "test": True\n  },\n  access_token=MY_ACCESS_TOKEN\n)\ncreated_entity_id = response.entity_id\n```\n\n##### `batch_create (resource_path, entities, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_CREATE request to create multiple entities in a single call.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `entities` | List[Dict[str,Any]] | Yes | A list of entities to create |\n\n**Return value:**\n\nReturns a [BatchCreateResponse](#class-batchcreateresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.batch_create(\n  resource_path="/adCampaignGroups",\n  entities=[\n    {\n        account: \'urn:li:sponsoredAccount:111\',\n        name: \'CampaignGroupTest1\',\n        status: \'DRAFT\'\n    },\n    {\n        account: \'urn:li:sponsoredAccount:222\',\n        name: \'CampaignGroupTest2\',\n        status: \'DRAFT\'\n    }\n  ],\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\ncreated_elements = response.elements\nfirst_created_element_id = response.elements[0].id\n```\n\n##### `update (resource_path, entity, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li UPDATE request to update an entity (overwriting the entity with the provided value).\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `entity` | Dict[str,Any] | Yes | The value of the updated entity. This will completely overwrite the entity. |\n\n**Return value:**\n\nReturns a [UpdateResponse](#class-updateresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.update(\n  resource_path="/adAccountUsers/{id}",\n  path_keys={\n    "id": {\n      "account": "urn:li:sponsoredAccount:123",\n      "user": "urn:li:person:foobar"\n    }\n  },\n  entity: {\n    "account": "urn:li:sponsoredAccount:123",\n    "user": "urn:li:person:foobar",\n    "role": "VIEWER"\n  },\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nstatus = response.status_code\n```\n\n##### `batch_update (resource_path, ids, entities, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_UPDATE request to update multiple entities in a single call.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The ids of the entities to update |\n| `entities` | List[Dict[str,Any]] | Yes | The values to update the specified entities to. This should be the same order as the `ids` argument. |\n\n**Return value:**\n\nReturns a [BatchUpdateResponse](#class-batchupdateresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.batch_update(\n  resource_path="/campaignConversions",\n  ids=[\n    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456" },\n    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:789" }\n  ],\n  entities=[\n    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456" },\n    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:789" }\n  ],\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nbatch_results = response.results.items()\n```\n\n##### `partial_update (resource_path, patch_set_object, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li PARTIAL_UPDATE request to update part of an entity. Directly specify the patch object to send in the request.\n\nNote: While the Rest.li protocol supports very granular patch objects with setting and deletion of nested properties, most LinkedIn APIs only support partial update on the top-level fields of an entity.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `patch_set_object` | Dict[str,Any] | Yes | The value of the entity with only the modified fields present. This will be sent directly in the request body as `patch: { $set: patch_set_object }`. |\n\n**Return value:**\n\nReturns a [UpdateResponse](#class-updateresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.partial_update(\n  resource_path="/adAccounts/{id}",\n  path_keys={ "id": 123 },\n  patch_set_object: {\n    "name": "TestAdAccountModified",\n    "reference": "urn:li:organization:456"\n  },\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nstatus = response.status_code\n```\n\n##### `batch_partial_update (resource_path, ids, patch_set_objects, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_PARTIAL_UPDATE request to update multiple entities at once, by only providing the fields of the entities that require updating.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to update. These will be encoded and added to the query parameters. |\n| `patch_set_objects` | List[Dict[str,Any]] | Yes | The list of entity values, represented as a dictionary, with only the modified fields present. |\n\n**Return value:**\n\nReturns a [BatchUpdateResponse](#class-batchupdateresponse) object.\n\n**Example:**\n\n```python\nresponse = restli_client.batch_partial_update(\n  resource_path="/adCampaignGroups",\n  ids=["123", "456"],\n  patch_set_objects: [\n    { "status": "ACTIVE" },\n    {\n      "runSchedule": {\n        "start": 1678029270721,\n        "end": 1679029270721\n      }\n    }\n  ],\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nresult_status = response.results["123"].status\n```\n\n##### `delete (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li DELETE request to delete an entity.\n\n**Parameters:**\n\nThis method only uses the [base request parameters](#base-request-parameters) defined above.\n\n**Return value:**\n\nReturns [BaseRestliResponse](#class-baserestliresponse) object\n\n**Example:**\n\n```python\nresponse = restli_client.delete(\n  resource_path="/adAccounts/{id}",\n  path_keys={ "id": 123 },\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nstatus_code = response.status_code\n```\n\n##### `batch_delete (resource_path, ids, access_token, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li BATCH_DELETE request to delete multiple entities at once.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to delete. These will be encoded and added to the query parameters. |\n\n**Return value:**\n\nReturns [BatchDeleteResponse](#class-batchdeleteresponse) object\n\n**Example:**\n\n```python\nresponse = restli_client.batch_delete(\n  resource_path="/adAccounts",\n  ids=["123", "456"],\n  access_token=MY_ACCESS_TOKEN,\n  version_string="202212"\n)\nstatus_code = response.results["123"].status\n```\n\n##### `action (resource_path, action_name, access_token, action_params=None, path_keys=None, query_params=None, version_string=None)`\n\nMakes a Rest.li ACTION request to perform an action on a specified resource. This method is flexible and generally used when the action does not fit within the standard behavior defined by the other Rest.li methods.\n\n**Parameters:**\n\nThe additional parameters besides the [base request parameters](#base-request-parameters) are:\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `action_name` | str | Yes | The action method name. This will be added to the query parameters. |\n| `action_params` | Dict[str,Any] | No | An optional map of action parameters and their values. This will be sent in the request body. |\n\n**Return value:**\n\nReturns [ActionResponse](#class-actionresponse) object\n\n**Example:**\n\n```python\nresponse = restli_client.action(\n  resource_path="/liveAssetActions",\n  action_name="register",\n  action_params={\n    "registerLiveEventRequest": {\n      "owner": "urn:li:person:12345",\n      "recipes": ["urn:li:digitalmediaRecipe:feedshare-live-video"],\n      "region": "WEST_US"\n    }\n  },\n  access_token=MY_ACCESS_TOKEN\n)\nstatus_code = response.status_code\n```\n\n#### Response Classes\n\n##### `class BaseRestliResponse`\n\nAll Rest.li request methods of the API client return a response object subclassed from BaseRestliResponse, containing standard response data, along with the original, raw response object.\n\n| Properties | Type | Description |\n|---|---|---|\n| `status_code` | int | Response status code |\n| `url` | str | The final URL location of the response |\n| `headers` | CaseInsensitiveDict | A case-insensitive dictionary of response headers |\n| `response` | Response | The raw requests.Response object |\n\n##### `class Paging`\n\nPaging metadata class\n\n| Properties | Type | Description |\n|---|---|---|\n| start | int | The start index of returned results (zero-based index) |\n| count | int | The number of results returned in the response |\n| total | int | The total number of results available |\n\n##### `class GetResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `entity` | Union[Dict[str,Any], str, int, bool] | The representation (typically a dictionary) of the retrieved entity, decoded from the json-encoded response content |\n\n##### `class BatchGetResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `results` | Dict[str,Any] | A map of entities that were successfully retrieved, with the key being the encoded entity id, and the value being a dictionary representing the entity |\n| `statuses` | Dict[str,int] | A map of entities and status code, with the key being the encoded entity id, and the value being the status code number value. |\n| `errors` | Dict[str,Any] | A map containing entities that could not be successfully fetched, with the key being the encoded entity id, and the value being the error response. |\n\n##### `class CollectionResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `elements` | List[Dict[str,Any]] | The list of entities returned in the response |\n| `paging` | [Paging](#class-paging) | Optional paging metadata object |\n| `metadata` | Any | Optional response metadata object |\n\n##### `class BatchFinderResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `results` | List[[BatchFinderResult](#class-batchfinderresult)] | The list of finder results, in the same order as the requested batch finder search criteria list |\n\n##### `class BatchFinderResult`\n\n| Properties | Type | Description |\n|---|---|---|\n| `elements` | List[Dict[str,Any]] | The list of entities found for the corresponding finder criteria |\n| `paging` | [Paging](#class-paging) | Optional paging metadata object |\n| `metadata` | Any | Optional response metadata object |\n| `error` | Any | Optional error details if finder call failed |\n| `isError` | bool | Flag if this finder call experienced an error |\n\n##### `class CreateResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `entity_id` | str | The encoded entity id |\n| `entity` | Dict[str,Any] | Optional created entity. Some APIs support returning the created entity to eliminate the need for a subsequent GET call. |\n\n##### `class BatchCreateResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `elements` | List[[BatchCreateResult](#class-batchcreateresult)] | The list of batch create results, corresponding to the order of the `entities` request parameter |\n\n##### `class BatchCreateResult`\n\n| Properties | Type | Description |\n|---|---|---|\n| `status` | int | The status code of the individual create call |\n| `id` | str | The id of the created entity |\n| `error` | Any | Error details if the create call experienced an error |\n\n##### `class UpdateResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `entity` | Dict[str,Any] | Optional entity after the update. Some APIs support returning the updated entity to eliminate the need for a subsequent GET call. |\n\n##### `class BatchUpdateResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `results` | Dict[str,[BatchUpdateResult](#class-batchupdateresult)] | The results map where the keys are the encoded entity ids, and the values are the individual update call results, which includes the status code. |\n\n##### `class BatchUpdateResult`\n\n| Properties | Type | Description |\n|---|---|---|\n| `status` | int | The status code of the individual update call |\n\n##### `class BatchDeleteResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `results` | Dict[str,[BatchDeleteResult](#class-batchdeleteresult)] | The results map where the keys are the encoded entity ids, and the values are the individual delete call results, which includes the status code. |\n\n##### `class BatchDeleteResult`\n\n| Properties | Type | Description |\n|---|---|---|\n| `status` | int | The status code of the delete call |\n\n##### `class ActionResponse`\n\nBase class: [BaseRestliResponse](#class-baserestliresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `value` | Any | The action response value |\n\n\n### `class AuthClient`\n\nWhile we recommend using any of several popular, open-source libraries for robustly managing OAuth 2.0 authentication, we provide a basic Auth Client as a convenience for testing APIs and getting started.\n\n#### Constructor\n\n```python\nfrom linkedin_api.clients.auth.client import AuthClient\n\nauth_client = AuthClient(client_id=MY_CLIENT_ID, client_secret=MY_CLIENT_SECRET, redirect_url=MY_REDIRECT_URL)\n```\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `client_id` | str | Yes | Client ID of your developer application. This can be found on your application auth settings page in the Developer Portal. |\n| `client_secret` | str | Yes | Client secret of your developer application. This can be found on your application auth settings page in the Developer Portal. |\n| `redirect_url` | str | No | If your integration will be using the authorization code flow to obtain 3-legged access tokens, this should be provided. This redirect URL must match one of the redirect URLs configured in the app auth settings page in the Developer Portal. |\n\n#### Properties\n\n| Property | Description |\n|---|---|\n| `session` | The session object used for making http requests. This is exposed to allow for additional configuration (e.g. adding custom request/response event hooks). |\n\n#### Methods\n\n##### `generate_member_auth_url (scopes, state=None)`\n\nGenerates the member authorization URL to direct members to. Once redirected, the member will be presented with LinkedIn\'s OAuth consent page showing the OAuth scopes your application is requesting on behalf of the user.\n\n**Parameters:**\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `scopes` | List[str] | Yes | An array of OAuth scopes (3-legged member permissions) your application is requesting on behalf of the user. |\n| `state` | str | No | An optional string that can be provided to test against CSRF attacks. |\n\n**Return value:**\n\nThe member authorization URL string\n\n##### `exchange_auth_code_for_access_token (code)`\n\nExchanges an authorization code for a 3-legged access token. After member authorization, the browser redirects to the provided redirect URL, setting the authorization code on the `code` query parameter.\n\n**Parameters:**\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `code` | str | Yes | The authorization code to exchange for an access token |\n\n**Return value:**\n\nReturns an [AccessToken3LResponse](#class-accesstoken3lresponse) object\n\n##### `exchange_refresh_token_for_access_token (refresh_token)`\n\nExchanges a refresh token for a new 3-legged access token. This allows access tokens to be refreshed without having the member reauthorize your application.\n\n**Parameters:**\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `refresh_token` | str | Yes | The authorization code to exchange for an access token |\n\n**Return value:**\n\nReturns a [RefreshTokenExchangeResponse](#class-refreshtokenexchangeresponse) object\n\n##### `get_two_legged_access_token ()`\n\nUse client credential flow (2-legged OAuth) to retrieve a 2-legged access token for accessing APIs that are not member-specific. Developer applications do not have the client credential flow enabled by default.\n\n**Parameters:**\n\nNone\n\n**Return value:**\n\nReturns an [AccessToken2LResponse](#class-accesstoken2lresponse) object\n\n##### `introspect_access_token (access_token)`\n\nIntrospect a 2-legged, 3-legged or Enterprise access token to get information on status, expiry, and other details.\n\n**Parameters:**\n\n| Parameter | Type | Required? | Description |\n|---|---|---|---|\n| `access_token` | str | Yes | A 2-legged, 3-legged or Enterprise access token. |\n\n**Return value:**\n\nReturns an [IntrospectTokenResponse](#class-introspecttokenresponse) object\n\n\n#### Response Classes\n\n##### `class BaseAuthResponse`\n\nAll request methods of the AuthClient return a response object subclassed from BaseAuthResponse, containing standard response data, along with the original, raw response object.\n\n| Properties | Type | Description |\n|---|---|---|\n| `status_code` | int | Response status code |\n| `url` | str | The final URL location of the response |\n| `headers` | CaseInsensitiveDict | A case-insensitive dictionary of response headers |\n| `response` | Response | The raw requests.Response object |\n\n##### `class AccessToken3LResponse`\n\nBase class: [BaseAuthResponse](#class-baseauthresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `access_token` | str | The 3-legged access token |\n| `expires_in` | int | The TTL of the access token, in seconds |\n| `refresh_token` | str | The refresh token value. This is only present if refresh tokens are enabled for the application. |\n| `refresh_token_expires_in` | Number | The TTL of the refresh token, in seconds. This is only present if refresh tokens are enabled for the application. |\n| `scope` | str | A comma-separated list of scopes authorized by the member (e.g. "r_liteprofile,r_ads") |\n\n##### `class AccessToken2LResponse`\n\nBase class: [BaseAuthResponse](#class-baseauthresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `access_token` | str | The 2-legged access token |\n| `expires_in` | int | The TTL of the access token, in seconds |\n\n##### `class RefreshTokenExchangeResponse`\n\nBase class: [BaseAuthResponse](#class-baseauthresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `access_token` | str | The 3-legged access token |\n| `expires_in` | int | The TTL of the access token, in seconds |\n| `refresh_token` | str | The refresh token value. This is only present if refresh tokens are enabled for the application. |\n| `refresh_token_expires_in` | Number | The TTL of the refresh token, in seconds. This is only present if refresh tokens are enabled for the application. |\n\n\n##### `class IntrospectTokenResponse`\n\nBase class: [BaseAuthResponse](#class-baseauthresponse)\n\n| Properties | Type | Description |\n|---|---|---|\n| `active` | str | Flag whether the token is a valid, active token. |\n| `auth_type` | str | The auth type of the token ("2L", "3L" or "Enterprise_User") |\n| `authorized_at` | str | Epoch time in seconds, indicating when the token was authorize |\n| `client_id` | str | Developer application client ID |\n| `created_at` | int | Epoch time in seconds, indicating when this token was originally issued |\n| `expires_at` | int | Epoch time in seconds, indicating when this token will expire |\n| `scope` | str | A string containing a comma-separated list of scopes associated with this token. This is only returned for 3-legged member tokens. |\n| `status` | str | The token status, which is an enum string with values "revoked", "expired" or "active" |\n\n---\n\n## List of dependencies\n\nThe following table is a list of production dependencies.\n\n| Component Name | License | Linked | Modified |\n|---|---|---|---|\n| [requests](https://pypi.org/project/requests/) | Apache 2.0 | Static | No |\n',
-    'author': 'Steven Shimizu',
-    'author_email': 'sshimizu@linkedin.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/linkedin-developers/linkedin-api-python-client',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+# LinkedIn API Python Client
 
+## Overview
+
+This library provides a thin Python client for making requests to LinkedIn APIs, utilizing the Python [requests](https://pypi.org/project/requests/) HTTP client library. LinkedIn's APIs are built on the [Rest.li](https://linkedin.github.io/rest.li/) framework with additional LinkedIn-specific constraints, which results in a robust yet complex protocol that can be challenging to implement correctly.
+
+This library helps reduce this complexity by formatting requests correctly, providing proper request headers, and providing interfaces to develop against for responses. The library also provides an auth client for inspecting, generating, and refreshing access tokens, along with other helpful utilities.
+
+> :warning: This API client library is currently in beta and is subject to change. It may contain bugs, errors, or other issues that we are working to resolve. Use of this library is at your own risk. Please use caution when using it in production environments and be prepared for the possibility of unexpected behavior. We welcome any feedback or reports of issues that you may encounter while using this library.
+
+### Features
+
+- Generic support for all Rest.li methods used in LinkedIn APIs
+- Supports Rest.li protocol version 2.0.0
+- Provide interfaces for request options/response payloads
+- Built-in parameter encoding
+- Utilities (e.g. URN handling, encoding)
+- Supports versioned APIs
+- Automatic query tunneling of requests
+- 2-legged and 3-legged OAuth2 support
+
+### Table of Contents
+
+- [Requirements](#requirements)
+- [Installation](#installation)
+- [Getting Started](#getting-started)
+  - [Pre-requisites](#pre-requisites)
+  - [Simple API Request Example](#simple-api-request-example)
+  - [Finder Request Example](#finder-request-example)
+  - [More Examples](#more-examples)
+- [API Reference](#api-reference)
+  - [RestliClient](#class-restliclient)
+    - [Constructor](#constructor)
+    - [Properties](#properties)
+    - [Methods](#methods)
+      - [`get()`](#get-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_get()`](#batch_get-resource_path-ids-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`get_all()`](#get_all-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`finder()`](#finder-resource_path-finder_name-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_finder()`](#batch_finder-resource_path-finder_name-finder_criteria-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`create()`](#create-resource_path-entity-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_create()`](#batch_create-resource_path-entities-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`update()`](#update-resource_path-entity-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_update()`](#batch_update-resource_path-ids-entities-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`partial_update()`](#partial_update-resource_path-patch_set_object-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_partial_update()`](#batch_partial_update-resource_path-ids-patch_set_objects-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`delete()`](#delete-resource_path-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`batch_delete()`](#batch_delete-resource_path-ids-access_token-path_keysnone-query_paramsnone-version_stringnone)
+      - [`action()`](#action-resource_path-action_name-access_token-action_paramsnone-path_keysnone-query_paramsnone-version_stringnone)
+  - [AuthClient](#class-authclient)
+    - [Constructor](#constructor-1)
+    - [Properties](#properties-1)
+    - [Methods](#methods-1)
+      - [`generate_member_auth_url()`](#generate_member_auth_url-scopes-statenone)
+      - [`exchange_auth_code_for_access_token()`](#exchange_auth_code_for_access_token-code)
+      - [`exchange_refresh_token_for_access_token()`](#exchange_refresh_token_for_access_token-refresh_token)
+      - [`get_two_legged_access_token()`](#get_two_legged_access_token-)
+      - [`introspect_access_token()`](#introspect_access_token-access_token)
+- [List of dependencies](#list-of-dependencies)
+
+
+## Requirements
+
+- Python >= 3.7
+
+
+## Installation
+
+```sh
+pip install linkedin-api-client
+```
+
+## Getting Started
+
+### Pre-requisites
+
+1. Create or use an existing developer application from the [LinkedIn Developer Portal](https://www.linkedin.com/developers/apps/)
+2. Request access to the Sign In With LinkedIn API product. This is a self-serve product that will be provisioned immediately to your application.
+3. Generate a 3-legged access token using the Developer Portal [token generator tool](https://www.linkedin.com/developers/tools/oauth/token-generator), selecting the r_liteprofile scope.
+
+### Simple API Request Example
+
+Here is an example of using the client to make a simple GET request to [fetch the current user's profile](https://learn.microsoft.com/en-us/linkedin/consumer/integrations/self-serve/sign-in-with-linkedin#retrieving-member-profiles). This requires a 3-legged access token with the "r_liteprofile" scope, which is included with the Sign In With LinkedIn API product.
+
+```python
+from linkedin_api.clients.restli.client import RestliClient
+
+restli_client = RestliClient()
+
+response = restli_client.get(
+  resource_path="/me",
+  access_token=<THREE_LEGGED_ACCESS_TOKEN>
+)
+print(response.entity)
+```
+
+### Finder Request Example
+
+Here is a more non-trivial example to [find ad accounts](https://learn.microsoft.com/en-us/linkedin/marketing/integrations/ads/account-structure/create-and-manage-accounts?#search-for-accounts) by some search criteria. This requires a 3-legged access token with the "r_ads" scope, which is included with the Advertising APIs product.
+
+The "search" query parameter in this case is not a primitive, but a complex object, which we represent as a dictionary. The client will handle the correct URL-encoding. This is a versioned API call, so we also need to provide the version string in the "YYYYMM" format.
+
+```python
+from linkedin_api.clients.restli.client import RestliClient
+
+restli_client = RestliClient()
+
+response = restli_client.finder(
+  resource_path="/adAccounts",
+  finder_name="search",
+  query_params={
+    "search": {
+      "status": {
+        "values": ["ACTIVE", "DRAFT"]
+      },
+      "reference": {
+        "values": ["urn:li:organization:123"]
+      },
+      "test": True
+    }
+  },
+  version_string="202212",
+  acccess_token=<THREE_LEGGED_ACCESS_TOKEN>
+)
+ad_accounts = response.elements
+```
+
+### More Examples
+
+There are more examples of using the client in [/examples](examples/) directory.
+
+
+## API Reference
+
+### `class RestliClient`
+
+The Rest.li API client defines instance methods for all the Rest.li methods which are used by LinkedIn APIs. All calls are blocking.
+
+Rest.li defines a standard set of methods that can operate on a resource, each of which maps to an HTTP method. Depending on the resource, some Rest.li methods are not applicable or not implemented. Read the API docs to determine what Rest.li method is applicable and the relevant request parameters.
+
+#### Constructor
+
+An instance of the API client must be created before using. This creates a session object that will be used for making all subsequent requests.
+
+```python
+from linkedin_api.clients.restli.client import RestliClient
+
+restli_client = RestliClient()
+```
+
+The Requests library [session](https://requests.readthedocs.io/en/latest/user/advanced/#session-objects) object is accessible to configure any additional global settings (e.g. configuring event hooks).
+
+```python
+restli_client.session.hooks = { 'response': [do_something_fn, do_something_2_fn] }
+```
+
+#### Properties
+
+| Property | Description |
+|---|---|
+| `session` | The session object used for making http requests. This is exposed to allow for additional configuration (e.g. adding custom request/response event hooks). |
+
+#### Methods
+
+##### Base Request Parameters
+
+All Rest.li request methods of the API client support the following request parameters:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `resource_path` | str | Yes | <p>The resource path after the base URL, beginning with a forward slash. If the path contains keys, add curly-brace placeholders for the keys and specify the path key-value map in the `path_keys` argument.</p><p>Examples:</p><ul><li>`resource_path="/me"`</li><li>`resource_path="/adAccounts/{id}"`</li><li>`resource_path="/socialActions/{actionUrn}/comments/{commentId}"`</li><li>`resource_path="/campaignConversions/{key}`</li></ul>|
+| `access_token` | str | Yes | The access token that should provide the application access to the specified API |
+| `path_keys` | Dict[str,Any] | No | <p>If there are path keys that are part of the `resource_path` argument, the key placeholders must be specified in the provided `path_keys` map. The path key values can be strings, numbers, or objects (dictionaries), and these will be properly encoded.</p><p>Examples:</p><p><ul><li>`path_keys={"id": 123"}`</li><li>`path_keys={"actionUrn":"urn:li:share:123","commentId":987`}</li><li>`path_keys={"key": {"campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456"}}`</li></ul></p> |
+| `query_params` | Dict[str,Any] | No | A map of query parameters. The query parameter values (strings, lists, objects) will be correctly encoded by this method, so these should not be encoded. |
+| `version_string` | str | No | An optional version string of the format "YYYYMM" or "YYYYMM.RR". If specified, the version header will be passed and the request will use the versioned APIs base URL |
+
+##### `get (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li GET request to fetch the specified entity on a resource. This method will perform query tunneling if necessary.
+
+**Parameters:**
+
+This method only uses the [base request parameters](#base-request-parameters) defined above.
+
+**Return value:**
+
+Returns [GetResponse](#class-getresponse) object
+
+**Example:**
+
+```python
+response = restli_client.get(
+  resource_path="/adAccounts/{id}"
+  path_keys={ "id": 123 },
+  query_params={ "fields": "id,name" }
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+ad_account = response.entity
+```
+
+
+##### `batch_get (resource_path, ids, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_GET request to fetch multiple entities on a resource. This method will perform query tunneling if necessary.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to fetch on the resource. These will be encoded and added to the query parameters. |
+
+**Return value:**
+
+Returns a [BatchGetResponse](#class-batchgetresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.batch_get(
+  resource_path="/adCampaignGroups",
+  ids=[123, 456, 789],
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+campaign_groups = response.results.items()
+```
+
+
+##### `get_all (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li GET_ALL request to fetch all entities on a resource.
+
+**Parameters:**
+
+This method only uses the [base request parameters](#base-request-parameters) defined above.
+
+**Return value:**
+
+Returns [CollectionResponse](#class-collectionresponse) object
+
+**Example:**
+
+```python
+response = restli_client.get_all(
+  resource_path="/fieldsOfStudy",
+  query_params={
+    "start": 0,
+    "count": 15
+  },
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+fields_of_study = response.elements
+total = response.paging.total
+```
+
+##### `finder (resource_path, finder_name, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li FINDER request to find entities by some specified criteria.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `finder_name` | str | Yes | The Rest.li finder name. This will be added to the request query parameters. |
+
+**Return value:**
+
+Returns a [CollectionResponse](#class-collectionresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.finder(
+  resource_path="/adAccounts",
+  finder_name="search",
+  query_params={
+    "search": {
+        "status": {
+            "values": ["ACTIVE", "DRAFT", "CANCELED"]
+        },
+        "reference": {
+            "values": ["urn:li:organization:123"]
+        },
+        "test": False
+    },
+    "start": 0,
+    "count": 5
+  },
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+ad_accounts = response.elements
+total = response.paging.total
+```
+
+##### `batch_finder (resource_path, finder_name, finder_criteria, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_FINDER request to find entities by multiple sets of criteria.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `finder_name` | str | Yes | The Rest.li batch finder name (the value of the "bq" query parameter). This will be added to the request query parameters. |
+| `finder_criteria` | Tuple[str, List[Dict[str,Any]]] | Yes | The required batch finder criteria information. This is a tuple with the first value being the batch finder criteria parameter name. The second value is the list of finder param objects. The batch finder results are correspondingly ordered according to this list. The batch finder criteria will be encoded and added to the request query parameters. |
+
+**Return value:**
+
+Returns a [BatchFinderResponse](#class-batchfinderresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.batch_finder(
+  resource_path="/organizationAuthorizations",
+  finder_name="authorizationActionsAndImpersonator",
+  finder_criteria=("authorizationActions", [
+      {
+        "OrganizationRoleAuthorizationAction": {
+          actionType: "ADMINISTRATOR_READ"
+        }
+      },
+      {
+        "OrganizationContentAuthorizationAction": {
+          actionType: "ORGANIC_SHARE_DELETE"
+        }
+      }
+    ]
+  ),
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+admin_read_authorizations = response.results[0].elements
+organic_share_delete_authorizations = response.results[1].elements
+```
+
+##### `create (resource_path, entity, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li CREATE request to create a new resource entity.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `entity` | Dict[str,Any] | Yes | A dictionary representation of the entity to create |
+
+**Return value:**
+
+Returns a [CreateResponse](#class-createresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.create(
+  resource_path="/adAccountsV2",
+  entity={
+    "name": "Test Ad Account",
+    "type": "BUSINESS",
+    "test": True
+  },
+  access_token=MY_ACCESS_TOKEN
+)
+created_entity_id = response.entity_id
+```
+
+##### `batch_create (resource_path, entities, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_CREATE request to create multiple entities in a single call.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `entities` | List[Dict[str,Any]] | Yes | A list of entities to create |
+
+**Return value:**
+
+Returns a [BatchCreateResponse](#class-batchcreateresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.batch_create(
+  resource_path="/adCampaignGroups",
+  entities=[
+    {
+        account: 'urn:li:sponsoredAccount:111',
+        name: 'CampaignGroupTest1',
+        status: 'DRAFT'
+    },
+    {
+        account: 'urn:li:sponsoredAccount:222',
+        name: 'CampaignGroupTest2',
+        status: 'DRAFT'
+    }
+  ],
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+created_elements = response.elements
+first_created_element_id = response.elements[0].id
+```
+
+##### `update (resource_path, entity, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li UPDATE request to update an entity (overwriting the entity with the provided value).
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `entity` | Dict[str,Any] | Yes | The value of the updated entity. This will completely overwrite the entity. |
+
+**Return value:**
+
+Returns a [UpdateResponse](#class-updateresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.update(
+  resource_path="/adAccountUsers/{id}",
+  path_keys={
+    "id": {
+      "account": "urn:li:sponsoredAccount:123",
+      "user": "urn:li:person:foobar"
+    }
+  },
+  entity: {
+    "account": "urn:li:sponsoredAccount:123",
+    "user": "urn:li:person:foobar",
+    "role": "VIEWER"
+  },
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+status = response.status_code
+```
+
+##### `batch_update (resource_path, ids, entities, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_UPDATE request to update multiple entities in a single call.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The ids of the entities to update |
+| `entities` | List[Dict[str,Any]] | Yes | The values to update the specified entities to. This should be the same order as the `ids` argument. |
+
+**Return value:**
+
+Returns a [BatchUpdateResponse](#class-batchupdateresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.batch_update(
+  resource_path="/campaignConversions",
+  ids=[
+    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456" },
+    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:789" }
+  ],
+  entities=[
+    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:456" },
+    { "campaign": "urn:li:sponsoredCampaign:123", "conversion": "urn:lla:llaPartnerConversion:789" }
+  ],
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+batch_results = response.results.items()
+```
+
+##### `partial_update (resource_path, patch_set_object, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li PARTIAL_UPDATE request to update part of an entity. Directly specify the patch object to send in the request.
+
+Note: While the Rest.li protocol supports very granular patch objects with setting and deletion of nested properties, most LinkedIn APIs only support partial update on the top-level fields of an entity.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `patch_set_object` | Dict[str,Any] | Yes | The value of the entity with only the modified fields present. This will be sent directly in the request body as `patch: { $set: patch_set_object }`. |
+
+**Return value:**
+
+Returns a [UpdateResponse](#class-updateresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.partial_update(
+  resource_path="/adAccounts/{id}",
+  path_keys={ "id": 123 },
+  patch_set_object: {
+    "name": "TestAdAccountModified",
+    "reference": "urn:li:organization:456"
+  },
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+status = response.status_code
+```
+
+##### `batch_partial_update (resource_path, ids, patch_set_objects, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_PARTIAL_UPDATE request to update multiple entities at once, by only providing the fields of the entities that require updating.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to update. These will be encoded and added to the query parameters. |
+| `patch_set_objects` | List[Dict[str,Any]] | Yes | The list of entity values, represented as a dictionary, with only the modified fields present. |
+
+**Return value:**
+
+Returns a [BatchUpdateResponse](#class-batchupdateresponse) object.
+
+**Example:**
+
+```python
+response = restli_client.batch_partial_update(
+  resource_path="/adCampaignGroups",
+  ids=["123", "456"],
+  patch_set_objects: [
+    { "status": "ACTIVE" },
+    {
+      "runSchedule": {
+        "start": 1678029270721,
+        "end": 1679029270721
+      }
+    }
+  ],
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+result_status = response.results["123"].status
+```
+
+##### `delete (resource_path, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li DELETE request to delete an entity.
+
+**Parameters:**
+
+This method only uses the [base request parameters](#base-request-parameters) defined above.
+
+**Return value:**
+
+Returns [BaseRestliResponse](#class-baserestliresponse) object
+
+**Example:**
+
+```python
+response = restli_client.delete(
+  resource_path="/adAccounts/{id}",
+  path_keys={ "id": 123 },
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+status_code = response.status_code
+```
+
+##### `batch_delete (resource_path, ids, access_token, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li BATCH_DELETE request to delete multiple entities at once.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `ids` | List[Union[str,int,Dict[str,Any]]] | Yes | The list of entity ids to delete. These will be encoded and added to the query parameters. |
+
+**Return value:**
+
+Returns [BatchDeleteResponse](#class-batchdeleteresponse) object
+
+**Example:**
+
+```python
+response = restli_client.batch_delete(
+  resource_path="/adAccounts",
+  ids=["123", "456"],
+  access_token=MY_ACCESS_TOKEN,
+  version_string="202212"
+)
+status_code = response.results["123"].status
+```
+
+##### `action (resource_path, action_name, access_token, action_params=None, path_keys=None, query_params=None, version_string=None)`
+
+Makes a Rest.li ACTION request to perform an action on a specified resource. This method is flexible and generally used when the action does not fit within the standard behavior defined by the other Rest.li methods.
+
+**Parameters:**
+
+The additional parameters besides the [base request parameters](#base-request-parameters) are:
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `action_name` | str | Yes | The action method name. This will be added to the query parameters. |
+| `action_params` | Dict[str,Any] | No | An optional map of action parameters and their values. This will be sent in the request body. |
+
+**Return value:**
+
+Returns [ActionResponse](#class-actionresponse) object
+
+**Example:**
+
+```python
+response = restli_client.action(
+  resource_path="/liveAssetActions",
+  action_name="register",
+  action_params={
+    "registerLiveEventRequest": {
+      "owner": "urn:li:person:12345",
+      "recipes": ["urn:li:digitalmediaRecipe:feedshare-live-video"],
+      "region": "WEST_US"
+    }
+  },
+  access_token=MY_ACCESS_TOKEN
+)
+status_code = response.status_code
+```
+
+#### Response Classes
+
+##### `class BaseRestliResponse`
+
+All Rest.li request methods of the API client return a response object subclassed from BaseRestliResponse, containing standard response data, along with the original, raw response object.
+
+| Properties | Type | Description |
+|---|---|---|
+| `status_code` | int | Response status code |
+| `url` | str | The final URL location of the response |
+| `headers` | CaseInsensitiveDict | A case-insensitive dictionary of response headers |
+| `response` | Response | The raw requests.Response object |
+
+##### `class Paging`
+
+Paging metadata class
+
+| Properties | Type | Description |
+|---|---|---|
+| start | int | The start index of returned results (zero-based index) |
+| count | int | The number of results returned in the response |
+| total | int | The total number of results available |
+
+##### `class GetResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `entity` | Union[Dict[str,Any], str, int, bool] | The representation (typically a dictionary) of the retrieved entity, decoded from the json-encoded response content |
+
+##### `class BatchGetResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `results` | Dict[str,Any] | A map of entities that were successfully retrieved, with the key being the encoded entity id, and the value being a dictionary representing the entity |
+| `statuses` | Dict[str,int] | A map of entities and status code, with the key being the encoded entity id, and the value being the status code number value. |
+| `errors` | Dict[str,Any] | A map containing entities that could not be successfully fetched, with the key being the encoded entity id, and the value being the error response. |
+
+##### `class CollectionResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `elements` | List[Dict[str,Any]] | The list of entities returned in the response |
+| `paging` | [Paging](#class-paging) | Optional paging metadata object |
+| `metadata` | Any | Optional response metadata object |
+
+##### `class BatchFinderResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `results` | List[[BatchFinderResult](#class-batchfinderresult)] | The list of finder results, in the same order as the requested batch finder search criteria list |
+
+##### `class BatchFinderResult`
+
+| Properties | Type | Description |
+|---|---|---|
+| `elements` | List[Dict[str,Any]] | The list of entities found for the corresponding finder criteria |
+| `paging` | [Paging](#class-paging) | Optional paging metadata object |
+| `metadata` | Any | Optional response metadata object |
+| `error` | Any | Optional error details if finder call failed |
+| `isError` | bool | Flag if this finder call experienced an error |
+
+##### `class CreateResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `entity_id` | str | The reduced-encoded entity id. |
+| `decoded_entity_id` | Union[str, Dict[str,Any]] | The decoded entity id. |
+| `entity` | Dict[str,Any] | Optional created entity. Some APIs support returning the created entity to eliminate the need for a subsequent GET call. |
+
+##### `class BatchCreateResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `elements` | List[[BatchCreateResult](#class-batchcreateresult)] | The list of batch create results, corresponding to the order of the `entities` request parameter |
+
+##### `class BatchCreateResult`
+
+| Properties | Type | Description |
+|---|---|---|
+| `status` | int | The status code of the individual create call |
+| `id` | str | The id of the created entity |
+| `error` | Any | Error details if the create call experienced an error |
+
+##### `class UpdateResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `entity` | Dict[str,Any] | Optional entity after the update. Some APIs support returning the updated entity to eliminate the need for a subsequent GET call. |
+
+##### `class BatchUpdateResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `results` | Dict[str,[BatchUpdateResult](#class-batchupdateresult)] | The results map where the keys are the encoded entity ids, and the values are the individual update call results, which includes the status code. |
+
+##### `class BatchUpdateResult`
+
+| Properties | Type | Description |
+|---|---|---|
+| `status` | int | The status code of the individual update call |
+
+##### `class BatchDeleteResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `results` | Dict[str,[BatchDeleteResult](#class-batchdeleteresult)] | The results map where the keys are the encoded entity ids, and the values are the individual delete call results, which includes the status code. |
+
+##### `class BatchDeleteResult`
+
+| Properties | Type | Description |
+|---|---|---|
+| `status` | int | The status code of the delete call |
+
+##### `class ActionResponse`
+
+Base class: [BaseRestliResponse](#class-baserestliresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `value` | Any | The action response value |
+
+
+### `class AuthClient`
+
+While we recommend using any of several popular, open-source libraries for robustly managing OAuth 2.0 authentication, we provide a basic Auth Client as a convenience for testing APIs and getting started.
+
+#### Constructor
+
+```python
+from linkedin_api.clients.auth.client import AuthClient
+
+auth_client = AuthClient(client_id=MY_CLIENT_ID, client_secret=MY_CLIENT_SECRET, redirect_url=MY_REDIRECT_URL)
+```
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `client_id` | str | Yes | Client ID of your developer application. This can be found on your application auth settings page in the Developer Portal. |
+| `client_secret` | str | Yes | Client secret of your developer application. This can be found on your application auth settings page in the Developer Portal. |
+| `redirect_url` | str | No | If your integration will be using the authorization code flow to obtain 3-legged access tokens, this should be provided. This redirect URL must match one of the redirect URLs configured in the app auth settings page in the Developer Portal. |
+
+#### Properties
+
+| Property | Description |
+|---|---|
+| `session` | The session object used for making http requests. This is exposed to allow for additional configuration (e.g. adding custom request/response event hooks). |
+
+#### Methods
+
+##### `generate_member_auth_url (scopes, state=None)`
+
+Generates the member authorization URL to direct members to. Once redirected, the member will be presented with LinkedIn's OAuth consent page showing the OAuth scopes your application is requesting on behalf of the user.
+
+**Parameters:**
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `scopes` | List[str] | Yes | An array of OAuth scopes (3-legged member permissions) your application is requesting on behalf of the user. |
+| `state` | str | No | An optional string that can be provided to test against CSRF attacks. |
+
+**Return value:**
+
+The member authorization URL string
+
+##### `exchange_auth_code_for_access_token (code)`
+
+Exchanges an authorization code for a 3-legged access token. After member authorization, the browser redirects to the provided redirect URL, setting the authorization code on the `code` query parameter.
+
+**Parameters:**
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `code` | str | Yes | The authorization code to exchange for an access token |
+
+**Return value:**
+
+Returns an [AccessToken3LResponse](#class-accesstoken3lresponse) object
+
+##### `exchange_refresh_token_for_access_token (refresh_token)`
+
+Exchanges a refresh token for a new 3-legged access token. This allows access tokens to be refreshed without having the member reauthorize your application.
+
+**Parameters:**
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `refresh_token` | str | Yes | The authorization code to exchange for an access token |
+
+**Return value:**
+
+Returns a [RefreshTokenExchangeResponse](#class-refreshtokenexchangeresponse) object
+
+##### `get_two_legged_access_token ()`
+
+Use client credential flow (2-legged OAuth) to retrieve a 2-legged access token for accessing APIs that are not member-specific. Developer applications do not have the client credential flow enabled by default.
+
+**Parameters:**
+
+None
+
+**Return value:**
+
+Returns an [AccessToken2LResponse](#class-accesstoken2lresponse) object
+
+##### `introspect_access_token (access_token)`
+
+Introspect a 2-legged, 3-legged or Enterprise access token to get information on status, expiry, and other details.
+
+**Parameters:**
+
+| Parameter | Type | Required? | Description |
+|---|---|---|---|
+| `access_token` | str | Yes | A 2-legged, 3-legged or Enterprise access token. |
+
+**Return value:**
+
+Returns an [IntrospectTokenResponse](#class-introspecttokenresponse) object
+
+
+#### Response Classes
+
+##### `class BaseAuthResponse`
+
+All request methods of the AuthClient return a response object subclassed from BaseAuthResponse, containing standard response data, along with the original, raw response object.
+
+| Properties | Type | Description |
+|---|---|---|
+| `status_code` | int | Response status code |
+| `url` | str | The final URL location of the response |
+| `headers` | CaseInsensitiveDict | A case-insensitive dictionary of response headers |
+| `response` | Response | The raw requests.Response object |
+
+##### `class AccessToken3LResponse`
+
+Base class: [BaseAuthResponse](#class-baseauthresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `access_token` | str | The 3-legged access token |
+| `expires_in` | int | The TTL of the access token, in seconds |
+| `refresh_token` | str | The refresh token value. This is only present if refresh tokens are enabled for the application. |
+| `refresh_token_expires_in` | Number | The TTL of the refresh token, in seconds. This is only present if refresh tokens are enabled for the application. |
+| `scope` | str | A comma-separated list of scopes authorized by the member (e.g. "r_liteprofile,r_ads") |
+
+##### `class AccessToken2LResponse`
+
+Base class: [BaseAuthResponse](#class-baseauthresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `access_token` | str | The 2-legged access token |
+| `expires_in` | int | The TTL of the access token, in seconds |
+
+##### `class RefreshTokenExchangeResponse`
+
+Base class: [BaseAuthResponse](#class-baseauthresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `access_token` | str | The 3-legged access token |
+| `expires_in` | int | The TTL of the access token, in seconds |
+| `refresh_token` | str | The refresh token value. This is only present if refresh tokens are enabled for the application. |
+| `refresh_token_expires_in` | Number | The TTL of the refresh token, in seconds. This is only present if refresh tokens are enabled for the application. |
+
+
+##### `class IntrospectTokenResponse`
+
+Base class: [BaseAuthResponse](#class-baseauthresponse)
+
+| Properties | Type | Description |
+|---|---|---|
+| `active` | str | Flag whether the token is a valid, active token. |
+| `auth_type` | str | The auth type of the token ("2L", "3L" or "Enterprise_User") |
+| `authorized_at` | str | Epoch time in seconds, indicating when the token was authorize |
+| `client_id` | str | Developer application client ID |
+| `created_at` | int | Epoch time in seconds, indicating when this token was originally issued |
+| `expires_at` | int | Epoch time in seconds, indicating when this token will expire |
+| `scope` | str | A string containing a comma-separated list of scopes associated with this token. This is only returned for 3-legged member tokens. |
+| `status` | str | The token status, which is an enum string with values "revoked", "expired" or "active" |
+
+---
+
+## List of dependencies
+
+The following table is a list of production dependencies.
+
+| Component Name | License | Linked | Modified |
+|---|---|---|---|
+| [requests](https://pypi.org/project/requests/) | Apache 2.0 | Static | No |
 
-setup(**setup_kwargs)
```

