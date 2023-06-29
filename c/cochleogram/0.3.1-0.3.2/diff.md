# Comparing `tmp/cochleogram-0.3.1.tar.gz` & `tmp/cochleogram-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochleogram-0.3.1.tar", last modified: Thu Jun 22 19:50:03 2023, max compression
+gzip compressed data, was "cochleogram-0.3.2.tar", last modified: Thu Jun 29 17:33:58 2023, max compression
```

## Comparing `cochleogram-0.3.1.tar` & `cochleogram-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.885881 cochleogram-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.885881 cochleogram-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-22 19:49:52.000000 cochleogram-0.3.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-22 19:49:52.000000 cochleogram-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-22 19:50:03.889881 cochleogram-0.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/gui.enaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/cells.png
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/exclude.png
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/main-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/make_icons.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/spiral.png
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/icons/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)    23257 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/instructions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/presenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-22 19:49:52.000000 cochleogram-0.3.1/cochleogram/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:50:03.889881 cochleogram-0.3.1/cochleogram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 19:50:03.000000 cochleogram-0.3.1/cochleogram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-22 19:49:52.000000 cochleogram-0.3.1/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 19:49:52.000000 cochleogram-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-06-22 19:49:52.000000 cochleogram-0.3.1/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:50:03.889881 cochleogram-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.467877 cochleogram-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.463877 cochleogram-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.467877 cochleogram-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-29 17:33:48.000000 cochleogram-0.3.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-29 17:33:48.000000 cochleogram-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-29 17:33:58.467877 cochleogram-0.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.467877 cochleogram-0.3.2/cochleogram/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23682 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/gui.enaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.467877 cochleogram-0.3.2/cochleogram/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/cells.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/exclude.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/main-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/make_icons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/spiral.png
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/icons/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23277 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/instructions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23013 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28052 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/presenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-29 17:33:48.000000 cochleogram-0.3.2/cochleogram/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:33:58.467877 cochleogram-0.3.2/cochleogram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 17:33:58.000000 cochleogram-0.3.2/cochleogram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-29 17:33:48.000000 cochleogram-0.3.2/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-29 17:33:48.000000 cochleogram-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-29 17:33:48.000000 cochleogram-0.3.2/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:33:58.467877 cochleogram-0.3.2/setup.cfg
```

### Comparing `cochleogram-0.3.1/.github/workflows/publish-to-pypi.yml` & `cochleogram-0.3.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/.gitignore` & `cochleogram-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/PKG-INFO` & `cochleogram-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.3.1
+Version: 0.3.2
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
@@ -36,19 +36,19 @@
 example:
 
     B009-8L-CtBP2-MyosinVIIa-PMT
 
 Inside each file, the pieces must be numbered sequentially from base (hook) to
 apex. If more htan one image is required for a piece, use letters for the
 suffixes (i.e., "piece2a", "piece2b", etc.). The order in which the images for
-a single piece are labeled does nto matter since the program will automatically
+a single piece are labeled does not matter since the program will automatically
 align them based on the stage coordinates stored in the file.
 
-We currently do not have support for missing pieces. This will be added
-shortly.
+We currently do not have support for missing pieces. This will be added once
+the need arises.
 
 Using the program
 -----------------
 
 Mouse interaction
 .................
 left click
@@ -104,26 +104,24 @@
 the result of the current step before moving to the next step. Although you can
 go back and edit a previous step, it may affect your analysis (e.g., if you
 need to move a tile after marking hair cells, you may have to manually edit
 a large number of hair cells).
 
 **Tile mode**
 
-Start by selecting "tiles" from the edit buttons, then left-clicking to select the tile that is
-misaligned. Using the arrow keys, you can move the tile until it is properly
-aligned with the other tiles. If you need to move the tile in smaller steps,
-hold down the shift key at the same time as the arrow keys. It may be helpful
-to toggle "highlight selected" so that you get a transparent overlay. When in
-"highlight selected" mode, the currently selected tile will be shown with a red
-border.
+Start by selecting "tiles" from the edit buttons, then left-clicking to select
+the tile that is misaligned. Using the arrow keys, you can move the tile until
+it is properly aligned with the other tiles. If you need to move the tile in
+smaller steps, hold down the shift key at the same time as the arrow keys. It
+may be helpful to toggle "highlight selected" so that you get a transparent
+overlay. When in "highlight selected" mode, the currently selected tile will be
+shown with a red border.
 
 left click
     Select tile
