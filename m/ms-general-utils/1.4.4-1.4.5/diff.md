# Comparing `tmp/ms_general_utils-1.4.4.tar.gz` & `tmp/ms_general_utils-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.4.4.tar", last modified: Thu Jun 29 09:36:03 2023, max compression
+gzip compressed data, was "ms_general_utils-1.4.5.tar", last modified: Thu Jun 29 09:43:23 2023, max compression
```

## Comparing `ms_general_utils-1.4.4.tar` & `ms_general_utils-1.4.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.835388 ms_general_utils-1.4.4/
--rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-06-29 09:36:03.834388 ms_general_utils-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.820106 ms_general_utils-1.4.4/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 09:36:03.000000 ms_general_utils-1.4.4/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.830107 ms_general_utils-1.4.4/ms_utils/
--rw-rw-rw-   0        0        0      567 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      568 2023-06-29 08:59:58.000000 ms_general_utils-1.4.4/ms_utils/deploy.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.832388 ms_general_utils-1.4.4/ms_utils/devops/
--rw-rw-rw-   0        0        0      577 2023-06-29 08:11:09.000000 ms_general_utils-1.4.4/ms_utils/devops/Dockerfile
-drwxrwxrwx   0        0        0        0 2023-06-29 09:36:03.833388 ms_general_utils-1.4.4/ms_utils/devops/deploy/
--rw-rw-rw-   0        0        0      196 2023-06-29 08:12:58.000000 ms_general_utils-1.4.4/ms_utils/devops/deploy/script.sh
--rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-1.4.4/ms_utils/devops/docker-compose.yml
--rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-1.4.4/ms_utils/devops/dockerfile.env
--rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      734 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      622 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4721 2023-06-27 12:08:58.000000 ms_general_utils-1.4.4/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-29 09:36:03.835388 ms_general_utils-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-06-29 09:35:31.000000 ms_general_utils-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.237273 ms_general_utils-1.4.5/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-06-29 09:43:23.236273 ms_general_utils-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.221286 ms_general_utils-1.4.5/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.232266 ms_general_utils-1.4.5/ms_utils/
+-rw-rw-rw-   0        0        0      567 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      566 2023-06-29 09:42:33.000000 ms_general_utils-1.4.5/ms_utils/deploy.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.234267 ms_general_utils-1.4.5/ms_utils/devops/
+-rw-rw-rw-   0        0        0      577 2023-06-29 08:11:09.000000 ms_general_utils-1.4.5/ms_utils/devops/Dockerfile
+drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.235275 ms_general_utils-1.4.5/ms_utils/devops/deploy/
+-rw-rw-rw-   0        0        0      196 2023-06-29 08:12:58.000000 ms_general_utils-1.4.5/ms_utils/devops/deploy/script.sh
+-rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-1.4.5/ms_utils/devops/docker-compose.yml
+-rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-1.4.5/ms_utils/devops/dockerfile.env
+-rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      734 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      622 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4721 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:43:23.237273 ms_general_utils-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-06-29 09:42:46.000000 ms_general_utils-1.4.5/setup.py
```

### Comparing `ms_general_utils-1.4.4/LICENSE.txt` & `ms_general_utils-1.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_general_utils.egg-info/SOURCES.txt` & `ms_general_utils-1.4.5/ms_general_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/__init__.py` & `ms_general_utils-1.4.5/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/binary_uuid.py` & `ms_general_utils-1.4.5/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/deploy.py` & `ms_general_utils-1.4.5/ms_utils/deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import errno
 import shutil
 
 import click
 import os
 
 
-# @click.command()
+@click.command()
 def generate():
     call_path = os.getcwd()
     devops_path = os.path.join(os.path.dirname(__file__), "devops")
     for file_name in os.listdir(devops_path):
         print(f"Copy: {file_name}")
         source = os.path.join(devops_path,file_name)
         if os.path.isdir(source):
```

### Comparing `ms_general_utils-1.4.4/ms_utils/devops/Dockerfile` & `ms_general_utils-1.4.5/ms_utils/devops/Dockerfile`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/func_date.py` & `ms_general_utils-1.4.5/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/generic_crud_class.py` & `ms_general_utils-1.4.5/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/generic_pagination.py` & `ms_general_utils-1.4.5/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/model_utils.py` & `ms_general_utils-1.4.5/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/validation_utils.py` & `ms_general_utils-1.4.5/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/ms_utils/view_utils.py` & `ms_general_utils-1.4.5/ms_utils/view_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.4/setup.py` & `ms_general_utils-1.4.5/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     package_data={'ms_utils': ['devops/*', 'devops/deploy/*']},
     include_package_data=True,
-    version='1.4.4',
+    version='1.4.5',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

