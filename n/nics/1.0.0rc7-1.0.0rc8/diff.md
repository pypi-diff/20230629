# Comparing `tmp/nics-1.0.0rc7.tar.gz` & `tmp/nics-1.0.0rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-42p7h2em/nics-1.0.0rc7.tar", last modified: Thu Jun 29 15:37:27 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-asyza3eh/nics-1.0.0rc8.tar", last modified: Thu Jun 29 21:06:05 2023, max compression
```

## Comparing `nics-1.0.0rc7.tar` & `nics-1.0.0rc8.tar`

### file list

```diff
@@ -1,59 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 15:37:10.000000 nics-1.0.0rc7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 15:37:10.000000 nics-1.0.0rc7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 15:37:27.000000 nics-1.0.0rc7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 15:37:10.000000 nics-1.0.0rc7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/404.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/assets/nics-logo500.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/2 -- Bar -- bar/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/rewrite_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/rewrite_the_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/compile/rewrite_the_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-29 15:37:10.000000 nics-1.0.0rc7/nics/wizard/workflows_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 15:37:27.000000 nics-1.0.0rc7/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-29 15:37:10.000000 nics-1.0.0rc7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 15:37:27.000000 nics-1.0.0rc7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 15:37:10.000000 nics-1.0.0rc7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 21:05:48.000000 nics-1.0.0rc8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 21:05:48.000000 nics-1.0.0rc8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:06:05.000000 nics-1.0.0rc8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 21:05:48.000000 nics-1.0.0rc8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_404_and_favicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_docs_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/compile/update_sass_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics/main/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-29 21:05:48.000000 nics-1.0.0rc8/nics/main/wizard/workflows_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 21:06:05.000000 nics-1.0.0rc8/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-29 21:05:48.000000 nics-1.0.0rc8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 21:06:05.000000 nics-1.0.0rc8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 21:05:48.000000 nics-1.0.0rc8/setup.py
```

### Comparing `nics-1.0.0rc7/LICENSE` & `nics-1.0.0rc8/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc7/PKG-INFO` & `nics-1.0.0rc8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc7/nics/compile/copying_template.py` & `nics-1.0.0rc8/nics/main/compile/copying_template.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import os
 import shutil
 
+from mykit.kit.utils import printer
+
 from ..constants import TEMPLATE_DIR_PTH
 
 
 def copying_template(dock):
 
+    LAYOUTS = os.path.join(dock, '_layouts')
+    SASS = os.path.join(dock, '_sass')
+    SCRIPTS = os.path.join(dock, 'scripts')
 
     ## handle the case when the template already exists
-    if os.path.isdir( os.path.join(dock, '_layouts') ):
-        shutil.rmtree( os.path.join(dock, '_layouts') )
-    if os.path.isdir( os.path.join(dock, '_sass') ):
-        shutil.rmtree( os.path.join(dock, '_sass') )
-    if os.path.isdir( os.path.join(dock, 'scripts') ):
-        shutil.rmtree( os.path.join(dock, 'scripts') )
-
+    if os.path.isdir(LAYOUTS): shutil.rmtree(LAYOUTS)
+    if os.path.isdir(SASS): shutil.rmtree(SASS)
+    if os.path.isdir(SCRIPTS): shutil.rmtree(SCRIPTS)
 
     shutil.copytree(
         os.path.join(TEMPLATE_DIR_PTH, 'web', '_layouts'),
-        os.path.join(dock, '_layouts')
+        LAYOUTS
     )
-
     shutil.copytree(
         os.path.join(TEMPLATE_DIR_PTH, 'web', '_sass'),
-        os.path.join(dock, '_sass')
+        SASS
     )
-
     shutil.copytree(
         os.path.join(TEMPLATE_DIR_PTH, 'web', 'scripts'),
-        os.path.join(dock, 'scripts')
-    )
+        SCRIPTS
+    )
+    printer(f'INFO: Template copied.')
```

### Comparing `nics-1.0.0rc7/nics/compile/inspect.py` & `nics-1.0.0rc8/nics/main/compile/inspect.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,41 @@
 import os
 import re
 
-from typing import Union, NoReturn
 
+def _inspect_tree_recursively(pth):
 
-AbsPath = Union[str, os.PathLike]
-
-
-def _check_format(name):
-    res = re.match(r'(?:\d+ -- )?(?P<name>[\w -.]+) -- (?P<url>[\w -]+)(?:.md)?', name)
-    if res is None:
-        raise
-
-def _inspect_tree_recursively(pth: AbsPath):
-    
-    for i in os.listdir(pth):
-        
-        subpth = os.path.join(pth, i)
-
-        if os.path.isdir(subpth):
+    for i in os.listdir(pth):        
+        pth2 = os.path.join(pth, i)
 
+        if os.path.isdir(pth2):
             ## check dir name format