-left click + drag
-    Pan image
 mouse wheel
     Zoom in/out
 arrow keys
     Move currently selected tile (large steps)
 shift + arrow keys
     Move currently selected tile (small steps)
 n
@@ -151,15 +149,15 @@
 the nuclei (IHCs) or cuticular plate (OHCs) as that will facilitate the
 semi-automated algorithms implemented by the program to help mark hair cells.
 
 right click
     Add point
 shift + right click
     Remove point
-contrl + right click
+control + right click
     Set point as origin for spiral
 
 **Cell mode**
 
 After marking the spiral, run the algorithm to automatically detect cells. You
 can play with the settings (each time you run, it will delete the existing
 cells and create new ones). You will likely have to manually edit the
@@ -168,33 +166,33 @@
 
 right click
     Add cell
 shift + right click
     Remove cell
 
 From time to time there will be a fourth row of OHCs. These should manually be
-identified by selecting "extra" from the edit mode and then selecting the cell
-tool. Since the fourth row tends to be very short in length, you cannot mark
-a spiral or mark the region as excluded.
+identified by selecting "extra" for the cell you would like to edit and then
+adding the cells using the cell tool.  Since the fourth row tends to be very
+short in length, you cannot mark a spiral or mark the region as excluded.
 
 **Exclude mode**
 
 Finally, go back through each row of hair cells. If there was a region you felt
 you could not intepret properly, select the exclude tool. Right-click the
 spiral at one end of the region then right-click again at the other end of the
 region you wish to exclude.
 
 right click
     Start region. Click again to end region.
-alt + rigth click
-    Remove region.
+shift + right click
+    Remove region under mouse cursor.
 escape
     Cancel current region.
 
 Some additional tools are made available to facilitate this process:
 
-* You can copy a set of excluded regions to any other spiral.
 * You can merge all excluded regions across the OHC spirals into a single set
-  of excluded regions that apply to all OHC spirals.</li>
+  of excluded regions that apply to all OHC spirals (`Combine OHC exclusions`
+  button).
 * You can simplify a set of excluded regions for a particular spiral if they
   are overlapping (this will combine overlapping exclusion regions into
-  a single exclusion region).
+  a single exclusion region) using the `Simplify exclusions` button.
```

### Comparing `cochleogram-0.3.1/cochleogram/gui.enaml` & `cochleogram-0.3.2/cochleogram/gui.enaml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/cells.png` & `cochleogram-0.3.2/cochleogram/icons/cells.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/exclude.png` & `cochleogram-0.3.2/cochleogram/icons/exclude.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/main-icon.png` & `cochleogram-0.3.2/cochleogram/icons/main-icon.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/make_icons.py` & `cochleogram-0.3.2/cochleogram/icons/make_icons.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/spiral.png` & `cochleogram-0.3.2/cochleogram/icons/spiral.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/icons/tile.png` & `cochleogram-0.3.2/cochleogram/icons/tile.png`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/instructions.html` & `cochleogram-0.3.2/cochleogram/instructions.html`

 * *Files 2% similar despite different names*

