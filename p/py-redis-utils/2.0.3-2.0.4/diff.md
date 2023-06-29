# Comparing `tmp/py-redis-utils-2.0.3.tar.gz` & `tmp/py-redis-utils-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-2.0.3.tar", last modified: Thu Jun 29 10:34:35 2023, max compression
+gzip compressed data, was "py-redis-utils-2.0.4.tar", last modified: Thu Jun 29 11:42:30 2023, max compression
```

## Comparing `py-redis-utils-2.0.3.tar` & `py-redis-utils-2.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/PKG-INFO
--rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.3/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/py_redis_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/pyredisutils/
--rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.3/pyredisutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     8848 2023-06-29 10:33:56.000000 py-redis-utils-2.0.3/pyredisutils/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)    15354 2023-06-29 10:12:06.000000 py-redis-utils-2.0.3/pyredisutils/_settings.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      787 2023-06-29 10:34:29.000000 py-redis-utils-2.0.3/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 11:42:30.478664 py-redis-utils-2.0.4/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 11:42:30.478664 py-redis-utils-2.0.4/PKG-INFO
+-rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.4/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 11:42:30.478664 py-redis-utils-2.0.4/py_redis_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 11:42:30.000000 py-redis-utils-2.0.4/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 11:42:30.000000 py-redis-utils-2.0.4/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 11:42:30.000000 py-redis-utils-2.0.4/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 11:42:30.000000 py-redis-utils-2.0.4/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 11:42:30.000000 py-redis-utils-2.0.4/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 11:42:30.478664 py-redis-utils-2.0.4/pyredisutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.4/pyredisutils/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     8809 2023-06-29 11:42:13.000000 py-redis-utils-2.0.4/pyredisutils/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)    15354 2023-06-29 10:12:06.000000 py-redis-utils-2.0.4/pyredisutils/_settings.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 11:42:30.478664 py-redis-utils-2.0.4/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      787 2023-06-29 11:42:13.000000 py-redis-utils-2.0.4/setup.py
```

### Comparing `py-redis-utils-2.0.3/README.md` & `py-redis-utils-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-2.0.3/pyredisutils/_decorators.py` & `py-redis-utils-2.0.4/pyredisutils/_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
                 redis_instance,
                 channel_name,
                 copy.deepcopy(publish_template),
                 copy.deepcopy(response_template),
                 copy.deepcopy(publish_changes),
                 copy.deepcopy(response_changes),
             )
-            settings.validate_redis()
 
             # Applies all necessary settings
             settings.get_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
```

### Comparing `py-redis-utils-2.0.3/pyredisutils/_settings.py` & `py-redis-utils-2.0.4/pyredisutils/_settings.py`

 * *Files identical despite different names*

### Comparing `py-redis-utils-2.0.3/setup.py` & `py-redis-utils-2.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "2.0.3"
+VERSION = "2.0.4"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

