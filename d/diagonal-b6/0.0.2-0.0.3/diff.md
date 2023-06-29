# Comparing `tmp/diagonal_b6-0.0.2.tar.gz` & `tmp/diagonal_b6-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagonal_b6-0.0.2.tar", last modified: Fri May 26 15:49:04 2023, max compression
+gzip compressed data, was "diagonal_b6-0.0.3.tar", last modified: Thu Jun 29 17:19:38 2023, max compression
```

## Comparing `diagonal_b6-0.0.2.tar` & `diagonal_b6-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.843417 diagonal_b6-0.0.2/diagonal_b6/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53768 2023-05-26 15:48:53.000000 diagonal_b6-0.0.2/diagonal_b6/api_generated.py
--rw-r--r--   0 root         (0) root         (0)     8373 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/diagonal_b6/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/diagonal_b6/api_pb2_grpc.py
--rwxr-xr-x   0 root         (0) root         (0)    26093 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/b6_test.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/connect.py
--rw-r--r--   0 root         (0) root         (0)     4181 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/expression.py
--rw-r--r--   0 root         (0) root         (0)     6684 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/features.py
--rw-r--r--   0 root         (0) root         (0)     3894 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/features_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/features_pb2_grpc.py
--rwxr-xr-x   0 root         (0) root         (0)     8424 2023-05-26 12:46:25.000000 diagonal_b6-0.0.2/diagonal_b6/generate_api.py
--rw-r--r--   0 root         (0) root         (0)     3791 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/geometry.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/geometry_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 14:11:40.000000 diagonal_b6-0.0.2/diagonal_b6/geometry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2168 2023-04-21 14:05:17.000000 diagonal_b6-0.0.2/diagonal_b6/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 15:49:04.845417 diagonal_b6-0.0.2/diagonal_b6.egg-info/
--rw-r--r--   0 root         (0) root         (0)      649 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-26 15:49:04.000000 diagonal_b6-0.0.2/diagonal_b6.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      803 2023-05-26 15:48:09.000000 diagonal_b6-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 15:49:04.846417 diagonal_b6-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.381563 diagonal_b6-0.0.3/diagonal_b6/
+-rw-rw-r--   0 root         (0) root         (0)      233 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54912 2023-06-29 17:19:24.000000 diagonal_b6-0.0.3/diagonal_b6/api_generated.py
+-rw-r--r--   0 root         (0) root         (0)     9079 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-06-29 17:17:43.000000 diagonal_b6-0.0.3/diagonal_b6/api_pb2_grpc.py
+-rwxrwxr-x   0 root         (0) root         (0)    27773 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/b6_test.py
+-rw-rw-r--   0 root         (0) root         (0)     1466 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/collection.py
+-rw-rw-r--   0 root         (0) root         (0)      976 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/connect.py
+-rw-rw-r--   0 root         (0) root         (0)     4238 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/expression.py
+-rw-rw-r--   0 root         (0) root         (0)     6766 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/features.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/features_pb2.py
+-rwxrwxr-x   0 root         (0) root         (0)     8424 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/generate_api.py
+-rw-rw-r--   0 root         (0) root         (0)     3927 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/geometry.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-06-29 17:17:42.000000 diagonal_b6-0.0.3/diagonal_b6/geometry_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     2168 2023-06-29 16:25:01.000000 diagonal_b6-0.0.3/diagonal_b6/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/diagonal_b6.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      649 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      553 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 17:19:38.000000 diagonal_b6-0.0.3/diagonal_b6.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      803 2023-06-29 17:17:43.000000 diagonal_b6-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 17:19:38.385563 diagonal_b6-0.0.3/setup.cfg
```

### Comparing `diagonal_b6-0.0.2/PKG-INFO` & `diagonal_b6-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagonal_b6
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
 Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/api_generated.py` & `diagonal_b6-0.0.3/diagonal_b6/api_generated.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,45 +4,48 @@
 from __future__ import annotations
 
 from typing import Callable
 
 import diagonal_b6.expression
 from diagonal_b6.expression import Call, Symbol, Lambda, Result
 
-VERSION = '0.0.2+modified'
+VERSION = '0.0.3+modified'
 
 class CollectionTraits:
 
+    def flattern(self) -> CollectionResult:
+        return flattern(self)
+
+    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+        return map(self, a0)
+
+    def count(self) -> IntTraits:
+        return count(self)
+
+    def map_parallel(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+        return map_parallel(self, a0)
+
+    def top(self, a0: IntTraits) -> CollectionResult:
+        return top(self, a0)
+
     def take(self, a0: IntTraits) -> CollectionResult:
         return take(self, a0)
 
-    def map_items(self, a0: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
-        return map_items(self, a0)
-
     def count_values(self) -> CollectionResult:
         return count_values(self)
 
-    def map_parallel(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-        return map_parallel(self, a0)
+    def map_items(self, a0: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
+        return map_items(self, a0)
 
     def sum_by_key(self) -> CollectionResult:
         return sum_by_key(self)
 
-    def count(self) -> IntTraits:
-        return count(self)
-
     def filter(self, a0: Callable[[AnyTraits],BoolTraits]) -> CollectionResult:
         return filter(self, a0)
 
-    def flattern(self) -> CollectionResult:
-        return flattern(self)
-
-    def map(self, a0: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-        return map(self, a0)
-
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class RenderableTraits:
 
     def to_geojson(self) -> GeoJSONTraits:
@@ -67,482 +70,482 @@
         return RenderableResult
 
 class GeometryTraits(RenderableTraits):
 
     def centroid(self) -> PointTraits:
         return centroid(self)
 
-    def points(self) -> PointCollectionResult:
-        return points(self)
+    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
+        return tile_paths(self, a0)
 
     def intersecting(self) -> QueryTraits:
         return intersecting(self)
 
-    def tile_paths(self, a0: IntTraits) -> IntStringCollectionResult:
-        return tile_paths(self, a0)
+    def points(self) -> PointCollectionResult:
+        return points(self)
 
     @classmethod
     def _collection(cls):
-        return CollectionResult
+        return AnyGeometryCollectionResult
 
 class GeometryValuesTraits(RenderableValuesTraits):
 
     def centroid(self) -> PointCollectionTraits:
         return self.map(Lambda(centroid, [self._values()]))
 
-    def points(self) -> CollectionTraits:
-        return self.map(Lambda(points, [self._values()]))
+    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
 
     def intersecting(self) -> CollectionTraits:
         return self.map(Lambda(intersecting, [self._values()]))
 
-    def tile_paths(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: tile_paths(x, a0), [self._values()]))
+    def points(self) -> CollectionTraits:
+        return self.map(Lambda(points, [self._values()]))
 
 class AnyGeometryValuesResult(Result, GeometryValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return GeometryResult
 
 class IdentifiableTraits:
 
-    def get_string(self, a0: StringTraits) -> StringTraits:
-        return get_string(self, a0)
+    def all_tags(self) -> IntTagCollectionResult:
+        return all_tags(self)
+
+    def remove_tag(self, a0: StringTraits) -> ChangeTraits:
+        return remove_tag(self, a0)
 
     def add_tag(self, a0: TagTraits) -> ChangeTraits:
         return add_tag(self, a0)
 
-    def get(self, a0: StringTraits) -> TagTraits:
-        return get(self, a0)
+    def count_tag_value(self, a0: StringTraits) -> CollectionResult:
+        return count_tag_value(self, a0)
 
-    def all_tags(self) -> IntTagCollectionResult:
-        return all_tags(self)
+    def get_int(self, a0: StringTraits) -> IntTraits:
+        return get_int(self, a0)
 
     def debug_tokens(self) -> IntStringCollectionResult:
         return debug_tokens(self)
 
-    def get_int(self, a0: StringTraits) -> IntTraits:
-        return get_int(self, a0)
-
-    def count_tag_value(self, a0: StringTraits) -> CollectionResult:
-        return count_tag_value(self, a0)
+    def get_string(self, a0: StringTraits) -> StringTraits:
+        return get_string(self, a0)
 
     def get_float(self, a0: StringTraits) -> FloatTraits:
         return get_float(self, a0)
 
-    def remove_tag(self, a0: StringTraits) -> ChangeTraits:
-        return remove_tag(self, a0)
+    def get(self, a0: StringTraits) -> TagTraits:
+        return get(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class IdentifiableValuesTraits:
 
-    def get_string(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
+    def all_tags(self) -> CollectionTraits:
+        return self.map(Lambda(all_tags, [self._values()]))
+
+    def remove_tag(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
 
     def add_tag(self, a0: TagTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: add_tag(x, a0), [self._values()]))
 
-    def get(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
+    def count_tag_value(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: count_tag_value(x, a0), [self._values()]))
 
-    def all_tags(self) -> CollectionTraits:
-        return self.map(Lambda(all_tags, [self._values()]))
+    def get_int(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get_int(x, a0), [self._values()]))
 
     def debug_tokens(self) -> CollectionTraits:
         return self.map(Lambda(debug_tokens, [self._values()]))
 
-    def get_int(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: get_int(x, a0), [self._values()]))
-
-    def count_tag_value(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: count_tag_value(x, a0), [self._values()]))
+    def get_string(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get_string(x, a0), [self._values()]))
 
     def get_float(self, a0: StringTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: get_float(x, a0), [self._values()]))
 
-    def remove_tag(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: remove_tag(x, a0), [self._values()]))
+    def get(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: get(x, a0), [self._values()]))
 
 class AnyIdentifiableValuesResult(Result, IdentifiableValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IdentifiableResult
 
 class FeatureTraits(IdentifiableTraits, RenderableTraits):
 
-    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FloatTraits:
-        return closest_distance(self, a0, a1, a2)
-
     def has_key(self, a0: StringTraits) -> BoolTraits:
         return has_key(self, a0)
 
+    def connect_to_network(self) -> ChangeTraits:
+        return connect_to_network(self)
+
+    def tile_ids_hex(self) -> FeatureIDStringCollectionResult:
+        return tile_ids_hex(self)
+
     def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureIDIntCollectionResult:
         return paths_to_reach(self, a0, a1, a2)
 
     def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionResult:
         return reachable(self, a0, a1, a2)
 
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
+        return reachable_points(self, a0, a1, a2)
+
     def point_features(self) -> PointFeatureCollectionResult:
         return point_features(self)
 
-    def tile_ids(self) -> FeatureIDIntCollectionResult:
-        return tile_ids(self)
-
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> PointFeatureCollectionResult:
-        return reachable_points(self, a0, a1, a2)
+    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> FloatTraits:
+        return reachable_area(self, a0, a1)
 
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureTraits:
         return closest(self, a0, a1, a2)
 
-    def tile_ids_hex(self) -> FeatureIDStringCollectionResult:
-        return tile_ids_hex(self)
-
-    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> FloatTraits:
-        return reachable_area(self, a0, a1)
+    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FloatTraits:
+        return closest_distance(self, a0, a1, a2)
 
-    def connect_to_network(self) -> ChangeTraits:
-        return connect_to_network(self)
+    def tile_ids(self) -> FeatureIDIntCollectionResult:
+        return tile_ids(self)
 
     @classmethod
     def _collection(cls):
         return FeatureCollectionResult
 
 class FeatureValuesTraits(IdentifiableValuesTraits, RenderableValuesTraits):
 
-    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: closest_distance(x, a0, a1, a2), [self._values()]))
-
     def has_key(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: has_key(x, a0), [self._values()]))
 
+    def connect_to_network(self) -> CollectionTraits:
+        return self.map(Lambda(connect_to_network, [self._values()]))
+
+    def tile_ids_hex(self) -> CollectionTraits:
+        return self.map(Lambda(tile_ids_hex, [self._values()]))
+
     def paths_to_reach(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: paths_to_reach(x, a0, a1, a2), [self._values()]))
 
     def reachable(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: reachable(x, a0, a1, a2), [self._values()]))
 
+    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
+
     def point_features(self) -> CollectionTraits:
         return self.map(Lambda(point_features, [self._values()]))
 
-    def tile_ids(self) -> CollectionTraits:
-        return self.map(Lambda(tile_ids, [self._values()]))
-
-    def reachable_points(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: reachable_points(x, a0, a1, a2), [self._values()]))
+    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: reachable_area(x, a0, a1), [self._values()]))
 
     def closest(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> FeatureCollectionTraits:
         return self.map(Lambda(lambda x: closest(x, a0, a1, a2), [self._values()]))
 
-    def tile_ids_hex(self) -> CollectionTraits:
-        return self.map(Lambda(tile_ids_hex, [self._values()]))
-
-    def reachable_area(self, a0: StringTraits, a1: FloatTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: reachable_area(x, a0, a1), [self._values()]))
+    def closest_distance(self, a0: StringTraits, a1: FloatTraits, a2: QueryTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: closest_distance(x, a0, a1, a2), [self._values()]))
 
