# Comparing `tmp/crossroads-schematization-0.1.3.tar.gz` & `tmp/crossroads-schematization-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.1.3.tar", last modified: Tue Jun  6 15:52:25 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.0.tar", last modified: Thu Jun 29 08:36:22 2023, max compression
```

## Comparing `crossroads-schematization-0.1.3.tar` & `crossroads-schematization-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.1.3/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.1.3/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-06 15:52:25.000000 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      794 2023-06-06 15:52:25.000000 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-06 15:52:25.000000 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-06 15:52:25.000000 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-06 15:52:25.000000 crossroads-schematization-0.1.3/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-06 15:52:04.000000 crossroads-schematization-0.1.3/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     6727 2023-06-06 12:30:02.000000 crossroads-schematization-0.1.3/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-06 12:40:32.000000 crossroads-schematization-0.1.3/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    23447 2023-06-06 15:51:33.000000 crossroads-schematization-0.1.3/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.1.3/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.1.3/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.1.3/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.1.3/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.1.3/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       36 2023-05-15 13:14:07.000000 crossroads-schematization-0.1.3/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-06 15:52:25.636342 crossroads-schematization-0.1.3/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.1.3/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:36:22.643933 crossroads-schematization-0.2.0/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.0/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 08:36:22.643933 crossroads-schematization-0.2.0/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.0/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:36:22.635934 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 08:36:22.000000 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)      967 2023-06-29 08:36:22.000000 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-29 08:36:22.000000 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-29 08:36:22.000000 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-29 08:36:22.000000 crossroads-schematization-0.2.0/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:36:22.635934 crossroads-schematization-0.2.0/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-29 08:35:41.000000 crossroads-schematization-0.2.0/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7030 2023-06-29 08:32:17.000000 crossroads-schematization-0.2.0/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.0/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    28233 2023-06-29 08:27:42.000000 crossroads-schematization-0.2.0/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.0/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:36:22.643933 crossroads-schematization-0.2.0/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     5615 2023-06-28 14:31:12.000000 crossroads-schematization-0.2.0/crschem/resources/crossing-3-300.png
+-rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.2.0/crschem/resources/crossing.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.0/crschem/resources/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.0/crschem/resources/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)      757 2023-06-28 14:31:12.000000 crossroads-schematization-0.2.0/crschem/resources/point-300.png
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.0/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 08:25:11.000000 crossroads-schematization-0.2.0/crschem/resources/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.0/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.0/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.0/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-29 08:36:22.643933 crossroads-schematization-0.2.0/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.0/setup.py
```

### Comparing `crossroads-schematization-0.1.3/PKG-INFO` & `crossroads-schematization-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.1.3
+Version: 0.2.0
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.1.3/README.md` & `crossroads-schematization-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.0/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.1.3
+Version: 0.2.0
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.1.3/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.2.0/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,16 +9,21 @@
 crossroads_schematization.egg-info/top_level.txt
 crschem/__init__.py
 crschem/cmd.py
 crschem/crossroad.py
 crschem/crossroad_schematization.py
 crschem/processing.py
 crschem/utils.py
+crschem/resources/crossing-3-300.png
 crschem/resources/crossing.svg
+crschem/resources/island-300-white.svg
+crschem/resources/island-300.svg
+crschem/resources/point-300.png
 crschem/resources/rendering-areas.qml
 crschem/resources/rendering-nodes-crossings.qml
 crschem/resources/rendering-nodes-islands.qml
 crschem/resources/rendering-nodes-space.qml
 crschem/resources/rendering-nodes.qml
 crschem/resources/rendering-polylines-space.qml
 crschem/resources/rendering-polylines.qml
+crschem/resources/style-300.xml
 crschem/resources/tactile-a5.qpt
```

### Comparing `crossroads-schematization-0.1.3/crschem/cmd.py` & `crossroads-schematization-0.2.0/crschem/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     group_process.add_argument('--use-fixed-width-on-branches', help='Use a fixed width on each branch (do not evaluate the width adjustment)', action='store_true')
     group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
-    group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif)', type=FileOpener('w'))
+    group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif, shp)', type=FileOpener('w'))
 
     group_preview = parser.add_argument_group("Preview options", "Parameters used by the preview display")
     group_preview.add_argument('--osm', help='display OpenStreetMap network', action='store_true')
     group_preview.add_argument('--branches', help='display branches', action='store_true')
     group_preview.add_argument('--sidewalks-on-branches', help='display sidewalks only on branches', action='store_true')
     group_preview.add_argument('--exact-islands', help='display exact shape of the islands', action='store_true')
     group_preview.add_argument("--non-reachable-islands", help="display non reachable islands.", action='store_true')
@@ -97,24 +97,29 @@
             if len(args.output.filename) < 4:
                 "Cannot deduce required format with small file names"
                 
         if args.output:
 
             if args.output.filename.endswith(".pdf"):
                 print("Exporting as pdf:", args.output.filename)
