# Comparing `tmp/crossroads-schematization-0.2.1.tar.gz` & `tmp/crossroads-schematization-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossroads-schematization-0.2.1.tar", last modified: Thu Jun 29 08:51:50 2023, max compression
+gzip compressed data, was "crossroads-schematization-0.2.2.tar", last modified: Thu Jun 29 12:41:53 2023, max compression
```

## Comparing `crossroads-schematization-0.2.1.tar` & `crossroads-schematization-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:51:50.543405 crossroads-schematization-0.2.1/
--rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.1/MANIFEST.in
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 08:51:50.543405 crossroads-schematization-0.2.1/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.1/README.md
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:51:50.539405 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/
--rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 08:51:50.000000 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/PKG-INFO
--rw-r--r--   0 jm        (1000) jm        (1000)      967 2023-06-29 08:51:50.000000 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/SOURCES.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-29 08:51:50.000000 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/dependency_links.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-29 08:51:50.000000 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/entry_points.txt
--rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-29 08:51:50.000000 crossroads-schematization-0.2.1/crossroads_schematization.egg-info/top_level.txt
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:51:50.539405 crossroads-schematization-0.2.1/crschem/
--rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-29 08:50:50.000000 crossroads-schematization-0.2.1/crschem/__init__.py
--rw-r--r--   0 jm        (1000) jm        (1000)     7030 2023-06-29 08:32:17.000000 crossroads-schematization-0.2.1/crschem/cmd.py
--rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.1/crschem/crossroad.py
--rw-r--r--   0 jm        (1000) jm        (1000)    28238 2023-06-29 08:50:42.000000 crossroads-schematization-0.2.1/crschem/crossroad_schematization.py
--rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.1/crschem/processing.py
-drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 08:51:50.539405 crossroads-schematization-0.2.1/crschem/resources/
--rw-r--r--   0 jm        (1000) jm        (1000)     5615 2023-06-28 14:31:12.000000 crossroads-schematization-0.2.1/crschem/resources/crossing-3-300.png
--rw-r--r--   0 jm        (1000) jm        (1000)     2425 2022-10-28 13:53:49.000000 crossroads-schematization-0.2.1/crschem/resources/crossing.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.1/crschem/resources/island-300-white.svg
--rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.1/crschem/resources/island-300.svg
--rw-r--r--   0 jm        (1000) jm        (1000)      757 2023-06-28 14:31:12.000000 crossroads-schematization-0.2.1/crschem/resources/point-300.png
--rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-areas.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-crossings.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-islands.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-nodes.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-polylines-space.qml
--rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.1/crschem/resources/rendering-polylines.qml
--rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 08:25:11.000000 crossroads-schematization-0.2.1/crschem/resources/style-300.xml
--rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.1/crschem/resources/tactile-a5.qpt
--rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.1/crschem/utils.py
--rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.1/requirements.txt
--rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-29 08:51:50.543405 crossroads-schematization-0.2.1/setup.cfg
--rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.1/setup.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/
+-rw-r--r--   0 jm        (1000) jm        (1000)      107 2022-11-30 16:15:16.000000 crossroads-schematization-0.2.2/MANIFEST.in
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     2897 2022-11-30 16:53:52.000000 crossroads-schematization-0.2.2/README.md
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.472530 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/
+-rw-r--r--   0 jm        (1000) jm        (1000)     3477 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/PKG-INFO
+-rw-r--r--   0 jm        (1000) jm        (1000)     1104 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/SOURCES.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        1 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/dependency_links.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       98 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/entry_points.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)        8 2023-06-29 12:41:53.000000 crossroads-schematization-0.2.2/crossroads_schematization.egg-info/top_level.txt
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.472530 crossroads-schematization-0.2.2/crschem/
+-rw-r--r--   0 jm        (1000) jm        (1000)       22 2023-06-29 12:38:10.000000 crossroads-schematization-0.2.2/crschem/__init__.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     7159 2023-06-29 12:41:17.000000 crossroads-schematization-0.2.2/crschem/cmd.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    51224 2023-06-28 14:41:35.000000 crossroads-schematization-0.2.2/crschem/crossroad.py
+-rw-r--r--   0 jm        (1000) jm        (1000)    28261 2023-06-29 12:29:38.000000 crossroads-schematization-0.2.2/crschem/crossroad_schematization.py
+-rw-r--r--   0 jm        (1000) jm        (1000)     5393 2023-05-12 08:32:50.000000 crossroads-schematization-0.2.2/crschem/processing.py
+drwxr-xr-x   0 jm        (1000) jm        (1000)        0 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/crschem/resources/
+-rw-r--r--   0 jm        (1000) jm        (1000)     1881 2023-06-29 12:36:54.000000 crossroads-schematization-0.2.2/crschem/resources/crossing-3-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1966 2023-06-29 12:26:45.000000 crossroads-schematization-0.2.2/crschem/resources/crossing-3-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1523 2023-06-29 08:24:15.000000 crossroads-schematization-0.2.2/crschem/resources/island-300-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1493 2023-06-29 08:16:55.000000 crossroads-schematization-0.2.2/crschem/resources/island-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1504 2023-06-29 12:25:46.000000 crossroads-schematization-0.2.2/crschem/resources/island-96-white.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1518 2023-06-29 12:26:15.000000 crossroads-schematization-0.2.2/crschem/resources/island-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1569 2023-06-29 12:17:13.000000 crossroads-schematization-0.2.2/crschem/resources/point-300.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1630 2023-06-29 12:25:06.000000 crossroads-schematization-0.2.2/crschem/resources/point-96.svg
+-rw-r--r--   0 jm        (1000) jm        (1000)    23130 2023-02-06 15:35:04.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-areas.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    29214 2023-05-19 13:30:46.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-crossings.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22244 2023-05-19 13:29:18.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-islands.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    22753 2023-05-19 13:31:32.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    35238 2023-05-19 13:31:15.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-nodes.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28654 2023-02-06 15:35:25.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-polylines-space.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)    28635 2023-01-16 09:29:31.000000 crossroads-schematization-0.2.2/crschem/resources/rendering-polylines.qml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3164 2023-06-29 12:12:19.000000 crossroads-schematization-0.2.2/crschem/resources/style-300.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     3162 2023-06-29 12:29:55.000000 crossroads-schematization-0.2.2/crschem/resources/style-96.xml
+-rw-r--r--   0 jm        (1000) jm        (1000)     7371 2022-11-10 14:22:27.000000 crossroads-schematization-0.2.2/crschem/resources/tactile-a5.qpt
+-rw-r--r--   0 jm        (1000) jm        (1000)     7843 2023-06-05 15:25:19.000000 crossroads-schematization-0.2.2/crschem/utils.py
+-rw-r--r--   0 jm        (1000) jm        (1000)       48 2023-06-29 08:31:26.000000 crossroads-schematization-0.2.2/requirements.txt
+-rw-r--r--   0 jm        (1000) jm        (1000)       38 2023-06-29 12:41:53.476531 crossroads-schematization-0.2.2/setup.cfg
+-rw-r--r--   0 jm        (1000) jm        (1000)     1207 2022-11-30 16:14:11.000000 crossroads-schematization-0.2.2/setup.py
```

### Comparing `crossroads-schematization-0.2.1/PKG-INFO` & `crossroads-schematization-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.1
+Version: 0.2.2
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.1/README.md` & `crossroads-schematization-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crossroads_schematization.egg-info/PKG-INFO` & `crossroads-schematization-0.2.2/crossroads_schematization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossroads-schematization
-Version: 0.2.1
+Version: 0.2.2
 Summary: Crossroads schematization is a python tool that produces automatic schematization of intersections from OpenStreetMap.
 Home-page: https://github.com/jmtrivial/crossroads-schematization/
 Author: Jean-Marie Favreau
 Author-email: j-marie.favreau@uca.fr
 License: AGPL-3.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crossroads-schematization-0.2.1/crossroads_schematization.egg-info/SOURCES.txt` & `crossroads-schematization-0.2.2/crossroads_schematization.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,21 +9,25 @@
 crossroads_schematization.egg-info/top_level.txt
 crschem/__init__.py
 crschem/cmd.py
 crschem/crossroad.py
 crschem/crossroad_schematization.py
 crschem/processing.py
 crschem/utils.py
