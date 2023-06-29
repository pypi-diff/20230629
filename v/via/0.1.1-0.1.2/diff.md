# Comparing `tmp/via-0.1.1.tar.gz` & `tmp/via-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-0.1.1.tar", last modified: Wed Jun 14 12:01:01 2023, max compression
+gzip compressed data, was "via-0.1.2.tar", last modified: Thu Jun 29 13:01:22 2023, max compression
```

## Comparing `via-0.1.1.tar` & `via-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-14 12:00:48.000000 via-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:01:01.897400 via-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-14 12:00:48.000000 via-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 12:01:01.897400 via-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-14 12:00:48.000000 via-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/via/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-14 12:00:48.000000 via-0.1.1/via/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-14 12:00:48.000000 via-0.1.1/via/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-14 12:00:48.000000 via-0.1.1/via/license.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-14 12:00:48.000000 via-0.1.1/via/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:01:01.897400 via-0.1.1/via.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-14 12:01:01.000000 via-0.1.1/via.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:01:22.666460 via-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-29 13:01:07.000000 via-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-29 13:01:22.666460 via-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-29 13:01:07.000000 via-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-29 13:01:07.000000 via-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:01:22.666460 via-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:01:22.666460 via-0.1.2/via/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-29 13:01:07.000000 via-0.1.2/via/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-29 13:01:07.000000 via-0.1.2/via/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-29 13:01:07.000000 via-0.1.2/via/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-29 13:01:07.000000 via-0.1.2/via/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:01:22.666460 via-0.1.2/via.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 13:01:22.000000 via-0.1.2/via.egg-info/top_level.txt
```

### Comparing `via-0.1.1/LICENSE` & `via-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `via-0.1.1/PKG-INFO` & `via-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: via
-Version: 0.1.1
-Summary: initialize your repos
-Home-page: https://github.com/kemingy/via
-Author: Keming Yang
-Author-email: kemingy94@gmail.com
+Version: 0.1.2
+Summary: initialize your repository
+Author-email: Keming <kemingy94@gmail.com>
+Project-URL: Homepage, https://github.com/kemingy/via
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Via: a command line tool to initialize your repos
 
 Initialize your repository.
```

### Comparing `via-0.1.1/README.md` & `via-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `via-0.1.1/via/__init__.py` & `via-0.1.2/via/__init__.py`

 * *Files identical despite different names*

### Comparing `via-0.1.1/via/ignore.py` & `via-0.1.2/via/ignore.py`

 * *Files identical despite different names*

### Comparing `via-0.1.1/via/license.py` & `via-0.1.2/via/license.py`

 * *Files identical despite different names*

### Comparing `via-0.1.1/via.egg-info/PKG-INFO` & `via-0.1.2/via.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: via
-Version: 0.1.1
-Summary: initialize your repos
-Home-page: https://github.com/kemingy/via
-Author: Keming Yang
-Author-email: kemingy94@gmail.com
+Version: 0.1.2
+Summary: initialize your repository
+Author-email: Keming <kemingy94@gmail.com>
+Project-URL: Homepage, https://github.com/kemingy/via
+Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Via: a command line tool to initialize your repos
 
 Initialize your repository.
```

