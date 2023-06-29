# Comparing `tmp/pyrdfsubset-0.0.2a0.tar.gz` & `tmp/pyrdfsubset-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdfsubset-0.0.2a0.tar", last modified: Thu Jun 29 11:24:44 2023, max compression
+gzip compressed data, was "pyrdfsubset-0.0.3.tar", last modified: Thu Jun 29 11:45:13 2023, max compression
```

## Comparing `pyrdfsubset-0.0.2a0.tar` & `pyrdfsubset-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:24:44.959914 pyrdfsubset-0.0.2a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-29 11:24:44.959914 pyrdfsubset-0.0.2a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:24:44.959914 pyrdfsubset-0.0.2a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:24:44.955914 pyrdfsubset-0.0.2a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:24:44.959914 pyrdfsubset-0.0.2a0/src/pyrdfsubset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-29 11:24:32.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset/rdfsubset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:24:44.959914 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 11:24:44.000000 pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/pyrdfsubset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/rdfsubset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/top_level.txt
```

### Comparing `pyrdfsubset-0.0.2a0/LICENSE` & `pyrdfsubset-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.0.2a0/PKG-INFO` & `pyrdfsubset-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.2a0
+Version: 0.0.3
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyrdfsubset-0.0.2a0/pyproject.toml` & `pyrdfsubset-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrdfsubset"
-version = "0.0.2a"
+version = "0.0.3"
 description = "Create RDF subsets based on ShEx constraints"
 readme = "README.md"
 authors = [{ name = "Andra Waagmeester", email = "andra@micelio.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["shex", "rdf", "subsets", "biohackathon"]
 dependencies = [
     "rdflib",
     "pyshex",
-    "io",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/micelio/PyRDFSubSet"
 
 [project.scripts]
```

### Comparing `pyrdfsubset-0.0.2a0/src/pyrdfsubset/rdfsubset.py` & `pyrdfsubset-0.0.3/src/pyrdfsubset/rdfsubset.py`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.0.2a0/src/pyrdfsubset.egg-info/PKG-INFO` & `pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.2a0
+Version: 0.0.3
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

