# Comparing `tmp/pyconvox-0.2.3.tar.gz` & `tmp/pyconvox-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconvox-0.2.3.tar", last modified: Thu Jun 29 12:29:02 2023, max compression
+gzip compressed data, was "pyconvox-2.0.0.dev0.tar", last modified: Fri Mar 18 22:11:08 2022, max compression
```

## Comparing `pyconvox-0.2.3.tar` & `pyconvox-2.0.0.dev0.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 12:29:02.202929 pyconvox-0.2.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1073 2023-06-29 12:28:52.000000 pyconvox-0.2.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6164 2023-06-29 12:29:02.202929 pyconvox-0.2.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5388 2023-06-29 12:28:52.000000 pyconvox-0.2.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 12:29:02.198929 pyconvox-0.2.3/pyconvox/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      556 2023-06-29 12:28:52.000000 pyconvox-0.2.3/pyconvox/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8299 2023-06-29 12:28:52.000000 pyconvox-0.2.3/pyconvox/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-29 12:28:52.000000 pyconvox-0.2.3/pyconvox/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-29 12:29:02.202929 pyconvox-0.2.3/pyconvox.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6164 2023-06-29 12:29:02.000000 pyconvox-0.2.3/pyconvox.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2023-06-29 12:29:02.000000 pyconvox-0.2.3/pyconvox.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-29 12:29:02.000000 pyconvox-0.2.3/pyconvox.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       52 2023-06-29 12:29:02.000000 pyconvox-0.2.3/pyconvox.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        9 2023-06-29 12:29:02.000000 pyconvox-0.2.3/pyconvox.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-29 12:29:02.202929 pyconvox-0.2.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1746 2023-06-29 12:28:52.000000 pyconvox-0.2.3/setup.py
+drwxr-xr-x   0 ak        (1000) ak        (1000)        0 2022-03-18 22:11:08.209145 pyconvox-2.0.0.dev0/
+-rw-r--r--   0 ak        (1000) ak        (1000)     1073 2022-03-18 21:35:16.000000 pyconvox-2.0.0.dev0/LICENSE
+-rw-r--r--   0 ak        (1000) ak        (1000)      748 2022-03-18 22:11:08.209145 pyconvox-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 ak        (1000) ak        (1000)        6 2022-03-18 21:35:16.000000 pyconvox-2.0.0.dev0/README.rst
+drwxr-xr-x   0 ak        (1000) ak        (1000)        0 2022-03-18 22:11:08.209145 pyconvox-2.0.0.dev0/bin/
+-rw-r--r--   0 ak        (1000) ak        (1000)      155 2022-03-18 21:59:27.000000 pyconvox-2.0.0.dev0/bin/pyconvox
+drwxr-xr-x   0 ak        (1000) ak        (1000)        0 2022-03-18 22:11:08.209145 pyconvox-2.0.0.dev0/pyconvox.egg-info/
+-rw-r--r--   0 ak        (1000) ak        (1000)      748 2022-03-18 22:11:08.000000 pyconvox-2.0.0.dev0/pyconvox.egg-info/PKG-INFO
+-rw-r--r--   0 ak        (1000) ak        (1000)      168 2022-03-18 22:11:08.000000 pyconvox-2.0.0.dev0/pyconvox.egg-info/SOURCES.txt
+-rw-r--r--   0 ak        (1000) ak        (1000)        1 2022-03-18 22:11:08.000000 pyconvox-2.0.0.dev0/pyconvox.egg-info/dependency_links.txt
+-rw-r--r--   0 ak        (1000) ak        (1000)        1 2022-03-18 22:11:08.000000 pyconvox-2.0.0.dev0/pyconvox.egg-info/top_level.txt
+-rw-r--r--   0 ak        (1000) ak        (1000)       38 2022-03-18 22:11:08.209145 pyconvox-2.0.0.dev0/setup.cfg
+-rw-r--r--   0 ak        (1000) ak        (1000)     1436 2022-03-18 22:10:59.000000 pyconvox-2.0.0.dev0/setup.py
```

### Comparing `pyconvox-0.2.3/LICENSE` & `pyconvox-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