-    def connect_to_network(self) -> CollectionTraits:
-        return self.map(Lambda(connect_to_network, [self._values()]))
+    def tile_ids(self) -> CollectionTraits:
+        return self.map(Lambda(tile_ids, [self._values()]))
 
 class AnyFeatureValuesResult(Result, FeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureResult
 
-class NumberTraits:
-
-    def divide(self, a0: NumberTraits) -> NumberTraits:
-        return divide(self, a0)
-
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
-
-class NumberValuesTraits:
-
-    def divide(self, a0: NumberTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: divide(x, a0), [self._values()]))
-
-class AnyNumberValuesResult(Result, NumberValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-    @classmethod
-    def _values(cls):
-        return NumberResult
-
 class AreaTraits(GeometryTraits):
 
-    def area(self) -> FloatTraits:
-        return area(self)
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
+        return snap_area_edges(self, a0, a1)
+
+    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
+        return s2_grid(self, a0)
 
     def s2_points(self, a0: IntTraits, a1: IntTraits) -> StringPointCollectionResult:
         return s2_points(self, a0, a1)
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaTraits:
-        return snap_area_edges(self, a0, a1)
-
     def within(self) -> QueryTraits:
         return within(self)
 
+    def area(self) -> FloatTraits:
+        return area(self)
+
     def s2_covering(self, a0: IntTraits, a1: IntTraits) -> StringStringCollectionResult:
         return s2_covering(self, a0, a1)
 
-    def s2_grid(self, a0: IntTraits) -> StringStringCollectionResult:
-        return s2_grid(self, a0)
-
     @classmethod
     def _collection(cls):
         return AreaCollectionResult
 
 class AreaValuesTraits(GeometryValuesTraits):
 
-    def area(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(area, [self._values()]))
+    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
+
+    def s2_grid(self, a0: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: s2_grid(x, a0), [self._values()]))
 
     def s2_points(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: s2_points(x, a0, a1), [self._values()]))
 
-    def snap_area_edges(self, a0: QueryTraits, a1: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: snap_area_edges(x, a0, a1), [self._values()]))
-
     def within(self) -> CollectionTraits:
         return self.map(Lambda(within, [self._values()]))
 
+    def area(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(area, [self._values()]))
+
     def s2_covering(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: s2_covering(x, a0, a1), [self._values()]))
 
-    def s2_grid(self, a0: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: s2_grid(x, a0), [self._values()]))
-
 class AnyAreaValuesResult(Result, AreaValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return AreaResult
 
-class PointTraits(GeometryTraits):
+class NumberTraits:
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
-        return cap_polygon(self, a0)
+    def divide(self, a0: NumberTraits) -> NumberTraits:
+        return divide(self, a0)
 
-    def distance_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_meters(self, a0)
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
+
+class NumberValuesTraits:
+
+    def divide(self, a0: NumberTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: divide(x, a0), [self._values()]))
+
+class AnyNumberValuesResult(Result, NumberValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return NumberResult
+
+class PointTraits(GeometryTraits):
+
+    def sightline(self, a0: FloatTraits) -> AreaTraits:
+        return sightline(self, a0)
 
     def intersecting_cap(self, a0: FloatTraits) -> QueryTraits:
         return intersecting_cap(self, a0)
 
     def add_point(self, a0: StringPointCollectionResult) -> StringPointCollectionResult:
         return add_point(self, a0)
 
     def within_cap(self, a0: FloatTraits) -> QueryTraits:
         return within_cap(self, a0)
 
     def rectangle_polygon(self, a0: PointTraits) -> AreaTraits:
         return rectangle_polygon(self, a0)
 
-    def sightline(self, a0: FloatTraits) -> AreaTraits:
-        return sightline(self, a0)
+    def distance_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_meters(self, a0)
+
+    def cap_polygon(self, a0: FloatTraits) -> AreaTraits:
+        return cap_polygon(self, a0)
 
     @classmethod
     def _collection(cls):
         return PointCollectionResult
 
 class PointValuesTraits(GeometryValuesTraits):
 
-    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
-
-    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
+    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
 
     def intersecting_cap(self, a0: FloatTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: intersecting_cap(x, a0), [self._values()]))
 
     def add_point(self, a0: StringPointCollectionResult) -> CollectionTraits:
         return self.map(Lambda(lambda x: add_point(x, a0), [self._values()]))
 
     def within_cap(self, a0: FloatTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: within_cap(x, a0), [self._values()]))
 
     def rectangle_polygon(self, a0: PointTraits) -> AreaCollectionTraits:
         return self.map(Lambda(lambda x: rectangle_polygon(x, a0), [self._values()]))
 
