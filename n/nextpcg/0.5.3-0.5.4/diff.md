# Comparing `tmp/nextpcg-0.5.3.tar.gz` & `tmp/nextpcg-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.3.tar", last modified: Thu Jun 29 08:41:33 2023, max compression
+gzip compressed data, was "nextpcg-0.5.4.tar", last modified: Thu Jun 29 08:50:36 2023, max compression
```

## Comparing `nextpcg-0.5.3.tar` & `nextpcg-0.5.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 08:41:33.471243 nextpcg-0.5.3/
--rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1344 2023-06-29 08:41:33.470242 nextpcg-0.5.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 08:41:33.437499 nextpcg-0.5.3/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1344 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      654 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 08:41:33.000000 nextpcg-0.5.3/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.3/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-06-29 08:41:33.465237 nextpcg-0.5.3/pypapi/
--rw-rw-rw-   0        0        0      749 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.3/pypapi/const.py
--rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/dson.py
--rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.3/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.3/pypapi/field.py
--rw-rw-rw-   0        0        0     1835 2023-06-01 07:22:33.000000 nextpcg-0.5.3/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.3/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.3/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.3/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.3/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.3/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.3/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.3/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.3/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-06-29 08:41:33.469241 nextpcg-0.5.3/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.3/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-06-29 08:41:33.471243 nextpcg-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2437 2023-06-29 08:41:23.000000 nextpcg-0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.990858 nextpcg-0.5.4/
+-rw-rw-rw-   0        0        0       91 2023-06-29 08:40:42.000000 nextpcg-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-29 08:50:36.989857 nextpcg-0.5.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.957828 nextpcg-0.5.4/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      654 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 08:50:36.000000 nextpcg-0.5.4/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.4/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.983851 nextpcg-0.5.4/pypapi/
+-rw-rw-rw-   0        0        0      713 2023-06-29 08:49:32.000000 nextpcg-0.5.4/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.4/pypapi/const.py
+-rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/dson.py
+-rw-rw-rw-   0        0        0    10186 2023-06-29 08:27:12.000000 nextpcg-0.5.4/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field.py
+-rw-rw-rw-   0        0        0     1835 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_heightfield.py
+-rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/field_texture.py
+-rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.4/pypapi/geo.py
+-rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/geo_heightfield.py
+-rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.4/pypapi/geo_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.4/pypapi/geo_texture.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.4/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 08:50:36.987855 nextpcg-0.5.4/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.4/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 08:50:36.990858 nextpcg-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-29 08:50:18.000000 nextpcg-0.5.4/setup.py
```

### Comparing `nextpcg-0.5.3/PKG-INFO` & `nextpcg-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.3
+Version: 0.5.4
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.3/nextpcg.egg-info/PKG-INFO` & `nextpcg-0.5.4/nextpcg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextpcg
-Version: 0.5.3
+Version: 0.5.4
 Summary: pypapi module in NextPCG
 Home-page: https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4
 Author: GenesisGroup
 Author-email: cheneyshen@tencent.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nextpcg-0.5.3/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.5.4/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/__init__.py` & `nextpcg-0.5.4/pypapi/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,12 +8,10 @@
 
 from .geo import GeoBase, save_output_file, write_attribs_to_file, add_custom_attributes
 from .geo_heightfield import HeightField, Volume
 from .geo_instanced_staticmesh import InstancedStaticMesh, InstanceNode
 
 from .macro import get_fun_name
 
-from .dispatch import Dispatcher
-
 from .dson import DsonManager, DsonBase, nextpcgmethod, DsonMetaInfo
 from .dson_create import create_dson_from_pda
 from . import plugin_protocol
```

### Comparing `nextpcg-0.5.3/pypapi/__main__.py` & `nextpcg-0.5.4/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/dson.py` & `nextpcg-0.5.4/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/dson_create.py` & `nextpcg-0.5.4/pypapi/dson_create.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/field.py` & `nextpcg-0.5.4/pypapi/field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/field_heightfield.py` & `nextpcg-0.5.4/pypapi/field_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/field_instanced_staticmesh.py` & `nextpcg-0.5.4/pypapi/field_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/field_texture.py` & `nextpcg-0.5.4/pypapi/field_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/geo.py` & `nextpcg-0.5.4/pypapi/geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/geo_heightfield.py` & `nextpcg-0.5.4/pypapi/geo_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/geo_instanced_staticmesh.py` & `nextpcg-0.5.4/pypapi/geo_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/geo_texture.py` & `nextpcg-0.5.4/pypapi/geo_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/meta_helper.py` & `nextpcg-0.5.4/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.4/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/pypapi/plugin_protocol.py` & `nextpcg-0.5.4/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.3/setup.py` & `nextpcg-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
     author='GenesisGroup',
-    version='0.5.3',
+    version='0.5.4',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced
```

