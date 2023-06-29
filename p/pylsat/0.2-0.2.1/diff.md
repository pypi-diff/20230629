# Comparing `tmp/pylsat-0.2.tar.gz` & `tmp/pylsat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylsat-0.2.tar", last modified: Thu Jun 29 14:11:31 2023, max compression
+gzip compressed data, was "pylsat-0.2.1.tar", last modified: Thu Jun 29 14:36:29 2023, max compression
```

## Comparing `pylsat-0.2.tar` & `pylsat-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 14:11:31.186502 pylsat-0.2/
--rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2/LICENSE
--rw-rw-rw-   0        0        0      300 2023-06-29 14:11:31.186502 pylsat-0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 14:11:31.184332 pylsat-0.2/pylsat.egg-info/
--rw-rw-rw-   0        0        0      300 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 14:11:31.000000 pylsat-0.2/pylsat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 14:11:31.186502 pylsat-0.2/setup.cfg
--rw-rw-rw-   0        0        0      542 2023-06-29 14:09:51.000000 pylsat-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 14:36:29.897328 pylsat-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2023-06-29 13:36:39.000000 pylsat-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      325 2023-06-29 14:36:29.896325 pylsat-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2179 2023-06-29 14:22:58.000000 pylsat-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 14:36:29.894024 pylsat-0.2.1/pylsat.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-06-29 14:36:29.000000 pylsat-0.2.1/pylsat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2023-06-29 14:36:29.000000 pylsat-0.2.1/pylsat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:36:29.000000 pylsat-0.2.1/pylsat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-29 14:36:29.000000 pylsat-0.2.1/pylsat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 14:36:29.000000 pylsat-0.2.1/pylsat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 14:36:29.898834 pylsat-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      569 2023-06-29 14:15:47.000000 pylsat-0.2.1/setup.py
```

### Comparing `pylsat-0.2/LICENSE` & `pylsat-0.2.1/LICENSE`

 * *Files identical despite different names*

