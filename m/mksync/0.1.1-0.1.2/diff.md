# Comparing `tmp/mksync-0.1.1.tar.gz` & `tmp/mksync-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mksync-0.1.1.tar", max compression
+gzip compressed data, was "mksync-0.1.2.tar", max compression
```

## Comparing `mksync-0.1.1.tar` & `mksync-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      998 2023-06-29 20:35:59.711226 mksync-0.1.1/LICENSE
--rw-r--r--   0        0        0     1633 2023-06-29 21:24:12.457641 mksync-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      781 2023-06-29 21:24:12.469640 mksync-0.1.1/src/mksync/__init__.py
--rw-r--r--   0        0        0     1123 2023-06-29 20:56:11.733080 mksync-0.1.1/src/mksync/__main__.py
--rw-r--r--   0        0        0      427 2023-06-29 16:54:45.263854 mksync-0.1.1/src/mksync/context.py
--rw-r--r--   0        0        0        5 2023-06-29 16:54:45.263854 mksync-0.1.1/src/mksync/directives/__init__.py
--rw-r--r--   0        0        0      984 2023-06-29 16:54:45.263854 mksync-0.1.1/src/mksync/directives/generic.py
--rw-r--r--   0        0        0     2359 2023-06-29 21:06:59.134817 mksync-0.1.1/src/mksync/directives/include.py
--rw-r--r--   0        0        0     2705 2023-06-29 21:06:40.479346 mksync-0.1.1/src/mksync/directives/parser.py
--rw-r--r--   0        0        0     1931 2023-06-29 21:04:20.275312 mksync-0.1.1/src/mksync/directives/runcmd.py
--rw-r--r--   0        0        0     1946 2023-06-29 21:06:40.471346 mksync-0.1.1/src/mksync/directives/toc.py
--rw-r--r--   0        0        0        0 2023-06-29 20:35:59.711226 mksync-0.1.1/src/mksync/py.typed
--rw-r--r--   0        0        0      330 2023-06-29 16:54:45.263854 mksync-0.1.1/src/mksync/readfile.py
--rw-r--r--   0        0        0     1063 2023-06-29 16:54:45.263854 mksync-0.1.1/src/mksync/targets.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 mksync-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      998 2023-06-29 20:35:59.711226 mksync-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1724 2023-06-29 21:08:58.643433 mksync-0.1.2/README.md
+-rw-r--r--   0        0        0     1654 2023-06-29 21:24:39.296893 mksync-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      781 2023-06-29 21:24:39.308893 mksync-0.1.2/src/mksync/__init__.py
+-rw-r--r--   0        0        0     1123 2023-06-29 20:56:11.733080 mksync-0.1.2/src/mksync/__main__.py
+-rw-r--r--   0        0        0      427 2023-06-29 16:54:45.263854 mksync-0.1.2/src/mksync/context.py
+-rw-r--r--   0        0        0        5 2023-06-29 16:54:45.263854 mksync-0.1.2/src/mksync/directives/__init__.py
+-rw-r--r--   0        0        0      984 2023-06-29 16:54:45.263854 mksync-0.1.2/src/mksync/directives/generic.py
+-rw-r--r--   0        0        0     2359 2023-06-29 21:06:59.134817 mksync-0.1.2/src/mksync/directives/include.py
+-rw-r--r--   0        0        0     2705 2023-06-29 21:06:40.479346 mksync-0.1.2/src/mksync/directives/parser.py
+-rw-r--r--   0        0        0     1931 2023-06-29 21:04:20.275312 mksync-0.1.2/src/mksync/directives/runcmd.py
+-rw-r--r--   0        0        0     1946 2023-06-29 21:06:40.471346 mksync-0.1.2/src/mksync/directives/toc.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:35:59.711226 mksync-0.1.2/src/mksync/py.typed
+-rw-r--r--   0        0        0      330 2023-06-29 16:54:45.263854 mksync-0.1.2/src/mksync/readfile.py
+-rw-r--r--   0        0        0     1063 2023-06-29 16:54:45.263854 mksync-0.1.2/src/mksync/targets.py
+-rw-r--r--   0        0        0     2331 1970-01-01 00:00:00.000000 mksync-0.1.2/PKG-INFO
```

### Comparing `mksync-0.1.1/LICENSE` & `mksync-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/pyproject.toml` & `mksync-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mksync"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 packages = [{ include = "mksync", from = "src" }]
 classifiers = []
 keywords = []
+readme = "README.md"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/mksync/issues"
 # Documentation = ""
 # Homepage = ""
 Repository = "https://github.com/NiklasRosenstein/mksync"
```

### Comparing `mksync-0.1.1/src/mksync/__init__.py` & `mksync-0.1.2/src/mksync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from pathlib import Path
 
 from adjudicator import Params, RuleEngine
 
 from mksync.targets import PreprocessFileResult, PreprocessFileTarget
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __all__ = ["mksync_file"]
 logger = logging.getLogger(__name__)
 modules = [
     "mksync." + x
     for x in [
         "readfile",
         "targets",
```

### Comparing `mksync-0.1.1/src/mksync/__main__.py` & `mksync-0.1.2/src/mksync/__main__.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/directives/generic.py` & `mksync-0.1.2/src/mksync/directives/generic.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/directives/include.py` & `mksync-0.1.2/src/mksync/directives/include.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/directives/parser.py` & `mksync-0.1.2/src/mksync/directives/parser.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/directives/runcmd.py` & `mksync-0.1.2/src/mksync/directives/runcmd.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/directives/toc.py` & `mksync-0.1.2/src/mksync/directives/toc.py`

 * *Files identical despite different names*

### Comparing `mksync-0.1.1/src/mksync/targets.py` & `mksync-0.1.2/src/mksync/targets.py`

 * *Files identical despite different names*

