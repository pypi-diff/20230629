# Comparing `tmp/bootstrapping_tools-0.5.7.tar.gz` & `tmp/bootstrapping_tools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bootstrapping_tools-0.5.7.tar", last modified: Thu Feb  9 20:52:48 2023, max compression
+gzip compressed data, was "bootstrapping_tools-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bootstrapping_tools-0.5.7.tar` & `bootstrapping_tools-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      187 2023-02-09 20:52:38.675441 bootstrapping_tools-0.5.7/README.md
--rw-r--r--   0        0        0      137 2023-02-09 20:52:38.675441 bootstrapping_tools-0.5.7/bootstrapping_tools/__init__.py
--rw-r--r--   0        0        0    13765 2023-02-09 20:52:38.675441 bootstrapping_tools-0.5.7/bootstrapping_tools/bootstrapping.py
--rw-r--r--   0        0        0      871 2023-02-09 20:52:38.675441 bootstrapping_tools-0.5.7/bootstrapping_tools/resample_by_blocks.py
--rw-r--r--   0        0        0      516 2023-02-09 20:52:38.675441 bootstrapping_tools-0.5.7/pyproject.toml
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 bootstrapping_tools-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/README.md
+-rw-r--r--   0        0        0      137 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/__init__.py
+-rw-r--r--   0        0        0    10923 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/bootstrapping.py
+-rw-r--r--   0        0        0      871 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/bootstrapping_tools/resample_by_blocks.py
+-rw-r--r--   0        0        0      516 2023-06-29 21:10:35.964802 bootstrapping_tools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 bootstrapping_tools-1.0.0/PKG-INFO
```

### Comparing `bootstrapping_tools-0.5.7/bootstrapping_tools/resample_by_blocks.py` & `bootstrapping_tools-1.0.0/bootstrapping_tools/resample_by_blocks.py`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-0.5.7/pyproject.toml` & `bootstrapping_tools-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bootstrapping_tools-0.5.7/PKG-INFO` & `bootstrapping_tools-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bootstrapping_tools
-Version: 0.5.7
+Version: 1.0.0
 Summary: GECI Tools for bootstrapping
 Home-page: https://github.com/IslasGECI/bootstrapping_tools
 Author: Ciencia de Datos • GECI
 Author-email: ciencia.datos@islas.org.mx
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -14,9 +14,11 @@
 Requires-Dist: scipy
 Requires-Dist: tqdm
 
 <a href="https://www.islas.org.mx/"><img src="https://www.islas.org.mx/img/logo.svg" align="right" width="256" /></a>
 
 # Bootstrapping tools
 
-GECI tools to perform bootstrapping sampling
+GECI tools to perform bootstrapping sampling by blocks.
+
+
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: bootstrapping_tools Version: 0.5.7 Summary: GECI
+Metadata-Version: 2.1 Name: bootstrapping_tools Version: 1.0.0 Summary: GECI
 Tools for bootstrapping Home-page: https://github.com/IslasGECI/
 bootstrapping_tools Author: Ciencia de Datos â¢ GECI Author-email:
 ciencia.datos@islas.org.mx Requires-Python: >=3 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 or later (GPLv3+) Requires-Dist: numpy Requires-Dist: pandas-stubs Requires-
 Dist: pandas Requires-Dist: scipy Requires-Dist: tqdm [https://
 www.islas.org.mx/img/logo.svg] # Bootstrapping tools GECI tools to perform
-bootstrapping sampling
+bootstrapping sampling by blocks.
```

