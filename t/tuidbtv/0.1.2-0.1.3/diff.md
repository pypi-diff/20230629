# Comparing `tmp/tuidbtv-0.1.2.tar.gz` & `tmp/tuidbtv-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuidbtv-0.1.2.tar", max compression
+gzip compressed data, was "tuidbtv-0.1.3.tar", max compression
```

## Comparing `tuidbtv-0.1.2.tar` & `tuidbtv-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1084 2023-06-27 17:22:14.783915 tuidbtv-0.1.2/LICENSE
--rw-r--r--   0        0        0      917 2023-06-29 20:38:42.296507 tuidbtv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      586 2023-06-29 20:45:18.516504 tuidbtv-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-27 17:29:23.492066 tuidbtv-0.1.2/tuidbtv/__init__.py
--rw-r--r--   0        0        0     2869 2023-06-29 00:27:37.312147 tuidbtv-0.1.2/tuidbtv/__main__.py
--rw-r--r--   0        0        0        0 2023-06-16 16:51:55.114223 tuidbtv-0.1.2/tuidbtv/config/__init__.py
--rw-r--r--   0        0        0     2366 2023-06-29 08:13:56.884461 tuidbtv-0.1.2/tuidbtv/config/ConfigParser.py
--rw-r--r--   0        0        0        0 2023-06-11 14:55:59.729538 tuidbtv-0.1.2/tuidbtv/controllers/__init__.py
--rw-r--r--   0        0        0      811 2023-06-28 23:21:03.594509 tuidbtv-0.1.2/tuidbtv/controllers/ControllerFactory.py
--rw-r--r--   0        0        0      472 2023-06-25 14:27:13.231327 tuidbtv-0.1.2/tuidbtv/controllers/DBController.py
--rw-r--r--   0        0        0     2447 2023-06-28 23:21:03.496526 tuidbtv-0.1.2/tuidbtv/controllers/MySQLController.py
--rw-r--r--   0        0        0     3117 2023-06-28 23:21:03.545522 tuidbtv-0.1.2/tuidbtv/controllers/PostgresController.py
--rw-r--r--   0        0        0     1429 2023-06-28 23:21:03.563518 tuidbtv-0.1.2/tuidbtv/controllers/SQLLiteController.py
--rw-r--r--   0        0        0     2808 2023-06-29 19:48:07.743714 tuidbtv-0.1.2/tuidbtv/default.css
--rw-r--r--   0        0        0      102 2023-06-26 16:04:15.427437 tuidbtv-0.1.2/tuidbtv/enums_and_variables/__init__.py
--rw-r--r--   0        0        0        0 2023-06-11 13:28:38.866786 tuidbtv-0.1.2/tuidbtv/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 12:40:36.587499 tuidbtv-0.1.2/tuidbtv/widgets/forms/__init__.py
--rw-r--r--   0        0        0     1704 2023-06-28 23:21:03.578504 tuidbtv-0.1.2/tuidbtv/widgets/forms/ConnectionForms.py
--rw-r--r--   0        0        0     3382 2023-06-29 19:03:01.527743 tuidbtv-0.1.2/tuidbtv/widgets/NewConnection.py
--rw-r--r--   0        0        0      612 2023-06-16 22:17:33.503450 tuidbtv-0.1.2/tuidbtv/widgets/PopUpScreen.py
--rw-r--r--   0        0        0      668 2023-06-11 14:32:32.205700 tuidbtv-0.1.2/tuidbtv/widgets/QuitScreen.py
--rw-r--r--   0        0        0     5706 2023-06-28 23:21:03.483540 tuidbtv-0.1.2/tuidbtv/widgets/SelectConnection.py
--rw-r--r--   0        0        0     1249 2023-06-28 23:21:03.466519 tuidbtv-0.1.2/tuidbtv/widgets/SQLEditor.py
--rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-06-27 17:22:14.783915 tuidbtv-0.1.3/LICENSE
+-rw-r--r--   0        0        0      917 2023-06-29 21:04:57.239599 tuidbtv-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      586 2023-06-29 20:45:18.516504 tuidbtv-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 17:29:23.492066 tuidbtv-0.1.3/tuidbtv/__init__.py
+-rw-r--r--   0        0        0     2869 2023-06-29 00:27:37.312147 tuidbtv-0.1.3/tuidbtv/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-16 16:51:55.114223 tuidbtv-0.1.3/tuidbtv/config/__init__.py
+-rw-r--r--   0        0        0     2366 2023-06-29 08:13:56.884461 tuidbtv-0.1.3/tuidbtv/config/ConfigParser.py
+-rw-r--r--   0        0        0        0 2023-06-11 14:55:59.729538 tuidbtv-0.1.3/tuidbtv/controllers/__init__.py
+-rw-r--r--   0        0        0      811 2023-06-28 23:21:03.594509 tuidbtv-0.1.3/tuidbtv/controllers/ControllerFactory.py
+-rw-r--r--   0        0        0      472 2023-06-25 14:27:13.231327 tuidbtv-0.1.3/tuidbtv/controllers/DBController.py
+-rw-r--r--   0        0        0     2447 2023-06-28 23:21:03.496526 tuidbtv-0.1.3/tuidbtv/controllers/MySQLController.py
+-rw-r--r--   0        0        0     3117 2023-06-28 23:21:03.545522 tuidbtv-0.1.3/tuidbtv/controllers/PostgresController.py
+-rw-r--r--   0        0        0     1429 2023-06-28 23:21:03.563518 tuidbtv-0.1.3/tuidbtv/controllers/SQLLiteController.py
+-rw-r--r--   0        0        0     2808 2023-06-29 19:48:07.743714 tuidbtv-0.1.3/tuidbtv/default.css
+-rw-r--r--   0        0        0      102 2023-06-26 16:04:15.427437 tuidbtv-0.1.3/tuidbtv/enums_and_variables/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-11 13:28:38.866786 tuidbtv-0.1.3/tuidbtv/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 12:40:36.587499 tuidbtv-0.1.3/tuidbtv/widgets/forms/__init__.py
+-rw-r--r--   0        0        0     1704 2023-06-28 23:21:03.578504 tuidbtv-0.1.3/tuidbtv/widgets/forms/ConnectionForms.py
+-rw-r--r--   0        0        0     3382 2023-06-29 19:03:01.527743 tuidbtv-0.1.3/tuidbtv/widgets/NewConnection.py
+-rw-r--r--   0        0        0      612 2023-06-16 22:17:33.503450 tuidbtv-0.1.3/tuidbtv/widgets/PopUpScreen.py
+-rw-r--r--   0        0        0      668 2023-06-11 14:32:32.205700 tuidbtv-0.1.3/tuidbtv/widgets/QuitScreen.py
+-rw-r--r--   0        0        0     5706 2023-06-28 23:21:03.483540 tuidbtv-0.1.3/tuidbtv/widgets/SelectConnection.py
+-rw-r--r--   0        0        0     1249 2023-06-28 23:21:03.466519 tuidbtv-0.1.3/tuidbtv/widgets/SQLEditor.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 tuidbtv-0.1.3/PKG-INFO
```

### Comparing `tuidbtv-0.1.2/LICENSE` & `tuidbtv-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/pyproject.toml` & `tuidbtv-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuidbtv"
-version = "0.1.2"
+version = "0.1.3"
 description = "console database client"
 authors = ["lakdemon"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/lakdemon/TUIDBTV"
 classifiers = [
     "Environment :: Console",
```

### Comparing `tuidbtv-0.1.2/README.md` & `tuidbtv-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/__main__.py` & `tuidbtv-0.1.3/tuidbtv/__main__.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/config/ConfigParser.py` & `tuidbtv-0.1.3/tuidbtv/config/ConfigParser.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/controllers/ControllerFactory.py` & `tuidbtv-0.1.3/tuidbtv/controllers/ControllerFactory.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/controllers/MySQLController.py` & `tuidbtv-0.1.3/tuidbtv/controllers/MySQLController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/controllers/PostgresController.py` & `tuidbtv-0.1.3/tuidbtv/controllers/PostgresController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/controllers/SQLLiteController.py` & `tuidbtv-0.1.3/tuidbtv/controllers/SQLLiteController.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/default.css` & `tuidbtv-0.1.3/tuidbtv/default.css`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/forms/ConnectionForms.py` & `tuidbtv-0.1.3/tuidbtv/widgets/forms/ConnectionForms.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/NewConnection.py` & `tuidbtv-0.1.3/tuidbtv/widgets/NewConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/PopUpScreen.py` & `tuidbtv-0.1.3/tuidbtv/widgets/PopUpScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/QuitScreen.py` & `tuidbtv-0.1.3/tuidbtv/widgets/QuitScreen.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/SelectConnection.py` & `tuidbtv-0.1.3/tuidbtv/widgets/SelectConnection.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/tuidbtv/widgets/SQLEditor.py` & `tuidbtv-0.1.3/tuidbtv/widgets/SQLEditor.py`

 * *Files identical despite different names*

### Comparing `tuidbtv-0.1.2/PKG-INFO` & `tuidbtv-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuidbtv
-Version: 0.1.2
+Version: 0.1.3
 Summary: console database client
 Home-page: https://github.com/lakdemon/TUIDBTV
 License: MIT
 Author: lakdemon
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

