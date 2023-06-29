# Comparing `tmp/omada_api-0.1.2.tar.gz` & `tmp/omada_api-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omada_api-0.1.2.tar", max compression
+gzip compressed data, was "omada_api-0.1.3.tar", max compression
```

## Comparing `omada_api-0.1.2.tar` & `omada_api-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-06-28 09:12:09.565932 omada_api-0.1.2/LICENSE
--rw-r--r--   0        0        0     3686 2023-06-28 09:12:09.565932 omada_api-0.1.2/README.md
--rw-r--r--   0        0        0      106 2023-06-28 09:12:09.565932 omada_api-0.1.2/omada/__init__.py
--rw-r--r--   0        0        0      524 2023-06-28 09:12:09.565932 omada_api-0.1.2/omada/api_bindings.py
--rw-r--r--   0        0        0      475 2023-06-28 09:12:09.565932 omada_api-0.1.2/omada/function_interface_bindings.py
--rw-r--r--   0        0        0    12658 2023-06-28 09:12:09.565932 omada_api-0.1.2/omada/omada.py
--rw-r--r--   0        0        0     2062 2023-06-28 09:12:19.418105 omada_api-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 omada_api-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-29 14:18:39.476672 omada_api-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3686 2023-06-29 14:18:39.476672 omada_api-0.1.3/README.md
+-rw-r--r--   0        0        0      106 2023-06-29 14:18:39.476672 omada_api-0.1.3/omada/__init__.py
+-rw-r--r--   0        0        0      524 2023-06-29 14:18:39.476672 omada_api-0.1.3/omada/api_bindings.py
+-rw-r--r--   0        0        0      475 2023-06-29 14:18:39.476672 omada_api-0.1.3/omada/function_interface_bindings.py
+-rw-r--r--   0        0        0    12757 2023-06-29 14:18:39.476672 omada_api-0.1.3/omada/omada.py
+-rw-r--r--   0        0        0     2062 2023-06-29 14:18:48.044827 omada_api-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 omada_api-0.1.3/PKG-INFO
```

### Comparing `omada_api-0.1.2/LICENSE` & `omada_api-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `omada_api-0.1.2/README.md` & `omada_api-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `omada_api-0.1.2/omada/api_bindings.py` & `omada_api-0.1.3/omada/api_bindings.py`

 * *Files identical despite different names*

### Comparing `omada_api-0.1.2/omada/omada.py` & `omada_api-0.1.3/omada/omada.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,20 +281,23 @@
     def get_site_devices(
         self, site: typing.Optional[str] = None
     ) -> typing.Iterable[dict]:
         """Returns the list of devices for given site."""
         return self._get(f"sites/{self._find_site(site)}/devices")
 
     def get_site_clients(
-        self, site: typing.Optional[str] = None, active: bool = True
+        self, site: typing.Optional[str] = None, active: typing.Optional[bool] = True
     ) -> typing.Iterable[dict]:
         """Returns the list of active clients for given site."""
+        params = {}
+        if active in (True, False):
+            params["filters.active"] = "true" if active else "false"
         return self._geterator(
             f"sites/{self._find_site(site)}/clients",
-            params={"filters.active": "true" if active else "false"},
+            params=params,
         )
 
     def get_site_alerts(
         self, site: typing.Optional[str] = None, archived: bool = False
     ) -> typing.Iterable[dict]:
         """Returns the list of alerts for given site."""
         params = {"filters.archived": "true" if archived else "false"}
```

### Comparing `omada_api-0.1.2/pyproject.toml` & `omada_api-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "omada-api"
-version = "v0.1.2"
+version = "v0.1.3"
 description = "A simple Python wrapper for the TP-Link Omada Software Controller API"
 authors = ["Ilja O <vrghost@gmail.com>", "Gregory Haberek <ghaberek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "omada"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `omada_api-0.1.2/PKG-INFO` & `omada_api-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omada-api
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple Python wrapper for the TP-Link Omada Software Controller API
 License: MIT
 Keywords: tplink,omada,wrapper
 Author: Ilja O
 Author-email: vrghost@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

