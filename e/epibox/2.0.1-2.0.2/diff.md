# Comparing `tmp/epibox-2.0.1.tar.gz` & `tmp/epibox-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epibox-2.0.1.tar", last modified: Tue Jun 27 17:31:38 2023, max compression
+gzip compressed data, was "epibox-2.0.2.tar", last modified: Thu Jun 29 17:29:13 2023, max compression
```

## Comparing `epibox-2.0.1.tar` & `epibox-2.0.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-27 17:31:22.000000 epibox-2.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-27 17:31:22.000000 epibox-2.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-27 17:31:22.000000 epibox-2.0.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-27 17:31:22.000000 epibox-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-27 17:31:22.000000 epibox-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:31:38.144710 epibox-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-27 17:31:22.000000 epibox-2.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.136710 epibox-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-27 17:31:22.000000 epibox-2.0.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.136710 epibox-2.0.1/epibox/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/create_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/get_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/read_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/run_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/common/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/config_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox/devices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/connect_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/devices/manage_devices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/exception_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/exceptions/system_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/mqtt_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/message_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/mqtt_manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.144710 epibox-2.0.1/epibox/run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-27 17:31:22.000000 epibox-2.0.1/epibox/run/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 17:31:38.140710 epibox-2.0.1/epibox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 17:31:37.000000 epibox-2.0.1/epibox.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-27 17:31:38.000000 epibox-2.0.1/epibox.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 17:31:38.144710 epibox-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-27 17:31:22.000000 epibox-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.009562 epibox-2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-29 17:29:03.000000 epibox-2.0.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-29 17:29:03.000000 epibox-2.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 17:29:03.000000 epibox-2.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-29 17:29:03.000000 epibox-2.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-29 17:29:03.000000 epibox-2.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-29 17:29:13.005562 epibox-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-29 17:29:03.000000 epibox-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 17:29:03.000000 epibox-2.0.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/create_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/get_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/read_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/run_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/common/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/config_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/connect_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/devices/manage_devices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/exception_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/exceptions/system_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/mqtt_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/message_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/mqtt_manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox/run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-29 17:29:03.000000 epibox-2.0.2/epibox/run/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:29:13.005562 epibox-2.0.2/epibox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-29 17:29:13.000000 epibox-2.0.2/epibox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 17:29:12.000000 epibox-2.0.2/epibox.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:29:13.009562 epibox-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-29 17:29:03.000000 epibox-2.0.2/setup.py
```

### Comparing `epibox-2.0.1/CONTRIBUTING.rst` & `epibox-2.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/LICENSE` & `epibox-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/PKG-INFO` & `epibox-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.1
+Version: 2.0.2
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.1/README.md` & `epibox-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/docs/Makefile` & `epibox-2.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/docs/conf.py` & `epibox-2.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/docs/installation.rst` & `epibox-2.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/docs/make.bat` & `epibox-2.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/common/get_defaults.py` & `epibox-2.0.2/epibox/common/get_defaults.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,32 +2,35 @@
 import ast
 import os
 from pathlib import Path
 
 
 def get_default():
 
-    defaults_path = os.path.join(
-        Path.home(), "Documents", "epibox", "args.json")
+    defaults_dir = os.path.join(
+        Path.home(), "Documents", "EpiBOX Core")
+    defaults_path = os.path.join(defaults_dir, "args.json")
 
