# Comparing `tmp/aioredisorm-0.1.2.tar.gz` & `tmp/aioredisorm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioredisorm-0.1.2.tar", max compression
+gzip compressed data, was "aioredisorm-0.1.3.tar", max compression
```

## Comparing `aioredisorm-0.1.2.tar` & `aioredisorm-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1082 2023-06-27 15:42:37.968974 aioredisorm-0.1.2/LICENSE
--rw-r--r--   0        0        0     2487 2023-06-27 15:42:37.968974 aioredisorm-0.1.2/README.md
--rw-r--r--   0        0        0       49 2023-06-27 14:42:54.674318 aioredisorm-0.1.2/aioredisorm/__init__.py
--rw-r--r--   0        0        0     4413 2023-06-27 15:33:22.348494 aioredisorm-0.1.2/aioredisorm/aioredisorm.py
--rw-r--r--   0        0        0      643 2023-06-29 06:37:23.917174 aioredisorm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3367 2023-06-29 06:37:31.691780 aioredisorm-0.1.2/setup.py
--rw-r--r--   0        0        0     3094 2023-06-29 06:37:31.692093 aioredisorm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-27 15:42:37.968974 aioredisorm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2467 2023-06-29 06:40:46.480305 aioredisorm-0.1.3/README.md
+-rw-r--r--   0        0        0       49 2023-06-27 14:42:54.674318 aioredisorm-0.1.3/aioredisorm/__init__.py
+-rw-r--r--   0        0        0     4413 2023-06-27 15:33:22.348494 aioredisorm-0.1.3/aioredisorm/aioredisorm.py
+-rw-r--r--   0        0        0      643 2023-06-29 06:41:37.320610 aioredisorm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3345 2023-06-29 06:41:42.460194 aioredisorm-0.1.3/setup.py
+-rw-r--r--   0        0        0     3074 2023-06-29 06:41:42.460589 aioredisorm-0.1.3/PKG-INFO
```

### Comparing `aioredisorm-0.1.2/LICENSE` & `aioredisorm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aioredisorm-0.1.2/README.md` & `aioredisorm-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Here is an example that demonstrates the usage of the AIORedisORM class:
 
 ```python
 import asyncio
 from aioredisorm import AIORedisORM
 
 async def main():
+    # Add prefix to beging of each key
     redis_client = AIORedisORM(key_prefix='my_prefix')
     await redis_client.connect()
 
     # Set a value
     await redis_client.set_value('my_key', 'my_value', ex=12)
 
     # Get a value
@@ -40,17 +41,14 @@
     print(hash_result)  # Output: {b'key1': b'value1', b'key2': b'value2', b'key3': b'123'}
 
     await asyncio.sleep(5)  # Wait for the expiration to pass
 
     hash_result = await redis_client.get_hash('my_hash')
     print(hash_result)  # Output: {}
 
-    # Close the connection
-    await redis_client.close()
-
     # Decode the bytes to a string if needed
     result = result.decode('utf-8')
     print(result)  # Output: 'my_value'
 
     # Set a set
     await redis_client.set_set('my_set', 'value1', 'value2', 'value3')
```

### Comparing `aioredisorm-0.1.2/aioredisorm/aioredisorm.py` & `aioredisorm-0.1.3/aioredisorm/aioredisorm.py`

 * *Files identical despite different names*

