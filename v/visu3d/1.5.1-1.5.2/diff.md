# Comparing `tmp/visu3d-1.5.1.tar.gz` & `tmp/visu3d-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visu3d-1.5.1.tar", last modified: Mon Mar 20 16:26:43 2023, max compression
+gzip compressed data, was "visu3d-1.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `visu3d-1.5.1.tar` & `visu3d-1.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2023-03-20 16:26:21.774883 visu3d-1.5.1/LICENSE
--rw-r--r--   0        0        0     4774 2023-03-20 16:26:21.774883 visu3d-1.5.1/README.md
--rw-r--r--   0        0        0     1868 2023-03-20 16:26:21.838883 visu3d-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     1811 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/__init__.py
--rw-r--r--   0        0        0     2257 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/array_dataclass.py
--rw-r--r--   0        0        0     7000 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/dc_arrays/camera.py
--rw-r--r--   0        0        0    13254 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/dc_arrays/camera_spec.py
--rw-r--r--   0        0        0     4890 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/dc_arrays/point.py
--rw-r--r--   0        0        0     4401 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/dc_arrays/ray.py
--rw-r--r--   0        0        0    17201 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/dc_arrays/transformation.py
--rw-r--r--   0        0        0     1301 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/math/__init__.py
--rw-r--r--   0        0        0     2980 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/math/coord_utils.py
--rw-r--r--   0        0        0     3523 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/math/interp_utils.py
--rw-r--r--   0        0        0     1259 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/math/math_utils.py
--rw-r--r--   0        0        0     7449 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/math/rotation_utils.py
--rw-r--r--   0        0        0     1245 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/plotly/__init__.py
--rw-r--r--   0        0        0     1674 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/plotly/auto_plot.py
--rw-r--r--   0        0        0     4054 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/plotly/fig_config_utils.py
--rw-r--r--   0        0        0    17401 2023-03-20 16:26:21.838883 visu3d-1.5.1/visu3d/plotly/fig_utils.py
--rw-r--r--   0        0        0     2018 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/plotly/traces_builder.py
--rw-r--r--   0        0        0      584 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/utils/__init__.py
--rw-r--r--   0        0        0      777 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/utils/file_utils.py
--rw-r--r--   0        0        0     1281 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/utils/lazy_imports.py
--rw-r--r--   0        0        0     3632 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/utils/np_utils.py
--rw-r--r--   0        0        0     2122 2023-03-20 16:26:21.842882 visu3d-1.5.1/visu3d/utils/py_utils.py
--rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 visu3d-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 09:54:22.492458 visu3d-1.5.2/LICENSE
+-rw-r--r--   0        0        0     4774 2023-06-29 09:54:22.492458 visu3d-1.5.2/README.md
+-rw-r--r--   0        0        0     1868 2023-06-29 09:54:22.548459 visu3d-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1811 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/__init__.py
+-rw-r--r--   0        0        0     2257 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/array_dataclass.py
+-rw-r--r--   0        0        0     7000 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/camera.py
+-rw-r--r--   0        0        0    13254 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/camera_spec.py
+-rw-r--r--   0        0        0     4890 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/point.py
+-rw-r--r--   0        0        0     4401 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/ray.py
+-rw-r--r--   0        0        0    17201 2023-06-29 09:54:22.548459 visu3d-1.5.2/visu3d/dc_arrays/transformation.py
+-rw-r--r--   0        0        0     1301 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/coord_utils.py
+-rw-r--r--   0        0        0     3523 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/interp_utils.py
+-rw-r--r--   0        0        0     1259 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/math_utils.py
+-rw-r--r--   0        0        0     7449 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/math/rotation_utils.py
+-rw-r--r--   0        0        0     1245 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/__init__.py
+-rw-r--r--   0        0        0     1674 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/auto_plot.py
+-rw-r--r--   0        0        0     4080 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/fig_config_utils.py
+-rw-r--r--   0        0        0    17401 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/fig_utils.py
+-rw-r--r--   0        0        0     2018 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/plotly/traces_builder.py
+-rw-r--r--   0        0        0      584 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/__init__.py
+-rw-r--r--   0        0        0      777 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/file_utils.py
+-rw-r--r--   0        0        0     1281 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/lazy_imports.py
+-rw-r--r--   0        0        0     3632 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/np_utils.py
+-rw-r--r--   0        0        0     2122 2023-06-29 09:54:22.552459 visu3d-1.5.2/visu3d/utils/py_utils.py
+-rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 visu3d-1.5.2/PKG-INFO
```

### Comparing `visu3d-1.5.1/LICENSE` & `visu3d-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.1/README.md` & `visu3d-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `visu3d-1.5.1/pyproject.toml` & `visu3d-1.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "visu3d"
 description = "3d geometry made easy."
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 authors = [{name = "Visu3d team", email="visu3d@google.com"}]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: Apache Software License",
     # Note: Python and license automatically added by some tools
```

