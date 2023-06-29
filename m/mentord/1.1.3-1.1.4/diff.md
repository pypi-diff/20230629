# Comparing `tmp/mentord-1.1.3.tar.gz` & `tmp/mentord-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentord-1.1.3.tar", last modified: Tue Jun 27 13:17:47 2023, max compression
+gzip compressed data, was "mentord-1.1.4.tar", last modified: Thu Jun 29 09:14:18 2023, max compression
```

## Comparing `mentord-1.1.3.tar` & `mentord-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.241837 mentord-1.1.3/
--rw-rw-rw-   0        0        0      612 2023-06-27 13:17:47.241837 mentord-1.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.236314 mentord-1.1.3/mentord/
--rw-rw-rw-   0        0        0      202 2023-06-27 13:13:33.000000 mentord-1.1.3/mentord/__init__.py
--rw-rw-rw-   0        0        0     2107 2023-06-27 12:58:51.000000 mentord-1.1.3/mentord/channel.py
--rw-rw-rw-   0        0        0     2884 2023-06-27 12:55:25.000000 mentord-1.1.3/mentord/client.py
--rw-rw-rw-   0        0        0     1443 2023-06-27 09:58:05.000000 mentord-1.1.3/mentord/embed.py
--rw-rw-rw-   0        0        0     1367 2023-06-27 08:08:39.000000 mentord-1.1.3/mentord/eother.py
--rw-rw-rw-   0        0        0     1121 2023-06-27 09:58:08.000000 mentord-1.1.3/mentord/guild.py
--rw-rw-rw-   0        0        0      882 2023-06-27 09:08:15.000000 mentord-1.1.3/mentord/http_.py
--rw-rw-rw-   0        0        0      629 2023-06-27 07:18:33.000000 mentord-1.1.3/mentord/member.py
--rw-rw-rw-   0        0        0      590 2023-06-27 09:58:12.000000 mentord-1.1.3/mentord/message.py
--rw-rw-rw-   0        0        0     1721 2023-06-27 09:58:21.000000 mentord-1.1.3/mentord/user.py
-drwxrwxrwx   0        0        0        0 2023-06-27 13:17:47.240838 mentord-1.1.3/mentord.egg-info/
--rw-rw-rw-   0        0        0      612 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-27 13:17:47.000000 mentord-1.1.3/mentord.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 13:17:47.242836 mentord-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      717 2023-06-27 13:17:38.000000 mentord-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.726765 mentord-1.1.4/
+-rw-rw-rw-   0        0        0      718 2023-06-29 09:14:18.727264 mentord-1.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.722272 mentord-1.1.4/mentord/
+-rw-rw-rw-   0        0        0      202 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/__init__.py
+-rw-rw-rw-   0        0        0     2107 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/channel.py
+-rw-rw-rw-   0        0        0     3288 2023-06-29 09:05:17.000000 mentord-1.1.4/mentord/client.py
+-rw-rw-rw-   0        0        0     1443 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/embed.py
+-rw-rw-rw-   0        0        0     1367 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/eother.py
+-rw-rw-rw-   0        0        0     1121 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/guild.py
+-rw-rw-rw-   0        0        0      882 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/http_.py
+-rw-rw-rw-   0        0        0      629 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/member.py
+-rw-rw-rw-   0        0        0      590 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/message.py
+-rw-rw-rw-   0        0        0     1721 2023-06-29 08:48:35.000000 mentord-1.1.4/mentord/user.py
+drwxrwxrwx   0        0        0        0 2023-06-29 09:14:18.726265 mentord-1.1.4/mentord.egg-info/
+-rw-rw-rw-   0        0        0      718 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-29 09:14:18.000000 mentord-1.1.4/mentord.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 09:14:18.728262 mentord-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      838 2023-06-29 09:13:49.000000 mentord-1.1.4/setup.py
```

### Comparing `mentord-1.1.3/PKG-INFO` & `mentord-1.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.3
-Summary: Library for discord self bots.
+Version: 1.1.4
+Summary: Sync library from discord self bots.
 Description-Content-Type: text/markdown
 
 
-### Example use:
+### Example use
+
 ```python
+from mentord import *
+
 User_client: Client = Client() 
 User_client.connect(token='YOUR TOKEN')
 ```
 
 ### Use decorators:
+
 ```python
 @User_client.on_message
 def client_wait_message(message: Message):
     print('new message!')
 
 @User_client.on_ready
 def client_on_ready():
-    print('client on connected!')    
+    print('client on connected!')
 ```
 