```diff
@@ -625,18 +625,18 @@
 example:</p>
 <blockquote>
 <p>B009-8L-CtBP2-MyosinVIIa-PMT</p>
 </blockquote>
 <p>Inside each file, the pieces must be numbered sequentially from base (hook) to
 apex. If more htan one image is required for a piece, use letters for the
 suffixes (i.e., &quot;piece2a&quot;, &quot;piece2b&quot;, etc.). The order in which the images for
-a single piece are labeled does nto matter since the program will automatically
+a single piece are labeled does not matter since the program will automatically
 align them based on the stage coordinates stored in the file.</p>
-<p>We currently do not have support for missing pieces. This will be added
-shortly.</p>
+<p>We currently do not have support for missing pieces. This will be added once
+the need arises.</p>
 </section>
 </section>
 <section id="using-the-program">
 <h2>Using the program</h2>
 <section id="mouse-interaction">
 <h3>Mouse interaction</h3>
 <dl class="simple">
@@ -708,28 +708,25 @@
 </ul>
 <p>Tools are provided to facilitate each step. Be sure that you are satisfied with
 the result of the current step before moving to the next step. Although you can
 go back and edit a previous step, it may affect your analysis (e.g., if you
 need to move a tile after marking hair cells, you may have to manually edit
 a large number of hair cells).</p>
 <p><strong>Tile mode</strong></p>
-<p>Start by selecting &quot;tiles&quot; from the edit buttons, then left-clicking to select the tile that is
-misaligned. Using the arrow keys, you can move the tile until it is properly
-aligned with the other tiles. If you need to move the tile in smaller steps,
-hold down the shift key at the same time as the arrow keys. It may be helpful
-to toggle &quot;highlight selected&quot; so that you get a transparent overlay. When in
-&quot;highlight selected&quot; mode, the currently selected tile will be shown with a red
-border.</p>
+<p>Start by selecting &quot;tiles&quot; from the edit buttons, then left-clicking to select
+the tile that is misaligned. Using the arrow keys, you can move the tile until
+it is properly aligned with the other tiles. If you need to move the tile in
+smaller steps, hold down the shift key at the same time as the arrow keys. It
+may be helpful to toggle &quot;highlight selected&quot; so that you get a transparent
+overlay. When in &quot;highlight selected&quot; mode, the currently selected tile will be
+shown with a red border.</p>
 <dl class="simple">
 <dt>left click</dt>
 <dd><p>Select tile</p>
 </dd>
-<dt>left click + drag</dt>
-<dd><p>Pan image</p>
-</dd>
 <dt>mouse wheel</dt>
 <dd><p>Zoom in/out</p>
 </dd>
 <dt>arrow keys</dt>
 <dd><p>Move currently selected tile (large steps)</p>
 </dd>
 <dt>shift + arrow keys</dt>
@@ -761,15 +758,15 @@
 <dl class="simple">
 <dt>right click</dt>
 <dd><p>Add point</p>
 </dd>
 <dt>shift + right click</dt>
 <dd><p>Remove point</p>
 </dd>
-<dt>contrl + right click</dt>
+<dt>control + right click</dt>
 <dd><p>Set point as origin for spiral</p>
 </dd>
 </dl>
 <p><strong>Cell mode</strong></p>
 <p>After marking the spiral, run the algorithm to automatically detect cells. You
 can play with the settings (each time you run, it will delete the existing
 cells and create new ones). You will likely have to manually edit the
@@ -780,40 +777,40 @@
 <dd><p>Add cell</p>
 </dd>
 <dt>shift + right click</dt>
 <dd><p>Remove cell</p>
 </dd>
 </dl>
 <p>From time to time there will be a fourth row of OHCs. These should manually be
-identified by selecting &quot;extra&quot; from the edit mode and then selecting the cell
-tool. Since the fourth row tends to be very short in length, you cannot mark
-a spiral or mark the region as excluded.</p>
+identified by selecting &quot;extra&quot; for the cell you would like to edit and then
+adding the cells using the cell tool.  Since the fourth row tends to be very
+short in length, you cannot mark a spiral or mark the region as excluded.</p>
 <p><strong>Exclude mode</strong></p>
 <p>Finally, go back through each row of hair cells. If there was a region you felt
 you could not intepret properly, select the exclude tool. Right-click the
 spiral at one end of the region then right-click again at the other end of the
 region you wish to exclude.</p>
 <dl class="simple">
 <dt>right click</dt>
 <dd><p>Start region. Click again to end region.</p>
 </dd>
-<dt>alt + rigth click</dt>
-<dd><p>Remove region.</p>
+<dt>shift + right click</dt>
+<dd><p>Remove region under mouse cursor.</p>
 </dd>
 <dt>escape</dt>
 <dd><p>Cancel current region.</p>
 </dd>
 </dl>
 <p>Some additional tools are made available to facilitate this process:</p>
 <ul class="simple">
-<li><p>You can copy a set of excluded regions to any other spiral.</p></li>
 <li><p>You can merge all excluded regions across the OHC spirals into a single set
-of excluded regions that apply to all OHC spirals.&lt;/li&gt;</p></li>
+of excluded regions that apply to all OHC spirals (<cite>Combine OHC exclusions</cite>
+button).</p></li>
 <li><p>You can simplify a set of excluded regions for a particular spiral if they
 are overlapping (this will combine overlapping exclusion regions into
-a single exclusion region).</p></li>
+a single exclusion region) using the <cite>Simplify exclusions</cite> button.</p></li>
 </ul>
 </section>
 </section>
 </main>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -15,18 +15,18 @@
 Files should be named with the identifier (e.g., animal ID and ear) followed
 byt the label for each channel in the order the channels were imaged. For
 example:
      B009-8L-CtBP2-MyosinVIIa-PMT
 Inside each file, the pieces must be numbered sequentially from base (hook) to
 apex. If more htan one image is required for a piece, use letters for the
 suffixes (i.e., "piece2a", "piece2b", etc.). The order in which the images for
-a single piece are labeled does nto matter since the program will automatically
+a single piece are labeled does not matter since the program will automatically
 align them based on the stage coordinates stored in the file.
-We currently do not have support for missing pieces. This will be added
-shortly.
+We currently do not have support for missing pieces. This will be added once
+the need arises.
 
 ***** Using the program *****
 **** Mouse interaction ****
   left click
       Select tile
   left click + drag
       Pan image
@@ -81,16 +81,14 @@
 it is properly aligned with the other tiles. If you need to move the tile in
 smaller steps, hold down the shift key at the same time as the arrow keys. It
 may be helpful to toggle "highlight selected" so that you get a transparent
 overlay. When in "highlight selected" mode, the currently selected tile will be
 shown with a red border.
   left click
       Select tile
-  left click + drag
-      Pan image
   mouse wheel
       Zoom in/out
   arrow keys
       Move currently selected tile (large steps)
   shift + arrow keys
       Move currently selected tile (small steps)
   n
@@ -112,42 +110,42 @@
 Repeat the process for OHC1, OHC2, and OHC3. Be sure that the spiral bisects
 the nuclei (IHCs) or cuticular plate (OHCs) as that will facilitate the semi-
 automated algorithms implemented by the program to help mark hair cells.
   right click
       Add point
   shift + right click
       Remove point
-  contrl + right click
+  control + right click
       Set point as origin for spiral
 Cell mode
 After marking the spiral, run the algorithm to automatically detect cells. You
 can play with the settings (each time you run, it will delete the existing
 cells and create new ones). You will likely have to manually edit the
 automatically-detected cells. Select the cell tool and then use right click to
 add cells and shift + left click to delete cells.
   right click
       Add cell
   shift + right click
       Remove cell
 From time to time there will be a fourth row of OHCs. These should manually be
-identified by selecting "extra" from the edit mode and then selecting the cell
-tool. Since the fourth row tends to be very short in length, you cannot mark a
-spiral or mark the region as excluded.
+identified by selecting "extra" for the cell you would like to edit and then
+adding the cells using the cell tool. Since the fourth row tends to be very
+short in length, you cannot mark a spiral or mark the region as excluded.
 Exclude mode
 Finally, go back through each row of hair cells. If there was a region you felt
 you could not intepret properly, select the exclude tool. Right-click the
 spiral at one end of the region then right-click again at the other end of the
 region you wish to exclude.
   right click
       Start region. Click again to end region.
-  alt + rigth click
-      Remove region.
+  shift + right click
+      Remove region under mouse cursor.
   escape
       Cancel current region.
 Some additional tools are made available to facilitate this process:
-    * You can copy a set of excluded regions to any other spiral.
     * You can merge all excluded regions across the OHC spirals into a single
-      set of excluded regions that apply to all OHC spirals.</li>
+      set of excluded regions that apply to all OHC spirals (Combine OHC
+      exclusionsbutton).
     * You can simplify a set of excluded regions for a particular spiral if
       they are overlapping (this will combine overlapping exclusion regions
-      into a single exclusion region).
+      into a single exclusion region) using theSimplify exclusionsbutton.
```

