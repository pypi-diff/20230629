# Comparing `tmp/FOFA-py-2.0.1.tar.gz` & `tmp/FOFA-py-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FOFA-py-2.0.1.tar", last modified: Thu Jun 29 11:51:40 2023, max compression
+gzip compressed data, was "dist/FOFA-py-2.0.2.tar", last modified: Thu Jun 29 12:00:30 2023, max compression
```

## Comparing `FOFA-py-2.0.1.tar` & `FOFA-py-2.0.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 ntestoc    (501) staff       (20)        0 2023-06-29 11:51:40.553207 FOFA-py-2.0.1/
-drwxr-xr-x   0 ntestoc    (501) staff       (20)        0 2023-06-29 11:51:40.551457 FOFA-py-2.0.1/FOFA_py.egg-info/
--rw-r--r--   0 ntestoc    (501) staff       (20)     4320 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/PKG-INFO
--rw-r--r--   0 ntestoc    (501) staff       (20)      296 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/SOURCES.txt
--rw-r--r--   0 ntestoc    (501) staff       (20)        1 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/dependency_links.txt
--rw-r--r--   0 ntestoc    (501) staff       (20)       44 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/entry_points.txt
--rw-r--r--   0 ntestoc    (501) staff       (20)       53 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/requires.txt
--rw-r--r--   0 ntestoc    (501) staff       (20)        5 2023-06-29 11:51:40.000000 FOFA-py-2.0.1/FOFA_py.egg-info/top_level.txt
--rw-r--r--   0 ntestoc    (501) staff       (20)     1066 2023-06-21 03:06:48.000000 FOFA-py-2.0.1/LICENSE
--rw-r--r--   0 ntestoc    (501) staff       (20)     4320 2023-06-29 11:51:40.553067 FOFA-py-2.0.1/PKG-INFO
--rw-r--r--   0 ntestoc    (501) staff       (20)     1123 2023-06-29 11:43:52.000000 FOFA-py-2.0.1/README.md
-drwxr-xr-x   0 ntestoc    (501) staff       (20)        0 2023-06-29 11:51:40.552883 FOFA-py-2.0.1/fofa/
--rw-r--r--   0 ntestoc    (501) staff       (20)       68 2023-06-27 06:09:52.000000 FOFA-py-2.0.1/fofa/__init__.py
--rw-r--r--   0 ntestoc    (501) staff       (20)    11199 2023-06-29 02:37:43.000000 FOFA-py-2.0.1/fofa/__main__.py
--rw-r--r--   0 ntestoc    (501) staff       (20)    12189 2023-06-29 08:06:55.000000 FOFA-py-2.0.1/fofa/client.py
--rw-r--r--   0 ntestoc    (501) staff       (20)      710 2023-06-28 02:50:16.000000 FOFA-py-2.0.1/fofa/exception.py
--rw-r--r--   0 ntestoc    (501) staff       (20)     1400 2023-06-28 07:22:28.000000 FOFA-py-2.0.1/fofa/helper.py
--rw-r--r--   0 ntestoc    (501) staff       (20)       38 2023-06-29 11:51:40.553240 FOFA-py-2.0.1/setup.cfg
--rw-r--r--   0 ntestoc    (501) staff       (20)     1206 2023-06-29 08:54:21.000000 FOFA-py-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/FOFA_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/fofa/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/fofa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11199 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/fofa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12189 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/fofa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/fofa/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/fofa/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:00:30.000000 FOFA-py-2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-06-29 12:00:12.000000 FOFA-py-2.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `FOFA-py-2.0.1/README.md` & `FOFA-py-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FOFA-py-2.0.1/fofa/__main__.py` & `FOFA-py-2.0.2/fofa/__main__.py`

 * *Files identical despite different names*

### Comparing `FOFA-py-2.0.1/fofa/client.py` & `FOFA-py-2.0.2/fofa/client.py`

 * *Files identical despite different names*

### Comparing `FOFA-py-2.0.1/fofa/exception.py` & `FOFA-py-2.0.2/fofa/exception.py`

 * *Files identical despite different names*

### Comparing `FOFA-py-2.0.1/fofa/helper.py` & `FOFA-py-2.0.2/fofa/helper.py`

 * *Files identical despite different names*

### Comparing `FOFA-py-2.0.1/setup.py` & `FOFA-py-2.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 DEPENDENCIES = open('requirements.txt', 'r').read().split('\n')
 README = open('./docs/README_CN.md', 'r').read()
 
 
 setup(
     name = 'FOFA-py',
-    version = '2.0.1',
+    version = '2.0.2',
     description = 'Python library for FOFA (https://fofa.info)',
     long_description=README,
     long_description_content_type="text/markdown",
     author = 'Fofa',
     author_email = 'fofabot@baimaohui.net',
     url = 'https://github.com/fofapro/fofa-py',
     packages = ['fofa'],
```

