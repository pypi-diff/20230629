# Comparing `tmp/test-proto-0.0.2.tar.gz` & `tmp/test-proto-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-proto-0.0.2.tar", last modified: Thu Jun 29 20:43:25 2023, max compression
+gzip compressed data, was "test-proto-0.0.3.tar", last modified: Thu Jun 29 21:18:00 2023, max compression
```

## Comparing `test-proto-0.0.2.tar` & `test-proto-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,16 @@
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 20:43:25.118265 test-proto-0.0.2/
--rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-29 20:43:25.118150 test-proto-0.0.2/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)      448 2023-06-29 20:43:22.000000 test-proto-0.0.2/pyproject.toml
--rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-29 20:43:25.118297 test-proto-0.0.2/setup.cfg
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 20:43:25.117995 test-proto-0.0.2/test_proto.egg-info/
--rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)      150 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/SOURCES.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/dependency_links.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/top_level.txt
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.711748 test-proto-0.0.3/
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1061 2023-06-29 21:09:14.000000 test-proto-0.0.3/LICENSE.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:18:00.711646 test-proto-0.0.3/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-28 15:00:54.000000 test-proto-0.0.3/README.md
+-rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-29 21:18:00.711778 test-proto-0.0.3/setup.cfg
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1660 2023-06-29 21:17:14.000000 test-proto-0.0.3/setup.py
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.710916 test-proto-0.0.3/test-proto/
+-rw-r--r--   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/__init__.py
+-rw-r--r--   0 moadwdev   (501) staff       (20)     1928 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/users_pb2.py
+-rw-r--r--   0 moadwdev   (501) staff       (20)     5366 2023-06-29 21:18:00.000000 test-proto-0.0.3/test-proto/users_pb2_grpc.py
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 21:18:00.711473 test-proto-0.0.3/test_proto.egg-info/
+-rw-r--r--   0 moadwdev   (501) staff       (20)      724 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)      275 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)       29 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/requires.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)       11 2023-06-29 21:18:00.000000 test-proto-0.0.3/test_proto.egg-info/top_level.txt
```

