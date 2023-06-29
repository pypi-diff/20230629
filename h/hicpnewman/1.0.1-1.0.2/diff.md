# Comparing `tmp/hicpnewman-1.0.1.tar.gz` & `tmp/hicpnewman-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hicpnewman-1.0.1.tar", last modified: Thu Jun 29 14:51:17 2023, max compression
+gzip compressed data, was "hicpnewman-1.0.2.tar", last modified: Thu Jun 29 15:08:18 2023, max compression
```

## Comparing `hicpnewman-1.0.1.tar` & `hicpnewman-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.912520 hicpnewman-1.0.1/
--rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.1/LICENSE.txt
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 14:51:17.912379 hicpnewman-1.0.1/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 11:42:21.000000 hicpnewman-1.0.1/README.md
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.908461 hicpnewman-1.0.1/hicpnewman/
--rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.1/hicpnewman/__init__.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.909532 hicpnewman-1.0.1/hicpnewman/config/
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.1/hicpnewman/config/config.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.1/hicpnewman/config/config_backup.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.1/hicpnewman/config/config_default.json
--rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.1/hicpnewman/config_manager.py
--rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.1/hicpnewman/hicpnewman_argparser.py
--rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.1/hicpnewman/hicpnewman_commands.py
--rw-r--r--   0 abuisson   (502) staff       (20)     4354 2023-06-27 15:33:54.000000 hicpnewman-1.0.1/hicpnewman/hicpnewman_helpers.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.907477 hicpnewman-1.0.1/hicpnewman/templates/
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.910299 hicpnewman-1.0.1/hicpnewman/templates/aggregated/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/aggregated/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/aggregated/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/aggregated/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.911174 hicpnewman-1.0.1/hicpnewman/templates/full/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/full/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/full/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/full/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.912057 hicpnewman-1.0.1/hicpnewman/templates/original/
--rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/original/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/original/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.1/hicpnewman/templates/original/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 14:51:17.909177 hicpnewman-1.0.1/hicpnewman.egg-info/
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/SOURCES.txt
--rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/dependency_links.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/entry_points.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       17 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/requires.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 14:51:17.000000 hicpnewman-1.0.1/hicpnewman.egg-info/top_level.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 14:51:17.912562 hicpnewman-1.0.1/setup.cfg
--rw-r--r--   0 abuisson   (502) staff       (20)     1064 2023-06-29 14:51:11.000000 hicpnewman-1.0.1/setup.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.817713 hicpnewman-1.0.2/
+-rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.2/LICENSE.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:08:18.817536 hicpnewman-1.0.2/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 14:58:36.000000 hicpnewman-1.0.2/README.md
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.800798 hicpnewman-1.0.2/hicpnewman/
+-rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.2/hicpnewman/__init__.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.802985 hicpnewman-1.0.2/hicpnewman/config/
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.2/hicpnewman/config/config.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.2/hicpnewman/config/config_backup.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.2/hicpnewman/config/config_default.json
+-rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.2/hicpnewman/config_manager.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_argparser.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_commands.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     4330 2023-06-29 15:07:20.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_helpers.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.799014 hicpnewman-1.0.2/hicpnewman/templates/
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.808339 hicpnewman-1.0.2/hicpnewman/templates/aggregated/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.812399 hicpnewman-1.0.2/hicpnewman/templates/full/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.815986 hicpnewman-1.0.2/hicpnewman/templates/original/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.801830 hicpnewman-1.0.2/hicpnewman.egg-info/
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/SOURCES.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/dependency_links.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/entry_points.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       93 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/requires.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/top_level.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 15:08:18.817755 hicpnewman-1.0.2/setup.cfg
+-rw-r--r--   0 abuisson   (502) staff       (20)     1203 2023-06-29 15:08:04.000000 hicpnewman-1.0.2/setup.py
```

### Comparing `hicpnewman-1.0.1/LICENSE.txt` & `hicpnewman-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/README.md` & `hicpnewman-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/config/config.json` & `hicpnewman-1.0.2/hicpnewman/config/config.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/config/config_backup.json` & `hicpnewman-1.0.2/hicpnewman/config/config_backup.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/config/config_default.json` & `hicpnewman-1.0.2/hicpnewman/config/config_default.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/config_manager.py` & `hicpnewman-1.0.2/hicpnewman/config_manager.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/hicpnewman_argparser.py` & `hicpnewman-1.0.2/hicpnewman/hicpnewman_argparser.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/hicpnewman_commands.py` & `hicpnewman-1.0.2/hicpnewman/hicpnewman_commands.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/hicpnewman_helpers.py` & `hicpnewman-1.0.2/hicpnewman/hicpnewman_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import argparse
 import os 
 from datetime import datetime
-import io
 import json
 import csv
-import base64
 import tempfile
 import subprocess
 
 # argparse Helper Functions
 def csv_file_type(file_path):
     if not file_path.endswith('.csv') or not os.path.isfile(file_path):
         raise argparse.ArgumentTypeError(f"'{file_path}' is not a valid CSV file.")
```

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/aggregated/htmlreqres.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/aggregated/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/aggregated/template-default-colored.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/aggregated/template-default.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/full/htmlreqres.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/full/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/full/template-default-colored.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/full/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/full/template-default.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/full/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/original/htmlreqres.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/original/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/original/template-default-colored.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/original/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman/templates/original/template-default.hbs` & `hicpnewman-1.0.2/hicpnewman/templates/original/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/hicpnewman.egg-info/SOURCES.txt` & `hicpnewman-1.0.2/hicpnewman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.1/setup.py` & `hicpnewman-1.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,20 +6,29 @@
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.9',
     ]
 
 # specify requirements of your package here
 REQUIREMENTS = [
+    'os',
+    'datetime',
+    'tempfile',
+    'subprocess',
+    'json',
+    'argparse',
+    'typing',
+    'dataclasses',
+    'setuptools',
     'dataclasses_json'
 ]
   
 # calling the setup function 
 setup(name='hicpnewman',
-      version='1.0.1',
+      version='1.0.2',
       description='a newman collection runner for hicp',
       url='https://kms-solutions.net',
       author='Antoine Buisson',
       author_email='antoine.buisson@kmse-tech.com',
       packages = ['hicpnewman'],
       package_data={'hicpnewman': ['config/*', 'templates/aggregated/*', 'templates/full/*', 'templates/original/*']},
         entry_points ={
```