-    def sightline(self, a0: FloatTraits) -> AreaCollectionTraits:
-        return self.map(Lambda(lambda x: sightline(x, a0), [self._values()]))
+    def distance_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_meters(x, a0), [self._values()]))
+
+    def cap_polygon(self, a0: FloatTraits) -> AreaCollectionTraits:
+        return self.map(Lambda(lambda x: cap_polygon(x, a0), [self._values()]))
 
 class AnyPointValuesResult(Result, PointValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return PointResult
 
+class PathTraits(GeometryTraits):
+
+    def ordered_join(self, a0: PathTraits) -> PathTraits:
+        return ordered_join(self, a0)
+
+    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
+        return distance_to_point_meters(self, a0)
+
+    def interpolate(self, a0: FloatTraits) -> PointTraits:
+        return interpolate(self, a0)
+
+    def sample_points(self, a0: FloatTraits) -> StringPointCollectionResult:
+        return sample_points(self, a0)
+
+    def join(self, a0: PathTraits) -> PathTraits:
+        return join(self, a0)
+
+    @classmethod
+    def _collection(cls):
+        return PathCollectionResult
+
+class PathValuesTraits(GeometryValuesTraits):
+
+    def ordered_join(self, a0: PathTraits) -> PathCollectionTraits:
+        return self.map(Lambda(lambda x: ordered_join(x, a0), [self._values()]))
+
+    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
+
+    def interpolate(self, a0: FloatTraits) -> PointCollectionTraits:
+        return self.map(Lambda(lambda x: interpolate(x, a0), [self._values()]))
+
+    def sample_points(self, a0: FloatTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: sample_points(x, a0), [self._values()]))
+
+    def join(self, a0: PathTraits) -> PathCollectionTraits:
+        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
+
+class AnyPathValuesResult(Result, PathValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PathResult
+
 class StringTraits:
 
     def s2_polygon(self) -> AreaTraits:
         return s2_polygon(self)
 
     def tagged(self, a0: StringTraits) -> QueryTraits:
         return tagged(self, a0)
 
-    def debug_all_query(self) -> QueryTraits:
-        return debug_all_query(self)
-
-    def keyed(self) -> QueryTraits:
-        return keyed(self)
+    def export_world(self) -> IntTraits:
+        return export_world(self)
 
     def tag(self, a0: StringTraits) -> TagTraits:
         return tag(self, a0)
 
     def parse_geojson(self) -> GeoJSONTraits:
         return parse_geojson(self)
 
-    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson_file(self, a0)
+    def keyed(self) -> QueryTraits:
+        return keyed(self)
 
     def s2_center(self) -> PointTraits:
         return s2_center(self)
 
-    def export_world(self) -> IntTraits:
-        return export_world(self)
+    def debug_all_query(self) -> QueryTraits:
+        return debug_all_query(self)
+
+    def import_geojson_file(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson_file(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class StringValuesTraits:
 
     def s2_polygon(self) -> AreaCollectionTraits:
         return self.map(Lambda(s2_polygon, [self._values()]))
 
     def tagged(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: tagged(x, a0), [self._values()]))
 
-    def debug_all_query(self) -> CollectionTraits:
-        return self.map(Lambda(debug_all_query, [self._values()]))
-
-    def keyed(self) -> CollectionTraits:
-        return self.map(Lambda(keyed, [self._values()]))
+    def export_world(self) -> CollectionTraits:
+        return self.map(Lambda(export_world, [self._values()]))
 
     def tag(self, a0: StringTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: tag(x, a0), [self._values()]))
 
     def parse_geojson(self) -> CollectionTraits:
         return self.map(Lambda(parse_geojson, [self._values()]))
 
-    def import_geojson_file(self, a0: StringTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
+    def keyed(self) -> CollectionTraits:
+        return self.map(Lambda(keyed, [self._values()]))
 
     def s2_center(self) -> PointCollectionTraits:
         return self.map(Lambda(s2_center, [self._values()]))
 
-    def export_world(self) -> CollectionTraits:
-        return self.map(Lambda(export_world, [self._values()]))
+    def debug_all_query(self) -> CollectionTraits:
+        return self.map(Lambda(debug_all_query, [self._values()]))
+
+    def import_geojson_file(self, a0: StringTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: import_geojson_file(x, a0), [self._values()]))
 
 class AnyStringValuesResult(Result, StringValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return StringResult
 
-class PathTraits(GeometryTraits):
-
-    def ordered_join(self, a0: PathTraits) -> PathTraits:
-        return ordered_join(self, a0)
-
-    def join(self, a0: PathTraits) -> PathTraits:
-        return join(self, a0)
-
-    def sample_points(self, a0: FloatTraits) -> StringPointCollectionResult:
-        return sample_points(self, a0)
-
-    def distance_to_point_meters(self, a0: PointTraits) -> FloatTraits:
-        return distance_to_point_meters(self, a0)
-
-    def interpolate(self, a0: FloatTraits) -> PointTraits:
-        return interpolate(self, a0)
-
-    @classmethod
-    def _collection(cls):
-        return PathCollectionResult
-
-class PathValuesTraits(GeometryValuesTraits):
-
-    def ordered_join(self, a0: PathTraits) -> PathCollectionTraits:
-        return self.map(Lambda(lambda x: ordered_join(x, a0), [self._values()]))
-
-    def join(self, a0: PathTraits) -> PathCollectionTraits:
-        return self.map(Lambda(lambda x: join(x, a0), [self._values()]))
-
-    def sample_points(self, a0: FloatTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: sample_points(x, a0), [self._values()]))
-
-    def distance_to_point_meters(self, a0: PointTraits) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(lambda x: distance_to_point_meters(x, a0), [self._values()]))
-
-    def interpolate(self, a0: FloatTraits) -> PointCollectionTraits:
-        return self.map(Lambda(lambda x: interpolate(x, a0), [self._values()]))
-
-class AnyPathValuesResult(Result, PathValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-    @classmethod
-    def _values(cls):
-        return PathResult
-
 class TagTraits:
 
-    def float_value(self) -> FloatTraits:
-        return float_value(self)
+    def int_value(self) -> IntTraits:
+        return int_value(self)
 
     def value(self) -> StringTraits:
         return value(self)
 
-    def int_value(self) -> IntTraits:
-        return int_value(self)
+    def float_value(self) -> FloatTraits:
+        return float_value(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class TagValuesTraits:
 
-    def float_value(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(float_value, [self._values()]))
+    def int_value(self) -> CollectionTraits:
+        return self.map(Lambda(int_value, [self._values()]))
 
     def value(self) -> CollectionTraits:
         return self.map(Lambda(value, [self._values()]))
 
-    def int_value(self) -> CollectionTraits:
-        return self.map(Lambda(int_value, [self._values()]))
+    def float_value(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(float_value, [self._values()]))
 
 class AnyTagValuesResult(Result, TagValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
@@ -568,111 +571,112 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IdentifiablePointResult
 
-class AreaFeatureTraits(AreaTraits, FeatureTraits):
+class FeatureIDTraits(IdentifiableTraits):
+
+    def find_relation(self) -> RelationFeatureTraits:
+        return find_relation(self)
+
+    def find_point(self) -> PointFeatureTraits:
+        return find_point(self)
+
+    def find_feature(self) -> FeatureTraits:
+        return find_feature(self)
+
+    def find_area(self) -> AreaFeatureTraits:
+        return find_area(self)
+
+    def find_path(self) -> PathFeatureTraits:
+        return find_path(self)
+
     @classmethod
     def _collection(cls):
-        return AreaFeatureCollectionResult
+        return CollectionResult
 
-class AreaFeatureValuesTraits(AreaValuesTraits, FeatureValuesTraits):
-    pass
+class FeatureIDValuesTraits(IdentifiableValuesTraits):
 
-class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
+    def find_relation(self) -> RelationFeatureCollectionTraits:
+        return self.map(Lambda(find_relation, [self._values()]))
+
+    def find_point(self) -> PointFeatureCollectionTraits:
+        return self.map(Lambda(find_point, [self._values()]))
+
+    def find_feature(self) -> FeatureCollectionTraits:
+        return self.map(Lambda(find_feature, [self._values()]))
+
+    def find_area(self) -> AreaFeatureCollectionTraits:
+        return self.map(Lambda(find_area, [self._values()]))
+
+    def find_path(self) -> PathFeatureCollectionTraits:
+        return self.map(Lambda(find_path, [self._values()]))
+
+class AnyFeatureIDValuesResult(Result, FeatureIDValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return FeatureIDResult
 
 class AnyTraits:
 
-    def pair(self, a0: AnyTraits) -> PairTraits:
-        return pair(self, a0)
-
     def gt(self, a0: AnyTraits) -> BoolTraits:
         return gt(self, a0)
 
+    def pair(self, a0: AnyTraits) -> PairTraits:
+        return pair(self, a0)
+
     def collection(self, a0: AnyTraits) -> CollectionResult:
         return collection(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class AnyValuesTraits:
 
-    def pair(self, a0: AnyTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
-
     def gt(self, a0: AnyTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: gt(x, a0), [self._values()]))
 
+    def pair(self, a0: AnyTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: pair(x, a0), [self._values()]))
+
     def collection(self, a0: AnyTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: collection(x, a0), [self._values()]))
 
 class AnyAnyValuesResult(Result, AnyValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return AnyResult
 
-class PointFeatureTraits(PointTraits, IdentifiablePointTraits, FeatureTraits):
-
-    def degree(self) -> IntTraits:
-        return degree(self)
-
-    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
-        return connect(self, a0)
-
-    @classmethod
-    def _collection(cls):
-        return PointFeatureCollectionResult
-
-class PointFeatureValuesTraits(PointValuesTraits, IdentifiablePointValuesTraits, FeatureValuesTraits):
-
-    def degree(self) -> CollectionTraits:
-        return self.map(Lambda(degree, [self._values()]))
-
-    def connect(self, a0: PointFeatureTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
-
-class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
-
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-    @classmethod
-    def _values(cls):
-        return PointFeatureResult
-
-class RelationFeatureTraits(FeatureTraits, GeometryTraits):
+class AreaFeatureTraits(AreaTraits, FeatureTraits):
     @classmethod
     def _collection(cls):
-        return RelationFeatureCollectionResult
+        return AreaFeatureCollectionResult
 
-class RelationFeatureValuesTraits(FeatureValuesTraits, GeometryValuesTraits):
+class AreaFeatureValuesTraits(AreaValuesTraits, FeatureValuesTraits):
     pass
 
-class AnyRelationFeatureValuesResult(Result, RelationFeatureValuesTraits, CollectionTraits):
+class AnyAreaFeatureValuesResult(Result, AreaFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RelationFeatureResult
+        return AreaFeatureResult
 
 class FloatTraits(NumberTraits):
 
     def ll(self, a0: FloatTraits) -> PointTraits:
         return ll(self, a0)
 
     @classmethod
@@ -689,311 +693,324 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FloatResult
 
-class PointCollectionTraits(CollectionTraits, PointValuesTraits):
+class PathFeatureTraits(FeatureTraits, PathTraits):
+
+    def length(self) -> FloatTraits:
+        return length(self)
+
     @classmethod
     def _collection(cls):
-        return CollectionResult
+        return PathFeatureCollectionResult
 
-class IntTraits(NumberTraits):
+class PathFeatureValuesTraits(FeatureValuesTraits, PathValuesTraits):
 
-    def clamp(self, a0: IntTraits, a1: IntTraits) -> IntTraits:
-        return clamp(self, a0, a1)
+    def length(self) -> AnyFloatCollectionTraits:
+        return self.map(Lambda(length, [self._values()]))
+
+class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PathFeatureResult
+
+class IntTraits(NumberTraits):
 
     def add_ints(self, a0: IntTraits) -> IntTraits:
         return add_ints(self, a0)
 
+    def clamp(self, a0: IntTraits, a1: IntTraits) -> IntTraits:
+        return clamp(self, a0, a1)
+
     def divide_int(self, a0: FloatTraits) -> FloatTraits:
         return divide_int(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class IntValuesTraits(NumberValuesTraits):
 
-    def clamp(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
-        return self.map(Lambda(lambda x: clamp(x, a0, a1), [self._values()]))
-
     def add_ints(self, a0: IntTraits) -> CollectionTraits:
         return self.map(Lambda(lambda x: add_ints(x, a0), [self._values()]))
 
+    def clamp(self, a0: IntTraits, a1: IntTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: clamp(x, a0, a1), [self._values()]))
+
     def divide_int(self, a0: FloatTraits) -> AnyFloatCollectionTraits:
         return self.map(Lambda(lambda x: divide_int(x, a0), [self._values()]))
 
 class AnyIntValuesResult(Result, IntValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return IntResult
 
-class PathFeatureTraits(PathTraits, FeatureTraits):
+class PointCollectionTraits(CollectionTraits, PointValuesTraits):
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def length(self) -> FloatTraits:
-        return length(self)
+class PathCollectionTraits(CollectionTraits, PathValuesTraits):
+
+    def sample_points_along_paths(self, a0: FloatTraits) -> PointCollectionResult:
+        return sample_points_along_paths(self, a0)
 
     @classmethod
     def _collection(cls):
-        return PathFeatureCollectionResult
+        return CollectionResult
 
-class PathFeatureValuesTraits(PathValuesTraits, FeatureValuesTraits):
+class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+    @classmethod
+    def _collection(cls):
+        return CollectionResult
 
-    def length(self) -> AnyFloatCollectionTraits:
-        return self.map(Lambda(length, [self._values()]))
+class RelationFeatureTraits(FeatureTraits, GeometryTraits):
+    @classmethod
+    def _collection(cls):
+        return RelationFeatureCollectionResult
 
-class AnyPathFeatureValuesResult(Result, PathFeatureValuesTraits, CollectionTraits):
+class RelationFeatureValuesTraits(FeatureValuesTraits, GeometryValuesTraits):
+    pass
+
+class AnyRelationFeatureValuesResult(Result, RelationFeatureValuesTraits, CollectionTraits):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathFeatureResult
+        return RelationFeatureResult
 
-class FeatureIDTraits(IdentifiableTraits):
+class PointFeatureTraits(PointTraits, IdentifiablePointTraits, FeatureTraits):
 
-    def find_feature(self) -> FeatureTraits:
-        return find_feature(self)
+    def connect(self, a0: PointFeatureTraits) -> ChangeTraits:
+        return connect(self, a0)
 
-    def find_point(self) -> PointFeatureTraits:
-        return find_point(self)
+    def degree(self) -> IntTraits:
+        return degree(self)
 
-    def find_area(self) -> AreaFeatureTraits:
-        return find_area(self)
+    @classmethod
+    def _collection(cls):
+        return PointFeatureCollectionResult
 
-    def find_path(self) -> PathFeatureTraits:
-        return find_path(self)
+class PointFeatureValuesTraits(PointValuesTraits, IdentifiablePointValuesTraits, FeatureValuesTraits):
 
-    def find_relation(self) -> RelationFeatureTraits:
-        return find_relation(self)
+    def connect(self, a0: PointFeatureTraits) -> CollectionTraits:
+        return self.map(Lambda(lambda x: connect(x, a0), [self._values()]))
+
+    def degree(self) -> CollectionTraits:
+        return self.map(Lambda(degree, [self._values()]))
+
+class AnyPointFeatureValuesResult(Result, PointFeatureValuesTraits, CollectionTraits):
+
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+    @classmethod
+    def _values(cls):
+        return PointFeatureResult
+
+class PairTraits:
+
+    def first(self) -> AnyTraits:
+        return first(self)
+
+    def second(self) -> AnyTraits:
+        return second(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDValuesTraits(IdentifiableValuesTraits):
+class QueryTraits:
 
-    def find_feature(self) -> FeatureCollectionTraits:
-        return self.map(Lambda(find_feature, [self._values()]))
+    def find_paths(self) -> PathFeatureCollectionResult:
+        return find_paths(self)
 
-    def find_point(self) -> PointFeatureCollectionTraits:
-        return self.map(Lambda(find_point, [self._values()]))
+    def find(self) -> FeatureCollectionResult:
+        return find(self)
 
-    def find_area(self) -> AreaFeatureCollectionTraits:
-        return self.map(Lambda(find_area, [self._values()]))
+    def or_(self, a0: QueryTraits) -> QueryTraits:
+        return or_(self, a0)
 
-    def find_path(self) -> PathFeatureCollectionTraits:
-        return self.map(Lambda(find_path, [self._values()]))
+    def find_points(self) -> PointFeatureCollectionResult:
+        return find_points(self)
 
-    def find_relation(self) -> RelationFeatureCollectionTraits:
-        return self.map(Lambda(find_relation, [self._values()]))
+    def find_areas(self) -> AreaFeatureCollectionResult:
+        return find_areas(self)
 
-class AnyFeatureIDValuesResult(Result, FeatureIDValuesTraits, CollectionTraits):
+    def find_relations(self) -> RelationFeatureCollectionResult:
+        return find_relations(self)
 
-    def __init__(self, node):
-        Result.__init__(self, node)
+    def and_(self, a0: QueryTraits) -> QueryTraits:
+        return and_(self, a0)
 
     @classmethod
-    def _values(cls):
-        return FeatureIDResult
+    def _collection(cls):
+        return CollectionResult
 
-class AreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PathCollectionTraits(CollectionTraits, PathValuesTraits):
+class GeoJSONTraits:
 
-    def sample_points_along_paths(self, a0: FloatTraits) -> PointCollectionResult:
-        return sample_points_along_paths(self, a0)
+    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+        return map_geometries(self, a0)
+
+    def geojson_areas(self) -> StringAreaCollectionResult:
+        return geojson_areas(self)
+
+    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
+        return import_geojson(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
-
-    def to_geojson_collection(self) -> GeoJSONTraits:
-        return to_geojson_collection(self)
-
+class RelationFeatureCollectionTraits(CollectionTraits, RelationFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class QueryProtoTraits:
+class BoolTraits:
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringPointCollectionTraits(CollectionTraits, PointValuesTraits):
+class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
+
+    def add_tags(self) -> ChangeTraits:
+        return add_tags(self)
+
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class RelationFeatureCollectionTraits(CollectionTraits, RelationFeatureValuesTraits):
+class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class AnyFloatCollectionTraits(CollectionTraits, FloatValuesTraits):
 
     def percentiles(self) -> AnyFloatCollectionResult:
         return percentiles(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
+class AnyRenderableCollectionTraits(CollectionTraits, RenderableValuesTraits):
 
-    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
-        return containing_areas(self, a0)
+    def to_geojson_collection(self) -> GeoJSONTraits:
+        return to_geojson_collection(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class IntStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class AreaFeatureCollectionTraits(AreaCollectionTraits, AreaFeatureValuesTraits):
+class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
+class StringStringCollectionTraits(CollectionTraits, StringValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
+class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
 
-    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
-        return building_access(self, a0, a1)
+    def remove_tags(self) -> ChangeTraits:
+        return remove_tags(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class IntTagCollectionTraits(CollectionTraits, TagValuesTraits):
+class QueryProtoTraits:
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class GeoJSONTraits:
-
-    def geojson_areas(self) -> StringAreaCollectionResult:
-        return geojson_areas(self)
-
-    def map_geometries(self, a0: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-        return map_geometries(self, a0)
+class ChangeTraits:
 
-    def import_geojson(self, a0: StringTraits) -> ChangeTraits:
-        return import_geojson(self, a0)
+    def with_change(self, a0: Callable[[],AnyTraits]) -> AnyTraits:
+        return with_change(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDIntCollectionTraits(CollectionTraits, IntValuesTraits):
+class AreaFeatureCollectionTraits(AreaCollectionTraits, AreaFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class QueryTraits:
-
-    def and_(self, a0: QueryTraits) -> QueryTraits:
-        return and_(self, a0)
+class AnyGeometryCollectionTraits(CollectionTraits, GeometryValuesTraits):
 
-    def find_areas(self) -> AreaFeatureCollectionResult:
-        return find_areas(self)
-
-    def find_points(self) -> PointFeatureCollectionResult:
-        return find_points(self)
-
-    def or_(self, a0: QueryTraits) -> QueryTraits:
-        return or_(self, a0)
-
-    def find_relations(self) -> RelationFeatureCollectionResult:
-        return find_relations(self)
-
-    def find_paths(self) -> PathFeatureCollectionResult:
-        return find_paths(self)
-
-    def find(self) -> FeatureCollectionResult:
-        return find(self)
+    def convex_hull(self) -> AreaTraits:
+        return convex_hull(self)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class BoolTraits:
+class StringAreaCollectionTraits(CollectionTraits, AreaValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class PairTraits:
-
-    def second(self) -> AnyTraits:
-        return second(self)
+class PointFeatureCollectionTraits(PointCollectionTraits, PointFeatureValuesTraits):
 
-    def first(self) -> AnyTraits:
-        return first(self)
+    def containing_areas(self, a0: QueryTraits) -> AreaFeatureCollectionResult:
+        return containing_areas(self, a0)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class PathFeatureCollectionTraits(PathCollectionTraits, PathFeatureValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDTagCollectionTraits(CollectionTraits, TagValuesTraits):
-
-    def add_tags(self) -> ChangeTraits:
-        return add_tags(self)
-
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
-
-class FeatureIDStringCollectionTraits(CollectionTraits, StringValuesTraits):
+class FeatureCollectionTraits(CollectionTraits, FeatureValuesTraits):
 
-    def remove_tags(self) -> ChangeTraits:
-        return remove_tags(self)
+    def building_access(self, a0: FloatTraits, a1: StringTraits) -> FeatureIDFeatureIDCollectionResult:
+        return building_access(self, a0, a1)
 
     @classmethod
     def _collection(cls):
         return CollectionResult
 
-class FeatureIDFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
-    @classmethod
-    def _collection(cls):
-        return CollectionResult
-
-class ChangeTraits:
-
-    def with_change(self, a0: Callable[[],AnyTraits]) -> AnyTraits:
-        return with_change(self, a0)
-
+class IntFeatureIDCollectionTraits(CollectionTraits, FeatureIDValuesTraits):
     @classmethod
     def _collection(cls):
         return CollectionResult
 
 class CollectionResult(Result, CollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
@@ -1014,632 +1031,654 @@
     def __init__(self, node):
         Result.__init__(self, node)
 
 class FeatureResult(Result, FeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class NumberResult(Result, NumberTraits):
+class AreaResult(Result, AreaTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaResult(Result, AreaTraits):
+class NumberResult(Result, NumberTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class PointResult(Result, PointTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class StringResult(Result, StringTraits):
+class PathResult(Result, PathTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathResult(Result, PathTraits):
+class StringResult(Result, StringTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class TagResult(Result, TagTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class IdentifiablePointResult(Result, IdentifiablePointTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaFeatureResult(Result, AreaFeatureTraits):
+class FeatureIDResult(Result, FeatureIDTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class AnyResult(Result, AnyTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PointFeatureResult(Result, PointFeatureTraits):
+class AreaFeatureResult(Result, AreaFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class RelationFeatureResult(Result, RelationFeatureTraits):
+class FloatResult(Result, FloatTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FloatResult(Result, FloatTraits):
+class PathFeatureResult(Result, PathFeatureTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class IntResult(Result, IntTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
 class PointCollectionResult(Result, PointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return PointResult
 
-class IntResult(Result, IntTraits):
+class PathCollectionResult(Result, PathCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathFeatureResult(Result, PathFeatureTraits):
+    @classmethod
+    def _values(cls):
+        return PathResult
+
+class AreaCollectionResult(Result, AreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FeatureIDResult(Result, FeatureIDTraits):
+    @classmethod
+    def _values(cls):
+        return AreaResult
+
+class RelationFeatureResult(Result, RelationFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class AreaCollectionResult(Result, AreaCollectionTraits):
+class PointFeatureResult(Result, PointFeatureTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return AreaResult
+class PairResult(Result, PairTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
 
-class PathCollectionResult(Result, PathCollectionTraits):
+class QueryResult(Result, QueryTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class StringPointCollectionResult(Result, StringPointCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathResult
+        return PointResult
 
-class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
+class GeoJSONResult(Result, GeoJSONTraits):
+    def __init__(self, node):
+        Result.__init__(self, node)
+
+class RelationFeatureCollectionResult(Result, RelationFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RenderableResult
+        return RelationFeatureResult
 
-class QueryProtoResult(Result, QueryProtoTraits):
+class BoolResult(Result, BoolTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class StringPointCollectionResult(Result, StringPointCollectionTraits):
+class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointResult
+        return TagResult
 
-class IntStringCollectionResult(Result, IntStringCollectionTraits):
+class IntTagCollectionResult(Result, IntTagCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return TagResult
 
-class RelationFeatureCollectionResult(Result, RelationFeatureCollectionTraits):
+class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return RelationFeatureResult
+        return IntResult
 
 class AnyFloatCollectionResult(Result, AnyFloatCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FloatResult
 
-class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
+class AnyRenderableCollectionResult(Result, AnyRenderableCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PointFeatureResult
+        return RenderableResult
 
-class StringStringCollectionResult(Result, StringStringCollectionTraits):
+class IntStringCollectionResult(Result, IntStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return StringResult
 
-class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
+class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaFeatureResult
+        return FeatureIDResult
 
-class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
+class StringStringCollectionResult(Result, StringStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return AreaResult
+        return StringResult
 
-class FeatureCollectionResult(Result, FeatureCollectionTraits):
+class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return FeatureResult
+        return StringResult
 
-class IntTagCollectionResult(Result, IntTagCollectionTraits):
+class QueryProtoResult(Result, QueryProtoTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-    @classmethod
-    def _values(cls):
-        return TagResult
-
-class GeoJSONResult(Result, GeoJSONTraits):
+class ChangeResult(Result, ChangeTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class FeatureIDIntCollectionResult(Result, FeatureIDIntCollectionTraits):
+class AreaFeatureCollectionResult(Result, AreaFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return IntResult
+        return AreaFeatureResult
 
-class QueryResult(Result, QueryTraits):
+class AnyGeometryCollectionResult(Result, AnyGeometryCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class BoolResult(Result, BoolTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
+    @classmethod
+    def _values(cls):
+        return GeometryResult
 
-class PairResult(Result, PairTraits):
+class StringAreaCollectionResult(Result, StringAreaCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
-class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
+    @classmethod
+    def _values(cls):
+        return AreaResult
+
+class PointFeatureCollectionResult(Result, PointFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return PathFeatureResult
+        return PointFeatureResult
 
-class FeatureIDTagCollectionResult(Result, FeatureIDTagCollectionTraits):
+class PathFeatureCollectionResult(Result, PathFeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return TagResult
+        return PathFeatureResult
 
-class FeatureIDStringCollectionResult(Result, FeatureIDStringCollectionTraits):
+class FeatureCollectionResult(Result, FeatureCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
-        return StringResult
+        return FeatureResult
 
-class FeatureIDFeatureIDCollectionResult(Result, FeatureIDFeatureIDCollectionTraits):
+class IntFeatureIDCollectionResult(Result, IntFeatureIDCollectionTraits):
     def __init__(self, node):
         Result.__init__(self, node)
 
     @classmethod
     def _values(cls):
         return FeatureIDResult
 
-class ChangeResult(Result, ChangeTraits):
-    def __init__(self, node):
-        Result.__init__(self, node)
-
-class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
+class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
+    def __call__(self, a0 : AnyTraits) -> BoolTraits:
         raise NotImplementedError()
 
 class FunctionAnyAnyResult(Result, Callable[[AnyTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     def __call__(self, a0 : AnyTraits) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionPointGeometryResult(Result, Callable[[PointTraits],GeometryTraits]):
+class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PointTraits) -> GeometryTraits:
+    def __call__(self, a0 : PathTraits) -> GeometryTraits:
         raise NotImplementedError()
 
 class FunctionPairAnyResult(Result, Callable[[PairTraits],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     def __call__(self, a0 : PairTraits) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionPathGeometryResult(Result, Callable[[PathTraits],GeometryTraits]):
+class FunctionAnyResult(Result, Callable[[],AnyTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : PathTraits) -> GeometryTraits:
+    def __call__(self, ) -> AnyTraits:
         raise NotImplementedError()
 
-class FunctionAnyBoolResult(Result, Callable[[AnyTraits],BoolTraits]):
+class FunctionAreaGeometryResult(Result, Callable[[AreaTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, a0 : AnyTraits) -> BoolTraits:
+    def __call__(self, a0 : AreaTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-class FunctionAnyResult(Result, Callable[[],AnyTraits]):
+class FunctionPointGeometryResult(Result, Callable[[PointTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
-    def __call__(self, ) -> AnyTraits:
+    def __call__(self, a0 : PointTraits) -> GeometryTraits:
         raise NotImplementedError()
 
 class FunctionGeometryGeometryResult(Result, Callable[[GeometryTraits],GeometryTraits]):
 
     def __init__(self, node):
         Result.__init__(self, node)
 
     def __call__(self, a0 : GeometryTraits) -> GeometryTraits:
         raise NotImplementedError()
 
-def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('closest-distance'), [a0, a1, a2, a3]))
+def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
+    return PathFeatureCollectionResult(Call(Symbol('find-paths'), [a0]))
 
-def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('cap-polygon'), [a0, a1]))
+def convex_hull(a0: AnyGeometryCollectionResult) -> AreaTraits:
+    return AreaResult(Call(Symbol('convex-hull'), [a0]))
 
-def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), [a0]))
+def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('to-geojson-collection'), [a0]))
 
-def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
-    return PairResult(Call(Symbol('pair'), [a0, a1]))
+def building_access(a0: FeatureCollectionResult, a1: FloatTraits, a2: StringTraits) -> FeatureIDFeatureIDCollectionResult:
+    return FeatureIDFeatureIDCollectionResult(Call(Symbol('building-access'), [a0, a1, a2]))
 
-def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('and'), [a0, a1]))
+def find(a0: QueryTraits) -> FeatureCollectionResult:
+    return FeatureCollectionResult(Call(Symbol('find'), [a0]))
 
-def take(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('take'), [a0, a1]))
+def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('or'), [a0, a1]))
 
-def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('find-feature'), [a0]))
+def s2_polygon(a0: StringTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('s2-polygon'), [a0]))
 
-def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('point-paths'), [a0]))
+def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
+    return BoolResult(Call(Symbol('gt'), [a0, a1]))
 
-def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('ordered-join'), [a0, a1]))
+def pair(a0: AnyTraits, a1: AnyTraits) -> PairTraits:
+    return PairResult(Call(Symbol('pair'), [a0, a1]))
 
-def area(a0: AreaTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('area'), [a0]))
+def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('tagged'), [a0, a1]))
 
-def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), [a0]))
+def centroid(a0: GeometryTraits) -> PointTraits:
+    return PointResult(Call(Symbol('centroid'), [a0]))
 
-def degree(a0: PointFeatureTraits) -> IntTraits:
-    return IntResult(Call(Symbol('degree'), [a0]))
+def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('sightline'), [a0, a1]))
 
-def s2_polygon(a0: StringTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('s2-polygon'), [a0]))
+def flattern(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('flattern'), [a0]))
 
 def has_key(a0: FeatureTraits, a1: StringTraits) -> BoolTraits:
     return BoolResult(Call(Symbol('has-key'), [a0, a1]))
 
-def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
-    return PathResult(Call(Symbol('join'), [a0, a1]))
+def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
+    return IntResult(Call(Symbol('add-ints'), [a0, a1]))
 
-def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('s2-points'), [a0, a1, a2]))
+def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('connect-to-network'), [a0]))
+
+def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
+    return IntTagCollectionResult(Call(Symbol('all-tags'), [a0]))
+
+def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
+    return NumberResult(Call(Symbol('divide'), [a0, a1]))
 
 def snap_area_edges(a0: AreaTraits, a1: QueryTraits, a2: FloatTraits) -> AreaTraits:
     return AreaResult(Call(Symbol('snap-area-edges'), [a0, a1, a2]))
 
-def paths_to_reach(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureIDIntCollectionResult:
-    return FeatureIDIntCollectionResult(Call(Symbol('paths-to-reach'), [a0, a1, a2, a3]))
+def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
+    return StringStringCollectionResult(Call(Symbol('s2-grid'), [a0, a1]))
 
-def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson'), [a0]))
+def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
+    return AnyFloatCollectionResult(Call(Symbol('percentiles'), [a0]))
 
-def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
-    return CollectionResult(Call(Symbol('map-items'), [a0, a1]))
+def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), [a0]))
 
-def tagged(a0: StringTraits, a1: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('tagged'), [a0, a1]))
+def export_world(a0: StringTraits) -> IntTraits:
+    return IntResult(Call(Symbol('export-world'), [a0]))
 
-def clamp(a0: IntTraits, a1: IntTraits, a2: IntTraits) -> IntTraits:
-    return IntResult(Call(Symbol('clamp'), [a0, a1, a2]))
+def int_value(a0: TagTraits) -> IntTraits:
+    return IntResult(Call(Symbol('int-value'), [a0]))
 
-def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect'), [a0, a1]))
+def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('map-geometries'), [a0, a1]))
 
-def to_geojson_collection(a0: AnyRenderableCollectionResult) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('to-geojson-collection'), [a0]))
+def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
+    return RelationFeatureResult(Call(Symbol('find-relation'), [a0]))
 
-def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), [a0]))
+def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
+    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), [a0]))
 
-def type_point() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-point'), []))
+def apply_to_area(a0: Callable[[AreaTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-area'), [a0]))
 
-def float_value(a0: TagTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('float-value'), [a0]))
+def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('remove-tag'), [a0, a1]))
+
+def connect(a0: PointFeatureTraits, a1: PointFeatureTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('connect'), [a0, a1]))
+
+def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
+    return IntStringCollectionResult(Call(Symbol('tile-paths'), [a0, a1]))
+
+def empty_points() -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('empty-points'), []))
 
 def geojson_areas(a0: GeoJSONTraits) -> StringAreaCollectionResult:
     return StringAreaCollectionResult(Call(Symbol('geojson-areas'), [a0]))
 
-def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
-    return PointFeatureResult(Call(Symbol('find-point'), [a0]))
+def intersecting(a0: GeometryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('intersecting'), [a0]))
 
-def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('find-points'), [a0]))
+def intersecting_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('intersecting-cap'), [a0, a1]))
 
-def value(a0: TagTraits) -> StringTraits:
-    return StringResult(Call(Symbol('value'), [a0]))
+def degree(a0: PointFeatureTraits) -> IntTraits:
+    return IntResult(Call(Symbol('degree'), [a0]))
 
-def reachable(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureCollectionResult:
-    return FeatureCollectionResult(Call(Symbol('reachable'), [a0, a1, a2, a3]))
+def s2_points(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('s2-points'), [a0, a1, a2]))
 
-def distance_meters(a0: PointTraits, a1: PointTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('distance-meters'), [a0, a1]))
+def add_tag(a0: IdentifiableTraits, a1: TagTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('add-tag'), [a0, a1]))
 
-def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('add-tags'), [a0]))
+map = diagonal_b6.expression._map
 
-def intersecting_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('intersecting-cap'), [a0, a1]))
+def first(a0: PairTraits) -> AnyTraits:
+    return AnyResult(Call(Symbol('first'), [a0]))
 
-def add_point(a0: PointTraits, a1: StringPointCollectionResult) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('add-point'), [a0, a1]))
+def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
+    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), [a0, a1]))
 
-def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
-    return AreaFeatureResult(Call(Symbol('find-area'), [a0]))
+def clamp(a0: IntTraits, a1: IntTraits, a2: IntTraits) -> IntTraits:
+    return IntResult(Call(Symbol('clamp'), [a0, a1, a2]))
 
-def gt(a0: AnyTraits, a1: AnyTraits) -> BoolTraits:
-    return BoolResult(Call(Symbol('gt'), [a0, a1]))
+def paths_to_reach(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureIDIntCollectionResult:
+    return FeatureIDIntCollectionResult(Call(Symbol('paths-to-reach'), [a0, a1, a2, a3]))
 
-def collection(a0: AnyTraits, a1: AnyTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('collection'), [a0, a1]))
+def find_point(a0: FeatureIDTraits) -> PointFeatureTraits:
+    return PointFeatureResult(Call(Symbol('find-point'), [a0]))
 
-def or_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('or'), [a0, a1]))
+def find_points(a0: QueryTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('find-points'), [a0]))
 
