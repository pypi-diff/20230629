# Comparing `tmp/pixelsparser-2.0.0.tar.gz` & `tmp/pixelsparser-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelsparser-2.0.0.tar", last modified: Thu Jun 29 10:57:43 2023, max compression
+gzip compressed data, was "pixelsparser-2.0.1.tar", last modified: Thu Jun 29 11:50:07 2023, max compression
```

## Comparing `pixelsparser-2.0.0.tar` & `pixelsparser-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/src/pixelsparser/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/src/pixelsparser/Pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/src/pixelsparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 10:57:29.000000 pixelsparser-2.0.0/src/pixelsparser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:57:43.428546 pixelsparser-2.0.0/src/pixelsparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-29 10:57:43.000000 pixelsparser-2.0.0/src/pixelsparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-29 10:57:43.000000 pixelsparser-2.0.0/src/pixelsparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:57:43.000000 pixelsparser-2.0.0/src/pixelsparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 10:57:43.000000 pixelsparser-2.0.0/src/pixelsparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/src/pixelsparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/src/pixelsparser/Pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/src/pixelsparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/src/pixelsparser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/src/pixelsparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-29 11:50:07.000000 pixelsparser-2.0.1/src/pixelsparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-29 11:50:07.000000 pixelsparser-2.0.1/src/pixelsparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:50:07.000000 pixelsparser-2.0.1/src/pixelsparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:50:07.000000 pixelsparser-2.0.1/src/pixelsparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:50:07.748184 pixelsparser-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/tests/test_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-29 11:49:50.000000 pixelsparser-2.0.1/tests/test_utils.py
```

### Comparing `pixelsparser-2.0.0/LICENSE` & `pixelsparser-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelsparser-2.0.0/PKG-INFO` & `pixelsparser-2.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelsparser
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python library that allows users to import their Pixels JSON data and use it in their python scripts.
 Author-email: Constantinos Psomadakis <business@tinosps.com>
 Project-URL: Homepage, https://github.com/pTinosq/pixelsparser/
 Project-URL: Bug Tracker, https://github.com/pTinosq/pixelsparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pixelsparser-2.0.0/README.md` & `pixelsparser-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pixelsparser-2.0.0/pyproject.toml` & `pixelsparser-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pixelsparser"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{ name = "Constantinos Psomadakis", email = "business@tinosps.com" }]
 description = "A python library that allows users to import their Pixels JSON data and use it in their python scripts."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `pixelsparser-2.0.0/src/pixelsparser/Pixel.py` & `pixelsparser-2.0.1/src/pixelsparser/Pixel.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,29 @@
     scores -- list of scores
     notes -- notes of the pixel
     tags -- list of tag categories
 
     Return: Pixel object
     """
 
-    def __init__(self, date: datetime, type: str, scores: list, notes: str, tags: list):
+    def __init__(self, date: str, type: str, scores: list, notes: str,
+                 tags: list):
         self.date = datetime.strptime(date, "%Y-%m-%d")
         self.pixelType = type
         self.notes = notes
         self.tags = tags
 
         # Multiple scores not yet implemented in the app
         self.scores = scores
         self.score = scores[0]
         self.mood = scores[0]
 
-
     def __str__(self):
-        return f"Pixel(date={self.date}, type={self.pixelType}, score={self.score}, mood={self.mood}, notes={self.notes}, tags={self.tags})"
+        return f"Pixel(date={self.date}, type={self.pixelType}," \
+                f"score={self.score}, mood={self.mood}, notes={self.notes}," \
+                f"tags={self.tags})"
 
     def __repr__(self):
         return self.__str__()
 
     def __eq__(self, other):
         return self.__dict__ == other.__dict__
```

### Comparing `pixelsparser-2.0.0/src/pixelsparser.egg-info/PKG-INFO` & `pixelsparser-2.0.1/src/pixelsparser.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pixelsparser
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python library that allows users to import their Pixels JSON data and use it in their python scripts.
 Author-email: Constantinos Psomadakis <business@tinosps.com>
 Project-URL: Homepage, https://github.com/pTinosq/pixelsparser/
 Project-URL: Bug Tracker, https://github.com/pTinosq/pixelsparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