+                print("!! Legacy export")
                 crschem.toPdf(args.output.filename, args.log_files)
             elif args.output.filename.endswith(".tif"):
                 print("Exporting as tif:", args.output.filename)
                 crschem.toTif(args.output.filename, args.log_files)
             elif args.output.filename.endswith(".svg"):
                 print("Exporting as svg:", args.output.filename)
+                print("!! Legacy export")
                 crschem.toSvg(args.output.filename, args.non_reachable_islands)
             elif args.output.filename.endswith(".geojson"):
                 print("Exporting as geojson:", args.output.filename)
                 crschem.toGeojson(args.output.filename, args.non_reachable_islands)
+            elif args.output.filename.endswith(".shp"):
+                print("Exporting as shapefile:", args.output.filename)
+                crschem.toShapefiles(args.output.filename, args.non_reachable_islands)
             else:
                 print("Unknown output format")
                 
 
     except ValueError as e:
         print("Error:", e)
         print("Intermediate files:", input_file)
```

### Comparing `crossroads-schematization-0.1.3/crschem/crossroad.py` & `crossroads-schematization-0.2.0/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.0/crschem/crossroad_schematization.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 from shapely.geometry import Point, LineString, MultiLineString, LinearRing, Polygon
 import osmnx
+import os
 import networkx
 import numpy as np
 import copy
 import itertools
 import geopandas
 import pandas
 import re
 import matplotlib.pyplot as plt
 import crseg.segmentation as cseg
+import shutil
+import mapnik
+import mapnik.printing
+from mapnik.printing.conversions import m2px
+import sys
+from osgeo import gdal, osr
+import tempfile
 
 from . import utils as u
 from . import processing as p
 from . import crossroad as c
 
 class CrossroadSchematization:
 
@@ -50,14 +58,19 @@
         self.cr_input = cr_input
         self.ignore_crossings_for_sidewalks = ignore_crossings_for_sidewalks
         self.use_fixed_width_on_branches = use_fixed_width_on_branches
         self.turn_shape = turn_shape
 
         self.load_osm(osm_oriented, osm_unoriented)
 
+        # get crossroad center
+        is_n = cr_input["type"] == "crossroads"
+        self.center = cr_input[is_n]["geometry"][0]
+
+
 
     def build(latitude, longitude,
               C0, C1, C2,
               ignore_crossings_for_sidewalks = False,
               use_fixed_width_on_branches = False,
               turn_shape = c.TurningSidewalk.TurnShape.ADJUSTED_ANGLE,
               verbose = True,
@@ -66,15 +79,14 @@
               log_files = False):
 
         import crseg.segmentation as cseg
         import crseg.utils as cru
         import crmodel.crmodel as cm
         import osmnx as ox
         from copy import deepcopy
-        import tempfile
         import os
 
         # load data from OSM
         if verbose:
             print("Loading data from OpenStreetMap")
         ox.settings.use_cache = not ignore_cache
         ox.settings.useful_tags_node = list(set(ox.settings.useful_tags_node + CrossroadSchematization.node_tags_to_keep))
@@ -460,18 +472,110 @@
         else:
             os.unlink(tmp.name)
 
 
 
     def toPdf(self, filename, log_files = False):
         self.to_printable_internal(filename, log_files)
-        
 