### Comparing `visu3d-1.5.1/visu3d/__init__.py` & `visu3d-1.5.2/visu3d/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -45,8 +45,8 @@
 from visu3d.dc_arrays.transformation import custom_transform
 from visu3d.dc_arrays.transformation import Transform
 
 # Updating this will auto-trigger a release on PyPI and GitHub
 # Note:
 # * Make sure to also update the `CHANGELOG.md` before this.
 # * Make sure to also trigger an `etils` release
-__version__ = '1.5.1'
+__version__ = '1.5.2'
```

### Comparing `visu3d-1.5.1/visu3d/array_dataclass.py` & `visu3d-1.5.2/visu3d/array_dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/dc_arrays/camera.py` & `visu3d-1.5.2/visu3d/dc_arrays/camera.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/dc_arrays/camera_spec.py` & `visu3d-1.5.2/visu3d/dc_arrays/camera_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/dc_arrays/point.py` & `visu3d-1.5.2/visu3d/dc_arrays/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/dc_arrays/ray.py` & `visu3d-1.5.2/visu3d/dc_arrays/ray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/dc_arrays/transformation.py` & `visu3d-1.5.2/visu3d/dc_arrays/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/math/__init__.py` & `visu3d-1.5.2/visu3d/math/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/math/coord_utils.py` & `visu3d-1.5.2/visu3d/math/coord_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/math/interp_utils.py` & `visu3d-1.5.2/visu3d/math/interp_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/math/math_utils.py` & `visu3d-1.5.2/visu3d/math/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/math/rotation_utils.py` & `visu3d-1.5.2/visu3d/math/rotation_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/plotly/__init__.py` & `visu3d-1.5.2/visu3d/plotly/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/plotly/auto_plot.py` & `visu3d-1.5.2/visu3d/plotly/auto_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/plotly/fig_config_utils.py` & `visu3d-1.5.2/visu3d/plotly/fig_config_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -84,15 +84,17 @@
   name: Optional[str] = None
   num_samples: Optional[int] = None
 
   # Hidden reference to the global `fig_config`.
   # This allow to locally overwrite the default `fig_config`, like:
   # `v3d.make_fig(rays, num_samples_ray=None)`
   # This is used for the lazy values
-  _fig_config: FigConfig = dataclasses.field(default=fig_config, repr=False)
+  _fig_config: FigConfig = dataclasses.field(
+      default_factory=lambda: fig_config, repr=False
+  )
 
   if not typing.TYPE_CHECKING:
 
     def __getattribute__(self, name: str):
       # Auto-resolve lazy values
       value = super().__getattribute__(name)
       if isinstance(value, LazyValue):
```

### Comparing `visu3d-1.5.1/visu3d/plotly/fig_utils.py` & `visu3d-1.5.2/visu3d/plotly/fig_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/plotly/traces_builder.py` & `visu3d-1.5.2/visu3d/plotly/traces_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/utils/__init__.py` & `visu3d-1.5.2/visu3d/utils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/utils/file_utils.py` & `visu3d-1.5.2/visu3d/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/utils/lazy_imports.py` & `visu3d-1.5.2/visu3d/utils/lazy_imports.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/utils/np_utils.py` & `visu3d-1.5.2/visu3d/utils/np_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/visu3d/utils/py_utils.py` & `visu3d-1.5.2/visu3d/utils/py_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 The visu3d Authors.
+# Copyright 2023 The visu3d Authors.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `visu3d-1.5.1/PKG-INFO` & `visu3d-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: visu3d
-Version: 1.5.1
+Version: 1.5.2
 Summary: 3d geometry made easy.
 Keywords: 3d,visu3d,visualization,neural rendering,nerf
 Author-email: Visu3d team <visu3d@google.com>
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Visualization
```

