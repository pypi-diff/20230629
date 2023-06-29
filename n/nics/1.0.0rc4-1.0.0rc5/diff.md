# Comparing `tmp/nics-1.0.0rc4.tar.gz` & `tmp/nics-1.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-7ycybw0i/nics-1.0.0rc4.tar", last modified: Thu Jun 29 11:33:30 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-ie569duj/nics-1.0.0rc5.tar", last modified: Thu Jun 29 11:47:34 2023, max compression
```

## Comparing `nics-1.0.0rc4.tar` & `nics-1.0.0rc5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 11:33:08.000000 nics-1.0.0rc4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 11:33:08.000000 nics-1.0.0rc4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:33:30.000000 nics-1.0.0rc4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 11:33:08.000000 nics-1.0.0rc4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/404.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/assets/nics-logo500.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/tree/2 -- Bar -- bar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/2 -- Bar -- bar/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/4 -- About -- about.md
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/docs/tree/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/web/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/web/_layouts/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/web/_layouts/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/web/_sass/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/web/_sass/footer.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/web/_sass/header.scss
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/web/_sass/main.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/_template/web/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/_template/web/scripts/header.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/copying_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/rewrite_jekyll_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/rewrite_the_footer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/compile/rewrite_the_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/wizard/settings_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 11:33:08.000000 nics-1.0.0rc4/nics/wizard/workflows_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:33:30.000000 nics-1.0.0rc4/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-29 11:33:08.000000 nics-1.0.0rc4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 11:33:30.000000 nics-1.0.0rc4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 11:33:08.000000 nics-1.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 11:47:18.000000 nics-1.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-29 11:47:18.000000 nics-1.0.0rc5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:47:34.000000 nics-1.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-29 11:47:18.000000 nics-1.0.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/404.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/assets/nics-logo500.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/1 -- THIS-IS-TITLE -- THIS-IS-URL.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/Hello -- world.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/Without Numbering -- Without-Numbering.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/2 -- Bar -- bar/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/01 -- Nested -- nested/Without index.md -- without-index-md.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/02 -- bar -- bar.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/3 -- Foo Bar Baz -- foo-bar-baz/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/4 -- About -- about.md
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/5 -- This is a demo -- This-Is-A-Demo.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/docs/tree/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/_layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_layouts/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/_sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/footer.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/header.scss
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/_sass/main.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/_template/web/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/_template/web/scripts/header.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/copying_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_jekyll_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_the_footer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/compile/rewrite_the_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/settings_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-29 11:47:18.000000 nics-1.0.0rc5/nics/wizard/workflows_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 11:47:34.000000 nics-1.0.0rc5/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-29 11:47:18.000000 nics-1.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-29 11:47:34.000000 nics-1.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 11:47:18.000000 nics-1.0.0rc5/setup.py
```

### Comparing `nics-1.0.0rc4/LICENSE` & `nics-1.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/PKG-INFO` & `nics-1.0.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc4/nics/__init__.py` & `nics-1.0.0rc5/nics/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/_template/docs/assets/nics-logo500.jpg` & `nics-1.0.0rc5/nics/_template/docs/assets/nics-logo500.jpg`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/_template/web/_sass/header.scss` & `nics-1.0.0rc5/nics/_template/web/_sass/header.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/_template/web/_sass/main.scss` & `nics-1.0.0rc5/nics/_template/web/_sass/main.scss`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/_template/web/scripts/header.js` & `nics-1.0.0rc5/nics/_template/web/scripts/header.js`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/compile/__init__.py` & `nics-1.0.0rc5/nics/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/compile/copying_template.py` & `nics-1.0.0rc5/nics/compile/copying_template.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/compile/inspect.py` & `nics-1.0.0rc5/nics/compile/inspect.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/compile/rewrite_the_header.py` & `nics-1.0.0rc5/nics/compile/rewrite_the_header.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/constants.py` & `nics-1.0.0rc5/nics/constants.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/wizard/__init__.py` & `nics-1.0.0rc5/nics/wizard/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,24 +25,34 @@
 def run():
 
     CWD = os.getcwd()
 
     WORKFLOWS = os.path.join(CWD, '.github', 'workflows', 'rebuild-docs.yml')
     DOCS = os.path.join(CWD, 'docs')
     SETTINGS = os.path.join(CWD, 'docs', 'settings.txt')
-    
+
     inspect(DOCS, WORKFLOWS)
 
-    print_screen('Welcome to NICS!')
+    print_screen(
+        'Welcome to NICS!\n\n'
+    )
 
     author = input('Enter your name: ')
     email = input('Enter your email: ')
     gh_username = input('Enter your GitHub username: ')
     gh_repo = input('Enter this GitHub repository name: ')
 
+    ## if the dirs don't exist
+    if not os.path.isdir( os.path.join(CWD, '.github') ):
+        os.mkdir( os.path.join(CWD, '.github') )
+        printer(f"INFO: Dir {repr( os.path.join(CWD, '.github') )} is created.")
+    if not os.path.isdir( os.path.join(CWD, '.github', 'workflows') ):
+        os.mkdir( os.path.join(CWD, '.github', 'workflows') )
+        printer(f"INFO: Dir {repr( os.path.join(CWD, '.github', 'workflows') )} is created.")
+
     workflows_writer(WORKFLOWS, author, email, gh_repo)
     
     printer(f"INFO: Copying 'docs/' folder.")
     shutil.copytree( os.path.join(TEMPLATE_DIR_PTH, 'docs'), DOCS )
     printer(f'INFO: Done, {repr(DOCS)} is created.')
 
     settings_writer(SETTINGS, author, gh_username, gh_repo)
```

### Comparing `nics-1.0.0rc4/nics/wizard/settings_writer.py` & `nics-1.0.0rc5/nics/wizard/settings_writer.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics/wizard/workflows_writer.py` & `nics-1.0.0rc5/nics/wizard/workflows_writer.py`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/nics.egg-info/PKG-INFO` & `nics-1.0.0rc5/nics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 1.0.0rc4
+Version: 1.0.0rc5
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-1.0.0rc4/nics.egg-info/SOURCES.txt` & `nics-1.0.0rc5/nics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nics-1.0.0rc4/pyproject.toml` & `nics-1.0.0rc5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "1.0.0-rc-4"
+version = "1.0.0-rc-5"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

