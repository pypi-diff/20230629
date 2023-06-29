# Comparing `tmp/pylsat-0.1.tar.gz` & `tmp/pylsat-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsat-0.1.tar", last modified: Thu Jun 29 13:51:18 2023, max compression
+gzip compressed data, was "pylsat-0.2.tar", last modified: Thu Jun 29 14:11:31 2023, max compression
```

## Comparing `pylsat-0.1.tar` & `pylsat-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:51:18.977038 pylsat-0.1/
--rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.1/LICENSE
--rw-rw-rw-   0        0        0      300 2023-06-29 13:51:18.975898 pylsat-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 13:51:18.972898 pylsat-0.1/pylsat.egg-info/
--rw-rw-rw-   0        0        0      300 2023-06-29 13:51:18.000000 pylsat-0.1/pylsat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-06-29 13:51:18.000000 pylsat-0.1/pylsat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:51:18.000000 pylsat-0.1/pylsat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-29 13:51:18.000000 pylsat-0.1/pylsat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:51:18.000000 pylsat-0.1/pylsat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:51:18.978039 pylsat-0.1/setup.cfg
--rw-rw-rw-   0        0        0      562 2023-06-29 13:48:00.000000 pylsat-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:11:31.186502 pylsat-0.2/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2/LICENSE
+-rw-rw-rw-   0        0        0      300 2023-06-29 14:11:31.186502 pylsat-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 14:11:31.184332 pylsat-0.2/pylsat.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:11:31.186502 pylsat-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      542 2023-06-29 14:09:51.000000 pylsat-0.2/setup.py
```

### Comparing `pylsat-0.1/LICENSE` & `pylsat-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pylsat-0.1/setup.py` & `pylsat-0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pylsat',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'fastapi', 
         'starlette', 
         'pymacaroons', 
         'datetime', 
         'hashlib', 
-        'uuid', 
-        'bolt11'
+        'uuid'
     ],
     url='https://github.com/plebos/pylsat',
     license='MIT',
     author='Tal Shmueli',
     author_email='tal@shmueli.org',
     description='A Python library for validating Lightning Service Authentication Tokens (LSAT) in a FastAPI application.'
 )
```

