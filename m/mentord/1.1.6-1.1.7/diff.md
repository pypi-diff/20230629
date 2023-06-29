# Comparing `tmp/mentord-1.1.6.tar.gz` & `tmp/mentord-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.6.tar", last modified: Thu Jun 29 18:34:34 2023, max compression
+gzip compressed data, was "mentord-1.1.7.tar", last modified: Thu Jun 29 18:37:28 2023, max compression
```

## Comparing `mentord-1.1.6.tar` & `mentord-1.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.227107 mentord-1.1.6/
--rw-rw-rw-   0        0        0      685 2023-06-29 18:34:34.227107 mentord-1.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.213131 mentord-1.1.6/mentord/
--rw-rw-rw-   0        0        0      112 2023-06-29 18:20:54.000000 mentord-1.1.6/mentord/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.221616 mentord-1.1.6/mentord/classes/
--rw-rw-rw-   0        0        0      114 2023-06-29 18:09:36.000000 mentord-1.1.6/mentord/classes/__init__.py
--rw-rw-rw-   0        0        0     2019 2023-06-29 18:09:33.000000 mentord-1.1.6/mentord/classes/channel.py
--rw-rw-rw-   0        0        0     1309 2023-06-29 18:06:30.000000 mentord-1.1.6/mentord/classes/guild.py
--rw-rw-rw-   0        0        0      618 2023-06-29 18:07:07.000000 mentord-1.1.6/mentord/classes/member.py
--rw-rw-rw-   0        0        0     1431 2023-06-29 18:06:36.000000 mentord-1.1.6/mentord/classes/message.py
--rw-rw-rw-   0        0        0     2836 2023-06-29 18:09:19.000000 mentord-1.1.6/mentord/classes/user.py
--rw-rw-rw-   0        0        0      959 2023-06-29 18:23:13.000000 mentord-1.1.6/mentord/client.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.224611 mentord-1.1.6/mentord/events/
--rw-rw-rw-   0        0        0       54 2023-06-29 17:25:45.000000 mentord-1.1.6/mentord/events/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-06-29 18:08:05.000000 mentord-1.1.6/mentord/events/eon_message.py
--rw-rw-rw-   0        0        0     1375 2023-06-29 18:08:49.000000 mentord-1.1.6/mentord/events/eon_ready.py
--rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.6/mentord/httpc.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.226608 mentord-1.1.6/mentord/utils/
--rw-rw-rw-   0        0        0       28 2023-06-29 18:20:49.000000 mentord-1.1.6/mentord/utils/__init__.py
--rw-rw-rw-   0        0        0      772 2023-06-29 18:20:33.000000 mentord-1.1.6/mentord/utils/channel_opers.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:34:34.216624 mentord-1.1.6/mentord.egg-info/
--rw-rw-rw-   0        0        0      685 2023-06-29 18:34:34.000000 mentord-1.1.6/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-06-29 18:34:34.000000 mentord-1.1.6/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:34:34.000000 mentord-1.1.6/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2023-06-29 18:34:34.000000 mentord-1.1.6/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 18:34:34.228106 mentord-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      845 2023-06-29 18:34:33.000000 mentord-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.597506 mentord-1.1.7/
+-rw-rw-rw-   0        0        0      652 2023-06-29 18:37:28.597506 mentord-1.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.582530 mentord-1.1.7/mentord/
+-rw-rw-rw-   0        0        0      112 2023-06-29 18:20:54.000000 mentord-1.1.7/mentord/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.591516 mentord-1.1.7/mentord/classes/
+-rw-rw-rw-   0        0        0      114 2023-06-29 18:09:36.000000 mentord-1.1.7/mentord/classes/__init__.py
+-rw-rw-rw-   0        0        0     2019 2023-06-29 18:09:33.000000 mentord-1.1.7/mentord/classes/channel.py
+-rw-rw-rw-   0        0        0     1309 2023-06-29 18:06:30.000000 mentord-1.1.7/mentord/classes/guild.py
+-rw-rw-rw-   0        0        0      618 2023-06-29 18:07:07.000000 mentord-1.1.7/mentord/classes/member.py
+-rw-rw-rw-   0        0        0     1431 2023-06-29 18:06:36.000000 mentord-1.1.7/mentord/classes/message.py
+-rw-rw-rw-   0        0        0     2836 2023-06-29 18:09:19.000000 mentord-1.1.7/mentord/classes/user.py
+-rw-rw-rw-   0        0        0      959 2023-06-29 18:23:13.000000 mentord-1.1.7/mentord/client.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.594511 mentord-1.1.7/mentord/events/
+-rw-rw-rw-   0        0        0       54 2023-06-29 17:25:45.000000 mentord-1.1.7/mentord/events/__init__.py
+-rw-rw-rw-   0        0        0     2016 2023-06-29 18:08:05.000000 mentord-1.1.7/mentord/events/eon_message.py
+-rw-rw-rw-   0        0        0     1375 2023-06-29 18:08:49.000000 mentord-1.1.7/mentord/events/eon_ready.py
+-rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.7/mentord/httpc.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.596508 mentord-1.1.7/mentord/utils/
+-rw-rw-rw-   0        0        0       28 2023-06-29 18:20:49.000000 mentord-1.1.7/mentord/utils/__init__.py
+-rw-rw-rw-   0        0        0      772 2023-06-29 18:20:33.000000 mentord-1.1.7/mentord/utils/channel_opers.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:37:28.586025 mentord-1.1.7/mentord.egg-info/
+-rw-rw-rw-   0        0        0      652 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2023-06-29 18:37:28.000000 mentord-1.1.7/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:37:28.598505 mentord-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      812 2023-06-29 18:37:05.000000 mentord-1.1.7/setup.py
```

### Comparing `mentord-1.1.6/PKG-INFO` & `mentord-1.1.7/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-Metadata-Version: 2.1
-Name: mentord
-Version: 1.1.6
-Summary: A sync library for creating self bots in python!
-Description-Content-Type: text/markdown
-
+from setuptools import setup
 
