# Comparing `tmp/kaiju_redis-2.1.0-py3-none-any.whl.zip` & `tmp/kaiju_redis-2.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8995 bytes, number of entries: 10
--rw-r--r--  2.0 unx      110 b- defN 23-Jun-27 19:32 kaiju_redis/__init__.py
--rw-r--r--  2.0 unx    14978 b- defN 23-Jun-27 19:32 kaiju_redis/services.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 19:32 kaiju_redis/tests/__init__.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jun-27 19:32 kaiju_redis/tests/fixtures.py
--rw-r--r--  2.0 unx     4086 b- defN 23-Jun-27 19:32 kaiju_redis/tests/test_redis.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3002 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      822 b- defN 23-Jun-27 19:32 kaiju_redis-2.1.0.dist-info/RECORD
-10 files, 26668 bytes uncompressed, 7585 bytes compressed:  71.6%
+Zip file size: 8989 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-29 12:21 kaiju_redis/__init__.py
+-rw-r--r--  2.0 unx    14924 b- defN 23-Jun-29 12:21 kaiju_redis/services.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 12:21 kaiju_redis/tests/__init__.py
+-rw-r--r--  2.0 unx     2956 b- defN 23-Jun-29 12:21 kaiju_redis/tests/fixtures.py
+-rw-r--r--  2.0 unx     4086 b- defN 23-Jun-29 12:21 kaiju_redis/tests/test_redis.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3002 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jun-29 12:22 kaiju_redis-2.1.1.dist-info/RECORD
+10 files, 26614 bytes uncompressed, 7579 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: kaiju_redis/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_redis/tests/test_redis.py
 Comment: 
 
-Filename: kaiju_redis-2.1.0.dist-info/LICENSE
+Filename: kaiju_redis-2.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_redis-2.1.0.dist-info/METADATA
+Filename: kaiju_redis-2.1.1.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_redis-2.1.0.dist-info/WHEEL
+Filename: kaiju_redis-2.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_redis-2.1.0.dist-info/top_level.txt
+Filename: kaiju_redis-2.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_redis-2.1.0.dist-info/RECORD
+Filename: kaiju_redis-2.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_redis/__init__.py

```diff
@@ -1,5 +1,5 @@
 from .services import *
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
```

## kaiju_redis/services.py

```diff
@@ -1,24 +1,22 @@
 """Redis services."""
 
 import textwrap
 from typing import Collection, FrozenSet, Type, List
 
-from kaiju_tools import NSKey
-from kaiju_tools.app import service_class_registry
-
 from coredis import Redis, RedisCluster  # noqa: pycharm
 from coredis.exceptions import ResponseError, StreamConsumerGroupError  # noqa: pycharm
 
-from kaiju_tools.app import ContextableService
+from kaiju_tools.app import ContextableService, service_class_registry
 from kaiju_tools.cache import BaseCacheService
 from kaiju_tools.encoding import msgpack_dumps, msgpack_loads
 from kaiju_tools.functions import retry
 from kaiju_tools.locks import BaseLocksService, NotLockOwnerError, LockExistsError
 from kaiju_tools.streams import StreamRPCClient, Listener
+from kaiju_tools.types import NSKey
 
 __all__ = ['RedisTransportService', 'RedisCacheService', 'RedisLocksService', 'RedisListener', 'RedisStreamRPCClient']
 
 
 class RedisTransportService(ContextableService):
     """Redis transport."""
 
@@ -417,25 +415,23 @@
     _transport: RedisTransportService
     _dumps = msgpack_dumps
 
     @classmethod
     def get_transport_cls(cls) -> Type:
         return RedisTransportService
 
-    async def write(self, body, headers: dict = None, key=None) -> None:
+    async def write(self, topic: NSKey, body, headers: dict = None, key=None) -> None:
         """Write data to the stream.
 
+        :param topic: topic key
         :param body: rpc request body
         :param headers: request headers
         :param key: (optional) message id
         """
-        msg = await self._transport.xadd(
-            self._topic, {b'_': self._dumps((body, headers))}, identifier=key if key else '*'
-        )
-        self.logger.debug('write: %s', msg)
+        await self._transport.xadd(topic, {b'_': self._dumps((body, headers))}, identifier=key if key else '*')
 
 
 service_class_registry.register_class(RedisTransportService)
 service_class_registry.register_class(RedisCacheService)
 service_class_registry.register_class(RedisLocksService)
 service_class_registry.register_class(RedisListener)
 service_class_registry.register_class(RedisStreamRPCClient)
```

## Comparing `kaiju_redis-2.1.0.dist-info/LICENSE` & `kaiju_redis-2.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_redis-2.1.0.dist-info/METADATA` & `kaiju_redis-2.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-redis
-Version: 2.1.0
+Version: 2.1.1
 Summary: Redis and keydb services
 Home-page: https://gitlab.com/kaiju-python/kaiju-redis
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

