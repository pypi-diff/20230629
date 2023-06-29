# Comparing `tmp/hicpnewman-1.0.4.tar.gz` & `tmp/hicpnewman-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hicpnewman-1.0.4.tar", last modified: Thu Jun 29 15:34:26 2023, max compression
+gzip compressed data, was "hicpnewman-1.0.5.tar", last modified: Thu Jun 29 15:39:04 2023, max compression
```

## Comparing `hicpnewman-1.0.4.tar` & `hicpnewman-1.0.5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.840931 hicpnewman-1.0.4/
--rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.4/LICENSE.txt
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:34:26.840778 hicpnewman-1.0.4/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 14:58:36.000000 hicpnewman-1.0.4/README.md
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.835505 hicpnewman-1.0.4/hicpnewman/
--rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.4/hicpnewman/__init__.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.837080 hicpnewman-1.0.4/hicpnewman/config/
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.4/hicpnewman/config/config.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.4/hicpnewman/config/config_backup.json
--rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.4/hicpnewman/config/config_default.json
--rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.4/hicpnewman/config_manager.py
--rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.4/hicpnewman/hicpnewman_argparser.py
--rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.4/hicpnewman/hicpnewman_commands.py
--rw-r--r--   0 abuisson   (502) staff       (20)     4330 2023-06-29 15:07:20.000000 hicpnewman-1.0.4/hicpnewman/hicpnewman_helpers.py
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.834547 hicpnewman-1.0.4/hicpnewman/templates/
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.838538 hicpnewman-1.0.4/hicpnewman/templates/aggregated/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/aggregated/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/aggregated/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/aggregated/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.839551 hicpnewman-1.0.4/hicpnewman/templates/full/
--rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/full/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/full/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/full/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.840448 hicpnewman-1.0.4/hicpnewman/templates/original/
--rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/original/htmlreqres.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/original/template-default-colored.hbs
--rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.4/hicpnewman/templates/original/template-default.hbs
-drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:34:26.836605 hicpnewman-1.0.4/hicpnewman.egg-info/
--rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/PKG-INFO
--rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/SOURCES.txt
--rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/dependency_links.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/entry_points.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       17 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/requires.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 15:34:26.000000 hicpnewman-1.0.4/hicpnewman.egg-info/top_level.txt
--rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 15:34:26.840968 hicpnewman-1.0.4/setup.cfg
--rw-r--r--   0 abuisson   (502) staff       (20)     1024 2023-06-29 15:34:22.000000 hicpnewman-1.0.4/setup.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.795167 hicpnewman-1.0.5/
+-rw-r--r--   0 abuisson   (502) staff       (20)     1074 2023-06-23 09:21:53.000000 hicpnewman-1.0.5/LICENSE.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:39:04.794989 hicpnewman-1.0.5/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)    12206 2023-06-29 14:58:36.000000 hicpnewman-1.0.5/README.md
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.781144 hicpnewman-1.0.5/hicpnewman/
+-rw-r--r--   0 abuisson   (502) staff       (20)        0 2023-06-23 09:22:38.000000 hicpnewman-1.0.5/hicpnewman/__init__.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.783115 hicpnewman-1.0.5/hicpnewman/config/
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:16:14.000000 hicpnewman-1.0.5/hicpnewman/config/config.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:20:15.000000 hicpnewman-1.0.5/hicpnewman/config/config_backup.json
+-rw-r--r--   0 abuisson   (502) staff       (20)    13402 2023-06-28 15:18:29.000000 hicpnewman-1.0.5/hicpnewman/config/config_default.json
+-rw-r--r--   0 abuisson   (502) staff       (20)     2297 2023-06-28 10:52:29.000000 hicpnewman-1.0.5/hicpnewman/config_manager.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     9475 2023-06-28 15:42:31.000000 hicpnewman-1.0.5/hicpnewman/hicpnewman_argparser.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     7441 2023-06-29 14:49:34.000000 hicpnewman-1.0.5/hicpnewman/hicpnewman_commands.py
+-rw-r--r--   0 abuisson   (502) staff       (20)     4330 2023-06-29 15:07:20.000000 hicpnewman-1.0.5/hicpnewman/hicpnewman_helpers.py
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.778711 hicpnewman-1.0.5/hicpnewman/templates/
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.786306 hicpnewman-1.0.5/hicpnewman/templates/aggregated/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396567 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/aggregated/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266944 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/aggregated/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263417 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/aggregated/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.790275 hicpnewman-1.0.5/hicpnewman/templates/full/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   396606 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/full/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   266948 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/full/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   263421 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/full/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.793548 hicpnewman-1.0.5/hicpnewman/templates/original/
+-rw-rw-r--   0 abuisson   (502) staff       (20)   392882 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/original/htmlreqres.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   252692 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/original/template-default-colored.hbs
+-rw-rw-r--   0 abuisson   (502) staff       (20)   253300 2023-06-28 09:52:05.000000 hicpnewman-1.0.5/hicpnewman/templates/original/template-default.hbs
+drwxr-xr-x   0 abuisson   (502) staff       (20)        0 2023-06-29 15:39:04.782251 hicpnewman-1.0.5/hicpnewman.egg-info/
+-rw-r--r--   0 abuisson   (502) staff       (20)      460 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/PKG-INFO
+-rw-r--r--   0 abuisson   (502) staff       (20)      954 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/SOURCES.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)        1 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/dependency_links.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       68 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/entry_points.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       24 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/requires.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       11 2023-06-29 15:39:04.000000 hicpnewman-1.0.5/hicpnewman.egg-info/top_level.txt
+-rw-r--r--   0 abuisson   (502) staff       (20)       38 2023-06-29 15:39:04.795207 hicpnewman-1.0.5/setup.cfg
+-rw-r--r--   0 abuisson   (502) staff       (20)     1038 2023-06-29 15:38:50.000000 hicpnewman-1.0.5/setup.py
```

### Comparing `hicpnewman-1.0.4/LICENSE.txt` & `hicpnewman-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/README.md` & `hicpnewman-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/config/config.json` & `hicpnewman-1.0.5/hicpnewman/config/config.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/config/config_backup.json` & `hicpnewman-1.0.5/hicpnewman/config/config_backup.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/config/config_default.json` & `hicpnewman-1.0.5/hicpnewman/config/config_default.json`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/config_manager.py` & `hicpnewman-1.0.5/hicpnewman/config_manager.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/hicpnewman_argparser.py` & `hicpnewman-1.0.5/hicpnewman/hicpnewman_argparser.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/hicpnewman_commands.py` & `hicpnewman-1.0.5/hicpnewman/hicpnewman_commands.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/hicpnewman_helpers.py` & `hicpnewman-1.0.5/hicpnewman/hicpnewman_helpers.py`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/aggregated/htmlreqres.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/aggregated/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/aggregated/template-default-colored.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/aggregated/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/aggregated/template-default.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/aggregated/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/full/htmlreqres.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/full/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/full/template-default-colored.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/full/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/full/template-default.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/full/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/original/htmlreqres.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/original/htmlreqres.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/original/template-default-colored.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/original/template-default-colored.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman/templates/original/template-default.hbs` & `hicpnewman-1.0.5/hicpnewman/templates/original/template-default.hbs`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/hicpnewman.egg-info/SOURCES.txt` & `hicpnewman-1.0.5/hicpnewman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hicpnewman-1.0.4/setup.py` & `hicpnewman-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,21 @@
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.9',
     ]
 
 # specify requirements of your package here
 REQUIREMENTS = [
+    'typing',
     'dataclasses_json'
 ]
   
 # calling the setup function 
 setup(name='hicpnewman',
-      version='1.0.4',
+      version='1.0.5',
       description='a newman collection runner for hicp',
       url='https://kms-solutions.net',
       author='Antoine Buisson',
       author_email='antoine.buisson@kmse-tech.com',
       packages = ['hicpnewman'],
       package_data={'hicpnewman': ['config/*', 'templates/aggregated/*', 'templates/full/*', 'templates/original/*']},
         entry_points ={
```

