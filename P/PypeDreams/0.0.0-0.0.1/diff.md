# Comparing `tmp/PypeDreams-0.0.0.tar.gz` & `tmp/PypeDreams-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PypeDreams-0.0.0.tar", last modified: Thu Jun 29 20:57:25 2023, max compression
+gzip compressed data, was "PypeDreams-0.0.1.tar", last modified: Thu Jun 29 21:01:19 2023, max compression
```

## Comparing `PypeDreams-0.0.0.tar` & `PypeDreams-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:57:25.208478 PypeDreams-0.0.0/
--rw-rw-rw-   0        0        0    11551 2023-06-29 15:48:37.000000 PypeDreams-0.0.0/LICENSE
--rw-rw-rw-   0        0        0    14448 2023-06-29 20:57:25.208478 PypeDreams-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      727 2023-06-29 20:10:05.000000 PypeDreams-0.0.0/README.md
--rw-rw-rw-   0        0        0      830 2023-06-29 20:57:03.000000 PypeDreams-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 20:57:25.208478 PypeDreams-0.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 20:57:25.175376 PypeDreams-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-29 20:57:25.186546 PypeDreams-0.0.0/src/PypeDreams/
--rw-rw-rw-   0        0        0      298 2023-06-29 20:08:14.000000 PypeDreams-0.0.0/src/PypeDreams/__init__.py
--rw-rw-rw-   0        0        0     3324 2023-06-29 17:55:09.000000 PypeDreams-0.0.0/src/PypeDreams/adjectives.py
--rw-rw-rw-   0        0        0     3383 2023-06-29 17:50:22.000000 PypeDreams-0.0.0/src/PypeDreams/animals.py
--rw-rw-rw-   0        0        0     3147 2023-06-29 18:43:43.000000 PypeDreams-0.0.0/src/PypeDreams/clothing.py
--rw-rw-rw-   0        0        0     3383 2023-06-29 15:48:37.000000 PypeDreams-0.0.0/src/PypeDreams/colors.py
--rw-rw-rw-   0        0        0      814 2023-06-29 15:48:37.000000 PypeDreams-0.0.0/src/PypeDreams/compress.py
--rw-rw-rw-   0        0        0     1451 2023-06-29 20:08:14.000000 PypeDreams-0.0.0/src/PypeDreams/pype_dreams.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:57:25.206178 PypeDreams-0.0.0/src/PypeDreams.egg-info/
--rw-rw-rw-   0        0        0    14448 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       44 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-29 20:57:25.000000 PypeDreams-0.0.0/src/PypeDreams.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 21:01:19.041883 PypeDreams-0.0.1/
+-rw-rw-rw-   0        0        0    11551 2023-06-29 15:48:37.000000 PypeDreams-0.0.1/LICENSE
+-rw-rw-rw-   0        0        0    14448 2023-06-29 21:01:19.040859 PypeDreams-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      727 2023-06-29 20:10:05.000000 PypeDreams-0.0.1/README.md
+-rw-rw-rw-   0        0        0      830 2023-06-29 21:00:49.000000 PypeDreams-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:01:19.041883 PypeDreams-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 21:01:19.001330 PypeDreams-0.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-29 21:01:19.015158 PypeDreams-0.0.1/src/PypeDreams/
+-rw-rw-rw-   0        0        0      298 2023-06-29 20:08:14.000000 PypeDreams-0.0.1/src/PypeDreams/__init__.py
+-rw-rw-rw-   0        0        0     3324 2023-06-29 17:55:09.000000 PypeDreams-0.0.1/src/PypeDreams/adjectives.py
+-rw-rw-rw-   0        0        0     3383 2023-06-29 17:50:22.000000 PypeDreams-0.0.1/src/PypeDreams/animals.py
+-rw-rw-rw-   0        0        0     3147 2023-06-29 18:43:43.000000 PypeDreams-0.0.1/src/PypeDreams/clothing.py
+-rw-rw-rw-   0        0        0     3383 2023-06-29 15:48:37.000000 PypeDreams-0.0.1/src/PypeDreams/colors.py
+-rw-rw-rw-   0        0        0      814 2023-06-29 15:48:37.000000 PypeDreams-0.0.1/src/PypeDreams/compress.py
+-rw-rw-rw-   0        0        0     1451 2023-06-29 20:08:14.000000 PypeDreams-0.0.1/src/PypeDreams/pype_dreams.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:01:19.039821 PypeDreams-0.0.1/src/PypeDreams.egg-info/
+-rw-rw-rw-   0        0        0    14448 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       44 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-29 21:01:18.000000 PypeDreams-0.0.1/src/PypeDreams.egg-info/top_level.txt
```

### Comparing `PypeDreams-0.0.0/LICENSE` & `PypeDreams-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/PKG-INFO` & `PypeDreams-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PypeDreams
-Version: 0.0.0
+Version: 0.0.1
 Summary: PypeDreams generates easy to remember animal-based hash digests
 Author-email: Huth S0lo <john@themorphium.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `PypeDreams-0.0.0/README.md` & `PypeDreams-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/pyproject.toml` & `PypeDreams-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PypeDreams"
-version = "0.0.0"
+version = "0.0.1"
 description = "PypeDreams generates easy to remember animal-based hash digests"
 readme = "README.md"
 authors = [{ name = "Huth S0lo", email = "john@themorphium.io" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
```

### Comparing `PypeDreams-0.0.0/src/PypeDreams/adjectives.py` & `PypeDreams-0.0.1/src/PypeDreams/adjectives.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams/animals.py` & `PypeDreams-0.0.1/src/PypeDreams/animals.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams/clothing.py` & `PypeDreams-0.0.1/src/PypeDreams/clothing.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams/colors.py` & `PypeDreams-0.0.1/src/PypeDreams/colors.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams/compress.py` & `PypeDreams-0.0.1/src/PypeDreams/compress.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams/pype_dreams.py` & `PypeDreams-0.0.1/src/PypeDreams/pype_dreams.py`

 * *Files identical despite different names*

### Comparing `PypeDreams-0.0.0/src/PypeDreams.egg-info/PKG-INFO` & `PypeDreams-0.0.1/src/PypeDreams.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PypeDreams
-Version: 0.0.0
+Version: 0.0.1
 Summary: PypeDreams generates easy to remember animal-based hash digests
 Author-email: Huth S0lo <john@themorphium.io>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

