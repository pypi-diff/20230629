# Comparing `tmp/tychos-0.0.0.tar.gz` & `tmp/tychos-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tychos-0.0.0.tar", last modified: Tue Jun 27 17:03:06 2023, max compression
+gzip compressed data, was "tychos-0.0.1.tar", last modified: Thu Jun 29 20:39:33 2023, max compression
```

## Comparing `tychos-0.0.0.tar` & `tychos-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-27 17:03:06.525946 tychos-0.0.0/
--rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.0/LICENSE
--rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-27 17:03:06.525819 tychos-0.0.0/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)       19 2023-06-27 16:59:52.000000 tychos-0.0.0/README.md
--rw-r--r--   0 abe732     (501) staff       (20)       38 2023-06-27 17:03:06.525981 tychos-0.0.0/setup.cfg
--rw-r--r--   0 abe732     (501) staff       (20)       37 2023-06-26 15:37:15.000000 tychos-0.0.0/setup.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-27 17:03:06.525263 tychos-0.0.0/tychos/
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:18:44.000000 tychos-0.0.0/tychos/__init__.py
--rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:20:14.000000 tychos-0.0.0/tychos/api.py
-drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-27 17:03:06.525679 tychos-0.0.0/tychos.egg-info/
--rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-27 17:03:06.000000 tychos-0.0.0/tychos.egg-info/PKG-INFO
--rw-r--r--   0 abe732     (501) staff       (20)      179 2023-06-27 17:03:06.000000 tychos-0.0.0/tychos.egg-info/SOURCES.txt
--rw-r--r--   0 abe732     (501) staff       (20)        1 2023-06-27 17:03:06.000000 tychos-0.0.0/tychos.egg-info/dependency_links.txt
--rw-r--r--   0 abe732     (501) staff       (20)        7 2023-06-27 17:03:06.000000 tychos-0.0.0/tychos.egg-info/top_level.txt
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.321531 tychos-0.0.1/
+-rw-r--r--   0 abe732     (501) staff       (20)     1086 2023-06-27 16:58:58.000000 tychos-0.0.1/LICENSE
+-rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-29 20:39:33.321416 tychos-0.0.1/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)       19 2023-06-27 16:59:52.000000 tychos-0.0.1/README.md
+-rw-r--r--   0 abe732     (501) staff       (20)       38 2023-06-29 20:39:33.321579 tychos-0.0.1/setup.cfg
+-rw-r--r--   0 abe732     (501) staff       (20)       58 2023-06-29 20:39:02.000000 tychos-0.0.1/setup.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.320662 tychos-0.0.1/tychos/
+-rw-r--r--   0 abe732     (501) staff       (20)       47 2023-06-29 19:17:21.000000 tychos-0.0.1/tychos/__init__.py
+-rw-r--r--   0 abe732     (501) staff       (20)        0 2023-06-26 15:20:14.000000 tychos-0.0.1/tychos/api.py
+-rw-r--r--   0 abe732     (501) staff       (20)      748 2023-06-29 20:37:31.000000 tychos-0.0.1/tychos/vector_data_store.py
+drwxr-xr-x   0 abe732     (501) staff       (20)        0 2023-06-29 20:39:33.321274 tychos-0.0.1/tychos.egg-info/
+-rw-r--r--   0 abe732     (501) staff       (20)       72 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/PKG-INFO
+-rw-r--r--   0 abe732     (501) staff       (20)      207 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/SOURCES.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        1 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/dependency_links.txt
+-rw-r--r--   0 abe732     (501) staff       (20)        7 2023-06-29 20:39:33.000000 tychos-0.0.1/tychos.egg-info/top_level.txt
```

### Comparing `tychos-0.0.0/LICENSE` & `tychos-0.0.1/LICENSE`

 * *Files identical despite different names*

