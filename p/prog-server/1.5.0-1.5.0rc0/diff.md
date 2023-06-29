# Comparing `tmp/prog_server-1.5.0.tar.gz` & `tmp/prog_server-1.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_server-1.5.0.tar", last modified: Thu Jun 29 15:36:40 2023, max compression
+gzip compressed data, was "prog_server-1.5.0rc0.tar", last modified: Thu Jun 29 15:29:23 2023, max compression
```

## Comparing `prog_server-1.5.0.tar` & `prog_server-1.5.0rc0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.009166 prog_server-1.5.0/
--rw-r--r--   0 cteubert   (507) staff       (20)     5984 2023-06-29 15:36:40.008987 prog_server-1.5.0/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     3990 2023-06-21 22:21:41.000000 prog_server-1.5.0/README.md
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-29 15:36:40.009204 prog_server-1.5.0/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2727 2023-06-29 15:33:40.000000 prog_server-1.5.0/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.005787 prog_server-1.5.0/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.006456 prog_server-1.5.0/src/prog_client/
--rw-r--r--   0 cteubert   (507) staff       (20)      211 2023-06-29 15:33:52.000000 prog_server-1.5.0/src/prog_client/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9298 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_client/session.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.006986 prog_server-1.5.0/src/prog_server/
--rw-r--r--   0 cteubert   (507) staff       (20)     1028 2023-06-29 15:33:55.000000 prog_server-1.5.0/src/prog_server/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      418 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/__main__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2370 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/app.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21604 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/controllers.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.008786 prog_server-1.5.0/src/prog_server/models/
--rw-r--r--   0 cteubert   (507) staff       (20)      159 2021-12-22 19:21:19.000000 prog_server-1.5.0/src/prog_server/models/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2405 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/models/load_ests.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1646 2022-01-18 16:47:38.000000 prog_server-1.5.0/src/prog_server/models/prediction_handler.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1811 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/models/prog_server.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5631 2023-06-20 20:26:30.000000 prog_server-1.5.0/src/prog_server/models/session.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:36:40.007701 prog_server-1.5.0/src/prog_server.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     5984 2023-06-29 15:36:40.000000 prog_server-1.5.0/src/prog_server.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)      565 2023-06-29 15:36:40.000000 prog_server-1.5.0/src/prog_server.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2023-06-29 15:36:40.000000 prog_server-1.5.0/src/prog_server.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)       33 2023-06-29 15:36:40.000000 prog_server-1.5.0/src/prog_server.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       24 2023-06-29 15:36:40.000000 prog_server-1.5.0/src/prog_server.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.762075 prog_server-1.5.0rc0/
+-rw-r--r--   0 cteubert   (507) staff       (20)     5987 2023-06-29 15:29:23.761921 prog_server-1.5.0rc0/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     3990 2023-06-21 22:21:41.000000 prog_server-1.5.0rc0/README.md
+-rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-29 15:29:23.762113 prog_server-1.5.0rc0/setup.cfg
+-rw-r--r--   0 cteubert   (507) staff       (20)     2731 2023-06-21 22:21:41.000000 prog_server-1.5.0rc0/setup.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.757111 prog_server-1.5.0rc0/src/
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.758117 prog_server-1.5.0rc0/src/prog_client/
+-rw-r--r--   0 cteubert   (507) staff       (20)      215 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_client/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     9298 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_client/session.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.759349 prog_server-1.5.0rc0/src/prog_server/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1033 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      418 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/__main__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2370 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/app.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    21604 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/controllers.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.761580 prog_server-1.5.0rc0/src/prog_server/models/
+-rw-r--r--   0 cteubert   (507) staff       (20)      159 2021-12-22 19:21:19.000000 prog_server-1.5.0rc0/src/prog_server/models/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2405 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/load_ests.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1646 2022-01-18 16:47:38.000000 prog_server-1.5.0rc0/src/prog_server/models/prediction_handler.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1811 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/prog_server.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5631 2023-06-20 20:26:30.000000 prog_server-1.5.0rc0/src/prog_server/models/session.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:29:23.760391 prog_server-1.5.0rc0/src/prog_server.egg-info/
+-rw-------   0 cteubert   (507) staff       (20)     5987 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/PKG-INFO
+-rw-------   0 cteubert   (507) staff       (20)      565 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/SOURCES.txt
+-rw-------   0 cteubert   (507) staff       (20)        1 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/dependency_links.txt
+-rw-------   0 cteubert   (507) staff       (20)       33 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/requires.txt
+-rw-------   0 cteubert   (507) staff       (20)       24 2023-06-29 15:29:23.000000 prog_server-1.5.0rc0/src/prog_server.egg-info/top_level.txt
```

### Comparing `prog_server-1.5.0/PKG-INFO` & `prog_server-1.5.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_server
-Version: 1.5.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures
 Home-page: https://nasa.github.com/progpy/prog_server_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_server/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_server_guide.html
```

### Comparing `prog_server-1.5.0/README.md` & `prog_server-1.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/setup.py` & `prog_server-1.5.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='prog_server',
-    version='1.5.0',
+    version='1.5.0-pre',
     description='The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://nasa.github.com/progpy/prog_server_guide.html',
     author='Christopher Teubert',
     author_email='christopher.a.teubert@nasa.gov',
     classifiers=[
```

### Comparing `prog_server-1.5.0/src/prog_client/session.py` & `prog_server-1.5.0rc0/src/prog_client/session.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/__init__.py` & `prog_server-1.5.0rc0/src/prog_server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the
 # National Aeronautics and Space Administration.  All Rights Reserved.
 
 from .models.prog_server import server
-__version__ = '1.5.0'
+
+__version__ = '1.5.0-pre'
 
 def run(**kwargs):
     """
     Start the server and block until it is stopped.
 
     Args:
         host (str, optional): Server host. Defaults to '127.0.0.1'.
```

### Comparing `prog_server-1.5.0/src/prog_server/app.py` & `prog_server-1.5.0rc0/src/prog_server/app.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/controllers.py` & `prog_server-1.5.0rc0/src/prog_server/controllers.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/models/load_ests.py` & `prog_server-1.5.0rc0/src/prog_server/models/load_ests.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/models/prediction_handler.py` & `prog_server-1.5.0rc0/src/prog_server/models/prediction_handler.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/models/prog_server.py` & `prog_server-1.5.0rc0/src/prog_server/models/prog_server.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server/models/session.py` & `prog_server-1.5.0rc0/src/prog_server/models/session.py`

 * *Files identical despite different names*

### Comparing `prog_server-1.5.0/src/prog_server.egg-info/PKG-INFO` & `prog_server-1.5.0rc0/src/prog_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-server
-Version: 1.5.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics As-A-Service (PaaS) Sandbox (a.k.a. prog_server) is a simplified Software Oriented Architecture (SOA) for performing prognostics of engineering systems. The PaaS Sandbox is a wrapper around the Prognostics Algorithms and Models Packages, allowing 1+ users to access these packages features through a REST API. The package is intended to be used as a research tool to prototype and benchmark Prognostics As-A-Service (PaaS) architectures and work on the challenges facing such architectures
 Home-page: https://nasa.github.com/progpy/prog_server_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_server/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_server_guide.html
```

### Comparing `prog_server-1.5.0/src/prog_server.egg-info/SOURCES.txt` & `prog_server-1.5.0rc0/src/prog_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

