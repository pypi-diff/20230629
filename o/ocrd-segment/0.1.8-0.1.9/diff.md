# Comparing `tmp/ocrd_segment-0.1.8.tar.gz` & `tmp/ocrd_segment-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ocrd_segment-0.1.8.tar", last modified: Mon Feb  8 17:37:22 2021, max compression
+gzip compressed data, was "dist/ocrd_segment-0.1.9.tar", last modified: Wed Feb 10 10:41:24 2021, max compression
```

## Comparing `ocrd_segment-0.1.8.tar` & `ocrd_segment-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment/
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2812 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/evaluate.py
--rw-rw-r--   0 xbert     (1000) xbert     (1000)    10336 2021-02-06 00:07:28.000000 ocrd_segment-0.1.8/ocrd_segment/extract_glyphs.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     5905 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/replace_original.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    18811 2021-02-08 17:34:52.000000 ocrd_segment-0.1.8/ocrd_segment/ocrd-tool.json
--rw-r--r--   0 xbert     (1000) xbert     (1000)    10954 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/import_coco_segmentation.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/config.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     6567 2021-02-07 14:43:51.000000 ocrd_segment-0.1.8/ocrd_segment/replace_page.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2267 2021-02-06 00:09:42.000000 ocrd_segment-0.1.8/ocrd_segment/cli.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    24898 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/repair.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)    21586 2021-02-08 17:25:29.000000 ocrd_segment-0.1.8/ocrd_segment/extract_pages.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)      496 2021-02-06 00:09:08.000000 ocrd_segment-0.1.8/ocrd_segment/__init__.py
--rw-rw-r--   0 xbert     (1000) xbert     (1000)     9889 2021-02-06 00:00:52.000000 ocrd_segment-0.1.8/ocrd_segment/extract_words.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     8247 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/extract_regions.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     8209 2021-02-08 17:33:07.000000 ocrd_segment-0.1.8/ocrd_segment/import_image_segmentation.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     8854 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/ocrd_segment/extract_lines.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2186 2021-01-27 11:34:31.000000 ocrd_segment-0.1.8/README.md
-drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/
--rw-r--r--   0 xbert     (1000) xbert     (1000)      678 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/SOURCES.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)       13 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/top_level.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2891 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/PKG-INFO
--rw-r--r--   0 xbert     (1000) xbert     (1000)       47 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/requires.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)        1 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/dependency_links.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)      794 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/ocrd_segment.egg-info/entry_points.txt
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2216 2021-02-06 00:10:05.000000 ocrd_segment-0.1.8/setup.py
--rw-r--r--   0 xbert     (1000) xbert     (1000)     2891 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/PKG-INFO
--rw-r--r--   0 xbert     (1000) xbert     (1000)       38 2021-02-08 17:37:22.000000 ocrd_segment-0.1.8/setup.cfg
+drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/
+drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment/
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2812 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/evaluate.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    10908 2021-02-10 10:19:59.000000 ocrd_segment-0.1.9/ocrd_segment/extract_glyphs.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     5905 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/replace_original.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    19583 2021-02-10 10:25:32.000000 ocrd_segment-0.1.9/ocrd_segment/ocrd-tool.json
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    10954 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/import_coco_segmentation.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      138 2021-01-27 11:34:31.000000 ocrd_segment-0.1.9/ocrd_segment/config.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     6567 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/replace_page.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2267 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/cli.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    24898 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/repair.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    21751 2021-02-09 09:48:20.000000 ocrd_segment-0.1.9/ocrd_segment/extract_pages.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      496 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/__init__.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)    10380 2021-02-10 10:19:29.000000 ocrd_segment-0.1.9/ocrd_segment/extract_words.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     8247 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/extract_regions.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     8209 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/ocrd_segment/import_image_segmentation.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     9153 2021-02-10 10:18:35.000000 ocrd_segment-0.1.9/ocrd_segment/extract_lines.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2186 2021-01-27 11:34:31.000000 ocrd_segment-0.1.9/README.md
+drwxr-xr-x   0 xbert     (1000) xbert     (1000)        0 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      678 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/SOURCES.txt
+-rw-r--r--   0 xbert     (1000) xbert     (1000)       13 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/top_level.txt
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2891 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/PKG-INFO
+-rw-r--r--   0 xbert     (1000) xbert     (1000)       47 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/requires.txt
+-rw-r--r--   0 xbert     (1000) xbert     (1000)        1 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/dependency_links.txt
+-rw-r--r--   0 xbert     (1000) xbert     (1000)      794 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/ocrd_segment.egg-info/entry_points.txt
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2216 2021-02-08 17:44:48.000000 ocrd_segment-0.1.9/setup.py
+-rw-r--r--   0 xbert     (1000) xbert     (1000)     2891 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/PKG-INFO
+-rw-r--r--   0 xbert     (1000) xbert     (1000)       38 2021-02-10 10:41:24.000000 ocrd_segment-0.1.9/setup.cfg
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment/evaluate.py` & `ocrd_segment-0.1.9/ocrd_segment/evaluate.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/extract_glyphs.py` & `ocrd_segment-0.1.9/ocrd_segment/extract_glyphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         
         Open and deserialize PAGE input files and their respective images,
         then iterate over the element hierarchy down to the glyph level.
         
         Extract an image for each glyph (which depending on the workflow
         can already be deskewed, dewarped, binarized etc.), cropped to its
         minimal bounding box, and masked by the coordinate polygon outline.
