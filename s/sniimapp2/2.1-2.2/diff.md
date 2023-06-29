# Comparing `tmp/sniimapp2-2.1.tar.gz` & `tmp/sniimapp2-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sniimapp2-2.1.tar", last modified: Wed Jun 28 06:49:35 2023, max compression
+gzip compressed data, was "sniimapp2-2.2.tar", last modified: Thu Jun 29 18:57:17 2023, max compression
```

## Comparing `sniimapp2-2.1.tar` & `sniimapp2-2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-28 06:49:35.754296 sniimapp2-2.1/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1074 2023-06-26 19:27:35.000000 sniimapp2-2.1/LICENSE
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-28 06:49:35.754296 sniimapp2-2.1/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      459 2023-06-28 06:36:27.000000 sniimapp2-2.1/README.md
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      500 2023-06-28 06:47:23.000000 sniimapp2-2.1/pyproject.toml
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-28 06:49:35.754296 sniimapp2-2.1/setup.cfg
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-28 06:49:35.754296 sniimapp2-2.1/sniimapp2.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-28 06:49:35.000000 sniimapp2-2.1/sniimapp2.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      178 2023-06-28 06:49:35.000000 sniimapp2-2.1/sniimapp2.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-28 06:49:35.000000 sniimapp2-2.1/sniimapp2.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       11 2023-06-28 06:49:35.000000 sniimapp2-2.1/sniimapp2.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3196 2023-06-28 02:39:38.000000 sniimapp2-2.1/sniimapp_2.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 18:57:17.847212 sniimapp2-2.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2023-06-29 18:21:41.000000 sniimapp2-2.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2023-06-29 18:57:17.847212 sniimapp2-2.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-06-29 18:33:29.000000 sniimapp2-2.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      514 2023-06-29 18:48:06.000000 sniimapp2-2.2/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 18:57:17.847212 sniimapp2-2.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 18:57:17.847212 sniimapp2-2.2/sniimapp2.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1034 2023-06-29 18:57:17.000000 sniimapp2-2.2/sniimapp2.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      178 2023-06-29 18:57:17.000000 sniimapp2-2.2/sniimapp2.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 18:57:17.000000 sniimapp2-2.2/sniimapp2.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-06-29 18:57:17.000000 sniimapp2-2.2/sniimapp2.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3359 2023-06-29 18:30:15.000000 sniimapp2-2.2/sniimapp_2.py
```

### Comparing `sniimapp2-2.1/LICENSE` & `sniimapp2-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sniimapp2-2.1/PKG-INFO` & `sniimapp2-2.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sniimapp2
-Version: 2.1
-Summary: Extraccion de precios SNIIM
+Version: 2.2
+Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -16,15 +16,15 @@
 
 - MC. Rodolfo Lopez
 - Dr. Oscar de la Torre
 - Dr. Felipe Andoni
 
 ### Descripcion:
 
-- Extraccion de datos del SNIIM.
+- Libreria para la extraccion de precios de granos, frutas y hortalizas del SNIIM.
 
 ### Requerimientos:
 
 - pip install SNIIM_2
 - pip install mysql-connector-Python
 
 ### Uso:
```

### Comparing `sniimapp2-2.1/sniimapp2.egg-info/PKG-INFO` & `sniimapp2-2.2/sniimapp2.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sniimapp2
-Version: 2.1
-Summary: Extraccion de precios SNIIM
+Version: 2.2
+Summary: Libreria para extraccion de precios SNIIM
 Author-email: Rodolfo Lopez <1803672F@umich.mx>
 Project-URL: Homepage, https://github.com/rodolfolopezfcca/sniimapp_2
 Project-URL: Bug Tracker, https://github.com/rodolfolopezfcca/sniimapp_2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -16,15 +16,15 @@
 
 - MC. Rodolfo Lopez
 - Dr. Oscar de la Torre
 - Dr. Felipe Andoni
 
 ### Descripcion:
 
-- Extraccion de datos del SNIIM.
+- Libreria para la extraccion de precios de granos, frutas y hortalizas del SNIIM.
 
 ### Requerimientos:
 
 - pip install SNIIM_2
 - pip install mysql-connector-Python
 
 ### Uso:
```

