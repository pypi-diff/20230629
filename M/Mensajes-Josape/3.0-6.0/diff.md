# Comparing `tmp/Mensajes-Josape-3.0.tar.gz` & `tmp/Mensajes-Josape-6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mensajes-Josape-3.0.tar", last modified: Thu Jun 29 07:04:50 2023, max compression
+gzip compressed data, was "Mensajes-Josape-6.0.tar", last modified: Thu Jun 29 07:20:14 2023, max compression
```

## Comparing `Mensajes-Josape-3.0.tar` & `Mensajes-Josape-6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.961948 Mensajes-Josape-3.0/
--rw-rw-rw-   0        0        0     1099 2023-06-29 06:43:35.000000 Mensajes-Josape-3.0/LICENSE
--rw-rw-rw-   0        0        0       60 2023-06-29 06:43:36.000000 Mensajes-Josape-3.0/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.938012 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/
--rw-rw-rw-   0        0        0      715 2023-06-29 07:04:50.000000 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-06-29 07:04:50.000000 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 07:04:50.000000 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-29 07:04:50.000000 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-29 07:04:50.000000 Mensajes-Josape-3.0/Mensajes_Josape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      715 2023-06-29 07:04:50.960950 Mensajes-Josape-3.0/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-06-29 06:32:38.000000 Mensajes-Josape-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.940007 Mensajes-Josape-3.0/mensajes/
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.945990 Mensajes-Josape-3.0/mensajes/Adios/
--rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-Josape-3.0/mensajes/Adios/__init__.py
--rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-Josape-3.0/mensajes/Adios/despedidas.py
--rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-Josape-3.0/mensajes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.953969 Mensajes-Josape-3.0/mensajes/hola/
--rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-Josape-3.0/mensajes/hola/__init__.py
--rw-rw-rw-   0        0        0      373 2023-06-29 06:43:50.000000 Mensajes-Josape-3.0/mensajes/hola/saludos.py
--rw-rw-rw-   0        0        0       15 2023-06-29 06:16:56.000000 Mensajes-Josape-3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 07:04:50.961948 Mensajes-Josape-3.0/setup.cfg
--rw-rw-rw-   0        0        0      983 2023-06-29 07:04:18.000000 Mensajes-Josape-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 07:04:50.958961 Mensajes-Josape-3.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-28 07:43:44.000000 Mensajes-Josape-3.0/tests/__init__.py
--rw-rw-rw-   0        0        0      266 2023-06-29 06:43:52.000000 Mensajes-Josape-3.0/tests/test_hola.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.260614 Mensajes-Josape-6.0/
+-rw-rw-rw-   0        0        0     1099 2023-06-29 06:43:35.000000 Mensajes-Josape-6.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-29 06:43:36.000000 Mensajes-Josape-6.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.224710 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/
+-rw-rw-rw-   0        0        0      715 2023-06-29 07:20:14.000000 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      414 2023-06-29 07:20:14.000000 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:20:14.000000 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 07:20:14.000000 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-29 07:20:14.000000 Mensajes-Josape-6.0/Mensajes_Josape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      715 2023-06-29 07:20:14.259617 Mensajes-Josape-6.0/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-06-29 06:32:38.000000 Mensajes-Josape-6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.230695 Mensajes-Josape-6.0/mensajes/
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.237675 Mensajes-Josape-6.0/mensajes/Adios/
+-rw-rw-rw-   0        0        0       47 2022-07-07 17:43:51.000000 Mensajes-Josape-6.0/mensajes/Adios/__init__.py
+-rw-rw-rw-   0        0        0      182 2022-07-07 17:45:52.000000 Mensajes-Josape-6.0/mensajes/Adios/despedidas.py
+-rw-rw-rw-   0        0        0       38 2022-07-07 17:39:14.000000 Mensajes-Josape-6.0/mensajes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.251638 Mensajes-Josape-6.0/mensajes/hola/
+-rw-rw-rw-   0        0        0       46 2022-07-07 17:41:56.000000 Mensajes-Josape-6.0/mensajes/hola/__init__.py
+-rw-rw-rw-   0        0        0      382 2023-06-29 07:20:04.000000 Mensajes-Josape-6.0/mensajes/hola/saludos.py
+-rw-rw-rw-   0        0        0       15 2023-06-29 06:16:56.000000 Mensajes-Josape-6.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:20:14.261611 Mensajes-Josape-6.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2023-06-29 07:19:59.000000 Mensajes-Josape-6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:20:14.256625 Mensajes-Josape-6.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-28 07:43:44.000000 Mensajes-Josape-6.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-06-29 06:43:52.000000 Mensajes-Josape-6.0/tests/test_hola.py
```

### Comparing `Mensajes-Josape-3.0/LICENSE` & `Mensajes-Josape-6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mensajes-Josape-3.0/Mensajes_Josape.egg-info/PKG-INFO` & `Mensajes-Josape-6.0/Mensajes_Josape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Josape
-Version: 3.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Joaquin Santias Pereira
 Author-email: josapemu10@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-Josape-3.0/PKG-INFO` & `Mensajes-Josape-6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mensajes-Josape
-Version: 3.0
+Version: 6.0
 Summary: Un paquete para saludar y despedir
 Home-page: https://www.hektor.dev
 Author: Joaquin Santias Pereira
 Author-email: josapemu10@gmail.com
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Mensajes-Josape-3.0/setup.py` & `Mensajes-Josape-6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Mensajes-Josape',
-    version='3.0',
+    version='6.0',
     description='Un paquete para saludar y despedir',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Joaquin Santias Pereira',
     author_email='josapemu10@gmail.com',
     url='https://www.hektor.dev',
     license_files=['LICENSE'],
```

