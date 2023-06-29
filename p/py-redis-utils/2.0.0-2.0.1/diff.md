# Comparing `tmp/py-redis-utils-2.0.0.tar.gz` & `tmp/py-redis-utils-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-redis-utils-2.0.0.tar", last modified: Thu Jun 29 07:17:44 2023, max compression
+gzip compressed data, was "py-redis-utils-2.0.1.tar", last modified: Thu Jun 29 09:08:44 2023, max compression
```

## Comparing `py-redis-utils-2.0.0.tar` & `py-redis-utils-2.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.517042 py-redis-utils-2.0.0/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/PKG-INFO
--rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.0/README.md
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/py_redis_utils.egg-info/
--rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/PKG-INFO
--rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/SOURCES.txt
--rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/dependency_links.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/requires.txt
--rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 07:17:44.000000 py-redis-utils-2.0.0/py_redis_utils.egg-info/top_level.txt
-drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 07:17:44.507042 py-redis-utils-2.0.0/pyredisutils/
--rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.0/pyredisutils/__init__.py
--rw-r--r--   0 erne      (1000) erne      (1000)     8535 2023-06-28 11:32:15.000000 py-redis-utils-2.0.0/pyredisutils/_decorators.py
--rw-r--r--   0 erne      (1000) erne      (1000)    14750 2023-06-29 07:17:11.000000 py-redis-utils-2.0.0/pyredisutils/_settings.py
--rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 07:17:44.517042 py-redis-utils-2.0.0/setup.cfg
--rw-r--r--   0 erne      (1000) erne      (1000)      786 2023-06-29 07:17:11.000000 py-redis-utils-2.0.0/setup.py
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 09:08:44.875553 py-redis-utils-2.0.1/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 09:08:44.875553 py-redis-utils-2.0.1/PKG-INFO
+-rwxrwxrwx   0 erne      (1000) erne      (1000)     1361 2023-02-03 14:24:27.000000 py-redis-utils-2.0.1/README.md
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 09:08:44.875553 py-redis-utils-2.0.1/py_redis_utils.egg-info/
+-rw-r--r--   0 erne      (1000) erne      (1000)      480 2023-06-29 09:08:44.000000 py-redis-utils-2.0.1/py_redis_utils.egg-info/PKG-INFO
+-rw-r--r--   0 erne      (1000) erne      (1000)      286 2023-06-29 09:08:44.000000 py-redis-utils-2.0.1/py_redis_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)        1 2023-06-29 09:08:44.000000 py-redis-utils-2.0.1/py_redis_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       63 2023-06-29 09:08:44.000000 py-redis-utils-2.0.1/py_redis_utils.egg-info/requires.txt
+-rw-r--r--   0 erne      (1000) erne      (1000)       13 2023-06-29 09:08:44.000000 py-redis-utils-2.0.1/py_redis_utils.egg-info/top_level.txt
+drwxr-xr-x   0 erne      (1000) erne      (1000)        0 2023-06-29 09:08:44.875553 py-redis-utils-2.0.1/pyredisutils/
+-rw-r--r--   0 erne      (1000) erne      (1000)       65 2023-06-28 11:32:15.000000 py-redis-utils-2.0.1/pyredisutils/__init__.py
+-rw-r--r--   0 erne      (1000) erne      (1000)     8576 2023-06-29 09:07:59.000000 py-redis-utils-2.0.1/pyredisutils/_decorators.py
+-rw-r--r--   0 erne      (1000) erne      (1000)    15354 2023-06-29 09:07:59.000000 py-redis-utils-2.0.1/pyredisutils/_settings.py
+-rw-r--r--   0 erne      (1000) erne      (1000)       38 2023-06-29 09:08:44.875553 py-redis-utils-2.0.1/setup.cfg
+-rw-r--r--   0 erne      (1000) erne      (1000)      787 2023-06-29 09:08:42.000000 py-redis-utils-2.0.1/setup.py
```

### Comparing `py-redis-utils-2.0.0/README.md` & `py-redis-utils-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py-redis-utils-2.0.0/pyredisutils/_decorators.py` & `py-redis-utils-2.0.1/pyredisutils/_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,26 +34,27 @@
     is the old value that should be changed, and the second is the value to which it will be changed.
     :param response_changes: Field that contains custom replaceable values for response message. It should be List of Lists *List[List]*.
     For example, you should pass this kind of list -  [["FIRST", "SECOND"], ["ABC", "QWE"]], and the decorator will look for value "FIRST" and change it to the
     "SECOND", as well as will look for value "ABC" and will change it to the "QWE". In that way, your list should contain lists with two parameters, where first
     is the old value that should be changed, and the second is the value to which it will be changed.
     :return: Returns nothing if Redis returned Successful message, and will return Flask Response *Any | Tuple[Any, int]* if Any error occurred.
     """
+
     def funct_decorator(org_function):
         @wraps(org_function)
         def authorize(*args, **kwargs):
-
             settings = Settings(
                 redis_instance,
                 channel_name,
                 copy.deepcopy(publish_template),
                 copy.deepcopy(response_template),
                 copy.deepcopy(publish_changes),
                 copy.deepcopy(response_changes),
             )
+            settings.validate_redis()
 
             # Applies all necessary settings
             settings.get_token()
             settings.generate_id()
             settings.update_publish_replaces()
             settings.update_response_replaces()
             settings.transform_publish_template()
@@ -100,18 +101,18 @@
     is the old value that should be changed, and the second is the value to which it will be changed.
     :param response_changes: Field that contains custom replaceable values for response message. It should be List of Lists *List[List]*.
     For example, you should pass this kind of list -  [["FIRST", "SECOND"], ["ABC", "QWE"]], and the decorator will look for value "FIRST" and change it to the
     "SECOND", as well as will look for value "ABC" and will change it to the "QWE". In that way, your list should contain lists with two parameters, where first
     is the old value that should be changed, and the second is the value to which it will be changed.
     :return: Returns nothing if Redis returned Successful message, and will return Flask Response *Any | Tuple[Any, int]* if Any error occurred.
     """
