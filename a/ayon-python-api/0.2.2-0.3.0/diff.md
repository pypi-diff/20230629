# Comparing `tmp/ayon-python-api-0.2.2.tar.gz` & `tmp/ayon-python-api-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayon-python-api-0.2.2.tar", last modified: Thu Jun 29 09:01:00 2023, max compression
+gzip compressed data, was "ayon-python-api-0.3.0.tar", last modified: Thu Jun 29 10:10:25 2023, max compression
```

## Comparing `ayon-python-api-0.2.2.tar` & `ayon-python-api-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/ayon_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30191 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/entity_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/graphql_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)   182164 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/thumbnails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/ayon_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/ayon_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 09:01:00.000000 ayon-python-api-0.2.2/ayon_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 09:01:00.908345 ayon-python-api-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 09:00:55.000000 ayon-python-api-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.258815 ayon-python-api-0.3.0/ayon_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30325 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59757 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/entity_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25639 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/graphql_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)   187411 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6856 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/thumbnails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/ayon_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/ayon_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16231 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 10:10:25.000000 ayon-python-api-0.3.0/ayon_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:10:25.262815 ayon-python-api-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 10:10:12.000000 ayon-python-api-0.3.0/setup.py
```

### Comparing `ayon-python-api-0.2.2/LICENSE` & `ayon-python-api-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/PKG-INFO` & `ayon-python-api-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: ayon-python-api
-Version: 0.2.2
-Summary: AYON Python API
-Home-page: https://github.com/ynput/ayon-python-api
-Author: ynput.io
-Author-email: info@ynput.io
-License: Apache License (2.0)
-Keywords: AYON,ynput,OpenPype,vfx
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # AYON server API
 Python client for connection server. Client must be (at least for some time) Python 2 compatible because will be used in DCC that are "older".
 
 AYON Python api should support connection to server with raw REST functions and prepared functionality for work with entities. Must not contain only functionality that can be used with core server functionality.
 
 Module support singleton connection which is using `AYON_SERVER_URL` and `AYON_API_KEY` environment variables as source for connection. The singleton connection is using `ServerAPI` object. There can be created multiple connection to different server at one time, for that purpose use `ServerAPIBase` object.
```

### Comparing `ayon-python-api-0.2.2/ayon_api/__init__.py` & `ayon-python-api-0.3.0/ayon_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 
     get_addon_site_settings_schema,
     get_addon_settings_schema,
 
     get_addon_studio_settings,
     get_addon_project_settings,
     get_addon_settings,
+    get_bundle_settings,
     get_addons_studio_settings,
     get_addons_project_settings,
     get_addons_settings,
 
     get_project_names,
     get_projects,
     get_project,
@@ -276,14 +277,15 @@
     "get_project_roots_for_site",
 
     "get_addon_site_settings_schema",
     "get_addon_settings_schema",
     "get_addon_studio_settings",
     "get_addon_project_settings",
     "get_addon_settings",
+    "get_bundle_settings",
     "get_addons_studio_settings",
     "get_addons_project_settings",
     "get_addons_settings",
 
     "get_project_names",
     "get_projects",
     "get_project",
