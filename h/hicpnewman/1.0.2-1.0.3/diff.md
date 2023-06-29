# Comparing `tmp/hicpnewman-1.0.2.tar.gz` & `tmp/hicpnewman-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hicpnewman-1.0.2.tar", last modified: Thu Jun 29 15:08:18 2023, max compression
+gzip compressed data, was "hicpnewman-1.0.3.tar", last modified: Thu Jun 29 15:13:47 2023, max compression
```

## Comparing `hicpnewman-1.0.2.tar` & `hicpnewman-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.817713 hicpnewman-1.0.2/
--rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.2/LICENSE.txt
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:08:18.817536 hicpnewman-1.0.2/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 14:58:36.000000 hicpnewman-1.0.2/README.md
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.800798 hicpnewman-1.0.2/hicpnewman/
--rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.2/hicpnewman/__init__.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.802985 hicpnewman-1.0.2/hicpnewman/config/
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.2/hicpnewman/config/config.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.2/hicpnewman/config/config_backup.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.2/hicpnewman/config/config_default.json
--rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.2/hicpnewman/config_manager.py
--rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_argparser.py
--rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_commands.py
--rw-r--r--   0 abuisson   (502) staff       (20)     4330 2023-06-29 15:07:20.000000 hicpnewman-1.0.2/hicpnewman/hicpnewman_helpers.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.799014 hicpnewman-1.0.2/hicpnewman/templates/
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.808339 hicpnewman-1.0.2/hicpnewman/templates/aggregated/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.812399 hicpnewman-1.0.2/hicpnewman/templates/full/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/full/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.815986 hicpnewman-1.0.2/hicpnewman/templates/original/
--rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.2/hicpnewman/templates/original/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:08:18.801830 hicpnewman-1.0.2/hicpnewman.egg-info/
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/SOURCES.txt
--rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/dependency_links.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/entry_points.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       93 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/requires.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 15:08:18.000000 hicpnewman-1.0.2/hicpnewman.egg-info/top_level.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 15:08:18.817755 hicpnewman-1.0.2/setup.cfg
--rw-r--r--   0 abuisson   (502) staff       (20)     1203 2023-06-29 15:08:04.000000 hicpnewman-1.0.2/setup.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.953615 hicpnewman-1.0.3/
+-rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.3/LICENSE.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:13:47.953460 hicpnewman-1.0.3/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 14:58:36.000000 hicpnewman-1.0.3/README.md
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.948182 hicpnewman-1.0.3/hicpnewman/
+-rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.3/hicpnewman/__init__.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.949742 hicpnewman-1.0.3/hicpnewman/config/
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.3/hicpnewman/config/config.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.3/hicpnewman/config/config_backup.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.3/hicpnewman/config/config_default.json
+-rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.3/hicpnewman/config_manager.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.3/hicpnewman/hicpnewman_argparser.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.3/hicpnewman/hicpnewman_commands.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     4330 2023-06-29 15:07:20.000000 hicpnewman-1.0.3/hicpnewman/hicpnewman_helpers.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.947154 hicpnewman-1.0.3/hicpnewman/templates/
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.950790 hicpnewman-1.0.3/hicpnewman/templates/aggregated/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/aggregated/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/aggregated/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/aggregated/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.951955 hicpnewman-1.0.3/hicpnewman/templates/full/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/full/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/full/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/full/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.953085 hicpnewman-1.0.3/hicpnewman/templates/original/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/original/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/original/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.3/hicpnewman/templates/original/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:13:47.949185 hicpnewman-1.0.3/hicpnewman.egg-info/
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/SOURCES.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/dependency_links.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/entry_points.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       93 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/requires.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 15:13:47.000000 hicpnewman-1.0.3/hicpnewman.egg-info/top_level.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 15:13:47.953657 hicpnewman-1.0.3/setup.cfg
+-rw-r--r--   0 abuisson   (502) staff       (20)     1163 2023-06-29 15:13:37.000000 hicpnewman-1.0.3/setup.py
```

### Comparing `hicpnewman-1.0.2/LICENSE.txt` & `hicpnewman-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/README.md` & `hicpnewman-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/config/config.json` & `hicpnewman-1.0.3/hicpnewman/config/config.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/config/config_backup.json` & `hicpnewman-1.0.3/hicpnewman/config/config_backup.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/config/config_default.json` & `hicpnewman-1.0.3/hicpnewman/config/config_default.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/config_manager.py` & `hicpnewman-1.0.3/hicpnewman/config_manager.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/hicpnewman_argparser.py` & `hicpnewman-1.0.3/hicpnewman/hicpnewman_argparser.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/hicpnewman_commands.py` & `hicpnewman-1.0.3/hicpnewman/hicpnewman_commands.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/hicpnewman_helpers.py` & `hicpnewman-1.0.3/hicpnewman/hicpnewman_helpers.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/aggregated/htmlreqres.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/aggregated/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default-colored.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/aggregated/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/aggregated/template-default.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/aggregated/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/full/htmlreqres.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/full/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/full/template-default-colored.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/full/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/full/template-default.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/full/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/original/htmlreqres.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/original/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/original/template-default-colored.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/original/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman/templates/original/template-default.hbs` & `hicpnewman-1.0.3/hicpnewman/templates/original/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/hicpnewman.egg-info/SOURCES.txt` & `hicpnewman-1.0.3/hicpnewman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.2/setup.py` & `hicpnewman-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages, find_namespace_packages
+from setuptools import setup
   
 # some more details
 CLASSIFIERS = [
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.9',
@@ -20,15 +20,15 @@
     'dataclasses',
     'setuptools',
     'dataclasses_json'
 ]
   
 # calling the setup function 
 setup(name='hicpnewman',
-      version='1.0.2',
+      version='1.0.3',
       description='a newman collection runner for hicp',
       url='https://kms-solutions.net',
       author='Antoine Buisson',
       author_email='antoine.buisson@kmse-tech.com',
       packages = ['hicpnewman'],
       package_data={'hicpnewman': ['config/*', 'templates/aggregated/*', 'templates/full/*', 'templates/original/*']},
         entry_points ={
```