+
     def wrapper(org_function):
         @wraps(org_function)
         def check(*args, **kwargs):
-
             settings = Settings(
                 redis_instance,
                 channel_name,
                 copy.deepcopy(publish_template),
                 copy.deepcopy(response_template),
                 copy.deepcopy(publish_changes),
                 copy.deepcopy(response_changes),
@@ -132,7 +133,8 @@
                 return org_function(*args, **kwargs)
             logging.info("Redis response - User does not has access")
             return settings.make_response("Forbidden", 403)
 
         return check
 
     return wrapper
+
```

### Comparing `py-redis-utils-2.0.0/pyredisutils/_settings.py` & `py-redis-utils-2.0.1/pyredisutils/_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         """
         Return Redis instance.
         :return: Redis instance
         """
         return self._redis_instance
 
     @redis_instance.setter
-    def redis_instance(self, v: redis) -> None:
+    def redis_instance(self, v: redis):
         """
         Set Redis instance.
         :param v: Redis instance.
         :return: None
         """
         self._redis_instance = v
 
@@ -362,37 +362,42 @@
                         key: self._transform_redis_response(value)
                         for key, value in message.items()
                     }
                     if redis_response["type"] != "message":
                         continue
                     diff = deepdiff.DeepDiff(self.response_template, redis_response)
                     if diff == {}:
-                        return self._redis_close(
-                            pubsub, redis_client, True
-                        )
+                        return self._redis_close(pubsub, redis_client, True)
                     values = diff.get("values_changed", {})
                     if all(
-                            change["old_value"] != self.request_id
-                            for change in values.values()
+                        change["old_value"] != self.request_id
+                        for change in values.values()
                     ):
-                        return self._redis_close(
-                            pubsub, redis_client, False
-                        )
+                        return self._redis_close(pubsub, redis_client, False)
             except TimeoutError:
                 logging.error("Haven't received any answer from Redis for 5 seconds.")
                 pubsub.unsubscribe(f"{self.channel_name}.reply")
                 redis_client.close()
                 return self.make_response("Gateway Timeout", 504)
         except redis.exceptions.ConnectionError:
             return self.make_response("Bad Gateway", 502)
 
-    def _redis_close(self, pubsub, redis_client, arg2):
+    def _redis_close(
+        self, pubsub: redis.client.pubsub, redis_client: redis, return_value: Any
+    ):
+        """
+        Private method to gracefully close redis, unsubscribe and return desired value
+        :param pubsub:  instance of redis.pubsub
+        :param redis_client:  instance to redis
+        :param return_value: any value which needs to be returned after closing redis
+        :return:
+        """
         pubsub.unsubscribe(f"{self.channel_name}.reply")
         redis_client.close()
-        return arg2
+        return return_value
 
     @classmethod
     def _transform_dict(cls, data: Dict, change_fields: List[List]) -> Dict:
         """
         Method to dynamically transform dictionary.
         Method finds value that should be replaced, and replaces them.
         :param data: Initial dictionary that should be transformed.
@@ -447,7 +452,16 @@
                         "message": message,
                         "statusCode": status_code,
                     }
                 )
             ),
             status_code,
         )
+
+    def validate_redis(self) -> Tuple[Response, int]:
+        """
+        Method to validate if redis is reachable or not
+        :return:
+        """
+        if not (response := self.redis_instance.ping()):
+            logging.error(f"Redis server is not responding: {response}")
+            return self.make_response("Redis timeout", 504)
```

