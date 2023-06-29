# Comparing `tmp/matplotlib_tufte-1.1.tar.gz` & `tmp/matplotlib_tufte-1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_tufte-1.1.tar", max compression
+gzip compressed data, was "matplotlib_tufte-1.1.dev0.tar", max compression
```

## Comparing `matplotlib_tufte-1.1.tar` & `matplotlib_tufte-1.1.dev0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1781 2023-06-29 19:33:34.395557 matplotlib_tufte-1.1/CHANGELOG.md
--rw-r--r--   0        0        0    11358 2023-06-29 19:33:34.396558 matplotlib_tufte-1.1/LICENSE
-drwxr-xr-x   0        0        0        0 2023-06-29 19:33:34.396558 matplotlib_tufte-1.1/LICENSES/
--rw-r--r--   0        0        0     1250 2023-06-29 19:33:34.396558 matplotlib_tufte-1.1/README.md
--rw-r--r--   0        0        0     1213 2023-06-29 19:33:34.398558 matplotlib_tufte-1.1/pyproject.toml
--rw-r--r--   0        0        0     7083 2023-06-29 19:33:34.398558 matplotlib_tufte-1.1/tuftelike/__init__.py
--rw-r--r--   0        0        0     2186 1970-01-01 00:00:00.000000 matplotlib_tufte-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1781 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSES/
+-rw-r--r--   0        0        0     1250 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/README.md
+-rw-r--r--   0        0        0     1218 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7088 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/tuftelike/__init__.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 matplotlib_tufte-1.1.dev0/PKG-INFO
```

### Comparing `matplotlib_tufte-1.1/CHANGELOG.md` & `matplotlib_tufte-1.1.dev0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `matplotlib_tufte-1.1/LICENSE` & `matplotlib_tufte-1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_tufte-1.1/README.md` & `matplotlib_tufte-1.1.dev0/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_tufte-1.1/pyproject.toml` & `matplotlib_tufte-1.1.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-FileCopyrightText: 2022 Thomas Lemberger <https://thomaslemberger.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "matplotlib-tufte"
-version = "1.1"
+version = "1.1.dev0"
 description = "Tufte-style plots for matplotlib"
 readme = "README.md"
 authors = ["Thomas Lemberger <lembergerth@gmail.com>"]
 repository = "https://gitlab.com/lemberger/matplotlib-tufte"
 keywords = ["plotting", "matplotlib"]
 classifiers = [
   "Framework :: Matplotlib",
```

### Comparing `matplotlib_tufte-1.1/tuftelike/__init__.py` & `matplotlib_tufte-1.1.dev0/tuftelike/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 import logging
 import math
 import matplotlib.pyplot as plt  # type: ignore
 from matplotlib.ticker import FixedFormatter, FixedLocator, NullLocator  # type: ignore
 
-__version__ = "1.1"
+__version__ = "1.1.dev0"
 
 logger = logging.getLogger(__name__)
 
 
 def _pad_xlabel(ax):
     label = ax.get_xlabel()
     if not label:
```

### Comparing `matplotlib_tufte-1.1/PKG-INFO` & `matplotlib_tufte-1.1.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-tufte
-Version: 1.1
+Version: 1.1.dev0
 Summary: Tufte-style plots for matplotlib
 Home-page: https://gitlab.com/lemberger/matplotlib-tufte
 License: Apache-2.0
 Keywords: plotting,matplotlib
 Author: Thomas Lemberger
 Author-email: lembergerth@gmail.com
 Requires-Python: >=3.7,<4.0
```