-            res = re.match(r'(?:\d+ -- )?(?P<name>[\w -.]+) -- (?P<url>[\w -]+)', i)
-            if res is None:
+            if re.match(r'(?:\d+ -- )?[\w -.]+ -- [\w -]+', i) is None:
                 raise AssertionError(f'Dir name {repr(i)} format is invalid.')
-
-            _inspect_tree_recursively(subpth)
+            ## inspect the dir
+            _inspect_tree_recursively(pth2)
         else:
-            
             ## only .md files are allowed
             if not i.endswith('.md'):
                 raise AssertionError(f"File {repr(i)} isn't an .md file.")
-
             ## check file name format
             if i != 'index.md':
-                res = re.match(r'(?:\d+ -- )?(?P<name>[\w -.]+) -- (?P<url>[\w -]+)(?:.md)?', i)
-                if res is None:
+                if re.match(r'(?:\d+ -- )?[\w -.]+ -- [\w -]+\.md$', i) is None:
                     raise AssertionError(f'File name {repr(i)} format is invalid.')
 
-def inspect_the_container(container: AbsPath) -> Union[None, NoReturn]:
-    """
-    These items are needed inside the container:
-    - tree/
-    - tree/index.md
-    - settings.txt
-    """
 
-    ## tree/ folder
+def inspect_the_container(container):
+
+    ## 'tree/' folder
     if not os.path.isdir( os.path.join(container, 'tree') ):
         raise AssertionError("Couldn't find 'tree/' in the container.")
 
-    ## homepage
+    ## homepage 'tree/index.md' file
     if not os.path.isfile( os.path.join(container, 'tree', 'index.md') ):
         raise AssertionError("Couldn't find 'tree/index.md' in the container.")
 
     ## settings file
     if not os.path.isfile( os.path.join(container, 'settings.txt') ):
         raise AssertionError("Couldn't find 'settings.txt' in the container.")
 
-    ## inspecting the tree/
-    _inspect_tree_recursively( os.path.join(container, 'tree') )
-
-
-def inspect_the_dock(dock):
-    """shallow inspection to ensure that we are on the correct branch"""
-
-    # if not os.path.isdir( os.path.join(dock, '_includes') ):
-    #     raise AssertionError("Folder '_includes' ")
+    ## inspecting the 'tree/' folder
+    _inspect_tree_recursively( os.path.join(container, 'tree') )
```

### Comparing `nics-1.0.0rc7/nics/wizard/__init__.py` & `nics-1.0.0rc8/nics/main/wizard/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,65 +1,77 @@
 import os
 import shutil
-import sys
 
 from mykit.kit.utils import printer, print_screen
 
-from ..constants import TEMPLATE_DIR_PTH
+from ..constants import TMPL_DOCS_DIR_PTH
+from .inspect import inspect
 from .workflows_writer import workflows_writer
 from .settings_writer import settings_writer
 
 
-def inspect(docs, workflows):
-    
-    ## docs/
-    if os.path.isdir(docs):
-        printer(f"ERROR: 'docs/' folder already exists.")
-        sys.exit(1)
-    
-    ## workflows
-    if os.path.isfile(workflows):
-        printer(f"ERROR: 'rebuild-docs.yml' file already exists.")
-        sys.exit(1)
-
-
 def run():
 
     CWD = os.getcwd()
 
-    WORKFLOWS = os.path.join(CWD, '.github', 'workflows', 'rebuild-docs.yml')
-    DOCS = os.path.join(CWD, 'docs')
-    SETTINGS = os.path.join(CWD, 'docs', 'settings.txt')
+    WORKFLOW_FILE_PTH = os.path.join(CWD, '.github', 'workflows', 'rebuild-docs.yml')
+    CONTAINER_DIR_PTH = os.path.join(CWD, 'docs')
+    SETTINGS_FILE_PTH = os.path.join(CWD, 'docs', 'settings.txt')
 
-    inspect(DOCS, WORKFLOWS)
+    ## inspection
+    inspect(CONTAINER_DIR_PTH, WORKFLOW_FILE_PTH)
 
+    ## intro
     print_screen(
-        'Welcome to NICS!\n\n'
+        'Welcome to NICS!\n'
+        '================\n\n'
     )
 
+    ## saving user's information
     author = input('Enter your name: ')
     email = input('Enter your email: ')
     gh_username = input('Enter your GitHub username: ')
     gh_repo = input('Enter this GitHub repository name: ')
-    main_branch_name = input("Your main branch name (e.g. 'master'): ")
+    main_branch_name = input("Enter the main branch name (e.g., master): ")
 
