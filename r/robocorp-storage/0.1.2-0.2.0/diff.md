# Comparing `tmp/robocorp_storage-0.1.2.tar.gz` & `tmp/robocorp_storage-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_storage-0.1.2.tar", max compression
+gzip compressed data, was "robocorp_storage-0.2.0.tar", max compression
```

## Comparing `robocorp_storage-0.1.2.tar` & `robocorp_storage-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      388 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/README.md
--rw-r--r--   0        0        0      801 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5321 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/src/robocorp/storage/__init__.py
--rw-r--r--   0        0        0     6642 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/src/robocorp/storage/_requests.py
--rw-r--r--   0        0        0     1759 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/src/robocorp/storage/_storage.py
--rw-r--r--   0        0        0     1203 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/src/robocorp/storage/_utils.py
--rw-r--r--   0        0        0        0 2023-06-22 02:43:13.828523 robocorp_storage-0.1.2/src/robocorp/storage/py.typed
--rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 robocorp_storage-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      388 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/README.md
+-rw-r--r--   0        0        0      801 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5321 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/__init__.py
+-rw-r--r--   0        0        0     6642 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/_requests.py
+-rw-r--r--   0        0        0     3739 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/_storage.py
+-rw-r--r--   0        0        0        0 2023-06-29 11:54:20.167071 robocorp_storage-0.2.0/src/robocorp/storage/py.typed
+-rw-r--r--   0        0        0     1255 1970-01-01 00:00:00.000000 robocorp_storage-0.2.0/PKG-INFO
```

### Comparing `robocorp_storage-0.1.2/pyproject.toml` & `robocorp_storage-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-storage"
-version = "0.1.2"
+version = "0.2.0"
 description = "Robocorp Asset Storage library"
 authors = [
 	"Cosmin P. <cosmin@robocorp.com>",
 	"Ossi R. <ossi@robocorp.com>",
 ]
 readme = "README.md"
 repository = "https://github.com/robocorp/robo/"
```

### Comparing `robocorp_storage-0.1.2/src/robocorp/storage/__init__.py` & `robocorp_storage-0.2.0/src/robocorp/storage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import requests
 
 from ._requests import RequestsHTTPError
 from ._storage import Asset, AssetMeta, AssetNotFound, AssetUploadFailed
 from ._storage import get_assets_client as _get_assets_client
 
-__version__ = "0.1.2"
+__version__ = "0.2.0"
 version_info = [int(x) for x in __version__.split(".")]
 
 LOGGER = logging.getLogger(__name__)
 
 
 def _handle_missing_asset(response: requests.Response, *, name: str, asset_id: str):
     assets_client = _get_assets_client()
```

### Comparing `robocorp_storage-0.1.2/src/robocorp/storage/_requests.py` & `robocorp_storage-0.2.0/src/robocorp/storage/_requests.py`

 * *Files identical despite different names*

### Comparing `robocorp_storage-0.1.2/PKG-INFO` & `robocorp_storage-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-storage
-Version: 0.1.2
+Version: 0.2.0
 Summary: Robocorp Asset Storage library
 Home-page: https://github.com/robocorp/robo/
 License: Apache-2.0
 Author: Cosmin P.
 Author-email: cosmin@robocorp.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

