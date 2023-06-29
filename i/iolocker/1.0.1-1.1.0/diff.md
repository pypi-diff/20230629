# Comparing `tmp/iolocker-1.0.1.tar.gz` & `tmp/iolocker-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iolocker-1.0.1.tar", last modified: Tue Jun 20 10:39:58 2023, max compression
+gzip compressed data, was "iolocker-1.1.0.tar", last modified: Thu Jun 29 11:59:50 2023, max compression
```

## Comparing `iolocker-1.0.1.tar` & `iolocker-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/
--rw-rw-rw-   0        0        0     1090 2023-06-16 15:15:34.000000 iolocker-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 iolocker-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1595 2023-06-20 10:39:58.027455 iolocker-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-06-19 17:02:14.000000 iolocker-1.0.1/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 iolocker-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0     1024 2023-06-20 10:39:58.043077 iolocker-1.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.011833 iolocker-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/src/iolocker/
--rw-rw-rw-   0        0        0      395 2023-06-19 09:49:23.000000 iolocker-1.0.1/src/iolocker/__init__.py
--rw-rw-rw-   0        0        0      877 2023-06-19 10:19:26.000000 iolocker-1.0.1/src/iolocker/constants.py
--rw-rw-rw-   0        0        0     3897 2023-06-19 10:19:26.000000 iolocker-1.0.1/src/iolocker/core.py
--rw-rw-rw-   0        0        0      816 2023-06-19 09:49:23.000000 iolocker-1.0.1/src/iolocker/exceptions.py
--rw-rw-rw-   0        0        0     2263 2023-06-20 09:28:55.000000 iolocker-1.0.1/src/iolocker/handlers.py
-drwxrwxrwx   0        0        0        0 2023-06-20 10:39:58.027455 iolocker-1.0.1/src/iolocker.egg-info/
--rw-rw-rw-   0        0        0     1595 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-06-20 10:39:58.000000 iolocker-1.0.1/src/iolocker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-19 17:22:43.000000 iolocker-1.0.1/src/iolocker.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       46 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-20 10:39:57.000000 iolocker-1.0.1/src/iolocker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 11:59:50.179891 iolocker-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-06-16 15:15:34.000000 iolocker-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 iolocker-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1914 2023-06-29 11:59:50.179891 iolocker-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1116 2023-06-29 11:51:01.000000 iolocker-1.1.0/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 iolocker-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1024 2023-06-29 11:59:50.180889 iolocker-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 11:59:50.163081 iolocker-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 11:59:50.174054 iolocker-1.1.0/src/iolocker/
+-rw-rw-rw-   0        0        0      483 2023-06-29 11:45:20.000000 iolocker-1.1.0/src/iolocker/__init__.py
+-rw-rw-rw-   0        0        0     1096 2023-06-29 11:45:20.000000 iolocker-1.1.0/src/iolocker/constants.py
+-rw-rw-rw-   0        0        0     3897 2023-06-19 10:19:26.000000 iolocker-1.1.0/src/iolocker/core.py
+-rw-rw-rw-   0        0        0      816 2023-06-19 09:49:23.000000 iolocker-1.1.0/src/iolocker/exceptions.py
+-rw-rw-rw-   0        0        0     5374 2023-06-29 11:45:20.000000 iolocker-1.1.0/src/iolocker/handlers.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:59:50.178894 iolocker-1.1.0/src/iolocker.egg-info/
+-rw-rw-rw-   0        0        0     1914 2023-06-29 11:59:50.000000 iolocker-1.1.0/src/iolocker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      392 2023-06-29 11:59:50.000000 iolocker-1.1.0/src/iolocker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:59:50.000000 iolocker-1.1.0/src/iolocker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-19 17:22:43.000000 iolocker-1.1.0/src/iolocker.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       46 2023-06-29 11:59:50.000000 iolocker-1.1.0/src/iolocker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 11:59:50.000000 iolocker-1.1.0/src/iolocker.egg-info/top_level.txt
```

### Comparing `iolocker-1.0.1/LICENSE` & `iolocker-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.1/PKG-INFO` & `iolocker-1.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: iolocker
-Version: 1.0.1
-Summary: Simple file locker.
-Home-page: https://github.com/ClaudiuDrug/iolocker
-Author: Claudiu DRUG
-Author-email: claudiu.drug@outlook.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/iolocker/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Utilities
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # iolocker
 
 Simple file locker.
 
 ---
 
 #### Installation:
@@ -32,14 +11,16 @@
 ```
 
 ---
 
 
 #### Usage:
 
+###### FileLocker:
+
 ```python
 # -*- coding: UTF-8 -*-
 
 from iolocker import FileLocker, LOCK
 
 if __name__ == '__main__':
 
@@ -60,7 +41,26 @@
 
 if __name__ == '__main__':
 
     with open("test_file.txt", "a", encoding="UTF-8") as fh:
         with FileLocker(fh, flags=LOCK.EX) as locked:
             locked.write("Testing file lockers...\n")
 ```
+
+
+###### FileHandler:
+
+```python
+# -*- coding: UTF-8 -*-
+
+from iolocker import FileHandler
+
+
+if __name__ == '__main__':
+
+    file_path: str = r"test_file.txt"
+
+    with FileHandler(file_path, "a", encoding="UTF-8") as fh:
+        fh.write("Testing file handlers...\n")
+```
+
+---
```

### Comparing `iolocker-1.0.1/setup.cfg` & `iolocker-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2069 6f6c 6f63 6b65 720d 0a76 6572   = iolocker..ver
-00000020: 7369 6f6e 203d 2031 2e30 2e31 0d0a 6175  sion = 1.0.1..au
+00000020: 7369 6f6e 203d 2031 2e31 2e30 0d0a 6175  sion = 1.1.0..au
 00000030: 7468 6f72 203d 2043 6c61 7564 6975 2044  thor = Claudiu D
 00000040: 5255 470d 0a61 7574 686f 725f 656d 6169  RUG..author_emai
 00000050: 6c20 3d20 636c 6175 6469 752e 6472 7567  l = claudiu.drug
 00000060: 406f 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69  @outlook.com..li
 00000070: 6365 6e73 6520 3d20 4d49 5420 4c69 6365  cense = MIT Lice
 00000080: 6e73 650d 0a64 6573 6372 6970 7469 6f6e  nse..description
 00000090: 203d 2053 696d 706c 6520 6669 6c65 206c   = Simple file l
```

### Comparing `iolocker-1.0.1/src/iolocker/core.py` & `iolocker-1.1.0/src/iolocker/core.py`

 * *Files identical despite different names*

### Comparing `iolocker-1.0.1/src/iolocker/exceptions.py` & `iolocker-1.1.0/src/iolocker/exceptions.py`

 * *Files identical despite different names*

