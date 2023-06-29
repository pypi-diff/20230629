# Comparing `tmp/keyflow-0.0.1.tar.gz` & `tmp/keyflow-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyflow-0.0.1.tar", last modified: Thu Jun 29 18:30:30 2023, max compression
+gzip compressed data, was "keyflow-0.0.2.tar", last modified: Thu Jun 29 20:33:21 2023, max compression
```

## Comparing `keyflow-0.0.1.tar` & `keyflow-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:30:30.322321 keyflow-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-29 18:24:41.000000 keyflow-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2549 2023-06-29 18:30:30.320323 keyflow-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1982 2023-06-29 18:23:45.000000 keyflow-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-29 18:30:30.106321 keyflow-0.0.1/keyflow/
--rw-rw-rw-   0        0        0        0 2023-06-29 16:52:00.000000 keyflow-0.0.1/keyflow/__init__.py
--rw-rw-rw-   0        0        0     8057 2023-06-29 13:59:07.000000 keyflow-0.0.1/keyflow/keyflow.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:30:30.315320 keyflow-0.0.1/keyflow.egg-info/
--rw-rw-rw-   0        0        0     2549 2023-06-29 18:30:29.000000 keyflow-0.0.1/keyflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-06-29 18:30:30.000000 keyflow-0.0.1/keyflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:30:29.000000 keyflow-0.0.1/keyflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 18:30:29.000000 keyflow-0.0.1/keyflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      675 2023-06-29 18:29:15.000000 keyflow-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 18:30:30.323323 keyflow-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.753905 keyflow-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-29 18:24:41.000000 keyflow-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     4898 2023-06-29 20:33:21.751904 keyflow-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4331 2023-06-29 20:27:36.000000 keyflow-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.655909 keyflow-0.0.2/keyflow/
+-rw-rw-rw-   0        0        0     8057 2023-06-29 13:59:07.000000 keyflow-0.0.2/keyflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:33:21.748908 keyflow-0.0.2/keyflow.egg-info/
+-rw-rw-rw-   0        0        0     4898 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 20:33:21.000000 keyflow-0.0.2/keyflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      675 2023-06-29 20:32:53.000000 keyflow-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:33:21.754907 keyflow-0.0.2/setup.cfg
```

### Comparing `keyflow-0.0.1/LICENSE` & `keyflow-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keyflow-0.0.1/keyflow/keyflow.py` & `keyflow-0.0.2/keyflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keyflow-0.0.1/pyproject.toml` & `keyflow-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0', 'keyboard', 'colorama']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keyflow"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Aneousion", email="sanusirry@gmail.com" },
 ]
 description = 'A small python library to simulate typing in the console and custom text formatting.'
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

