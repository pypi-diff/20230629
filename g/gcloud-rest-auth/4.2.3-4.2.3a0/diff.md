# Comparing `tmp/gcloud_rest_auth-4.2.3.tar.gz` & `tmp/gcloud_rest_auth-4.2.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_rest_auth-4.2.3.tar", max compression
+gzip compressed data, was "gcloud_rest_auth-4.2.3a0.tar", max compression
```

## Comparing `gcloud_rest_auth-4.2.3.tar` & `gcloud_rest_auth-4.2.3a0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/LICENSE
--rw-r--r--   0        0        0     2998 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/README.rst
--rw-r--r--   0        0        0      212 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/gcloud/py.typed
--rw-r--r--   0        0        0      216 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/__init__.py
--rw-r--r--   0        0        0     2048 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/__init__.py
--rw-r--r--   0        0        0      184 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/build_constants.py
--rw-r--r--   0        0        0     5254 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/iam.py
--rw-r--r--   0        0        0        0 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/py.typed
--rw-r--r--   0        0        0    11655 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/session.py
--rw-r--r--   0        0        0     9748 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/token.py
--rw-r--r--   0        0        0      735 2023-06-29 16:17:55.000000 gcloud_rest_auth-4.2.3/gcloud/rest/auth/utils.py
--rw-r--r--   0        0        0        0 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/gcloud/rest/py.typed
--rw-r--r--   0        0        0     1110 2023-06-29 16:17:54.000000 gcloud_rest_auth-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     4128 1970-01-01 00:00:00.000000 gcloud_rest_auth-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/LICENSE
+-rw-r--r--   0        0        0     2998 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/README.rst
+-rw-r--r--   0        0        0      212 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/gcloud/py.typed
+-rw-r--r--   0        0        0      216 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/__init__.py
+-rw-r--r--   0        0        0     2048 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/__init__.py
+-rw-r--r--   0        0        0      184 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/build_constants.py
+-rw-r--r--   0        0        0     5254 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/iam.py
+-rw-r--r--   0        0        0        0 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/py.typed
+-rw-r--r--   0        0        0    11655 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/session.py
+-rw-r--r--   0        0        0     9748 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/token.py
+-rw-r--r--   0        0        0      735 2023-06-28 12:59:38.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/gcloud/rest/py.typed
+-rw-r--r--   0        0        0     1112 2023-06-28 12:59:37.000000 gcloud_rest_auth-4.2.3a0/pyproject.toml
+-rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 gcloud_rest_auth-4.2.3a0/PKG-INFO
```

### Comparing `gcloud_rest_auth-4.2.3/LICENSE` & `gcloud_rest_auth-4.2.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/README.rst` & `gcloud_rest_auth-4.2.3a0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/gcloud/rest/auth/__init__.py` & `gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/gcloud/rest/auth/iam.py` & `gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/iam.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/gcloud/rest/auth/session.py` & `gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/session.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/gcloud/rest/auth/token.py` & `gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/token.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/gcloud/rest/auth/utils.py` & `gcloud_rest_auth-4.2.3a0/gcloud/rest/auth/utils.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-4.2.3/pyproject.toml` & `gcloud_rest_auth-4.2.3a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-rest-auth"
-version = "4.2.3"
+version = "4.2.3a0"
 description = "Python Client for Google Cloud Auth"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
```

### Comparing `gcloud_rest_auth-4.2.3/PKG-INFO` & `gcloud_rest_auth-4.2.3a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-rest-auth
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

