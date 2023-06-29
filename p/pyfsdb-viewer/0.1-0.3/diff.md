# Comparing `tmp/pyfsdb-viewer-0.1.tar.gz` & `tmp/pyfsdb-viewer-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfsdb-viewer-0.1.tar", last modified: Tue May 23 15:45:19 2023, max compression
+gzip compressed data, was "pyfsdb-viewer-0.3.tar", last modified: Thu Jun 29 21:17:58 2023, max compression
```

## Comparing `pyfsdb-viewer-0.1.tar` & `pyfsdb-viewer-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:45:19.512300 pyfsdb-viewer-0.1/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-05-23 15:45:19.511300 pyfsdb-viewer-0.1/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      212 2023-05-23 15:38:23.000000 pyfsdb-viewer-0.1/README.md
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:45:19.511300 pyfsdb-viewer-0.1/pyfsdb_viewer/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:40:34.000000 pyfsdb-viewer-0.1/pyfsdb_viewer/__init__.py
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       71 2023-05-23 15:13:00.000000 pyfsdb-viewer-0.1/pyfsdb_viewer/pyfsdb_viewer.css
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)     1886 2023-05-23 15:43:01.000000 pyfsdb-viewer-0.1/pyfsdb_viewer/view.py
-drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:45:19.511300 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/PKG-INFO
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      322 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/SOURCES.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/dependency_links.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       52 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/entry_points.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       15 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/requires.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       14 2023-05-23 15:45:19.000000 pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/top_level.txt
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-05-23 15:45:19.512300 pyfsdb-viewer-0.1/setup.cfg
--rw-r--r--   0 hardaker  (2174) hardaker  (2174)      964 2023-05-23 15:45:05.000000 pyfsdb-viewer-0.1/setup.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.031031 pyfsdb-viewer-0.3/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      212 2023-05-23 15:38:23.000000 pyfsdb-viewer-0.3/README.md
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/pyfsdb_viewer/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        0 2023-05-23 15:40:34.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/__init__.py
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      403 2023-06-21 15:38:50.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/pyfsdb_viewer.css
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)     8820 2023-06-21 15:38:50.000000 pyfsdb-viewer-0.3/pyfsdb_viewer/view.py
+drwxr-xr-x   0 hardaker  (2174) hardaker  (2174)        0 2023-06-29 21:17:58.030031 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      581 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/PKG-INFO
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      322 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/SOURCES.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)        1 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/dependency_links.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       52 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/entry_points.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       30 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/requires.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       14 2023-06-29 21:17:57.000000 pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/top_level.txt
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)       38 2023-06-29 21:17:58.031031 pyfsdb-viewer-0.3/setup.cfg
+-rw-r--r--   0 hardaker  (2174) hardaker  (2174)      979 2023-06-29 21:17:38.000000 pyfsdb-viewer-0.3/setup.py
```

### Comparing `pyfsdb-viewer-0.1/PKG-INFO` & `pyfsdb-viewer-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb-viewer
-Version: 0.1
+Version: 0.3
 Summary: A pyfsdb and textual based viewer
 Home-page: https://github.com/gawseed/pyfsdb-viewer
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-viewer-0.1/pyfsdb_viewer.egg-info/PKG-INFO` & `pyfsdb-viewer-0.3/pyfsdb_viewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfsdb-viewer
-Version: 0.1
+Version: 0.3
 Summary: A pyfsdb and textual based viewer
 Home-page: https://github.com/gawseed/pyfsdb-viewer
 Author: Wes Hardaker
 Author-email: opensource@hardakers.net
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pyfsdb-viewer-0.1/setup.py` & `pyfsdb-viewer-0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfsdb-viewer",
-    version="0.1",
+    version="0.3",
     author="Wes Hardaker",
     author_email="opensource@hardakers.net",
     description="A pyfsdb and textual based viewer",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gawseed/pyfsdb-viewer",
     packages=setuptools.find_packages(),
@@ -23,14 +23,14 @@
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
     test_suite="nose.collector",
     tests_require=["nose"],
     install_requires=[
-        "pyfsdb",
-        "textual",
+        "pyfsdb>=2.1.5",
+        "textual>=0.26.0",
     ],
     package_data = {
         'pyfsdb_viewer': ['pyfsdb_viewer.css']
     }
 )
```

