# Comparing `tmp/pyrdfsubset-0.0.3.tar.gz` & `tmp/pyrdfsubset-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrdfsubset-0.0.3.tar", last modified: Thu Jun 29 11:45:13 2023, max compression
+gzip compressed data, was "pyrdfsubset-0.0.4.tar", last modified: Thu Jun 29 12:34:09 2023, max compression
```

## Comparing `pyrdfsubset-0.0.3.tar` & `pyrdfsubset-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/pyrdfsubset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-06-29 11:45:00.000000 pyrdfsubset-0.0.3/src/pyrdfsubset/rdfsubset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:45:13.785312 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 11:45:13.000000 pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/pyrdfsubset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-29 12:33:57.000000 pyrdfsubset-0.0.4/src/pyrdfsubset/rdfsubset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:34:09.216430 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 12:34:09.000000 pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/top_level.txt
```

### Comparing `pyrdfsubset-0.0.3/LICENSE` & `pyrdfsubset-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrdfsubset-0.0.3/PKG-INFO` & `pyrdfsubset-0.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyrdfsubset-0.0.3/pyproject.toml` & `pyrdfsubset-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyrdfsubset"
-version = "0.0.3"
+version = "0.0.4"
 description = "Create RDF subsets based on ShEx constraints"
 readme = "README.md"
 authors = [{ name = "Andra Waagmeester", email = "andra@micelio.be" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyrdfsubset-0.0.3/src/pyrdfsubset/rdfsubset.py` & `pyrdfsubset-0.0.4/src/pyrdfsubset/rdfsubset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from rdflib import Graph, URIRef
 from pyshex import ShExEvaluator
 import io
 
 def get_subset(shex, rdf, inputformat="turtle", outputformat="turtle", subsettype="open"):
-
     graph = Graph()
     graph.parse(data=rdf, format=inputformat)
 
     # Create a new RDF graph for storing the RDF subset
     new_graph = Graph()
 
     # ShEx validate
 
     results = ShExEvaluator().evaluate(rdf, shex)
     for r in results:
-        print(r)
         if r.result:
-            print(r.focus)
             # Define the URI for which you want to retrieve the outgoing arcs
             uri = URIRef(r.focus)
 
             # Construct a SPARQL query to retrieve the outgoing arcs of the given URI
             query = """
                 SELECT ?predicate ?object
                 WHERE {
```

### Comparing `pyrdfsubset-0.0.3/src/pyrdfsubset.egg-info/PKG-INFO` & `pyrdfsubset-0.0.4/src/pyrdfsubset.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrdfsubset
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create RDF subsets based on ShEx constraints
 Author-email: Andra Waagmeester <andra@micelio.be>
 License: MIT License
         
         Copyright (c) 2023 Micelio
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

