# Comparing `tmp/ayon-python-api-0.3.0.tar.gz` & `tmp/ayon-python-api-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.3.0.tar", last modified: Thu Jun 29 10:10:25 2023, max compression
+gzip compressed data, was "ayon-python-api-0.3.1.tar", last modified: Thu Jun 29 15:14:29 2023, max compression
```

## Comparing `ayon-python-api-0.3.0.tar` & `ayon-python-api-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.258815 ayon-python-api-0.3.0/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   187411 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.796687 ayon-python-api-0.3.1/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187387 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:14:29.796687 ayon-python-api-0.3.1/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:14:29.000000 ayon-python-api-0.3.1/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:14:29.800687 ayon-python-api-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 15:14:20.000000 ayon-python-api-0.3.1/setup.py
```

### Comparing `ayon-python-api-0.3.0/LICENSE` & `ayon-python-api-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/PKG-INFO` & `ayon-python-api-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.0/README.md` & `ayon-python-api-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/__init__.py` & `ayon-python-api-0.3.1/ayon_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/_api.py` & `ayon-python-api-0.3.1/ayon_api/_api.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/constants.py` & `ayon-python-api-0.3.1/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/entity_hub.py` & `ayon-python-api-0.3.1/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/events.py` & `ayon-python-api-0.3.1/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/exceptions.py` & `ayon-python-api-0.3.1/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/graphql.py` & `ayon-python-api-0.3.1/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/graphql_queries.py` & `ayon-python-api-0.3.1/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/operations.py` & `ayon-python-api-0.3.1/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/server_api.py` & `ayon-python-api-0.3.1/ayon_api/server_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1960,14 +1960,32 @@
                 server.
         """
 
         result = self.get("desktop/dependency_packages")
         result.raise_for_status()
         return result.data
 
+    def _get_dependency_package_route(
+        self, filename=None, platform_name=None
+    ):
+        major, minor, patch, _, _ = self.server_version_tuple
+        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
+            base = "desktop/dependency_packages"
+            if not filename:
+                return base
+            return "{}/{}".format(base, filename)
+
+        # Backwards compatibility for AYON server 0.2.0 and lower
+        if platform_name is None:
+            platform_name = platform.system().lower()
+        base = "dependencies"
+        if not filename:
+            return base
+        return "{}/{}/{}".format(base, filename, platform_name)
+
     def create_dependency_package(
         self,
         filename,
         python_modules,
         source_addons,
         installer_version,
         checksum,
@@ -2010,29 +2028,30 @@
             "checksumAlgorithm": checksum_algorithm,
             "size": file_size,
             "platform": platform_name or platform.system().lower(),
         }
         if sources:
             post_body["sources"] = sources
 
-        response = self.post("desktop/dependency_packages", **post_body)
+        route = self._get_dependency_package_route()
+        response = self.post(route, **post_body)
         response.raise_for_status()
 
     def update_dependency_package(self, filename, sources):
         """Update dependency package metadata on server.
 
         Args:
             filename (str): Filename of dependency package.
             sources (list[dict[str, Any]]): Information about
                 sources from where it is possible to get file. Fully replaces
                 existing sources.
         """
 
         response = self.patch(
-            "desktop/dependency_packages/{}".format(filename),
+            self._get_dependency_package_route(filename),
             sources=sources
         )
         response.raise_for_status()
 
     def delete_dependency_package(self, filename, platform_name=None):
         """Remove dependency package for specific platform.
 
@@ -2040,24 +2059,16 @@
             filename (str): Filename of dependency package. Or name of package
                 for server version 0.2.0 or lower.
             platform_name (Optional[str]): Which platform of the package
                 should be removed. Current platform is used if not passed.
                 Deprecated since version 0.2.1
         """
 
-        major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
-            url = "desktop/dependency_packages/{}".format(filename)
-        else:
-            # Backwards compatibility for AYON server 0.2.0 and lower
-            if platform_name is None:
-                platform_name = platform.system().lower()
-            url = "dependencies/{}/{}".format(filename, platform_name)
-
-        response = self.delete(url)
+        route = self._get_dependency_package_route(filename, platform_name)
+        response = self.delete(route)
         if response.status != 200:
             raise ServerError("Failed to delete dependency file")
         return response.data
 
     def download_dependency_package(
         self,
         src_filename,
@@ -2085,26 +2096,18 @@
             progress (Optional[TransferProgress]): Object that gives ability
                 to track download progress.
 
         Returns:
             str: Filepath to downloaded file.
        """
 