-crschem/resources/crossing-3-300.png
-crschem/resources/crossing.svg
+crschem/resources/crossing-3-300.svg
+crschem/resources/crossing-3-96.svg
 crschem/resources/island-300-white.svg
 crschem/resources/island-300.svg
-crschem/resources/point-300.png
+crschem/resources/island-96-white.svg
+crschem/resources/island-96.svg
+crschem/resources/point-300.svg
+crschem/resources/point-96.svg
 crschem/resources/rendering-areas.qml
 crschem/resources/rendering-nodes-crossings.qml
 crschem/resources/rendering-nodes-islands.qml
 crschem/resources/rendering-nodes-space.qml
 crschem/resources/rendering-nodes.qml
 crschem/resources/rendering-polylines-space.qml
 crschem/resources/rendering-polylines.qml
 crschem/resources/style-300.xml
+crschem/resources/style-96.xml
 crschem/resources/tactile-a5.qpt
```

### Comparing `crossroads-schematization-0.2.1/crschem/cmd.py` & `crossroads-schematization-0.2.2/crschem/cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     group_process.add_argument('--turn-shape', help='Turn shape.', type=lambda s: c.TurningSidewalk.TurnShape[s], choices=list(c.TurningSidewalk.TurnShape))
 
     group_output = parser.add_argument_group("Output", "Display, log or save results")
     group_output.add_argument('-l', '--log-files', help='keep intermediate files and give their name in output', action='store_true')
     group_output.add_argument('-d', '--display-all', help='display all steps', action='store_true')
     group_output.add_argument('--display-preview', help='display a preview of the crossroad schematization', action='store_true')
     group_output.add_argument('-o', '--output', help='output file (supported format: geojson, pdf, tif, shp)', type=FileOpener('w'))
+    group_output.add_argument('--dpi', help='dpi for tif export', type=int, choices=[96, 300], default=300)
 
     group_preview = parser.add_argument_group("Preview options", "Parameters used by the preview display")
     group_preview.add_argument('--osm', help='display OpenStreetMap network', action='store_true')
     group_preview.add_argument('--branches', help='display branches', action='store_true')
     group_preview.add_argument('--sidewalks-on-branches', help='display sidewalks only on branches', action='store_true')
     group_preview.add_argument('--exact-islands', help='display exact shape of the islands', action='store_true')
     group_preview.add_argument("--non-reachable-islands", help="display non reachable islands.", action='store_true')