-    if os.path.isfile(defaults_path):
-
-        with open(defaults_path, "r") as json_file:
-            defaults = json_file.read()
-            defaults = ast.literal_eval(defaults)
-
-    else:  # the first time using EpiBOX Core, there will be no default file
-        os.makedirs(os.path.dirname(defaults_path))
-        defaults = {
+    defaults = {
             "initial_dir": "EpiBOX Core",
             "fs": 1000,
             "channels": [],
             "devices_mac": {"MAC1": "COM3"},
             "save_raw": "true",
             "patient_id": "default",
             "service": "scientisst",
         }
 
+    if os.path.isdir(defaults_dir):
+        
+        if os.path.isfile(defaults_path):
+            with open(defaults_path, "r") as json_file:
+                defaults = json_file.read()
+                defaults = ast.literal_eval(defaults)
+
+    else:  # the first time using EpiBOX Core, there will be no default file
+        os.makedirs(defaults_dir)
+
     with open(defaults_path, "w+") as json_file:
         json.dump(defaults, json_file)
 
     return defaults
```

### Comparing `epibox-2.0.1/epibox/common/open_file.py` & `epibox-2.0.2/epibox/common/open_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/common/process_data.py` & `epibox-2.0.2/epibox/common/process_data.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/common/read_modules.py` & `epibox-2.0.2/epibox/common/read_modules.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/common/run_system.py` & `epibox-2.0.2/epibox/common/run_system.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/common/setup.py` & `epibox-2.0.2/epibox/common/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # built-in
 import time
 import os
 from sys import platform
+from pathlib import Path
 
 # third-party
 import paho.mqtt.client as mqtt
 from epibox.common.get_defaults import get_default
 from epibox.exceptions.system_exceptions import (
     MQTTConnectionError,
     PlatformNotSupportedError,
@@ -116,38 +117,40 @@
     return t_all, already_notified_pause, system_started
 
 
 def check_storage(client, opt):
     # Check if default storage is available | loop runs continuosly until it find the storage or until timeout
     # If timeout, setup loop and acquisition are terminated
 
-    if platform == "linux" or platform == "linux2":
-        # linux
-        drive_path = os.path.join("media", os.getlogin())
-    elif platform == "darwin":
-        # macos
-        drive_path = "/Volumes"
+    if opt["initial_dir"] == "EpiBOX Core":
+        drive_path = os.path.join(Path.home(), "Documents", "EpiBOX Core")
+        opt["initial_dir"] = os.path.join(drive_path, "acquisitions")
+
     else:
-        # import win32api
-        drive_path = ""
+        if platform == "linux" or platform == "linux2":
+            # linux
+            drive_path = os.path.join("/media", os.getlogin(), opt["initial_dir"])
+        elif platform == "darwin":
+            # macos
+            drive_path = os.path.join("/Volumes", opt["initial_dir"])
+        else:
+            drive_path = opt["initial_dir"]
 
-    init_connect_time = time.time()
-    config_debug.log(f'Searching for storage module: {opt["initial_dir"]}')
+        init_connect_time = time.time()
+        config_debug.log(f'Searching for storage module: {opt["initial_dir"]}')
 
-    for i in range(100000):
+        for i in range(100000):
 
-        if (time.time() - init_connect_time) > 120:
-            raise StorageTimeout
-
-        if os.path.isdir(f"/{drive_path}/" + opt["initial_dir"]):
-            opt["initial_dir"] = (
-                f"/{drive_path}/" + opt["initial_dir"] + "/acquisitions"
-            )
-            break
+            if (time.time() - init_connect_time) > 120:
+                raise StorageTimeout
 
-        else:
-            if time.time() - init_connect_time > 3 * i:
-                message_info = client.publish("rpi", str(["INSERT STORAGE"]))
-                if message_info.rc == 4:
-                    raise MQTTConnectionError
+            if os.path.isdir(drive_path):
+                opt["initial_dir"] = os.path.join(drive_path, "acquisitions")
+                break
+
+            else:
+                if time.time() - init_connect_time > 3 * i:
+                    message_info = client.publish("rpi", str(["INSERT STORAGE"]))
+                    if message_info.rc == 4:
+                        raise MQTTConnectionError
 
     return opt
```

### Comparing `epibox-2.0.1/epibox/common/write_file.py` & `epibox-2.0.2/epibox/common/write_file.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/devices/connect_device.py` & `epibox-2.0.2/epibox/devices/connect_device.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/devices/header.py` & `epibox-2.0.2/epibox/devices/header.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/devices/manage_devices.py` & `epibox-2.0.2/epibox/devices/manage_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,14 +96,16 @@
     for mac in opt["devices_mac"]:
 
         init_connect_time = time.time()
         config_debug.log(f"Searching for Module... {mac}")
 
         for i in range(100000):
 
+            if not client.keepAlive: break
+
             if (time.time() - init_connect_time) > 120:
                 raise DeviceConnectionTimeout
 
             try:
                 connected = False
                 connected, devices = connect_device(
                     mac, client, devices, opt["service"]
```

### Comparing `epibox-2.0.1/epibox/exceptions/exception_manager.py` & `epibox-2.0.2/epibox/exceptions/exception_manager.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/exceptions/system_exceptions.py` & `epibox-2.0.2/epibox/exceptions/system_exceptions.py`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/epibox/mqtt_manager/message_handler.py` & `epibox-2.0.2/epibox/mqtt_manager/message_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # built-in
 import ast
 import os
 import subprocess
 import json
 import shutil
 from sys import platform
+from pathlib import Path
 
 # local
 from epibox import config_debug
 from epibox.common.get_defaults import get_default
 from epibox.exceptions.system_exceptions import (
     MQTTConnectionError,
 
@@ -18,30 +19,30 @@
 def send_default(client):
 
     ######## Available drives ########
     listDrives = ["DRIVES"]
 
     if platform == "linux" or platform == "linux2":
         # linux
-        drive_path = os.path.join("media", os.getlogin())
-        drives = os.listdir(f"/{drive_path}/")
+        drive_path = os.path.join("/media", os.getlogin())
+        drives = [os.path.join(drive_path, d) for d in os.listdir(drive_path)]
     elif platform == "darwin":
         # macos
         drive_path = "/Volumes"
-        drives = os.listdir(f"{drive_path}/")
+        drives = [os.path.join(drive_path, d) for d in os.listdir(drive_path)]
     else:
         import win32api
         import win32con
         import win32file
         drives = [i for i in win32api.GetLogicalDriveStrings().split('\x00') if i]
         drives = [d for d in drives if win32file.GetDriveType(
             d) == win32con.DRIVE_REMOVABLE]
 
     for drive in drives:
-        total, _, free = shutil.disk_usage(f"/{drive_path}/{drive}")
+        total, _, free = shutil.disk_usage(drive)
         listDrives += ["{} ({:.1f}% livre)".format(drive,
                                                    (free / total) * 100)]
 
     message_info = client.publish(
         topic="rpi", qos=2, payload="{}".format(listDrives)
     )  # raises ValueError and TypeError
     if message_info.rc == 4:
@@ -119,15 +120,15 @@
 
         username = os.getlogin()
 
         for key in message[1].keys():
             defaults[key] = message[1][key]
 
         with open(
-            "/home/{}/Documents/epibox/args.json".format(username), "w+"
+            os.path.join(Path.home(), "Documents", "EpiBOX Core", "args.json"), "w+"
         ) as json_file:
             json.dump(defaults, json_file)
 
         msg = json.dumps(["RECEIVED DEFAULT"])
         message_info = client.publish(topic="rpi", qos=2, payload=msg)
         if message_info.rc == 4:
             raise MQTTConnectionError
```

### Comparing `epibox-2.0.1/epibox/run/run.py` & `epibox-2.0.2/epibox/run/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,18 @@
     # Setup MQTT client | read default configurations | initiate variables ===========================
     try:
         client = setup_client()
 
     except (MQTTConnectionError, ConnectionRefusedError, ValueError, TypeError) as e:
         config_debug.log(e)
         kill_case_1()
+    except (TimeoutError, ConnectionAbortedError):
+        config_debug.log("Wrong network - connect to PreEpiSeizures")
+        kill_case_1()
+
 
     try:
         opt, channels, sensors, service, save_raw = setup_config(client)
 
         (
             t_all,
             already_notified_pause,
@@ -106,33 +110,26 @@
 
     config_debug.log("Initial setup complete!")
 
     while client.keepAlive:
 
         try:
 
-            if client.newAnnot != None:
-                # Write user annotation to file if one is received via MQTT ===============================
-                # TODO exception handling
-                config_debug.log(f"annot: {client.newAnnot}")
-                write_annot_file(a_file.name, client.newAnnot)
-                client.newAnnot = None
-
             if client.pauseAcq and not already_notified_pause:
                 # Pause acquisition if command is received via MQTT ========================================
 
                 # devices = pause_devices(client, devices)
                 system_started = handle_case_6(devices, a_file, system_started)
                 message_info = client.publish("rpi", str(["PAUSED"]))
                 if message_info.rc == 4:
                     raise MQTTConnectionError
                 already_notified_pause = True
 
             if not client.pauseAcq:
-
+                
                 if already_notified_pause:
                     message_info = client.publish("rpi", str(["RECONNECTING"]))
                     if message_info.rc == 4:
                         raise MQTTConnectionError
                     already_notified_pause = False
 
                 if not system_started:
@@ -142,14 +139,22 @@
                         devices,
                         channels,
                         sensors,
                         opt["fs"],
                         save_raw,
                         service,
                     )
+
+                    if client.newAnnot != None:
+                        # Write user annotation to file if one is received via MQTT ===============================
+                        # TODO exception handling
+                        config_debug.log(f"annot: {client.newAnnot}")
+                        write_annot_file(a_file.name, client.newAnnot)
+                        client.newAnnot = None
+
                     sync_param = start_devices(
                         client, devices, opt["fs"], channels, header
                     )
                     system_started = True
                     already_timed_out = False
 
                 # Read batch of samples from the acquisition devices and store on the active session's file
```

### Comparing `epibox-2.0.1/epibox.egg-info/PKG-INFO` & `epibox-2.0.2/epibox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epibox
-Version: 2.0.1
+Version: 2.0.2
 Summary: EpiBOX is a Raspberry Pi tool for easy signal acquisition.
 Home-page: https://github.com/anascacais/epibox
 Author: Ana Sofia Carmo
 Author-email: anascacais@gmail.com
 License: MIT license
 Keywords: epibox,signal acquisition,Raspberry Pi
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `epibox-2.0.1/epibox.egg-info/SOURCES.txt` & `epibox-2.0.2/epibox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `epibox-2.0.1/setup.py` & `epibox-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,10 +51,10 @@
     include_package_data=True,
     keywords=["epibox", "signal acquisition", "Raspberry Pi"],
     name="epibox",
     packages=find_packages(include=["epibox", "epibox.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/anascacais/epibox",
-    version="2.0.1",
+    version="2.0.2",
     zip_safe=False,
 )
```

