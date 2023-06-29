# Comparing `tmp/fewlines-0.0.2.tar.gz` & `tmp/fewlines-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fewlines-0.0.2.tar", last modified: Thu Jun 29 03:44:18 2023, max compression
+gzip compressed data, was "fewlines-0.0.3.tar", last modified: Thu Jun 29 15:41:44 2023, max compression
```

## Comparing `fewlines-0.0.2.tar` & `fewlines-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 03:44:18.225951 fewlines-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 03:44:07.000000 fewlines-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 03:44:18.225951 fewlines-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 03:44:07.000000 fewlines-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 03:44:18.225951 fewlines-0.0.2/fewlines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 03:44:07.000000 fewlines-0.0.2/fewlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 03:44:07.000000 fewlines-0.0.2/fewlines/horizon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 03:44:18.225951 fewlines-0.0.2/fewlines.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 03:44:18.000000 fewlines-0.0.2/fewlines.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 03:44:18.000000 fewlines-0.0.2/fewlines.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 03:44:18.000000 fewlines-0.0.2/fewlines.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 03:44:18.000000 fewlines-0.0.2/fewlines.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 03:44:18.225951 fewlines-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 03:44:07.000000 fewlines-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 15:41:32.000000 fewlines-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 15:41:44.529752 fewlines-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-29 15:41:32.000000 fewlines-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/fewlines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:32.000000 fewlines-0.0.3/fewlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-29 15:41:32.000000 fewlines-0.0.3/fewlines/horizon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:41:44.529752 fewlines-0.0.3/fewlines.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 15:41:44.000000 fewlines-0.0.3/fewlines.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:41:44.529752 fewlines-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-29 15:41:32.000000 fewlines-0.0.3/setup.py
```

### Comparing `fewlines-0.0.2/LICENSE` & `fewlines-0.0.3/LICENSE`

 * *Files identical despite different names*

