# Comparing `tmp/numpydoc-1.5.0rc1.tar.gz` & `tmp/numpydoc-1.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numpydoc-1.5.0rc1.tar", last modified: Tue Oct  4 21:50:12 2022, max compression
+gzip compressed data, was "numpydoc-1.6.0rc0.tar", last modified: Thu Jun 29 21:35:01 2023, max compression
```

## Comparing `numpydoc-1.5.0rc1.tar` & `numpydoc-1.6.0rc0.tar`

### file list

```diff
@@ -1,52 +1,62 @@
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.672233 numpydoc-1.5.0rc1/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1298 2022-03-29 22:37:32.000000 numpydoc-1.5.0rc1/LICENSE.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      306 2022-04-30 19:35:11.000000 numpydoc-1.5.0rc1/MANIFEST.in
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2055 2022-10-04 21:50:12.672233 numpydoc-1.5.0rc1/PKG-INFO
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1217 2022-08-09 17:09:18.000000 numpydoc-1.5.0rc1/README.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1497 2022-04-30 19:35:11.000000 numpydoc-1.5.0rc1/RELEASE.rst
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.668233 numpydoc-1.5.0rc1/doc/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     7213 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/doc/Makefile
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     4974 2022-09-27 23:40:39.000000 numpydoc-1.5.0rc1/doc/conf.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     4109 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/doc/example.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      251 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/doc/example.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    24124 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/doc/format.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      790 2022-10-04 21:34:41.000000 numpydoc-1.5.0rc1/doc/index.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     6199 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/doc/install.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     6721 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/doc/make.bat
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    17450 2022-10-04 21:47:22.000000 numpydoc-1.5.0rc1/doc/release_notes.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2381 2022-07-26 22:15:00.000000 numpydoc-1.5.0rc1/doc/validation.rst
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.669233 numpydoc-1.5.0rc1/numpydoc/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      280 2022-08-09 17:09:18.000000 numpydoc-1.5.0rc1/numpydoc/__init__.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     1550 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/__main__.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       25 2022-10-04 21:48:04.000000 numpydoc-1.5.0rc1/numpydoc/_version.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    23532 2022-10-04 16:45:48.000000 numpydoc-1.5.0rc1/numpydoc/docscrape.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    15586 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/numpydoc/docscrape_sphinx.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    17059 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/numpydoc/numpydoc.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.670233 numpydoc-1.5.0rc1/numpydoc/templates/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      227 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/numpydoc/templates/numpydoc_docstring.rst
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.671233 numpydoc-1.5.0rc1/numpydoc/tests/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    36934 2022-10-04 16:45:48.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_docscrape.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     3761 2022-07-12 21:53:18.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_full.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2828 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_main.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     7652 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_numpydoc.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    36216 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_validate.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     6285 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/tests/test_xref.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.672233 numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      249 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/Makefile
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      670 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/conf.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      146 2022-01-08 02:57:34.000000 numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/index.rst
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      925 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/numpydoc_test_module.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)    21336 2022-09-27 22:28:20.000000 numpydoc-1.5.0rc1/numpydoc/validate.py
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     6541 2022-05-27 20:38:55.000000 numpydoc-1.5.0rc1/numpydoc/xref.py
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.670233 numpydoc-1.5.0rc1/numpydoc.egg-info/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2055 2022-10-04 21:50:12.000000 numpydoc-1.5.0rc1/numpydoc.egg-info/PKG-INFO
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      996 2022-10-04 21:50:12.000000 numpydoc-1.5.0rc1/numpydoc.egg-info/SOURCES.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)        1 2022-10-04 21:50:12.000000 numpydoc-1.5.0rc1/numpydoc.egg-info/dependency_links.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       65 2022-10-04 21:50:12.000000 numpydoc-1.5.0rc1/numpydoc.egg-info/requires.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)        9 2022-10-04 21:50:12.000000 numpydoc-1.5.0rc1/numpydoc.egg-info/top_level.txt
-drwxrwxr-x   0 jarrod   (10000) jarrod   (10000)        0 2022-10-04 21:50:12.672233 numpydoc-1.5.0rc1/requirements/
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       17 2022-07-26 22:15:00.000000 numpydoc-1.5.0rc1/requirements/developer.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       55 2022-10-04 21:34:41.000000 numpydoc-1.5.0rc1/requirements/doc.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)       29 2022-04-09 15:59:53.000000 numpydoc-1.5.0rc1/requirements/test.txt
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)      196 2022-10-04 21:50:12.673233 numpydoc-1.5.0rc1/setup.cfg
--rw-rw-r--   0 jarrod   (10000) jarrod   (10000)     2221 2022-10-04 21:41:44.000000 numpydoc-1.5.0rc1/setup.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1298 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/LICENSE.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      306 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/MANIFEST.in
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2003 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1215 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/README.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1500 2023-06-29 21:33:27.000000 numpydoc-1.6.0rc0/RELEASE.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.449235 numpydoc-1.6.0rc0/doc/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7213 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/Makefile
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4585 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/conf.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     4109 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/example.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      251 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/example.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    24124 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/format.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      790 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/index.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6197 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/doc/install.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6721 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/doc/make.bat
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21266 2023-06-29 21:26:11.000000 numpydoc-1.6.0rc0/doc/release_notes.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     5173 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/doc/validation.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.452235 numpydoc-1.6.0rc0/numpydoc/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      280 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1550 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/__main__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       25 2023-06-29 21:26:38.000000 numpydoc-1.6.0rc0/numpydoc/_version.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    23449 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/numpydoc/docscrape.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    15214 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/docscrape_sphinx.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.454235 numpydoc-1.6.0rc0/numpydoc/hooks/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       39 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1393 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/utils.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    13601 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/hooks/validate_docstrings.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    17055 2023-06-08 22:44:13.000000 numpydoc-1.6.0rc0/numpydoc/numpydoc.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.455235 numpydoc-1.6.0rc0/numpydoc/templates/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      227 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/templates/numpydoc_docstring.rst
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.457235 numpydoc-1.6.0rc0/numpydoc/tests/
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.458235 numpydoc-1.6.0rc0/numpydoc/tests/hooks/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       23 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/__init__.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      497 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/example_module.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1027 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_utils.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    14473 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/tests/hooks/test_validate_hook.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    36826 2023-06-09 04:29:05.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_docscrape.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     3761 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_full.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2828 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_main.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     7652 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_numpydoc.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    37154 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_validate.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6285 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/test_xref.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.459235 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      249 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/Makefile
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      670 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/conf.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      146 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/index.rst
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      925 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/numpydoc_test_module.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)    21812 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/numpydoc/validate.py
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     6541 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/numpydoc/xref.py
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.453235 numpydoc-1.6.0rc0/numpydoc.egg-info/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2003 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/PKG-INFO
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     1270 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/SOURCES.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        1 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/dependency_links.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       80 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/entry_points.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      121 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/requires.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)        9 2023-06-29 21:35:01.000000 numpydoc-1.6.0rc0/numpydoc.egg-info/top_level.txt
+drwxr-xr-x   0 jarrod   (10000) jarrod   (10000)        0 2023-06-29 21:35:01.460235 numpydoc-1.6.0rc0/requirements/
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       16 2023-06-27 17:09:18.000000 numpydoc-1.6.0rc0/requirements/developer.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       64 2023-06-27 17:49:05.000000 numpydoc-1.6.0rc0/requirements/doc.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)       29 2023-06-08 19:37:36.000000 numpydoc-1.6.0rc0/requirements/test.txt
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)      302 2023-06-29 21:35:01.461235 numpydoc-1.6.0rc0/setup.cfg
+-rw-r--r--   0 jarrod   (10000) jarrod   (10000)     2285 2023-06-29 21:22:00.000000 numpydoc-1.6.0rc0/setup.py
```

### Comparing `numpydoc-1.5.0rc1/LICENSE.txt` & `numpydoc-1.6.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/PKG-INFO` & `numpydoc-1.6.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: numpydoc
-Version: 1.5.0rc1
+Version: 1.6.0rc0
 Summary: Sphinx extension to support docstrings in Numpy format
 Home-page: https://numpydoc.readthedocs.io
 Author: Pauli Virtanen and others
 Author-email: pav@iki.fi
 License: BSD
 Keywords: sphinx numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 =====================================
 numpydoc -- Numpy's Sphinx extensions
 =====================================
 
