# Comparing `tmp/dymoprint-2.0.0.tar.gz` & `tmp/dymoprint-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dymoprint-2.0.0.tar", last modified: Thu Jun 29 16:56:53 2023, max compression
+gzip compressed data, was "dymoprint-2.0.0b0.tar", last modified: Sun Jun 11 11:49:04 2023, max compression
```

## Comparing `dymoprint-2.0.0.tar` & `dymoprint-2.0.0b0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.426355 dymoprint-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.418355 dymoprint-2.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-29 16:56:37.000000 dymoprint-2.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.418355 dymoprint-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-29 16:56:37.000000 dymoprint-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-29 16:56:37.000000 dymoprint-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-29 16:56:37.000000 dymoprint-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-29 16:56:37.000000 dymoprint-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-29 16:56:37.000000 dymoprint-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-29 16:56:53.426355 dymoprint-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-29 16:56:37.000000 dymoprint-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-29 16:56:37.000000 dymoprint-2.0.0/TODO.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.418355 dymoprint-2.0.0/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.422355 dymoprint-2.0.0/data/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/Carlito-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/Carlito-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/Carlito-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/barcode_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/gui_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/img_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/qr_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-29 16:56:37.000000 dymoprint-2.0.0/data/fonts/txt_icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.426355 dymoprint-2.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-29 16:56:37.000000 dymoprint-2.0.0/doc/DymoPrint_example_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-06-29 16:56:37.000000 dymoprint-2.0.0/doc/DymoPrint_example_2.png
--rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-06-29 16:56:37.000000 dymoprint-2.0.0/doc/DymoPrint_example_3.png
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-29 16:56:37.000000 dymoprint-2.0.0/dymoprint.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-29 16:56:37.000000 dymoprint-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-29 16:56:53.426355 dymoprint-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-29 16:56:37.000000 dymoprint-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.426355 dymoprint-2.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.426355 dymoprint-2.0.0/src/dymoprint/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/barcode_writer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5743 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2217 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/dymo_print_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/font_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/gui.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/q_dymo_label_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/q_dymo_labels_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/unicode_blocks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-29 16:56:37.000000 dymoprint-2.0.0/src/dymoprint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:56:53.426355 dymoprint-2.0.0/src/dymoprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-29 16:56:53.000000 dymoprint-2.0.0/src/dymoprint.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      536 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/TODO.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.989323 dymoprint-2.0.0b0/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/data/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   690516 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   816716 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   623416 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   635996 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4247 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/barcode_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/gui_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/img_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/qr_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/data/fonts/txt_icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    34893 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40573 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37194 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/doc/DymoPrint_example_3.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/dymoprint.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.993323 dymoprint-2.0.0b0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/src/dymoprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3811 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/barcode_writer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5743 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2217 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17404 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/dymo_print_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/font_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/gui.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7608 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11420 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/q_dymo_label_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/q_dymo_labels_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/unicode_blocks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      897 2023-06-11 11:48:49.000000 dymoprint-2.0.0b0/src/dymoprint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 11:49:03.997323 dymoprint-2.0.0b0/src/dymoprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-11 11:49:03.000000 dymoprint-2.0.0b0/src/dymoprint.egg-info/top_level.txt
```

### Comparing `dymoprint-2.0.0/.github/workflows/pypi-publish.yml` & `dymoprint-2.0.0b0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/.github/workflows/tests.yml` & `dymoprint-2.0.0b0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/.gitignore` & `dymoprint-2.0.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/.pre-commit-config.yaml` & `dymoprint-2.0.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/LICENSE` & `dymoprint-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/PKG-INFO` & `dymoprint-2.0.0b0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 2.0.0
+Version: 2.0.0b0
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
@@ -29,29 +29,25 @@
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Text printing
-* QR code printing
-* Barcode printing
-* Image printing
-* Combinations of the above
-* GUI Application based on PyQt6
-
-### Experimental
-
-* LabelManager 280
-* LabelManager 420P
-* LabelManager Wireless PnP
-* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
+* Works on python 3.7 and up
+* Supports text printing
+* Supports qr code printing
+* Supports barcode printing
+* Supports image printing
+* Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
-For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -65,28 +61,15 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-By default, users don't have permission to access generic USB devices, so you will
-need to add a rule. The first time you run `dymoprint`, it will give instructions
-about how to do this:
-
-```bash
-$ dymoprint "Hello world"
-...
-You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
-
-  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
-...
-```
-
-## Testing experimental features
+## Experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -109,14 +92,77 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
+## Configuration
+
+### For ubuntu based distributions
+
+Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo systemctl restart udev.service
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
+### For arch based distributions
+
+(should also work for manjaro, but not tested yet)
+use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+Install **usb_modeswitch** at first:
+
+```bash
+sudo pacman -S usb_modeswitch
+```
+
+if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
+
+```bash
+sudo mkdir /etc/usb_modeswitch.d/
+````
+
+now copy the udev and usb_modswitch configs:
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo udevadm control --reload
+```
+
+you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
+
+```bash
+sudo chown your_user:users /dev/hidraw0
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -219,21 +265,18 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
+* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
-* refactor code with better abstractions
-* pixel fonts
-* web interface
```