### Comparing `cochleogram-0.3.1/cochleogram/main.py` & `cochleogram-0.3.2/cochleogram/main.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/model.py` & `cochleogram-0.3.2/cochleogram/model.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/plot.py` & `cochleogram-0.3.2/cochleogram/plot.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/presenter.py` & `cochleogram-0.3.2/cochleogram/presenter.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/readers.py` & `cochleogram-0.3.2/cochleogram/readers.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram/util.py` & `cochleogram-0.3.2/cochleogram/util.py`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/cochleogram.egg-info/PKG-INFO` & `cochleogram-0.3.2/cochleogram.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cochleogram
-Version: 0.3.1
+Version: 0.3.2
 Summary: Module for creating cochleograms from confocal images
 Author-email: Brad Buran <buran@ohsu.edu>
 Maintainer-email: Brad Buran <buran@ohsu.edu>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: czi
 Provides-Extra: lif
@@ -36,19 +36,19 @@
 example:
 
     B009-8L-CtBP2-MyosinVIIa-PMT
 
 Inside each file, the pieces must be numbered sequentially from base (hook) to
 apex. If more htan one image is required for a piece, use letters for the
 suffixes (i.e., "piece2a", "piece2b", etc.). The order in which the images for
-a single piece are labeled does nto matter since the program will automatically
+a single piece are labeled does not matter since the program will automatically
 align them based on the stage coordinates stored in the file.
 
