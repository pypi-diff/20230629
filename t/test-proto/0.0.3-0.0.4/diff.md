# Comparing `tmp/test-proto-0.0.3.tar.gz` & `tmp/test_proto-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-proto-0.0.3.tar", last modified: Thu Jun 29 21:18:00 2023, max compression
+gzip compressed data, was "test_proto-0.0.4.tar", last modified: Thu Jun 29 21:28:23 2023, max compression
```

## Comparing `test-proto-0.0.3.tar` & `test_proto-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.711748 test-proto-0.0.3/
--rw-r--r--   0 moadwdev   (501) staff       (20)     1061 2023-06-29 21:09:14.000000 test-proto-0.0.3/LICENSE.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:18:00.711646 test-proto-0.0.3/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-28 15:00:54.000000 test-proto-0.0.3/README.md
--rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-29 21:18:00.711778 test-proto-0.0.3/setup.cfg
--rw-r--r--   0 moadwdev   (501) staff       (20)     1660 2023-06-29 21:17:14.000000 test-proto-0.0.3/setup.py
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.710916 test-proto-0.0.3/test-proto/
--rw-r--r--   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/__init__.py
--rw-r--r--   0 moadwdev   (501) staff       (20)     1928 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/users_pb2.py
--rw-r--r--   0 moadwdev   (501) staff       (20)     5366 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/users_pb2_grpc.py
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.711473 test-proto-0.0.3/test_proto.egg-info/
--rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)      275 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/SOURCES.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/dependency_links.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)       29 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/requires.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)       11 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/top_level.txt
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:28:23.734028 test_proto-0.0.4/
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1061 2023-06-29 21:09:14.000000 test_proto-0.0.4/LICENSE.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:28:23.733922 test_proto-0.0.4/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-28 15:00:54.000000 test_proto-0.0.4/README.md
+-rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-29 21:28:23.734059 test_proto-0.0.4/setup.cfg
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1660 2023-06-29 21:27:52.000000 test_proto-0.0.4/setup.py
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:28:23.733165 test_proto-0.0.4/test_proto/
+-rw-r--r--   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto/__init__.py
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1928 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto/users_pb2.py
+-rw-r--r--   0 moadwdev   (501) staff       (20)     5366 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto/users_pb2_grpc.py
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:28:23.733749 test_proto-0.0.4/test_proto.egg-info/
+-rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto.egg-info/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)      275 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)       29 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto.egg-info/requires.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)       11 2023-06-29 21:28:23.000000 test_proto-0.0.4/test_proto.egg-info/top_level.txt
```

### Comparing `test-proto-0.0.3/LICENSE.txt` & `test_proto-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `test-proto-0.0.3/PKG-INFO` & `test_proto-0.0.4/test_proto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-proto
-Version: 0.0.3
+Version: 0.0.4
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

### Comparing `test-proto-0.0.3/setup.py` & `test_proto-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
-  name = 'test-proto',         # How you named your package folder (MyLib)
-  packages = ['test-proto'],   # Chose the same as "name"
-  version = '0.0.3',      # Start with a small number and increase it with every change you make
+  name = 'test_proto',         # How you named your package folder (MyLib)
+  packages = ['test_proto'],   # Chose the same as "name"
+  version = '0.0.4',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'TYPE YOUR DESCRIPTION HERE',   # Give a short description about your library
   author = 'YOUR NAME',                   # Type in your name
   author_email = 'your.email@domain.com',      # Type in your E-Mail
   url = 'https://github.com/user/reponame',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/user/reponame/archive/v_01.tar.gz',    # I explain this later on
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   # Keywords that define your package best
```

### Comparing `test-proto-0.0.3/test-proto/users_pb2.py` & `test_proto-0.0.4/test_proto/users_pb2.py`

 * *Files identical despite different names*

### Comparing `test-proto-0.0.3/test-proto/users_pb2_grpc.py` & `test_proto-0.0.4/test_proto/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `test-proto-0.0.3/test_proto.egg-info/PKG-INFO` & `test_proto-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: test-proto
-Version: 0.0.3
+Name: test_proto
+Version: 0.0.4
 Summary: TYPE YOUR DESCRIPTION HERE
 Home-page: https://github.com/user/reponame
 Download-URL: https://github.com/user/reponame/archive/v_01.tar.gz
 Author: YOUR NAME
 Author-email: your.email@domain.com
 License: MIT
 Keywords: SOME,MEANINGFULL,KEYWORDS
```