-        major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
-            url = "desktop/dependency_packages/{}".format(src_filename)
-        else:
-            # Backwards compatibility for AYON server 0.2.0 and lower
-            if platform_name is None:
-                platform_name = platform.system().lower()
-            url = "dependencies/{}/{}".format(src_filename, platform_name)
-
+        route = self._get_dependency_package_route(src_filename, platform_name)
         package_filepath = os.path.join(dst_directory, dst_filename)
         self.download_file(
-            url,
+            route,
             package_filepath,
             chunk_size=chunk_size,
             progress=progress
         )
         return package_filepath
 
     def upload_dependency_package(
@@ -2118,24 +2121,16 @@
                 for server version 0.2.0 or lower. Must be unique.
             platform_name (Optional[str]): For which platform is the
                 package targeted. Deprecated since server version 0.2.1.
             progress (Optional[TransferProgress]): Object to keep track about
                 upload state.
         """
 
-        major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
-            url = "desktop/dependency_packages/{}".format(dst_filename)
-        else:
-            # Backwards compatibility for AYON server 0.2.0 and lower
-            if platform_name is None:
-                platform_name = platform.system().lower()
-            url = "dependencies/{}/{}".format(dst_filename, platform_name)
-
-        self.upload_file(url, src_filepath, progress=progress)
+        route = self._get_dependency_package_route(dst_filename, platform_name)
+        self.upload_file(route, src_filepath, progress=progress)
 
     def create_dependency_package_basename(self, platform_name=None):
         """Create basename for dependency package file.
 
         Args:
             platform_name (Optional[str]): Name of platform for which the
                 bundle is targeted. Default value is current platform.
@@ -2147,14 +2142,22 @@
         if platform_name is None:
             platform_name = platform.system().lower()
 
         now_date = datetime.datetime.now()
         time_stamp = now_date.strftime("%y%m%d%H%M")
         return "ayon_{}_{}".format(time_stamp, platform_name)
 
+    def _get_bundles_route(self):
+        major, minor, patch, _, _ = self.server_version_tuple
+        # Backwards compatibility for AYON server 0.3.0
+        # - first version where bundles were available
+        if major == 0 and minor == 3 and patch == 0:
+            return "desktop/bundles"
+        return "bundles"
+
     def get_bundles(self):
         """Server bundles with basic information.
 
         Example output:
             {
                 "bundles": [
                     {
@@ -2177,15 +2180,15 @@
                 "stagingBundle": "test_bundle"
             }
 
         Returns:
             dict[str, Any]: Server bundles with basic information.
         """
 
-        response = self.get("desktop/bundles")
+        response = self.get(self._get_bundles_route())
         response.raise_for_status()
         return response.data
 
     def create_bundle(
         self,
         name,
         addon_versions,
@@ -2220,15 +2223,15 @@
             ("dependencyPackages", dependency_packages),
             ("isProduction", is_production),
             ("isStaging", is_staging),
         ):
             if value is not None:
                 body[key] = value
 
-        response = self.post("desktop/bundles", **body)
+        response = self.post(self._get_bundles_route(), **body)
         response.raise_for_status()
 
     def update_bundle(
         self,
         bundle_name,
         dependency_packages=None,
         is_production=None,
@@ -2255,26 +2258,29 @@
                 ("dependencyPackages", dependency_packages),
                 ("isProduction", is_production),
                 ("isStaging", is_staging),
             )
             if value is not None
         }
         response = self.patch(
-            "desktop/bundles/{}".format(bundle_name), **body
+            "{}/{}".format(self._get_bundles_route(), bundle_name),
+            **body
         )
         response.raise_for_status()
 
     def delete_bundle(self, bundle_name):
         """Delete bundle from server.
 
         Args:
             bundle_name (str): Name of bundle to delete.
         """
 
-        response = self.delete("desktop/bundles/{}".format(bundle_name))
+        response = self.delete(
+            "{}/{}".format(self._get_bundles_route(), bundle_name)
+        )
         response.raise_for_status()
 
     # Anatomy presets
     def get_project_anatomy_presets(self):
         """Anatomy presets available on server.
 
         Content has basic information about presets. Example output:
```

### Comparing `ayon-python-api-0.3.0/ayon_api/thumbnails.py` & `ayon-python-api-0.3.1/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_api/utils.py` & `ayon-python-api-0.3.1/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/ayon_python_api.egg-info/PKG-INFO` & `ayon-python-api-0.3.1/ayon_python_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ayon-python-api
-Version: 0.3.0
+Version: 0.3.1
 Summary: AYON Python API
 Home-page: https://github.com/ynput/ayon-python-api
 Author: ynput.io
 Author-email: "ynput.io" <info@ynput.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `ayon-python-api-0.3.0/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.3.1/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.3.0/pyproject.toml` & `ayon-python-api-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ayon-python-api"
-version = "0.3.0"
+version = "0.3.1"
 description = "AYON Python API"
 license = {file = "LICENSE"}
 readme = {file = "README.md", content-type = "text/markdown"}
 authors = [
     {name = "ynput.io", email = "info@ynput.io"}
 ]
 keywords = ["AYON", "ynput", "OpenPype", "vfx"]
```

### Comparing `ayon-python-api-0.3.0/setup.py` & `ayon-python-api-0.3.1/setup.py`

 * *Files identical despite different names*

