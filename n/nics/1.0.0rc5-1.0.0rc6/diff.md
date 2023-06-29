# Comparing `tmp/nics-1.0.0rc5.tar.gz` & `tmp/nics-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-ie569duj/nics-1.0.0rc5.tar", last modified: Thu Jun 29 11:47:34 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-5omaxn_y/nics-1.0.0rc6.tar", last modified: Thu Jun 29 11:58:29 2023, max compression
```

## Comparing `nics-1.0.0rc5.tar` & `nics-1.0.0rc6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 11:47:18.000000 nics-1.0.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 11:47:18.000000 nics-1.0.0rc5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:47:34.000000 nics-1.0.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 11:47:18.000000 nics-1.0.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/404.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/assets/nics-logo500.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_the_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_the_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/workflows_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-29 11:47:18.000000 nics-1.0.0rc5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 11:47:34.000000 nics-1.0.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 11:47:18.000000 nics-1.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 11:58:10.000000 nics-1.0.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 11:58:10.000000 nics-1.0.0rc6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:58:29.000000 nics-1.0.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 11:58:10.000000 nics-1.0.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/404.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/assets/nics-logo500.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/2 -- Bar -- bar/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/rewrite_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/rewrite_the_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/compile/rewrite_the_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-29 11:58:10.000000 nics-1.0.0rc6/nics/wizard/workflows_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:58:29.000000 nics-1.0.0rc6/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-29 11:58:10.000000 nics-1.0.0rc6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 11:58:29.000000 nics-1.0.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 11:58:10.000000 nics-1.0.0rc6/setup.py
```

### Comparing `nics-1.0.0rc5/LICENSE` & `nics-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/PKG-INFO` & `nics-1.0.0rc6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc5/nics/__init__.py` & `nics-1.0.0rc6/nics/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/_template/docs/assets/nics-logo500.jpg` & `nics-1.0.0rc6/nics/_template/docs/assets/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/_template/web/_sass/header.scss` & `nics-1.0.0rc6/nics/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/_template/web/_sass/main.scss` & `nics-1.0.0rc6/nics/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/_template/web/scripts/header.js` & `nics-1.0.0rc6/nics/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/compile/__init__.py` & `nics-1.0.0rc6/nics/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/compile/copying_template.py` & `nics-1.0.0rc6/nics/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/compile/inspect.py` & `nics-1.0.0rc6/nics/compile/inspect.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/compile/rewrite_the_header.py` & `nics-1.0.0rc6/nics/compile/rewrite_the_header.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/constants.py` & `nics-1.0.0rc6/nics/constants.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/nics/wizard/__init__.py` & `nics-1.0.0rc6/nics/wizard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,24 +36,25 @@
         'Welcome to NICS!\n\n'
     )
 
     author = input('Enter your name: ')
     email = input('Enter your email: ')
     gh_username = input('Enter your GitHub username: ')
     gh_repo = input('Enter this GitHub repository name: ')
+    main_branch_name = input("Your main branch name (e.g. 'master'): ")
 
     ## if the dirs don't exist
     if not os.path.isdir( os.path.join(CWD, '.github') ):
         os.mkdir( os.path.join(CWD, '.github') )
         printer(f"INFO: Dir {repr( os.path.join(CWD, '.github') )} is created.")
     if not os.path.isdir( os.path.join(CWD, '.github', 'workflows') ):
         os.mkdir( os.path.join(CWD, '.github', 'workflows') )
         printer(f"INFO: Dir {repr( os.path.join(CWD, '.github', 'workflows') )} is created.")
 
-    workflows_writer(WORKFLOWS, author, email, gh_repo)
+    workflows_writer(WORKFLOWS, author, email, gh_repo, main_branch_name)
     
     printer(f"INFO: Copying 'docs/' folder.")
     shutil.copytree( os.path.join(TEMPLATE_DIR_PTH, 'docs'), DOCS )
     printer(f'INFO: Done, {repr(DOCS)} is created.')
 
     settings_writer(SETTINGS, author, gh_username, gh_repo)
```

### Comparing `nics-1.0.0rc5/nics/wizard/settings_writer.py` & `nics-1.0.0rc6/nics/wizard/settings_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import random
+
 from mykit.kit.utils import printer
 
 
 def _writer(author, gh_username, gh_repo):
     return f"""
 #-- Welcome to NICS settings!
 #----------------------------
 
 #-- Everything starts with "#--" is a comment.
 #-- Read documentation at https://nvfp.github.io/now-i-can-sleep
 
 
 author: '{author}'
-color_hue: 28
+color_hue: {random.randint(0, 359)}
 show_credit: True
 
 
 #-- The below variables are for NICS internal use only and should not be changed.
 
 _gh_username: '{gh_username}'
 _gh_repo: '{gh_repo}'
```

### Comparing `nics-1.0.0rc5/nics/wizard/workflows_writer.py` & `nics-1.0.0rc6/nics/wizard/workflows_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from mykit.kit.utils import printer
 
 from ..constants import __version__
 
 
-def workflows_writer(pth, author, email, gh_repo):
-    printer(f'INFO: Writing GitHub workflows.')
-
-    text = f"""
-
+def _writer(author, email, gh_repo, main_branch_name):
+    return f"""
 name: Rebuild docs
 
 on:
   push:
     branches:
-      - main
+      - {main_branch_name}
 
     paths:
       - 'docs/**'  # only rebuild docs webpage if docs/ folder is modified
 
   # Allows you to run this workflow manually from the Actions tab
   workflow_dispatch:
 
@@ -26,18 +23,18 @@
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
 
-      - name: Checkout main branch
+      - name: Checkout {main_branch_name} branch
         uses: actions/checkout@v3
         with:
-          ref: main
+          ref: {main_branch_name}
 
       - name: Creating NICS working directory
         run: |
           cd ..
           mkdir __nics_work_dir__
           cd __nics_work_dir__
           cp -r ../{gh_repo}/docs/ .
@@ -68,11 +65,16 @@
           git config user.name "{author} (via NICS)"
           git config user.email "{email}"
           git add .
           git commit -m "NICS rebuild the docs"
           git push
 """
 
+
+def workflows_writer(pth, author, email, gh_repo, main_branch_name):
+    printer(f'INFO: Writing GitHub workflows.')
+
+    text = _writer(author, email, gh_repo, main_branch_name)
     with open(pth, 'w') as f:
         f.write(text)
 
     printer(f'INFO: Done, {repr(pth)} is created.')
```

### Comparing `nics-1.0.0rc5/nics.egg-info/PKG-INFO` & `nics-1.0.0rc6/nics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc5/nics.egg-info/SOURCES.txt` & `nics-1.0.0rc6/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc5/pyproject.toml` & `nics-1.0.0rc6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "1.0.0-rc-5"
+version = "1.0.0-rc-6"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

