# Comparing `tmp/rubika-6.6.6.tar.gz` & `tmp/rubika-6.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubika-6.6.6.tar", last modified: Thu Jun 29 17:57:52 2023, max compression
+gzip compressed data, was "rubika-6.6.7.tar", last modified: Thu Jun 29 20:45:08 2023, max compression
```

## Comparing `rubika-6.6.6.tar` & `rubika-6.6.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/
--rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.6.6/LICENSE
--rw-rw----   0 root         (0)     9997     4192 2023-06-29 17:57:52.630000 rubika-6.6.6/PKG-INFO
--rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.6.6/README.md
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/rubika/
--rw-rw----   0 root         (0)     9997     5307 2023-06-29 17:52:20.000000 rubika-6.6.6/rubika/Types.py
--rw-rw----   0 root         (0)     9997      116 2023-06-19 10:36:07.000000 rubika-6.6.6/rubika/__init__.py
--rw-rw----   0 root         (0)     9997    42801 2023-06-29 17:49:59.000000 rubika-6.6.6/rubika/client.py
--rw-rw----   0 root         (0)     9997     6535 2023-06-29 17:50:36.000000 rubika-6.6.6/rubika/configs.py
--rw-rw----   0 root         (0)     9997     3771 2023-06-29 17:49:51.000000 rubika-6.6.6/rubika/encryption.py
--rw-rw----   0 root         (0)     9997      170 2023-06-13 09:40:35.000000 rubika-6.6.6/rubika/exceptions.py
--rw-rw----   0 root         (0)     9997     5458 2023-06-29 17:50:51.000000 rubika-6.6.6/rubika/fileIO.py
--rw-rw----   0 root         (0)     9997     5469 2023-06-09 08:44:46.000000 rubika-6.6.6/rubika/filters.py
--rw-rw----   0 root         (0)     9997     6444 2023-06-29 17:51:07.000000 rubika-6.6.6/rubika/rubino.py
--rw-rw----   0 root         (0)     9997     4580 2023-06-29 17:53:02.000000 rubika-6.6.6/rubika/setup.py
--rw-rw----   0 root         (0)     9997     6944 2023-06-29 17:52:00.000000 rubika-6.6.6/rubika/tools.py
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/rubika.egg-info/
--rw-rw----   0 root         (0)     9997     4192 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      410 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.6.6/rubika.egg-info/not-zip-safe
--rw-rw----   0 root         (0)     9997       82 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/requires.txt
--rw-rw----   0 root         (0)     9997        7 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/top_level.txt
--rw-rw----   0 root         (0)     9997       79 2023-06-29 17:57:52.640000 rubika-6.6.6/setup.cfg
--rw-rw----   0 root         (0)     9997     2484 2023-06-13 10:32:27.000000 rubika-6.6.6/setup.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:45:08.740000 rubika-6.6.7/
+-rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.6.7/LICENSE
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:45:08.740000 rubika-6.6.7/PKG-INFO
+-rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.6.7/README.md
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:45:08.730000 rubika-6.6.7/rubika/
+-rw-rw----   0 root         (0)     9997     5307 2023-06-29 17:52:20.000000 rubika-6.6.7/rubika/Types.py
+-rw-rw----   0 root         (0)     9997      116 2023-06-19 10:36:07.000000 rubika-6.6.7/rubika/__init__.py
+-rw-rw----   0 root         (0)     9997    42801 2023-06-29 17:49:59.000000 rubika-6.6.7/rubika/client.py
+-rw-rw----   0 root         (0)     9997     6535 2023-06-29 17:50:36.000000 rubika-6.6.7/rubika/configs.py
+-rw-rw----   0 root         (0)     9997     3771 2023-06-29 17:49:51.000000 rubika-6.6.7/rubika/encryption.py
+-rw-rw----   0 root         (0)     9997      170 2023-06-13 09:40:35.000000 rubika-6.6.7/rubika/exceptions.py
+-rw-rw----   0 root         (0)     9997     5458 2023-06-29 17:50:51.000000 rubika-6.6.7/rubika/fileIO.py
+-rw-rw----   0 root         (0)     9997     5469 2023-06-09 08:44:46.000000 rubika-6.6.7/rubika/filters.py
+-rw-rw----   0 root         (0)     9997     6444 2023-06-29 17:51:07.000000 rubika-6.6.7/rubika/rubino.py
+-rw-rw----   0 root         (0)     9997     4580 2023-06-29 17:53:02.000000 rubika-6.6.7/rubika/setup.py
+-rw-rw----   0 root         (0)     9997     6944 2023-06-29 17:52:00.000000 rubika-6.6.7/rubika/tools.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:45:08.740000 rubika-6.6.7/rubika.egg-info/
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:45:08.000000 rubika-6.6.7/rubika.egg-info/PKG-INFO
+-rw-rw----   0 root         (0)     9997      410 2023-06-29 20:45:08.000000 rubika-6.6.7/rubika.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0)     9997        1 2023-06-29 20:45:08.000000 rubika-6.6.7/rubika.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.6.7/rubika.egg-info/not-zip-safe
+-rw-rw----   0 root         (0)     9997       82 2023-06-29 20:45:08.000000 rubika-6.6.7/rubika.egg-info/requires.txt
+-rw-rw----   0 root         (0)     9997        7 2023-06-29 20:45:08.000000 rubika-6.6.7/rubika.egg-info/top_level.txt
+-rw-rw----   0 root         (0)     9997       79 2023-06-29 20:45:08.740000 rubika-6.6.7/setup.cfg
+-rw-rw----   0 root         (0)     9997     2501 2023-06-29 20:44:55.000000 rubika-6.6.7/setup.py
```

### Comparing `rubika-6.6.6/LICENSE` & `rubika-6.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/PKG-INFO` & `rubika-6.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.6.6
+Version: 6.6.7
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
```

### Comparing `rubika-6.6.6/README.md` & `rubika-6.6.7/README.md`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/Types.py` & `rubika-6.6.7/rubika/Types.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/client.py` & `rubika-6.6.7/rubika/client.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/configs.py` & `rubika-6.6.7/rubika/configs.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/encryption.py` & `rubika-6.6.7/rubika/encryption.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/fileIO.py` & `rubika-6.6.7/rubika/fileIO.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/filters.py` & `rubika-6.6.7/rubika/filters.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/rubino.py` & `rubika-6.6.7/rubika/rubino.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/setup.py` & `rubika-6.6.7/rubika/setup.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika/tools.py` & `rubika-6.6.7/rubika/tools.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.6/rubika.egg-info/PKG-INFO` & `rubika-6.6.7/rubika.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.6.6
+Version: 6.6.7
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
```

### Comparing `rubika-6.6.6/setup.py` & `rubika-6.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import re
 from sys import argv
 from requests import get
 from setuptools import setup, find_packages
 
-requires = ["requests", "pycryptodome==3.10.1", "urllib3", "tqdm", "aiohttp", "rich", "websocket-client", "schedule"]
-version = "6.6.6"
-readme = get("https://raw.githubusercontent.com/Bahman-Ahmadi/rubika/main/README.md").text
+requires = ["requests", "pycryptodome==3.10.1", "urllib3",
+            "tqdm", "aiohttp", "rich", "websocket-client", "schedule"]
+version = "6.6.7"
+readme = get(
+    "https://raw.githubusercontent.com/Bahman-Ahmadi/rubika/main/README.md").text
 
 setup(
     name="rubika",
     version=version,
     description="this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that",
     long_description=readme,
     long_description_content_type="text/markdown",
```

