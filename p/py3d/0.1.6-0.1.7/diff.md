# Comparing `tmp/py3d-0.1.6.tar.gz` & `tmp/py3d-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.1.6.tar", last modified: Thu Jun 22 04:01:25 2023, max compression
+gzip compressed data, was "py3d-0.1.7.tar", last modified: Thu Jun 29 14:23:12 2023, max compression
```

## Comparing `py3d-0.1.6.tar` & `py3d-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-22 04:01:25.459198 py3d-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-22 04:01:05.000000 py3d-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    29619 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-06-22 04:00:23.000000 py3d-0.1.6/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 04:01:25.459198 py3d-0.1.6/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 04:01:25.000000 py3d-0.1.6/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 04:01:25.459198 py3d-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-22 04:00:23.000000 py3d-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-29 14:23:12.246305 py3d-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-29 14:22:49.000000 py3d-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29856 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22693 2023-06-29 14:21:54.000000 py3d-0.1.7/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 14:23:12.246305 py3d-0.1.7/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-29 14:23:12.000000 py3d-0.1.7/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 14:23:12.246305 py3d-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-29 14:21:54.000000 py3d-0.1.7/setup.py
```

### Comparing `py3d-0.1.6/PKG-INFO` & `py3d-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.6
+Version: 0.1.7
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.6/README.md` & `py3d-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.1.6/py3d/core.py` & `py3d-0.1.7/py3d/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
 
 def label(text, position: list = [0, 0, 0], color="grey", t=0):
     return default_view.label(text, position, color, t)
 
 
 def show():
-    return default_view
+    return display(HTML(default_view._repr_html_()))
 
 
 def read_pcd(path):
     f = open(path, "rb")
     data_type = ""
     ret = []
     tp_map = {
@@ -247,23 +247,23 @@
 
     @property
     def M(self) -> Vector | Vector2 | Vector3 | Vector4:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
-    def L(self) -> Vector:
+    def L(self) -> numpy.ndarray:
         # length
-        return numpy.linalg.norm(self, axis=self.ndim - 1).view(Vector)
+        return numpy.linalg.norm(self, axis=self.ndim - 1)
 
-    def min(self) -> Vector:
-        return super().min(axis=self.ndim-2)
+    def min(self, axis=-2, keepdims=False) -> Vector:
+        return super().min(axis=axis, keepdims=keepdims)
 
-    def max(self) -> Vector:
-        return super().max(axis=self.ndim-2)
+    def max(self, axis=-2, keepdims=False) -> Vector:
+        return super().max(axis=axis, keepdims=keepdims)
 
     def diff(self, n=1) -> Vector:
         return numpy.diff(self, n, axis=self.ndim-2)
 
     def lerp(self, x, xp) -> Vector:
         '''
         linear interpolation
@@ -418,14 +418,17 @@
         d: Vector = (self[..., numpy.newaxis, :] - pts).L
         d = d.reshape(*d.shape[:-2], -1)
         idx = d.argmin(d.ndim-1)
         spts = sum(pts.n)
         idx0 = idx//spts
         idx1 = idx % spts
         return idx0, idx1
+    
+    def distance_to_points(self, points: Vector3) -> numpy.ndarray:
+        return (self[..., None, :] - points).L.min(axis=-1).mean()
 
     def as_scaling(self) -> Transform:
         ret = Transform
         ret[..., 0, 0] = self[..., 0]
         ret[..., 1, 1] = self[..., 1]
         ret[..., 2, 2] = self[..., 2]
         return ret.view(Transform)
```

### Comparing `py3d-0.1.6/py3d/viewer.html` & `py3d-0.1.7/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.1.6/py3d.egg-info/PKG-INFO` & `py3d-0.1.7/py3d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.1.6
+Version: 0.1.7
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.1.6/setup.py` & `py3d-0.1.7/setup.py`

 * *Files identical despite different names*

