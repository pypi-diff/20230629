# Comparing `tmp/openapi3-1.8.0.tar.gz` & `tmp/openapi3-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openapi3-1.8.0.tar", last modified: Fri May 26 17:44:28 2023, max compression
+gzip compressed data, was "dist/openapi3-1.8.1.tar", last modified: Thu Jun 29 20:28:50 2023, max compression
```

## Comparing `openapi3-1.8.0.tar` & `openapi3-1.8.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.102370 openapi3-1.8.0/
--rw-r--r--   0 wsmith     (501) staff       (20)     1484 2020-12-11 20:20:15.000000 openapi3-1.8.0/LICENSE
--rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-05-26 17:44:28.102080 openapi3-1.8.0/PKG-INFO
--rw-r--r--   0 wsmith     (501) staff       (20)     2707 2023-05-25 12:30:25.000000 openapi3-1.8.0/README.rst
-drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.099468 openapi3-1.8.0/openapi3/
--rw-r--r--   0 wsmith     (501) staff       (20)      437 2022-03-09 16:00:00.000000 openapi3-1.8.0/openapi3/__init__.py
--rw-r--r--   0 wsmith     (501) staff       (20)      541 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/__main__.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1531 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/components.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1818 2022-03-09 16:00:00.000000 openapi3-1.8.0/openapi3/errors.py
--rw-r--r--   0 wsmith     (501) staff       (20)      672 2022-03-08 20:37:40.000000 openapi3-1.8.0/openapi3/example.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1718 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/general.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1803 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/info.py
--rw-r--r--   0 wsmith     (501) staff       (20)    27370 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/object_base.py
--rw-r--r--   0 wsmith     (501) staff       (20)     9324 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/openapi.py
--rw-r--r--   0 wsmith     (501) staff       (20)    19211 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/paths.py
--rw-r--r--   0 wsmith     (501) staff       (20)    11096 2023-05-26 17:39:29.000000 openapi3-1.8.0/openapi3/schemas.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1026 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/security.py
--rw-r--r--   0 wsmith     (501) staff       (20)     1169 2022-01-10 18:30:07.000000 openapi3-1.8.0/openapi3/servers.py
--rw-r--r--   0 wsmith     (501) staff       (20)      610 2023-03-17 12:43:51.000000 openapi3-1.8.0/openapi3/tag.py
-drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-05-26 17:44:28.101615 openapi3-1.8.0/openapi3.egg-info/
--rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/PKG-INFO
--rw-r--r--   0 wsmith     (501) staff       (20)      466 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 wsmith     (501) staff       (20)        1 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 wsmith     (501) staff       (20)      118 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/requires.txt
--rw-r--r--   0 wsmith     (501) staff       (20)        9 2023-05-26 17:44:27.000000 openapi3-1.8.0/openapi3.egg-info/top_level.txt
--rw-r--r--   0 wsmith     (501) staff       (20)       38 2023-05-26 17:44:28.102473 openapi3-1.8.0/setup.cfg
--rwxr-xr-x   0 wsmith     (501) staff       (20)      777 2023-05-26 17:41:20.000000 openapi3-1.8.0/setup.py
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-06-29 20:28:50.298495 openapi3-1.8.1/
+-rw-r--r--   0 wsmith     (501) staff       (20)     1484 2020-12-11 20:20:15.000000 openapi3-1.8.1/LICENSE
+-rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-06-29 20:28:50.298162 openapi3-1.8.1/PKG-INFO
+-rw-r--r--   0 wsmith     (501) staff       (20)     2707 2023-05-25 12:30:25.000000 openapi3-1.8.1/README.rst
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-06-29 20:28:50.295387 openapi3-1.8.1/openapi3/
+-rw-r--r--   0 wsmith     (501) staff       (20)      437 2022-03-09 16:00:00.000000 openapi3-1.8.1/openapi3/__init__.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      541 2022-01-10 18:30:07.000000 openapi3-1.8.1/openapi3/__main__.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1531 2023-05-26 17:39:29.000000 openapi3-1.8.1/openapi3/components.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1818 2022-03-09 16:00:00.000000 openapi3-1.8.1/openapi3/errors.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      672 2022-03-08 20:37:40.000000 openapi3-1.8.1/openapi3/example.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1718 2023-05-26 17:39:29.000000 openapi3-1.8.1/openapi3/general.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1803 2023-03-17 12:43:51.000000 openapi3-1.8.1/openapi3/info.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    27370 2023-05-26 17:39:29.000000 openapi3-1.8.1/openapi3/object_base.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     9324 2023-05-26 17:39:29.000000 openapi3-1.8.1/openapi3/openapi.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    19211 2023-03-17 12:43:51.000000 openapi3-1.8.1/openapi3/paths.py
+-rw-r--r--   0 wsmith     (501) staff       (20)    11118 2023-06-29 20:25:43.000000 openapi3-1.8.1/openapi3/schemas.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1026 2022-01-10 18:30:07.000000 openapi3-1.8.1/openapi3/security.py
+-rw-r--r--   0 wsmith     (501) staff       (20)     1169 2022-01-10 18:30:07.000000 openapi3-1.8.1/openapi3/servers.py
+-rw-r--r--   0 wsmith     (501) staff       (20)      610 2023-03-17 12:43:51.000000 openapi3-1.8.1/openapi3/tag.py
+drwxr-xr-x   0 wsmith     (501) staff       (20)        0 2023-06-29 20:28:50.297651 openapi3-1.8.1/openapi3.egg-info/
+-rw-r--r--   0 wsmith     (501) staff       (20)     3633 2023-06-29 20:28:50.000000 openapi3-1.8.1/openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 wsmith     (501) staff       (20)      466 2023-06-29 20:28:50.000000 openapi3-1.8.1/openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)        1 2023-06-29 20:28:50.000000 openapi3-1.8.1/openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)      118 2023-06-29 20:28:50.000000 openapi3-1.8.1/openapi3.egg-info/requires.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)        9 2023-06-29 20:28:50.000000 openapi3-1.8.1/openapi3.egg-info/top_level.txt
+-rw-r--r--   0 wsmith     (501) staff       (20)       38 2023-06-29 20:28:50.298625 openapi3-1.8.1/setup.cfg
+-rwxr-xr-x   0 wsmith     (501) staff       (20)      777 2023-06-29 20:25:50.000000 openapi3-1.8.1/setup.py
```

### Comparing `openapi3-1.8.0/LICENSE` & `openapi3-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/PKG-INFO` & `openapi3-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3
-Version: 1.8.0
+Version: 1.8.1
 Summary: Client and Validator of OpenAPI 3 Specifications
 Home-page: https://github.com/dorthu/openapi3
 Author: dorthu
 License: BSD 3-Clause License
 Description: openapi3
         ========
