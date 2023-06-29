# Comparing `tmp/remla12_lib_release-0.1.8.tar.gz` & `tmp/remla12_lib_release-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remla12_lib_release-0.1.8.tar", last modified: Tue Jun 27 09:41:36 2023, max compression
+gzip compressed data, was "remla12_lib_release-0.1.9.tar", last modified: Thu Jun 29 16:31:55 2023, max compression
```

## Comparing `remla12_lib_release-0.1.8.tar` & `remla12_lib_release-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:41:36.005122 remla12_lib_release-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-27 09:41:36.005122 remla12_lib_release-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-27 09:41:24.000000 remla12_lib_release-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:41:36.005122 remla12_lib_release-0.1.8/remla12_lib_release/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-27 09:41:24.000000 remla12_lib_release-0.1.8/remla12_lib_release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-27 09:41:24.000000 remla12_lib_release-0.1.8/remla12_lib_release/version_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:41:36.005122 remla12_lib_release-0.1.8/remla12_lib_release.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-27 09:41:35.000000 remla12_lib_release-0.1.8/remla12_lib_release.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 09:41:35.000000 remla12_lib_release-0.1.8/remla12_lib_release.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:41:35.000000 remla12_lib_release-0.1.8/remla12_lib_release.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-27 09:41:35.000000 remla12_lib_release-0.1.8/remla12_lib_release.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 09:41:36.005122 remla12_lib_release-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-27 09:41:24.000000 remla12_lib_release-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:31:55.189536 remla12_lib_release-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 16:31:55.189536 remla12_lib_release-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-29 16:31:44.000000 remla12_lib_release-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:31:55.189536 remla12_lib_release-0.1.9/remla12_lib_release/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-29 16:31:44.000000 remla12_lib_release-0.1.9/remla12_lib_release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 16:31:44.000000 remla12_lib_release-0.1.9/remla12_lib_release/version_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:31:55.189536 remla12_lib_release-0.1.9/remla12_lib_release.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-29 16:31:55.000000 remla12_lib_release-0.1.9/remla12_lib_release.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-29 16:31:55.000000 remla12_lib_release-0.1.9/remla12_lib_release.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:31:55.000000 remla12_lib_release-0.1.9/remla12_lib_release.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 16:31:55.000000 remla12_lib_release-0.1.9/remla12_lib_release.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:31:55.189536 remla12_lib_release-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-29 16:31:44.000000 remla12_lib_release-0.1.9/setup.py
```

### Comparing `remla12_lib_release-0.1.8/PKG-INFO` & `remla12_lib_release-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: remla12_lib_release
-Version: 0.1.8
+Version: 0.1.9
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.8
+Here you can find all the versions of our lib in PyPi: https://pypi.org/project/remla12-lib-release/#history
+
+Release 0.1.9
```

### Comparing `remla12_lib_release-0.1.8/remla12_lib_release.egg-info/PKG-INFO` & `remla12_lib_release-0.1.9/remla12_lib_release.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: remla12-lib-release
-Version: 0.1.8
+Version: 0.1.9
 Summary: A version-aware library for REMLA12 project
 Home-page: https://github.com/remla23-team12/lib
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Library
 
 The lib repository requires a library that the app repository will depend on. The app repository will intall the lib through a package manager (PyPI). The library has to be published as a package in the same programming language as the app repository.
 
 Changing the below number by incrementing the PATCH version + 1 will trigger the automated workflow (e.g., 0.0.5 --> 0.0.6)
 Note: you need to change init.py,readme,setup 
 
-Release 0.1.8
+Here you can find all the versions of our lib in PyPi: https://pypi.org/project/remla12-lib-release/#history
+
+Release 0.1.9
```

