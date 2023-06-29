# Comparing `tmp/activeconfigparser-0.9.0.0.tar.gz` & `tmp/activeconfigparser-0.9.0.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activeconfigparser-0.9.0.0.tar", max compression
+gzip compressed data, was "activeconfigparser-0.9.0.0a0.tar", max compression
```

## Comparing `activeconfigparser-0.9.0.0.tar` & `activeconfigparser-0.9.0.0a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    17773 2023-06-29 11:08:24.620970 activeconfigparser-0.9.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/LICENSE
--rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0/README.md
--rw-r--r--   0        0        0     1906 2023-06-29 11:15:03.320862 activeconfigparser-0.9.0.0/pyproject.toml
--rw-r--r--   0        0        0    75272 2023-06-29 09:53:50.912341 activeconfigparser-0.9.0.0/src/activeconfigparser/ActiveConfigParser.py
--rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0/src/activeconfigparser/HandlerParameters.py
--rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.0.0/src/activeconfigparser/__init__.py
--rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/__init__.py
--rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/common.py
--rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
--rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
--rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
--rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
--rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
--rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
--rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
--rw-r--r--   0        0        0    88870 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/test_ActiveConfigParser.py
--rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/test_HandlerParameters.py
--rw-r--r--   0        0        0     2511 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0/src/activeconfigparser/version.py
--rw-r--r--   0        0        0     5321 1970-01-01 00:00:00.000000 activeconfigparser-0.9.0.0/PKG-INFO
+-rw-r--r--   0        0        0    17773 2023-06-29 11:08:24.620970 activeconfigparser-0.9.0.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1732 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/LICENSE
+-rw-r--r--   0        0        0     3565 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0a0/README.md
+-rw-r--r--   0        0        0     1907 2023-06-29 11:09:54.430951 activeconfigparser-0.9.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0    75272 2023-06-29 09:53:50.912341 activeconfigparser-0.9.0.0a0/src/activeconfigparser/ActiveConfigParser.py
+-rw-r--r--   0        0        0     5186 2023-06-29 11:02:00.401110 activeconfigparser-0.9.0.0a0/src/activeconfigparser/HandlerParameters.py
+-rw-r--r--   0        0        0     2559 2023-06-28 01:15:21.993938 activeconfigparser-0.9.0.0a0/src/activeconfigparser/__init__.py
+-rw-r--r--   0        0        0      158 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/__init__.py
+-rw-r--r--   0        0        0     4416 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/common.py
+-rw-r--r--   0        0        0     3111 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini
+-rw-r--r--   0        0        0      373 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_badkeys.ini
+-rw-r--r--   0        0        0      183 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_default.ini
+-rw-r--r--   0        0        0      253 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_01.ini
+-rw-r--r--   0        0        0      451 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_02.ini
+-rw-r--r--   0        0        0      355 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03a.ini
+-rw-r--r--   0        0        0      409 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser_validation_03b.ini
+-rw-r--r--   0        0        0    88870 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_ActiveConfigParser.py
+-rw-r--r--   0        0        0     9706 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_HandlerParameters.py
+-rw-r--r--   0        0        0     2511 2023-06-26 03:08:47.049809 activeconfigparser-0.9.0.0a0/src/activeconfigparser/version.py
+-rw-r--r--   0        0        0     5323 1970-01-01 00:00:00.000000 activeconfigparser-0.9.0.0a0/PKG-INFO
```

### Comparing `activeconfigparser-0.9.0.0/CHANGELOG.md` & `activeconfigparser-0.9.0.0a0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/LICENSE` & `activeconfigparser-0.9.0.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/README.md` & `activeconfigparser-0.9.0.0a0/README.md`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/pyproject.toml` & `activeconfigparser-0.9.0.0a0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "activeconfigparser"
 description = "A tool that extends configparser to enable enhanced processing of .ini files."
-version = "0.9.0.0"
+version = "0.9.0.0a"
 license = "LICENSE"
 readme = "README.md"
 keywords = [
     "Utility",
     "Bash",
     "Configuration",
     "ActiveConfigParser",
```

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/ActiveConfigParser.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/ActiveConfigParser.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/HandlerParameters.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/__init__.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/__init__.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/common.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/common.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/config_test_activeconfigparser.ini`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/test_ActiveConfigParser.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_ActiveConfigParser.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/unittests/test_HandlerParameters.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/unittests/test_HandlerParameters.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/src/activeconfigparser/version.py` & `activeconfigparser-0.9.0.0a0/src/activeconfigparser/version.py`

 * *Files identical despite different names*

### Comparing `activeconfigparser-0.9.0.0/PKG-INFO` & `activeconfigparser-0.9.0.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activeconfigparser
-Version: 0.9.0.0
+Version: 0.9.0.0a0
 Summary: A tool that extends configparser to enable enhanced processing of .ini files.
 Home-page: https://gitlab.com/semantik-software/code/python/ActiveConfigParser
 License: LICENSE
 Keywords: Utility,Bash,Configuration,ActiveConfigParser,ConfigParser
 Author: William McLendon
 Author-email: Semantik-Code@outlook.com
 Maintainer: William McLendon
```

