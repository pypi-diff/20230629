# Comparing `tmp/atomlite-1.2.0.tar.gz` & `tmp/atomlite-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atomlite-1.2.0.tar", last modified: Wed May 24 15:24:01 2023, max compression
+gzip compressed data, was "atomlite-1.3.0.tar", last modified: Thu Jun 29 14:56:20 2023, max compression
```

## Comparing `atomlite-1.2.0.tar` & `atomlite-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 15:24:01.492031 atomlite-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1230 2023-05-24 15:23:47.000000 atomlite-1.2.0/README.rst
--rw-r--r--   0 root         (0) root         (0)     1156 2023-05-24 15:23:47.000000 atomlite-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 15:24:01.492031 atomlite-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.488031 atomlite-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.488031 atomlite-1.2.0/src/atomlite/
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/src/atomlite/_internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11418 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/database.py
--rw-r--r--   0 root         (0) root         (0)     5633 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/_internal/json.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-24 15:23:47.000000 atomlite-1.2.0/src/atomlite/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/src/atomlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1545 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      375 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-24 15:24:01.000000 atomlite-1.2.0/src/atomlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 15:24:01.492031 atomlite-1.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)    10139 2023-05-24 15:23:47.000000 atomlite-1.2.0/tests/test_database.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-29 14:56:20.944223 atomlite-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-06-29 14:56:08.000000 atomlite-1.3.0/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1156 2023-06-29 14:56:08.000000 atomlite-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 14:56:20.944223 atomlite-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite/
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite/_internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11418 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/database.py
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/_internal/json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 14:56:08.000000 atomlite-1.3.0/src/atomlite/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/src/atomlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      375 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-29 14:56:20.000000 atomlite-1.3.0/src/atomlite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 14:56:20.944223 atomlite-1.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    10139 2023-06-29 14:56:08.000000 atomlite-1.3.0/tests/test_database.py
```

### Comparing `atomlite-1.2.0/PKG-INFO` & `atomlite-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.2.0
+Version: 1.3.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.2.0/README.rst` & `atomlite-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `atomlite-1.2.0/pyproject.toml` & `atomlite-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `atomlite-1.2.0/src/atomlite/_internal/database.py` & `atomlite-1.3.0/src/atomlite/_internal/database.py`

 * *Files identical despite different names*

### Comparing `atomlite-1.2.0/src/atomlite/_internal/json.py` & `atomlite-1.3.0/src/atomlite/_internal/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 import rdkit.Chem as rdkit
 
 Json: typing.TypeAlias = (
-    bool | float | str | None | list["Json"] | dict[str, "Json"]
+    bool | int | float | str | None | list["Json"] | dict[str, "Json"]
 )
 Conformer: typing.TypeAlias = list[list[float]]
 
 
 class Bonds(typing.TypedDict):
     """
     JSON representation of bonds.
```

### Comparing `atomlite-1.2.0/src/atomlite.egg-info/PKG-INFO` & `atomlite-1.3.0/src/atomlite.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atomlite
-Version: 1.2.0
+Version: 1.3.0
 Maintainer-email: Lukas Turcani <lukasturcani93@gmail.com>
 Project-URL: github, https://github.com/lukasturcani/atomlite
 Project-URL: documentation, https://atomlite.readthedocs.io
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
```

### Comparing `atomlite-1.2.0/tests/test_database.py` & `atomlite-1.3.0/tests/test_database.py`

 * *Files identical despite different names*

