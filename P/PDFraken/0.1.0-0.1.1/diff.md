# Comparing `tmp/PDFraken-0.1.0.tar.gz` & `tmp/PDFraken-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PDFraken-0.1.0.tar", last modified: Thu Jun 29 19:50:46 2023, max compression
+gzip compressed data, was "dist/PDFraken-0.1.1.tar", last modified: Thu Jun 29 20:09:58 2023, max compression
```

## Comparing `PDFraken-0.1.0.tar` & `PDFraken-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 19:50:46.000000 PDFraken-0.1.0/
-drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken/
--rw-r--r--   0 patrickfleith   (501) staff       (20)        0 2023-06-29 19:38:28.000000 PDFraken-0.1.0/PDFraken/__init__.py
--rw-r--r--   0 patrickfleith   (501) staff       (20)     6015 2023-06-29 19:38:28.000000 PDFraken-0.1.0/PDFraken/cli.py
--rw-r--r--   0 patrickfleith   (501) staff       (20)      294 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PKG-INFO
--rw-r--r--   0 patrickfleith   (501) staff       (20)       10 2023-06-29 19:38:28.000000 PDFraken-0.1.0/README.md
--rw-r--r--   0 patrickfleith   (501) staff       (20)      502 2023-06-29 19:38:28.000000 PDFraken-0.1.0/setup.py
--rw-r--r--   0 patrickfleith   (501) staff       (20)       38 2023-06-29 19:50:46.000000 PDFraken-0.1.0/setup.cfg
-drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/
--rw-r--r--   0 patrickfleith   (501) staff       (20)      294 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/PKG-INFO
--rw-r--r--   0 patrickfleith   (501) staff       (20)      249 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/SOURCES.txt
--rw-r--r--   0 patrickfleith   (501) staff       (20)       47 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/entry_points.txt
--rw-r--r--   0 patrickfleith   (501) staff       (20)       13 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/requires.txt
--rw-r--r--   0 patrickfleith   (501) staff       (20)        9 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/top_level.txt
--rw-r--r--   0 patrickfleith   (501) staff       (20)        1 2023-06-29 19:50:46.000000 PDFraken-0.1.0/PDFraken.egg-info/dependency_links.txt
+drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 20:09:58.364929 PDFraken-0.1.1/
+-rw-r--r--   0 patrickfleith   (501) staff       (20)     1071 2023-06-29 19:38:28.000000 PDFraken-0.1.1/LICENSE
+drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 20:09:58.359401 PDFraken-0.1.1/PDFraken/
+-rw-r--r--   0 patrickfleith   (501) staff       (20)        0 2023-06-29 19:38:28.000000 PDFraken-0.1.1/PDFraken/__init__.py
+-rw-r--r--   0 patrickfleith   (501) staff       (20)     6015 2023-06-29 19:38:28.000000 PDFraken-0.1.1/PDFraken/cli.py
+drwxr-xr-x   0 patrickfleith   (501) staff       (20)        0 2023-06-29 20:09:58.363728 PDFraken-0.1.1/PDFraken.egg-info/
+-rw-r--r--   0 patrickfleith   (501) staff       (20)      298 2023-06-29 20:09:57.000000 PDFraken-0.1.1/PDFraken.egg-info/PKG-INFO
+-rw-r--r--   0 patrickfleith   (501) staff       (20)      257 2023-06-29 20:09:58.000000 PDFraken-0.1.1/PDFraken.egg-info/SOURCES.txt
+-rw-r--r--   0 patrickfleith   (501) staff       (20)        1 2023-06-29 20:09:57.000000 PDFraken-0.1.1/PDFraken.egg-info/dependency_links.txt
+-rw-r--r--   0 patrickfleith   (501) staff       (20)       46 2023-06-29 20:09:57.000000 PDFraken-0.1.1/PDFraken.egg-info/entry_points.txt
+-rw-r--r--   0 patrickfleith   (501) staff       (20)       13 2023-06-29 20:09:57.000000 PDFraken-0.1.1/PDFraken.egg-info/requires.txt
+-rw-r--r--   0 patrickfleith   (501) staff       (20)        9 2023-06-29 20:09:58.000000 PDFraken-0.1.1/PDFraken.egg-info/top_level.txt
+-rw-r--r--   0 patrickfleith   (501) staff       (20)      298 2023-06-29 20:09:58.364341 PDFraken-0.1.1/PKG-INFO
+-rw-r--r--   0 patrickfleith   (501) staff       (20)       10 2023-06-29 19:38:28.000000 PDFraken-0.1.1/README.md
+-rw-r--r--   0 patrickfleith   (501) staff       (20)       38 2023-06-29 20:09:58.365107 PDFraken-0.1.1/setup.cfg
+-rw-r--r--   0 patrickfleith   (501) staff       (20)      502 2023-06-29 20:05:15.000000 PDFraken-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PDFraken-0.1.0/PDFraken/cli.py` & `PDFraken-0.1.1/PDFraken/cli.py`

 * *Files identical despite different names*

