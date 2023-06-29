# Comparing `tmp/pylsat-0.2.3.tar.gz` & `tmp/pylsat-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsat-0.2.3.tar", last modified: Thu Jun 29 15:43:35 2023, max compression
+gzip compressed data, was "pylsat-0.2.5.tar", last modified: Thu Jun 29 17:16:31 2023, max compression
```

## Comparing `pylsat-0.2.3.tar` & `pylsat-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 15:43:35.220666 pylsat-0.2.3/
--rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.3/LICENSE
--rw-rw-rw-   0        0        0      325 2023-06-29 15:43:35.220163 pylsat-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 15:43:35.217593 pylsat-0.2.3/pylsat.egg-info/
--rw-rw-rw-   0        0        0      325 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 15:43:35.000000 pylsat-0.2.3/pylsat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 15:43:35.220666 pylsat-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-06-29 15:43:14.000000 pylsat-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.812717 pylsat-0.2.5/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0      325 2023-06-29 17:16:31.811712 pylsat-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.779677 pylsat-0.2.5/pylsat/
+-rw-rw-rw-   0        0        0       75 2023-06-29 17:08:01.000000 pylsat-0.2.5/pylsat/__init__.py
+-rw-rw-rw-   0        0        0     5279 2023-06-29 14:08:53.000000 pylsat-0.2.5/pylsat/pylsat.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.796365 pylsat-0.2.5/pylsat.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-29 17:16:31.000000 pylsat-0.2.5/pylsat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 17:16:31.813722 pylsat-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      504 2023-06-29 17:06:31.000000 pylsat-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.797369 pylsat-0.2.5/vendor/
+-rw-rw-rw-   0        0        0        0 2023-06-29 16:21:16.000000 pylsat-0.2.5/vendor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:16:31.809609 pylsat-0.2.5/vendor/bolt11/
+-rw-rw-rw-   0        0        0      155 2023-06-29 17:03:55.000000 pylsat-0.2.5/vendor/bolt11/__init__.py
+-rw-rw-rw-   0        0        0      253 2023-06-29 14:05:03.000000 pylsat-0.2.5/vendor/bolt11/compat.py
+-rw-rw-rw-   0        0        0     6626 2023-06-29 14:04:41.000000 pylsat-0.2.5/vendor/bolt11/core.py
+-rw-rw-rw-   0        0        0     2743 2023-06-29 17:10:16.000000 pylsat-0.2.5/vendor/bolt11/types.py
+-rw-rw-rw-   0        0        0     2149 2023-06-29 14:05:55.000000 pylsat-0.2.5/vendor/bolt11/utils.py
```

### Comparing `pylsat-0.2.3/LICENSE` & `pylsat-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pylsat-0.2.3/README.md` & `pylsat-0.2.5/README.md`

 * *Files identical despite different names*