@@ -38,15 +37,15 @@
    :target: https://github.com/numpy/numpydoc/actions/workflows/test.yml
 
 This package provides the ``numpydoc`` Sphinx extension for handling
 docstrings formatted according to the NumPy documentation format.
 The extension also adds the code description directives
 ``np:function``, ``np-c:function``, etc.
 
-numpydoc requires Python 3.7+ and sphinx 4.2+.
+numpydoc requires Python 3.8+ and sphinx 5+.
 
 For usage information, please refer to the `documentation
 <https://numpydoc.readthedocs.io/>`_.
 
 The `numpydoc docstring guide
 <https://numpydoc.readthedocs.io/en/latest/format.html>`_ explains how
 to write docs formatted for this extension, and the `user guide
```

### Comparing `numpydoc-1.5.0rc1/README.rst` & `numpydoc-1.6.0rc0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
    :target: https://github.com/numpy/numpydoc/actions/workflows/test.yml
 
 This package provides the ``numpydoc`` Sphinx extension for handling
 docstrings formatted according to the NumPy documentation format.
 The extension also adds the code description directives
 ``np:function``, ``np-c:function``, etc.
 
-numpydoc requires Python 3.7+ and sphinx 4.2+.
+numpydoc requires Python 3.8+ and sphinx 5+.
 
 For usage information, please refer to the `documentation
 <https://numpydoc.readthedocs.io/>`_.
 
 The `numpydoc docstring guide
 <https://numpydoc.readthedocs.io/en/latest/format.html>`_ explains how
 to write docs formatted for this extension, and the `user guide
```