```

### Comparing `openapi3-1.8.0/README.rst` & `openapi3-1.8.1/README.rst`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/__main__.py` & `openapi3-1.8.1/openapi3/__main__.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/components.py` & `openapi3-1.8.1/openapi3/components.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/errors.py` & `openapi3-1.8.1/openapi3/errors.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/example.py` & `openapi3-1.8.1/openapi3/example.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/general.py` & `openapi3-1.8.1/openapi3/general.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/info.py` & `openapi3-1.8.1/openapi3/info.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/object_base.py` & `openapi3-1.8.1/openapi3/object_base.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/openapi.py` & `openapi3-1.8.1/openapi3/openapi.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/paths.py` & `openapi3-1.8.1/openapi3/paths.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/schemas.py` & `openapi3-1.8.1/openapi3/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         "xml",
         "externalDocs",
         "example",
         "deprecated",
         "contentEncoding",
         "contentMediaType",
         "contentSchema",
+        "extensions",
         "_model_type",
         "_request_model_type",
         "_resolved_allOfs",
     ]
     required_fields = []
 
     def _parse_data(self):
```

### Comparing `openapi3-1.8.0/openapi3/security.py` & `openapi3-1.8.1/openapi3/security.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/servers.py` & `openapi3-1.8.1/openapi3/servers.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3/tag.py` & `openapi3-1.8.1/openapi3/tag.py`

 * *Files identical despite different names*

### Comparing `openapi3-1.8.0/openapi3.egg-info/PKG-INFO` & `openapi3-1.8.1/openapi3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapi3
-Version: 1.8.0
+Version: 1.8.1
 Summary: Client and Validator of OpenAPI 3 Specifications
 Home-page: https://github.com/dorthu/openapi3
 Author: dorthu
 License: BSD 3-Clause License
 Description: openapi3
         ========
```

### Comparing `openapi3-1.8.0/setup.py` & `openapi3-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # get the long description from the README.rst
 with open(path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="openapi3",
-    version="1.8.0",
+    version="1.8.1",
     description="Client and Validator of OpenAPI 3 Specifications",
     long_description=long_description,
     author="dorthu",
     url="https://github.com/dorthu/openapi3",
     packages=["openapi3"],
     license="BSD 3-Clause License",
     install_requires=["PyYaml", "requests"],
```

