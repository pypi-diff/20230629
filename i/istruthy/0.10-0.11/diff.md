# Comparing `tmp/istruthy-0.10.tar.gz` & `tmp/istruthy-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istruthy-0.10.tar", last modified: Thu Jun 29 20:00:39 2023, max compression
+gzip compressed data, was "istruthy-0.11.tar", last modified: Thu Jun 29 20:04:35 2023, max compression
```

## Comparing `istruthy-0.10.tar` & `istruthy-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:39.319078 istruthy-0.10/
--rw-rw-rw-   0        0        0     1148 2023-06-29 20:00:34.000000 istruthy-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0       95 2023-06-29 20:00:33.000000 istruthy-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     6943 2023-06-29 20:00:39.319078 istruthy-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     6220 2023-06-29 19:57:09.000000 istruthy-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:39.312096 istruthy-0.10/istruthy/
--rw-rw-rw-   0        0        0     6220 2023-06-29 19:57:09.000000 istruthy-0.10/istruthy/README.MD
--rw-rw-rw-   0        0        0      949 2023-06-29 19:56:27.000000 istruthy-0.10/istruthy/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-29 20:00:38.000000 istruthy-0.10/istruthy/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-06-29 20:00:38.000000 istruthy-0.10/istruthy/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-06-29 20:00:39.318081 istruthy-0.10/istruthy.egg-info/
--rw-rw-rw-   0        0        0     6943 2023-06-29 20:00:39.000000 istruthy-0.10/istruthy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-06-29 20:00:39.000000 istruthy-0.10/istruthy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:00:39.000000 istruthy-0.10/istruthy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 20:00:39.000000 istruthy-0.10/istruthy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-06-29 20:00:39.320075 istruthy-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-06-29 20:00:38.000000 istruthy-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.984889 istruthy-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-06-29 20:04:31.000000 istruthy-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0       95 2023-06-29 20:04:30.000000 istruthy-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     6942 2023-06-29 20:04:35.985887 istruthy-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     6219 2023-06-29 20:04:09.000000 istruthy-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.981897 istruthy-0.11/istruthy/
+-rw-rw-rw-   0        0        0     6219 2023-06-29 20:04:09.000000 istruthy-0.11/istruthy/README.MD
+-rw-rw-rw-   0        0        0      949 2023-06-29 19:56:27.000000 istruthy-0.11/istruthy/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-06-29 20:04:35.984889 istruthy-0.11/istruthy.egg-info/
+-rw-rw-rw-   0        0        0     6942 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-29 20:04:35.000000 istruthy-0.11/istruthy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-06-29 20:04:35.985887 istruthy-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-06-29 20:04:35.000000 istruthy-0.11/setup.py
```

### Comparing `istruthy-0.10/LICENSE.rst` & `istruthy-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `istruthy-0.10/PKG-INFO` & `istruthy-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istruthy
-Version: 0.10
+Version: 0.11
 Summary: extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 Home-page: https://github.com/hansalemaos/istruthy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,pandas,truthy,falsy
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 
-## pip install istruthty
+## pip install istruthy
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 ```python
 
     Args:
         x: A value of any type.
```

### Comparing `istruthy-0.10/README.md` & `istruthy-0.11/README.md`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 # extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 
-## pip install istruthty
+## pip install istruthy
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 ```python
 
     Args:
         x: A value of any type.
```

### Comparing `istruthy-0.10/istruthy/README.MD` & `istruthy-0.11/istruthy/README.MD`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 # extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 
-## pip install istruthty
+## pip install istruthy
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 ```python
 
     Args:
         x: A value of any type.
```

### Comparing `istruthy-0.10/istruthy/__init__.py` & `istruthy-0.11/istruthy/__init__.py`

 * *Files identical despite different names*

### Comparing `istruthy-0.10/istruthy.egg-info/PKG-INFO` & `istruthy-0.11/istruthy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: istruthy
-Version: 0.10
+Version: 0.11
 Summary: extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 Home-page: https://github.com/hansalemaos/istruthy
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: numpy,pandas,truthy,falsy
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,15 @@
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
 # extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays
 
-## pip install istruthty
+## pip install istruthy
 
 #### Tested against Windows 10 / Python 3.10 / Anaconda
 ```python
 
     Args:
         x: A value of any type.
```

### Comparing `istruthy-0.10/setup.py` & `istruthy-0.11/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''extends the capability of truthiness evaluation beyond the standard Python truthiness rules to handle pandas DataFrames/Series and NumPy Arrays'''
 
 # Setting up
 setup(
     name="istruthy",
     version=VERSION,
     license='MIT',
```

