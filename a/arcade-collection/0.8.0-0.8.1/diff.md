# Comparing `tmp/arcade_collection-0.8.0.tar.gz` & `tmp/arcade_collection-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcade_collection-0.8.0.tar", max compression
+gzip compressed data, was "arcade_collection-0.8.1.tar", max compression
```

## Comparing `arcade_collection-0.8.0.tar` & `arcade_collection-0.8.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1519 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/LICENSE
--rw-r--r--   0        0        0      748 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/README.md
--rw-r--r--   0        0        0     1854 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/src/arcade_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/src/arcade_collection/__main__.py
--rw-r--r--   0        0        0      592 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/src/arcade_collection/input/__init__.py
--rw-r--r--   0        0        0     6982 2023-04-04 21:38:27.087713 arcade_collection-0.8.0/src/arcade_collection/input/convert_to_cells_file.py
--rw-r--r--   0        0        0     2313 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/input/convert_to_locations_file.py
--rw-r--r--   0        0        0     2607 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/input/generate_setup_file.py
--rw-r--r--   0        0        0     2375 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/input/group_template_conditions.py
--rw-r--r--   0        0        0     2517 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/input/merge_region_samples.py
--rw-r--r--   0        0        0      916 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/__init__.py
--rw-r--r--   0        0        0     1015 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/convert_model_units.py
--rw-r--r--   0        0        0     2777 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/convert_to_images.py
--rw-r--r--   0        0        0     2682 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/convert_to_meshes.py
--rw-r--r--   0        0        0     3709 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/convert_to_simularium.py
--rw-r--r--   0        0        0      301 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/extract_tick_json.py
--rw-r--r--   0        0        0      308 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/get_location_voxels.py
--rw-r--r--   0        0        0      260 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/merge_parsed_results.py
--rw-r--r--   0        0        0     1457 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/parse_cells_file.py
--rw-r--r--   0        0        0     2103 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/output/parse_locations_file.py
--rw-r--r--   0        0        0        0 2023-04-04 21:38:27.091713 arcade_collection-0.8.0/src/arcade_collection/py.typed
--rw-r--r--   0        0        0     1465 1970-01-01 00:00:00.000000 arcade_collection-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2502 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/README.md
+-rw-r--r--   0        0        0     1870 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/__main__.py
+-rw-r--r--   0        0        0      592 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/input/__init__.py
+-rw-r--r--   0        0        0     6982 2023-06-29 21:02:53.041198 arcade_collection-0.8.1/src/arcade_collection/input/convert_to_cells_file.py
+-rw-r--r--   0        0        0     2313 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/convert_to_locations_file.py
+-rw-r--r--   0        0        0     2607 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/generate_setup_file.py
+-rw-r--r--   0        0        0     2375 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/group_template_conditions.py
+-rw-r--r--   0        0        0     2517 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/input/merge_region_samples.py
+-rw-r--r--   0        0        0      916 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/__init__.py
+-rw-r--r--   0        0        0     1015 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_model_units.py
+-rw-r--r--   0        0        0     2777 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_images.py
+-rw-r--r--   0        0        0     2682 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_meshes.py
+-rw-r--r--   0        0        0     3709 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/convert_to_simularium.py
+-rw-r--r--   0        0        0      301 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/extract_tick_json.py
+-rw-r--r--   0        0        0      308 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/get_location_voxels.py
+-rw-r--r--   0        0        0      260 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/merge_parsed_results.py
+-rw-r--r--   0        0        0     1457 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/parse_cells_file.py
+-rw-r--r--   0        0        0     2103 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/output/parse_locations_file.py
+-rw-r--r--   0        0        0        0 2023-06-29 21:02:53.045198 arcade_collection-0.8.1/src/arcade_collection/py.typed
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 arcade_collection-0.8.1/PKG-INFO
```

### Comparing `arcade_collection-0.8.0/LICENSE` & `arcade_collection-0.8.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Bagheri Lab
+Copyright (c) 2023, Bagheri Lab
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `arcade_collection-0.8.0/pyproject.toml` & `arcade_collection-0.8.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arcade-collection"
-version = "0.8.0"
+version = "0.8.1"
 description = "Collection of tasks for working with ARCADE."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -15,23 +15,24 @@
 pandas = "^1.5.3"
 scikit-image = "^0.19.3"
 simulariumio = "^1.7.0"
 
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

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/__init__.py` & `arcade_collection-0.8.1/src/arcade_collection/input/__init__.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/convert_to_cells_file.py` & `arcade_collection-0.8.1/src/arcade_collection/input/convert_to_cells_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/convert_to_locations_file.py` & `arcade_collection-0.8.1/src/arcade_collection/input/convert_to_locations_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/generate_setup_file.py` & `arcade_collection-0.8.1/src/arcade_collection/input/generate_setup_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/group_template_conditions.py` & `arcade_collection-0.8.1/src/arcade_collection/input/group_template_conditions.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/input/merge_region_samples.py` & `arcade_collection-0.8.1/src/arcade_collection/input/merge_region_samples.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/__init__.py` & `arcade_collection-0.8.1/src/arcade_collection/output/__init__.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/convert_model_units.py` & `arcade_collection-0.8.1/src/arcade_collection/output/convert_model_units.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/convert_to_images.py` & `arcade_collection-0.8.1/src/arcade_collection/output/convert_to_images.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/convert_to_meshes.py` & `arcade_collection-0.8.1/src/arcade_collection/output/convert_to_meshes.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/convert_to_simularium.py` & `arcade_collection-0.8.1/src/arcade_collection/output/convert_to_simularium.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/parse_cells_file.py` & `arcade_collection-0.8.1/src/arcade_collection/output/parse_cells_file.py`

 * *Files identical despite different names*

### Comparing `arcade_collection-0.8.0/src/arcade_collection/output/parse_locations_file.py` & `arcade_collection-0.8.1/src/arcade_collection/output/parse_locations_file.py`

 * *Files identical despite different names*

