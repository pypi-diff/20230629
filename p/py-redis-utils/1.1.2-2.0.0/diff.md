# Comparing `tmp/py-redis-utils-1.1.2.tar.gz` & `tmp/py-redis-utils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-1.1.2.tar", last modified: Wed Jun 28 11:48:05 2023, max compression
+gzip compressed data, was "py-redis-utils-2.0.0.tar", last modified: Thu Jun 29 07:17:44 2023, max compression
```

## Comparing `py-redis-utils-1.1.2.tar` & `py-redis-utils-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 11:48:05.065652 py-redis-utils-1.1.2/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-28 11:48:05.065652 py-redis-utils-1.1.2/PKG-INFO
--rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-1.1.2/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 11:48:05.065652 py-redis-utils-1.1.2/py_redis_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-28 11:48:04.000000 py-redis-utils-1.1.2/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-28 11:48:04.000000 py-redis-utils-1.1.2/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-28 11:48:04.000000 py-redis-utils-1.1.2/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-28 11:48:04.000000 py-redis-utils-1.1.2/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-28 11:48:04.000000 py-redis-utils-1.1.2/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-28 11:48:05.065652 py-redis-utils-1.1.2/pyredisutils/
--rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-1.1.2/pyredisutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     8535 2023-06-28 11:32:15.000000 py-redis-utils-1.1.2/pyredisutils/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)    14393 2023-06-28 11:46:46.000000 py-redis-utils-1.1.2/pyredisutils/_settings.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-28 11:48:05.065652 py-redis-utils-1.1.2/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      786 2023-06-28 11:47:23.000000 py-redis-utils-1.1.2/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.517042 py-redis-utils-2.0.0/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/PKG-INFO
+-rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.0/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/py_redis_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/pyredisutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.0/pyredisutils/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     8535 2023-06-28 11:32:15.000000 py-redis-utils-2.0.0/pyredisutils/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)    14750 2023-06-29 07:17:11.000000 py-redis-utils-2.0.0/pyredisutils/_settings.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 07:17:44.517042 py-redis-utils-2.0.0/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      786 2023-06-29 07:17:11.000000 py-redis-utils-2.0.0/setup.py
```

### Comparing `py-redis-utils-1.1.2/README.md` & `py-redis-utils-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.1.2/pyredisutils/_decorators.py` & `py-redis-utils-2.0.0/pyredisutils/_decorators.py`

 * *Files identical despite different names*

### Comparing `py-redis-utils-1.1.2/pyredisutils/_settings.py` & `py-redis-utils-2.0.0/pyredisutils/_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,33 +358,42 @@
                         raise TimeoutError
                     if not (message := pubsub.get_message(timeout=timeout)):
                         raise TimeoutError
                     redis_response = {
                         key: self._transform_redis_response(value)
                         for key, value in message.items()
                     }
+                    if redis_response["type"] != "message":
+                        continue
                     diff = deepdiff.DeepDiff(self.response_template, redis_response)
                     if diff == {}:
-                        pubsub.unsubscribe(f"{self.channel_name}.reply")
-                        redis_client.close()
-                        return True
+                        return self._redis_close(
+                            pubsub, redis_client, True
+                        )
                     values = diff.get("values_changed", {})
                     if all(
                             change["old_value"] != self.request_id
                             for change in values.values()
                     ):
-                        redis_client.close()
-                        return False
+                        return self._redis_close(
+                            pubsub, redis_client, False
+                        )
             except TimeoutError:
                 logging.error("Haven't received any answer from Redis for 5 seconds.")
+                pubsub.unsubscribe(f"{self.channel_name}.reply")
                 redis_client.close()
                 return self.make_response("Gateway Timeout", 504)
         except redis.exceptions.ConnectionError:
             return self.make_response("Bad Gateway", 502)
 
+    def _redis_close(self, pubsub, redis_client, arg2):
+        pubsub.unsubscribe(f"{self.channel_name}.reply")
+        redis_client.close()
+        return arg2
+
     @classmethod
     def _transform_dict(cls, data: Dict, change_fields: List[List]) -> Dict:
         """
         Method to dynamically transform dictionary.
         Method finds value that should be replaced, and replaces them.
         :param data: Initial dictionary that should be transformed.
         :param change_fields: List of lists, where contains data that should be changed.
```

### Comparing `py-redis-utils-1.1.2/setup.py` & `py-redis-utils-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "1.1.2"
+VERSION = "2.0.0"
 DESCRIPTION = "Utilities with Redis"
 
 # Setting up
 setup(
     name="py-redis-utils",
     version=VERSION,
     author="KE",
```

