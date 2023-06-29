# Comparing `tmp/racetime-bot-1.9.0.tar.gz` & `tmp/racetime-bot-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racetime-bot-1.9.0.tar", last modified: Thu Feb 17 09:39:34 2022, max compression
+gzip compressed data, was "racetime-bot-2.0.0.tar", last modified: Thu Jun 29 16:25:30 2023, max compression
```

## Comparing `racetime-bot-1.9.0.tar` & `racetime-bot-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:39:34.010157 racetime-bot-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-02-17 09:39:34.010157 racetime-bot-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1749 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:39:34.010157 racetime-bot-1.9.0/racetime_bot/
--rw-r--r--   0 runner    (1001) docker     (121)     1894 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/racetime_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8650 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/racetime_bot/bot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11348 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/racetime_bot/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-17 09:39:34.010157 racetime-bot-1.9.0/racetime_bot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      604 2022-02-17 09:39:33.000000 racetime-bot-1.9.0/racetime_bot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-02-17 09:39:33.000000 racetime-bot-1.9.0/racetime_bot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-17 09:39:33.000000 racetime-bot-1.9.0/racetime_bot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-02-17 09:39:33.000000 racetime-bot-1.9.0/racetime_bot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-17 09:39:33.000000 racetime-bot-1.9.0/racetime_bot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-17 09:39:34.010157 racetime-bot-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-02-17 09:39:12.000000 racetime-bot-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:25:30.288225 racetime-bot-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-29 16:25:30.288225 racetime-bot-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:25:30.288225 racetime-bot-2.0.0/racetime_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/racetime_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/racetime_bot/bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11424 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/racetime_bot/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:25:30.288225 racetime-bot-2.0.0/racetime_bot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-29 16:25:30.000000 racetime-bot-2.0.0/racetime_bot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-29 16:25:30.000000 racetime-bot-2.0.0/racetime_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:25:30.000000 racetime-bot-2.0.0/racetime_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-29 16:25:30.000000 racetime-bot-2.0.0/racetime_bot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 16:25:30.000000 racetime-bot-2.0.0/racetime_bot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:25:30.288225 racetime-bot-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-29 16:25:17.000000 racetime-bot-2.0.0/setup.py
```

### Comparing `racetime-bot-1.9.0/LICENSE` & `racetime-bot-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `racetime-bot-1.9.0/PKG-INFO` & `racetime-bot-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 Metadata-Version: 2.1
 Name: racetime-bot
-Version: 1.9.0
+Version: 2.0.0
 Summary: Foundation system for creating chat bots for racetime.gg
 Home-page: https://github.com/racetimeGG/racetime-bot
 License: MIT
 Project-URL: Source, https://github.com/racetimeGG/racetime-bot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `racetime-bot-1.9.0/README.md` & `racetime-bot-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `racetime-bot-1.9.0/racetime_bot/__init__.py` & `racetime-bot-2.0.0/racetime_bot/__init__.py`

 * *Files identical despite different names*

### Comparing `racetime-bot-1.9.0/racetime_bot/bot.py` & `racetime-bot-2.0.0/racetime_bot/bot.py`

 * *Files identical despite different names*

### Comparing `racetime-bot-1.9.0/racetime_bot/handler.py` & `racetime-bot-2.0.0/racetime_bot/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         self.conn = conn
         self.data = {}
         self.logger = logger
         self.state = state
         self.command_prefix = command_prefix
         self.ws = None
 
-    def should_stop(self):
+    async def should_stop(self):
         """
         Determine if the handler should be terminated. This is checked after
         every receieved message.
 
         By default, checks if the race state matches one of the values in
         `stop_at`.
         """
@@ -345,14 +345,16 @@
         processing any messages that come in.
         """
         self.logger.info('[%(race)s] Handler started' % {
             'race': self.data.get('name'),
         })
         async with self.conn as ws:
             self.ws = ws
+            if await self.should_stop():
+                return
             await self.begin()
             async for message in self.ws:
                 data = json.loads(message)
                 await self.consume(data)
-                if self.should_stop():
+                if await self.should_stop():
                     await self.end()
                     break
```

### Comparing `racetime-bot-1.9.0/racetime_bot.egg-info/PKG-INFO` & `racetime-bot-2.0.0/racetime_bot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 Metadata-Version: 2.1
 Name: racetime-bot
-Version: 1.9.0
+Version: 2.0.0
 Summary: Foundation system for creating chat bots for racetime.gg
 Home-page: https://github.com/racetimeGG/racetime-bot
 License: MIT
 Project-URL: Source, https://github.com/racetimeGG/racetime-bot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `racetime-bot-1.9.0/setup.py` & `racetime-bot-2.0.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     url='https://github.com/racetimeGG/racetime-bot',
     project_urls={
         'Source': 'https://github.com/racetimeGG/racetime-bot',
     },
-    version='1.9.0',
+    version='2.0.0',
     install_requires=[
         'aiohttp',
         'asgiref',
         'requests',
         'websockets',
     ],
     packages=find_packages(),
```

