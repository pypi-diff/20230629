# Comparing `tmp/abm_colony_collection-0.3.2.tar.gz` & `tmp/abm_colony_collection-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_colony_collection-0.3.2.tar", max compression
+gzip compressed data, was "abm_colony_collection-0.3.3.tar", max compression
```

## Comparing `abm_colony_collection-0.3.2.tar` & `abm_colony_collection-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1519 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/LICENSE
--rw-r--r--   0        0        0      852 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/README.md
--rw-r--r--   0        0        0     1874 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1036 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/__main__.py
--rw-r--r--   0        0        0     1497 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_centrality_measures.py
--rw-r--r--   0        0        0     2320 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_cluster_distances.py
--rw-r--r--   0        0        0      831 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_cluster_sizes.py
--rw-r--r--   0        0        0      663 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_degree_measures.py
--rw-r--r--   0        0        0     1561 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_distance_measures.py
--rw-r--r--   0        0        0      561 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/convert_to_network.py
--rw-r--r--   0        0        0     1702 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/get_depth_map.py
--rw-r--r--   0        0        0     2590 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/get_neighbors_map.py
--rw-r--r--   0        0        0      918 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/make_voxels_array.py
--rw-r--r--   0        0        0        0 2023-03-30 19:21:39.106237 abm_colony_collection-0.3.2/src/abm_colony_collection/py.typed
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 abm_colony_collection-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-06-29 20:38:59.829201 abm_colony_collection-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2590 2023-06-29 20:38:59.829201 abm_colony_collection-0.3.3/README.md
+-rw-r--r--   0        0        0     1890 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1036 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/__main__.py
+-rw-r--r--   0        0        0     1497 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_centrality_measures.py
+-rw-r--r--   0        0        0     2320 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_cluster_distances.py
+-rw-r--r--   0        0        0      831 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_cluster_sizes.py
+-rw-r--r--   0        0        0      663 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_degree_measures.py
+-rw-r--r--   0        0        0     1561 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_distance_measures.py
+-rw-r--r--   0        0        0      561 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/convert_to_network.py
+-rw-r--r--   0        0        0     1702 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/get_depth_map.py
+-rw-r--r--   0        0        0     2590 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/get_neighbors_map.py
+-rw-r--r--   0        0        0      918 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/make_voxels_array.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:38:59.833201 abm_colony_collection-0.3.3/src/abm_colony_collection/py.typed
+-rw-r--r--   0        0        0     3347 1970-01-01 00:00:00.000000 abm_colony_collection-0.3.3/PKG-INFO
```

### Comparing `abm_colony_collection-0.3.2/LICENSE` & `abm_colony_collection-0.3.3/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Bagheri Lab
+Copyright (c) 2023, Allen Institute for Cell Science
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `abm_colony_collection-0.3.2/pyproject.toml` & `abm_colony_collection-0.3.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abm-colony-collection"
-version = "0.3.2"
+version = "0.3.3"
 description = "Collection of tasks for analyzing colony dynamics."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -16,23 +16,24 @@
 scipy = "^1.9.3"
 scikit-image = "^0.19.3"
 networkx = "^3.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
-mypy = "^0.991"
+mypy = "^1.3.0"
 pylint = "^2.16.2"
-pytest = "^7.2.0"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
-pytest-subtests = "^0.8.0"
-Sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.2.0"
-sphinx_mdinclude = "^0.5.3"
-tox = "^3.26.0"
+pytest-subtests = "^0.11.0"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
+myst-parser = "^2.0.0"
+sphinx-copybutton = "^0.5.2"
+tox = "^4.5.1"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/__init__.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_centrality_measures.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_centrality_measures.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_cluster_distances.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_cluster_distances.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_cluster_sizes.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_cluster_sizes.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_degree_measures.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_degree_measures.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/calculate_distance_measures.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/calculate_distance_measures.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/convert_to_network.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/convert_to_network.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/get_depth_map.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/get_depth_map.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/get_neighbors_map.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/get_neighbors_map.py`

 * *Files identical despite different names*

### Comparing `abm_colony_collection-0.3.2/src/abm_colony_collection/make_voxels_array.py` & `abm_colony_collection-0.3.3/src/abm_colony_collection/make_voxels_array.py`

 * *Files identical despite different names*

