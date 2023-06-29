# Comparing `tmp/nextpcg-0.5.0.tar.gz` & `tmp/nextpcg-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextpcg-0.5.0.tar", last modified: Thu Apr 13 03:59:05 2023, max compression
+gzip compressed data, was "nextpcg-0.5.1.tar", last modified: Thu Jun 29 07:30:35 2023, max compression
```

## Comparing `nextpcg-0.5.0.tar` & `nextpcg-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 03:59:05.115725 nextpcg-0.5.0/
--rw-rw-rw-   0        0        0       72 2023-03-17 08:38:04.000000 nextpcg-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1321 2023-04-13 03:59:05.113729 nextpcg-0.5.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 03:59:05.037933 nextpcg-0.5.0/nextpcg.egg-info/
--rw-rw-rw-   0        0        0     1321 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 03:59:04.000000 nextpcg-0.5.0/nextpcg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-03-02 08:29:40.000000 nextpcg-0.5.0/nextpcg.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2023-04-13 03:59:05.103757 nextpcg-0.5.0/pypapi/
--rw-rw-rw-   0        0        0      749 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/__main__.py
--rw-rw-rw-   0        0        0      391 2023-04-11 03:30:49.000000 nextpcg-0.5.0/pypapi/const.py
--rw-rw-rw-   0        0        0     5482 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/dispatch.py
--rw-rw-rw-   0        0        0     2124 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/dson.py
--rw-rw-rw-   0        0        0     3061 2023-04-11 04:04:20.000000 nextpcg-0.5.0/pypapi/dson_create.py
--rw-rw-rw-   0        0        0    14387 2023-03-29 08:40:38.000000 nextpcg-0.5.0/pypapi/field.py
--rw-rw-rw-   0        0        0     1835 2023-02-20 07:01:34.000000 nextpcg-0.5.0/pypapi/field_heightfield.py
--rw-rw-rw-   0        0        0     1098 2023-03-28 09:08:32.000000 nextpcg-0.5.0/pypapi/field_instanced_staticmesh.py
--rw-rw-rw-   0        0        0     1060 2023-03-28 09:08:38.000000 nextpcg-0.5.0/pypapi/field_texture.py
--rw-rw-rw-   0        0        0     9095 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/geo.py
--rw-rw-rw-   0        0        0     9503 2023-02-20 07:01:34.000000 nextpcg-0.5.0/pypapi/geo_heightfield.py
--rw-rw-rw-   0        0        0     6603 2023-02-20 07:01:34.000000 nextpcg-0.5.0/pypapi/geo_instanced_staticmesh.py
--rw-rw-rw-   0        0        0    14047 2023-04-13 03:56:42.000000 nextpcg-0.5.0/pypapi/geo_texture.py
--rw-rw-rw-   0        0        0      160 2023-02-20 07:01:34.000000 nextpcg-0.5.0/pypapi/macro.py
--rw-rw-rw-   0        0        0      906 2023-02-20 07:01:34.000000 nextpcg-0.5.0/pypapi/meta_helper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 03:59:05.109746 nextpcg-0.5.0/pypapi/pantry/
--rw-rw-rw-   0        0        0      270 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/pantry/dson_config.yaml
--rw-rw-rw-   0        0        0     6520 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/pantry/dson_generator.py
--rw-rw-rw-   0        0        0     2300 2023-03-17 08:38:04.000000 nextpcg-0.5.0/pypapi/plugin_protocol.py
--rw-rw-rw-   0        0        0       42 2023-04-13 03:59:05.116722 nextpcg-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2435 2023-04-13 03:58:36.000000 nextpcg-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:30:35.845920 nextpcg-0.5.1/
+-rw-rw-rw-   0        0        0       72 2023-03-21 06:03:49.000000 nextpcg-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1344 2023-06-29 07:30:35.844919 nextpcg-0.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 07:30:35.808885 nextpcg-0.5.1/nextpcg.egg-info/
+-rw-rw-rw-   0        0        0     1344 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       45 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 07:30:35.000000 nextpcg-0.5.1/nextpcg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-10 06:19:04.000000 nextpcg-0.5.1/nextpcg.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-29 07:30:35.838914 nextpcg-0.5.1/pypapi/
+-rw-rw-rw-   0        0        0      749 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/__init__.py
+-rw-rw-rw-   0        0        0     2001 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/__main__.py
+-rw-rw-rw-   0        0        0      391 2023-04-17 03:32:23.000000 nextpcg-0.5.1/pypapi/const.py
+-rw-rw-rw-   0        0        0     6574 2023-06-01 09:07:56.000000 nextpcg-0.5.1/pypapi/dispatch.py
+-rw-rw-rw-   0        0        0     2124 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/dson.py
+-rw-rw-rw-   0        0        0     3061 2023-04-17 03:32:23.000000 nextpcg-0.5.1/pypapi/dson_create.py
+-rw-rw-rw-   0        0        0    14387 2023-06-01 07:22:33.000000 nextpcg-0.5.1/pypapi/field.py
+-rw-rw-rw-   0        0        0     1835 2023-06-01 07:22:33.000000 nextpcg-0.5.1/pypapi/field_heightfield.py
+-rw-rw-rw-   0        0        0     1098 2023-06-01 07:22:33.000000 nextpcg-0.5.1/pypapi/field_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0     1060 2023-06-01 07:22:33.000000 nextpcg-0.5.1/pypapi/field_texture.py
+-rw-rw-rw-   0        0        0     9095 2023-03-02 03:22:48.000000 nextpcg-0.5.1/pypapi/geo.py
+-rw-rw-rw-   0        0        0     9503 2023-02-10 06:47:34.000000 nextpcg-0.5.1/pypapi/geo_heightfield.py
+-rw-rw-rw-   0        0        0     6603 2023-06-01 07:22:33.000000 nextpcg-0.5.1/pypapi/geo_instanced_staticmesh.py
+-rw-rw-rw-   0        0        0    14047 2023-04-17 03:32:23.000000 nextpcg-0.5.1/pypapi/geo_texture.py
+-rw-rw-rw-   0        0        0      160 2023-02-10 06:47:34.000000 nextpcg-0.5.1/pypapi/macro.py
+-rw-rw-rw-   0        0        0      906 2023-02-10 06:47:34.000000 nextpcg-0.5.1/pypapi/meta_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-29 07:30:35.842917 nextpcg-0.5.1/pypapi/pantry/
+-rw-rw-rw-   0        0        0      270 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/pantry/dson_config.yaml
+-rw-rw-rw-   0        0        0     6520 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/pantry/dson_generator.py
+-rw-rw-rw-   0        0        0     2300 2023-03-21 06:03:49.000000 nextpcg-0.5.1/pypapi/plugin_protocol.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 07:30:35.845920 nextpcg-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2437 2023-06-29 07:22:19.000000 nextpcg-0.5.1/setup.py
```

### Comparing `nextpcg-0.5.0/nextpcg.egg-info/SOURCES.txt` & `nextpcg-0.5.1/nextpcg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/__init__.py` & `nextpcg-0.5.1/pypapi/__init__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/__main__.py` & `nextpcg-0.5.1/pypapi/__main__.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/dispatch.py` & `nextpcg-0.5.1/pypapi/dispatch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # -*- coding: utf-8 -*-
 """
 Author  : NextPCG
 """
 
