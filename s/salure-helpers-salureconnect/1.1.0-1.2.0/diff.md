# Comparing `tmp/salure_helpers_salureconnect-1.1.0.tar.gz` & `tmp/salure_helpers_salureconnect-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_salureconnect-1.1.0.tar", last modified: Tue Jan 24 16:22:01 2023, max compression
+gzip compressed data, was "dist/salure_helpers_salureconnect-1.2.0.tar", last modified: Thu Jun 29 12:20:56 2023, max compression
```

## Comparing `salure_helpers_salureconnect-1.1.0.tar` & `salure_helpers_salureconnect-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      283 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-01-24 16:21:47.000000 salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2579 2023-01-24 16:21:47.000000 salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/files.py
--rw-rw-rw-   0 root         (0) root         (0)     3639 2023-01-24 16:21:47.000000 salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/salureconnect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/
--rw-r--r--   0 root         (0) root         (0)      283 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      443 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       33 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/salure_helpers_salureconnect.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-24 16:22:01.000000 salure_helpers_salureconnect-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      466 2023-01-24 16:21:47.000000 salure_helpers_salureconnect-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-29 12:20:40.000000 salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2579 2023-06-29 12:20:40.000000 salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/files.py
+-rw-rw-rw-   0 root         (0) root         (0)     4491 2023-06-29 12:20:40.000000 salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/salureconnect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      283 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      443 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/salure_helpers_salureconnect.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 12:20:56.000000 salure_helpers_salureconnect-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-06-29 12:20:40.000000 salure_helpers_salureconnect-1.2.0/setup.py
```

### Comparing `salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/files.py` & `salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/files.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_salureconnect-1.1.0/salure_helpers/salureconnect/salureconnect.py` & `salure_helpers_salureconnect-1.2.0/salure_helpers/salureconnect/salureconnect.py`

 * *Files 23% similar despite different names*

```diff
@@ -66,7 +66,24 @@
         :return json response from salureconnect
         """
         response = requests.post(url=f'{self.url}connector/{system}/{system_id}/refresh', headers=self.__get_headers())
         response.raise_for_status()
         credentials = response.json()
 
         return credentials
+
+    def get_mappings(self, task_id: int) -> dict:
+        """
+        Get the mappings from the task in salureconnect
+        :param task_id: The id of the task in salureconnect. this does not have to be the task id of the current task
+        :return: A dictionary with the following structure: {mapping_title: {tuple(input): output}}
+        """
+        response = requests.get(url=f'{self.url}connectors/{task_id}/data-mapping', headers=self.__get_headers())
+
+        data = response.json()
+
+        # transform the data to a dictionary where the key is the title of the mapping and the value is the mapping as a dict
+        mappings = {
+            item['title']: {tuple(mapping['input']) if len(mapping['input']) > 1 else mapping['input'][0]: mapping['output'] for mapping in item['mapping']} for item in data
+        }
+
+        return mappings
```

