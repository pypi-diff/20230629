# Comparing `tmp/prefai-0.0.4.tar.gz` & `tmp/prefai-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefai-0.0.4.tar", last modified: Sat Jun 10 06:00:28 2023, max compression
+gzip compressed data, was "prefai-0.0.5.tar", last modified: Thu Jun 29 16:54:18 2023, max compression
```

## Comparing `prefai-0.0.4.tar` & `prefai-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.962169 prefai-0.0.4/
--rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.4/LICENSE.txt
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-10 06:00:28.962021 prefai-0.0.4/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.4/README.md
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.960837 prefai-0.0.4/prefai/
--rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.4/prefai/__init__.py
--rw-r--r--   0 bjaros     (501) staff       (20)     5863 2023-06-10 05:52:41.000000 prefai-0.0.4/prefai/client.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.961549 prefai-0.0.4/prefai.egg-info/
--rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/PKG-INFO
--rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/SOURCES.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/dependency_links.txt
--rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-10 06:00:28.000000 prefai-0.0.4/prefai.egg-info/top_level.txt
--rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-10 06:00:28.962214 prefai-0.0.4/setup.cfg
--rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-10 05:13:24.000000 prefai-0.0.4/setup.py
-drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-10 06:00:28.961662 prefai-0.0.4/tests/
--rw-r--r--   0 bjaros     (501) staff       (20)     3665 2023-06-09 23:46:47.000000 prefai-0.0.4/tests/test_client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-29 16:54:18.763543 prefai-0.0.5/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1079 2023-06-01 06:14:59.000000 prefai-0.0.5/LICENSE.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-29 16:54:18.763357 prefai-0.0.5/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)     1238 2023-06-03 22:24:22.000000 prefai-0.0.5/README.md
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-29 16:54:18.761674 prefai-0.0.5/prefai/
+-rw-r--r--   0 bjaros     (501) staff       (20)       46 2023-05-31 03:58:40.000000 prefai-0.0.5/prefai/__init__.py
+-rw-r--r--   0 bjaros     (501) staff       (20)     5866 2023-06-29 16:26:26.000000 prefai-0.0.5/prefai/client.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-29 16:54:18.762717 prefai-0.0.5/prefai.egg-info/
+-rw-r--r--   0 bjaros     (501) staff       (20)     1682 2023-06-29 16:54:18.000000 prefai-0.0.5/prefai.egg-info/PKG-INFO
+-rw-r--r--   0 bjaros     (501) staff       (20)      207 2023-06-29 16:54:18.000000 prefai-0.0.5/prefai.egg-info/SOURCES.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        1 2023-06-29 16:54:18.000000 prefai-0.0.5/prefai.egg-info/dependency_links.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)        7 2023-06-29 16:54:18.000000 prefai-0.0.5/prefai.egg-info/top_level.txt
+-rw-r--r--   0 bjaros     (501) staff       (20)       38 2023-06-29 16:54:18.763587 prefai-0.0.5/setup.cfg
+-rw-r--r--   0 bjaros     (501) staff       (20)      710 2023-06-29 16:53:42.000000 prefai-0.0.5/setup.py
+drwxr-xr-x   0 bjaros     (501) staff       (20)        0 2023-06-29 16:54:18.762873 prefai-0.0.5/tests/
+-rw-r--r--   0 bjaros     (501) staff       (20)     3665 2023-06-09 23:46:47.000000 prefai-0.0.5/tests/test_client.py
```

### Comparing `prefai-0.0.4/LICENSE.txt` & `prefai-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prefai-0.0.4/PKG-INFO` & `prefai-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.4/README.md` & `prefai-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `prefai-0.0.4/prefai/client.py` & `prefai-0.0.5/prefai/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                     "user_action": user_action,
                     "context": context,
                     "interaction_title": interaction_title,
                     "observation": observation,
                     "create_observation": create_observation,
                 },
                 headers=headers,
-                timeout=5
+                timeout=10
             )
 
             response.raise_for_status()
             json_response = response.json()
 
             return json_response
             # return {
@@ -115,15 +115,15 @@
                     "user_action": user_action,
                     "user_email": user_email,
                     "user_id": user_id,
                     "max_results": max_results,
                     "min_similarity": min_similarity,
                 },
                 headers=headers,
-                timeout=5
+                timeout=10
             )
 
             response.raise_for_status()
             json_response = response.json()
 
             return json_response
 
@@ -160,15 +160,15 @@
                     "user_action": user_action,
                     "user_email": user_email,
                     "user_id": user_id,
                     "max_tokens": max_tokens,
                     "min_similarity": min_similarity,
                 },
                 headers=headers,
-                timeout=5
+                timeout=10
             )
 
             response.raise_for_status()
             json_response = response.json()
 
             return json_response
```

### Comparing `prefai-0.0.4/prefai.egg-info/PKG-INFO` & `prefai-0.0.5/prefai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefai
-Version: 0.0.4
+Version: 0.0.5
 Summary: A brief description of your package
 Home-page: http://github.com/prefai/pythonclient
 Author: Bobby Jaros
 Author-email: bobby@pref.ai
 License: LICENSE.txt
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `prefai-0.0.4/setup.py` & `prefai-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="prefai",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     author="Bobby Jaros",
     author_email="bobby@pref.ai",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="http://github.com/prefai/pythonclient",
```

### Comparing `prefai-0.0.4/tests/test_client.py` & `prefai-0.0.5/tests/test_client.py`

 * *Files identical despite different names*

