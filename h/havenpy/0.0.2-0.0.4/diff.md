# Comparing `tmp/havenpy-0.0.2.tar.gz` & `tmp/havenpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "havenpy-0.0.2.tar", last modified: Thu Jun 29 14:27:41 2023, max compression
+gzip compressed data, was "havenpy-0.0.4.tar", last modified: Thu Jun 29 14:38:50 2023, max compression
```

## Comparing `havenpy-0.0.2.tar` & `havenpy-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:27:41.018148 havenpy-0.0.2/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:27:41.018024 havenpy-0.0.2/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-06 11:14:59.000000 havenpy-0.0.2/README.md
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:27:41.016824 havenpy-0.0.2/havenpy/
--rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-06 11:52:59.000000 havenpy-0.0.2/havenpy/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-07 11:20:36.000000 havenpy-0.0.2/havenpy/interceptor.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:27:41.017843 havenpy-0.0.2/havenpy/pb/
--rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-29 14:21:05.000000 havenpy-0.0.2/havenpy/pb/__init__.py
--rw-r--r--   0 konsti     (501) staff       (20)     4223 2023-06-29 14:21:05.000000 havenpy-0.0.2/havenpy/pb/manager_pb2.py
--rw-r--r--   0 konsti     (501) staff       (20)    13059 2023-06-29 14:21:05.000000 havenpy-0.0.2/havenpy/pb/manager_pb2_grpc.py
--rw-r--r--   0 konsti     (501) staff       (20)     2317 2023-06-29 07:31:37.000000 havenpy-0.0.2/havenpy/run.py
-drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:27:41.017519 havenpy-0.0.2/havenpy.egg-info/
--rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:27:40.000000 havenpy-0.0.2/havenpy.egg-info/PKG-INFO
--rw-r--r--   0 konsti     (501) staff       (20)      310 2023-06-29 14:27:41.000000 havenpy-0.0.2/havenpy.egg-info/SOURCES.txt
--rw-r--r--   0 konsti     (501) staff       (20)        1 2023-06-29 14:27:40.000000 havenpy-0.0.2/havenpy.egg-info/dependency_links.txt
--rw-r--r--   0 konsti     (501) staff       (20)       15 2023-06-29 14:27:40.000000 havenpy-0.0.2/havenpy.egg-info/requires.txt
--rw-r--r--   0 konsti     (501) staff       (20)        8 2023-06-29 14:27:40.000000 havenpy-0.0.2/havenpy.egg-info/top_level.txt
--rw-r--r--   0 konsti     (501) staff       (20)       38 2023-06-29 14:27:41.018188 havenpy-0.0.2/setup.cfg
--rw-r--r--   0 konsti     (501) staff       (20)      287 2023-06-29 14:27:32.000000 havenpy-0.0.2/setup.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.312173 havenpy-0.0.4/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:38:50.312052 havenpy-0.0.4/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-06 11:14:59.000000 havenpy-0.0.4/README.md
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.310522 havenpy-0.0.4/havenpy/
+-rw-r--r--   0 konsti     (501) staff       (20)       22 2023-06-06 11:52:59.000000 havenpy-0.0.4/havenpy/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2733 2023-06-07 11:20:36.000000 havenpy-0.0.4/havenpy/interceptor.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.311751 havenpy-0.0.4/havenpy/pb/
+-rw-r--r--   0 konsti     (501) staff       (20)        0 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/__init__.py
+-rw-r--r--   0 konsti     (501) staff       (20)     4223 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/manager_pb2.py
+-rw-r--r--   0 konsti     (501) staff       (20)    13059 2023-06-29 14:21:05.000000 havenpy-0.0.4/havenpy/pb/manager_pb2_grpc.py
+-rw-r--r--   0 konsti     (501) staff       (20)     2317 2023-06-29 07:31:37.000000 havenpy-0.0.4/havenpy/run.py
+drwxr-xr-x   0 konsti     (501) staff       (20)        0 2023-06-29 14:38:50.311331 havenpy-0.0.4/havenpy.egg-info/
+-rw-r--r--   0 konsti     (501) staff       (20)      135 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/PKG-INFO
+-rw-r--r--   0 konsti     (501) staff       (20)      310 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/SOURCES.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        1 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/dependency_links.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       32 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/requires.txt
+-rw-r--r--   0 konsti     (501) staff       (20)        8 2023-06-29 14:38:50.000000 havenpy-0.0.4/havenpy.egg-info/top_level.txt
+-rw-r--r--   0 konsti     (501) staff       (20)       38 2023-06-29 14:38:50.312213 havenpy-0.0.4/setup.cfg
+-rw-r--r--   0 konsti     (501) staff       (20)      314 2023-06-29 14:37:33.000000 havenpy-0.0.4/setup.py
```

### Comparing `havenpy-0.0.2/havenpy/interceptor.py` & `havenpy-0.0.4/havenpy/interceptor.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.2/havenpy/pb/manager_pb2.py` & `havenpy-0.0.4/havenpy/pb/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.2/havenpy/pb/manager_pb2_grpc.py` & `havenpy-0.0.4/havenpy/pb/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `havenpy-0.0.2/havenpy/run.py` & `havenpy-0.0.4/havenpy/run.py`

 * *Files identical despite different names*