### Comparing `aioredisorm-0.1.2/pyproject.toml` & `aioredisorm-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioredisorm"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python class for interacting with Redis using asyncio and aioredis."
 authors = ["fadedreams7 <fadedreams7@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.3"
```

### Comparing `aioredisorm-0.1.2/setup.py` & `aioredisorm-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['aioredis>=2.0.1,<3.0.0', 'asyncio>=3.4.3,<4.0.0']
 
 setup_kwargs = {
     'name': 'aioredisorm',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A Python class for interacting with Redis using asyncio and aioredis.',
-    'long_description': '## AIORedisORM\n\nA Python class for interacting with Redis using asyncio and aioredis.\n\n### Installation\n\nYou can install AIORedisORM using pip:\n\n```\npip install aioredisorm\n```\n\n### Example Usage\n\nHere is an example that demonstrates the usage of the AIORedisORM class:\n\n```python\nimport asyncio\nfrom aioredisorm import AIORedisORM\n\nasync def main():\n    redis_client = AIORedisORM(key_prefix=\'my_prefix\')\n    await redis_client.connect()\n\n    # Set a value\n    await redis_client.set_value(\'my_key\', \'my_value\', ex=12)\n\n    # Get a value\n    result = await redis_client.get_value(\'my_key\')\n    print(result)  # Output: b\'my_value\'\n\n    # Set a hash\n    await redis_client.set_hash(\'my_hash\', {\'key1\': \'value1\', \'key2\': \'value2\', \'key3\': 13})\n\n    # Set a hash with expiration\n    await redis_client.set_hash(\'my_hash\', {\'key1\': \'value1\', \'key2\': \'value2\', \'key3\': 13}, ex=5)\n\n    # Get a hash\n    hash_result = await redis_client.get_hash(\'my_hash\')\n    print(hash_result)  # Output: {b\'key1\': b\'value1\', b\'key2\': b\'value2\', b\'key3\': b\'123\'}\n\n    await asyncio.sleep(5)  # Wait for the expiration to pass\n\n    hash_result = await redis_client.get_hash(\'my_hash\')\n    print(hash_result)  # Output: {}\n\n    # Close the connection\n    await redis_client.close()\n\n    # Decode the bytes to a string if needed\n    result = result.decode(\'utf-8\')\n    print(result)  # Output: \'my_value\'\n\n    # Set a set\n    await redis_client.set_set(\'my_set\', \'value1\', \'value2\', \'value3\')\n\n    # Get a set\n    set_result = await redis_client.get_set(\'my_set\')\n    print("set_result", set_result)  # Output: {b\'value1\', b\'value2\', b\'value3\'}\n\n    # Transaction example\n    commands = [\n        (\'set\', \'key1\', \'value1\'),\n        (\'set\', \'key2\', \'value2\')\n    ]\n    results = await redis_client.execute_transaction(commands)\n    print(results)  # Output: [(True, True)]\n\n    # Set a list\n    await redis_client.set_list(\'my_list\', \'value1\', \'value2\', \'value3\')\n\n    # Get a list\n    list_result = await redis_client.get_list(\'my_list\')\n    print(list_result)  # Output: [b\'value1\', b\'value2\', b\'value3\']\n\n    # Get the expiration time of a key\n    ttl, pttl = await redis_client.get_key_expiration(\'key1\')\n    print(f"TTL of \'my_key\': {ttl} seconds")\n    print(f"PTTL of \'my_key\': {pttl} milliseconds")\n\n    # Close the connection\n    await redis_client.close()\n\n# Run the async example\nasyncio.run(main())\n```\n\nMake sure to import the AIORedisORM class and replace \'my_prefix\' with your desired key prefix.\n',
+    'long_description': '## AIORedisORM\n\nA Python class for interacting with Redis using asyncio and aioredis.\n\n### Installation\n\nYou can install AIORedisORM using pip:\n\n```\npip install aioredisorm\n```\n\n### Example Usage\n\nHere is an example that demonstrates the usage of the AIORedisORM class:\n\n```python\nimport asyncio\nfrom aioredisorm import AIORedisORM\n\nasync def main():\n    # Add prefix to beging of each key\n    redis_client = AIORedisORM(key_prefix=\'my_prefix\')\n    await redis_client.connect()\n\n    # Set a value\n    await redis_client.set_value(\'my_key\', \'my_value\', ex=12)\n\n    # Get a value\n    result = await redis_client.get_value(\'my_key\')\n    print(result)  # Output: b\'my_value\'\n\n    # Set a hash\n    await redis_client.set_hash(\'my_hash\', {\'key1\': \'value1\', \'key2\': \'value2\', \'key3\': 13})\n\n    # Set a hash with expiration\n    await redis_client.set_hash(\'my_hash\', {\'key1\': \'value1\', \'key2\': \'value2\', \'key3\': 13}, ex=5)\n\n    # Get a hash\n    hash_result = await redis_client.get_hash(\'my_hash\')\n    print(hash_result)  # Output: {b\'key1\': b\'value1\', b\'key2\': b\'value2\', b\'key3\': b\'123\'}\n\n    await asyncio.sleep(5)  # Wait for the expiration to pass\n\n    hash_result = await redis_client.get_hash(\'my_hash\')\n    print(hash_result)  # Output: {}\n\n    # Decode the bytes to a string if needed\n    result = result.decode(\'utf-8\')\n    print(result)  # Output: \'my_value\'\n\n    # Set a set\n    await redis_client.set_set(\'my_set\', \'value1\', \'value2\', \'value3\')\n\n    # Get a set\n    set_result = await redis_client.get_set(\'my_set\')\n    print("set_result", set_result)  # Output: {b\'value1\', b\'value2\', b\'value3\'}\n\n    # Transaction example\n    commands = [\n        (\'set\', \'key1\', \'value1\'),\n        (\'set\', \'key2\', \'value2\')\n    ]\n    results = await redis_client.execute_transaction(commands)\n    print(results)  # Output: [(True, True)]\n\n    # Set a list\n    await redis_client.set_list(\'my_list\', \'value1\', \'value2\', \'value3\')\n\n    # Get a list\n    list_result = await redis_client.get_list(\'my_list\')\n    print(list_result)  # Output: [b\'value1\', b\'value2\', b\'value3\']\n\n    # Get the expiration time of a key\n    ttl, pttl = await redis_client.get_key_expiration(\'key1\')\n    print(f"TTL of \'my_key\': {ttl} seconds")\n    print(f"PTTL of \'my_key\': {pttl} milliseconds")\n\n    # Close the connection\n    await redis_client.close()\n\n# Run the async example\nasyncio.run(main())\n```\n\nMake sure to import the AIORedisORM class and replace \'my_prefix\' with your desired key prefix.\n',
     'author': 'fadedreams7',
     'author_email': 'fadedreams7@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
     'packages': packages,
     'package_data': package_data,
```

### Comparing `aioredisorm-0.1.2/PKG-INFO` & `aioredisorm-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioredisorm
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python class for interacting with Redis using asyncio and aioredis.
 Author: fadedreams7
 Author-email: fadedreams7@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
@@ -31,14 +31,15 @@
 Here is an example that demonstrates the usage of the AIORedisORM class:
 
 ```python
 import asyncio
 from aioredisorm import AIORedisORM
 
 async def main():
+    # Add prefix to beging of each key
     redis_client = AIORedisORM(key_prefix='my_prefix')
     await redis_client.connect()
 
     # Set a value
     await redis_client.set_value('my_key', 'my_value', ex=12)
 
     # Get a value
@@ -56,17 +57,14 @@
     print(hash_result)  # Output: {b'key1': b'value1', b'key2': b'value2', b'key3': b'123'}
 
     await asyncio.sleep(5)  # Wait for the expiration to pass
 
     hash_result = await redis_client.get_hash('my_hash')
     print(hash_result)  # Output: {}
 
-    # Close the connection
-    await redis_client.close()
-
     # Decode the bytes to a string if needed
     result = result.decode('utf-8')
     print(result)  # Output: 'my_value'
 
     # Set a set
     await redis_client.set_set('my_set', 'value1', 'value2', 'value3')
```