### Comparing `dymoprint-2.0.0/README.md` & `dymoprint-2.0.0b0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,29 +7,25 @@
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Text printing
-* QR code printing
-* Barcode printing
-* Image printing
-* Combinations of the above
-* GUI Application based on PyQt6
-
-### Experimental
-
-* LabelManager 280
-* LabelManager 420P
-* LabelManager Wireless PnP
-* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
+* Works on python 3.7 and up
+* Supports text printing
+* Supports qr code printing
+* Supports barcode printing
+* Supports image printing
+* Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
-For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -43,28 +39,15 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-By default, users don't have permission to access generic USB devices, so you will
-need to add a rule. The first time you run `dymoprint`, it will give instructions
-about how to do this:
-
-```bash
-$ dymoprint "Hello world"
-...
-You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
-
-  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
-...
-```
-
-## Testing experimental features
+## Experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -87,14 +70,77 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
+## Configuration
+
+### For ubuntu based distributions
+
+Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo systemctl restart udev.service
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
+### For arch based distributions
+
+(should also work for manjaro, but not tested yet)
+use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+Install **usb_modeswitch** at first:
+
+```bash
+sudo pacman -S usb_modeswitch
+```
+
+if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
+
+```bash
+sudo mkdir /etc/usb_modeswitch.d/
+````
+
+now copy the udev and usb_modswitch configs:
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo udevadm control --reload
+```
+
+you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
+
+```bash
+sudo chown your_user:users /dev/hidraw0
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -197,21 +243,18 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
+* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
-* refactor code with better abstractions
-* pixel fonts
-* web interface
```