-def int_value(a0: TagTraits) -> IntTraits:
-    return IntResult(Call(Symbol('int-value'), [a0]))
+def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
+    return TagResult(Call(Symbol('tag'), [a0, a1]))
 
-def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
-    return StringResult(Call(Symbol('get-string'), [a0, a1]))
+def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('count-tag-value'), [a0, a1]))
 
-def empty_points() -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('empty-points'), []))
+def count(a0: CollectionResult) -> IntTraits:
+    return IntResult(Call(Symbol('count'), [a0]))
 
-def second(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('second'), [a0]))
+def reachable(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureCollectionResult:
+    return FeatureCollectionResult(Call(Symbol('reachable'), [a0, a1, a2, a3]))
 
-def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
-    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), [a0]))
+def map_parallel(a0: CollectionResult, a1: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
+    return CollectionResult(Call(Symbol('map-parallel'), [a0, a1]))
 
-def map_geometries(a0: GeoJSONTraits, a1: Callable[[GeometryTraits],GeometryTraits]) -> GeoJSONTraits:
-    return GeoJSONResult(Call(Symbol('map-geometries'), [a0, a1]))
+def top(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('top'), [a0, a1]))
 
-def building_access(a0: FeatureCollectionResult, a1: FloatTraits, a2: StringTraits) -> FeatureIDFeatureIDCollectionResult:
-    return FeatureIDFeatureIDCollectionResult(Call(Symbol('building-access'), [a0, a1, a2]))
+def find_areas(a0: QueryTraits) -> AreaFeatureCollectionResult:
+    return AreaFeatureCollectionResult(Call(Symbol('find-areas'), [a0]))
 