+import os
 import logging
 from typing import Dict, List, Union, Tuple
 from .const import *
 from .field import FieldManager, Field, FieldDesc
 from .meta_helper import Singleton
 from .dson import DsonMetaInfo, DsonManager
 
+import common.nextpcg as nextpcg
+import server_cache
+
 
 class Dispatcher(metaclass=Singleton):
     def __init__(self):
         pass
 
     @staticmethod
     def prepare_inputs(inputs_json: Dict, field_desc: FieldDesc):
@@ -51,23 +55,29 @@
         """find function in mod and run it
 
         side effects: change json_data
         """
         # clear error info
         if 'error' in json_data:
             del json_data['error']
+
         # get raw compress
         raw_compress = False
         if 'raw_compress' in json_data:
             raw_compress = bool(json_data['raw_compress'])
+
         # get io mode
         io_mode = 1
         if 'io_mode' in json_data:
             io_mode = int(json_data['io_mode'])
 
+        # nextpcg admin report.
+        folder = os.path.basename(work_path)
+        user = json_data[nextpcg.pson_system_tag]['user']
+
         # create field_desc
         field_desc = FieldDesc(work_path, io_mode, raw_compress)
 
         # find dson class
         dson_meta_info = self.get_dson_meta_info(json_data)
         cls_name = dson_meta_info.cls_name
         if cls_name not in DsonManager().dsonMap:
@@ -82,50 +92,58 @@
                     if dson_inputs_tag in json_value:
                         inputs = self.prepare_inputs(json_value[dson_inputs_tag], field_desc)
                     logger.info("Finish handing inputs!")
                 except Exception as e:
                     json_error_data['Error_Tag'] = 'dispatcher handing inputs error'
                     json_error_data['Error_Info'] = str(e)
                     logger.exception(e)
+                    server_cache.send_nextpcg_admin_report(user, folder, json_error_data['Error_Tag'],
+                                                           json_error_data['Error_Info'], 'Cook Python Functions')
                     return
                 params = {}
                 try:
                     logger.info("Start handing params...")
                     if dson_params_tag in json_value:
                         params = self.prepare_params(json_value[dson_params_tag], field_desc)
                     logger.info("Start handing params!")
                 except Exception as e:
                     json_error_data['Error_Tag'] = 'dispatcher handing params error'
                     json_error_data['Error_Info'] = str(e)
                     logger.exception(e)
