# Comparing `tmp/matplotlib-tufte-1.0.tar.gz` & `tmp/matplotlib_tufte-1.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib-tufte-1.0.tar", max compression
+gzip compressed data, was "matplotlib_tufte-1.1.dev0.tar", max compression
```

## Comparing `matplotlib-tufte-1.0.tar` & `matplotlib_tufte-1.1.dev0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0      573 2022-04-07 07:45:48.096988 matplotlib-tufte-1.0/CHANGELOG.md
-drwxr-xr-x   0        0        0        0 2022-04-08 10:06:04.432342 matplotlib-tufte-1.0/LICENSES/
--rw-r--r--   0        0        0    11358 2022-04-07 07:39:25.866988 matplotlib-tufte-1.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0     1055 2022-04-28 10:43:47.433996 matplotlib-tufte-1.0/README.md
--rw-r--r--   0        0        0     1213 2022-04-28 12:37:03.799280 matplotlib-tufte-1.0/pyproject.toml
--rw-r--r--   0        0        0     4942 2022-04-28 12:35:28.109280 matplotlib-tufte-1.0/tuftelike/__init__.py
--rw-r--r--   0        0        0     1765 2022-04-28 12:37:18.607878 matplotlib-tufte-1.0/setup.py
--rw-r--r--   0        0        0     1940 2022-04-28 12:37:18.608113 matplotlib-tufte-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1781 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/CHANGELOG.md
+-rw-r--r--   0        0        0    11358 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSE
+drwxr-xr-x   0        0        0        0 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/LICENSES/
+-rw-r--r--   0        0        0     1250 2023-06-29 19:28:35.197576 matplotlib_tufte-1.1.dev0/README.md
+-rw-r--r--   0        0        0     1218 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/pyproject.toml
+-rw-r--r--   0        0        0     7088 2023-06-29 19:28:35.199576 matplotlib_tufte-1.1.dev0/tuftelike/__init__.py
+-rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 matplotlib_tufte-1.1.dev0/PKG-INFO
```

### Comparing `matplotlib-tufte-1.0/LICENSES/Apache-2.0.txt` & `matplotlib_tufte-1.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib-tufte-1.0/pyproject.toml` & `matplotlib_tufte-1.1.dev0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # SPDX-FileCopyrightText: 2022 Thomas Lemberger <https://thomaslemberger.com>
 #
 # SPDX-License-Identifier: Apache-2.0
 
 [tool.poetry]
 name = "matplotlib-tufte"
-version = "1.0"
+version = "1.1.dev0"
 description = "Tufte-style plots for matplotlib"
 readme = "README.md"
 authors = ["Thomas Lemberger <lembergerth@gmail.com>"]
 repository = "https://gitlab.com/lemberger/matplotlib-tufte"
 keywords = ["plotting", "matplotlib"]
 classifiers = [
   "Framework :: Matplotlib",
```

### Comparing `matplotlib-tufte-1.0/PKG-INFO` & `matplotlib_tufte-1.1.dev0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: matplotlib-tufte
-Version: 1.0
+Version: 1.1.dev0
 Summary: Tufte-style plots for matplotlib
 Home-page: https://gitlab.com/lemberger/matplotlib-tufte
 License: Apache-2.0
 Keywords: plotting,matplotlib
 Author: Thomas Lemberger
 Author-email: lembergerth@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Matplotlib
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: matplotlib (>=3,<4)
 Project-URL: Repository, https://gitlab.com/lemberger/matplotlib-tufte
 Description-Content-Type: text/markdown
 
 <!--
 This file is part of matplotlib-tufte, Tufte-style plots for matplotlib.
 https://gitlab.com/lemberger/matplotlib-tufte
@@ -30,24 +31,27 @@
 SPDX-License-Identifier: Apache-2.0
 -->
 # matplotlib-tufte
 
 matplotlib-tufte is a python module
 to create Tufte-like plots with matplotlib.
 
-Inspiration is drawn from *Edward Tufte: The Visual Display of Quantitative Data*.
+Inspiration is drawn from [*Edward Tufte: The Visual Display of Quantitative Information*][TufteBook].
+
+[TufteBook]: https://www.edwardtufte.com/tufte/books_vdqi
 
 ## Requirements
 
 - python >= 3.7
 - matplotlib
 
 ## Examples
 
-See [examples/Basic.ipynb](examples/Basic.ipynb) for some small examples of tuftelike plots.
+See [examples/Basic.ipynb](https://gitlab.com/lemberger/matplotlib-tufte/-/blob/main/examples/Basic.ipynb)
+for some small examples of tuftelike plots.
 
 ## Usage
 
 Create your plots with matplotlib as usual.
 Then, run `tuftelike.adjust` with the x- and y-values of your plot to adjust it in-place.
 
 ```
@@ -60,8 +64,9 @@
 tuftelike.adjust(xs, ys)
 plt.savefig("example.png")
 ```
 
 Tuftelike needs the x- and y-values because matplotlib does not store these internally.
 The above code produces:
 
-![an example tuftelike plot](examples/simple.png).
+![an example tuftelike plot](https://gitlab.com/lemberger/matplotlib-tufte/-/raw/main/examples/simple.png).
+
```