```

### Comparing `ayon-python-api-0.2.2/ayon_api/_api.py` & `ayon-python-api-0.3.0/ayon_api/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -684,14 +684,19 @@
 
 
 def get_addon_site_settings(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_addon_site_settings(*args, **kwargs)
 
 
+def get_bundle_settings(*args, **kwargs):
+    con = get_server_api_connection()
+    return con.get_bundle_settings(*args, **kwargs)
+
+
 def get_addons_studio_settings(*args, **kwargs):
     con = get_server_api_connection()
     return con.get_addons_studio_settings(*args, **kwargs)
 
 
 def get_addons_project_settings(*args, **kwargs):
     con = get_server_api_connection()
```

### Comparing `ayon-python-api-0.2.2/ayon_api/constants.py` & `ayon-python-api-0.3.0/ayon_api/constants.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/entity_hub.py` & `ayon-python-api-0.3.0/ayon_api/entity_hub.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/events.py` & `ayon-python-api-0.3.0/ayon_api/events.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/exceptions.py` & `ayon-python-api-0.3.0/ayon_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/graphql.py` & `ayon-python-api-0.3.0/ayon_api/graphql.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/graphql_queries.py` & `ayon-python-api-0.3.0/ayon_api/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/operations.py` & `ayon-python-api-0.3.0/ayon_api/operations.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/server_api.py` & `ayon-python-api-0.3.0/ayon_api/server_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,17 +306,17 @@
     Args:
         base_url (str): Example: http://localhost:5000
         token (Optional[str]): Access token (api key) to server.
         site_id (Optional[str]): Unique name of site. Should be the same when
             connection is created from the same machine under same user.
         client_version (Optional[str]): Version of client application (used in
             desktop client application).
-        default_settings_variant (Optional[str]): Settings variant used by
-            default if a method for settings won't get any (by default is
-            'production').
+        default_settings_variant (Optional[Literal["production", "staging"]]):
+            Settings variant used by default if a method for settings won't
+            get any (by default is 'production').
         ssl_verify (Union[bool, str, None]): Verify SSL certificate
             Looks for env variable value 'AYON_CA_FILE' by default. If not
             available then 'True' is used.
         cert (Optional[str]): Path to certificate file. Looks for env
             variable value 'AYON_CERT_FILE' by default.
     """
 
@@ -337,15 +337,18 @@
         self._base_url = base_url
         self._rest_url = "{}/api".format(base_url)
         self._graphql_url = "{}/graphql".format(base_url)
         self._log = None
         self._access_token = token
         self._site_id = site_id
         self._client_version = client_version
-        self._default_settings_variant = default_settings_variant
+        self._default_settings_variant = (
+            default_settings_variant
+            or "production"
+        )
 
         if ssl_verify is None:
             # Custom AYON env variable for CA file or 'True'
             # - that should cover most default behaviors in 'requests'
             #   with 'certifi'
             ssl_verify = os.environ.get("AYON_CA_FILE") or True
 
@@ -523,17 +526,21 @@
         """Change default variant for addon settings.
 
         Note:
             It is recommended to set only 'production' or 'staging' variants
                 as default variant.
 
         Args:
-            variant (Union[str, None]): Settings variant name.
+            variant (Literal['production', 'staging']): Settings variant name.
         """
 
+        if variant not in ("production", "staging"):
+            raise ValueError((
+                "Invalid variant name {}. Expected 'production' or 'staging'"
+            ).format(variant))
         self._default_settings_variant = variant
 
     default_settings_variant = property(
         get_default_settings_variant,
         set_default_settings_variant
     )
 
@@ -2034,20 +2041,21 @@
                 for server version 0.2.0 or lower.
             platform_name (Optional[str]): Which platform of the package
                 should be removed. Current platform is used if not passed.
                 Deprecated since version 0.2.1
         """
 
         major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
+            url = "desktop/dependency_packages/{}".format(filename)
+        else:
+            # Backwards compatibility for AYON server 0.2.0 and lower
             if platform_name is None:
                 platform_name = platform.system().lower()
             url = "dependencies/{}/{}".format(filename, platform_name)
