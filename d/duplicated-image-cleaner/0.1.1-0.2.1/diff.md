# Comparing `tmp/duplicated_image_cleaner-0.1.1.tar.gz` & `tmp/duplicated_image_cleaner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplicated_image_cleaner-0.1.1.tar", last modified: Thu Jun 29 20:58:57 2023, max compression
+gzip compressed data, was "duplicated_image_cleaner-0.2.1.tar", last modified: Thu Jun 29 21:03:27 2023, max compression
```

## Comparing `duplicated_image_cleaner-0.1.1.tar` & `duplicated_image_cleaner-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 20:58:57.372105 duplicated_image_cleaner-0.1.1/
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      179 2023-06-29 20:58:57.371967 duplicated_image_cleaner-0.1.1/PKG-INFO
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)     2624 2023-06-29 20:57:14.000000 duplicated_image_cleaner-0.1.1/README.md
-drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 20:58:57.370559 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner/
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 20:28:25.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner/__init__.py
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)     3836 2023-06-29 20:09:49.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner/duplicated_image_cleaner.py
-drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 20:58:57.371729 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      179 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/PKG-INFO
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      398 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/SOURCES.txt
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        1 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/dependency_links.txt
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       68 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/entry_points.txt
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       31 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/requires.txt
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       25 2023-06-29 20:58:57.000000 duplicated_image_cleaner-0.1.1/duplicated_image_cleaner.egg-info/top_level.txt
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       38 2023-06-29 20:58:57.372148 duplicated_image_cleaner-0.1.1/setup.cfg
--rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      485 2023-06-29 20:58:15.000000 duplicated_image_cleaner-0.1.1/setup.py
+drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 21:03:27.556214 duplicated_image_cleaner-0.2.1/
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      179 2023-06-29 21:03:27.556053 duplicated_image_cleaner-0.2.1/PKG-INFO
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)     2624 2023-06-29 20:57:14.000000 duplicated_image_cleaner-0.2.1/README.md
+drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 21:03:27.554593 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner/
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)     3836 2023-06-29 21:02:53.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner/__init__.py
+drwxr-xr-x   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        0 2023-06-29 21:03:27.555783 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      179 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/PKG-INFO
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      345 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/SOURCES.txt
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)        1 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/dependency_links.txt
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       68 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/entry_points.txt
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       31 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/requires.txt
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       25 2023-06-29 21:03:27.000000 duplicated_image_cleaner-0.2.1/duplicated_image_cleaner.egg-info/top_level.txt
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)       38 2023-06-29 21:03:27.556279 duplicated_image_cleaner-0.2.1/setup.cfg
+-rw-r--r--   0 JORGE.ANZOLAOROPEZA   (502) staff       (20)      485 2023-06-29 21:03:06.000000 duplicated_image_cleaner-0.2.1/setup.py
```

### Comparing `duplicated_image_cleaner-0.1.1/README.md` & `duplicated_image_cleaner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `duplicated_image_cleaner-0.1.1/duplicated_image_cleaner/duplicated_image_cleaner.py` & `duplicated_image_cleaner-0.2.1/duplicated_image_cleaner/__init__.py`

 * *Files identical despite different names*

