# Comparing `tmp/antimeridian-0.2.6.tar.gz` & `tmp/antimeridian-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.2.6.tar", last modified: Wed May 31 18:12:09 2023, max compression
+gzip compressed data, was "antimeridian-0.3.0.tar", last modified: Thu Jun 29 13:43:08 2023, max compression
```

## Comparing `antimeridian-0.2.6.tar` & `antimeridian-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-05-31 18:12:01.000000 antimeridian-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 18:12:09.593973 antimeridian-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-31 18:12:01.000000 antimeridian-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-31 18:12:01.000000 antimeridian-0.2.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 18:12:09.593973 antimeridian-0.2.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-05-31 18:12:01.000000 antimeridian-0.2.6/src/antimeridian/_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 18:12:09.000000 antimeridian-0.2.6/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 18:12:09.593973 antimeridian-0.2.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-31 18:12:01.000000 antimeridian-0.2.6/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.762039 antimeridian-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9723 2023-06-29 13:42:59.000000 antimeridian-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-29 13:43:08.762039 antimeridian-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-29 13:42:59.000000 antimeridian-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-29 13:42:59.000000 antimeridian-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 13:43:08.762039 antimeridian-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.754038 antimeridian-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-06-29 13:42:59.000000 antimeridian-0.3.0/src/antimeridian/_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 13:43:08.000000 antimeridian-0.3.0/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 13:43:08.758039 antimeridian-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-29 13:42:59.000000 antimeridian-0.3.0/tests/test_segment.py
```

### Comparing `antimeridian-0.2.6/LICENSE` & `antimeridian-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.6/PKG-INFO` & `antimeridian-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.6
+Version: 0.3.0
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.6/README.md` & `antimeridian-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.6/pyproject.toml` & `antimeridian-0.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "antimeridian"
-version = "0.2.6"
+version = "0.3.0"
 authors = [
     {name = "Pete Gadomski", email = "pete.gadomski@gmail.com"}
 ]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
@@ -30,25 +30,25 @@
     "black~=23.3",
     "blacken-docs~=1.13",
     "mypy~=1.2",
     "packaging~=23.1",
     "pre-commit~=3.2",
     "pytest~=7.3",
     "pytest-console-scripts~=1.3",
-    "ruff==0.0.270",
+    "ruff==0.0.275",
     "tomli~=2.0; python_version<'3.11'"
 ]
 docs = [
     "cartopy~=0.21",
     "ipykernel~=6.22",
     "jupytext~=1.14",
     "nbsphinx~=0.9",
     "pydata-sphinx-theme~=0.13",
-    "scipy~=1.10",
-    "sphinx>=6.1,<8.0",
+    "scipy~=1.10.0",  # need to stay below 1.11 due to https://github.com/SciTools/cartopy/issues/2199
+    "sphinx~=7.0",
     "sphinx-click~=4.4",
 ]
 
 [project.scripts]
 antimeridian = "antimeridian._cli:cli"
 
 [tool.ruff]
```

### Comparing `antimeridian-0.2.6/src/antimeridian/_cli.py` & `antimeridian-0.3.0/src/antimeridian/_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,23 +39,37 @@
 @click.option(
     "--force-south-pole",
     is_flag=True,
     show_default=True,
     default=False,
     help="Force the fixed polygon to enclose the south pole",
 )