+        Apply ``feature_filter`` (a comma-separated list of image features,
+        cf. :py:func:`ocrd.workspace.Workspace.image_from_page`) to skip
+        specific features when retrieving derived images.
         If ``transparency`` is true, then also add an alpha channel which is
         fully transparent outside of the mask.
         
         Create a JSON file with:
         * the IDs of the glyph and its parents,
         * the glyph's text content,
         * the glyph's coordinates relative to the line image,
@@ -71,14 +74,15 @@
             page_id = input_file.pageId or input_file.ID
             LOG.info("INPUT FILE %i / %s", n, page_id)
             pcgts = page_from_file(self.workspace.download_file(input_file))
             self.add_metadata(pcgts)
             page = pcgts.get_Page()
             page_image, page_coords, page_image_info = self.workspace.image_from_page(
                 page, page_id,
+                feature_filter=self.parameter['feature_filter'],
                 transparency=self.parameter['transparency'])
             if page_image_info.resolution != 1:
                 dpi = page_image_info.resolution
                 if page_image_info.resolutionUnit == 'cm':
                     dpi = round(dpi * 2.54)
             else:
                 dpi = None
@@ -88,37 +92,41 @@
                 [page.get_TextRegion()] +
                 [subregion.get_TextRegion() for subregion in page.get_TableRegion()])
             if not regions:
                 LOG.warning("Page '%s' contains no text regions", page_id)
             for region in regions:
                 region_image, region_coords = self.workspace.image_from_segment(
                     region, page_image, page_coords,
+                    feature_filter=self.parameter['feature_filter'],
                     transparency=self.parameter['transparency'])
                 rtype = region.get_type()
                 
                 lines = region.get_TextLine()
                 if not lines:
                     LOG.warning("Region '%s' contains no text lines", region.id)
                 for line in lines:
                     line_image, line_coords = self.workspace.image_from_segment(
                         line, region_image, region_coords,
+                        feature_filter=self.parameter['feature_filter'],
                         transparency=self.parameter['transparency'])
                     words = line.get_Word()
                     if not words:
                         LOG.warning("Line '%s' contains no words", line.id)
                     for word in words:
                         word_image, word_coords = self.workspace.image_from_segment(
                             word, line_image, line_coords,
+                            feature_filter=self.parameter['feature_filter'],
                             transparency=self.parameter['transparency'])
                         glyphs = word.get_Glyph()
                         if not glyphs:
                             LOG.warning("Word '%s' contains no glyphs", word.id)
                         for glyph in glyphs:
                             glyph_image, glyph_coords = self.workspace.image_from_segment(
                                 glyph, word_image, word_coords,
+                                feature_filter=self.parameter['feature_filter'],
                                 transparency=self.parameter['transparency'])
                             lpolygon_rel = coordinates_of_segment(
                                 glyph, glyph_image, glyph_coords).tolist()
                             lpolygon_abs = polygon_from_points(glyph.get_Coords().points)
                             ltext = glyph.get_TextEquiv()
                             if not ltext:
                                 LOG.warning("Glyph '%s' contains no text content", glyph.id)
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment/replace_original.py` & `ocrd_segment-0.1.9/ocrd_segment/replace_original.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/ocrd-tool.json` & `ocrd_segment-0.1.9/ocrd_segment/ocrd-tool.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.829064454064454%*

 * *Differences: {"'tools'": "{'ocrd-segment-extract-pages': {'output_file_grp': ['OCR-D-IMG-PAGE']}, "*

 * *            "'ocrd-segment-extract-regions': {'output_file_grp': ['OCR-D-IMG-REGION'], "*

 * *            "'parameters': {'feature_filter': OrderedDict([('type', 'string'), ('default', ''), "*

 * *            "('description', 'Comma-separated list of forbidden image features (e.g. "*

 * *            "`binarized,despeckled`).')])}}, 'ocrd-segment-extract-lines': {'output_file_grp': "*

 * *            "['OCR-D-IMG-LINE'], 'parameters': {'featu […]*

```diff
@@ -23,17 +23,22 @@
             "description": "Extract glyph segmentation as glyph images (deskewed according to `*/@orientation` and cropped+masked along `*/Coords` polygon and dewarped as in `*/AlternativeImage`) + text file (according to `*/TextEquiv`) + JSON (including line coordinates and meta-data).",
             "executable": "ocrd-segment-extract-glyphs",
             "input_file_grp": [
                 "OCR-D-SEG-GLYPH",
                 "OCR-D-GT-SEG-GLYPH"
             ],
             "output_file_grp": [
-                "OCR-D-IMG-CROP"
+                "OCR-D-IMG-GLYPH"
             ],
             "parameters": {
+                "feature_filter": {
+                    "default": "",
+                    "description": "Comma-separated list of forbidden image features (e.g. `binarized,despeckled`).",
+                    "type": "string"
+                },
                 "mimetype": {
                     "default": "image/png",
                     "description": "File format to save extracted images in.",
                     "enum": [
                         "image/bmp",
                         "application/postscript",
                         "image/gif",
@@ -62,17 +67,22 @@
             "description": "Extract line segmentation as line images (deskewed according to `*/@orientation` and cropped+masked along `*/Coords` polygon and dewarped as in `*/AlternativeImage`) + text file (according to `*/TextEquiv`) + JSON (including line coordinates and meta-data).",
             "executable": "ocrd-segment-extract-lines",
             "input_file_grp": [
                 "OCR-D-SEG-LINE",
                 "OCR-D-GT-SEG-LINE"
             ],
             "output_file_grp": [
-                "OCR-D-IMG-CROP"
+                "OCR-D-IMG-LINE"
             ],
             "parameters": {
+                "feature_filter": {
+                    "default": "",
+                    "description": "Comma-separated list of forbidden image features (e.g. `binarized,despeckled`).",
+                    "type": "string"
+                },
                 "mimetype": {
                     "default": "image/png",
                     "description": "File format to save extracted images in.",
                     "enum": [
                         "image/bmp",
                         "application/postscript",
                         "image/gif",
@@ -103,15 +113,15 @@
             "input_file_grp": [
                 "OCR-D-SEG-PAGE",
                 "OCR-D-GT-SEG-PAGE",
                 "OCR-D-SEG-BLOCK",
                 "OCR-D-GT-SEG-BLOCK"
             ],
             "output_file_grp": [
-                "OCR-D-IMG-CROP"
+                "OCR-D-IMG-PAGE"
             ],
             "parameters": {
                 "colordict": {
                     "default": {
                         "": "FFFFFF00",
                         "AdvertRegion": "4682B4FF",
                         "Border": "FFFFFFFF",
@@ -225,17 +235,22 @@
             "description": "Extract region segmentation as region images (deskewed according to `*/@orientation` and cropped+masked along `*/Coords` polygon) + JSON (including region coordinates/classes and meta-data).",
             "executable": "ocrd-segment-extract-regions",
             "input_file_grp": [
                 "OCR-D-SEG-BLOCK",
                 "OCR-D-GT-SEG-BLOCK"
             ],
             "output_file_grp": [
-                "OCR-D-IMG-CROP"
+                "OCR-D-IMG-REGION"
             ],
             "parameters": {
+                "feature_filter": {
+                    "default": "",
+                    "description": "Comma-separated list of forbidden image features (e.g. `binarized,despeckled`).",
+                    "type": "string"
+                },
                 "mimetype": {
                     "default": "image/png",
                     "description": "File format to save extracted images in.",
                     "enum": [
                         "image/bmp",
                         "application/postscript",
                         "image/gif",
@@ -264,17 +279,22 @@
             "description": "Extract word segmentation as word images (deskewed according to `*/@orientation` and cropped+masked along `*/Coords` polygon and dewarped as in `*/AlternativeImage`) + text file (according to `*/TextEquiv`) + JSON (including line coordinates and meta-data).",
             "executable": "ocrd-segment-extract-words",
             "input_file_grp": [
                 "OCR-D-SEG-WORD",
                 "OCR-D-GT-SEG-WORD"
             ],
             "output_file_grp": [
-                "OCR-D-IMG-CROP"
+                "OCR-D-IMG-WORD"
             ],
             "parameters": {
+                "feature_filter": {
+                    "default": "",
+                    "description": "Comma-separated list of forbidden image features (e.g. `binarized,despeckled`).",
+                    "type": "string"
+                },
                 "mimetype": {
                     "default": "image/png",
                     "description": "File format to save extracted images in.",
                     "enum": [
                         "image/bmp",
                         "application/postscript",
                         "image/gif",
@@ -434,26 +454,25 @@
             "executable": "ocrd-segment-replace-original",
             "input_file_grp": [
                 "OCR-D-SEG-LINE",
                 "OCR-D-GT-SEG-LINE",
                 "OCR-D-OCR"
             ],
             "output_file_grp": [
-                "OCR-D-SEG-CROP",
-                "OCR-D-IMG-CROP"
+                "OCR-D-SEG-CROP"
             ],
             "parameters": {
                 "feature_filter": {
                     "default": "",
-                    "description": "comma-separated list of forbidden image features (e.g. binarized,despeckled)",
+                    "description": "Comma-separated list of forbidden image features (e.g. `binarized,despeckled`)",
                     "type": "string"
                 },
                 "feature_selector": {
                     "default": "",
-                    "description": "comma-separated list of required image features (e.g. binarized,despeckled)",
+                    "description": "Comma-separated list of required image features (e.g. `binarized,despeckled`)",
                     "type": "string"
                 },
                 "transform_coordinates": {
                     "default": true,
                     "description": "re-calculate coordinates for all segments of the structural hierarchy to be consistent with the coordinate system of the chosen image again (vital after cropping, deskewing etc; disable only if input coordinates must be assumed to be inconsistent with the original)",
                     "type": "boolean"
                 }
@@ -470,24 +489,24 @@
             "executable": "ocrd-segment-replace-page",
             "input_file_grp": [
                 "OCR-D-SEG-LINE",
                 "OCR-D-GT-SEG-LINE",
                 "OCR-D-OCR"
             ],
             "output_file_grp": [
-                "OCR-D-SEG-CROP",
-                "OCR-D-IMG-CROP"
+                "OCR-D-SEG-LINE",
+                "OCR-D-OCR"
             ],
             "parameters": {
                 "transform_coordinates": {
                     "default": true,
                     "description": "re-calculate coordinates for all segments of the structural hierarchy to be consistent with the coordinate system of the first input file group (vital after cropping, deskewing etc; disable only if input coordinates can be assumed to be consistent with the second input file group)",
                     "type": "boolean"
                 }
             },
             "steps": [
                 "layout/analysis"
             ]
         }
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment/import_coco_segmentation.py` & `ocrd_segment-0.1.9/ocrd_segment/import_coco_segmentation.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/replace_page.py` & `ocrd_segment-0.1.9/ocrd_segment/replace_page.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/cli.py` & `ocrd_segment-0.1.9/ocrd_segment/cli.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/repair.py` & `ocrd_segment-0.1.9/ocrd_segment/repair.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/extract_pages.py` & `ocrd_segment-0.1.9/ocrd_segment/extract_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,19 @@
                  'source': 'PAGE', 'color': color})
             i += 1
 
         i = 0
         # pylint: disable=attribute-defined-outside-init
         for n, input_file in enumerate(self.input_files):
             page_id = input_file.pageId or input_file.ID
-            num_page_id = int(page_id.strip(page_id.strip("0123456789")))
+            try:
+                # separate non-numeric part of page ID to retain the numeric part
+                num_page_id = int(page_id.strip(page_id.strip("0123456789")))
+            except Exception:
+                num_page_id = n
             LOG.info("INPUT FILE %i / %s", n, page_id)
             pcgts = page_from_file(self.workspace.download_file(input_file))
             self.add_metadata(pcgts)
             page = pcgts.get_Page()
             ptype = page.get_type()
             page_image, page_coords, page_image_info = self.workspace.image_from_page(
                 page, page_id,
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment/extract_words.py` & `ocrd_segment-0.1.9/ocrd_segment/extract_words.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,17 @@
         
         Open and deserialize PAGE input files and their respective images,
         then iterate over the element hierarchy down to the word level.
         
         Extract an image for each word (which depending on the workflow
         can already be deskewed, dewarped, binarized etc.), cropped to its
         minimal bounding box, and masked by the coordinate polygon outline.
+        Apply ``feature_filter`` (a comma-separated list of image features,
+        cf. :py:func:`ocrd.workspace.Workspace.image_from_page`) to skip
+        specific features when retrieving derived images.
         If ``transparency`` is true, then also add an alpha channel which is
         fully transparent outside of the mask.
         
         Create a JSON file with:
         * the IDs of the word and its parents,
         * the word's text content,
         * the word's coordinates relative to the line image,
@@ -71,14 +74,15 @@
             page_id = input_file.pageId or input_file.ID
             LOG.info("INPUT FILE %i / %s", n, page_id)
             pcgts = page_from_file(self.workspace.download_file(input_file))
             self.add_metadata(pcgts)
             page = pcgts.get_Page()
             page_image, page_coords, page_image_info = self.workspace.image_from_page(
                 page, page_id,
+                feature_filter=self.parameter['feature_filter'],
                 transparency=self.parameter['transparency'])
             if page_image_info.resolution != 1:
                 dpi = page_image_info.resolution
                 if page_image_info.resolutionUnit == 'cm':
                     dpi = round(dpi * 2.54)
             else:
                 dpi = None
@@ -88,30 +92,33 @@
                 [page.get_TextRegion()] +
                 [subregion.get_TextRegion() for subregion in page.get_TableRegion()])
             if not regions:
                 LOG.warning("Page '%s' contains no text regions", page_id)
             for region in regions:
                 region_image, region_coords = self.workspace.image_from_segment(
                     region, page_image, page_coords,
+                    feature_filter=self.parameter['feature_filter'],
                     transparency=self.parameter['transparency'])
                 rtype = region.get_type()
                 
                 lines = region.get_TextLine()
                 if not lines:
                     LOG.warning("Region '%s' contains no text lines", region.id)
                 for line in lines:
                     line_image, line_coords = self.workspace.image_from_segment(
                         line, region_image, region_coords,
+                        feature_filter=self.parameter['feature_filter'],
                         transparency=self.parameter['transparency'])
                     words = line.get_Word()
                     if not words:
                         LOG.warning("Line '%s' contains no words", line.id)
                     for word in words:
                         word_image, word_coords = self.workspace.image_from_segment(
                             word, line_image, line_coords,
+                            feature_filter=self.parameter['feature_filter'],
                             transparency=self.parameter['transparency'])
                         lpolygon_rel = coordinates_of_segment(
                             word, word_image, word_coords).tolist()
                         lpolygon_abs = polygon_from_points(word.get_Coords().points)
                         ltext = word.get_TextEquiv()
                         if not ltext:
                             LOG.warning("Word '%s' contains no text content", word.id)
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment/extract_regions.py` & `ocrd_segment-0.1.9/ocrd_segment/extract_regions.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/import_image_segmentation.py` & `ocrd_segment-0.1.9/ocrd_segment/import_image_segmentation.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment/extract_lines.py` & `ocrd_segment-0.1.9/ocrd_segment/extract_lines.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import absolute_import
 
 import json
-import itertools
 
 from ocrd_utils import (
     getLogger,
     make_file_id,
     assert_file_grp_cardinality,
     coordinates_of_segment,
     polygon_from_points,
@@ -30,14 +29,17 @@
         
         Open and deserialize PAGE input files and their respective images,
         then iterate over the element hierarchy down to the line level.
         
         Extract an image for each textline (which depending on the workflow
         can already be deskewed, dewarped, binarized etc.), cropped to its
         minimal bounding box, and masked by the coordinate polygon outline.
+        Apply ``feature_filter`` (a comma-separated list of image features,
+        cf. :py:func:`ocrd.workspace.Workspace.image_from_page`) to skip
+        specific features when retrieving derived images.
         If ``transparency`` is true, then also add an alpha channel which is
         fully transparent outside of the mask.
         
         Create a JSON file with:
         * the IDs of the textline and its parents,
         * the textline's text content,
         * the textline's coordinates relative to the line image,
@@ -71,40 +73,41 @@
             page_id = input_file.pageId or input_file.ID
             LOG.info("INPUT FILE %i / %s", n, page_id)
             pcgts = page_from_file(self.workspace.download_file(input_file))
             self.add_metadata(pcgts)
             page = pcgts.get_Page()
             page_image, page_coords, page_image_info = self.workspace.image_from_page(
                 page, page_id,
+                feature_filter=self.parameter['feature_filter'],
                 transparency=self.parameter['transparency'])
             if page_image_info.resolution != 1:
                 dpi = page_image_info.resolution
                 if page_image_info.resolutionUnit == 'cm':
                     dpi = round(dpi * 2.54)
             else:
                 dpi = None
             ptype = page.get_type()
             
-            regions = itertools.chain.from_iterable(
-                [page.get_TextRegion()] +
-                [subregion.get_TextRegion() for subregion in page.get_TableRegion()])
+            regions = page.get_AllRegions(classes=['Text'], order='reading-order')
             if not regions:
                 LOG.warning("Page '%s' contains no text regions", page_id)
             for region in regions:
                 region_image, region_coords = self.workspace.image_from_segment(
                     region, page_image, page_coords,
+                    feature_filter=self.parameter['feature_filter'],
                     transparency=self.parameter['transparency'])
                 rtype = region.get_type()
                 
                 lines = region.get_TextLine()
                 if not lines:
                     LOG.warning("Region '%s' contains no text lines", region.id)
                 for line in lines:
                     line_image, line_coords = self.workspace.image_from_segment(
                         line, region_image, region_coords,
+                        feature_filter=self.parameter['feature_filter'],
                         transparency=self.parameter['transparency'])
                     lpolygon_rel = coordinates_of_segment(
                         line, line_image, line_coords).tolist()
                     lpolygon_abs = polygon_from_points(line.get_Coords().points)
                     ltext = line.get_TextEquiv()
                     if not ltext:
                         LOG.warning("Line '%s' contains no text content", line.id)
```

### Comparing `ocrd_segment-0.1.8/README.md` & `ocrd_segment-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment.egg-info/SOURCES.txt` & `ocrd_segment-0.1.9/ocrd_segment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/ocrd_segment.egg-info/PKG-INFO` & `ocrd_segment-0.1.9/ocrd_segment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrd-segment
-Version: 0.1.8
+Version: 0.1.9
 Summary: Page segmentation and segmentation evaluation
 Home-page: https://github.com/OCR-D/ocrd_segment
 Author: Konstantin Baierer, Kay-Michael Würzner, Robert Sachunsky
 Author-email: unixprog@gmail.com, wuerzner@gmail.com, sachunsky@informatik.uni-leipzig.de
 License: Apache License 2.0
 Description: # ocrd_segment
```

### Comparing `ocrd_segment-0.1.8/ocrd_segment.egg-info/entry_points.txt` & `ocrd_segment-0.1.9/ocrd_segment.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/setup.py` & `ocrd_segment-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ocrd_segment-0.1.8/PKG-INFO` & `ocrd_segment-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocrd_segment
-Version: 0.1.8
+Version: 0.1.9
 Summary: Page segmentation and segmentation evaluation
 Home-page: https://github.com/OCR-D/ocrd_segment
 Author: Konstantin Baierer, Kay-Michael Würzner, Robert Sachunsky
 Author-email: unixprog@gmail.com, wuerzner@gmail.com, sachunsky@informatik.uni-leipzig.de
 License: Apache License 2.0
 Description: # ocrd_segment
```

