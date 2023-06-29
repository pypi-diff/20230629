# Comparing `tmp/telexy.mars-1.23.627.tar.gz` & `tmp/telexy.mars-1.23.629.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telexy.mars-1.23.627.tar", last modified: Tue Jun 27 16:37:03 2023, max compression
+gzip compressed data, was "telexy.mars-1.23.629.tar", last modified: Thu Jun 29 17:53:24 2023, max compression
```

## Comparing `telexy.mars-1.23.627.tar` & `telexy.mars-1.23.629.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 16:37:03.664072 telexy.mars-1.23.627/
--rw-rw-rw-   0        0        0     1076 2023-06-21 19:06:45.000000 telexy.mars-1.23.627/LICENSE.txt
--rw-rw-rw-   0        0        0      419 2023-06-27 16:37:03.664072 telexy.mars-1.23.627/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-06-21 19:13:15.000000 telexy.mars-1.23.627/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 16:37:03.651960 telexy.mars-1.23.627/mars/
--rw-rw-rw-   0        0        0       23 2023-06-21 19:06:45.000000 telexy.mars-1.23.627/mars/__init__.py
--rw-rw-rw-   0        0        0      939 2023-06-21 19:13:46.000000 telexy.mars-1.23.627/mars/__main__.py
--rw-rw-rw-   0        0        0     1863 2023-06-27 16:01:45.000000 telexy.mars-1.23.627/mars/registry.py
--rw-rw-rw-   0        0        0       42 2023-06-27 16:37:03.665073 telexy.mars-1.23.627/setup.cfg
--rw-rw-rw-   0        0        0     1337 2023-06-27 16:01:53.000000 telexy.mars-1.23.627/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-27 16:37:03.662071 telexy.mars-1.23.627/telexy.mars.egg-info/
--rw-rw-rw-   0        0        0      419 2023-06-27 16:37:03.000000 telexy.mars-1.23.627/telexy.mars.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-27 16:37:03.000000 telexy.mars-1.23.627/telexy.mars.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 16:37:03.000000 telexy.mars-1.23.627/telexy.mars.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-27 16:37:03.000000 telexy.mars-1.23.627/telexy.mars.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-27 16:37:03.000000 telexy.mars-1.23.627/telexy.mars.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 17:53:24.038529 telexy.mars-1.23.629/
+-rw-rw-rw-   0        0        0     1076 2023-06-21 19:06:45.000000 telexy.mars-1.23.629/LICENSE.txt
+-rw-rw-rw-   0        0        0      419 2023-06-29 17:53:24.036526 telexy.mars-1.23.629/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-06-21 19:13:15.000000 telexy.mars-1.23.629/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:53:24.025920 telexy.mars-1.23.629/mars/
+-rw-rw-rw-   0        0        0       46 2023-06-29 17:16:54.000000 telexy.mars-1.23.629/mars/__init__.py
+-rw-rw-rw-   0        0        0      961 2023-06-29 17:17:21.000000 telexy.mars-1.23.629/mars/__main__.py
+-rw-rw-rw-   0        0        0     1608 2023-06-29 17:51:25.000000 telexy.mars-1.23.629/mars/plugin.py
+-rw-rw-rw-   0        0        0     1700 2023-06-29 17:16:06.000000 telexy.mars-1.23.629/mars/registry.py
+-rw-rw-rw-   0        0        0       42 2023-06-29 17:53:24.038529 telexy.mars-1.23.629/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2023-06-29 17:51:57.000000 telexy.mars-1.23.629/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:53:24.034526 telexy.mars-1.23.629/telexy.mars.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-06-29 17:53:23.000000 telexy.mars-1.23.629/telexy.mars.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-29 17:53:23.000000 telexy.mars-1.23.629/telexy.mars.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:53:23.000000 telexy.mars-1.23.629/telexy.mars.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-29 17:53:23.000000 telexy.mars-1.23.629/telexy.mars.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-29 17:53:23.000000 telexy.mars-1.23.629/telexy.mars.egg-info/top_level.txt
```

### Comparing `telexy.mars-1.23.627/LICENSE.txt` & `telexy.mars-1.23.629/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `telexy.mars-1.23.627/mars/__main__.py` & `telexy.mars-1.23.629/mars/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import cherrypy
 from .registry import *
+from .plugin import *
 
 class Mars(object):
 
     def __init__(self, keys, values):
         for(key, value) in zip(keys, values):
             self.__dict__[key] = value
```

### Comparing `telexy.mars-1.23.627/mars/registry.py` & `telexy.mars-1.23.629/mars/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 import jsonpickle
 import os
 import importlib
 
-class MarsPluginBase(object):
-
-    def __init__(self):
-        """constructor"""
-
-    def configuration(self):
-        """get configuration"""
-        return {}
-
-
 class MarsApplicationRegistryPlugin(object):
     def __init__(self, name, appPath, nameSpace = None):
         """Application registration plugin"""
         self.name = name
         self.nameSpace = nameSpace
         self.applicationPath = appPath
```

### Comparing `telexy.mars-1.23.627/setup.py` & `telexy.mars-1.23.629/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="telexy.mars",                     # This is the name of the package
-    version="1.23.627",                        # The initial release version
+    version="1.23.629",                        # The initial release version
     author="Telexy",                     # Full name of the author
     author_email="support@telexy.com", # Full email of author
     description="Mars Inference server",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
```