-def debug_all_query(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('debug-all-query'), [a0]))
+def ordered_join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    return PathResult(Call(Symbol('ordered-join'), [a0, a1]))
 
-def count_values(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-values'), [a0]))
+def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
+    return IntResult(Call(Symbol('get-int'), [a0, a1]))
 
 def within(a0: AreaTraits) -> QueryTraits:
     return QueryResult(Call(Symbol('within'), [a0]))
 
-def import_geojson(a0: GeoJSONTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('import-geojson'), [a0, a1]))
+def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), [a0, a1, a2, a3]))
 
-def add_tag(a0: IdentifiableTraits, a1: TagTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('add-tag'), [a0, a1]))
+def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
+    return IntStringCollectionResult(Call(Symbol('debug-tokens'), [a0]))
 
-def map_parallel(a0: CollectionResult, a1: Callable[[AnyTraits],AnyTraits]) -> CollectionResult:
-    return CollectionResult(Call(Symbol('map-parallel'), [a0, a1]))
+def take(a0: CollectionResult, a1: IntTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('take'), [a0, a1]))
 
-def sum_by_key(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('sum-by-key'), [a0]))
+def add_point(a0: PointTraits, a1: StringPointCollectionResult) -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('add-point'), [a0, a1]))
 
-def keyed(a0: StringTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('keyed'), [a0]))
+def with_change(a0: ChangeTraits, a1: Callable[[],AnyTraits]) -> AnyTraits:
+    return AnyResult(Call(Symbol('with-change'), [a0, a1]))
 
-def sample_points(a0: PathTraits, a1: FloatTraits) -> StringPointCollectionResult:
-    return StringPointCollectionResult(Call(Symbol('sample-points'), [a0, a1]))
+def count_values(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('count-values'), [a0]))
 
-def find_paths(a0: QueryTraits) -> PathFeatureCollectionResult:
-    return PathFeatureCollectionResult(Call(Symbol('find-paths'), [a0]))
+def import_geojson(a0: GeoJSONTraits, a1: StringTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('import-geojson'), [a0, a1]))
 
 def type_path() -> QueryProtoTraits:
     return QueryProtoResult(Call(Symbol('type-path'), []))
 
-def type_area() -> QueryProtoTraits:
-    return QueryProtoResult(Call(Symbol('type-area'), []))
-
 def within_cap(a0: PointTraits, a1: FloatTraits) -> QueryTraits:
     return QueryResult(Call(Symbol('within-cap'), [a0, a1]))
 
-def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-covering'), [a0, a1, a2]))
-
-def centroid(a0: GeometryTraits) -> PointTraits:
-    return PointResult(Call(Symbol('centroid'), [a0]))
-
-def find(a0: QueryTraits) -> FeatureCollectionResult:
-    return FeatureCollectionResult(Call(Symbol('find'), [a0]))
-
-def all() -> QueryTraits:
-    return QueryResult(Call(Symbol('all'), []))
+def divide_int(a0: IntTraits, a1: FloatTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('divide-int'), [a0, a1]))
 
 def distance_to_point_meters(a0: PathTraits, a1: PointTraits) -> FloatTraits:
     return FloatResult(Call(Symbol('distance-to-point-meters'), [a0, a1]))
 
-def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('point-features'), [a0]))
-
-def count(a0: CollectionResult) -> IntTraits:
-    return IntResult(Call(Symbol('count'), [a0]))
-
-def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
-    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), [a0]))
-
-def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
-    return PathFeatureResult(Call(Symbol('find-path'), [a0]))
-
-def tag(a0: StringTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('tag'), [a0, a1]))
-
-def points(a0: GeometryTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('points'), [a0]))
+def map_items(a0: CollectionResult, a1: Callable[[PairTraits],AnyTraits]) -> CollectionResult:
+    return CollectionResult(Call(Symbol('map-items'), [a0, a1]))
 
-def apply_to_point(a0: Callable[[PointTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
-    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-point'), [a0]))
+def collection(a0: AnyTraits, a1: AnyTraits) -> CollectionResult:
+    return CollectionResult(Call(Symbol('collection'), [a0, a1]))
 
-def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
-    return TagResult(Call(Symbol('get'), [a0, a1]))
+def area(a0: AreaTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('area'), [a0]))
 
 def rectangle_polygon(a0: PointTraits, a1: PointTraits) -> AreaTraits:
     return AreaResult(Call(Symbol('rectangle-polygon'), [a0, a1]))
 
-def s2_grid(a0: AreaTraits, a1: IntTraits) -> StringStringCollectionResult:
-    return StringStringCollectionResult(Call(Symbol('s2-grid'), [a0, a1]))
-
-def sightline(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
-    return AreaResult(Call(Symbol('sightline'), [a0, a1]))
-
 def parse_geojson(a0: StringTraits) -> GeoJSONTraits:
     return GeoJSONResult(Call(Symbol('parse-geojson'), [a0]))
 
-def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tags'), [a0]))
+def point_features(a0: FeatureTraits) -> PointFeatureCollectionResult:
+    return PointFeatureCollectionResult(Call(Symbol('point-features'), [a0]))
 
-filter = diagonal_b6.expression._filter
+def reachable_area(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('reachable-area'), [a0, a1, a2]))
 
-def intersecting(a0: GeometryTraits) -> QueryTraits:
-    return QueryResult(Call(Symbol('intersecting'), [a0]))
+def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
+    return FeatureResult(Call(Symbol('closest'), [a0, a1, a2, a3]))
 
-def percentiles(a0: AnyFloatCollectionResult) -> AnyFloatCollectionResult:
-    return AnyFloatCollectionResult(Call(Symbol('percentiles'), [a0]))
+def add_tags(a0: FeatureIDTagCollectionResult) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('add-tags'), [a0]))
 
-def tile_paths(a0: GeometryTraits, a1: IntTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('tile-paths'), [a0, a1]))
+def sum_by_key(a0: CollectionResult) -> CollectionResult:
+    return CollectionResult(Call(Symbol('sum-by-key'), [a0]))
 
-def all_tags(a0: IdentifiableTraits) -> IntTagCollectionResult:
-    return IntTagCollectionResult(Call(Symbol('all-tags'), [a0]))
+def find_feature(a0: FeatureIDTraits) -> FeatureTraits:
+    return FeatureResult(Call(Symbol('find-feature'), [a0]))
 
-def reachable_points(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> PointFeatureCollectionResult:
-    return PointFeatureCollectionResult(Call(Symbol('reachable-points'), [a0, a1, a2, a3]))
+def keyed(a0: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('keyed'), [a0]))
 
-def closest(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FeatureTraits:
-    return FeatureResult(Call(Symbol('closest'), [a0, a1, a2, a3]))
+def value(a0: TagTraits) -> StringTraits:
+    return StringResult(Call(Symbol('value'), [a0]))
+
+def second(a0: PairTraits) -> AnyTraits:
+    return AnyResult(Call(Symbol('second'), [a0]))
+
+def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
+    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), [a0, a1]))
+
+def find_area(a0: FeatureIDTraits) -> AreaFeatureTraits:
+    return AreaFeatureResult(Call(Symbol('find-area'), [a0]))
+
+def length(a0: PathFeatureTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('length'), [a0]))
 
 def interpolate(a0: PathTraits, a1: FloatTraits) -> PointTraits:
     return PointResult(Call(Symbol('interpolate'), [a0, a1]))
 
-def import_geojson_file(a0: StringTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('import-geojson-file'), [a0, a1]))
+def points(a0: GeometryTraits) -> PointCollectionResult:
+    return PointCollectionResult(Call(Symbol('points'), [a0]))
 
-def debug_tokens(a0: IdentifiableTraits) -> IntStringCollectionResult:
-    return IntStringCollectionResult(Call(Symbol('debug-tokens'), [a0]))
+def s2_center(a0: StringTraits) -> PointTraits:
+    return PointResult(Call(Symbol('s2-center'), [a0]))
 
-def first(a0: PairTraits) -> AnyTraits:
-    return AnyResult(Call(Symbol('first'), [a0]))
+def get_string(a0: IdentifiableTraits, a1: StringTraits) -> StringTraits:
+    return StringResult(Call(Symbol('get-string'), [a0, a1]))
 
-def sample_points_along_paths(a0: PathCollectionResult, a1: FloatTraits) -> PointCollectionResult:
-    return PointCollectionResult(Call(Symbol('sample-points-along-paths'), [a0, a1]))
+def point_paths(a0: IdentifiablePointTraits) -> PathFeatureCollectionResult:
+    return PathFeatureCollectionResult(Call(Symbol('point-paths'), [a0]))
 
-def divide(a0: NumberTraits, a1: NumberTraits) -> NumberTraits:
-    return NumberResult(Call(Symbol('divide'), [a0, a1]))
+def distance_meters(a0: PointTraits, a1: PointTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('distance-meters'), [a0, a1]))
+
+def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('get-float'), [a0, a1]))
 
 def ll(a0: FloatTraits, a1: FloatTraits) -> PointTraits:
     return PointResult(Call(Symbol('ll'), [a0, a1]))
 
-def tile_ids_hex(a0: FeatureTraits) -> FeatureIDStringCollectionResult:
-    return FeatureIDStringCollectionResult(Call(Symbol('tile-ids-hex'), [a0]))
+def find_relations(a0: QueryTraits) -> RelationFeatureCollectionResult:
+    return RelationFeatureCollectionResult(Call(Symbol('find-relations'), [a0]))
 
-def find_relation(a0: FeatureIDTraits) -> RelationFeatureTraits:
-    return RelationFeatureResult(Call(Symbol('find-relation'), [a0]))
+def get(a0: IdentifiableTraits, a1: StringTraits) -> TagTraits:
+    return TagResult(Call(Symbol('get'), [a0, a1]))
 
-def add_ints(a0: IntTraits, a1: IntTraits) -> IntTraits:
-    return IntResult(Call(Symbol('add-ints'), [a0, a1]))
+filter = diagonal_b6.expression._filter
 
-def flattern(a0: CollectionResult) -> CollectionResult:
-    return CollectionResult(Call(Symbol('flattern'), [a0]))
+def closest_distance(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits, a3: QueryTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('closest-distance'), [a0, a1, a2, a3]))
 
-def get_int(a0: IdentifiableTraits, a1: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('get-int'), [a0, a1]))
+def cap_polygon(a0: PointTraits, a1: FloatTraits) -> AreaTraits:
+    return AreaResult(Call(Symbol('cap-polygon'), [a0, a1]))
 
-def s2_center(a0: StringTraits) -> PointTraits:
-    return PointResult(Call(Symbol('s2-center'), [a0]))
+def tile_ids(a0: FeatureTraits) -> FeatureIDIntCollectionResult:
+    return FeatureIDIntCollectionResult(Call(Symbol('tile-ids'), [a0]))
 
-def with_change(a0: ChangeTraits, a1: Callable[[],AnyTraits]) -> AnyTraits:
-    return AnyResult(Call(Symbol('with-change'), [a0, a1]))
+def find_path(a0: FeatureIDTraits) -> PathFeatureTraits:
+    return PathFeatureResult(Call(Symbol('find-path'), [a0]))
 
-def export_world(a0: StringTraits) -> IntTraits:
-    return IntResult(Call(Symbol('export-world'), [a0]))
+def sample_points(a0: PathTraits, a1: FloatTraits) -> StringPointCollectionResult:
+    return StringPointCollectionResult(Call(Symbol('sample-points'), [a0, a1]))
 
-def containing_areas(a0: PointFeatureCollectionResult, a1: QueryTraits) -> AreaFeatureCollectionResult:
-    return AreaFeatureCollectionResult(Call(Symbol('containing-areas'), [a0, a1]))
+def and_(a0: QueryTraits, a1: QueryTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('and'), [a0, a1]))
 
-def count_tag_value(a0: IdentifiableTraits, a1: StringTraits) -> CollectionResult:
-    return CollectionResult(Call(Symbol('count-tag-value'), [a0, a1]))
+def to_geojson(a0: RenderableTraits) -> GeoJSONTraits:
+    return GeoJSONResult(Call(Symbol('to-geojson'), [a0]))
 
-def reachable_area(a0: FeatureTraits, a1: StringTraits, a2: FloatTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('reachable-area'), [a0, a1, a2]))
+def debug_all_query(a0: StringTraits) -> QueryTraits:
+    return QueryResult(Call(Symbol('debug-all-query'), [a0]))
 
-def get_float(a0: IdentifiableTraits, a1: StringTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('get-float'), [a0, a1]))
+def type_point() -> QueryProtoTraits:
+    return QueryProtoResult(Call(Symbol('type-point'), []))
 
-def length(a0: PathFeatureTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('length'), [a0]))
+def type_area() -> QueryProtoTraits:
+    return QueryProtoResult(Call(Symbol('type-area'), []))
 
-def remove_tag(a0: IdentifiableTraits, a1: StringTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('remove-tag'), [a0, a1]))
+def float_value(a0: TagTraits) -> FloatTraits:
+    return FloatResult(Call(Symbol('float-value'), [a0]))
 
