# Comparing `tmp/regrez-1.1.5.tar.gz` & `tmp/regrez-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regrez-1.1.5.tar", last modified: Thu Jun 29 12:35:17 2023, max compression
+gzip compressed data, was "regrez-1.1.6.tar", last modified: Thu Jun 29 12:38:48 2023, max compression
```

## Comparing `regrez-1.1.5.tar` & `regrez-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:35:17.179421 regrez-1.1.5/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:35:17.176423 regrez-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      974 2023-06-27 18:39:50.000000 regrez-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 12:35:17.090585 regrez-1.1.5/regrez/
--rw-rw-rw-   0        0        0       42 2023-06-29 12:34:31.000000 regrez-1.1.5/regrez/__init__.py
--rw-rw-rw-   0        0        0     2639 2023-06-27 12:04:53.000000 regrez-1.1.5/regrez/main.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:35:17.171450 regrez-1.1.5/regrez.egg-info/
--rw-rw-rw-   0        0        0     1469 2023-06-29 12:35:16.000000 regrez-1.1.5/regrez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-29 12:35:16.000000 regrez-1.1.5/regrez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:35:16.000000 regrez-1.1.5/regrez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-29 12:35:16.000000 regrez-1.1.5/regrez.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 12:35:16.000000 regrez-1.1.5/regrez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 12:35:17.186860 regrez-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 12:35:06.000000 regrez-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.236747 regrez-1.1.6/
+-rw-rw-rw-   0        0        0     1469 2023-06-29 12:38:48.226174 regrez-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      974 2023-06-27 18:39:50.000000 regrez-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.124079 regrez-1.1.6/regrez/
+-rw-rw-rw-   0        0        0       23 2023-06-29 12:37:40.000000 regrez-1.1.6/regrez/__init__.py
+-rw-rw-rw-   0        0        0     2639 2023-06-27 12:04:53.000000 regrez-1.1.6/regrez/main.py
+drwxrwxrwx   0        0        0        0 2023-06-29 12:38:48.214965 regrez-1.1.6/regrez.egg-info/
+-rw-rw-rw-   0        0        0     1469 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 12:38:47.000000 regrez-1.1.6/regrez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 12:38:48.237756 regrez-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      845 2023-06-29 12:38:30.000000 regrez-1.1.6/setup.py
```

### Comparing `regrez-1.1.5/PKG-INFO` & `regrez-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.1.5
+Version: 1.1.6
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-1.1.5/README.md` & `regrez-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `regrez-1.1.5/regrez/main.py` & `regrez-1.1.6/regrez/main.py`

 * *Files identical despite different names*

### Comparing `regrez-1.1.5/regrez.egg-info/PKG-INFO` & `regrez-1.1.6/regrez.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regrez
-Version: 1.1.5
+Version: 1.1.6
 Summary: Easiest way to implement linear regression.
 Home-page: UNKNOWN
 Author: Mehmet Utku OZTURK
 Author-email: <contact@ælphard.tk>
 License: UNKNOWN
 Keywords: regression,machine learning
 Platform: UNKNOWN
```

### Comparing `regrez-1.1.5/setup.py` & `regrez-1.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.5' 
+VERSION = '1.1.6' 
 DESCRIPTION = 'Easiest way to implement linear regression.'
 
 with open('README.md') as f:
     long = f.read()
 setup(
         name="regrez", 
         version=VERSION,
```

