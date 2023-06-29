# Comparing `tmp/tlv-1.3.7.tar.gz` & `tmp/tlv-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlv-1.3.7.tar", last modified: Tue Apr 11 10:44:24 2023, max compression
+gzip compressed data, was "tlv-1.4.0.tar", last modified: Thu Jun 29 12:08:11 2023, max compression
```

## Comparing `tlv-1.3.7.tar` & `tlv-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:44:24.392349 tlv-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 10:44:04.000000 tlv-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 10:44:04.000000 tlv-1.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-11 10:44:24.392349 tlv-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-04-11 10:44:04.000000 tlv-1.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-11 10:44:04.000000 tlv-1.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-11 10:44:24.392349 tlv-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-11 10:44:24.000000 tlv-1.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:44:24.392349 tlv-1.3.7/tlv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/cls_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/src_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-11 10:44:04.000000 tlv-1.3.7/tlv/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:44:24.392349 tlv-1.3.7/tlv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 10:44:24.000000 tlv-1.3.7/tlv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:08:11.591482 tlv-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-29 12:07:55.000000 tlv-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 12:07:55.000000 tlv-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-29 12:08:11.591482 tlv-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-06-29 12:07:55.000000 tlv-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 12:07:55.000000 tlv-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-29 12:08:11.595482 tlv-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 12:08:11.000000 tlv-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:08:11.591482 tlv-1.4.0/tlv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/cls_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/src_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-06-29 12:07:55.000000 tlv-1.4.0/tlv/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:08:11.591482 tlv-1.4.0/tlv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11688 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 12:08:11.000000 tlv-1.4.0/tlv.egg-info/top_level.txt
```

### Comparing `tlv-1.3.7/LICENSE` & `tlv-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/PKG-INFO` & `tlv-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.3.7
+Version: 1.4.0
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
```

### Comparing `tlv-1.3.7/README.md` & `tlv-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/setup.py` & `tlv-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 requirements = []
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="tlv",
-    version="1.3.7",
+    version="1.4.0",
     author="Konrad Weihmann",
     author_email="kweihmann@outlook.com",
     description="-- Too less variation -- Find duplicates in source code for various languages",
     long_description=_long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/priv-kweihmann/tlv",
     packages=setuptools.find_packages(),
@@ -27,15 +27,14 @@
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         "Programming Language :: Python :: 3",
         "Topic :: Software Development :: Quality Assurance",
     ],
```

### Comparing `tlv-1.3.7/tlv/arg_parser.py` & `tlv-1.4.0/tlv/arg_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/tlv/cls_ast.py` & `tlv-1.4.0/tlv/cls_ast.py`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/tlv/lexer.py` & `tlv-1.4.0/tlv/lexer.py`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/tlv/src_parser.py` & `tlv-1.4.0/tlv/src_parser.py`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/tlv/tokens.py` & `tlv-1.4.0/tlv/tokens.py`

 * *Files identical despite different names*

### Comparing `tlv-1.3.7/tlv.egg-info/PKG-INFO` & `tlv-1.4.0/tlv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: tlv
-Version: 1.3.7
+Version: 1.4.0
 Summary: -- Too less variation -- Find duplicates in source code for various languages
 Home-page: https://github.com/priv-kweihmann/tlv
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Python: >=3.7
```

