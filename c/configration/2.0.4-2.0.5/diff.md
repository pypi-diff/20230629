# Comparing `tmp/configration-2.0.4.tar.gz` & `tmp/configration-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.4.tar", last modified: Sun Jun 18 11:48:33 2023, max compression
+gzip compressed data, was "configration-2.0.5.tar", last modified: Thu Jun 29 10:59:40 2023, max compression
```

## Comparing `configration-2.0.4.tar` & `configration-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.4/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1121 2023-06-18 11:48:33.176785 configration-2.0.4/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.4/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.173452 configration-2.0.4/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.4/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 11:41:45.000000 configration-2.0.4/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.4/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2228 2023-06-09 11:25:05.000000 configration-2.0.4/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.4/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.4/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-18 11:40:32.000000 configration-2.0.4/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.176785 configration-2.0.4/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.4/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2852 2023-06-18 11:39:33.000000 configration-2.0.4/configration/tests/test_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      229 2023-06-18 11:34:14.000000 configration-2.0.4/configration/xxx.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 11:48:33.173452 configration-2.0.4/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1121 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      469 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-18 11:48:33.000000 configration-2.0.4/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 11:48:33.176785 configration-2.0.4/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.4/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.5/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1162 2023-06-29 10:59:40.925925 configration-2.0.5/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.5/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.5/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-29 10:57:45.000000 configration-2.0.5/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.5/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2631 2023-06-29 10:57:45.000000 configration-2.0.5/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.5/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-09 14:31:15.000000 configration-2.0.5/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2779 2023-06-18 11:40:32.000000 configration-2.0.5/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.5/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2909 2023-06-29 10:57:45.000000 configration-2.0.5/configration/tests/test_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      229 2023-06-18 11:34:14.000000 configration-2.0.5/configration/xxx.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-29 10:59:40.925925 configration-2.0.5/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1162 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      469 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-06-29 10:59:40.000000 configration-2.0.5/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-29 10:59:40.925925 configration-2.0.5/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.5/setup.py
```

### Comparing `configration-2.0.4/LICENSE.txt` & `configration-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.4/PKG-INFO` & `configration-2.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.4
+Version: 2.0.5
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -21,14 +20,19 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.5 29 Jun 2023
+
+1. Tests on json and Toml
+------
+
 Version 2.0.4 18 June 2023
 
 1. Invalid toml test corrected
 2. Add tomli to requirements.txt
 
 ------
 
@@ -68,9 +72,7 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `configration-2.0.4/configration/src/config.py` & `configration-2.0.5/configration/src/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Base class for config object for the application."""
 
 from termcolor import cprint
 import colorama
 
-from .constants import ERROR_COLOUR, CORRUPT_FILE_MSG, MISSING_ATTR_MSG, NOT_OF_TYPE_MSG
+from .constants import (ERROR_COLOUR, CORRUPT_FILE_MSG, MISSING_ATTR_MSG,
+                        NOT_OF_TYPE_MSG, FIELD, NOT_IN_DICT)
 
 colorama.init()
 
+MODULE_COLOUR = 'red'
+
 
 class Config():
     """
     The class takes a path to a json file and if valid, returns a config dict.
 
     Attributes
     ----------
@@ -65,7 +68,15 @@
             if name not in config:
                 cprint(f"{CORRUPT_FILE_MSG} {MISSING_ATTR_MSG} {name}", ERROR_COLOUR)
                 return False
             if type(config[name]) not in item_types:
                 cprint(f"{CORRUPT_FILE_MSG} {name} {NOT_OF_TYPE_MSG} {item_types}", ERROR_COLOUR)
                 return False
         return True
+
+    def update(self, field: str, value: object, force: bool = False) -> None:
+        """Update the value of an attribute in config."""
+        if not force and field not in self.__dict__['config']:
+            cprint(f"{FIELD} {field} {NOT_IN_DICT}", ERROR_COLOUR)
+            return
+
+        self.__dict__['config'][field] = value
```

### Comparing `configration-2.0.4/configration/src/json_config.py` & `configration-2.0.5/configration/src/json_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.4/configration/src/toml_config.py` & `configration-2.0.5/configration/src/toml_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.4/configration/tests/test_config.py` & `configration-2.0.5/configration/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,7 +73,12 @@
         pass
     config = config_class(path, CONFIG_ATTRS, create=True)
     assert isinstance(config.config, dict)
     assert isinstance(config.month, int)
     assert isinstance(config.payment, float)
     assert isinstance(config.transactions, list)
     assert len(config.config) == 3
+
+
+def test_update_config():
+    # TODO add tests
+    ...
```

### Comparing `configration-2.0.4/configration.egg-info/PKG-INFO` & `configration-2.0.5/configration.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.4
+Version: 2.0.5
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -21,14 +20,19 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.5 29 Jun 2023
+
+1. Tests on json and Toml
+------
+
 Version 2.0.4 18 June 2023
 
 1. Invalid toml test corrected
 2. Add tomli to requirements.txt
 
 ------
 
@@ -68,9 +72,7 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `configration-2.0.4/setup.py` & `configration-2.0.5/setup.py`

 * *Files identical despite different names*