-We currently do not have support for missing pieces. This will be added
-shortly.
+We currently do not have support for missing pieces. This will be added once
+the need arises.
 
 Using the program
 -----------------
 
 Mouse interaction
 .................
 left click
@@ -104,26 +104,24 @@
 the result of the current step before moving to the next step. Although you can
 go back and edit a previous step, it may affect your analysis (e.g., if you
 need to move a tile after marking hair cells, you may have to manually edit
 a large number of hair cells).
 
 **Tile mode**
 
-Start by selecting "tiles" from the edit buttons, then left-clicking to select the tile that is
-misaligned. Using the arrow keys, you can move the tile until it is properly
-aligned with the other tiles. If you need to move the tile in smaller steps,
-hold down the shift key at the same time as the arrow keys. It may be helpful
-to toggle "highlight selected" so that you get a transparent overlay. When in
-"highlight selected" mode, the currently selected tile will be shown with a red
-border.
+Start by selecting "tiles" from the edit buttons, then left-clicking to select
+the tile that is misaligned. Using the arrow keys, you can move the tile until
+it is properly aligned with the other tiles. If you need to move the tile in
+smaller steps, hold down the shift key at the same time as the arrow keys. It
+may be helpful to toggle "highlight selected" so that you get a transparent
+overlay. When in "highlight selected" mode, the currently selected tile will be
+shown with a red border.
 
 left click
     Select tile
-left click + drag
-    Pan image
 mouse wheel
     Zoom in/out
 arrow keys
     Move currently selected tile (large steps)
 shift + arrow keys
     Move currently selected tile (small steps)
 n
@@ -151,15 +149,15 @@
 the nuclei (IHCs) or cuticular plate (OHCs) as that will facilitate the
 semi-automated algorithms implemented by the program to help mark hair cells.
 
 right click
     Add point
 shift + right click
     Remove point
-contrl + right click
+control + right click
     Set point as origin for spiral
 
 **Cell mode**
 
 After marking the spiral, run the algorithm to automatically detect cells. You
 can play with the settings (each time you run, it will delete the existing
 cells and create new ones). You will likely have to manually edit the
@@ -168,33 +166,33 @@
 
 right click
     Add cell
 shift + right click
     Remove cell
 
 From time to time there will be a fourth row of OHCs. These should manually be
-identified by selecting "extra" from the edit mode and then selecting the cell
-tool. Since the fourth row tends to be very short in length, you cannot mark
-a spiral or mark the region as excluded.
+identified by selecting "extra" for the cell you would like to edit and then
+adding the cells using the cell tool.  Since the fourth row tends to be very
+short in length, you cannot mark a spiral or mark the region as excluded.
 
 **Exclude mode**
 
 Finally, go back through each row of hair cells. If there was a region you felt
 you could not intepret properly, select the exclude tool. Right-click the
 spiral at one end of the region then right-click again at the other end of the
 region you wish to exclude.
 
 right click
     Start region. Click again to end region.
-alt + rigth click
-    Remove region.
+shift + right click
+    Remove region under mouse cursor.
 escape
     Cancel current region.
 
 Some additional tools are made available to facilitate this process:
 
-* You can copy a set of excluded regions to any other spiral.
 * You can merge all excluded regions across the OHC spirals into a single set