+setup(
+    name="mentord",
+    version="1.1.7",
+    description="A sync library for creating self bots in python!",
+    packages=["mentord", "mentord/classes", "mentord/events", "mentord/utils"],
+    long_description_content_type="text/markdown",
+    long_description="""
 ### Example use:
 
 ```python
 from mentord import *
 
 User_client: Client = Client()
 User_client.connect(token='YOUR TOKEN')
 ```
 
 ### Use decorators:
 
 ```python
-@client.eon_ready.on_ready(client=User_client, delay=5.0)
+@on_ready(client=User_client, delay=5.0)
 def client_on_ready() -> None:
     print('Self-bot is started!')
 
-@client.eon_message.message(client=User_client, delay=0.5)
+@on_message(client=User_client, delay=0.5)
 def client_on_message(message: Message) -> None:
     utils.channel_opers.ChannelOperations(channel=message.channel_id, client=User_client).send_message("hello!")
-```
+```""",
+)
```

### Comparing `mentord-1.1.6/mentord/classes/channel.py` & `mentord-1.1.7/mentord/classes/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/classes/guild.py` & `mentord-1.1.7/mentord/classes/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/classes/member.py` & `mentord-1.1.7/mentord/classes/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/classes/message.py` & `mentord-1.1.7/mentord/classes/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/classes/user.py` & `mentord-1.1.7/mentord/classes/user.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/client.py` & `mentord-1.1.7/mentord/client.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/events/eon_message.py` & `mentord-1.1.7/mentord/events/eon_message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/events/eon_ready.py` & `mentord-1.1.7/mentord/events/eon_ready.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/httpc.py` & `mentord-1.1.7/mentord/httpc.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.6/mentord/utils/channel_opers.py` & `mentord-1.1.7/mentord/utils/channel_opers.py`

 * *Files identical despite different names*

