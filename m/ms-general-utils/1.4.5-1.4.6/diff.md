# Comparing `tmp/ms_general_utils-1.4.5.tar.gz` & `tmp/ms_general_utils-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-1.4.5.tar", last modified: Thu Jun 29 09:43:23 2023, max compression
+gzip compressed data, was "ms_general_utils-1.4.6.tar", last modified: Thu Jun 29 11:07:11 2023, max compression
```

## Comparing `ms_general_utils-1.4.5.tar` & `ms_general_utils-1.4.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.237273 ms_general_utils-1.4.5/
--rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2023-06-29 09:43:23.236273 ms_general_utils-1.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.221286 ms_general_utils-1.4.5/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 09:43:23.000000 ms_general_utils-1.4.5/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.232266 ms_general_utils-1.4.5/ms_utils/
--rw-rw-rw-   0        0        0      567 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/__init__.py
--rw-rw-rw-   0        0        0      401 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      566 2023-06-29 09:42:33.000000 ms_general_utils-1.4.5/ms_utils/deploy.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.234267 ms_general_utils-1.4.5/ms_utils/devops/
--rw-rw-rw-   0        0        0      577 2023-06-29 08:11:09.000000 ms_general_utils-1.4.5/ms_utils/devops/Dockerfile
-drwxrwxrwx   0        0        0        0 2023-06-29 09:43:23.235275 ms_general_utils-1.4.5/ms_utils/devops/deploy/
--rw-rw-rw-   0        0        0      196 2023-06-29 08:12:58.000000 ms_general_utils-1.4.5/ms_utils/devops/deploy/script.sh
--rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-1.4.5/ms_utils/devops/docker-compose.yml
--rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-1.4.5/ms_utils/devops/dockerfile.env
--rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/func_date.py
--rw-rw-rw-   0        0        0     2570 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      734 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0      622 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     4721 2023-06-27 12:08:58.000000 ms_general_utils-1.4.5/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2023-06-29 09:43:23.237273 ms_general_utils-1.4.5/setup.cfg
--rw-rw-rw-   0        0        0      888 2023-06-29 09:42:46.000000 ms_general_utils-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:07:11.850180 ms_general_utils-1.4.6/
+-rw-rw-rw-   0        0        0     1091 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2023-06-29 11:07:11.849178 ms_general_utils-1.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      123 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 11:07:11.771604 ms_general_utils-1.4.6/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2023-06-29 11:07:11.000000 ms_general_utils-1.4.6/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-06-29 11:07:11.000000 ms_general_utils-1.4.6/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 11:07:11.000000 ms_general_utils-1.4.6/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-06-29 11:07:11.000000 ms_general_utils-1.4.6/ms_general_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 11:07:11.000000 ms_general_utils-1.4.6/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 11:07:11.838083 ms_general_utils-1.4.6/ms_utils/
+-rw-rw-rw-   0        0        0      567 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     1073 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      566 2023-06-29 09:42:33.000000 ms_general_utils-1.4.6/ms_utils/deploy.py
+drwxrwxrwx   0        0        0        0 2023-06-29 11:07:11.847199 ms_general_utils-1.4.6/ms_utils/devops/
+-rw-rw-rw-   0        0        0      659 2023-06-29 11:06:01.000000 ms_general_utils-1.4.6/ms_utils/devops/Dockerfile
+drwxrwxrwx   0        0        0        0 2023-06-29 11:07:11.848179 ms_general_utils-1.4.6/ms_utils/devops/deploy/
+-rw-rw-rw-   0        0        0      185 2023-06-29 11:06:01.000000 ms_general_utils-1.4.6/ms_utils/devops/deploy/script.sh
+-rw-rw-rw-   0        0        0      288 2023-06-29 08:11:09.000000 ms_general_utils-1.4.6/ms_utils/devops/docker-compose.yml
+-rw-rw-rw-   0        0        0       48 2023-06-29 08:12:49.000000 ms_general_utils-1.4.6/ms_utils/devops/dockerfile.env
+-rw-rw-rw-   0        0        0      727 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0     2570 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      734 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1527 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      357 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0      622 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     4721 2023-06-27 12:08:58.000000 ms_general_utils-1.4.6/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 11:07:11.850180 ms_general_utils-1.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      888 2023-06-29 11:06:37.000000 ms_general_utils-1.4.6/setup.py
```

### Comparing `ms_general_utils-1.4.5/LICENSE.txt` & `ms_general_utils-1.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_general_utils.egg-info/SOURCES.txt` & `ms_general_utils-1.4.6/ms_general_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/__init__.py` & `ms_general_utils-1.4.6/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/binary_uuid.py` & `ms_general_utils-1.4.6/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/deploy.py` & `ms_general_utils-1.4.6/ms_utils/deploy.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/func_date.py` & `ms_general_utils-1.4.6/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/generic_crud_class.py` & `ms_general_utils-1.4.6/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/generic_pagination.py` & `ms_general_utils-1.4.6/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/model_utils.py` & `ms_general_utils-1.4.6/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/validation_utils.py` & `ms_general_utils-1.4.6/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/ms_utils/view_utils.py` & `ms_general_utils-1.4.6/ms_utils/view_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-1.4.5/setup.py` & `ms_general_utils-1.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     package_data={'ms_utils': ['devops/*', 'devops/deploy/*']},
     include_package_data=True,
-    version='1.4.5',
+    version='1.4.6',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

