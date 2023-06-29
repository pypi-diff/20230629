# Comparing `tmp/polytope-client-0.6.3.tar.gz` & `tmp/polytope-client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polytope-client-0.6.3.tar", last modified: Thu Feb  3 00:22:20 2022, max compression
+gzip compressed data, was "polytope-client-0.7.1.tar", last modified: Thu Jun 29 16:12:39 2023, max compression
```

## Comparing `polytope-client-0.6.3.tar` & `polytope-client-0.7.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.739525 polytope-client-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11380 2022-02-03 00:22:11.000000 polytope-client-0.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-03 00:22:11.000000 polytope-client-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-03 00:22:20.739525 polytope-client-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6474 2022-02-03 00:22:11.000000 polytope-client-0.6.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.735525 polytope-client-0.6.3/polytope/
--rw-r--r--   0 runner    (1001) docker     (121)     1205 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.735525 polytope-client-0.6.3/polytope/api/
--rw-r--r--   0 runner    (1001) docker     (121)     3157 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/Admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    10510 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/Auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     8310 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/Client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2509 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/CollectionVisitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    20113 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/Config.py
--rw-r--r--   0 runner    (1001) docker     (121)    44595 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/RequestManager.py
--rw-r--r--   0 runner    (1001) docker     (121)     2553 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/Result.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/config_schema.json
--rw-r--r--   0 runner    (1001) docker     (121)    21745 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/api/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.735525 polytope-client-0.6.3/polytope/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1055 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.735525 polytope-client-0.6.3/polytope/cli/binders/
--rw-r--r--   0 runner    (1001) docker     (121)     1034 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2278 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3393 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     6933 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/binders/request.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2455 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-03 00:22:11.000000 polytope-client-0.6.3/polytope/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-03 00:22:20.739525 polytope-client-0.6.3/polytope_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-02-03 00:22:20.000000 polytope-client-0.6.3/polytope_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-02-03 00:22:11.000000 polytope-client-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-03 00:22:20.739525 polytope-client-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-02-03 00:22:11.000000 polytope-client-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.814700 polytope-client-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11380 2023-06-29 16:12:26.000000 polytope-client-0.7.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 16:12:26.000000 polytope-client-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 16:12:39.814700 polytope-client-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-06-29 16:12:26.000000 polytope-client-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.810699 polytope-client-0.7.1/polytope/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.810699 polytope-client-0.7.1/polytope/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/Admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/Auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8310 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/CollectionVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20113 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45070 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/RequestManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/Result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/config_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21745 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/api/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.810699 polytope-client-0.7.1/polytope/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.810699 polytope-client-0.7.1/polytope/cli/binders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/binders/request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2455 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 16:12:26.000000 polytope-client-0.7.1/polytope/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:12:39.814700 polytope-client-0.7.1/polytope_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 16:12:39.000000 polytope-client-0.7.1/polytope_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-29 16:12:26.000000 polytope-client-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:12:39.814700 polytope-client-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-29 16:12:26.000000 polytope-client-0.7.1/setup.py
```

### Comparing `polytope-client-0.6.3/LICENSE.txt` & `polytope-client-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/PKG-INFO` & `polytope-client-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: polytope-client
-Version: 0.6.3
+Version: 0.7.1
 Summary: A Python and command-line client to communicate with a Polytope API server.
 Home-page: https://github.com/ecmwf-projects/polytope-client
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `polytope-client-0.6.3/README.md` & `polytope-client-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/__init__.py` & `polytope-client-0.7.1/polytope/__init__.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/Admin.py` & `polytope-client-0.7.1/polytope/api/Admin.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/Auth.py` & `polytope-client-0.7.1/polytope/api/Auth.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/Client.py` & `polytope-client-0.7.1/polytope/api/Client.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/CollectionVisitor.py` & `polytope-client-0.7.1/polytope/api/CollectionVisitor.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/Config.py` & `polytope-client-0.7.1/polytope/api/Config.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/RequestManager.py` & `polytope-client-0.7.1/polytope/api/RequestManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,18 +325,27 @@
         helpers.recover_stream_handler_level(self._logger, replaced_level)
         if name not in colls:
             raise ValueError("Collection name '" + name + "' not available.")
 
         if not inline_request:
             self._logger.info("Reading request file...")
             request = os.path.expanduser(request)
-            with open(request) as request_file_handler:
-                request = yaml.safe_load(request_file_handler)
+            # If we receive a file, pass it on as a string
+            with open(request, "r") as request_file_handler:
+                request = request_file_handler.read()
         else:
-            request = copy.deepcopy(request)
+            # If we receive a Python dictionary, encode it as yaml
+            # TODO: we don't know what the eventual data source requires,
+            # encoding to YAML is the most flexible approach for now, but
+            # this needs a more robust solution.
+            if isinstance(request, dict):
+                request = yaml.safe_dump(request)
+            # else try to convert plainly to string
+            else:
+                request = str(request)
         if not isinstance(request, list):
             user_requests = [request]
         else:
             user_requests = request
 
         request_ids_pending_for_download = []
         request_urls_pending_for_download = []
```

### Comparing `polytope-client-0.6.3/polytope/api/Result.py` & `polytope-client-0.7.1/polytope/api/Result.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/__init__.py` & `polytope-client-0.7.1/polytope/api/__init__.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/config_schema.json` & `polytope-client-0.7.1/polytope/api/config_schema.json`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/api/helpers.py` & `polytope-client-0.7.1/polytope/api/helpers.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/__init__.py` & `polytope-client-0.7.1/polytope/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/__init__.py` & `polytope-client-0.7.1/polytope/cli/binders/__init__.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/admin.py` & `polytope-client-0.7.1/polytope/cli/binders/admin.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/auth.py` & `polytope-client-0.7.1/polytope/cli/binders/auth.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/collection.py` & `polytope-client-0.7.1/polytope/cli/binders/collection.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/config.py` & `polytope-client-0.7.1/polytope/cli/binders/config.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/helpers.py` & `polytope-client-0.7.1/polytope/cli/binders/helpers.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/binders/request.py` & `polytope-client-0.7.1/polytope/cli/binders/request.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope/cli/cli.py` & `polytope-client-0.7.1/polytope/cli/cli.py`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/polytope_client.egg-info/PKG-INFO` & `polytope-client-0.7.1/polytope_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: polytope-client
-Version: 0.6.3
+Version: 0.7.1
 Summary: A Python and command-line client to communicate with a Polytope API server.
 Home-page: https://github.com/ecmwf-projects/polytope-client
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `polytope-client-0.6.3/polytope_client.egg-info/SOURCES.txt` & `polytope-client-0.7.1/polytope_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polytope-client-0.6.3/setup.py` & `polytope-client-0.7.1/setup.py`

 * *Files identical despite different names*