-def fix(infile: str, force_north_pole: bool, force_south_pole: bool) -> None:
+@click.option(
+    "--fix-winding/--no-fix-winding",
+    show_default=True,
+    default=True,
+    help=(
+        "Automatically fix clockwise polygons to be the correct counterclockwise "
+        "winding order"
+    ),
+)
+def fix(
+    infile: str, force_north_pole: bool, force_south_pole: bool, fix_winding: bool
+) -> None:
     """Fixes any antimeridian problems a GeoJSON file
 
     Writes the fixed GeoJSON to standard output.
     """
     with open(infile) as f:
         data = json.load(f)
     fixed = antimeridian.fix_geojson(
-        data, force_north_pole=force_north_pole, force_south_pole=force_south_pole
+        data,
+        force_north_pole=force_north_pole,
+        force_south_pole=force_south_pole,
+        fix_winding=fix_winding,
     )
     print(json.dumps(fixed))
 
 
 @cli.command()
 @click.argument("infile", type=str)
 @click.option(
```

### Comparing `antimeridian-0.2.6/src/antimeridian/_implementation.py` & `antimeridian-0.3.0/src/antimeridian/_implementation.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,23 +4,48 @@
 should not use these functions and objects directly; instead, use the functions
 explicitly imported into the top-level of the package. The interfaces in this
 module can change at any time without warning.
 """
 
 from __future__ import annotations
 
+import copy
+import warnings
 from typing import Any, Dict, List, Optional, Protocol, Tuple, Union, cast
 
 import shapely
 import shapely.geometry
-from shapely.geometry import MultiLineString, MultiPolygon, Polygon
+from shapely.geometry import LinearRing, MultiLineString, MultiPolygon, Polygon
 
 Point = Tuple[float, float]
 
 
+class AntimeridianWarning(UserWarning):
+    """Base class for all package-specific warnings."""
+
+
+class FixWindingWarning(AntimeridianWarning):
+    """The input shape is wound clockwise (instead of counter-clockwise), so
+    this package is reversing the winding order before fixing the shape.
+    """
+
+    MESSAGE = (
+        "The exterior ring of this shape is wound "
+        "clockwise. Since this is a common error in real-world "
+        "geometries, this package is reversing the exterior coordinates of the "
+        "input shape before running its algorithm. If you know that your input "
+        "shape is correct (i.e. if your data encompasses both poles), pass "
+        "`fix_winding=False`."
+    )
+
+    @classmethod
+    def warn(cls) -> None:
+        warnings.warn(cls.MESSAGE, cls, stacklevel=2)
+
+
 class GeoInterface(Protocol):
     """A simple protocol for things that have a ``__geo_interface__`` method.
 
     The ``__geo_interface__`` protocol is described `here
     <https://gist.github.com/sgillies/2217756>`_, and is used within `shapely
     <https://shapely.readthedocs.io/en/stable/manual.html>`_ to
     extract geometries from objects.
@@ -31,28 +56,31 @@
 
 
 def fix_geojson(
     geojson: Dict[str, Any],
     *,
     force_north_pole: bool = False,
     force_south_pole: bool = False,
+    fix_winding: bool = True,
 ) -> Dict[str, Any]:
     """Fixes a GeoJSON object that crosses the antimeridian.
 
     If the object does not cross the antimeridian, it is returned unchanged.
 
-    See :py:func:`fix_polygon` for a description of the ``force_north_pole`` and
-    ``force_south_pole`` arguments.
+    See :py:func:`fix_polygon` for a description of the ``force_north_pole``,
+    ``force_south_pole``, and ``fix_winding`` arguments.
 
     Args:
         geojson: A GeoJSON object as a dictionary
         force_north_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the north pole.
         force_south_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the south pole.
+        fix_winding: If the polygon is wound clockwise, reverse its
+            coordinates before applying the algorithm.
 
     Return:
         The same GeoJSON with a fixed geometry or geometries
     """
     type_ = geojson.get("type", None)
     if type_ is None:
         raise ValueError("no 'type' field found in GeoJSON")
@@ -60,33 +88,36 @@
         geometry = geojson.get("geometry", None)
         if geometry is None:
             raise ValueError("no 'geometry' field found in GeoJSON Feature")
         geojson["geometry"] = fix_shape(
             geometry,
             force_north_pole=force_north_pole,
             force_south_pole=force_south_pole,
+            fix_winding=fix_winding,
         )
         return geojson
     elif type_ == "FeatureCollection":
         features = geojson.get("features", None)
         if features is None:
             raise ValueError("no 'features' field found in GeoJSON FeatureCollection")
         for i, feature in enumerate(features):
             features[i] = fix_geojson(
                 feature,
                 force_north_pole=force_north_pole,
                 force_south_pole=force_south_pole,
+                fix_winding=fix_winding,
             )
         geojson["features"] = features
         return geojson
     else:
         return fix_shape(
             geojson,
             force_north_pole=force_north_pole,
             force_south_pole=force_south_pole,
+            fix_winding=fix_winding,
         )
 
 
 def segment_geojson(geojson: Dict[str, Any]) -> MultiLineString:
     """Segments a GeoJSON object into a MultiLineString.
 
     If the object does not cross the antimeridian, its exterior and interior
@@ -119,52 +150,57 @@
 
 
 def fix_shape(
     shape: Dict[str, Any] | GeoInterface,
     *,
     force_north_pole: bool = False,
     force_south_pole: bool = False,
+    fix_winding: bool = True,
 ) -> Dict[str, Any]:
     """Fixes a shape that crosses the antimeridian.
 
-    See :py:func:`fix_polygon` for a description of the ``force_north_pole`` and
-    ``force_south_pole`` arguments.
+    See :py:func:`fix_polygon` for a description of the ``force_north_pole``,
+    ``force_south_pole``, and ``fix_winding`` arguments.
 
     Args:
         shape: A polygon or multi-polygon, either as a dictionary or as a
             :py:class:`GeoInterface`. Uses :py:func:`shapely.geometry.shape`
             under the hood.
         force_north_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the north pole.
         force_south_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the south pole.
+        fix_winding: If the polygon is wound clockwise, reverse its
+            coordinates before applying the algorithm.
 
     Returns:
         The fixed shape as a dictionary
     """
     geom = shapely.geometry.shape(shape)
     if geom.geom_type == "Polygon":
         return cast(
             Dict[str, Any],
             shapely.geometry.mapping(
                 fix_polygon(
                     geom,
                     force_north_pole=force_north_pole,
                     force_south_pole=force_south_pole,
+                    fix_winding=fix_winding,
                 )
             ),
         )
     elif geom.geom_type == "MultiPolygon":
         return cast(
             Dict[str, Any],
             shapely.geometry.mapping(
                 fix_multi_polygon(
                     geom,
                     force_north_pole=force_north_pole,
                     force_south_pole=force_south_pole,
+                    fix_winding=fix_winding,
                 )
             ),
         )
     else:
         raise ValueError(f"unsupported geom_type: {geom.geom_type}")
 
 
@@ -182,69 +218,88 @@
 
 
 def fix_multi_polygon(
     multi_polygon: MultiPolygon,
     *,
     force_north_pole: bool = False,
     force_south_pole: bool = False,
+    fix_winding: bool = True,
 ) -> MultiPolygon:
     """Fixes a :py:class:`shapely.geometry.MultiPolygon`.
 
-    See :py:func:`fix_polygon` for a description of the ``force_north_pole`` and
-    ``force_south_pole`` arguments.
+    See :py:func:`fix_polygon` for a description of the ``force_north_pole``,
+    ``force_south_pole``, and ``fix_winding`` arguments.
 
     Args:
         multi_polygon: The multi-polygon
         force_north_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the north pole.
         force_south_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the south pole.
+        fix_winding: If the polygon is wound clockwise, reverse its
+            coordinates before applying the algorithm.
 
     Returns:
         The fixed multi-polygon
     """
     polygons = list()
     for polygon in multi_polygon.geoms:
         polygons += fix_polygon_to_list(
             polygon,
             force_north_pole=force_north_pole,
             force_south_pole=force_south_pole,
+            fix_winding=fix_winding,
         )
     return MultiPolygon(polygons)
 
 
 def fix_polygon(
-    polygon: Polygon, *, force_north_pole: bool = False, force_south_pole: bool = False
+    polygon: Polygon,
+    *,
+    force_north_pole: bool = False,
+    force_south_pole: bool = False,
+    fix_winding: bool = True,
 ) -> Union[Polygon, MultiPolygon]:
     """Fixes a :py:class:`shapely.geometry.Polygon`.
 
-    If the input polygon is a single polygon that is wound clockwise and doesn't
-    cross the antimeridian, it will be corrected by adding a counter-clockwise
-    polygon from (-180, -90) to (180, 90) as its exterior.
+    If the input polygon is wound clockwise, it will be fixed to be wound
+    counterclockwise _unless_ ``fix_winding`` is ``False``, in which case it
+    will be corrected by adding a counterclockwise polygon from (-180, -90) to
+    (180, 90) as its exterior.
 
     In rare cases, the underlying algorithm might need a little help to fix the polygon.
     For example, a polygon that just barely crosses over a pole might have very
     few points at high latitudes, leading to ambiguous antimeridian crossing
     points and invalid geometries. We provide two flags, ``force_north_pole``
     and ``force_south_pole``, for those cases. Most users can ignore these
     flags.
 
+    If either ``force_north_pole`` or ``force_south_pole`` is ``True``,
+    ``fix_winding`` is set to ``False``.
+
     Args:
         polygon: The input polygon
         force_north_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the north pole.
         force_south_pole: If the polygon crosses the antimeridian, force the
             joined segments to enclose the south pole.
+        fix_winding: If the polygon is wound clockwise, reverse its
+            coordinates before applying the algorithm.
 
     Returns:
         The fixed polygon, either as a single polygon or a multi-polygon (if it
         was split)
     """
+    if force_north_pole or force_south_pole:
+        fix_winding = False
     polygons = fix_polygon_to_list(
-        polygon, force_north_pole=force_north_pole, force_south_pole=force_south_pole
+        polygon,
+        force_north_pole=force_north_pole,
+        force_south_pole=force_south_pole,
+        fix_winding=fix_winding,
     )
     if len(polygons) == 1:
         polygon = polygons[0]
         if shapely.is_ccw(polygon.exterior):
             return polygon
         else:
             return Polygon(
@@ -265,29 +320,50 @@
             segments.extend(interior_segments)
         else:
             segments.append(list(interior.coords))
     return segments
 
 
 def fix_polygon_to_list(
-    polygon: Polygon, *, force_north_pole: bool, force_south_pole: bool
+    polygon: Polygon,
+    *,
+    force_north_pole: bool,
+    force_south_pole: bool,
+    fix_winding: bool,
 ) -> List[Polygon]:
     segments = segment(list(polygon.exterior.coords))
     if not segments:
-        return [polygon]
+        if fix_winding and (
+            not shapely.is_ccw(polygon.exterior)
+            or any(shapely.is_ccw(interior) for interior in polygon.interiors)
+        ):
+            FixWindingWarning.warn()
+            return [shapely.geometry.polygon.orient(polygon)]
+        else:
+            return [polygon]
     else:
         interiors = []
         for interior in polygon.interiors:
             interior_segments = segment(list(interior.coords))
             if interior_segments:
+                if fix_winding:
+                    unwrapped_linearring = LinearRing(
+                        list((x % 360, y) for x, y in interior.coords)
+                    )
+                    if shapely.is_ccw(unwrapped_linearring):
+                        FixWindingWarning.warn()
+                        interior_segments = segment(list(reversed(interior.coords)))
                 segments.extend(interior_segments)
             else:
                 interiors.append(interior)
     segments = extend_over_poles(
-        segments, force_north_pole=force_north_pole, force_south_pole=force_south_pole
+        segments,
+        force_north_pole=force_north_pole,
+        force_south_pole=force_south_pole,
+        fix_winding=fix_winding,
     )
     polygons = build_polygons(segments)
     assert polygons
     for i, polygon in enumerate(polygons):
         for j, interior in enumerate(interiors):
             if polygon.contains(interior):
                 interior = interiors.pop(j)
@@ -343,14 +419,15 @@
 
 
 def extend_over_poles(
     segments: List[List[Point]],
     *,
     force_north_pole: bool,
     force_south_pole: bool,
+    fix_winding: bool,
 ) -> List[List[Point]]:
     left_starts = list()
     right_starts = list()
     left_ends = list()
     right_ends = list()
     for i, segment in enumerate(segments):
         if segment[0][0] == -180:
@@ -361,25 +438,45 @@
             left_ends.append((i, segment[-1][1]))
         else:
             right_ends.append((i, segment[-1][1]))
     left_ends.sort(key=lambda v: v[1])
     left_starts.sort(key=lambda v: v[1])
     right_ends.sort(key=lambda v: v[1], reverse=True)
     right_starts.sort(key=lambda v: v[1], reverse=True)
+    is_over_north_pole = False
+    is_over_south_pole = False
+    original_segments = copy.deepcopy(segments)
     # If there's no segment ends between a start and the pole, extend the
     # segment over the pole.
     if left_ends and (
         force_south_pole or not left_starts or left_ends[0][1] < left_starts[0][1]
     ):
+        is_over_south_pole = True
         segments[left_ends[0][0]] += [(-180, -90), (180, -90)]
     if right_ends and (
         force_north_pole or not right_starts or right_ends[0][1] > right_starts[0][1]
     ):
+        is_over_north_pole = True
         segments[right_ends[0][0]] += [(180, 90), (-180, 90)]
-    return segments
+    if fix_winding and is_over_north_pole and is_over_south_pole:
+        # These assertions are here because we're assuming that we set
+        # `fix_winding` to `False` up in `fix_polygon` if either of the
+        # `force_*` variables are set.
+        assert not force_north_pole
+        assert not force_south_pole
+
+        # If we're over both poles and we haven't explicitly disabled the
+        # fix behavior, reverse all segments, effectively reversing the
+        # winding order.
+        FixWindingWarning.warn()
+        for segment in original_segments:
+            segment.reverse()
+        return original_segments
+    else:
+        return segments
 
 
 def build_polygons(
     segments: List[List[Point]],
 ) -> List[Polygon]:
     if not segments:
         return []
```

### Comparing `antimeridian-0.2.6/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.3.0/src/antimeridian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.2.6
+Version: 0.3.0
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: documentation, https://antimeridian.readthedocs.io
 Project-URL: repository, https://github.com/gadomski/antimeridan
 Project-URL: changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.2.6/tests/test_cli.py` & `antimeridian-0.3.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.6/tests/test_geojson.py` & `antimeridian-0.3.0/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.6/tests/test_multi_polygon.py` & `antimeridian-0.3.0/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.2.6/tests/test_polygon.py` & `antimeridian-0.3.0/tests/test_polygon.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import antimeridian
 import pytest
 import shapely.geometry
+from antimeridian import FixWindingWarning
 from shapely.geometry import MultiPolygon, Polygon
 
 from .conftest import Reader
 
 
 @pytest.mark.parametrize(
     ("name"),
     [
-        "both-poles",
         "complex-split",
         "crossing-latitude",
-        "cw-only",
         "extra-crossing",
         "latitude-band",
         "north-pole",
         "one-hole",
         "over-180",
         "overlap",
         "simple",
@@ -34,28 +33,37 @@
     assert isinstance(input, Polygon)
     output = read_output(name)
     assert isinstance(input, Polygon | MultiPolygon)
     fixed = antimeridian.fix_polygon(input).normalize()
     assert fixed == output.normalize()
 
 
+def test_both_poles(read_input: Reader, read_output: Reader) -> None:
+    input = read_input("both-poles")
+    assert isinstance(input, Polygon)
+    output = read_output("both-poles")
+    assert isinstance(input, Polygon)
+    fixed = antimeridian.fix_polygon(input, fix_winding=False).normalize()
+    assert fixed == output.normalize()
+
+
 def test_fix_shape(read_input: Reader) -> None:
     # Just a smoke test
     input = shapely.geometry.mapping(read_input("simple"))
     antimeridian.fix_shape(input)
 
 
 def test_double_fix(
     read_input: Reader,
     read_output: Reader,
 ) -> None:
     input = read_input("north-pole")
     output = read_output("north-pole")
     fixed = antimeridian.fix_polygon(input)
-    fixed = antimeridian.fix_polygon(input)
+    fixed = antimeridian.fix_polygon(fixed)
     assert fixed.normalize() == output.normalize()
 
 
 def test_force_north_pole(read_input: Reader, read_output: Reader) -> None:
     input = read_input("force-north-pole")
     output = read_output("force-north-pole")
     fixed = antimeridian.fix_polygon(input, force_north_pole=True)
@@ -63,7 +71,60 @@
 
 
 @pytest.mark.parametrize("minx,maxx", [(-180, -170), (170, 180)])
 def test_dont_segment_antimeridian_overlap(minx: float, maxx: float) -> None:
     shape = shapely.geometry.box(minx=minx, miny=-10, maxx=maxx, maxy=10)
     fixed = antimeridian.fix_polygon(shape)
     assert fixed.geom_type == "Polygon"
+
+
+@pytest.mark.parametrize("name", ("cw-only", "cw-split"))
+def test_fix_winding(read_input: Reader, read_output: Reader, name: str) -> None:
+    input = read_input(name)
+    output = read_output(name)
+    with pytest.warns(FixWindingWarning):
+        fixed = antimeridian.fix_polygon(input)
+    assert fixed.normalize() == output.normalize()
+
+
+@pytest.mark.parametrize("name", ("cw-only", "cw-split"))
+def test_no_fix_winding(read_input: Reader, read_output: Reader, name: str) -> None:
+    input = read_input(name)
+    output = read_output(f"{name}-no-fix")
+    fixed = antimeridian.fix_polygon(input, fix_winding=False)
+    assert fixed.normalize() == output.normalize()
+
+
+@pytest.mark.parametrize("name", ("cw-only", "cw-split"))
+@pytest.mark.parametrize(
+    "force_north_pole,force_south_pole", [(True, False), (False, True), (True, True)]
+)
+def test_no_fix_winding_when_forcing_poles(
+    read_input: Reader,
+    read_output: Reader,
+    name: str,
+    force_north_pole: bool,
+    force_south_pole: bool,
+) -> None:
+    input = read_input(name)
+    output = read_output(f"{name}-no-fix")
+    fixed = antimeridian.fix_polygon(
+        input,
+        force_north_pole=force_north_pole,
+        force_south_pole=force_south_pole,
+    )
+    assert fixed.normalize() == output.normalize()
+
+
+def test_fix_winding_interior_no_segments(read_input: Reader) -> None:
+    input = read_input("simple-with-ccw-hole")
+    with pytest.warns(FixWindingWarning):
+        fixed = antimeridian.fix_polygon(input)
+    assert all(not shapely.is_ccw(interior) for interior in fixed.interiors)
+
+
+def test_fix_winding_interior_segments(read_input: Reader, read_output: Reader) -> None:
+    input = read_input("one-ccw-hole")
+    output = read_output("one-hole")
+    with pytest.warns(FixWindingWarning):
+        fixed = antimeridian.fix_polygon(input)
+    assert fixed.normalize() == output.normalize()
```