-    def toTif(self, filename, log_files = False, dpi = -1):
-        self.to_printable_internal(filename, log_files, dpi)
+
+    def toTifInternal(self, dirName, filename, log_files, resolution, scale):
+        widthMeter = 0.2
+        heightMeter = 0.14
+
+        # scale (ie 1cm in the map is scale "scale" * 1 cm in reality)
+        scale = 400
+
+        width = int(m2px(widthMeter, resolution))
+        height = int(m2px(heightMeter, resolution))
+
+        mapfile = dirName + "/style-" + str(resolution) + ".xml"
+        output = filename
+
+        pseudo_mercator = mapnik.Projection('+proj=merc +a=6378137 +b=6378137 +lat_ts=0.0 +lon_0=0.0 +x_0=0.0 +y_0=0 +k=1.0 +units=m +nadgrids=@null +no_defs +over')
+        mercator = mapnik.Projection('+proj=longlat +ellps=WGS84 +datum=WGS84 +no_defs')
+        trans = mapnik.ProjTransform(mercator, pseudo_mercator)
+
+
+        # make a new Map object for the given mapfile
+        m = mapnik.Map(width, height)
+        mapnik.load_map(m, mapfile)
+
+        # ensure the target map projection is pseudo-mercator
+        m.srs = pseudo_mercator.params()
+
+        # get crossroads center
+
+        pmerc_centre = trans.forward(mapnik.Coord(self.center.x, self.center.y))
+
+        # compute min and max coordinates
+        dx = widthMeter / 2 * scale
+        minx = pmerc_centre.x - dx
+        maxx = pmerc_centre.x + dx
+
+        # grow the height bbox, as we only accurately set the width bbox
+        m.aspect_fix_mode = mapnik.aspect_fix_mode.ADJUST_BBOX_HEIGHT
+
+        bounds = mapnik.Box2d(minx, pmerc_centre.y - 10, maxx, pmerc_centre.y + 10) # the y bounds will be fixed by mapnik due to ADJUST_BBOX_HEIGHT
+        m.zoom_to_box(bounds)
+
+        # render the map image to a file
+        mapnik.render_to_file(m, output)
+
+        # set geotiff information
+        gdal.UseExceptions()
+        pxSize = 1 / m2px(1, resolution) * scale
+        ds = gdal.Open(output, gdal.GA_Update)
+        gt = [
+            #GT(0) x-coordinate of the upper-left corner of the upper-left pixel.
+            m.envelope()[0],
+            #GT(1) w-e pixel resolution / pixel width.
+            pxSize,
+            #GT(2) row rotation (typically zero).
+            0.0,
+            #GT(3) y-coordinate of the upper-left corner of the upper-left pixel.
+            m.envelope()[3],
+            #GT(4) column rotation (typically zero).
+            0.0,
+            #GT(5) n-s pixel resolution / pixel height (negative value for a north-up image).
+            -pxSize
+        ]
+        ds.SetGeoTransform(gt)
+
+        sr = osr.SpatialReference()
+        sr.SetFromUserInput(pseudo_mercator.params())
+        wkt = sr.ExportToWkt()
+        ds.SetProjection(wkt)
+
+
+
+    def toTif(self, filename, log_files = False, resolution = 300, scale = 400):
+        # first export to shapefiles in a temporary directory
+        dirName = tempfile.mkdtemp()
+        if log_files:
+            print('Temporary directory (styling):', dirName)
+        self.toShapefiles(dirName + "/crossroad.shp")
+
+        # then move style file (xml) in this directory
+        if resolution in [300]:
+            for f in ["style-" + str(resolution) + ".xml",
+                        "crossing-3-" + str(resolution) + ".png", 
+                        "point-" + str(resolution) + ".png",
+                        "island-" + str(resolution) + ".svg",
+                        "island-" + str(resolution) + "-white.svg"]:
+                shutil.copy(os.path.dirname(__file__) + "/resources/" + f, dirName)
+        else:
+            print("not supported DPI")
+
+        # finally render the image
+        self.toTifInternal(dirName, filename, log_files, resolution, scale)
+
+        # then delete the temporary directory
+        if not log_files:
+            os.rmdir(dirName)
         
 
     def toSvg(self, filename, only_reachable_islands = False):
         # TODO
         print("not yet implemented")
 
 
@@ -486,14 +590,30 @@
                             c.Branch.toGDFBranches(self.branches).to_crs(crs),
                             c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs),
                             c.Crossing.toGDFCrossings(self.crossings).to_crs(crs)])
         
         df.to_file(filename, driver='GeoJSON')
 
 
+    def toShapefiles(self, filename, only_reachable_islands = False, crs = "EPSG:4326"):
+        filename, file_extension = os.path.splitext(filename)
+
+        self.toGDFInnerRegion().to_crs(crs).to_file(filename + "-inner" + file_extension) # region
+        c.TurningSidewalk.toGDFSidewalks(self.merged_sidewalks).to_crs(crs).to_file(filename + "-sidewalks" + file_extension) # lines
+        c.Branch.toGDFBranches(self.branches).to_crs(crs).to_file(filename + "-branches" + file_extension) # lines
+        
+        # islands can be points and lines
+        islands = c.TrafficIsland.toGDFTrafficIslands(self.traffic_islands, only_reachable_islands).to_crs(crs)
+        islands[islands.geometry.type == 'LineString'].to_file(filename + "-islands-lines" + file_extension)
+        islands[islands.geometry.type == 'Point'].to_file(filename + "-islands-points" + file_extension)
+
+        # points
+        c.Crossing.toGDFCrossings(self.crossings).to_crs(crs).to_file(filename + "-crossings" + file_extension)
+
+
     def show(self, 
              osm_graph = False,
              branches = False,
              simple_sidewalks = False,
              merged_sidewalks = True,
              inner_region = True,
              exact_islands = False,
```

### Comparing `crossroads-schematization-0.1.3/crschem/processing.py` & `crossroads-schematization-0.2.0/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/crossing.svg` & `crossroads-schematization-0.2.0/crschem/resources/crossing.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-crossings.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-nodes-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-nodes.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.2.0/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.2.0/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/crschem/utils.py` & `crossroads-schematization-0.2.0/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.1.3/setup.py` & `crossroads-schematization-0.2.0/setup.py`

 * *Files identical despite different names*