-        else:
-            url = "desktop/dependency_packages/{}".format(filename)
 
         response = self.delete(url)
         if response.status != 200:
             raise ServerError("Failed to delete dependency file")
         return response.data
 
     def download_dependency_package(
@@ -2078,20 +2086,21 @@
                 to track download progress.
 
         Returns:
             str: Filepath to downloaded file.
        """
 
         major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
+            url = "desktop/dependency_packages/{}".format(src_filename)
+        else:
+            # Backwards compatibility for AYON server 0.2.0 and lower
             if platform_name is None:
                 platform_name = platform.system().lower()
             url = "dependencies/{}/{}".format(src_filename, platform_name)
-        else:
-            url = "desktop/dependency_packages/{}".format(src_filename)
 
         package_filepath = os.path.join(dst_directory, dst_filename)
         self.download_file(
             url,
             package_filepath,
             chunk_size=chunk_size,
             progress=progress
@@ -2110,20 +2119,21 @@
             platform_name (Optional[str]): For which platform is the
                 package targeted. Deprecated since server version 0.2.1.
             progress (Optional[TransferProgress]): Object to keep track about
                 upload state.
         """
 
         major, minor, patch, _, _ = self.server_version_tuple
-        if major == 0 and (minor < 2 or (minor == 2 and patch < 1)):
+        if major == 0 and (minor > 2 or (minor == 2 and patch >= 1)):
+            url = "desktop/dependency_packages/{}".format(dst_filename)
+        else:
+            # Backwards compatibility for AYON server 0.2.0 and lower
             if platform_name is None:
                 platform_name = platform.system().lower()
             url = "dependencies/{}/{}".format(dst_filename, platform_name)
-        else:
-            url = "desktop/dependency_packages/{}".format(dst_filename)
 
         self.upload_file(url, src_filepath, progress=progress)
 
     def create_dependency_package_basename(self, platform_name=None):
         """Create basename for dependency package file.
 
         Args:
@@ -2400,25 +2410,25 @@
         self,
         addon_name,
         addon_version,
         variant=None
     ):
         """Addon studio settings.
 
-       Receive studio settings for specific version of an addon.
+        Receive studio settings for specific version of an addon.
 
-       Args:
-           addon_name (str): Name of addon.
-           addon_version (str): Version of addon.
-           variant (Optional[str]): Name of settings variant. By default,
-                is used 'default_settings_variant' passed on init.
+        Args:
+            addon_name (str): Name of addon.
+            addon_version (str): Version of addon.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
 
-       Returns:
+        Returns:
            dict[str, Any]: Addon settings.
-       """
+        """
 
         if variant is None:
             variant = self.default_settings_variant
 
         query_items = {}
         if variant:
             query_items["variant"] = variant
@@ -2448,16 +2458,16 @@
         make sure any site id is used set 'use_site' to 'False'.
 
         Args:
             addon_name (str): Name of addon.
             addon_version (str): Version of addon.
             project_name (str): Name of project for which the settings are
                 received.
-            variant (Optional[str]): Name of settings variant. By default,
-                is used 'production'.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
             site_id (Optional[str]): Name of site which is used for site
                 overrides. Is filled with connection 'site_id' attribute
                 if not passed.
             use_site (Optional[bool]): To force disable option of using site
                 overrides set to 'False'. In that case won't be applied
                 any site overrides.
 
@@ -2505,16 +2515,16 @@
 
         Args:
             addon_name (str): Name of addon.
             addon_version (str): Version of addon.
             project_name (Optional[str]): Name of project for which the
                 settings are received. A studio settings values are received
                 if is 'None'.
-            variant (Optional[str]): Name of settings variant. By default,
-                is used 'production'.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
             site_id (Optional[str]): Name of site which is used for site
                 overrides. Is filled with connection 'site_id' attribute
                 if not passed.
             use_site (Optional[bool]): To force disable option of using
                 site overrides set to 'False'. In that case won't be applied
                 any site overrides.
 
@@ -2556,41 +2566,143 @@
         query = prepare_query_string({"site": site_id})
         result = self.get("addons/{}/{}/siteSettings{}".format(
             addon_name, addon_version, query
         ))
         result.raise_for_status()
         return result.data
 
-    def get_addons_studio_settings(self, variant=None, only_values=True):
+    def get_bundle_settings(
+        self,
+        bundle_name=None,
+        project_name=None,
+        variant=None,
+        site_id=None,
+        use_site=True
+    ):
+        """Get complete set of settings for given data.
+
+        If project is not passed then studio settings are returned. If variant
+        is not passed 'default_settings_variant' is used. If bundle name is
+        not passed then current production/staging bundle is used, based on
+        variant value.
+
+        Output contains addon settings and site settings in single dictionary.
+
+        TODOs:
+            - test how it behaves if there is not any bundle.
+            - test how it behaves if there is not any production/staging
+                bundle.
+
+        Warnings:
+            For AYON server < 0.3.0 bundle name will be ignored.
+
+        Example output:
+            {
+                "addons": [
+                    {
+                        "name": "addon-name",
+                        "version": "addon-version",
+                        "settings": {...}
+                        "siteSettings": {...}
+                    }
+                ]
+            }
+
+        Returns:
+            dict[str, Any]: All settings for single bundle.
+        """
+
+        major, minor, _, _, _ = self.server_version_tuple
+        query_values = {
+            key: value
+            for key, value in (
+                ("project_name", project_name),
+                ("variant", variant or self.default_settings_variant),
+                ("bundle_name", bundle_name),
+            )
+            if value
+        }
+        if use_site:
+            if not site_id:
+                site_id = self.site_id
+            if site_id:
+                query_values["site_id"] = site_id
+
+        if major == 0 and minor >= 3:
+            url = "settings"
+        else:
+            # Backward compatibility for AYON server < 0.3.0
+            url = "settings/addons"
+            query_values.pop("bundle_name", None)
+            for new_key, old_key in (
+                ("project_name", "project"),
+                ("site_id", "site"),
+            ):
+                if new_key in query_values:
+                    query_values[old_key] = query_values.pop(new_key)
+
+        query = prepare_query_string(query_values)
+        response = self.get("{}{}".format(url, query))
+        response.raise_for_status()
+        return response.data
+
+    def get_addons_studio_settings(
+        self,
+        bundle_name=None,
+        variant=None,
+        site_id=None,
+        use_site=True,
+        only_values=True
+    ):
         """All addons settings in one bulk.
 
+        Warnings:
+            Behavior of this function changed with AYON server version 0.3.0.
+                Structure of output from server changed. If using
+                'only_values=True' then output should be same as before.
+
         Args:
-            variant (Optional[Literal[production, staging]]): Variant of
-                settings. By default, is used 'production'.
+            bundle_name (Optional[str]): Name of bundle for which should be
+                settings received.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
+            site_id (Optional[str]): Id of site for which want to receive
+                site overrides.
+            use_site (bool): To force disable option of using site overrides
+                set to 'False'. In that case won't be applied any site
+                overrides.
             only_values (Optional[bool]): Output will contain only settings
                 values without metadata about addons.
 
         Returns:
             dict[str, Any]: Settings of all addons on server.
         """
 
-        query_values = {}
-        if variant:
-            query_values["variant"] = variant
-        query = prepare_query_string(query_values)
-        response = self.get("settings/addons{}".format(query))
-        response.raise_for_status()
-        output = response.data
+        output = self.get_bundle_settings(
+            bundle_name=bundle_name,
+            variant=variant,
+            site_id=site_id,
+            use_site=use_site
+        )
         if only_values:
-            output = output["settings"]
+            major, minor, patch, _, _ = self.server_version_tuple
+            if major == 0 and minor >= 3:
+                output = {
+                    addon["name"]: addon["settings"]
+                    for addon in output["addons"]
+                }
+            else:
+                # Backward compatibility for AYON server < 0.3.0
+                output = output["settings"]
         return output
 
     def get_addons_project_settings(
         self,
         project_name,
+        bundle_name=None,
         variant=None,
         site_id=None,
         use_site=True,
         only_values=True
     ):
         """Project settings of all addons.
 
@@ -2601,83 +2713,112 @@
                 "addons": {...}
             }
 
         The output can be limited to only values. To do so is 'only_values'
         argument which is by default set to 'True'. In that case output
         contains only value of 'settings' key.
 
+        Warnings:
+            Behavior of this function changed with AYON server version 0.3.0.
+                Structure of output from server changed. If using
+                'only_values=True' then output should be same as before.
+
         Args:
             project_name (str): Name of project for which are settings
                 received.
-            variant (Optional[Literal[production, staging]]): Variant of
-                settings. By default, is used 'production'.
+            bundle_name (Optional[str]): Name of bundle for which should be
+                settings received.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
             site_id (Optional[str]): Id of site for which want to receive
                 site overrides.
             use_site (bool): To force disable option of using site overrides
                 set to 'False'. In that case won't be applied any site
                 overrides.
             only_values (Optional[bool]): Output will contain only settings
                 values without metadata about addons.
 
         Returns:
             dict[str, Any]: Settings of all addons on server for passed
                 project.
         """
 
-        query_values = {
-            "project": project_name
-        }
-        if variant:
-            query_values["variant"] = variant
+        if not project_name:
+            raise ValueError("Project name must be passed.")
 
-        if use_site:
-            if not site_id:
-                site_id = self.default_settings_variant
-            if site_id:
-                query_values["site"] = site_id
-        query = prepare_query_string(query_values)
-        response = self.get("settings/addons{}".format(query))
-        response.raise_for_status()
-        output = response.data
+        output = self.get_bundle_settings(
+            project_name=project_name,
+            bundle_name=bundle_name,
+            variant=variant,
+            site_id=site_id,
+            use_site=use_site
+        )
         if only_values:
-            output = output["settings"]
+            major, minor, patch, _, _ = self.server_version_tuple
+            if major == 0 and minor >= 3:
+                output = {
+                    addon["name"]: addon["settings"]
+                    for addon in output["addons"]
+                }
+            else:
+                # Backward compatibility for AYON server < 0.3.0
+                output = output["settings"]
         return output
 
     def get_addons_settings(
         self,
+        bundle_name=None,
         project_name=None,
         variant=None,
         site_id=None,
         use_site=True,
         only_values=True
     ):
         """Universal function to receive all addon settings.
 
         Based on 'project_name' will receive studio settings or project
         settings. In case project is not passed is 'site_id' ignored.
 
+        Warnings:
+            Behavior of this function changed with AYON server version 0.3.0.
+                Structure of output from server changed. If using
+                'only_values=True' then output should be same as before.
+
         Args:
+            bundle_name (Optional[str]): Name of bundle for which should be
+                settings received.
             project_name (Optional[str]): Name of project for which should be
                 settings received.
-            variant (Optional[Literal[production, staging]]): Settings variant.
-                By default, is used 'production'.
+            variant (Optional[Literal['production', 'staging']]): Name of
+                settings variant. Used 'default_settings_variant' by default.
             site_id (Optional[str]): Id of site for which want to receive
                 site overrides.
             use_site (Optional[bool]): To force disable option of using site
                 overrides set to 'False'. In that case won't be applied
                 any site overrides.
             only_values (Optional[bool]): Only settings values will be
                 returned. By default, is set to 'True'.
         """
 
         if project_name is None:
-            return self.get_addons_studio_settings(variant, only_values)
+            return self.get_addons_studio_settings(
+                bundle_name=bundle_name,
+                variant=variant,
+                site_id=site_id,
+                use_site=use_site,
+                only_values=only_values
+            )
 
         return self.get_addons_project_settings(
-            project_name, variant, site_id, use_site, only_values
+            project_name=project_name,
+            bundle_name=bundle_name,
+            variant=variant,
+            site_id=site_id,
+            use_site=use_site,
+            only_values=only_values
         )
 
     # Entity getters
     def get_rest_project(self, project_name):
         """Query project by name.
 
         This call returns project with anatomy data.
```

### Comparing `ayon-python-api-0.2.2/ayon_api/thumbnails.py` & `ayon-python-api-0.3.0/ayon_api/thumbnails.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_api/utils.py` & `ayon-python-api-0.3.0/ayon_api/utils.py`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/ayon_python_api.egg-info/SOURCES.txt` & `ayon-python-api-0.3.0/ayon_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayon-python-api-0.2.2/setup.py` & `ayon-python-api-0.3.0/setup.py`

 * *Files identical despite different names*