### Comparing `dymoprint-2.0.0/TODO.md` & `dymoprint-2.0.0b0/TODO.md`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/Carlito-Bold.ttf` & `dymoprint-2.0.0b0/data/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/Carlito-BoldItalic.ttf` & `dymoprint-2.0.0b0/data/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/Carlito-Italic.ttf` & `dymoprint-2.0.0b0/data/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/Carlito-Regular.ttf` & `dymoprint-2.0.0b0/data/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/LICENSE` & `dymoprint-2.0.0b0/data/fonts/LICENSE`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/barcode_icon.png` & `dymoprint-2.0.0b0/data/fonts/barcode_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/gui_icon.png` & `dymoprint-2.0.0b0/data/fonts/gui_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/img_icon.png` & `dymoprint-2.0.0b0/data/fonts/img_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/data/fonts/txt_icon.png` & `dymoprint-2.0.0b0/data/fonts/txt_icon.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/doc/DymoPrint_example_1.png` & `dymoprint-2.0.0b0/doc/DymoPrint_example_1.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/doc/DymoPrint_example_2.png` & `dymoprint-2.0.0b0/doc/DymoPrint_example_2.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/doc/DymoPrint_example_3.png` & `dymoprint-2.0.0b0/doc/DymoPrint_example_3.png`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/pyproject.toml` & `dymoprint-2.0.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/setup.cfg` & `dymoprint-2.0.0b0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/setup.py` & `dymoprint-2.0.0b0/setup.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/README.md` & `dymoprint-2.0.0b0/src/README.md`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/barcode_writer.py` & `dymoprint-2.0.0b0/src/dymoprint/barcode_writer.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/command_line.py` & `dymoprint-2.0.0b0/src/dymoprint/command_line.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/constants.py` & `dymoprint-2.0.0b0/src/dymoprint/constants.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/dymo_print_engines.py` & `dymoprint-2.0.0b0/src/dymoprint/dymo_print_engines.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,17 @@
     lines.append("")
     udev_rule = ", ".join(
         [
             'ACTION=="add"',
             'SUBSYSTEMS=="usb"',
             f'ATTRS{{idVendor}}=="{dev.idVendor:04x}"',
             f'ATTRS{{idProduct}}=="{dev.idProduct:04x}"',
-            'MODE="0666"',
+            'MODE="0660"',
+            'GROUP="plugdev"',
+            'TAG+="uaccess"',
         ]
     )
     lines.append(
         f"  echo '{udev_rule}' "
         f"| sudo tee /etc/udev/rules.d/91-dymo-{dev.idProduct:x}.rules"
     )
     lines.append("")
```

### Comparing `dymoprint-2.0.0/src/dymoprint/font_config.py` & `dymoprint-2.0.0b0/src/dymoprint/font_config.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/gui.py` & `dymoprint-2.0.0b0/src/dymoprint/gui.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/labeler.py` & `dymoprint-2.0.0b0/src/dymoprint/labeler.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/q_dymo_label_widgets.py` & `dymoprint-2.0.0b0/src/dymoprint/q_dymo_label_widgets.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/q_dymo_labels_list.py` & `dymoprint-2.0.0b0/src/dymoprint/q_dymo_labels_list.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/unicode_blocks.py` & `dymoprint-2.0.0b0/src/dymoprint/unicode_blocks.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint/utils.py` & `dymoprint-2.0.0b0/src/dymoprint/utils.py`

 * *Files identical despite different names*

### Comparing `dymoprint-2.0.0/src/dymoprint.egg-info/PKG-INFO` & `dymoprint-2.0.0b0/src/dymoprint.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dymoprint
-Version: 2.0.0
+Version: 2.0.0b0
 Summary: Linux Software to print with LabelManager PnP from Dymo
 Home-page: https://github.com/computerlyrik/dymoprint
 Author: Sebastian J. Bronner
 Author-email: waschtl@sbronner.com
 Maintainer: Ben Mares
 Maintainer-email: services-dymoprint@tensorial.com
 License: Apache License 2.0
@@ -29,29 +29,25 @@
 
 * First version from Sebastian Bronner: <https://sbronner.com/dymoprint.html>
 * Cloned to Github and formerly maintained by @computerlyrik: <https://github.com/computerlyrik/dymoprint>
 * Currently maintained by @maresb
 
 ## Features
 
