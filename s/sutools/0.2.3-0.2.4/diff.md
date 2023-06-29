# Comparing `tmp/sutools-0.2.3.tar.gz` & `tmp/sutools-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sutools-0.2.3.tar", last modified: Sun Jun 18 23:27:48 2023, max compression
+gzip compressed data, was "sutools-0.2.4.tar", last modified: Thu Jun 29 17:09:49 2023, max compression
```

## Comparing `sutools-0.2.3.tar` & `sutools-0.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-18 23:27:27.000000 sutools-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-18 23:27:48.512372 sutools-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-18 23:27:27.000000 sutools-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-18 23:27:27.000000 sutools-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 23:27:48.512372 sutools-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-18 23:27:27.000000 sutools-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/sutools/
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/bench_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-18 23:27:27.000000 sutools-0.2.3/sutools/meta_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/sutools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-18 23:27:48.000000 sutools-0.2.3/sutools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:27:48.512372 sutools-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_bench_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_cli_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_meta_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-18 23:27:27.000000 sutools-0.2.3/tests/test_sutools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:09:49.673044 sutools-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 17:09:30.000000 sutools-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-29 17:09:49.673044 sutools-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-29 17:09:30.000000 sutools-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 17:09:30.000000 sutools-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:09:49.673044 sutools-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-29 17:09:30.000000 sutools-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:09:49.669044 sutools-0.2.4/sutools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-29 17:09:30.000000 sutools-0.2.4/sutools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-29 17:09:30.000000 sutools-0.2.4/sutools/bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-06-29 17:09:30.000000 sutools-0.2.4/sutools/cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-29 17:09:30.000000 sutools-0.2.4/sutools/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-06-29 17:09:30.000000 sutools-0.2.4/sutools/meta_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:09:49.669044 sutools-0.2.4/sutools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-06-29 17:09:49.000000 sutools-0.2.4/sutools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-29 17:09:49.000000 sutools-0.2.4/sutools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:09:49.000000 sutools-0.2.4/sutools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 17:09:49.000000 sutools-0.2.4/sutools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:09:49.669044 sutools-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-29 17:09:30.000000 sutools-0.2.4/tests/test_bench_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-06-29 17:09:30.000000 sutools-0.2.4/tests/test_cli_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18499 2023-06-29 17:09:30.000000 sutools-0.2.4/tests/test_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-29 17:09:30.000000 sutools-0.2.4/tests/test_meta_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-29 17:09:30.000000 sutools-0.2.4/tests/test_sutools.py
```

### Comparing `sutools-0.2.3/LICENSE` & `sutools-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/PKG-INFO` & `sutools-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.2.3
+Version: 0.2.4
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
 Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
 Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/sutools/badge/?version=latest)](https://sutools.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/aastopher/sutools/branch/master/graph/badge.svg?token=ZB0AX8D6JI)](https://codecov.io/gh/aastopher/sutools)
 [![PyPI version](https://badge.fury.io/py/sutools.svg)](https://badge.fury.io/py/sutools)
 [![DeepSource](https://deepsource.io/gh/aastopher/sutools.svg/?label=active+issues&show_trend=true&token=RVDa2T7M-E-YSg2DVFbr1ro-)](https://deepsource.io/gh/aastopher/sutools/?ref=repository-badge)
```

### Comparing `sutools-0.2.3/README.md` & `sutools-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/setup.py` & `sutools-0.2.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="sutools",
-    version="0.2.3",
+    version="0.2.4",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["sutools"]),
     description="su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/sutools",
     project_urls={
@@ -18,9 +18,9 @@
     },
     keywords=['logs', 'logger', 'logging', 'cli', 'utils','performance counter', 'benchmark'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.8",
+    python_requires=">=3.6",
 )
```

### Comparing `sutools-0.2.3/sutools/__init__.py` & `sutools-0.2.4/sutools/__init__.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/sutools/bench_handler.py` & `sutools-0.2.4/sutools/bench_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/sutools/cli_handler.py` & `sutools-0.2.4/sutools/cli_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/sutools/log_handler.py` & `sutools-0.2.4/sutools/log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/sutools/meta_handler.py` & `sutools-0.2.4/sutools/meta_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/sutools.egg-info/PKG-INFO` & `sutools-0.2.4/sutools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: sutools
-Version: 0.2.3
+Version: 0.2.4
 Summary: su (Super User) tools; per module utilities, designed to be lightweight, easy to configure, and reduce boilerplate code.
 Home-page: https://github.com/aastopher/sutools
 Author: Aaron Stopher
 Project-URL: Documentation, https://sutools.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/aastopher/sutools/issues
 Keywords: logs,logger,logging,cli,utils,performance counter,benchmark
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Documentation Status](https://readthedocs.org/projects/sutools/badge/?version=latest)](https://sutools.readthedocs.io/en/latest/?badge=latest)
 [![codecov](https://codecov.io/gh/aastopher/sutools/branch/master/graph/badge.svg?token=ZB0AX8D6JI)](https://codecov.io/gh/aastopher/sutools)
 [![PyPI version](https://badge.fury.io/py/sutools.svg)](https://badge.fury.io/py/sutools)
 [![DeepSource](https://deepsource.io/gh/aastopher/sutools.svg/?label=active+issues&show_trend=true&token=RVDa2T7M-E-YSg2DVFbr1ro-)](https://deepsource.io/gh/aastopher/sutools/?ref=repository-badge)
```

### Comparing `sutools-0.2.3/tests/test_bench_handler.py` & `sutools-0.2.4/tests/test_bench_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/tests/test_cli_handler.py` & `sutools-0.2.4/tests/test_cli_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/tests/test_log_handler.py` & `sutools-0.2.4/tests/test_log_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/tests/test_meta_handler.py` & `sutools-0.2.4/tests/test_meta_handler.py`

 * *Files identical despite different names*

### Comparing `sutools-0.2.3/tests/test_sutools.py` & `sutools-0.2.4/tests/test_sutools.py`

 * *Files identical despite different names*

