# Comparing `tmp/mentord-1.1.4.tar.gz` & `tmp/mentord-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.4.tar", last modified: Thu Jun 29 09:14:18 2023, max compression
+gzip compressed data, was "mentord-1.1.5.tar", last modified: Thu Jun 29 18:29:54 2023, max compression
```

## Comparing `mentord-1.1.4.tar` & `mentord-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.726765 mentord-1.1.4/
--rw-rw-rw-   0        0        0      718 2023-06-29 09:14:18.727264 mentord-1.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.722272 mentord-1.1.4/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/__init__.py
--rw-rw-rw-   0        0        0     2107 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/channel.py
--rw-rw-rw-   0        0        0     3288 2023-06-29 09:05:17.000000 mentord-1.1.4/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.726265 mentord-1.1.4/mentord.egg-info/
--rw-rw-rw-   0        0        0      718 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 09:14:18.728262 mentord-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      838 2023-06-29 09:13:49.000000 mentord-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:29:54.887025 mentord-1.1.5/
+-rw-rw-rw-   0        0        0      685 2023-06-29 18:29:54.887025 mentord-1.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 18:29:54.883032 mentord-1.1.5/mentord/
+-rw-rw-rw-   0        0        0      112 2023-06-29 18:20:54.000000 mentord-1.1.5/mentord/__init__.py
+-rw-rw-rw-   0        0        0      959 2023-06-29 18:23:13.000000 mentord-1.1.5/mentord/client.py
+-rw-rw-rw-   0        0        0      972 2023-06-29 18:06:21.000000 mentord-1.1.5/mentord/httpc.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:29:54.886027 mentord-1.1.5/mentord.egg-info/
+-rw-rw-rw-   0        0        0      685 2023-06-29 18:29:54.000000 mentord-1.1.5/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-29 18:29:54.000000 mentord-1.1.5/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:29:54.000000 mentord-1.1.5/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 18:29:54.000000 mentord-1.1.5/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:29:54.888024 mentord-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-06-29 18:28:09.000000 mentord-1.1.5/setup.py
```

### Comparing `mentord-1.1.4/setup.py` & `mentord-1.1.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 from setuptools import setup
 
-setup(name='mentord',
-      version='1.1.4',
-      long_description_content_type='text/markdown',
-      description="""
-Sync library from discord self bots.
-      """,
-      long_description="""
-### Example use
+setup(
+    name="mentord",
+    version="1.1.5",
+    description="A sync library for creating self bots in python!",
+    packages=["mentord"],
+    long_description_content_type="text/markdown",
+    long_description="""
+### Example use:
 
 ```python
 from mentord import *
 
-User_client: Client = Client() 
+User_client: Client = Client()
 User_client.connect(token='YOUR TOKEN')
 ```
 
 ### Use decorators:
 
 ```python
-@User_client.on_message
-def client_wait_message(message: Message):
-    print('new message!')
-
-@User_client.on_ready
-def client_on_ready():
-    print('client on connected!')
-```
-
-### Send message in channel:
-
-```python
-@User_client.on_message
-def client_wait_message(message: Message):
-    User_client.send_message(content="Hello!", embeds=[], channel_id=message.channel_id)
-```
-      """,
-      packages=['mentord'],)
+@client.eon_ready.on_ready(client=User_client, delay=5.0)
+def client_on_ready() -> None:
+    print('Self-bot is started!')
+
+@client.eon_message.message(client=User_client, delay=0.5)
+def client_on_message(message: Message) -> None:
+    utils.channel_opers.ChannelOperations(channel=message.channel_id, client=User_client).send_message("hello!")
+```""",
+)
```