-  of excluded regions that apply to all OHC spirals.</li>
+  of excluded regions that apply to all OHC spirals (`Combine OHC exclusions`
+  button).
 * You can simplify a set of excluded regions for a particular spiral if they
   are overlapping (this will combine overlapping exclusion regions into
-  a single exclusion region).
+  a single exclusion region) using the `Simplify exclusions` button.
```

### Comparing `cochleogram-0.3.1/cochleogram.egg-info/SOURCES.txt` & `cochleogram-0.3.2/cochleogram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/pyproject.toml` & `cochleogram-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cochleogram-0.3.1/readme.rst` & `cochleogram-0.3.2/readme.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 example:
 
     B009-8L-CtBP2-MyosinVIIa-PMT
 
 Inside each file, the pieces must be numbered sequentially from base (hook) to
 apex. If more htan one image is required for a piece, use letters for the
 suffixes (i.e., "piece2a", "piece2b", etc.). The order in which the images for
-a single piece are labeled does nto matter since the program will automatically
+a single piece are labeled does not matter since the program will automatically
 align them based on the stage coordinates stored in the file.
 
-We currently do not have support for missing pieces. This will be added
-shortly.
+We currently do not have support for missing pieces. This will be added once
+the need arises.
 
 Using the program
 -----------------
 
 Mouse interaction
 .................
 left click
@@ -92,26 +92,24 @@
 the result of the current step before moving to the next step. Although you can
 go back and edit a previous step, it may affect your analysis (e.g., if you
 need to move a tile after marking hair cells, you may have to manually edit
 a large number of hair cells).
 
 **Tile mode**
 
-Start by selecting "tiles" from the edit buttons, then left-clicking to select the tile that is
-misaligned. Using the arrow keys, you can move the tile until it is properly
-aligned with the other tiles. If you need to move the tile in smaller steps,
-hold down the shift key at the same time as the arrow keys. It may be helpful
-to toggle "highlight selected" so that you get a transparent overlay. When in
-"highlight selected" mode, the currently selected tile will be shown with a red
-border.
+Start by selecting "tiles" from the edit buttons, then left-clicking to select
+the tile that is misaligned. Using the arrow keys, you can move the tile until
+it is properly aligned with the other tiles. If you need to move the tile in
+smaller steps, hold down the shift key at the same time as the arrow keys. It
+may be helpful to toggle "highlight selected" so that you get a transparent
+overlay. When in "highlight selected" mode, the currently selected tile will be
+shown with a red border.
 
 left click
     Select tile
-left click + drag
-    Pan image
 mouse wheel
     Zoom in/out
 arrow keys
     Move currently selected tile (large steps)
 shift + arrow keys
     Move currently selected tile (small steps)
 n
@@ -139,15 +137,15 @@
 the nuclei (IHCs) or cuticular plate (OHCs) as that will facilitate the
 semi-automated algorithms implemented by the program to help mark hair cells.
 
 right click
     Add point
 shift + right click
     Remove point
-contrl + right click
+control + right click
     Set point as origin for spiral
 
 **Cell mode**
 
 After marking the spiral, run the algorithm to automatically detect cells. You
 can play with the settings (each time you run, it will delete the existing
 cells and create new ones). You will likely have to manually edit the
@@ -156,33 +154,33 @@
 
 right click
     Add cell
 shift + right click
     Remove cell
 
 From time to time there will be a fourth row of OHCs. These should manually be
-identified by selecting "extra" from the edit mode and then selecting the cell
-tool. Since the fourth row tends to be very short in length, you cannot mark
-a spiral or mark the region as excluded.
+identified by selecting "extra" for the cell you would like to edit and then
+adding the cells using the cell tool.  Since the fourth row tends to be very
+short in length, you cannot mark a spiral or mark the region as excluded.
 
 **Exclude mode**
 
 Finally, go back through each row of hair cells. If there was a region you felt
 you could not intepret properly, select the exclude tool. Right-click the
 spiral at one end of the region then right-click again at the other end of the
 region you wish to exclude.
 
 right click
     Start region. Click again to end region.
-alt + rigth click
-    Remove region.
+shift + right click
+    Remove region under mouse cursor.
 escape
     Cancel current region.
 
 Some additional tools are made available to facilitate this process:
 
-* You can copy a set of excluded regions to any other spiral.
 * You can merge all excluded regions across the OHC spirals into a single set
-  of excluded regions that apply to all OHC spirals.</li>
+  of excluded regions that apply to all OHC spirals (`Combine OHC exclusions`
+  button).
 * You can simplify a set of excluded regions for a particular spiral if they
   are overlapping (this will combine overlapping exclusion regions into
-  a single exclusion region).
+  a single exclusion region) using the `Simplify exclusions` button.
```

