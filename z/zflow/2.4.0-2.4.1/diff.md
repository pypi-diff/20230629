# Comparing `tmp/zflow-2.4.0.tar.gz` & `tmp/zflow-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zflow-2.4.0.tar", last modified: Fri Jun 16 13:27:17 2023, max compression
+gzip compressed data, was "zflow-2.4.1.tar", last modified: Thu Jun 29 12:39:19 2023, max compression
```

## Comparing `zflow-2.4.0.tar` & `zflow-2.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:27:17.470065 zflow-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-16 13:27:16.000000 zflow-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:27:17.470065 zflow-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-16 13:27:16.000000 zflow-2.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-16 13:27:16.000000 zflow-2.4.0/__version__.py
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-16 13:27:17.470065 zflow-2.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1441 2023-06-16 13:27:16.000000 zflow-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 13:27:17.470065 zflow-2.4.0/zflow.egg-info/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-16 13:27:17.000000 zflow-2.4.0/zflow.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2023-06-16 13:27:17.000000 zflow-2.4.0/zflow.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 13:27:17.000000 zflow-2.4.0/zflow.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 13:27:17.000000 zflow-2.4.0/zflow.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-16 13:27:17.000000 zflow-2.4.0/zflow.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:39:19.555512 zflow-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-29 12:39:18.000000 zflow-2.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-29 12:39:19.555512 zflow-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-29 12:39:18.000000 zflow-2.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-06-29 12:39:18.000000 zflow-2.4.1/__version__.py
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-29 12:39:19.555512 zflow-2.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1441 2023-06-29 12:39:18.000000 zflow-2.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 12:39:19.555512 zflow-2.4.1/zflow.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-29 12:39:19.000000 zflow-2.4.1/zflow.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-29 12:39:19.000000 zflow-2.4.1/zflow.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:39:19.000000 zflow-2.4.1/zflow.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 12:39:19.000000 zflow-2.4.1/zflow.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-29 12:39:19.000000 zflow-2.4.1/zflow.egg-info/top_level.txt
```

### Comparing `zflow-2.4.0/LICENSE` & `zflow-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zflow-2.4.0/setup.py` & `zflow-2.4.1/setup.py`

 * *Files identical despite different names*