-### Send message in chat:
+### Send message in channel:
+
 ```python
-User_client.send_message(content="Hello!", embeds=[], channel_id="916385464238370826")
+@User_client.on_message
+def client_wait_message(message: Message):
+    User_client.send_message(content="Hello!", embeds=[], channel_id=message.channel_id)
 ```
```

### Comparing `mentord-1.1.3/mentord/channel.py` & `mentord-1.1.4/mentord/channel.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/client.py` & `mentord-1.1.4/mentord/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,26 +57,35 @@
 
         messages: dict = self.get_messages_id()
 
         while True:
 
             for channel in self.user.channels:
 
-                response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=1'.format(channel.id, messages[channel.id]),
+                try:
+
+                    response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=1'.format(channel.id, messages[channel.id]),
+                                        headers={"Authorization": self.user.token, "Content-Type": "application/json"}, )
+
+                except:
+
+                    messages: dict = self.get_messages_id()
+
+                    response = requests.get('https://discordapp.com/api/v9/channels/{0}/messages?after={1}&limit=1'.format(channel.id, messages[channel.id]),
                                         headers={"Authorization": self.user.token, "Content-Type": "application/json"}, )
 
                 if response.json().count != 0:
 
                     for message in response.json():
 
                         func(Message(message))
                 
                         messages[channel.id] = Message(message).id
 
-            time.sleep(1)
+            time.sleep(0.5)
 
     def send_message(self, content: str = "", embeds: list[Embed] = [], channel_id: str = "") -> any:
 
         repsonse = HttpClient().request("POST", 'https://discordapp.com/api/v9//channels/{0}/messages'.format(channel_id),
                                         header={"Authorization": self.user.token, "Content-Type": "application/json"}, json={
             'content': content,
             'tts': False,
```

### Comparing `mentord-1.1.3/mentord/embed.py` & `mentord-1.1.4/mentord/embed.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/eother.py` & `mentord-1.1.4/mentord/eother.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/guild.py` & `mentord-1.1.4/mentord/guild.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/http_.py` & `mentord-1.1.4/mentord/http_.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/member.py` & `mentord-1.1.4/mentord/member.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/message.py` & `mentord-1.1.4/mentord/message.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord/user.py` & `mentord-1.1.4/mentord/user.py`

 * *Files identical despite different names*

### Comparing `mentord-1.1.3/mentord.egg-info/PKG-INFO` & `mentord-1.1.4/mentord.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: mentord
-Version: 1.1.3
-Summary: Library for discord self bots.
+Version: 1.1.4
+Summary: Sync library from discord self bots.
 Description-Content-Type: text/markdown
 
 
-### Example use:
+### Example use
+
 ```python
+from mentord import *
+
 User_client: Client = Client() 
 User_client.connect(token='YOUR TOKEN')
 ```
 
 ### Use decorators:
+
 ```python
 @User_client.on_message
 def client_wait_message(message: Message):
     print('new message!')
 
 @User_client.on_ready
 def client_on_ready():
-    print('client on connected!')    
+    print('client on connected!')
 ```
 
-### Send message in chat:
+### Send message in channel:
+
 ```python
-User_client.send_message(content="Hello!", embeds=[], channel_id="916385464238370826")
+@User_client.on_message
+def client_wait_message(message: Message):
+    User_client.send_message(content="Hello!", embeds=[], channel_id=message.channel_id)
 ```
```

### Comparing `mentord-1.1.3/setup.py` & `mentord-1.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 from setuptools import setup
 
 setup(name='mentord',
-      version='1.1.3',
-      description='Library for discord self bots.',
-      packages=['mentord'],
+      version='1.1.4',
+      long_description_content_type='text/markdown',
+      description="""
+Sync library from discord self bots.
+      """,
       long_description="""
-### Example use:
+### Example use
+
 ```python
+from mentord import *
+
 User_client: Client = Client() 
 User_client.connect(token='YOUR TOKEN')
 ```
 
 ### Use decorators:
+
 ```python
 @User_client.on_message
 def client_wait_message(message: Message):
     print('new message!')
 
 @User_client.on_ready
 def client_on_ready():
-    print('client on connected!')    
+    print('client on connected!')
 ```
 
-### Send message in chat:
+### Send message in channel:
+
 ```python
-User_client.send_message(content="Hello!", embeds=[], channel_id="916385464238370826")
+@User_client.on_message
+def client_wait_message(message: Message):
+    User_client.send_message(content="Hello!", embeds=[], channel_id=message.channel_id)
 ```
       """,
-      long_description_content_type='text/markdown')
+      packages=['mentord'],)
```