-def divide_int(a0: IntTraits, a1: FloatTraits) -> FloatTraits:
-    return FloatResult(Call(Symbol('divide-int'), [a0, a1]))
+def remove_tags(a0: FeatureIDStringCollectionResult) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('remove-tags'), [a0]))
 
-map = diagonal_b6.expression._map
+def apply_to_path(a0: Callable[[PathTraits],GeometryTraits]) -> Callable[[GeometryTraits],GeometryTraits]:
+    return FunctionGeometryGeometryResult(Call(Symbol('apply-to-path'), [a0]))
 
-def connect_to_network(a0: FeatureTraits) -> ChangeTraits:
-    return ChangeResult(Call(Symbol('connect-to-network'), [a0]))
+def all() -> QueryTraits:
+    return QueryResult(Call(Symbol('all'), []))
+
+def join(a0: PathTraits, a1: PathTraits) -> PathTraits:
+    return PathResult(Call(Symbol('join'), [a0, a1]))
+
+def s2_covering(a0: AreaTraits, a1: IntTraits, a2: IntTraits) -> StringStringCollectionResult:
+    return StringStringCollectionResult(Call(Symbol('s2-covering'), [a0, a1, a2]))
+
+def import_geojson_file(a0: StringTraits, a1: StringTraits) -> ChangeTraits:
+    return ChangeResult(Call(Symbol('import-geojson-file'), [a0, a1]))
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/api_pb2.py` & `diagonal_b6-0.0.3/diagonal_b6/api_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: api.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import diagonal_b6.geometry_pb2 as geometry__pb2
 import diagonal_b6.features_pb2 as features__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x03\x61pi\x1a\x0egeometry.proto\x1a\x0e\x66\x65\x61tures.proto\"]\n\x0f\x43ollectionProto\x12#\n\x04keys\x18\x02 \x03(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06values\x18\x04 \x03(\x0b\x32\x15.api.LiteralNodeProto\"X\n\tPairProto\x12$\n\x05\x66irst\x18\x01 \x01(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06second\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProto\">\n\x15ModifiedFeaturesProto\x12%\n\x03ids\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\"l\n\x12\x41ppliedChangeProto\x12*\n\x08original\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\x12*\n\x08modified\x18\x02 \x03(\x0b\x32\x18.features.FeatureIDProto\"\xb8\x01\n\tNodeProto\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12(\n\x07literal\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProtoH\x00\x12\"\n\x04\x63\x61ll\x18\x03 \x01(\x0b\x32\x12.api.CallNodeProtoH\x00\x12\'\n\x07lambda_\x18\x04 \x01(\x0b\x32\x14.api.LambdaNodeProtoH\x00\x12\r\n\x05\x42\x65gin\x18\x06 \x01(\x05\x12\x0b\n\x03\x45nd\x18\x07 \x01(\x05\x42\x06\n\x04node\"\xe9\x04\n\x10LiteralNodeProto\x12\x12\n\x08nilValue\x18\x01 \x01(\x08H\x00\x12\x13\n\tboolValue\x18\x02 \x01(\x08H\x00\x12\x15\n\x0bstringValue\x18\x03 \x01(\tH\x00\x12\x12\n\x08intValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x01H\x00\x12/\n\x0f\x63ollectionValue\x18\x06 \x01(\x0b\x32\x14.api.CollectionProtoH\x00\x12#\n\tpairValue\x18\x07 \x01(\x0b\x32\x0e.api.PairProtoH\x00\x12.\n\x0c\x66\x65\x61tureValue\x18\x08 \x01(\x0b\x32\x16.features.FeatureProtoH\x00\x12%\n\nqueryValue\x18\t \x01(\x0b\x32\x0f.api.QueryProtoH\x00\x12\x32\n\x0e\x66\x65\x61tureIDValue\x18\n \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12*\n\npointValue\x18\x0b \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12,\n\tpathValue\x18\x0c \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12\x30\n\tareaValue\x18\r \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12\x35\n\x12\x61ppliedChangeValue\x18\x0e \x01(\x0b\x32\x17.api.AppliedChangeProtoH\x00\x12\x16\n\x0cgeoJSONValue\x18\x0f \x01(\x0cH\x00\x12&\n\x08tagValue\x18\x10 \x01(\x0b\x32\x12.features.TagProtoH\x00\x42\x07\n\x05value\"O\n\rCallNodeProto\x12 \n\x08\x66unction\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x1c\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\x0e.api.NodeProto\"=\n\x0fLambdaNodeProto\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x1c\n\x04node\x18\x02 \x01(\x0b\x32\x0e.api.NodeProto\"\x1c\n\rKeyQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\"0\n\x12KeyValueQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"V\n\x0fTypedQueryProto\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.features.FeatureType\x12\x1e\n\x05query\x18\x02 \x01(\x0b\x32\x0f.api.QueryProto\"0\n\x0cQueriesProto\x12 \n\x07queries\x18\x01 \x03(\x0b\x32\x0f.api.QueryProto\"\x0f\n\rAllQueryProto\"\x11\n\x0f\x45mptyQueryProto\"F\n\x08\x43\x61pProto\x12$\n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x14.geometry.PointProto\x12\x14\n\x0cradiusMeters\x18\x02 \x01(\x01\"#\n\x0eS2CellIDsProto\x12\x11\n\ts2CellIDs\x18\x01 \x03(\x04\"\xf1\x04\n\nQueryProto\x12!\n\x03\x61ll\x18\x01 \x01(\x0b\x32\x12.api.AllQueryProtoH\x00\x12%\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\x14.api.EmptyQueryProtoH\x00\x12\x0f\n\x05keyed\x18\x03 \x01(\tH\x00\x12$\n\x06tagged\x18\x04 \x01(\x0b\x32\x12.features.TagProtoH\x00\x12%\n\x05typed\x18\x05 \x01(\x0b\x32\x14.api.TypedQueryProtoH\x00\x12)\n\x0cintersection\x18\x06 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12\"\n\x05union\x18\x07 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12&\n\rintersectsCap\x18\x08 \x01(\x0b\x32\r.api.CapProtoH\x00\x12\x35\n\x11intersectsFeature\x18\t \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12/\n\x0fintersectsPoint\x18\n \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12\x35\n\x12intersectsPolyline\x18\x0b \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12=\n\x16intersectsMultiPolygon\x18\x0c \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12.\n\x0fintersectsCells\x18\r \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x12-\n\x0emightIntersect\x18\x0e \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x42\x07\n\x05query\"C\n\x1b\x46indFeatureByIDRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\"G\n\x1c\x46indFeatureByIDResponseProto\x12\'\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32\x16.features.FeatureProto\":\n\x18\x46indFeaturesRequestProto\x12\x1e\n\x05query\x18\x01 \x01(\x0b\x32\x0f.api.QueryProto\"E\n\x19\x46indFeaturesResponseProto\x12(\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x16.features.FeatureProto\"`\n\x16ModifyTagsRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\"L\n\x1bModifyTagsBatchRequestProto\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.api.ModifyTagsRequestProto\"\x1e\n\x1cModifyTagsBatchResponseProto\"H\n\x14\x45valuateRequestProto\x12\x1f\n\x07request\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x0f\n\x07version\x18\x02 \x01(\t\"7\n\x15\x45valuateResponseProto\x12\x1e\n\x06result\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto2G\n\x02\x42\x36\x12\x41\n\x08\x45valuate\x12\x19.api.EvaluateRequestProto\x1a\x1a.api.EvaluateResponseProtoB\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tapi.proto\x12\x03\x61pi\x1a\x0egeometry.proto\x1a\x0e\x66\x65\x61tures.proto\"]\n\x0f\x43ollectionProto\x12#\n\x04keys\x18\x02 \x03(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06values\x18\x04 \x03(\x0b\x32\x15.api.LiteralNodeProto\"X\n\tPairProto\x12$\n\x05\x66irst\x18\x01 \x01(\x0b\x32\x15.api.LiteralNodeProto\x12%\n\x06second\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProto\">\n\x15ModifiedFeaturesProto\x12%\n\x03ids\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\"l\n\x12\x41ppliedChangeProto\x12*\n\x08original\x18\x01 \x03(\x0b\x32\x18.features.FeatureIDProto\x12*\n\x08modified\x18\x02 \x03(\x0b\x32\x18.features.FeatureIDProto\"\xb8\x01\n\tNodeProto\x12\x10\n\x06symbol\x18\x01 \x01(\tH\x00\x12(\n\x07literal\x18\x02 \x01(\x0b\x32\x15.api.LiteralNodeProtoH\x00\x12\"\n\x04\x63\x61ll\x18\x03 \x01(\x0b\x32\x12.api.CallNodeProtoH\x00\x12\'\n\x07lambda_\x18\x04 \x01(\x0b\x32\x14.api.LambdaNodeProtoH\x00\x12\r\n\x05\x42\x65gin\x18\x06 \x01(\x05\x12\x0b\n\x03\x45nd\x18\x07 \x01(\x05\x42\x06\n\x04node\"\xe9\x04\n\x10LiteralNodeProto\x12\x12\n\x08nilValue\x18\x01 \x01(\x08H\x00\x12\x13\n\tboolValue\x18\x02 \x01(\x08H\x00\x12\x15\n\x0bstringValue\x18\x03 \x01(\tH\x00\x12\x12\n\x08intValue\x18\x04 \x01(\x03H\x00\x12\x14\n\nfloatValue\x18\x05 \x01(\x01H\x00\x12/\n\x0f\x63ollectionValue\x18\x06 \x01(\x0b\x32\x14.api.CollectionProtoH\x00\x12#\n\tpairValue\x18\x07 \x01(\x0b\x32\x0e.api.PairProtoH\x00\x12.\n\x0c\x66\x65\x61tureValue\x18\x08 \x01(\x0b\x32\x16.features.FeatureProtoH\x00\x12%\n\nqueryValue\x18\t \x01(\x0b\x32\x0f.api.QueryProtoH\x00\x12\x32\n\x0e\x66\x65\x61tureIDValue\x18\n \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12*\n\npointValue\x18\x0b \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12,\n\tpathValue\x18\x0c \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12\x30\n\tareaValue\x18\r \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12\x35\n\x12\x61ppliedChangeValue\x18\x0e \x01(\x0b\x32\x17.api.AppliedChangeProtoH\x00\x12\x16\n\x0cgeoJSONValue\x18\x0f \x01(\x0cH\x00\x12&\n\x08tagValue\x18\x10 \x01(\x0b\x32\x12.features.TagProtoH\x00\x42\x07\n\x05value\"b\n\rCallNodeProto\x12 \n\x08\x66unction\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x1c\n\x04\x61rgs\x18\x02 \x03(\x0b\x32\x0e.api.NodeProto\x12\x11\n\tpipelined\x18\x03 \x01(\x08\"=\n\x0fLambdaNodeProto\x12\x0c\n\x04\x61rgs\x18\x01 \x03(\t\x12\x1c\n\x04node\x18\x02 \x01(\x0b\x32\x0e.api.NodeProto\"\x1c\n\rKeyQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\"0\n\x12KeyValueQueryProto\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"V\n\x0fTypedQueryProto\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.features.FeatureType\x12\x1e\n\x05query\x18\x02 \x01(\x0b\x32\x0f.api.QueryProto\"0\n\x0cQueriesProto\x12 \n\x07queries\x18\x01 \x03(\x0b\x32\x0f.api.QueryProto\"\x0f\n\rAllQueryProto\"\x11\n\x0f\x45mptyQueryProto\"F\n\x08\x43\x61pProto\x12$\n\x06\x63\x65nter\x18\x01 \x01(\x0b\x32\x14.geometry.PointProto\x12\x14\n\x0cradiusMeters\x18\x02 \x01(\x01\"#\n\x0eS2CellIDsProto\x12\x11\n\ts2CellIDs\x18\x01 \x03(\x04\"\xf1\x04\n\nQueryProto\x12!\n\x03\x61ll\x18\x01 \x01(\x0b\x32\x12.api.AllQueryProtoH\x00\x12%\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\x14.api.EmptyQueryProtoH\x00\x12\x0f\n\x05keyed\x18\x03 \x01(\tH\x00\x12$\n\x06tagged\x18\x04 \x01(\x0b\x32\x12.features.TagProtoH\x00\x12%\n\x05typed\x18\x05 \x01(\x0b\x32\x14.api.TypedQueryProtoH\x00\x12)\n\x0cintersection\x18\x06 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12\"\n\x05union\x18\x07 \x01(\x0b\x32\x11.api.QueriesProtoH\x00\x12&\n\rintersectsCap\x18\x08 \x01(\x0b\x32\r.api.CapProtoH\x00\x12\x35\n\x11intersectsFeature\x18\t \x01(\x0b\x32\x18.features.FeatureIDProtoH\x00\x12/\n\x0fintersectsPoint\x18\n \x01(\x0b\x32\x14.geometry.PointProtoH\x00\x12\x35\n\x12intersectsPolyline\x18\x0b \x01(\x0b\x32\x17.geometry.PolylineProtoH\x00\x12=\n\x16intersectsMultiPolygon\x18\x0c \x01(\x0b\x32\x1b.geometry.MultiPolygonProtoH\x00\x12.\n\x0fintersectsCells\x18\r \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x12-\n\x0emightIntersect\x18\x0e \x01(\x0b\x32\x13.api.S2CellIDsProtoH\x00\x42\x07\n\x05query\"C\n\x1b\x46indFeatureByIDRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\"G\n\x1c\x46indFeatureByIDResponseProto\x12\'\n\x07\x66\x65\x61ture\x18\x01 \x01(\x0b\x32\x16.features.FeatureProto\":\n\x18\x46indFeaturesRequestProto\x12\x1e\n\x05query\x18\x01 \x01(\x0b\x32\x0f.api.QueryProto\"E\n\x19\x46indFeaturesResponseProto\x12(\n\x08\x66\x65\x61tures\x18\x01 \x03(\x0b\x32\x16.features.FeatureProto\"`\n\x16ModifyTagsRequestProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\"L\n\x1bModifyTagsBatchRequestProto\x12-\n\x08requests\x18\x01 \x03(\x0b\x32\x1b.api.ModifyTagsRequestProto\"\x1e\n\x1cModifyTagsBatchResponseProto\"H\n\x14\x45valuateRequestProto\x12\x1f\n\x07request\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto\x12\x0f\n\x07version\x18\x02 \x01(\t\"7\n\x15\x45valuateResponseProto\x12\x1e\n\x06result\x18\x01 \x01(\x0b\x32\x0e.api.NodeProto2G\n\x02\x42\x36\x12\x41\n\x08\x45valuate\x12\x19.api.EvaluateRequestProto\x1a\x1a.api.EvaluateResponseProtoB\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\027diagonal.works/b6/proto'
-  _COLLECTIONPROTO._serialized_start=50
-  _COLLECTIONPROTO._serialized_end=143
-  _PAIRPROTO._serialized_start=145
-  _PAIRPROTO._serialized_end=233
-  _MODIFIEDFEATURESPROTO._serialized_start=235
-  _MODIFIEDFEATURESPROTO._serialized_end=297
-  _APPLIEDCHANGEPROTO._serialized_start=299
-  _APPLIEDCHANGEPROTO._serialized_end=407
-  _NODEPROTO._serialized_start=410
-  _NODEPROTO._serialized_end=594
-  _LITERALNODEPROTO._serialized_start=597
-  _LITERALNODEPROTO._serialized_end=1214
-  _CALLNODEPROTO._serialized_start=1216
-  _CALLNODEPROTO._serialized_end=1295
-  _LAMBDANODEPROTO._serialized_start=1297
-  _LAMBDANODEPROTO._serialized_end=1358
-  _KEYQUERYPROTO._serialized_start=1360
-  _KEYQUERYPROTO._serialized_end=1388
-  _KEYVALUEQUERYPROTO._serialized_start=1390
-  _KEYVALUEQUERYPROTO._serialized_end=1438
-  _TYPEDQUERYPROTO._serialized_start=1440
-  _TYPEDQUERYPROTO._serialized_end=1526
-  _QUERIESPROTO._serialized_start=1528
-  _QUERIESPROTO._serialized_end=1576
-  _ALLQUERYPROTO._serialized_start=1578
-  _ALLQUERYPROTO._serialized_end=1593
-  _EMPTYQUERYPROTO._serialized_start=1595
-  _EMPTYQUERYPROTO._serialized_end=1612
-  _CAPPROTO._serialized_start=1614
-  _CAPPROTO._serialized_end=1684
-  _S2CELLIDSPROTO._serialized_start=1686
-  _S2CELLIDSPROTO._serialized_end=1721
-  _QUERYPROTO._serialized_start=1724
-  _QUERYPROTO._serialized_end=2349
-  _FINDFEATUREBYIDREQUESTPROTO._serialized_start=2351
-  _FINDFEATUREBYIDREQUESTPROTO._serialized_end=2418
-  _FINDFEATUREBYIDRESPONSEPROTO._serialized_start=2420
-  _FINDFEATUREBYIDRESPONSEPROTO._serialized_end=2491
-  _FINDFEATURESREQUESTPROTO._serialized_start=2493
-  _FINDFEATURESREQUESTPROTO._serialized_end=2551
-  _FINDFEATURESRESPONSEPROTO._serialized_start=2553
-  _FINDFEATURESRESPONSEPROTO._serialized_end=2622
-  _MODIFYTAGSREQUESTPROTO._serialized_start=2624
-  _MODIFYTAGSREQUESTPROTO._serialized_end=2720
-  _MODIFYTAGSBATCHREQUESTPROTO._serialized_start=2722
-  _MODIFYTAGSBATCHREQUESTPROTO._serialized_end=2798
-  _MODIFYTAGSBATCHRESPONSEPROTO._serialized_start=2800
-  _MODIFYTAGSBATCHRESPONSEPROTO._serialized_end=2830
-  _EVALUATEREQUESTPROTO._serialized_start=2832
-  _EVALUATEREQUESTPROTO._serialized_end=2904
-  _EVALUATERESPONSEPROTO._serialized_start=2906
-  _EVALUATERESPONSEPROTO._serialized_end=2961
-  _B6._serialized_start=2963
-  _B6._serialized_end=3034
+  _globals['_COLLECTIONPROTO']._serialized_start=50
+  _globals['_COLLECTIONPROTO']._serialized_end=143
+  _globals['_PAIRPROTO']._serialized_start=145
+  _globals['_PAIRPROTO']._serialized_end=233
+  _globals['_MODIFIEDFEATURESPROTO']._serialized_start=235
+  _globals['_MODIFIEDFEATURESPROTO']._serialized_end=297
+  _globals['_APPLIEDCHANGEPROTO']._serialized_start=299
+  _globals['_APPLIEDCHANGEPROTO']._serialized_end=407
+  _globals['_NODEPROTO']._serialized_start=410
+  _globals['_NODEPROTO']._serialized_end=594
+  _globals['_LITERALNODEPROTO']._serialized_start=597
+  _globals['_LITERALNODEPROTO']._serialized_end=1214
+  _globals['_CALLNODEPROTO']._serialized_start=1216
+  _globals['_CALLNODEPROTO']._serialized_end=1314
+  _globals['_LAMBDANODEPROTO']._serialized_start=1316
+  _globals['_LAMBDANODEPROTO']._serialized_end=1377
+  _globals['_KEYQUERYPROTO']._serialized_start=1379
+  _globals['_KEYQUERYPROTO']._serialized_end=1407
+  _globals['_KEYVALUEQUERYPROTO']._serialized_start=1409
+  _globals['_KEYVALUEQUERYPROTO']._serialized_end=1457
+  _globals['_TYPEDQUERYPROTO']._serialized_start=1459
+  _globals['_TYPEDQUERYPROTO']._serialized_end=1545
+  _globals['_QUERIESPROTO']._serialized_start=1547
+  _globals['_QUERIESPROTO']._serialized_end=1595
+  _globals['_ALLQUERYPROTO']._serialized_start=1597
+  _globals['_ALLQUERYPROTO']._serialized_end=1612
+  _globals['_EMPTYQUERYPROTO']._serialized_start=1614
+  _globals['_EMPTYQUERYPROTO']._serialized_end=1631
+  _globals['_CAPPROTO']._serialized_start=1633
+  _globals['_CAPPROTO']._serialized_end=1703
+  _globals['_S2CELLIDSPROTO']._serialized_start=1705
+  _globals['_S2CELLIDSPROTO']._serialized_end=1740
+  _globals['_QUERYPROTO']._serialized_start=1743
+  _globals['_QUERYPROTO']._serialized_end=2368
+  _globals['_FINDFEATUREBYIDREQUESTPROTO']._serialized_start=2370
+  _globals['_FINDFEATUREBYIDREQUESTPROTO']._serialized_end=2437
+  _globals['_FINDFEATUREBYIDRESPONSEPROTO']._serialized_start=2439
+  _globals['_FINDFEATUREBYIDRESPONSEPROTO']._serialized_end=2510
+  _globals['_FINDFEATURESREQUESTPROTO']._serialized_start=2512
+  _globals['_FINDFEATURESREQUESTPROTO']._serialized_end=2570
+  _globals['_FINDFEATURESRESPONSEPROTO']._serialized_start=2572
+  _globals['_FINDFEATURESRESPONSEPROTO']._serialized_end=2641
+  _globals['_MODIFYTAGSREQUESTPROTO']._serialized_start=2643
+  _globals['_MODIFYTAGSREQUESTPROTO']._serialized_end=2739
+  _globals['_MODIFYTAGSBATCHREQUESTPROTO']._serialized_start=2741
+  _globals['_MODIFYTAGSBATCHREQUESTPROTO']._serialized_end=2817
+  _globals['_MODIFYTAGSBATCHRESPONSEPROTO']._serialized_start=2819
+  _globals['_MODIFYTAGSBATCHRESPONSEPROTO']._serialized_end=2849
+  _globals['_EVALUATEREQUESTPROTO']._serialized_start=2851
+  _globals['_EVALUATEREQUESTPROTO']._serialized_end=2923
+  _globals['_EVALUATERESPONSEPROTO']._serialized_start=2925
+  _globals['_EVALUATERESPONSEPROTO']._serialized_end=2980
+  _globals['_B6']._serialized_start=2982
+  _globals['_B6']._serialized_end=3053
 # @@protoc_insertion_point(module_scope)
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/api_pb2_grpc.py` & `diagonal_b6-0.0.3/diagonal_b6/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.2/diagonal_b6/b6_test.py` & `diagonal_b6-0.0.3/diagonal_b6/b6_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 
 class B6Test(unittest.TestCase):
 
     def __init__(self, name, connection):
         unittest.TestCase.__init__(self, name)
         self.connection = connection
 
+    def test_get_tag(self):
+        name = b6.find_feature(b6.osm_way_area_id(LIGHTERMAN_WAY_ID)).get("name")
+        self.assertEqual(("name", "The Lighterman"), self.connection(name))
+
     def test_find_areas(self):
         names = [building.get_string("name") for (id, building) in self.connection(b6.find_areas(b6.keyed("#building")))]
         self.assertEqual(len(names), BUILDINGS_IN_GRANARY_SQUARE)
 
     def test_find_point_by_id(self):        
         area = self.connection(b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_SOUTH_END_ID)))
         self.assertEqual(area.id.value, STABLE_STREET_BRIDGE_SOUTH_END_ID)
