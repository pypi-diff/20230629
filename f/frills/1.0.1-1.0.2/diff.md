# Comparing `tmp/frills-1.0.1.tar.gz` & `tmp/frills-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Y:\Projects\frills\src\dist\.tmp-zh3d6j5o\frills-1.0.1.tar", last modified: Thu Jun 29 12:50:17 2023, max compression
+gzip compressed data, was "Y:\Projects\frills\src\dist\.tmp-j9z05spi\frills-1.0.2.tar", last modified: Thu Jun 29 14:25:12 2023, max compression
```

## Comparing `frills-1.0.1.tar` & `frills-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 12:50:17.000000 frills-1.0.1/
--rw-rw-rw-   0        0        0     1087 2023-06-26 13:57:41.000000 frills-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      496 2023-06-29 12:50:17.000000 frills-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2023-06-29 12:30:59.000000 frills-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 12:50:17.000000 frills-1.0.1/frills/
--rw-rw-rw-   0        0        0      267 2023-06-29 12:18:10.000000 frills-1.0.1/frills/debugging.py
--rw-rw-rw-   0        0        0      243 2023-06-29 12:03:34.000000 frills-1.0.1/frills/graphics.py
--rw-rw-rw-   0        0        0        0 2023-06-26 13:33:12.000000 frills-1.0.1/frills/init.py
-drwxrwxrwx   0        0        0        0 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/
--rw-rw-rw-   0        0        0      496 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-29 12:50:17.000000 frills-1.0.1/frills.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      525 2023-06-29 12:50:07.000000 frills-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 12:50:17.000000 frills-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 14:25:12.000000 frills-1.0.2/
+-rw-rw-rw-   0        0        0     1087 2023-06-26 13:57:41.000000 frills-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      499 2023-06-29 14:25:12.000000 frills-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      103 2023-06-29 14:24:33.000000 frills-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:25:12.000000 frills-1.0.2/frills/
+-rw-rw-rw-   0        0        0      267 2023-06-29 12:18:10.000000 frills-1.0.2/frills/debugging.py
+-rw-rw-rw-   0        0        0      243 2023-06-29 12:03:34.000000 frills-1.0.2/frills/graphics.py
+-rw-rw-rw-   0        0        0        0 2023-06-26 13:33:12.000000 frills-1.0.2/frills/init.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/
+-rw-rw-rw-   0        0        0      499 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 14:25:12.000000 frills-1.0.2/frills.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      525 2023-06-29 14:24:26.000000 frills-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:25:12.000000 frills-1.0.2/setup.cfg
```

### Comparing `frills-1.0.1/LICENSE` & `frills-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frills-1.0.1/pyproject.toml` & `frills-1.0.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frills"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="Seb Gregory", email="sebgregory4@gmail.com" },
 ]
 readme = "README.md"
 description = "Helpful utilities for python development"
 requires-python = ">=3.7"
 classifiers = [
```