+                    server_cache.send_nextpcg_admin_report(user, folder, json_error_data['Error_Tag'],
+                                                           json_error_data['Error_Info'], 'Cook Python Functions')
                     return
                 results = None
                 try:
                     # exec function
                     logger.info("Start calling functions...")
                     func_name = json_key
                     func_name = func_name.split('.')[0]
                     func = mod.__dict__[func_name].__func__
                     results = func(*inputs, **params)
                     logger.info("Finish calling functions!")
                 except Exception as e:
                     json_error_data['Error_Tag'] = 'dispatcher error in running function'
                     json_error_data['Error_Info'] = str(e)
                     logger.exception("running function error")
+                    server_cache.send_nextpcg_admin_report(user, folder, json_error_data['Error_Tag'],
+                                                           json_error_data['Error_Info'], 'Cook Python Functions')
                     return
                 try:
                     # handing outputs
                     logger.info("Start handing outputs...")
                     if dson_outputs_tag in json_value:
                         self.prepare_outputs(json_value[dson_outputs_tag], results, field_desc)
                     logger.info("Finish handing outputs!")
                 except Exception as e:
                     json_error_data['Error_Tag'] = 'dispatcher error in handing outputs'
                     json_error_data['Error_Info'] = str(e)
                     logger.exception("error in handing outputs")
+                    server_cache.send_nextpcg_admin_report(user, folder, json_error_data['Error_Tag'],
+                                                           json_error_data['Error_Info'], 'Cook Python Functions')
                     return
 
     @staticmethod
     def get_dson_meta_info(json_data):
         return DsonMetaInfo.from_dson(json_data)
```

### Comparing `nextpcg-0.5.0/pypapi/dson.py` & `nextpcg-0.5.1/pypapi/dson.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/dson_create.py` & `nextpcg-0.5.1/pypapi/dson_create.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/field.py` & `nextpcg-0.5.1/pypapi/field.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/field_heightfield.py` & `nextpcg-0.5.1/pypapi/field_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/field_instanced_staticmesh.py` & `nextpcg-0.5.1/pypapi/field_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/field_texture.py` & `nextpcg-0.5.1/pypapi/field_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/geo.py` & `nextpcg-0.5.1/pypapi/geo.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/geo_heightfield.py` & `nextpcg-0.5.1/pypapi/geo_heightfield.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/geo_instanced_staticmesh.py` & `nextpcg-0.5.1/pypapi/geo_instanced_staticmesh.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/geo_texture.py` & `nextpcg-0.5.1/pypapi/geo_texture.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/meta_helper.py` & `nextpcg-0.5.1/pypapi/meta_helper.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/pantry/dson_generator.py` & `nextpcg-0.5.1/pypapi/pantry/dson_generator.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/pypapi/plugin_protocol.py` & `nextpcg-0.5.1/pypapi/plugin_protocol.py`

 * *Files identical despite different names*

### Comparing `nextpcg-0.5.0/setup.py` & `nextpcg-0.5.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='nextpcg',
-    author='IEGG',
-    version='0.5.0',
+    author='GenesisGroup',
+    version='0.5.1',
     license='MIT',
 
     description='pypapi module in NextPCG',
     long_description='''Create by AI: 
     The pypapi module in NextPCG is a powerful tool that allows users to create sophisticated programs and applications 
     with ease. It provides a comprehensive suite of features and commands that makes coding much simpler and faster. 
     With the help of this module, users can quickly and easily develop programs and applications with advanced 
     capabilities, such as natural language processing, artificial intelligence, and other complex tasks. 
     In addition, the pypapi module makes it easy to create programs and applications that are compatible with 
     different platforms and operating systems, ensuring that users can deploy their creations on a variety of platforms. 
     All in all, the pypapi module in NextPCG is a great tool for developers who want to quickly and easily create 
     complex applications.''',
     author_email='cheneyshen@tencent.com',
-    url='https://glacier-request-888.notion.site/Wiki-f2600ce902b743f3ac7a40322496390a',
+    url='https://nextpcg.notion.site/Wiki-384dc1d9d9f64306bd8774ff1138f618?pvs=4',
 
     # packages=setuptools.find_packages(exclude=["dson_test", "dson_generator", "dispatch"]),
     # packages=setuptools.find_packages(where=['pypapi']),
     packages=['pypapi', 'pypapi.pantry'],
     package_dir={'pypapi':'pypapi'},
     package_data={'pypapi.pantry':['*']},
```