@@ -61,14 +65,18 @@
     def test_find_area_by_wrong_id_type(self):
         with self.assertRaises(Exception): # TODO: Make more specific
             self.connection(b6.find_area(b6.osm_node_id(STABLE_STREET_BRIDGE_SOUTH_END_ID)))
 
     def test_uk_ons_boundary_id(self):
         self.assertEqual(b6.uk_ons_boundary_id("E01000953").value, 76343044687353)
 
+    def test_area_str(self):
+        area = self.connection(b6.find_area(b6.osm_way_area_id(COAL_DROPS_YARD_WEST_BUILDING_ID)))
+        self.assertEqual("<Area /area/openstreetmap.org/way/222021572>", str(area))
+
     def test_relation_members(self):
         greenway = self.connection(b6.find_relation(b6.osm_relation_id(JUBILEE_GREENWAY_ID)))
         paths = ([str(m) for m in greenway.members() if m.is_path()])
         self.assertGreater(len(paths), 10)
         self.assertLess(len(paths), 800)
 
     def test_or_query(self):
@@ -78,14 +86,19 @@
     def test_point_degree(self):
         self.assertEqual(self.connection(b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_NORTH_END_ID)).degree()), STABLE_STREET_BRIDGE_NORTH_END_DEGREE)
         degrees = [degree for (id, degree) in self.connection(b6.find_points(b6.within_cap(b6.ll(51.535241, -0.124364), 100)).degree())]
         for d in degrees:
             self.assertGreaterEqual(d, 0)
             self.assertLess(d, 10)
 
+    def test_send_evaluated_feature_back_to_server(self):
+        point = self.connection(b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_NORTH_END_ID)))
+        degree = self.connection(b6.degree(point))
+        self.assertEqual(degree, self.connection(b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_NORTH_END_ID)).degree()))
+
     def test_path_lengths(self):
         lengths = [length for (id, length) in self.connection(b6.find_paths(b6.keyed("#highway")).length())]
         self.assertGreater(len(lengths), 0)
         for l in lengths:
             self.assertGreater(l, 0)
             self.assertLess(l, 1000)
 
@@ -456,14 +469,30 @@
     def test_evaluate_with_changed_world(self):
         close_road = b6.remove_tag(b6.osm_way_id(STABLE_STREET_BRIDGE_ID), "#highway")
         reachable = b6.find_point(b6.osm_node_id(STABLE_STREET_BRIDGE_SOUTH_END_ID)).reachable("walk", 200.0, b6.keyed("#amenity")).get_string("name")
         before = len(self.connection(reachable))
         after = len(self.connection(b6.with_change(close_road, lambda: reachable)))
         self.assertGreater(before, after)
 
+    def test_get_tags_from_list_of_ids(self):
+        names = b6.feature_ids([b6.osm_way_area_id(id) for id in (LIGHTERMAN_WAY_ID, GRANARY_SQUARE_WAY_ID)]).map(lambda f: f.get_string("name"))
+        expected = [(0, "The Lighterman"), (1, "Granary Square")]
+        self.assertEqual(expected, self.connection(names))
+
+    def test_make_tags_from_list_of_strings(self):
+        tags = b6.strings(["primary", "secondary"]).map(lambda v: b6.tag("#highway", v))
+        expected = [(0, ("#highway", "primary")), (1, ("#highway", "secondary"))]
+        self.assertEqual(expected, self.connection(tags))
+
+    def test_convex_hull_from_list_of_lat_lngs(self):
+        caps = b6.lls([(51.535387, -0.125277), (51.537088, -0.125781)]).map(lambda c: b6.cap_polygon(c, 20.0))
+        areas = self.connection(caps.map(b6.area))
+        hull_area = self.connection(b6.convex_hull(caps).area())
+        self.assertGreater(hull_area, sum([a for _, a in areas]))
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("--http-port", default="10080", help="Host and port on which to serve HTTP")
     parser.add_argument("--grpc-port", default="10081", help="Host and port on which to serve GRPC")
     parser.add_argument("--platform", default=None, help="Current platform, eg darwin/x86_64")
     parser.add_argument("tests", type=str, nargs="*")
     args = parser.parse_args()
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/connect.py` & `diagonal_b6-0.0.3/diagonal_b6/connect.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.2/diagonal_b6/expression.py` & `diagonal_b6-0.0.3/diagonal_b6/expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 def register_literal(oneof, from_proto):
     _literals[oneof] = from_proto
 
 register_literal("nilValue", lambda v: None)
 register_literal("intValue", lambda v: v)
 register_literal("floatValue", lambda v: v)
 register_literal("stringValue", lambda v: v)
