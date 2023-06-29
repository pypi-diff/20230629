# Comparing `tmp/ayon-python-api-0.2.1.tar.gz` & `tmp/ayon-python-api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.2.1.tar", last modified: Tue Jun 13 09:28:06 2023, max compression
+gzip compressed data, was "ayon-python-api-0.2.2.tar", last modified: Thu Jun 29 09:01:00 2023, max compression
```

## Comparing `ayon-python-api-0.2.1.tar` & `ayon-python-api-0.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.862134 ayon-python-api-0.2.1/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30053 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   180006 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:28:06.000000 ayon-python-api-0.2.1/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:28:06.866135 ayon-python-api-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-13 09:27:58.000000 ayon-python-api-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   182164 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/setup.py
```

### Comparing `ayon-python-api-0.2.1/LICENSE` & `ayon-python-api-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/PKG-INFO` & `ayon-python-api-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Keywords: AYON,ynput,OpenPype,vfx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ayon-python-api-0.2.1/README.md` & `ayon-python-api-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/__init__.py` & `ayon-python-api-0.2.2/ayon_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,14 +112,15 @@
     update_project,
     delete_project,
 
     get_folder_by_id,
     get_folder_by_name,
     get_folder_by_path,
     get_folders,
+    get_folders_hierarchy,
 
     get_tasks,
 
     get_folder_ids_with_products,
     get_product_by_id,
     get_product_by_name,
     get_products,
```

### Comparing `ayon-python-api-0.2.1/ayon_api/_api.py` & `ayon-python-api-0.2.2/ayon_api/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,14 +719,19 @@
 
 
 def get_folders(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_folders(*args, **kwargs)
 
 
+def get_folders_hierarchy(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_folders_hierarchy(*args, **kwargs)
+
+
 def get_tasks(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_tasks(*args, **kwargs)
 
 
 def get_folder_by_id(*args, **kwargs):
     con = get_server_api_connection()
```

### Comparing `ayon-python-api-0.2.1/ayon_api/constants.py` & `ayon-python-api-0.2.2/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/entity_hub.py` & `ayon-python-api-0.2.2/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/events.py` & `ayon-python-api-0.2.2/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/exceptions.py` & `ayon-python-api-0.2.2/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/graphql.py` & `ayon-python-api-0.2.2/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/graphql_queries.py` & `ayon-python-api-0.2.2/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/operations.py` & `ayon-python-api-0.2.2/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/server_api.py` & `ayon-python-api-0.2.2/ayon_api/server_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,36 +309,56 @@
         site_id (Optional[str]): Unique name of site. Should be the same when
             connection is created from the same machine under same user.
         client_version (Optional[str]): Version of client application (used in
             desktop client application).
         default_settings_variant (Optional[str]): Settings variant used by
             default if a method for settings won't get any (by default is
             'production').
+        ssl_verify (Union[bool, str, None]): Verify SSL certificate
+            Looks for env variable value 'AYON_CA_FILE' by default. If not
+            available then 'True' is used.
+        cert (Optional[str]): Path to certificate file. Looks for env
+            variable value 'AYON_CERT_FILE' by default.
     """
 
     def __init__(
         self,
         base_url,
         token=None,
         site_id=None,
         client_version=None,
-        default_settings_variant=None
+        default_settings_variant=None,
+        ssl_verify=None,
+        cert=None,
     ):
         if not base_url:
             raise ValueError("Invalid server URL {}".format(str(base_url)))
 
         base_url = base_url.rstrip("/")
         self._base_url = base_url
         self._rest_url = "{}/api".format(base_url)
         self._graphql_url = "{}/graphql".format(base_url)
         self._log = None
         self._access_token = token
         self._site_id = site_id
         self._client_version = client_version
         self._default_settings_variant = default_settings_variant
+
+        if ssl_verify is None:
+            # Custom AYON env variable for CA file or 'True'
+            # - that should cover most default behaviors in 'requests'
+            #   with 'certifi'
+            ssl_verify = os.environ.get("AYON_CA_FILE") or True
+
+        if cert is None:
+            cert = os.environ.get("AYON_CERT_FILE")
+
+        self._ssl_verify = ssl_verify
+        self._cert = cert
+
         self._access_token_is_service = None
         self._token_is_valid = None
         self._server_available = None
         self._server_version = None
         self._server_version_tuple = None
 
         self._session = None
@@ -370,14 +390,62 @@
 
     def get_rest_url(self):
         return self._rest_url
 
     base_url = property(get_base_url)
     rest_url = property(get_rest_url)
 
+    def get_ssl_verify(self):
+        """Enable ssl verification.
+
+        Returns:
+            bool: Current state of ssl verification.
+        """
+
+        return self._ssl_verify
+
+    def set_ssl_verify(self, ssl_verify):
+        """Change ssl verification state.
+
+        Args:
+            ssl_verify (Union[bool, str, None]): Enabled/disable
+                ssl verification, can be a path to file.
+        """
+
+        if self._ssl_verify == ssl_verify:
+            return
+        self._ssl_verify = ssl_verify
+        if self._session is not None:
+            self._session.verify = ssl_verify
+
+    def get_cert(self):
+        """Current cert file used for connection to server.
+
+        Returns:
+            Union[str, None]: Path to cert file.
+        """
+
+        return self._cert
+
+    def set_cert(self, cert):
+        """Change cert file used for connection to server.
+
+        Args:
+            cert (Union[str, None]): Path to cert file.
+        """
+
+        if cert == self._cert:
+            return
+        self._cert = cert
+        if self._session is not None:
+            self._session.cert = cert
+
+    ssl_verify = property(get_ssl_verify, set_ssl_verify)
+    cert = property(get_cert, set_cert)
+
     @property
     def access_token(self):
         """Access token used for authorization to server.
 
         Returns:
             Union[str, None]: Token string or None if not authorized yet.
         """
@@ -541,15 +609,19 @@
                 yield o
             finally:
                 self._update_session_headers()
 
     @property
     def is_server_available(self):
         if self._server_available is None:
-            response = requests.get(self._base_url)
+            response = requests.get(
+                self._base_url,
+                cert=self._cert,
+                verify=self._ssl_verify
+            )
             self._server_available = response.status_code == 200
         return self._server_available
 
     @property
     def has_valid_token(self):
         if self._access_token is None:
             return False
@@ -592,14 +664,16 @@
             raise ValueError("Session is already created.")
 
         self._as_user_stack.clear()
         # Validate token before session creation
         self.validate_token()
 
         session = requests.Session()
+        session.cert = self._cert
+        session.verify = self._ssl_verify
         session.headers.update(self.get_headers())
 
         self._session_functions_mapping = {
             RequestTypes.get: session.get,
             RequestTypes.post: session.post,
             RequestTypes.put: session.put,
             RequestTypes.patch: session.patch,
```

### Comparing `ayon-python-api-0.2.1/ayon_api/thumbnails.py` & `ayon-python-api-0.2.2/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_api/utils.py` & `ayon-python-api-0.2.2/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.2.2/ayon_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.2.1
+Version: 0.2.2
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: info@ynput.io
 License: Apache License (2.0)
 Keywords: AYON,ynput,OpenPype,vfx
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ayon-python-api-0.2.1/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.2.2/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.1/setup.py` & `ayon-python-api-0.2.2/setup.py`

 * *Files identical despite different names*

