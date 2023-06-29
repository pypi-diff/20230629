# Comparing `tmp/regrez-1.0.4.tar.gz` & `tmp/regrez-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-1.0.4.tar", last modified: Thu Jun 29 12:13:58 2023, max compression
+gzip compressed data, was "regrez-1.0.5.tar", last modified: Thu Jun 29 12:28:36 2023, max compression
```

## Comparing `regrez-1.0.4.tar` & `regrez-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:13:58.516142 regrez-1.0.4/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:13:58.299881 regrez-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-06-27 18:39:50.000000 regrez-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 12:13:57.205735 regrez-1.0.4/regrez/
--rw-rw-rw-   0        0        0       22 2023-06-27 11:42:02.000000 regrez-1.0.4/regrez/__init__.py
--rw-rw-rw-   0        0        0     2639 2023-06-27 12:04:53.000000 regrez-1.0.4/regrez/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:13:58.242403 regrez-1.0.4/regrez.egg-info/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:13:56.000000 regrez-1.0.4/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-29 12:13:56.000000 regrez-1.0.4/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:13:56.000000 regrez-1.0.4/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 12:13:56.000000 regrez-1.0.4/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 12:13:56.000000 regrez-1.0.4/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 12:13:58.535524 regrez-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 12:13:40.000000 regrez-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:28:36.924508 regrez-1.0.5/
+-rw-rw-rw-   0        0        0     1469 2023-06-29 12:28:36.911148 regrez-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-06-27 18:39:50.000000 regrez-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 12:28:36.803504 regrez-1.0.5/regrez/
+-rw-rw-rw-   0        0        0       18 2023-06-29 12:27:17.000000 regrez-1.0.5/regrez/__init__.py
+-rw-rw-rw-   0        0        0     2639 2023-06-27 12:04:53.000000 regrez-1.0.5/regrez/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:28:36.900684 regrez-1.0.5/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1469 2023-06-29 12:28:36.000000 regrez-1.0.5/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-29 12:28:36.000000 regrez-1.0.5/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:28:36.000000 regrez-1.0.5/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 12:28:36.000000 regrez-1.0.5/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 12:28:36.000000 regrez-1.0.5/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:28:36.926510 regrez-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-29 12:28:28.000000 regrez-1.0.5/setup.py
```

### Comparing `regrez-1.0.4/PKG-INFO` & `regrez-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.0.4
+Version: 1.0.5
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-1.0.4/README.md` & `regrez-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `regrez-1.0.4/regrez/main.py` & `regrez-1.0.5/regrez/main.py`

 * *Files identical despite different names*

### Comparing `regrez-1.0.4/regrez.egg-info/PKG-INFO` & `regrez-1.0.5/regrez.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.0.4
+Version: 1.0.5
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-1.0.4/setup.py` & `regrez-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.4' 
+VERSION = '1.0.5' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
```

