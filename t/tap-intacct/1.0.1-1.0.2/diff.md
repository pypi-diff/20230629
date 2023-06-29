# Comparing `tmp/tap-intacct-1.0.1.tar.gz` & `tmp/tap-intacct-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-intacct-1.0.1.tar", last modified: Fri Oct 23 15:13:25 2020, max compression
+gzip compressed data, was "tap-intacct-1.0.2.tar", last modified: Thu Jun 29 07:46:07 2023, max compression
```

## Comparing `tap-intacct-1.0.1.tar` & `tap-intacct-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       12 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      342 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      288 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct.egg-info/requires.txt
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/tap_intacct/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     7490 2020-10-23 15:04:49.000000 tap-intacct-1.0.1/tap_intacct/s3.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1956 2020-10-23 15:04:49.000000 tap-intacct-1.0.1/tap_intacct/__init__.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1968 2019-10-15 19:22:37.000000 tap-intacct-1.0.1/tap_intacct/sync.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     2408 2019-10-15 19:22:37.000000 tap-intacct-1.0.1/tap_intacct/conversion.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      850 2019-10-15 19:22:37.000000 tap-intacct-1.0.1/tap_intacct/discover.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      288 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      618 2020-10-23 15:13:15.000000 tap-intacct-1.0.1/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2020-10-23 15:13:25.000000 tap-intacct-1.0.1/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1215 2019-10-15 19:22:37.000000 tap-intacct-1.0.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 07:46:07.224390 tap-intacct-1.0.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32393 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-06-29 07:46:07.224390 tap-intacct-1.0.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1215 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-29 07:46:07.224390 tap-intacct-1.0.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      618 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 07:46:07.224390 tap-intacct-1.0.2/tap_intacct/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1956 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/tap_intacct/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2408 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/tap_intacct/conversion.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      850 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/tap_intacct/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7489 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/tap_intacct/s3.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1968 2023-06-29 06:29:12.000000 tap-intacct-1.0.2/tap_intacct/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-29 07:46:07.224390 tap-intacct-1.0.2/tap_intacct.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      232 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      350 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       74 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2023-06-29 07:46:07.000000 tap-intacct-1.0.2/tap_intacct.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-intacct-1.0.1/tap_intacct/s3.py` & `tap-intacct-1.0.2/tap_intacct/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     to_return = []
 
     path = config.get('path')
     company_id = config['company_id']
     prefix = str.join('/', [path, company_id]) if path else company_id
     s3_objects = list_files_in_bucket(bucket, prefix)
 
-    pattern = "^" + prefix + '/' + table_name + "\..*\.csv"
+    pattern = "^" + prefix + '/' + table_name + "\.*\.csv"
     matcher = re.compile(pattern)
 
     LOGGER.info(
         'Checking bucket "%s" for keys matching "%s"', bucket, pattern)
 
     matched_files = []
     for s3_object in s3_objects:
```

### Comparing `tap-intacct-1.0.1/tap_intacct/__init__.py` & `tap-intacct-1.0.2/tap_intacct/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-intacct-1.0.1/tap_intacct/sync.py` & `tap-intacct-1.0.2/tap_intacct/sync.py`

 * *Files identical despite different names*

### Comparing `tap-intacct-1.0.1/tap_intacct/conversion.py` & `tap-intacct-1.0.2/tap_intacct/conversion.py`

 * *Files identical despite different names*

### Comparing `tap-intacct-1.0.1/tap_intacct/discover.py` & `tap-intacct-1.0.2/tap_intacct/discover.py`

 * *Files identical despite different names*

### Comparing `tap-intacct-1.0.1/setup.py` & `tap-intacct-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 import subprocess
 
 setup(name="tap-intacct",
-      version='1.0.1',
+      version='1.0.2',
       description="Singer.io tap for extracting data from Intacct",
       author="Stitch",
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       url="http://singer.io",
       install_requires=[
           'singer-encodings==0.0.2',
           'singer-python==5.1.5',
```

### Comparing `tap-intacct-1.0.1/README.md` & `tap-intacct-1.0.2/README.md`

 * *Files identical despite different names*

