# Comparing `tmp/prodiapy-3.2.tar.gz` & `tmp/prodiapy-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodiapy-3.2.tar", last modified: Fri Jun 16 04:43:41 2023, max compression
+gzip compressed data, was "prodiapy-3.3.tar", last modified: Thu Jun 29 19:00:12 2023, max compression
```

## Comparing `prodiapy-3.2.tar` & `prodiapy-3.3.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.809860 prodiapy-3.2/
--rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.2/LICENSE
--rw-rw-rw-   0        0        0     1050 2023-06-16 04:43:41.808592 prodiapy-3.2/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-06-16 04:43:22.000000 prodiapy-3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.800596 prodiapy-3.2/prodia/
--rw-rw-rw-   0        0        0      240 2023-06-15 12:59:58.000000 prodiapy-3.2/prodia/__init__.py
--rw-rw-rw-   0        0        0     4226 2023-06-14 12:51:44.000000 prodiapy-3.2/prodia/ext.py
--rw-rw-rw-   0        0        0    12255 2023-06-16 04:42:15.000000 prodiapy-3.2/prodia/main.py
-drwxrwxrwx   0        0        0        0 2023-06-16 04:43:41.807259 prodiapy-3.2/prodiapy.egg-info/
--rw-rw-rw-   0        0        0     1050 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-16 04:43:41.000000 prodiapy-3.2/prodiapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 04:43:41.809860 prodiapy-3.2/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-06-16 04:43:12.000000 prodiapy-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.221973 prodiapy-3.3/
+-rw-rw-rw-   0        0        0    11558 2023-04-21 18:41:23.000000 prodiapy-3.3/LICENSE
+-rw-rw-rw-   0        0        0     1041 2023-06-29 19:00:12.220683 prodiapy-3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2023-06-29 18:59:44.000000 prodiapy-3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.208530 prodiapy-3.3/prodia/
+-rw-rw-rw-   0        0        0      155 2023-06-29 15:03:14.000000 prodiapy-3.3/prodia/__init__.py
+-rw-rw-rw-   0        0        0    17337 2023-06-29 15:09:24.000000 prodiapy-3.3/prodia/async_prodia.py
+-rw-rw-rw-   0        0        0     3809 2023-06-29 13:54:34.000000 prodiapy-3.3/prodia/constants.py
+-rw-rw-rw-   0        0        0      340 2023-06-29 12:58:05.000000 prodiapy-3.3/prodia/exceptions.py
+-rw-rw-rw-   0        0        0    17271 2023-06-29 15:10:51.000000 prodiapy-3.3/prodia/sync_prodia.py
+-rw-rw-rw-   0        0        0     2645 2023-06-29 18:12:53.000000 prodiapy-3.3/prodia/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 19:00:12.220683 prodiapy-3.3/prodiapy.egg-info/
+-rw-rw-rw-   0        0        0     1041 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 19:00:12.000000 prodiapy-3.3/prodiapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 19:00:12.221973 prodiapy-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      414 2023-06-29 18:59:16.000000 prodiapy-3.3/setup.py
```

### Comparing `prodiapy-3.2/LICENSE` & `prodiapy-3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prodiapy-3.2/PKG-INFO` & `prodiapy-3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.2
+Version: 3.3
 Summary: Prodia API Python Wrapper
-Author: yoou3-cyber
+Author: zenafey
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.2
+pip install prodiapy
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

### Comparing `prodiapy-3.2/README.md` & `prodiapy-3.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.2
+pip install prodiapy
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

### Comparing `prodiapy-3.2/prodiapy.egg-info/PKG-INFO` & `prodiapy-3.3/prodiapy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: prodiapy
-Version: 3.2
+Version: 3.3
 Summary: Prodia API Python Wrapper
-Author: yoou3-cyber
+Author: zenafey
 Author-email: zenafey@eugw.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # prodiapy
 This module makes generation of image by Prodia API easier
 
 ### Installation 
 ```
-pip install prodiapy==3.2
+pip install prodiapy
 ```
 For using this script you need to get your Prodia api key, you can make it on https://app.prodia.com/api
 
 
 ### Example of txt2img usage
 ```python
 import prodia
```