-* Text printing
-* QR code printing
-* Barcode printing
-* Image printing
-* Combinations of the above
-* GUI Application based on PyQt6
-
-### Experimental
-
-* LabelManager 280
-* LabelManager 420P
-* LabelManager Wireless PnP
-* Windows support by setting the driver to WinUSB using [Zadig](https://zadig.akeo.ie/)
+* Works on python 3.7 and up
+* Supports text printing
+* Supports qr code printing
+* Supports barcode printing
+* Supports image printing
+* Supports combined barcode / qrcode and text printing
+* GUI Application based on PyQt6 - expanded combinations
 
-For more information about experimental device support, see [#44](https://github.com/computerlyrik/dymoprint/issues/44).
+## HELP WANTED
+
+Test the latest [experimental version](https://github.com/computerlyrik/dymoprint/pull/56) and report back if it works for you.
 
 ## Installation
 
 It is recommended to install dymoprint with [pipx](https://pypa.github.io/pipx/) so that it runs in an isolated virtual environment:
 
 ```bash
 pipx install dymoprint
@@ -65,28 +61,15 @@
 
 or on Arch with
 
 ```bash
 sudo pacman -S python-pipx
 ```
 
-By default, users don't have permission to access generic USB devices, so you will
-need to add a rule. The first time you run `dymoprint`, it will give instructions
-about how to do this:
-
-```bash
-$ dymoprint "Hello world"
-...
-You do not have sufficient access to the device. You probably want to add the a udev rule in /etc/udev/rules.d with the following command:
-
-  echo 'ACTION=="add", SUBSYSTEMS=="usb", ATTRS{idVendor}=="0922", ATTRS{idProduct}=="1001", MODE="0666"' | sudo tee /etc/udev/rules.d/91-dymo-1001.rules
-...
-```
-
-## Testing experimental features
+## Experimental features
 
 To install a test branch, by user `ghuser` for the branch `branchname`, run
 
 ```bash
 pipx install --force git+https://github.com/ghuser/dymoprint@branchname
 ```
 
@@ -109,14 +92,77 @@
 This project uses [pre-commit](https://pre-commit.com/) to run some checks before committing.
 After installing the `pre-commit` executable, please run
 
 ```bash
 pre-commit install
 ```
 
+## Configuration
+
+### For ubuntu based distributions
+
+Use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo systemctl restart udev.service
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
+### For arch based distributions
+
+(should also work for manjaro, but not tested yet)
+use **udev** and **modeswitch** configurations to work with the LabelManager PNP.
+**modeswitch** changes the mode (and USB Id) from mass storage device to printer device.
+
+Install **usb_modeswitch** at first:
+
+```bash
+sudo pacman -S usb_modeswitch
+```
+
+if the **/etc/usb_modeswitch.d/** folder was not created at installation do:
+
+```bash
+sudo mkdir /etc/usb_modeswitch.d/
+````
+
+now copy the udev and usb_modswitch configs:
+
+```bash
+sudo cp 91-dymo-labelmanager-pnp.rules /etc/udev/rules.d/
+sudo cp dymo-labelmanager-pnp.conf /etc/usb_modeswitch.d/
+```
+
+and restart services with:
+
+```bash
+sudo udevadm control --reload
+```
+
+you might need to change the permissions of the hid device (dymoprint will tell if it is the case):
+
+```bash
+sudo chown your_user:users /dev/hidraw0
+```
+
+Finally, physically disconnect and reconnect the LabelManager PnP.
+
+([more info](http://www.draisberghof.de/usb_modeswitch/bb/viewtopic.php?t=947))
+
 ## Font management
 
 Fonts are managed via [dymoprint.ini](dymoprint.ini). This should be placed in your
 config folder (normally `~/.config`). An example file is provided here.
 
 You may choose any TTF Font you like
 
@@ -219,21 +265,18 @@
 dymoprint -c code128 Tst && \
 dymoprint -qr qrencoded "qr_txt" && \
 dymoprint -c code128 Test "bc_txt"
 ```
 
 ### ToDo
 
-* ~~(?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?~~
+* (?)support multiple ProductIDs (1001, 1002) -> use usb-modeswitch?
 * ~~put everything in classes that would need to be used by a GUI~~
 * ~~for more options use command line parser framework~~
 * ~~allow selection of font with command line options~~
 * ~~allow font size specification with command line option (points, pixels?)~~
 * ~~provide an option to show a preview of what the label will look like~~
 * ~~read and write a .dymoprint file containing user preferences~~
 * ~~print barcodes~~
 * ~~print graphics~~
 * ~~plot frame around label~~
 * vertical print
-* refactor code with better abstractions
-* pixel fonts
-* web interface
```

### Comparing `dymoprint-2.0.0/src/dymoprint.egg-info/SOURCES.txt` & `dymoprint-2.0.0b0/src/dymoprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

