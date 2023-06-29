# Comparing `tmp/py-redis-utils-2.0.2.tar.gz` & `tmp/py-redis-utils-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-2.0.2.tar", last modified: Thu Jun 29 10:13:35 2023, max compression
+gzip compressed data, was "py-redis-utils-2.0.3.tar", last modified: Thu Jun 29 10:34:35 2023, max compression
```

## Comparing `py-redis-utils-2.0.2.tar` & `py-redis-utils-2.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:13:35.468664 py-redis-utils-2.0.2/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:13:35.468664 py-redis-utils-2.0.2/PKG-INFO
--rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.2/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:13:35.468664 py-redis-utils-2.0.2/py_redis_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:13:35.000000 py-redis-utils-2.0.2/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 10:13:35.000000 py-redis-utils-2.0.2/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 10:13:35.000000 py-redis-utils-2.0.2/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 10:13:35.000000 py-redis-utils-2.0.2/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 10:13:35.000000 py-redis-utils-2.0.2/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:13:35.468664 py-redis-utils-2.0.2/pyredisutils/
--rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.2/pyredisutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     8576 2023-06-29 09:07:59.000000 py-redis-utils-2.0.2/pyredisutils/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)    15354 2023-06-29 10:12:06.000000 py-redis-utils-2.0.2/pyredisutils/_settings.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 10:13:35.468664 py-redis-utils-2.0.2/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      787 2023-06-29 10:13:06.000000 py-redis-utils-2.0.2/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/PKG-INFO
+-rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.3/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/py_redis_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 10:34:35.000000 py-redis-utils-2.0.3/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/pyredisutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.3/pyredisutils/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     8848 2023-06-29 10:33:56.000000 py-redis-utils-2.0.3/pyredisutils/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)    15354 2023-06-29 10:12:06.000000 py-redis-utils-2.0.3/pyredisutils/_settings.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 10:34:35.928664 py-redis-utils-2.0.3/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      787 2023-06-29 10:34:29.000000 py-redis-utils-2.0.3/setup.py
```

### Comparing `py-redis-utils-2.0.2/README.md` & `py-redis-utils-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-2.0.2/pyredisutils/_decorators.py` & `py-redis-utils-2.0.3/pyredisutils/_decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,19 +56,22 @@
             settings.get_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
             settings.transform_response_template()
 
+            redis_response = settings.publish_message_to_redis()
             # Publishes message to Redis
-            if settings.publish_message_to_redis():
+            if redis_response == True:
                 settings.publish_template = None
                 settings.response_template = None
                 return org_function(*args, **kwargs)
+            elif redis_response != False:
+                return redis_response
             settings.publish_template = None
             settings.response_template = None
             logging.info("Redis response - Token is not valid")
             return settings.make_response("Unauthorized", 401)
 
         return authorize
 
@@ -125,16 +128,20 @@
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
             settings.transform_response_template()
 
             # Publishes message to Redis
-            if settings.publish_message_to_redis():
+            redis_response = settings.publish_message_to_redis()
+            if redis_response == True:
                 return org_function(*args, **kwargs)
+            elif redis_response != False:
+                return redis_response
+
             logging.info("Redis response - User does not has access")
             return settings.make_response("Forbidden", 403)
 
         return check
 
     return wrapper
```

### Comparing `py-redis-utils-2.0.2/pyredisutils/_settings.py` & `py-redis-utils-2.0.3/pyredisutils/_settings.py`

 * *Files identical despite different names*

### Comparing `py-redis-utils-2.0.2/setup.py` & `py-redis-utils-2.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "2.0.2"
+VERSION = "2.0.3"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

