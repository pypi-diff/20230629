# Comparing `tmp/pynegex-0.0.2.dev0.tar.gz` & `tmp/pynegex-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynegex-0.0.2.dev0.tar", last modified: Thu Jun 29 11:52:24 2023, max compression
+gzip compressed data, was "pynegex-0.0.3.dev0.tar", last modified: Thu Jun 29 13:02:58 2023, max compression
```

## Comparing `pynegex-0.0.2.dev0.tar` & `pynegex-0.0.3.dev0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/src/pynegex/
--rwxr-xr-x   0 runner    (1001) docker     (123)      295 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/src/pynegex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/src/pynegex/model/
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/src/pynegex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/src/pynegex/model/negex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-06-29 11:52:12.000000 pynegex-0.0.2.dev0/src/pynegex/model/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:52:24.470400 pynegex-0.0.2.dev0/src/pynegex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-29 11:52:24.000000 pynegex-0.0.2.dev0/src/pynegex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 11:52:24.000000 pynegex-0.0.2.dev0/src/pynegex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:52:24.000000 pynegex-0.0.2.dev0/src/pynegex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 11:52:24.000000 pynegex-0.0.2.dev0/src/pynegex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:02:58.357818 pynegex-0.0.3.dev0/pynegex/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      306 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/pynegex/model/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/model/negex.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1015 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/model/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/pynegex/model/triggersets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/model/triggersets/chapman-en.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14865 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/pynegex/model/triggersets/cotik-de.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/pynegex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-29 13:02:58.000000 pynegex-0.0.3.dev0/pynegex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-29 13:02:58.000000 pynegex-0.0.3.dev0/pynegex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:02:58.000000 pynegex-0.0.3.dev0/pynegex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 13:02:58.000000 pynegex-0.0.3.dev0/pynegex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:02:58.361818 pynegex-0.0.3.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-29 13:02:44.000000 pynegex-0.0.3.dev0/setup.py
```

### Comparing `pynegex-0.0.2.dev0/LICENSE` & `pynegex-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynegex-0.0.2.dev0/PKG-INFO` & `pynegex-0.0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynegex
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Pypi package for negex with multilingual support
 Author: Moe Bin Sumait
 Author-email: mh.binsumait@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pynegex-0.0.2.dev0/README.md` & `pynegex-0.0.3.dev0/README.md`

 * *Files identical despite different names*

### Comparing `pynegex-0.0.2.dev0/setup.py` & `pynegex-0.0.3.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 #!/usr/bin/env python
 # from distutils.core import setup
 import os
 from setuptools import Extension, find_packages, setup
 from pathlib import Path
-cwd = Path(__file__).parent
 
+cwd = Path(__file__).parent
 long_description = (cwd / "README.md").read_text()
 
-# cwd = os.path.dirname(os.path.abspath(__file__))
-# with open(os.path.join(cwd, "src/pynegex", "VERSION")) as fin:
-#     version = fin.read().strip()
+version = "0.0.3-dev"
+
 setup(
     name='pynegex',
-    version="0.0.2-dev",
+    version=version,
     author="Moe Bin Sumait",
     author_email="mh.binsumait@gmail.com",
     description="Pypi package for negex with multilingual support",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Find packages under the 'src' directory
-    packages=find_packages(where='src'),
-    package_dir={'': 'src'},              # Root directory for the packages
+    packages=find_packages(),
+    # Root directory for the packages
+    package_dir={'pynegex': 'pynegex'},
+    package_data={'pynegex': [
+        "model/triggersets/*.txt"
+    ]},
     py_modules=["pynegex"],                # Name of the python package
     # List any dependencies required by your package)
     python_requires='>=3.6',                # Minimum version requirement of the package
     install_requires=[],
     classifiers=[
         "Programming Language :: Python",
         "Operating System :: OS Independent",
```

### Comparing `pynegex-0.0.2.dev0/src/pynegex/model/negex.py` & `pynegex-0.0.3.dev0/pynegex/model/negex.py`

 * *Files identical despite different names*

### Comparing `pynegex-0.0.2.dev0/src/pynegex/model/runners.py` & `pynegex-0.0.3.dev0/pynegex/model/runners.py`

 * *Files identical despite different names*

### Comparing `pynegex-0.0.2.dev0/src/pynegex.egg-info/PKG-INFO` & `pynegex-0.0.3.dev0/pynegex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynegex
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Pypi package for negex with multilingual support
 Author: Moe Bin Sumait
 Author-email: mh.binsumait@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

