# Comparing `tmp/funcOAI-0.0.1.tar.gz` & `tmp/funcOAI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcOAI-0.0.1.tar", last modified: Thu Jun 29 07:42:07 2023, max compression
+gzip compressed data, was "funcOAI-0.0.2.tar", last modified: Thu Jun 29 07:52:43 2023, max compression
```

## Comparing `funcOAI-0.0.1.tar` & `funcOAI-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:42:07.793958 funcOAI-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-29 07:42:07.793958 funcOAI-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1815 2023-06-29 07:17:55.000000 funcOAI-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:42:07.793958 funcOAI-0.0.1/funcOAI.egg-info/
--rw-r--r--   0 root         (0) root         (0)      658 2023-06-29 07:42:07.000000 funcOAI-0.0.1/funcOAI.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      199 2023-06-29 07:42:07.000000 funcOAI-0.0.1/funcOAI.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:42:07.000000 funcOAI-0.0.1/funcOAI.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 07:42:07.000000 funcOAI-0.0.1/funcOAI.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:42:07.793958 funcOAI-0.0.1/functionalOAI/
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-29 07:17:55.000000 funcOAI-0.0.1/functionalOAI/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3462 2023-06-29 07:17:55.000000 funcOAI-0.0.1/functionalOAI/funAI.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:42:07.793958 funcOAI-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-29 07:41:08.000000 funcOAI-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 07:17:55.000000 funcOAI-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 07:52:43.203927 funcOAI-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1815 2023-06-29 07:17:55.000000 funcOAI-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/funcOAI.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      199 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 07:52:43.000000 funcOAI-0.0.2/funcOAI.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 07:52:43.203927 funcOAI-0.0.2/functionalOAI/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-29 07:17:55.000000 funcOAI-0.0.2/functionalOAI/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3462 2023-06-29 07:17:55.000000 funcOAI-0.0.2/functionalOAI/funAI.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 07:52:43.203927 funcOAI-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      979 2023-06-29 07:52:21.000000 funcOAI-0.0.2/setup.py
```

### Comparing `funcOAI-0.0.1/LICENSE` & `funcOAI-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcOAI-0.0.1/README.md` & `funcOAI-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `funcOAI-0.0.1/functionalOAI/funAI.py` & `funcOAI-0.0.2/functionalOAI/funAI.py`

 * *Files identical despite different names*