+register_literal("tagValue", lambda v: (v.key, v.value))
 register_literal("geoJSONValue", lambda v: json.loads(gzip.decompress(v)))
 
 def from_literal_node_proto(literal):
     oneof = literal.WhichOneof("value")
     from_proto = _literals.get(oneof, None)
     if from_proto is not None:
         return from_proto(getattr(literal, oneof))
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/features.py` & `diagonal_b6-0.0.3/diagonal_b6/features.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         l.featureIDValue.type = self.type
         l.featureIDValue.namespace = self.namespace
         l.featureIDValue.value = self.value
         return l
 
     def __str__(self):
         type = features_pb2.FeatureType.Name(self.type).replace("FeatureType", "").lower()
-        return "%s/%s/%d" % (type, self.namespace, self.value)
+        return "/%s/%s/%d" % (type, self.namespace, self.value)
 
     def __repr__(self):
         return str(self)
 
     def __eq__(self, other):
         return self.type == other.type and self.namespace == other.namespace and self.value == other.value
 
@@ -54,15 +54,15 @@
         return hash(self.type) ^ hash(self.namespace) ^ hash(self.value)
 
     def _fill_query(self, query):
         query.spatial.area.id.type = self.type
         query.spatial.area.id.namespace = self.namespace
         query.spatial.area.id.value = self.value
 
-class Feature:
+class Feature(expression.Node):
 
     def is_point(self):
         return self.id.is_point()
 
     def is_path(self):
         return self.id.is_path()
     
@@ -101,18 +101,23 @@
             except:
                 pass
         return 0
 
     def all_tags(self):
         return [(tag.key, tag.value) for tag in self._pb.tags]
 
+    def to_node_proto(self):
+        node = api_pb2.NodeProto()
+        node.call.function.symbol = "find-feature"
+        node.call.args.add().CopyFrom(self.id.to_node_proto())
+        return node
+
     def __str__(self):
         type = features_pb2.FeatureType.Name(self.id.type).replace("FeatureType", "").title()
-        namespace = features_pb2.FeatureIDProto.Namespace.Name(self.id.namespace).replace("Namespace", "").lower()
-        return "<%s %s:%d>" % (type, namespace, self.id.value)
+        return "<%s %s>" % (type, self.id)
 
     def _fill_query(self, query):
         return self.id._fill_query(query)
 
 class PointFeature(Feature):
 
     def __init__(self, p):
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/features_pb2.py` & `diagonal_b6-0.0.3/diagonal_b6/features_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: features.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import diagonal_b6.geometry_pb2 as geometry__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x66\x65\x61tures.proto\x12\x08\x66\x65\x61tures\x1a\x0egeometry.proto\"&\n\x08TagProto\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"W\n\x0e\x46\x65\x61tureIDProto\x12#\n\x04type\x18\x01 \x01(\x0e\x32\x15.features.FeatureType\x12\x11\n\tnamespace\x18\x02 \x01(\t\x12\r\n\x05value\x18\x03 \x01(\x04\"\x80\x01\n\x11PointFeatureProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\x12#\n\x05point\x18\x03 \x01(\x0b\x32\x14.geometry.PointProto\"\x9f\x01\n\x10PathFeatureProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\x12-\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32\x1b.features.PointFeatureProto\x12\x14\n\x0clengthMeters\x18\x04 \x01(\x01\">\n\x11PathFeaturesProto\x12)\n\x05paths\x18\x01 \x03(\x0b\x32\x1a.features.PathFeatureProto\"\x89\x01\n\x10\x41reaFeatureProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\x12-\n\x08\x66\x65\x61tures\x18\x03 \x03(\x0b\x32\x1b.features.PathFeaturesProto\"I\n\x13RelationMemberProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12\x0c\n\x04role\x18\x03 \x01(\t\"\x8e\x01\n\x14RelationFeatureProto\x12$\n\x02id\x18\x01 \x01(\x0b\x32\x18.features.FeatureIDProto\x12 \n\x04tags\x18\x02 \x03(\x0b\x32\x12.features.TagProto\x12.\n\x07members\x18\x03 \x03(\x0b\x32\x1d.features.RelationMemberProto\"\xd3\x01\n\x0c\x46\x65\x61tureProto\x12,\n\x05point\x18\x01 \x01(\x0b\x32\x1b.features.PointFeatureProtoH\x00\x12*\n\x04path\x18\x02 \x01(\x0b\x32\x1a.features.PathFeatureProtoH\x00\x12*\n\x04\x61rea\x18\x03 \x01(\x0b\x32\x1a.features.AreaFeatureProtoH\x00\x12\x32\n\x08relation\x18\x04 \x01(\x0b\x32\x1e.features.RelationFeatureProtoH\x00\x42\t\n\x07\x66\x65\x61ture*~\n\x0b\x46\x65\x61tureType\x12\x14\n\x10\x46\x65\x61tureTypePoint\x10\x00\x12\x13\n\x0f\x46\x65\x61tureTypePath\x10\x01\x12\x13\n\x0f\x46\x65\x61tureTypeArea\x10\x02\x12\x17\n\x13\x46\x65\x61tureTypeRelation\x10\x03\x12\x16\n\x12\x46\x65\x61tureTypeInvalid\x10\x04\x42\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'features_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'features_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\027diagonal.works/b6/proto'
-  _FEATURETYPE._serialized_start=1104
-  _FEATURETYPE._serialized_end=1230
-  _TAGPROTO._serialized_start=44
-  _TAGPROTO._serialized_end=82
-  _FEATUREIDPROTO._serialized_start=84
-  _FEATUREIDPROTO._serialized_end=171
-  _POINTFEATUREPROTO._serialized_start=174
-  _POINTFEATUREPROTO._serialized_end=302
-  _PATHFEATUREPROTO._serialized_start=305
-  _PATHFEATUREPROTO._serialized_end=464
-  _PATHFEATURESPROTO._serialized_start=466
-  _PATHFEATURESPROTO._serialized_end=528
-  _AREAFEATUREPROTO._serialized_start=531
-  _AREAFEATUREPROTO._serialized_end=668
-  _RELATIONMEMBERPROTO._serialized_start=670
-  _RELATIONMEMBERPROTO._serialized_end=743
-  _RELATIONFEATUREPROTO._serialized_start=746
-  _RELATIONFEATUREPROTO._serialized_end=888
-  _FEATUREPROTO._serialized_start=891
-  _FEATUREPROTO._serialized_end=1102
+  _globals['_FEATURETYPE']._serialized_start=1104
+  _globals['_FEATURETYPE']._serialized_end=1230
+  _globals['_TAGPROTO']._serialized_start=44
+  _globals['_TAGPROTO']._serialized_end=82
+  _globals['_FEATUREIDPROTO']._serialized_start=84
+  _globals['_FEATUREIDPROTO']._serialized_end=171
+  _globals['_POINTFEATUREPROTO']._serialized_start=174
+  _globals['_POINTFEATUREPROTO']._serialized_end=302
+  _globals['_PATHFEATUREPROTO']._serialized_start=305
+  _globals['_PATHFEATUREPROTO']._serialized_end=464
+  _globals['_PATHFEATURESPROTO']._serialized_start=466
+  _globals['_PATHFEATURESPROTO']._serialized_end=528
+  _globals['_AREAFEATUREPROTO']._serialized_start=531
+  _globals['_AREAFEATUREPROTO']._serialized_end=668
+  _globals['_RELATIONMEMBERPROTO']._serialized_start=670
+  _globals['_RELATIONMEMBERPROTO']._serialized_end=743
+  _globals['_RELATIONFEATUREPROTO']._serialized_start=746
+  _globals['_RELATIONFEATUREPROTO']._serialized_end=888
+  _globals['_FEATUREPROTO']._serialized_start=891
+  _globals['_FEATUREPROTO']._serialized_end=1102
 # @@protoc_insertion_point(module_scope)
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/generate_api.py` & `diagonal_b6-0.0.3/diagonal_b6/generate_api.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.2/diagonal_b6/geometry.py` & `diagonal_b6-0.0.3/diagonal_b6/geometry.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 from diagonal_b6 import geometry_pb2
 
 def from_point_proto(p):
     return (float(p.lat_e7) / 1e7, float(p.lng_e7) / 1e7)
 
 expression.register_literal("pointValue", from_point_proto)
 
+def to_point_proto(ll):
+    p = geometry_pb2.PointProto()
+    p.lat_e7 = int(ll[0] * 1e7)
+    p.lng_e7 = int(ll[1] * 1e7)
+    return p
+
 def from_polyline_proto(p):
     return Polyline(p)
 
 expression.register_literal("pathValue", from_polyline_proto)
 
 def from_multipolygon_proto(p):
     return MultiPolygon(p)
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/geometry_pb2.py` & `diagonal_b6-0.0.3/diagonal_b6/geometry_pb2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: geometry.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0egeometry.proto\x12\x08geometry\"L\n\rPolylineProto\x12$\n\x06points\x18\x01 \x03(\x0b\x32\x14.geometry.PointProto\x12\x15\n\rlength_meters\x18\x02 \x01(\x01\"=\n\x11MultiPolygonProto\x12(\n\x08polygons\x18\x01 \x03(\x0b\x32\x16.geometry.PolygonProto\"2\n\x0cPolygonProto\x12\"\n\x05loops\x18\x01 \x03(\x0b\x32\x13.geometry.LoopProto\"1\n\tLoopProto\x12$\n\x06points\x18\x01 \x03(\x0b\x32\x14.geometry.PointProto\",\n\nPointProto\x12\x0e\n\x06lat_e7\x18\x01 \x01(\x05\x12\x0e\n\x06lng_e7\x18\x02 \x01(\x05\x42\x19Z\x17\x64iagonal.works/b6/protob\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'geometry_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'geometry_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z\027diagonal.works/b6/proto'
-  _POLYLINEPROTO._serialized_start=28
-  _POLYLINEPROTO._serialized_end=104
-  _MULTIPOLYGONPROTO._serialized_start=106
-  _MULTIPOLYGONPROTO._serialized_end=167
-  _POLYGONPROTO._serialized_start=169
-  _POLYGONPROTO._serialized_end=219
-  _LOOPPROTO._serialized_start=221
-  _LOOPPROTO._serialized_end=270
-  _POINTPROTO._serialized_start=272
-  _POINTPROTO._serialized_end=316
+  _globals['_POLYLINEPROTO']._serialized_start=28
+  _globals['_POLYLINEPROTO']._serialized_end=104
+  _globals['_MULTIPOLYGONPROTO']._serialized_start=106
+  _globals['_MULTIPOLYGONPROTO']._serialized_end=167
+  _globals['_POLYGONPROTO']._serialized_start=169
+  _globals['_POLYGONPROTO']._serialized_end=219
+  _globals['_LOOPPROTO']._serialized_start=221
+  _globals['_LOOPPROTO']._serialized_end=270
+  _globals['_POINTPROTO']._serialized_start=272
+  _globals['_POINTPROTO']._serialized_end=316
 # @@protoc_insertion_point(module_scope)
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6/query.py` & `diagonal_b6-0.0.3/diagonal_b6/query.py`

 * *Files identical despite different names*

### Comparing `diagonal_b6-0.0.2/diagonal_b6.egg-info/PKG-INFO` & `diagonal_b6-0.0.3/diagonal_b6.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagonal-b6
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client library for b6, Diagonal's geospatial analysis engine.
 Author-email: Diagonal Works <hello@diagonal.works>
 License: Apache License
 Project-URL: Homepage, https://diagonal.works/b6
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `diagonal_b6-0.0.2/diagonal_b6.egg-info/SOURCES.txt` & `diagonal_b6-0.0.3/diagonal_b6.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 README.md
 pyproject.toml
 diagonal_b6/__init__.py
 diagonal_b6/api_generated.py
 diagonal_b6/api_pb2.py
 diagonal_b6/api_pb2_grpc.py
 diagonal_b6/b6_test.py
+diagonal_b6/collection.py
 diagonal_b6/connect.py
 diagonal_b6/expression.py
 diagonal_b6/features.py
 diagonal_b6/features_pb2.py
-diagonal_b6/features_pb2_grpc.py
 diagonal_b6/generate_api.py
 diagonal_b6/geometry.py
 diagonal_b6/geometry_pb2.py
-diagonal_b6/geometry_pb2_grpc.py
 diagonal_b6/query.py
 diagonal_b6.egg-info/PKG-INFO
 diagonal_b6.egg-info/SOURCES.txt
 diagonal_b6.egg-info/dependency_links.txt
 diagonal_b6.egg-info/requires.txt
 diagonal_b6.egg-info/top_level.txt
```

### Comparing `diagonal_b6-0.0.2/pyproject.toml` & `diagonal_b6-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "diagonal_b6"
 description = "A Python client library for b6, Diagonal's geospatial analysis engine."
 readme = "README.md"
 license = {text = "Apache License"}
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   {name="Diagonal Works", email="hello@diagonal.works"},
 ]
 requires-python = ">=3.10"
 dependencies = [
     "grpcio>=1.43.0",
     "protobuf>=3.14.0",
```

