# Comparing `tmp/test-proto-0.0.1.tar.gz` & `tmp/test-proto-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-proto-0.0.1.tar", last modified: Wed Jun 28 17:13:25 2023, max compression
+gzip compressed data, was "test-proto-0.0.2.tar", last modified: Thu Jun 29 20:43:25 2023, max compression
```

## Comparing `test-proto-0.0.1.tar` & `test-proto-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-28 17:13:25.796470 test-proto-0.0.1/
--rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-28 17:13:25.796360 test-proto-0.0.1/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)      448 2023-06-28 17:13:22.000000 test-proto-0.0.1/pyproject.toml
--rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-28 17:13:25.796501 test-proto-0.0.1/setup.cfg
-drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-28 17:13:25.796221 test-proto-0.0.1/test_proto.egg-info/
--rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-28 17:13:25.000000 test-proto-0.0.1/test_proto.egg-info/PKG-INFO
--rw-r--r--   0 moadwdev   (501) staff       (20)      150 2023-06-28 17:13:25.000000 test-proto-0.0.1/test_proto.egg-info/SOURCES.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-28 17:13:25.000000 test-proto-0.0.1/test_proto.egg-info/dependency_links.txt
--rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-28 17:13:25.000000 test-proto-0.0.1/test_proto.egg-info/top_level.txt
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 20:43:25.118265 test-proto-0.0.2/
+-rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-29 20:43:25.118150 test-proto-0.0.2/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)      448 2023-06-29 20:43:22.000000 test-proto-0.0.2/pyproject.toml
+-rw-r--r--   0 moadwdev   (501) staff       (20)       38 2023-06-29 20:43:25.118297 test-proto-0.0.2/setup.cfg
+drwxr-xr-x   0 moadwdev   (501) staff       (20)        0 2023-06-29 20:43:25.117995 test-proto-0.0.2/test_proto.egg-info/
+-rw-r--r--   0 moadwdev   (501) staff       (20)      304 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/PKG-INFO
+-rw-r--r--   0 moadwdev   (501) staff       (20)      150 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 moadwdev   (501) staff       (20)        1 2023-06-29 20:43:25.000000 test-proto-0.0.2/test_proto.egg-info/top_level.txt
```

