# Comparing `tmp/gcloud_aio_auth-4.2.3.tar.gz` & `tmp/gcloud_aio_auth-4.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_aio_auth-4.2.3.tar", max compression
+gzip compressed data, was "gcloud_aio_auth-4.2.3a0.tar", max compression
```

## Comparing `gcloud_aio_auth-4.2.3.tar` & `gcloud_aio_auth-4.2.3a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/LICENSE
--rw-r--r--   0        0        0     2988 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/README.rst
--rw-r--r--   0        0        0      212 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/__init__.py
--rw-r--r--   0        0        0      212 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/__init__.py
--rw-r--r--   0        0        0     2055 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/__init__.py
--rw-r--r--   0        0        0      184 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/build_constants.py
--rw-r--r--   0        0        0     5377 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/iam.py
--rw-r--r--   0        0        0        0 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/py.typed
--rw-r--r--   0        0        0    11871 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/session.py
--rw-r--r--   0        0        0     9919 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/token.py
--rw-r--r--   0        0        0      735 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/auth/utils.py
--rw-r--r--   0        0        0        0 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/aio/py.typed
--rw-r--r--   0        0        0        0 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/gcloud/py.typed
--rw-r--r--   0        0        0     1105 2023-06-29 18:47:56.939321 gcloud_aio_auth-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     4116 1970-01-01 00:00:00.000000 gcloud_aio_auth-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/LICENSE
+-rw-r--r--   0        0        0     2988 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/README.rst
+-rw-r--r--   0        0        0      212 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/__init__.py
+-rw-r--r--   0        0        0     2055 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/__init__.py
+-rw-r--r--   0        0        0      184 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/build_constants.py
+-rw-r--r--   0        0        0     5377 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/iam.py
+-rw-r--r--   0        0        0        0 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/py.typed
+-rw-r--r--   0        0        0    11871 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/session.py
+-rw-r--r--   0        0        0     9919 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/token.py
+-rw-r--r--   0        0        0      735 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/aio/py.typed
+-rw-r--r--   0        0        0        0 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/gcloud/py.typed
+-rw-r--r--   0        0        0     1107 2023-06-28 13:28:28.522250 gcloud_aio_auth-4.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 gcloud_aio_auth-4.2.3a0/PKG-INFO
```

### Comparing `gcloud_aio_auth-4.2.3/LICENSE` & `gcloud_aio_auth-4.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/README.rst` & `gcloud_aio_auth-4.2.3a0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/gcloud/aio/auth/__init__.py` & `gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/gcloud/aio/auth/iam.py` & `gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/iam.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/gcloud/aio/auth/session.py` & `gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/session.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/gcloud/aio/auth/token.py` & `gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/token.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/gcloud/aio/auth/utils.py` & `gcloud_aio_auth-4.2.3a0/gcloud/aio/auth/utils.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-4.2.3/pyproject.toml` & `gcloud_aio_auth-4.2.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-aio-auth"
-version = "4.2.3"
+version = "4.2.3a0"
 description = "Python Client for Google Cloud Auth"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
```

### Comparing `gcloud_aio_auth-4.2.3/PKG-INFO` & `gcloud_aio_auth-4.2.3a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-aio-auth
-Version: 4.2.3
+Version: 4.2.3a0
 Summary: Python Client for Google Cloud Auth
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