### Comparing `numpydoc-1.5.0rc1/RELEASE.rst` & `numpydoc-1.6.0rc0/RELEASE.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 - Review the github release page::
 
     https://github.com/numpy/numpydoc/releases
 
 - Publish on PyPi::
 
     git clean -fxd
-    pip install build wheel twine
+    pip install -U build wheel twine
     python -m build --sdist --wheel
     twine upload -s dist/*
 
 - Update ``__version__`` in ``numpydoc/_version.py``.
 
 - Commit changes::
```

### Comparing `numpydoc-1.5.0rc1/doc/Makefile` & `numpydoc-1.6.0rc0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/doc/conf.py` & `numpydoc-1.6.0rc0/doc/conf.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,31 +77,25 @@
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 html_theme = "pydata_sphinx_theme"
 html_theme_options = {
-    "github_url": "https://github.com/numpy/numpydoc",
     "show_prev_next": False,
-    "navbar_end": ["search-field.html", "navbar-icon-links.html"],
+    "navbar_end": ["theme-switcher", "search-field.html", "navbar-icon-links.html"],
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/numpy/numpydoc",
+            "icon": "fab fa-github-square",
+            "type": "fontawesome",
+        },
+    ],
 }
-# NOTE: The following is required for supporting of older sphinx toolchains.
-#       The "theme-switcher" templated should be added directly to navbar_end
-#       above and the following lines removed when the minimum supported
-#       version of pydata_sphinx_theme is 0.9.0
-# Add version switcher for versions of pydata_sphinx_theme that support it
-import packaging
-import pydata_sphinx_theme
-
-if packaging.version.parse(pydata_sphinx_theme.__version__) >= packaging.version.parse(
-    "0.9.0"
-):
-    html_theme_options["navbar_end"].insert(0, "theme-switcher")
-
 
 html_sidebars = {
     "**": [],
 }
 html_context = {
     "default_mode": "light",
 }
```

### Comparing `numpydoc-1.5.0rc1/doc/example.py` & `numpydoc-1.6.0rc0/doc/example.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/doc/format.rst` & `numpydoc-1.6.0rc0/doc/format.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/doc/index.rst` & `numpydoc-1.6.0rc0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/doc/install.rst` & `numpydoc-1.6.0rc0/doc/install.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ===============
 Getting started
 ===============
 
 Installation
 ============
 
-This extension requires Python 3.7+, sphinx 4.2+ and is available from:
+This extension requires Python 3.8+, sphinx 5+ and is available from:
 
 * `numpydoc on PyPI <http://pypi.python.org/pypi/numpydoc>`_
 * `numpydoc on GitHub <https://github.com/numpy/numpydoc/>`_
 
 `'numpydoc'` should be added to the ``extensions`` option in your Sphinx
 ``conf.py``. ``'sphinx.ext.autosummary'`` will automatically be loaded
 as well.
```

### Comparing `numpydoc-1.5.0rc1/doc/make.bat` & `numpydoc-1.6.0rc0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/doc/release_notes.rst` & `numpydoc-1.6.0rc0/doc/release_notes.rst`

 * *Files 11% similar despite different names*

```diff
@@ -13,23 +13,69 @@
    :depth: 2
 
 .. note::
 
    For release notes (sparsely) kept prior to 1.0.0, look at the `releases page
    on GitHub <https://github.com/numpy/numpydoc/releases>`__.
 
+1.6.0rc0
+--------
+
+Release date: 29 June 2023
+
+Requires Python 3.8+ and Sphinx 5+.
 
 1.5.0
 -----
 
-Release date: TBD
+Release date: 8 October 2022
 
 Requires Python 3.7+ and Sphinx 4.2+.
 
-`Full Changelog <https://github.com/numpy/numpydoc/compare/v1.4.0...v1.5.0rc1>`__
+`Full Changelog <https://github.com/numpy/numpydoc/compare/v1.4.0...v1.5.0>`__
+
+Fixed bugs
+~~~~~~~~~~
+
+-  Parsing ``returns`` section with several types and no name `#428 <https://github.com/numpy/numpydoc/issues/428>`__
+-  BUG: Fix returns parsing no name `#429 <https://github.com/numpy/numpydoc/pull/429>`__ (`rossbar <https://github.com/rossbar>`__)
+
+Closed issues
+~~~~~~~~~~~~~
+
+-  readthedocs build failing `#439 <https://github.com/numpy/numpydoc/issues/439>`__
+-  Exclude class properties from being listed under METHODS section `#339 <https://github.com/numpy/numpydoc/issues/339>`__
+-  BUG: Numpydoc doesn’t render attributes decorated with ``cached\_property`` in the Attributes section `#432 <https://github.com/numpy/numpydoc/issues/432>`__
+-  Is numpydoc_use_blockquotes deprecated or not yet? `#420 <https://github.com/numpy/numpydoc/issues/420>`__
+-  No light theme available in docs `#413 <https://github.com/numpy/numpydoc/issues/413>`__
+-  1.4.0 release plan `#408 <https://github.com/numpy/numpydoc/issues/408>`__
+
+Merged pull requests
+~~~~~~~~~~~~~~~~~~~~
+
+-  Update doc requirements `#441 <https://github.com/numpy/numpydoc/pull/441>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Update pydata-sphinx-theme `#440 <https://github.com/numpy/numpydoc/pull/440>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Support Python 3.11 `#438 <https://github.com/numpy/numpydoc/pull/438>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Update precommit hooks `#437 <https://github.com/numpy/numpydoc/pull/437>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Use Python 3.10 to build docs `#436 <https://github.com/numpy/numpydoc/pull/436>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Use `requirements/*.txt` files for CI `#435 <https://github.com/numpy/numpydoc/pull/435>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Fix front page `#434 <https://github.com/numpy/numpydoc/pull/434>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Add cached property support `#433 <https://github.com/numpy/numpydoc/pull/433>`__ (`rossbar <https://github.com/rossbar>`__)
+-  ENH: Update validate.py to allow parameters with trailing underscores. `#425 <https://github.com/numpy/numpydoc/pull/425>`__ (`stefmolin <https://github.com/stefmolin>`__)
+-  DOC: Use ``:ref:`` when referring to section headers `#424 <https://github.com/numpy/numpydoc/pull/424>`__ (`namurphy <https://github.com/namurphy>`__)
+-  Remove numpydoc_use_blockquotes `#422 <https://github.com/numpy/numpydoc/pull/422>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Require sphinx>=4.2 (cleanup) `#421 <https://github.com/numpy/numpydoc/pull/421>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  docs: fix validation include line numbers `#418 <https://github.com/numpy/numpydoc/pull/418>`__ (`thatlittleboy <https://github.com/thatlittleboy>`__)
+-  Update precommit linters `#417 <https://github.com/numpy/numpydoc/pull/417>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  Update GH actions `#416 <https://github.com/numpy/numpydoc/pull/416>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+-  ENH: Add support for dict show_inherited_class_members `#415 <https://github.com/numpy/numpydoc/pull/415>`__ (`larsoner <https://github.com/larsoner>`__)
+-  DOC: Add theme switcher and default to lightmode. `#414 <https://github.com/numpy/numpydoc/pull/414>`__ (`rossbar <https://github.com/rossbar>`__)
+-  Require sphinx>=4.2 `#411 <https://github.com/numpy/numpydoc/pull/411>`__ (`jarrodmillman <https://github.com/jarrodmillman>`__)
+
+\* *This Changelog was automatically generated by*\ `github_changelog_generator <https://github.com/github-changelog-generator/github-changelog-generator>`__
 
 1.4.0
 -----
 
 Release date: 9 June 2022
 
 Requires Python 3.7+ and Sphinx 3.0+.
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/__main__.py` & `numpydoc-1.6.0rc0/numpydoc/__main__.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/docscrape.py` & `numpydoc-1.6.0rc0/numpydoc/docscrape.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,20 +7,15 @@
 import pydoc
 from warnings import warn
 from collections import namedtuple
 from collections.abc import Callable, Mapping
 import copy
 import sys
 
-
-# TODO: Remove try-except when support for Python 3.7 is dropped
-try:
-    from functools import cached_property
-except ImportError:  # cached_property added in Python 3.8
-    cached_property = property
+from functools import cached_property
 
 
 def strip_blank_lines(l):
     "Remove leading and trailing blank lines from a list of lines"
     while l and not l[0].strip():
         del l[0]
     while l and not l[-1].strip():
@@ -404,15 +399,15 @@
         if has_returns and has_yields:
             msg = "Docstring contains both a Returns and Yields section."
             raise ValueError(msg)
         if not has_yields and "Receives" in section_names:
             msg = "Docstring contains a Receives section but not Yields."
             raise ValueError(msg)
 
-        for (section, content) in sections:
+        for section, content in sections:
             if not section.startswith(".."):
                 section = (s.capitalize() for s in section.split(" "))
                 section = " ".join(section)
                 if self.get(section):
                     self._error_location(
                         "The section %s appears twice in  %s"
                         % (section, "\n".join(self._doc._str))
@@ -627,15 +622,14 @@
         self._f = obj
         if config is None:
             config = {}
         NumpyDocString.__init__(self, doc, config=config)
 
 
 class ClassDoc(NumpyDocString):
-
     extra_public_methods = ["__call__"]
 
     def __init__(self, cls, doc=None, modulename="", func_doc=FunctionDoc, config=None):
         if not inspect.isclass(cls) and cls is not None:
             raise ValueError(f"Expected a class or None, but got {cls!r}")
         self._cls = cls
 
@@ -724,28 +718,36 @@
         if self.show_inherited_members:
             return True  # show all class members
         if name not in self._cls.__dict__:
             return False  # class member is inherited, we do not show it
         return True
 
 
-def get_doc_object(obj, what=None, doc=None, config=None):
+def get_doc_object(
+    obj,
+    what=None,
+    doc=None,
+    config=None,
+    class_doc=ClassDoc,
+    func_doc=FunctionDoc,
+    obj_doc=ObjDoc,
+):
     if what is None:
         if inspect.isclass(obj):
             what = "class"
         elif inspect.ismodule(obj):
             what = "module"
         elif isinstance(obj, Callable):
             what = "function"
         else:
             what = "object"
     if config is None:
         config = {}
 
     if what == "class":
-        return ClassDoc(obj, func_doc=FunctionDoc, doc=doc, config=config)
+        return class_doc(obj, func_doc=func_doc, doc=doc, config=config)
     elif what in ("function", "method"):
-        return FunctionDoc(obj, doc=doc, config=config)
+        return func_doc(obj, doc=doc, config=config)
     else:
         if doc is None:
             doc = pydoc.getdoc(obj)
-        return ObjDoc(obj, doc, config=config)
+        return obj_doc(obj, doc, config=config)
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/docscrape_sphinx.py` & `numpydoc-1.6.0rc0/numpydoc/docscrape_sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from jinja2 import FileSystemLoader
 from jinja2.sandbox import SandboxedEnvironment
 import sphinx
 from sphinx.jinja2glue import BuiltinTemplateLoader
 
 from .docscrape import NumpyDocString, FunctionDoc, ClassDoc, ObjDoc
+from .docscrape import get_doc_object as get_doc_object_orig
 from .xref import make_xref
 
 
 IMPORT_MATPLOTLIB_RE = r"\b(import +matplotlib|from +matplotlib +import)\b"
 
 
 class SphinxDocString(NumpyDocString):
@@ -403,38 +404,29 @@
     def __init__(self, obj, doc=None, config=None):
         if config is None:
             config = {}
         self.load_config(config)
         ObjDoc.__init__(self, obj, doc=doc, config=config)
 
 
-# TODO: refactor to use docscrape.get_doc_object
 def get_doc_object(obj, what=None, doc=None, config=None, builder=None):
-    if what is None:
-        if inspect.isclass(obj):
-            what = "class"
-        elif inspect.ismodule(obj):
-            what = "module"
-        elif isinstance(obj, Callable):
-            what = "function"
-        else:
-            what = "object"
-
     if config is None:
         config = {}
+
     template_dirs = [os.path.join(os.path.dirname(__file__), "templates")]
     if builder is not None:
         template_loader = BuiltinTemplateLoader()
         template_loader.init(builder, dirs=template_dirs)
     else:
         template_loader = FileSystemLoader(template_dirs)
     template_env = SandboxedEnvironment(loader=template_loader)
     config["template"] = template_env.get_template("numpydoc_docstring.rst")
 
-    if what == "class":
-        return SphinxClassDoc(obj, func_doc=SphinxFunctionDoc, doc=doc, config=config)
-    elif what in ("function", "method"):
-        return SphinxFunctionDoc(obj, doc=doc, config=config)
-    else:
-        if doc is None:
-            doc = pydoc.getdoc(obj)
-        return SphinxObjDoc(obj, doc, config=config)
+    return get_doc_object_orig(
+        obj,
+        what=what,
+        doc=doc,
+        config=config,
+        class_doc=SphinxClassDoc,
+        func_doc=SphinxFunctionDoc,
+        obj_doc=SphinxObjDoc,
+    )
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/numpydoc.py` & `numpydoc-1.6.0rc0/numpydoc/numpydoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
 
 from docutils.nodes import citation, Text, section, comment, reference
 import sphinx
 from sphinx.addnodes import pending_xref, desc_content
 from sphinx.util import logging
 from sphinx.errors import ExtensionError
 
-if sphinx.__version__ < "4.2":
-    raise RuntimeError("Sphinx 4.2 or newer is required")
+if sphinx.__version__ < "5":
+    raise RuntimeError("Sphinx 5 or newer is required")
 
 from .docscrape_sphinx import get_doc_object
 from .validate import validate, ERROR_MSGS
 from .xref import DEFAULT_LINKS
 from . import __version__
 
 logger = logging.getLogger(__name__)
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_docscrape.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_docscrape.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections import namedtuple
 from copy import deepcopy
 import re
-import sys
 import textwrap
 import warnings
 
 import jinja2
 
 from numpydoc.numpydoc import update_config
 from numpydoc.xref import DEFAULT_LINKS
@@ -1439,15 +1438,14 @@
             else:
                 return obj._data.axes[self.axis]
 
         def __set__(self, obj, value):
             obj._set_axis(self.axis, value)
 
     class Dummy:
-
         attr = SpecialProperty(doc="test attribute")
 
     doc = get_doc_object(Dummy)
     assert "test attribute" in str(doc)
 
 
 def test_args_and_kwargs():
@@ -1621,17 +1619,14 @@
     nds = get_doc_object(foo)
 
     msg = "Potentially wrong underline length.*Foo.*"
     with pytest.raises(ValueError, match=msg):
         nds._error_location(msg=msg)
 
 
-@pytest.mark.skipif(
-    sys.version_info < (3, 8), reason="cached_property was added in 3.8"
-)
 def test_class_docstring_cached_property():
     """Ensure that properties marked with the `cached_property` decorator
     are listed in the Methods section. See gh-432."""
     from functools import cached_property
 
     class Foo:
         _x = [1, 2, 3]
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_full.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_full.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_main.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_numpydoc.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_numpydoc.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_validate.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -502,20 +502,53 @@
 
         Examples
         --------
         >>> result = 1 + 1
         """
         pass
 
+    def parameter_with_wrong_types_as_substrings(self, a, b, c, d, e, f):
+        r"""
+        Ensure PR06 doesn't fail when non-preferable types are substrings.
+
+        While PR06 checks for parameter types which contain non-preferable type
+        names like integer (int), string (str), and boolean (bool), PR06 should
+        not fail if those types are used only as susbtrings in, for example,
+        custom type names.
+
+        Parameters
+        ----------
+        a : Myint
+           Some text.
+        b : intClass
+           Some text.
+        c : Mystring
+           Some text.
+        d : stringClass
+           Some text.
+        e : Mybool
+           Some text.
+        f : boolClass
+           Some text.
+
+        See Also
+        --------
+        related : Something related.
+
+        Examples
+        --------
+        >>> result = 1 + 1
+        """
+        pass
+
 
 class BadGenericDocStrings:
     """Everything here has a bad docstring"""
 
     def func(self):
-
         """Some function.
 
         With several mistakes in the docstring.
 
         It has a blank like after the signature `def func():`.
 
         The text 'Some function' should go in the line after the
@@ -1141,14 +1174,15 @@
             "no_returns",
             "empty_returns",
             "multiple_variables_on_one_line",
             "other_parameters",
             "warnings",
             "valid_options_in_parameter_description_sets",
             "parameters_with_trailing_underscores",
+            "parameter_with_wrong_types_as_substrings",
         ],
     )
     def test_good_functions(self, capsys, func):
         errors = validate_one(self._import_path(klass="GoodDocStrings", func=func))[
             "errors"
         ]
         assert isinstance(errors, list)
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/test_xref.py` & `numpydoc-1.6.0rc0/numpydoc/tests/test_xref.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/conf.py` & `numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/conf.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/tests/tinybuild/numpydoc_test_module.py` & `numpydoc-1.6.0rc0/numpydoc/tests/tinybuild/numpydoc_test_module.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc/validate.py` & `numpydoc-1.6.0rc0/numpydoc/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,25 +446,30 @@
         # Not ending in "." is only an error if the last bit is not
         # indented (e.g., quote or code block)
         if not desc[-1].endswith(".") and not desc[-1].startswith(IGNORE_STARTS):
             errs.append(error(code_no_period, **kwargs))
     return errs
 
 
-def validate(obj_name):
+def validate(obj_name, validator_cls=None, **validator_kwargs):
     """
     Validate the docstring.
 
     Parameters
     ----------
     obj_name : str
         The name of the object whose docstring will be evaluated, e.g.
         'pandas.read_csv'. The string must include the full, unabbreviated
         package/module names, i.e. 'pandas.read_csv', not 'pd.read_csv' or
         'read_csv'.
+    validator_cls : Validator, optional
+        The Validator class to use. By default, :class:`Validator` will be used.
+    **validator_kwargs
+        Keyword arguments to pass to ``validator_cls`` upon initialization.
+        Note that ``obj_name`` will be passed as a named argument as well.
 
     Returns
     -------
     dict
         A dictionary containing all the information obtained from validating
         the docstring.
 
@@ -489,18 +494,21 @@
     For example, PR02 is the second codified error in the Parameters section
     (which in this case is assigned to the error when unknown parameters are documented).
 
     The error codes, their corresponding error messages, and the details on how
     they are validated, are not documented more than in the source code of this
     function.
     """
-    if isinstance(obj_name, str):
-        doc = Validator(get_doc_object(Validator._load_obj(obj_name)))
+    if not validator_cls:
+        if isinstance(obj_name, str):
+            doc = Validator(get_doc_object(Validator._load_obj(obj_name)))
+        else:
+            doc = Validator(obj_name)
     else:
-        doc = Validator(obj_name)
+        doc = validator_cls(obj_name=obj_name, **validator_kwargs)
 
     errs = []
     if not doc.raw_doc:
         errs.append(error("GL08"))
         return {
             "type": doc.type,
             "docstring": doc.clean_doc,
@@ -580,15 +588,15 @@
                     continue
                 common_type_errors = [
                     ("integer", "int"),
                     ("boolean", "bool"),
                     ("string", "str"),
                 ]
                 for wrong_type, right_type in common_type_errors:
-                    if wrong_type in doc.parameter_type(param):
+                    if wrong_type in set(re.split(r"\W", doc.parameter_type(param))):
                         errs.append(
                             error(
                                 "PR06",
                                 param_name=param,
                                 right_type=right_type,
                                 wrong_type=wrong_type,
                             )
```

### Comparing `numpydoc-1.5.0rc1/numpydoc/xref.py` & `numpydoc-1.6.0rc0/numpydoc/xref.py`

 * *Files identical despite different names*

### Comparing `numpydoc-1.5.0rc1/numpydoc.egg-info/PKG-INFO` & `numpydoc-1.6.0rc0/numpydoc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: numpydoc
-Version: 1.5.0rc1
+Version: 1.6.0rc0
 Summary: Sphinx extension to support docstrings in Numpy format
 Home-page: https://numpydoc.readthedocs.io
 Author: Pauli Virtanen and others
 Author-email: pav@iki.fi
 License: BSD
 Keywords: sphinx numpy
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Documentation
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 =====================================
 numpydoc -- Numpy's Sphinx extensions
 =====================================
 
@@ -38,15 +37,15 @@
    :target: https://github.com/numpy/numpydoc/actions/workflows/test.yml
 
 This package provides the ``numpydoc`` Sphinx extension for handling
 docstrings formatted according to the NumPy documentation format.
 The extension also adds the code description directives
 ``np:function``, ``np-c:function``, etc.
 
-numpydoc requires Python 3.7+ and sphinx 4.2+.
+numpydoc requires Python 3.8+ and sphinx 5+.
 
 For usage information, please refer to the `documentation
 <https://numpydoc.readthedocs.io/>`_.
 
 The `numpydoc docstring guide
 <https://numpydoc.readthedocs.io/en/latest/format.html>`_ explains how
 to write docs formatted for this extension, and the `user guide
```

### Comparing `numpydoc-1.5.0rc1/numpydoc.egg-info/SOURCES.txt` & `numpydoc-1.6.0rc0/numpydoc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -21,23 +21,31 @@
 numpydoc/docscrape_sphinx.py
 numpydoc/numpydoc.py
 numpydoc/validate.py
 numpydoc/xref.py
 numpydoc.egg-info/PKG-INFO
 numpydoc.egg-info/SOURCES.txt
 numpydoc.egg-info/dependency_links.txt
+numpydoc.egg-info/entry_points.txt
 numpydoc.egg-info/requires.txt
 numpydoc.egg-info/top_level.txt
+numpydoc/hooks/__init__.py
+numpydoc/hooks/utils.py
+numpydoc/hooks/validate_docstrings.py
 numpydoc/templates/numpydoc_docstring.rst
 numpydoc/tests/test_docscrape.py
 numpydoc/tests/test_full.py
 numpydoc/tests/test_main.py
 numpydoc/tests/test_numpydoc.py
 numpydoc/tests/test_validate.py
 numpydoc/tests/test_xref.py
+numpydoc/tests/hooks/__init__.py
+numpydoc/tests/hooks/example_module.py
+numpydoc/tests/hooks/test_utils.py
+numpydoc/tests/hooks/test_validate_hook.py
 numpydoc/tests/tinybuild/Makefile
 numpydoc/tests/tinybuild/conf.py
 numpydoc/tests/tinybuild/index.rst
 numpydoc/tests/tinybuild/numpydoc_test_module.py
 requirements/developer.txt
 requirements/doc.txt
 requirements/test.txt
```

### Comparing `numpydoc-1.5.0rc1/setup.py` & `numpydoc-1.6.0rc0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     for line in (line.strip() for line in fid):
         if line.startswith("__version__"):
             version = line.split("=")[1].strip().strip('"')
             break
 if version is None:
     raise RuntimeError("Could not determine version")
 
-if sys.version_info < (3, 7):
-    raise RuntimeError("Python version >= 3.7 required.")
+if sys.version_info < (3, 8):
+    raise RuntimeError("Python version >= 3.8 required.")
 
 
 def read(fname):
     """Utility function to get README.rst into long_description.
 
     ``long_description`` is what ends up on the PyPI front page.
     """
@@ -26,39 +26,43 @@
         contents = f.read()
 
     return contents
 
 
 setup(
     name="numpydoc",
-    packages=["numpydoc"],
+    packages=["numpydoc", "numpydoc.hooks"],
     version=version,
     description="Sphinx extension to support docstrings in Numpy format",
     long_description=read("README.rst"),
     # classifiers from http://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Plugins",
         "License :: OSI Approved :: BSD License",
         "Topic :: Documentation",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     keywords="sphinx numpy",
     author="Pauli Virtanen and others",
     author_email="pav@iki.fi",
     url="https://numpydoc.readthedocs.io",
     license="BSD",
-    install_requires=["sphinx>=4.2", "Jinja2>=2.10"],
-    python_requires=">=3.7",
+    install_requires=[
+        "sphinx>=5",
+        "Jinja2>=2.10",
+        "tabulate>=0.8.10",
+        "tomli>=1.1.0;python_version<'3.11'",
+    ],
+    python_requires=">=3.8",
     extras_require={
         "testing": [
             req
             for req in read("requirements/test.txt").split("\n")
             if not req.startswith("#")
         ],
     },
```

