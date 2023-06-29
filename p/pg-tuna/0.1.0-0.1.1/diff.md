# Comparing `tmp/pg_tuna-0.1.0.tar.gz` & `tmp/pg_tuna-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg_tuna-0.1.0.tar", last modified: Thu Jun 29 10:51:36 2023, max compression
+gzip compressed data, was "pg_tuna-0.1.1.tar", last modified: Thu Jun 29 10:59:10 2023, max compression
```

## Comparing `pg_tuna-0.1.0.tar` & `pg_tuna-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/
--rw-r--r--   0 delicj    (1002) delicj    (1002)     1069 2023-06-28 19:22:48.000000 pg_tuna-0.1.0/LICENSE
--rw-r--r--   0 delicj    (1002) delicj    (1002)     8078 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/PKG-INFO
--rw-r--r--   0 delicj    (1002) delicj    (1002)     7509 2023-06-29 10:51:16.000000 pg_tuna-0.1.0/README.md
--rw-r--r--   0 delicj    (1002) delicj    (1002)       38 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/setup.cfg
--rw-r--r--   0 delicj    (1002) delicj    (1002)     1031 2023-06-29 10:29:10.000000 pg_tuna-0.1.0/setup.py
-drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/src/
-drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/src/pg_tuna/
--rw-r--r--   0 delicj    (1002) delicj    (1002)        2 2023-06-28 19:23:06.000000 pg_tuna-0.1.0/src/pg_tuna/__init__.py
--rw-r--r--   0 delicj    (1002) delicj    (1002)    11378 2023-06-28 19:23:06.000000 pg_tuna-0.1.0/src/pg_tuna/wizard.py
-drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/src/pg_tuna.egg-info/
--rw-r--r--   0 delicj    (1002) delicj    (1002)     8078 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/PKG-INFO
--rw-r--r--   0 delicj    (1002) delicj    (1002)      337 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/SOURCES.txt
--rw-r--r--   0 delicj    (1002) delicj    (1002)        1 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/dependency_links.txt
--rw-r--r--   0 delicj    (1002) delicj    (1002)       48 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/entry_points.txt
--rw-r--r--   0 delicj    (1002) delicj    (1002)        1 2023-06-28 19:23:06.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/not-zip-safe
--rw-r--r--   0 delicj    (1002) delicj    (1002)       34 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/requires.txt
--rw-r--r--   0 delicj    (1002) delicj    (1002)        8 2023-06-29 10:51:36.000000 pg_tuna-0.1.0/src/pg_tuna.egg-info/top_level.txt
-drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:51:36.440325 pg_tuna-0.1.0/tests/
--rw-r--r--   0 delicj    (1002) delicj    (1002)     2805 2023-06-28 19:23:06.000000 pg_tuna-0.1.0/tests/test_tuna.py
+drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     1069 2023-06-28 19:22:48.000000 pg_tuna-0.1.1/LICENSE
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     4042 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/PKG-INFO
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     3473 2023-06-29 10:57:06.000000 pg_tuna-0.1.1/README.md
+-rw-r--r--   0 delicj    (1002) delicj    (1002)       38 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/setup.cfg
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     1031 2023-06-29 10:58:56.000000 pg_tuna-0.1.1/setup.py
+drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/src/
+drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/src/pg_tuna/
+-rw-r--r--   0 delicj    (1002) delicj    (1002)        2 2023-06-28 19:23:06.000000 pg_tuna-0.1.1/src/pg_tuna/__init__.py
+-rw-r--r--   0 delicj    (1002) delicj    (1002)    11378 2023-06-28 19:23:06.000000 pg_tuna-0.1.1/src/pg_tuna/wizard.py
+drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/src/pg_tuna.egg-info/
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     4042 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/PKG-INFO
+-rw-r--r--   0 delicj    (1002) delicj    (1002)      337 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/SOURCES.txt
+-rw-r--r--   0 delicj    (1002) delicj    (1002)        1 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/dependency_links.txt
+-rw-r--r--   0 delicj    (1002) delicj    (1002)       48 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/entry_points.txt
+-rw-r--r--   0 delicj    (1002) delicj    (1002)        1 2023-06-28 19:23:06.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/not-zip-safe
+-rw-r--r--   0 delicj    (1002) delicj    (1002)       34 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/requires.txt
+-rw-r--r--   0 delicj    (1002) delicj    (1002)        8 2023-06-29 10:59:10.000000 pg_tuna-0.1.1/src/pg_tuna.egg-info/top_level.txt
+drwxr-xr-x   0 delicj    (1002) delicj    (1002)        0 2023-06-29 10:59:10.562798 pg_tuna-0.1.1/tests/
+-rw-r--r--   0 delicj    (1002) delicj    (1002)     2805 2023-06-28 19:23:06.000000 pg_tuna-0.1.1/tests/test_tuna.py
```

### Comparing `pg_tuna-0.1.0/LICENSE` & `pg_tuna-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pg_tuna-0.1.0/setup.py` & `pg_tuna-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="pg_tuna",
-    version="0.1.0",
+    version="0.1.1",
     author="Josip Delic",
     description="pg_tuna",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/delijati/py-tuna",
     classifiers=[
         "Programming Language :: Python :: 3.6",
```

### Comparing `pg_tuna-0.1.0/src/pg_tuna/wizard.py` & `pg_tuna-0.1.1/src/pg_tuna/wizard.py`

 * *Files identical despite different names*

### Comparing `pg_tuna-0.1.0/tests/test_tuna.py` & `pg_tuna-0.1.1/tests/test_tuna.py`

 * *Files identical despite different names*

