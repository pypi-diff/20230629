# Comparing `tmp/pylsat-0.2.2.tar.gz` & `tmp/pylsat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsat-0.2.2.tar", last modified: Thu Jun 29 14:45:20 2023, max compression
+gzip compressed data, was "pylsat-0.2.3.tar", last modified: Thu Jun 29 15:43:35 2023, max compression
```

## Comparing `pylsat-0.2.2.tar` & `pylsat-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:20.818321 pylsat-0.2.2/
--rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      325 2023-06-29 14:45:20.817215 pylsat-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 14:45:20.815174 pylsat-0.2.2/pylsat.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-29 14:45:20.000000 pylsat-0.2.2/pylsat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-06-29 14:45:20.000000 pylsat-0.2.2/pylsat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:45:20.000000 pylsat-0.2.2/pylsat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-29 14:45:20.000000 pylsat-0.2.2/pylsat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:45:20.000000 pylsat-0.2.2/pylsat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:45:20.818321 pylsat-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-06-29 14:43:48.000000 pylsat-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 15:43:35.220666 pylsat-0.2.3/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0      325 2023-06-29 15:43:35.220163 pylsat-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 15:43:35.217593 pylsat-0.2.3/pylsat.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 15:43:35.220666 pylsat-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-06-29 15:43:14.000000 pylsat-0.2.3/setup.py
```

### Comparing `pylsat-0.2.2/LICENSE` & `pylsat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylsat-0.2.2/README.md` & `pylsat-0.2.3/README.md`

 * *Files identical despite different names*

