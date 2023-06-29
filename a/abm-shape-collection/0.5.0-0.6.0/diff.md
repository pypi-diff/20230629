# Comparing `tmp/abm_shape_collection-0.5.0.tar.gz` & `tmp/abm_shape_collection-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abm_shape_collection-0.5.0.tar", max compression
+gzip compressed data, was "abm_shape_collection-0.6.0.tar", max compression
```

## Comparing `abm_shape_collection-0.5.0.tar` & `abm_shape_collection-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     1519 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/LICENSE
--rw-r--r--   0        0        0      844 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/README.md
--rw-r--r--   0        0        0     1924 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      924 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/__main__.py
--rw-r--r--   0        0        0     2898 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_shape_stats.py
--rw-r--r--   0        0        0     2765 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_size_stats.py
--rw-r--r--   0        0        0     6161 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/compile_shape_modes.py
--rw-r--r--   0        0        0     3201 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/extract_shape_modes.py
--rw-r--r--   0        0        0      508 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/fit_pca_model.py
--rw-r--r--   0        0        0      430 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/get_shape_coefficients.py
--rw-r--r--   0        0        0      352 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/get_shape_properties.py
--rw-r--r--   0        0        0      942 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/make_voxels_array.py
--rw-r--r--   0        0        0     3648 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/merge_shape_modes.py
--rw-r--r--   0        0        0        0 2023-05-08 18:03:55.678392 abm_shape_collection-0.5.0/src/abm_shape_collection/py.typed
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 abm_shape_collection-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1540 2023-06-29 20:18:32.131239 abm_shape_collection-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2573 2023-06-29 20:18:32.131239 abm_shape_collection-0.6.0/README.md
+-rw-r--r--   0        0        0     1933 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1307 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/__main__.py
+-rw-r--r--   0        0        0     2898 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_shape_stats.py
+-rw-r--r--   0        0        0     2765 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_size_stats.py
+-rw-r--r--   0        0        0     6161 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/compile_shape_modes.py
+-rw-r--r--   0        0        0      383 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_array.py
+-rw-r--r--   0        0        0     1016 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_coeffs.py
+-rw-r--r--   0        0        0      576 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/construct_mesh_from_points.py
+-rw-r--r--   0        0        0     2506 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/extract_shape_modes.py
+-rw-r--r--   0        0        0      508 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/fit_pca_model.py
+-rw-r--r--   0        0        0      430 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/get_shape_coefficients.py
+-rw-r--r--   0        0        0      352 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/get_shape_properties.py
+-rw-r--r--   0        0        0      942 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/make_voxels_array.py
+-rw-r--r--   0        0        0     3648 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/merge_shape_modes.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:18:32.135239 abm_shape_collection-0.6.0/src/abm_shape_collection/py.typed
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 abm_shape_collection-0.6.0/PKG-INFO
```

### Comparing `abm_shape_collection-0.5.0/LICENSE` & `abm_shape_collection-0.6.0/LICENSE`

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

### Comparing `abm_shape_collection-0.5.0/pyproject.toml` & `abm_shape_collection-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "abm-shape-collection"
-version = "0.5.0"
+version = "0.6.0"
 description = "Collection of tasks for analyzing cell shapes."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -16,23 +16,24 @@
 aicsshparam = "^0.1.1"
 vtk = "^9.2.5"
 trimesh = "^3.18.3"
 
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
@@ -58,15 +59,15 @@
 module = [
     "aicsshparam.*",
     "pandas.*",
     "scipy.*",
     "skimage.*",
     "sklearn.*",
     "trimesh.*",
-    "vtkmodules.*",
+    "vtk.*",
 ]
 ignore_missing_imports = true
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = True
```

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_shape_stats.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_shape_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/calculate_size_stats.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/calculate_size_stats.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/compile_shape_modes.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/compile_shape_modes.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/extract_shape_modes.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/extract_shape_modes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import tempfile
 
 import numpy as np
 import pandas as pd
 import trimesh
-from aicsshparam import shtools
 from sklearn.decomposition import PCA
-from vtkmodules.vtkCommonDataModel import vtkPolyData
-from vtkmodules.vtkIOPLY import vtkPLYWriter
+from vtk import vtkPLYWriter, vtkPolyData
+
+from abm_shape_collection.construct_mesh_from_points import construct_mesh_from_points
 
 
 def extract_shape_modes(
     pca: PCA, data: pd.DataFrame, components: int, regions: list[str], order: int, delta: float
 ) -> dict:
     features = data.filter(like="shcoeffs").columns.values
     data_transform = pca.transform(data[features].values)
@@ -46,35 +46,14 @@
     suffix = f".{region}" if region != "DEFAULT" else ""
     mesh = construct_mesh_from_points(pca, vector, feature_names, order, prefix, suffix)
     mesh = convert_vtk_to_trimesh(mesh)
     slices = get_mesh_slices(mesh)
     return slices
 
 
-def construct_mesh_from_points(
-    pca: PCA,
-    points: np.ndarray,
-    feature_names: list[str],
-    order: int,
-    prefix: str = "",
-    suffix: str = "",
-) -> vtkPolyData:
-    """Constructs mesh given PCA transformation points."""
-    coeffs = pd.Series(pca.inverse_transform(points), index=feature_names)
-    coeffs_map = np.zeros((2, order + 1, order + 1), dtype=np.float32)
-
-    for l in range(order + 1):
-        for m in range(order + 1):
-            coeffs_map[0, l, m] = coeffs[f"{prefix}shcoeffs_L{l}M{m}C{suffix}"]
-            coeffs_map[1, l, m] = coeffs[f"{prefix}shcoeffs_L{l}M{m}S{suffix}"]
-
-    mesh, _ = shtools.get_reconstruction_from_coeffs(coeffs_map)
-    return mesh
-
-
 def convert_vtk_to_trimesh(mesh: vtkPolyData) -> trimesh.Trimesh:
     with tempfile.NamedTemporaryFile() as temp:
         writer = vtkPLYWriter()
         writer.SetInputData(mesh)
         writer.SetFileTypeToASCII()
         writer.SetFileName(f"{temp.name}.ply")
         _ = writer.Write()
```

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/make_voxels_array.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/make_voxels_array.py`

 * *Files identical despite different names*

### Comparing `abm_shape_collection-0.5.0/src/abm_shape_collection/merge_shape_modes.py` & `abm_shape_collection-0.6.0/src/abm_shape_collection/merge_shape_modes.py`

 * *Files identical despite different names*

