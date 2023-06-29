# Comparing `tmp/abm_initialization_collection-0.5.0.tar.gz` & `tmp/abm_initialization_collection-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_initialization_collection-0.5.0.tar", max compression
+gzip compressed data, was "abm_initialization_collection-0.5.1.tar", max compression
```

## Comparing `abm_initialization_collection-0.5.0.tar` & `abm_initialization_collection-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1519 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/LICENSE
--rw-r--r--   0        0        0      916 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/README.md
--rw-r--r--   0        0        0     1964 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/__main__.py
--rw-r--r--   0        0        0      257 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/coordinate/__init__.py
--rw-r--r--   0        0        0      904 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
--rw-r--r--   0        0        0     3061 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
--rw-r--r--   0        0        0      411 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/__init__.py
--rw-r--r--   0        0        0     4099 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/create_voronoi_image.py
--rw-r--r--   0        0        0      407 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/get_image_bounds.py
--rw-r--r--   0        0        0     3181 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/plot_contact_sheet.py
--rw-r--r--   0        0        0     1131 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/select_fov_images.py
--rw-r--r--   0        0        0        0 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/py.typed
--rw-r--r--   0        0        0      778 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/__init__.py
--rw-r--r--   0        0        0      453 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/exclude_selected_ids.py
--rw-r--r--   0        0        0      715 2023-05-26 02:17:04.715932 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/get_image_samples.py
--rw-r--r--   0        0        0     2724 2023-05-26 02:17:04.719933 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/get_sample_indices.py
--rw-r--r--   0        0        0      449 2023-05-26 02:17:04.719933 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/include_selected_ids.py
--rw-r--r--   0        0        0     1812 2023-05-26 02:17:04.719933 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/remove_edge_regions.py
--rw-r--r--   0        0        0     6170 2023-05-26 02:17:04.719933 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py
--rw-r--r--   0        0        0     1453 2023-05-26 02:17:04.719933 abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 abm_initialization_collection-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-06-29 20:52:01.998432 abm_initialization_collection-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2739 2023-06-29 20:52:01.998432 abm_initialization_collection-0.5.1/README.md
+-rw-r--r--   0        0        0     1980 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/__main__.py
+-rw-r--r--   0        0        0      257 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/coordinate/__init__.py
+-rw-r--r--   0        0        0      904 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py
+-rw-r--r--   0        0        0     3061 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py
+-rw-r--r--   0        0        0      411 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/__init__.py
+-rw-r--r--   0        0        0     4099 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/create_voronoi_image.py
+-rw-r--r--   0        0        0      407 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/get_image_bounds.py
+-rw-r--r--   0        0        0     3181 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/plot_contact_sheet.py
+-rw-r--r--   0        0        0     1131 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/select_fov_images.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/py.typed
+-rw-r--r--   0        0        0      778 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/__init__.py
+-rw-r--r--   0        0        0      453 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/exclude_selected_ids.py
+-rw-r--r--   0        0        0      715 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/get_image_samples.py
+-rw-r--r--   0        0        0     2724 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/get_sample_indices.py
+-rw-r--r--   0        0        0      449 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/include_selected_ids.py
+-rw-r--r--   0        0        0     1812 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/remove_edge_regions.py
+-rw-r--r--   0        0        0     6170 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py
+-rw-r--r--   0        0        0     1453 2023-06-29 20:52:02.002432 abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py
+-rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 abm_initialization_collection-0.5.1/PKG-INFO
```

### Comparing `abm_initialization_collection-0.5.0/LICENSE` & `abm_initialization_collection-0.5.1/LICENSE`

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

### Comparing `abm_initialization_collection-0.5.0/pyproject.toml` & `abm_initialization_collection-0.5.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abm-initialization-collection"
-version = "0.5.0"
+version = "0.5.1"
 description = "Collection of tasks for initializing abm simulations."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -23,17 +23,18 @@
 black = "^22.12.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 pylint = "^2.16.2"
 pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
 pytest-subtests = "^0.11.0"
-sphinx = "^1.6.0"
-sphinx-rtd-theme = "^1.2.0"
-sphinx_mdinclude = "^0.5.3"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
+myst-parser = "^2.0.0"
+sphinx-copybutton = "^0.5.2"
 tox = "^4.5.1"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/coordinate/filter_coordinate_bounds.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/coordinate/make_grid_coordinates.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/coordinate/make_grid_coordinates.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/create_voronoi_image.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/create_voronoi_image.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/plot_contact_sheet.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/plot_contact_sheet.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/image/select_fov_images.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/image/select_fov_images.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/__init__.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/get_image_samples.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/get_image_samples.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/get_sample_indices.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/get_sample_indices.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/remove_edge_regions.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/remove_edge_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/remove_unconnected_regions.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/remove_unconnected_regions.py`

 * *Files identical despite different names*

### Comparing `abm_initialization_collection-0.5.0/src/abm_initialization_collection/sample/scale_sample_coordinates.py` & `abm_initialization_collection-0.5.1/src/abm_initialization_collection/sample/scale_sample_coordinates.py`

 * *Files identical despite different names*

