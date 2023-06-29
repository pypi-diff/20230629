# Comparing `tmp/aicoder-0.1.1.tar.gz` & `tmp/aicoder-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicoder-0.1.1.tar", last modified: Thu Jun 29 00:56:43 2023, max compression
+gzip compressed data, was "aicoder-0.1.2.tar", last modified: Thu Jun 29 11:02:58 2023, max compression
```

## Comparing `aicoder-0.1.1.tar` & `aicoder-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 00:56:43.725958 aicoder-0.1.1/
--rw-r--r--   0 carlospolop   (501) staff       (20)    18809 2023-06-29 00:13:10.000000 aicoder-0.1.1/LICENSE
--rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 00:56:43.725795 aicoder-0.1.1/PKG-INFO
--rw-r--r--   0 carlospolop   (501) staff       (20)      507 2023-06-29 00:52:18.000000 aicoder-0.1.1/README.md
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 00:56:43.724282 aicoder-0.1.1/aicoder/
--rw-r--r--   0 carlospolop   (501) staff       (20)    12624 2023-06-28 23:41:03.000000 aicoder-0.1.1/aicoder/AICoder.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     8120 2023-06-28 17:08:14.000000 aicoder-0.1.1/aicoder/AICoderFull.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     4803 2023-06-28 17:02:35.000000 aicoder-0.1.1/aicoder/AICoderPartial.py
--rw-r--r--   0 carlospolop   (501) staff       (20)     3481 2023-06-28 23:49:28.000000 aicoder-0.1.1/aicoder/AICoderPrompts.py
--rw-r--r--   0 carlospolop   (501) staff       (20)        0 2023-06-28 23:57:06.000000 aicoder-0.1.1/aicoder/__init__.py
-drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 00:56:43.725560 aicoder-0.1.1/aicoder.egg-info/
--rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/PKG-INFO
--rw-r--r--   0 carlospolop   (501) staff       (20)      328 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/SOURCES.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)        1 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/dependency_links.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       41 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/entry_points.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       39 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/requires.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)        8 2023-06-29 00:56:43.000000 aicoder-0.1.1/aicoder.egg-info/top_level.txt
--rw-r--r--   0 carlospolop   (501) staff       (20)       38 2023-06-29 00:56:43.726009 aicoder-0.1.1/setup.cfg
--rw-r--r--   0 carlospolop   (501) staff       (20)      684 2023-06-29 00:56:07.000000 aicoder-0.1.1/setup.py
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.419856 aicoder-0.1.2/
+-rw-r--r--   0 carlospolop   (501) staff       (20)    18809 2023-06-29 00:13:10.000000 aicoder-0.1.2/LICENSE
+-rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:02:58.419707 aicoder-0.1.2/PKG-INFO
+-rw-r--r--   0 carlospolop   (501) staff       (20)      507 2023-06-29 00:52:18.000000 aicoder-0.1.2/README.md
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.418267 aicoder-0.1.2/aicoder/
+-rw-r--r--   0 carlospolop   (501) staff       (20)    12624 2023-06-28 23:41:03.000000 aicoder-0.1.2/aicoder/AICoder.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     8120 2023-06-28 17:08:14.000000 aicoder-0.1.2/aicoder/AICoderFull.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     4803 2023-06-28 17:02:35.000000 aicoder-0.1.2/aicoder/AICoderPartial.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)     3481 2023-06-28 23:49:28.000000 aicoder-0.1.2/aicoder/AICoderPrompts.py
+-rw-r--r--   0 carlospolop   (501) staff       (20)        0 2023-06-28 23:57:06.000000 aicoder-0.1.2/aicoder/__init__.py
+drwxr-xr-x   0 carlospolop   (501) staff       (20)        0 2023-06-29 11:02:58.419457 aicoder-0.1.2/aicoder.egg-info/
+-rw-r--r--   0 carlospolop   (501) staff       (20)      359 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/PKG-INFO
+-rw-r--r--   0 carlospolop   (501) staff       (20)      328 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/SOURCES.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)        1 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/dependency_links.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       41 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/entry_points.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       39 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/requires.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)        8 2023-06-29 11:02:58.000000 aicoder-0.1.2/aicoder.egg-info/top_level.txt
+-rw-r--r--   0 carlospolop   (501) staff       (20)       38 2023-06-29 11:02:58.419909 aicoder-0.1.2/setup.cfg
+-rw-r--r--   0 carlospolop   (501) staff       (20)      731 2023-06-29 11:02:52.000000 aicoder-0.1.2/setup.py
```

### Comparing `aicoder-0.1.1/LICENSE` & `aicoder-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.1/aicoder/AICoder.py` & `aicoder-0.1.2/aicoder/AICoder.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.1/aicoder/AICoderFull.py` & `aicoder-0.1.2/aicoder/AICoderFull.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.1/aicoder/AICoderPartial.py` & `aicoder-0.1.2/aicoder/AICoderPartial.py`

 * *Files identical despite different names*

### Comparing `aicoder-0.1.1/aicoder/AICoderPrompts.py` & `aicoder-0.1.2/aicoder/AICoderPrompts.py`

 * *Files identical despite different names*