-    ## if the dirs don't exist
-    if not os.path.isdir( os.path.join(CWD, '.github') ):
-        os.mkdir( os.path.join(CWD, '.github') )
-        printer(f"INFO: Dir {repr( os.path.join(CWD, '.github') )} is created.")
-    if not os.path.isdir( os.path.join(CWD, '.github', 'workflows') ):
-        os.mkdir( os.path.join(CWD, '.github', 'workflows') )
-        printer(f"INFO: Dir {repr( os.path.join(CWD, '.github', 'workflows') )} is created.")
+    ## handle the case where the '.github/workflows/' directory does not exist yet
+    def handle_workflow_dirs():
+        pth = os.path.join(CWD, '.github')
+        if not os.path.isdir(pth):
+            os.mkdir(pth)
+            printer(f"INFO: Folder {repr(pth)} is created.")
+        pth = os.path.join(CWD, '.github', 'workflows')
+        if not os.path.isdir(pth):
+            os.mkdir(pth)
+            printer(f"INFO: Folder {repr(pth)} is created.")
+    handle_workflow_dirs()
 
-    workflows_writer(WORKFLOWS, author, email, gh_repo, main_branch_name)
+    workflows_writer(WORKFLOW_FILE_PTH, author, email, gh_repo, main_branch_name)
     
     printer(f"INFO: Copying 'docs/' folder.")
-    shutil.copytree( os.path.join(TEMPLATE_DIR_PTH, 'docs'), DOCS )
-    printer(f'INFO: Done, {repr(DOCS)} is created.')
+    shutil.copytree(TMPL_DOCS_DIR_PTH, CONTAINER_DIR_PTH)
+    printer(f'INFO: Done, {repr(CONTAINER_DIR_PTH)} is created.')
 
-    settings_writer(SETTINGS, author, gh_username, gh_repo)
+    settings_writer(SETTINGS_FILE_PTH, author, gh_username, gh_repo)
 
-    print_screen(
-        'Everything is done, now follow these last steps:\n'
-        '1. foo\n'
-        '2. \n'
+    ## outro
+    print_screen(f"""
+Almost done, now you need to do these final steps:
+1. Create docs branch
+   - git commit -am "NICS init"
+   - git checkout --orphan docs
+   - git rm -rf .
+   - git commit --allow-empty -m init
+   - git push origin docs
+2. Activate the GitHub Pages
+   - Visit https://github.com/{gh_username}/{gh_repo}/settings/pages
+   - Under 'Build and deployment' section,
+     - For 'Source', select 'Deploy from a branch'
+     - For 'Branch', select 'docs' branch
+     - Click the 'Save' button
+3. Back to {main_branch_name} branch
+   - git checkout {main_branch_name}
+   - git push
+
+That's it! The documentation will be at https://{gh_username}.github.io/{gh_repo} .
+Visit https://nvfp.github.io/now-i-can-sleep/usage/init-command to visually see the final steps above."""
     )
```

### Comparing `nics-1.0.0rc7/nics/wizard/settings_writer.py` & `nics-1.0.0rc8/nics/main/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc7/nics/wizard/workflows_writer.py` & `nics-1.0.0rc8/nics/main/wizard/workflows_writer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from mykit.kit.utils import printer
 
-from ..constants import __version__
+from ..constants import __version__, SOFTWARE_DIST_NAME, SOFTWARE_REPO
 
 
 def _writer(author, email, gh_repo, main_branch_name):
     return f"""
+
+# This file was generated by {SOFTWARE_DIST_NAME}-v{__version__}.
+# Please make sure to be careful when modifying the values below. For more information, visit: {SOFTWARE_REPO}
+
 name: Rebuild docs
 
 on:
   push:
     branches:
       - {main_branch_name}
 
     paths:
-      - 'docs/**'  # only rebuild docs webpage if docs/ folder is modified
+      - 'docs/**'  # only rebuild if 'docs/' folder is modified
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
 permissions:
   contents: write
 
@@ -61,20 +65,20 @@
           nics _compile "$(pwd)/docs" "$(pwd)/../{gh_repo}"
 
       - name: Deploy
         run: |
           git config user.name "{author} (via NICS)"
           git config user.email "{email}"
           git add .
-          git commit -m "NICS rebuild the docs"
+          git commit -m "NICS rebuilds the docs"
           git push
 """
 
 
 def workflows_writer(pth, author, email, gh_repo, main_branch_name):
-    printer(f'INFO: Writing GitHub workflows.')
+    printer(f'INFO: Writing GitHub workflow file.')
 
     text = _writer(author, email, gh_repo, main_branch_name)
     with open(pth, 'w') as f:
         f.write(text)
 
     printer(f'INFO: Done, {repr(pth)} is created.')
```

### Comparing `nics-1.0.0rc7/nics.egg-info/PKG-INFO` & `nics-1.0.0rc8/nics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc7
+Version: 1.0.0rc8
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc7/pyproject.toml` & `nics-1.0.0rc8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "1.0.0-rc-7"
+version = "1.0.0rc8"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