@@ -101,15 +102,15 @@
 
             if args.output.filename.endswith(".pdf"):
                 print("Exporting as pdf:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toPdf(args.output.filename, args.log_files)
             elif args.output.filename.endswith(".tif"):
                 print("Exporting as tif:", args.output.filename)
-                crschem.toTif(args.output.filename, args.log_files)
+                crschem.toTif(args.output.filename, args.log_files, resolution=args.dpi)
             elif args.output.filename.endswith(".svg"):
                 print("Exporting as svg:", args.output.filename)
                 print("!! Legacy export")
                 crschem.toSvg(args.output.filename, args.non_reachable_islands)
             elif args.output.filename.endswith(".geojson"):
                 print("Exporting as geojson:", args.output.filename)
                 crschem.toGeojson(args.output.filename, args.non_reachable_islands)
```

### Comparing `crossroads-schematization-0.2.1/crschem/crossroad.py` & `crossroads-schematization-0.2.2/crschem/crossroad.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/crossroad_schematization.py` & `crossroads-schematization-0.2.2/crschem/crossroad_schematization.py`

 * *Files 1% similar despite different names*

```diff
@@ -552,23 +552,24 @@
         # first export to shapefiles in a temporary directory
         dirName = tempfile.mkdtemp()
         if log_files:
             print('Temporary directory (styling):', dirName)
         self.toShapefiles(dirName + "/crossroad.shp")
 
         # then move style file (xml) in this directory
-        if resolution in [300]:
+        if resolution in [96, 300]:
             for f in ["style-" + str(resolution) + ".xml",
-                        "crossing-3-" + str(resolution) + ".png", 
-                        "point-" + str(resolution) + ".png",
+                        "crossing-3-" + str(resolution) + ".svg", 
+                        "point-" + str(resolution) + ".svg",
                         "island-" + str(resolution) + ".svg",
                         "island-" + str(resolution) + "-white.svg"]:
                 shutil.copy(os.path.dirname(__file__) + "/resources/" + f, dirName)
         else:
             print("not supported DPI")
+            return
 
         # finally render the image
         self.toTifInternal(dirName, filename, log_files, resolution, scale)
 
         # then delete the temporary directory
         if not log_files:
             shutil.rmtree(dirName)
```

### Comparing `crossroads-schematization-0.2.1/crschem/processing.py` & `crossroads-schematization-0.2.2/crschem/processing.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/crossing.svg` & `crossroads-schematization-0.2.2/crschem/resources/crossing-3-300.svg`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,118 @@
 00000000: 3c3f 786d 6c20 7665 7273 696f 6e3d 2231  <?xml version="1
 00000010: 2e30 2220 656e 636f 6469 6e67 3d22 5554  .0" encoding="UT
 00000020: 462d 3822 2073 7461 6e64 616c 6f6e 653d  F-8" standalone=
 00000030: 226e 6f22 3f3e 0a3c 212d 2d20 4372 6561  "no"?>.<!-- Crea
 00000040: 7465 6420 7769 7468 2049 6e6b 7363 6170  ted with Inkscap
 00000050: 6520 2868 7474 703a 2f2f 7777 772e 696e  e (http://www.in
 00000060: 6b73 6361 7065 2e6f 7267 2f29 202d 2d3e  kscape.org/) -->
-00000070: 0a0a 3c73 7667 0a20 2020 7769 6474 683d  ..<svg.   width=
-00000080: 2231 326d 6d22 0a20 2020 6865 6967 6874  "12mm".   height
-00000090: 3d22 3132 6d6d 220a 2020 2076 6965 7742  ="12mm".   viewB
-000000a0: 6f78 3d22 3020 3020 3132 2031 3222 0a20  ox="0 0 12 12". 
-000000b0: 2020 7665 7273 696f 6e3d 2231 2e31 220a    version="1.1".
-000000c0: 2020 2069 643d 2273 7667 3522 0a20 2020     id="svg5".   
-000000d0: 696e 6b73 6361 7065 3a76 6572 7369 6f6e  inkscape:version
-000000e0: 3d22 312e 322e 3120 2839 6336 6434 3165  ="1.2.1 (9c6d41e
-000000f0: 3431 302c 2032 3032 322d 3037 2d31 3429  410, 2022-07-14)
-00000100: 220a 2020 2073 6f64 6970 6f64 693a 646f  ".   sodipodi:do
-00000110: 636e 616d 653d 2263 726f 7373 696e 672e  cname="crossing.
-00000120: 7376 6722 0a20 2020 786d 6c6e 733a 696e  svg".   xmlns:in
-00000130: 6b73 6361 7065 3d22 6874 7470 3a2f 2f77  kscape="http://w
-00000140: 7777 2e69 6e6b 7363 6170 652e 6f72 672f  ww.inkscape.org/
-00000150: 6e61 6d65 7370 6163 6573 2f69 6e6b 7363  namespaces/inksc
-00000160: 6170 6522 0a20 2020 786d 6c6e 733a 736f  ape".   xmlns:so
-00000170: 6469 706f 6469 3d22 6874 7470 3a2f 2f73  dipodi="http://s
-00000180: 6f64 6970 6f64 692e 736f 7572 6365 666f  odipodi.sourcefo
-00000190: 7267 652e 6e65 742f 4454 442f 736f 6469  rge.net/DTD/sodi
-000001a0: 706f 6469 2d30 2e64 7464 220a 2020 2078  podi-0.dtd".   x
-000001b0: 6d6c 6e73 3d22 6874 7470 3a2f 2f77 7777  mlns="http://www
-000001c0: 2e77 332e 6f72 672f 3230 3030 2f73 7667  .w3.org/2000/svg
-000001d0: 220a 2020 2078 6d6c 6e73 3a73 7667 3d22  ".   xmlns:svg="
-000001e0: 6874 7470 3a2f 2f77 7777 2e77 332e 6f72  http://www.w3.or
-000001f0: 672f 3230 3030 2f73 7667 223e 0a20 203c  g/2000/svg">.  <
-00000200: 736f 6469 706f 6469 3a6e 616d 6564 7669  sodipodi:namedvi
-00000210: 6577 0a20 2020 2020 6964 3d22 6e61 6d65  ew.     id="name
-00000220: 6476 6965 7737 220a 2020 2020 2070 6167  dview7".     pag
-00000230: 6563 6f6c 6f72 3d22 2366 6666 6666 6622  ecolor="#ffffff"
-00000240: 0a20 2020 2020 626f 7264 6572 636f 6c6f  .     bordercolo
-00000250: 723d 2223 3636 3636 3636 220a 2020 2020  r="#666666".    
-00000260: 2062 6f72 6465 726f 7061 6369 7479 3d22   borderopacity="
-00000270: 312e 3022 0a20 2020 2020 696e 6b73 6361  1.0".     inksca
-00000280: 7065 3a73 686f 7770 6167 6573 6861 646f  pe:showpageshado
-00000290: 773d 2232 220a 2020 2020 2069 6e6b 7363  w="2".     inksc
-000002a0: 6170 653a 7061 6765 6f70 6163 6974 793d  ape:pageopacity=
-000002b0: 2230 2e30 220a 2020 2020 2069 6e6b 7363  "0.0".     inksc
-000002c0: 6170 653a 7061 6765 6368 6563 6b65 7262  ape:pagecheckerb
-000002d0: 6f61 7264 3d22 3022 0a20 2020 2020 696e  oard="0".     in
-000002e0: 6b73 6361 7065 3a64 6573 6b63 6f6c 6f72  kscape:deskcolor
-000002f0: 3d22 2364 3164 3164 3122 0a20 2020 2020  ="#d1d1d1".     
-00000300: 696e 6b73 6361 7065 3a64 6f63 756d 656e  inkscape:documen
-00000310: 742d 756e 6974 733d 226d 6d22 0a20 2020  t-units="mm".   
-00000320: 2020 7368 6f77 6772 6964 3d22 6661 6c73    showgrid="fals
-00000330: 6522 0a20 2020 2020 696e 6b73 6361 7065  e".     inkscape
-00000340: 3a7a 6f6f 6d3d 2238 2e37 3238 3238 3438  :zoom="8.7282848
-00000350: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
-00000360: 6378 3d22 392e 3130 3833 3138 3722 0a20  cx="9.1083187". 
-00000370: 2020 2020 696e 6b73 6361 7065 3a63 793d      inkscape:cy=
-00000380: 2231 372e 3532 3932 3137 220a 2020 2020  "17.529217".    
-00000390: 2069 6e6b 7363 6170 653a 7769 6e64 6f77   inkscape:window
-000003a0: 2d77 6964 7468 3d22 3132 3830 220a 2020  -width="1280".  
-000003b0: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
-000003c0: 6f77 2d68 6569 6768 743d 2236 3931 220a  ow-height="691".
-000003d0: 2020 2020 2069 6e6b 7363 6170 653a 7769       inkscape:wi
-000003e0: 6e64 6f77 2d78 3d22 3239 3522 0a20 2020  ndow-x="295".   
-000003f0: 2020 696e 6b73 6361 7065 3a77 696e 646f    inkscape:windo
-00000400: 772d 793d 2231 3330 3322 0a20 2020 2020  w-y="1303".     
-00000410: 696e 6b73 6361 7065 3a77 696e 646f 772d  inkscape:window-
-00000420: 6d61 7869 6d69 7a65 643d 2230 220a 2020  maximized="0".  
-00000430: 2020 2069 6e6b 7363 6170 653a 6375 7272     inkscape:curr
-00000440: 656e 742d 6c61 7965 723d 226c 6179 6572  ent-layer="layer
-00000450: 3122 202f 3e0a 2020 3c64 6566 730a 2020  1" />.  <defs.  
-00000460: 2020 2069 643d 2264 6566 7332 2220 2f3e     id="defs2" />
-00000470: 0a20 203c 670a 2020 2020 2069 6e6b 7363  .  <g.     inksc
-00000480: 6170 653a 6c61 6265 6c3d 2243 616c 7175  ape:label="Calqu
-00000490: 6520 3122 0a20 2020 2020 696e 6b73 6361  e 1".     inksca
-000004a0: 7065 3a67 726f 7570 6d6f 6465 3d22 6c61  pe:groupmode="la
-000004b0: 7965 7222 0a20 2020 2020 6964 3d22 6c61  yer".     id="la
-000004c0: 7965 7231 220a 2020 2020 2074 7261 6e73  yer1".     trans
-000004d0: 666f 726d 3d22 7472 616e 736c 6174 6528  form="translate(
-000004e0: 2d34 372e 3331 3735 3831 2c2d 3339 2e32  -47.317581,-39.2
-000004f0: 3632 3932 3829 223e 0a20 2020 203c 7265  62928)">.    <re
-00000500: 6374 0a20 2020 2020 2020 7374 796c 653d  ct.       style=
-00000510: 2266 696c 6c3a 2366 6666 6666 663b 7374  "fill:#ffffff;st
-00000520: 726f 6b65 3a6e 6f6e 653b 7374 726f 6b65  roke:none;stroke
-00000530: 2d77 6964 7468 3a31 2e39 3133 333b 7374  -width:1.9133;st
-00000540: 726f 6b65 2d6c 696e 6563 6170 3a72 6f75  roke-linecap:rou
-00000550: 6e64 3b73 7472 6f6b 652d 6c69 6e65 6a6f  nd;stroke-linejo
-00000560: 696e 3a72 6f75 6e64 220a 2020 2020 2020  in:round".      
-00000570: 2069 643d 2272 6563 7431 3133 220a 2020   id="rect113".  
-00000580: 2020 2020 2077 6964 7468 3d22 3132 220a       width="12".
-00000590: 2020 2020 2020 2068 6569 6768 743d 2231         height="1
-000005a0: 3222 0a20 2020 2020 2020 783d 2233 392e  2".       x="39.
-000005b0: 3236 3239 3238 220a 2020 2020 2020 2079  262928".       y
-000005c0: 3d22 2d35 392e 3331 3735 3831 220a 2020  ="-59.317581".  
-000005d0: 2020 2020 2072 793d 2231 2e34 3933 3035       ry="1.49305
-000005e0: 3522 0a20 2020 2020 2020 7472 616e 7366  5".       transf
-000005f0: 6f72 6d3d 2272 6f74 6174 6528 3930 2922  orm="rotate(90)"
-00000600: 202f 3e0a 2020 2020 3c67 0a20 2020 2020   />.    <g.     
-00000610: 2020 6964 3d22 6731 3231 3422 0a20 2020    id="g1214".   
-00000620: 2020 2020 7472 616e 7366 6f72 6d3d 2272      transform="r
-00000630: 6f74 6174 6528 3930 2c35 332e 3231 3730  otate(90,53.2170
-00000640: 3734 2c34 352e 3136 3234 3231 2922 3e0a  74,45.162421)">.
-00000650: 2020 2020 2020 3c70 6174 680a 2020 2020        <path.    
-00000660: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
-00000670: 3a6e 6f6e 653b 7374 726f 6b65 3a23 3030  :none;stroke:#00
-00000680: 3030 3030 3b73 7472 6f6b 652d 7769 6474  0000;stroke-widt
-00000690: 683a 322e 3037 3037 363b 7374 726f 6b65  h:2.07076;stroke
-000006a0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
-000006b0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a62  troke-linejoin:b
-000006c0: 6576 656c 3b73 7472 6f6b 652d 6461 7368  evel;stroke-dash
-000006d0: 6172 7261 793a 6e6f 6e65 3b73 7472 6f6b  array:none;strok
-000006e0: 652d 6f70 6163 6974 793a 3122 0a20 2020  e-opacity:1".   
-000006f0: 2020 2020 2020 643d 226d 2034 392e 3338        d="m 49.38
-00000700: 3935 3837 2c34 312e 3830 3433 3838 2068  9587,41.804388 h
-00000710: 2037 2e38 3535 3938 3822 0a20 2020 2020   7.855988".     
-00000720: 2020 2020 6964 3d22 7061 7468 3438 3222      id="path482"
-00000730: 0a20 2020 2020 2020 2020 736f 6469 706f  .         sodipo
-00000740: 6469 3a6e 6f64 6574 7970 6573 3d22 6363  di:nodetypes="cc
-00000750: 2220 2f3e 0a20 2020 2020 203c 7061 7468  " />.      <path
-00000760: 0a20 2020 2020 2020 2020 7374 796c 653d  .         style=
-00000770: 2266 696c 6c3a 6e6f 6e65 3b73 7472 6f6b  "fill:none;strok
-00000780: 653a 2330 3030 3030 303b 7374 726f 6b65  e:#000000;stroke
-00000790: 2d77 6964 7468 3a32 2e30 3730 3736 3b73  -width:2.07076;s
-000007a0: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
-000007b0: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
-000007c0: 6f69 6e3a 6265 7665 6c3b 7374 726f 6b65  oin:bevel;stroke
-000007d0: 2d64 6173 6861 7272 6179 3a6e 6f6e 653b  -dasharray:none;
-000007e0: 7374 726f 6b65 2d6f 7061 6369 7479 3a31  stroke-opacity:1
-000007f0: 220a 2020 2020 2020 2020 2064 3d22 6d20  ".         d="m 
-00000800: 3439 2e33 3839 3538 372c 3435 2e30 3631  49.389587,45.061
-00000810: 3931 3420 6820 372e 3835 3539 3838 220a  914 h 7.855988".
-00000820: 2020 2020 2020 2020 2069 643d 2270 6174           id="pat
-00000830: 6834 3832 2d33 220a 2020 2020 2020 2020  h482-3".        
-00000840: 2073 6f64 6970 6f64 693a 6e6f 6465 7479   sodipodi:nodety
-00000850: 7065 733d 2263 6322 202f 3e0a 2020 2020  pes="cc" />.    
-00000860: 2020 3c70 6174 680a 2020 2020 2020 2020    <path.        
-00000870: 2073 7479 6c65 3d22 6669 6c6c 3a6e 6f6e   style="fill:non
-00000880: 653b 7374 726f 6b65 3a23 3030 3030 3030  e;stroke:#000000
-00000890: 3b73 7472 6f6b 652d 7769 6474 683a 322e  ;stroke-width:2.
-000008a0: 3037 3037 363b 7374 726f 6b65 2d6c 696e  07076;stroke-lin
-000008b0: 6563 6170 3a72 6f75 6e64 3b73 7472 6f6b  ecap:round;strok
-000008c0: 652d 6c69 6e65 6a6f 696e 3a62 6576 656c  e-linejoin:bevel
-000008d0: 3b73 7472 6f6b 652d 6461 7368 6172 7261  ;stroke-dasharra
-000008e0: 793a 6e6f 6e65 3b73 7472 6f6b 652d 6f70  y:none;stroke-op
-000008f0: 6163 6974 793a 3122 0a20 2020 2020 2020  acity:1".       
-00000900: 2020 643d 226d 2034 392e 3338 3935 3837    d="m 49.389587
-00000910: 2c34 382e 3331 3934 3420 6820 372e 3835  ,48.31944 h 7.85
-00000920: 3539 3838 220a 2020 2020 2020 2020 2069  5988".         i
-00000930: 643d 2270 6174 6834 3832 2d36 220a 2020  d="path482-6".  
-00000940: 2020 2020 2020 2073 6f64 6970 6f64 693a         sodipodi:
-00000950: 6e6f 6465 7479 7065 733d 2263 6322 202f  nodetypes="cc" /
-00000960: 3e0a 2020 2020 3c2f 673e 0a20 203c 2f67  >.    </g>.  </g
-00000970: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
+00000070: 0a0a 3c73 7667 0a20 2020 7665 7273 696f  ..<svg.   versio
+00000080: 6e3d 2231 2e31 220a 2020 2069 643d 2273  n="1.1".   id="s
+00000090: 7667 3222 0a20 2020 7769 6474 683d 2231  vg2".   width="1
+000000a0: 3539 2e32 3837 3038 220a 2020 2068 6569  59.28708".   hei
+000000b0: 6768 743d 2231 3338 2e30 3438 3831 220a  ght="138.04881".
+000000c0: 2020 2076 6965 7742 6f78 3d22 3020 3020     viewBox="0 0 
+000000d0: 3135 392e 3238 3730 3820 3133 382e 3034  159.28708 138.04
+000000e0: 3838 3122 0a20 2020 736f 6469 706f 6469  881".   sodipodi
+000000f0: 3a64 6f63 6e61 6d65 3d22 6372 6f73 7369  :docname="crossi
+00000100: 6e67 2d33 2d33 3030 2e73 7667 220a 2020  ng-3-300.svg".  
+00000110: 2069 6e6b 7363 6170 653a 7665 7273 696f   inkscape:versio
+00000120: 6e3d 2231 2e32 2e32 2028 6230 6138 3438  n="1.2.2 (b0a848
+00000130: 3635 3431 2c20 3230 3232 2d31 322d 3031  6541, 2022-12-01
+00000140: 2922 0a20 2020 786d 6c6e 733a 696e 6b73  )".   xmlns:inks
+00000150: 6361 7065 3d22 6874 7470 3a2f 2f77 7777  cape="http://www
+00000160: 2e69 6e6b 7363 6170 652e 6f72 672f 6e61  .inkscape.org/na
+00000170: 6d65 7370 6163 6573 2f69 6e6b 7363 6170  mespaces/inkscap
+00000180: 6522 0a20 2020 786d 6c6e 733a 736f 6469  e".   xmlns:sodi
+00000190: 706f 6469 3d22 6874 7470 3a2f 2f73 6f64  podi="http://sod
+000001a0: 6970 6f64 692e 736f 7572 6365 666f 7267  ipodi.sourceforg
+000001b0: 652e 6e65 742f 4454 442f 736f 6469 706f  e.net/DTD/sodipo
+000001c0: 6469 2d30 2e64 7464 220a 2020 2078 6d6c  di-0.dtd".   xml
+000001d0: 6e73 3d22 6874 7470 3a2f 2f77 7777 2e77  ns="http://www.w
+000001e0: 332e 6f72 672f 3230 3030 2f73 7667 220a  3.org/2000/svg".
+000001f0: 2020 2078 6d6c 6e73 3a73 7667 3d22 6874     xmlns:svg="ht
+00000200: 7470 3a2f 2f77 7777 2e77 332e 6f72 672f  tp://www.w3.org/
+00000210: 3230 3030 2f73 7667 223e 0a20 203c 6465  2000/svg">.  <de
+00000220: 6673 0a20 2020 2020 6964 3d22 6465 6673  fs.     id="defs
+00000230: 3622 202f 3e0a 2020 3c73 6f64 6970 6f64  6" />.  <sodipod
+00000240: 693a 6e61 6d65 6476 6965 770a 2020 2020  i:namedview.    
+00000250: 2069 643d 226e 616d 6564 7669 6577 3422   id="namedview4"
+00000260: 0a20 2020 2020 7061 6765 636f 6c6f 723d  .     pagecolor=
+00000270: 2223 6666 6666 6666 220a 2020 2020 2062  "#ffffff".     b
+00000280: 6f72 6465 7263 6f6c 6f72 3d22 2336 3636  ordercolor="#666
+00000290: 3636 3622 0a20 2020 2020 626f 7264 6572  666".     border
+000002a0: 6f70 6163 6974 793d 2231 2e30 220a 2020  opacity="1.0".  
+000002b0: 2020 2069 6e6b 7363 6170 653a 7368 6f77     inkscape:show
+000002c0: 7061 6765 7368 6164 6f77 3d22 3222 0a20  pageshadow="2". 
+000002d0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
+000002e0: 656f 7061 6369 7479 3d22 302e 3022 0a20  eopacity="0.0". 
+000002f0: 2020 2020 696e 6b73 6361 7065 3a70 6167      inkscape:pag
+00000300: 6563 6865 636b 6572 626f 6172 643d 2230  echeckerboard="0
+00000310: 220a 2020 2020 2069 6e6b 7363 6170 653a  ".     inkscape:
+00000320: 6465 736b 636f 6c6f 723d 2223 6431 6431  deskcolor="#d1d1
+00000330: 6431 220a 2020 2020 2073 686f 7767 7269  d1".     showgri
+00000340: 643d 2266 616c 7365 220a 2020 2020 2069  d="false".     i
+00000350: 6e6b 7363 6170 653a 7a6f 6f6d 3d22 342e  nkscape:zoom="4.
+00000360: 3132 3737 3637 3322 0a20 2020 2020 696e  1277673".     in
+00000370: 6b73 6361 7065 3a63 783d 2236 312e 3431  kscape:cx="61.41
+00000380: 3333 3435 220a 2020 2020 2069 6e6b 7363  3345".     inksc
+00000390: 6170 653a 6379 3d22 3130 322e 3233 3434  ape:cy="102.2344
+000003a0: 3422 0a20 2020 2020 696e 6b73 6361 7065  4".     inkscape
+000003b0: 3a77 696e 646f 772d 7769 6474 683d 2231  :window-width="1
+000003c0: 3932 3022 0a20 2020 2020 696e 6b73 6361  920".     inksca
+000003d0: 7065 3a77 696e 646f 772d 6865 6967 6874  pe:window-height
+000003e0: 3d22 3130 3139 220a 2020 2020 2069 6e6b  ="1019".     ink
+000003f0: 7363 6170 653a 7769 6e64 6f77 2d78 3d22  scape:window-x="
+00000400: 3022 0a20 2020 2020 696e 6b73 6361 7065  0".     inkscape
+00000410: 3a77 696e 646f 772d 793d 2230 220a 2020  :window-y="0".  
+00000420: 2020 2069 6e6b 7363 6170 653a 7769 6e64     inkscape:wind
+00000430: 6f77 2d6d 6178 696d 697a 6564 3d22 3122  ow-maximized="1"
+00000440: 0a20 2020 2020 696e 6b73 6361 7065 3a63  .     inkscape:c
+00000450: 7572 7265 6e74 2d6c 6179 6572 3d22 6738  urrent-layer="g8
+00000460: 2220 2f3e 0a20 203c 670a 2020 2020 2069  " />.  <g.     i
+00000470: 6e6b 7363 6170 653a 6772 6f75 706d 6f64  nkscape:groupmod
+00000480: 653d 226c 6179 6572 220a 2020 2020 2069  e="layer".     i
+00000490: 6e6b 7363 6170 653a 6c61 6265 6c3d 2249  nkscape:label="I
+000004a0: 6d61 6765 220a 2020 2020 2069 643d 2267  mage".     id="g
+000004b0: 3822 3e0a 2020 2020 3c72 6563 740a 2020  8">.    <rect.  
+000004c0: 2020 2020 2073 7479 6c65 3d22 6669 6c6c       style="fill
+000004d0: 3a23 6666 6666 6666 3b73 7472 6f6b 652d  :#ffffff;stroke-
+000004e0: 7769 6474 683a 302e 3830 3237 3037 3b73  width:0.802707;s
+000004f0: 7472 6f6b 652d 6c69 6e65 6361 703a 726f  troke-linecap:ro
+00000500: 756e 643b 7374 726f 6b65 2d6c 696e 656a  und;stroke-linej
+00000510: 6f69 6e3a 6265 7665 6c22 0a20 2020 2020  oin:bevel".     
+00000520: 2020 6964 3d22 7265 6374 3238 3722 0a20    id="rect287". 
+00000530: 2020 2020 2020 7769 6474 683d 2231 3539        width="159
+00000540: 2e32 3837 3038 220a 2020 2020 2020 2068  .28708".       h
+00000550: 6569 6768 743d 2231 3338 2e30 3438 3831  eight="138.04881
+00000560: 220a 2020 2020 2020 2078 3d22 3022 0a20  ".       x="0". 
+00000570: 2020 2020 2020 793d 2230 220a 2020 2020        y="0".    
+00000580: 2020 2072 793d 2237 2e37 3939 3830 3835     ry="7.7998085
+00000590: 2220 2f3e 0a20 2020 203c 7265 6374 0a20  " />.    <rect. 
+000005a0: 2020 2020 2020 7374 796c 653d 2266 696c        style="fil
+000005b0: 6c3a 2330 3030 3030 303b 7374 726f 6b65  l:#000000;stroke
+000005c0: 2d77 6964 7468 3a30 2e38 3032 3730 373b  -width:0.802707;
+000005d0: 7374 726f 6b65 2d6c 696e 6563 6170 3a72  stroke-linecap:r
+000005e0: 6f75 6e64 3b73 7472 6f6b 652d 6c69 6e65  ound;stroke-line
+000005f0: 6a6f 696e 3a62 6576 656c 220a 2020 2020  join:bevel".    
+00000600: 2020 2069 643d 2272 6563 7436 3032 220a     id="rect602".
+00000610: 2020 2020 2020 2077 6964 7468 3d22 3132         width="12
+00000620: 2e35 3936 3136 3422 0a20 2020 2020 2020  .596164".       
+00000630: 6865 6967 6874 3d22 3937 2e35 3034 3033  height="97.50403
+00000640: 3622 0a20 2020 2020 2020 783d 2232 372e  6".       x="27.
+00000650: 3437 3737 3236 220a 2020 2020 2020 2079  477726".       y
+00000660: 3d22 3231 2e35 3131 3934 2220 2f3e 0a20  ="21.51194" />. 
+00000670: 2020 203c 7265 6374 0a20 2020 2020 2020     <rect.       
+00000680: 7374 796c 653d 2266 696c 6c3a 2330 3030  style="fill:#000
+00000690: 3030 303b 7374 726f 6b65 2d77 6964 7468  000;stroke-width
+000006a0: 3a30 2e38 3032 3730 373b 7374 726f 6b65  :0.802707;stroke
+000006b0: 2d6c 696e 6563 6170 3a72 6f75 6e64 3b73  -linecap:round;s
+000006c0: 7472 6f6b 652d 6c69 6e65 6a6f 696e 3a62  troke-linejoin:b
+000006d0: 6576 656c 220a 2020 2020 2020 2069 643d  evel".       id=
+000006e0: 2272 6563 7436 3032 2d33 220a 2020 2020  "rect602-3".    
+000006f0: 2020 2077 6964 7468 3d22 3132 2e35 3936     width="12.596
+00000700: 3136 3422 0a20 2020 2020 2020 6865 6967  164".       heig
+00000710: 6874 3d22 3937 2e35 3034 3033 3622 0a20  ht="97.504036". 
+00000720: 2020 2020 2020 783d 2231 3138 2e30 3332        x="118.032
+00000730: 3038 220a 2020 2020 2020 2079 3d22 3231  08".       y="21
+00000740: 2e35 3131 3934 2220 2f3e 0a20 203c 2f67  .51194" />.  </g
+00000750: 3e0a 3c2f 7376 673e 0a                   >.</svg>.
```

### Comparing `crossroads-schematization-0.2.1/crschem/resources/island-300-white.svg` & `crossroads-schematization-0.2.2/crschem/resources/island-300-white.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/island-300.svg` & `crossroads-schematization-0.2.2/crschem/resources/island-300.svg`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-areas.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-areas.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-crossings.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-crossings.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-islands.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-islands.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-nodes-space.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-nodes.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-nodes.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-polylines-space.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-polylines-space.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/rendering-polylines.qml` & `crossroads-schematization-0.2.2/crschem/resources/rendering-polylines.qml`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/resources/style-300.xml` & `crossroads-schematization-0.2.2/crschem/resources/style-300.xml`

 * *Files 2% similar despite different names*

#### Comparing `crossroads-schematization-0.2.1/crschem/resources/style-300.xml` & `crossroads-schematization-0.2.2/crschem/resources/style-300.xml`

```diff
@@ -2,15 +2,15 @@
 <!-- 300 DPI correspond à 118,11 pixels par centimètre.
   On va donc utiliser l'approximation: 1mm = 12 pixels
  -->
 <Map background-color="white">
   <Style name="inner">
     <Rule>
       <!-- inner region with dots -->
-      <PolygonPatternSymbolizer file="point-300.png"/>
+      <PolygonPatternSymbolizer file="point-300.svg"/>
     </Rule>
   </Style>
   <Style name="sidewalks-space">
     <Rule>
       <!-- confort space (white) -->
       <LineSymbolizer stroke="#fff" stroke-width="48" stroke-linejoin="round" stroke-linecap="round"/>
     </Rule>
@@ -33,15 +33,15 @@
     </Rule>
   </Style>
   <Style name="crossings">
     <Rule>
       <Filter>[type] = crossing</Filter>
       <!-- TODO: add images for streets with a different width -->
       <!-- 3 meter street -->
-      <PointSymbolizer file="crossing-3-300.png" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
+      <PointSymbolizer file="crossing-3-300.svg" transform="rotate(180 + (-[orientatio] / 3.14) * 180)" allow-overlap="yes"/>
     </Rule>
   </Style>
   <Layer>
     <StyleName>inner</StyleName>
     <Datasource>
       <Parameter name="file">crossroad-inner.shp</Parameter>
       <Parameter name="type">shape</Parameter>
```

### Comparing `crossroads-schematization-0.2.1/crschem/resources/tactile-a5.qpt` & `crossroads-schematization-0.2.2/crschem/resources/tactile-a5.qpt`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/crschem/utils.py` & `crossroads-schematization-0.2.2/crschem/utils.py`

 * *Files identical despite different names*

### Comparing `crossroads-schematization-0.2.1/setup.py` & `crossroads-schematization-0.2.2/setup.py`

 * *Files identical despite different names*

