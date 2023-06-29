# Comparing `tmp/rubpy-6.2.4.tar.gz` & `tmp/rubpy-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubpy-6.2.4.tar", last modified: Fri Jun 16 08:33:15 2023, max compression
+gzip compressed data, was "rubpy-6.2.5.tar", last modified: Thu Jun 29 13:17:33 2023, max compression
```

## Comparing `rubpy-6.2.4.tar` & `rubpy-6.2.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.115081 rubpy-6.2.4/
--rw-rw-rw-   0        0        0     3378 2023-06-16 08:33:15.115081 rubpy-6.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.068218 rubpy-6.2.4/rubpy/
--rw-rw-rw-   0        0        0      240 2023-06-16 08:33:04.000000 rubpy-6.2.4/rubpy/__init__.py
--rw-rw-rw-   0        0        0    42789 2023-06-16 08:22:32.000000 rubpy-6.2.4/rubpy/client.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.099492 rubpy-6.2.4/rubpy/crypto/
--rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/crypto/__init__.py
--rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.4/rubpy/crypto/crypto.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.099492 rubpy-6.2.4/rubpy/gadgets/
--rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/gadgets/__init__.py
--rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.4/rubpy/gadgets/classino.py
--rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.4/rubpy/gadgets/exceptions.py
--rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.4/rubpy/gadgets/grouping.py
--rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.4/rubpy/gadgets/methods.py
--rw-rw-rw-   0        0        0     2524 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/gadgets/thumbnail.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.099492 rubpy-6.2.4/rubpy/network/
--rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/network/__init__.py
--rw-rw-rw-   0        0        0    12030 2023-06-16 08:31:13.000000 rubpy-6.2.4/rubpy/network/connection.py
--rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/network/proxies.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.099492 rubpy-6.2.4/rubpy/sessions/
--rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/sessions/__init__.py
--rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.4/rubpy/sessions/sqliteSession.py
--rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/sessions/stringSession.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.115081 rubpy-6.2.4/rubpy/structs/
--rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/structs/__init__.py
--rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/structs/handlers.py
--rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/structs/models.py
--rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.4/rubpy/structs/results.py
--rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.4/rubpy/structs/struct.py
-drwxrwxrwx   0        0        0        0 2023-06-16 08:33:15.099492 rubpy-6.2.4/rubpy.egg-info/
--rw-rw-rw-   0        0        0     3378 2023-06-16 08:33:14.000000 rubpy-6.2.4/rubpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      697 2023-06-16 08:33:14.000000 rubpy-6.2.4/rubpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 08:33:14.000000 rubpy-6.2.4/rubpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-06-16 08:33:14.000000 rubpy-6.2.4/rubpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-16 08:33:14.000000 rubpy-6.2.4/rubpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-16 08:33:15.115081 rubpy-6.2.4/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-06-16 08:32:55.000000 rubpy-6.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.295670 rubpy-6.2.5/
+-rw-rw-rw-   0        0        0     3378 2023-06-29 13:17:33.295670 rubpy-6.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2238 2023-04-26 17:35:11.000000 rubpy-6.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.256893 rubpy-6.2.5/rubpy/
+-rw-rw-rw-   0        0        0      240 2023-06-29 13:16:44.000000 rubpy-6.2.5/rubpy/__init__.py
+-rw-rw-rw-   0        0        0    44119 2023-06-29 13:13:18.000000 rubpy-6.2.5/rubpy/client.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.278092 rubpy-6.2.5/rubpy/crypto/
+-rw-rw-rw-   0        0        0       26 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2891 2023-06-14 11:35:15.000000 rubpy-6.2.5/rubpy/crypto/crypto.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/gadgets/
+-rw-rw-rw-   0        0        0      106 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/gadgets/__init__.py
+-rw-rw-rw-   0        0        0      892 2023-06-14 19:16:37.000000 rubpy-6.2.5/rubpy/gadgets/classino.py
+-rw-rw-rw-   0        0        0     2118 2023-04-26 18:12:01.000000 rubpy-6.2.5/rubpy/gadgets/exceptions.py
+-rw-rw-rw-   0        0        0    27137 2023-06-15 19:36:00.000000 rubpy-6.2.5/rubpy/gadgets/grouping.py
+-rw-rw-rw-   0        0        0    14188 2023-04-26 17:30:17.000000 rubpy-6.2.5/rubpy/gadgets/methods.py
+-rw-rw-rw-   0        0        0     6772 2023-06-29 12:36:38.000000 rubpy-6.2.5/rubpy/gadgets/thumbnail.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/network/
+-rw-rw-rw-   0        0        0       64 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/network/__init__.py
+-rw-rw-rw-   0        0        0    12030 2023-06-16 08:31:13.000000 rubpy-6.2.5/rubpy/network/connection.py
+-rw-rw-rw-   0        0        0    14807 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/network/proxies.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.288661 rubpy-6.2.5/rubpy/sessions/
+-rw-rw-rw-   0        0        0       82 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/sessions/__init__.py
+-rw-rw-rw-   0        0        0     2295 2023-06-14 11:13:33.000000 rubpy-6.2.5/rubpy/sessions/sqliteSession.py
+-rw-rw-rw-   0        0        0     1223 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/sessions/stringSession.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.295670 rubpy-6.2.5/rubpy/structs/
+-rw-rw-rw-   0        0        0       99 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/__init__.py
+-rw-rw-rw-   0        0        0     1985 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/handlers.py
+-rw-rw-rw-   0        0        0     4585 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/models.py
+-rw-rw-rw-   0        0        0      702 2022-09-12 11:03:20.000000 rubpy-6.2.5/rubpy/structs/results.py
+-rw-rw-rw-   0        0        0    15140 2023-04-23 17:55:22.000000 rubpy-6.2.5/rubpy/structs/struct.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:17:33.278092 rubpy-6.2.5/rubpy.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      697 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-29 13:17:33.000000 rubpy-6.2.5/rubpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:17:33.295670 rubpy-6.2.5/setup.cfg
+-rw-rw-rw-   0        0        0     1547 2023-06-29 13:16:58.000000 rubpy-6.2.5/setup.py
```

### Comparing `rubpy-6.2.4/PKG-INFO` & `rubpy-6.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.4
+Version: 6.2.5
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.4 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.5 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.4/README.md` & `rubpy-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/client.py` & `rubpy-6.2.5/rubpy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from .crypto import Crypto
 from .structs import Struct
 from Crypto.PublicKey import RSA
 from . import __name__ as logger_name
 from .network import Connection, Proxies
 from .gadgets import exceptions, methods, thumbnail
 from .sessions import StringSession, SQLiteSession
-
+try:
+    import cv2
+    import numpy
+except ImportError:
+    cv2 = None
+    numpy = None
 
 class Client:
     configuire = {
         'package': 'web.rubika.ir',
         'platform': 'Web',
         'app_name': 'Main',
         'user_agent': ('Mozilla/5.0 (Windows NT 10.0; Win64; x64) '
@@ -389,15 +394,15 @@
 
     async def unban_group_member(self, group_guid: str, member_guid: str):
         return await self(methods.groups.BanGroupMember(group_guid, member_guid, 'Unset'))
 
     async def add_group_members(self, group_guid: str, member_guids: list):
         return await self(methods.groups.AddGroupMembers(group_guid, member_guids))
 
-    async def get_group_all_members(self, group_guid: str, search_text: str = '', start_id: int = None):
+    async def get_group_all_members(self, group_guid: str, search_text: str = None, start_id: int = None):
         return await self(methods.groups.GetGroupAllMembers(group_guid, search_text, start_id))
 
     async def get_group_admin_members(self, group_guid: str, start_id: int = None):
         return await self(methods.groups.GetGroupAdminMembers(group_guid, start_id))
 
     async def get_group_mention_list(self, group_guid: str, search_mention: str = None):
         return await self(methods.groups.GetGroupMentionList(group_guid, search_mention))
@@ -514,36 +519,41 @@
         width: int = None,
         height: int = None,
         thumb: str = None,
         reply_to_message_id: str = None,
         *args,
         **kwargs,
     ):
+        if cv2 == None and numpy == None:
+            thumb, width, height = (thumbnail.thumb,
+                                          thumbnail.width,
+                                          thumbnail.height
+            )
+
         if object_guid.lower() in ('me', 'self', 'cloud'):
             object_guid = self._guid
 
         if type(photo) != bytes:
             async with aiofiles.open(photo, 'rb') as file:
                 file_name = os.path.basename(photo)
                 kwargs['file_name'] = kwargs.get('file_name', file_name)
                 photo = await file.read()
                 await file.close()
         else:
             kwargs['file_name'] = kwargs.get('file_name', file_name)
 
-        thumb = thumbnail.MakeThumbnail(photo)
-
         file_inline = await self.upload(photo, *args, **kwargs)
         file_inline['type'] = 'Image'
 
-        if thumb and width and height != None:
+        if cv2 == None and numpy == None:
             file_inline['width'] = width
             file_inline['height'] = height
             file_inline['thumb_inline'] = thumb
         else:
+            thumb = thumbnail.MakeThumbnail(photo)
             if isinstance(thumb, thumbnail.Thumbnail):
                 file_inline['width'] = thumb.width
                 file_inline['height'] = thumb.height
                 file_inline['thumb_inline'] = thumb.to_base64()
 
         return await self(
             methods.messages.SendMessage(
@@ -592,14 +602,21 @@
         time: str = None,
         width: int = None,
         height: int = None,
         reply_to_message_id: str = None,
         *args,
         **kwargs,
     ):
+        if cv2 == None and numpy == None:
+            thumb, time, width, height = (thumbnail.thumb,
+                                          thumbnail.time,
+                                          thumbnail.width,
+                                          thumbnail.height
+            )
+
         if object_guid.lower() in ('me', 'self', 'cloud'):
             object_guid = self._guid
 
         if type(gif) != bytes:
             async with aiofiles.open(gif, 'rb') as file:
                 file_name = os.path.basename(gif)
                 kwargs['file_name'] = kwargs.get('file_name', file_name)
@@ -607,22 +624,21 @@
                 await file.close()
         else:
             kwargs['file_name'] = kwargs.get('file_name', file_name)
 
         file_inline = await self.upload(gif, *args, **kwargs)
         file_inline['type'] = 'Gif'
 
-        thumb = thumbnail.MakeThumbnail.from_video(gif)
-
-        if thumb and width and height and time != None:
+        if cv2 == None and numpy == None:
             file_inline['width'] = width
             file_inline['height'] = height
             file_inline['thumb_inline'] = thumb
             file_inline['time'] = time
         else:
+            thumb = thumbnail.MakeThumbnail.from_video(gif)
             if isinstance(thumb, thumbnail.Thumbnail):
                 file_inline['time'] = thumb.seconds
                 file_inline['width'] = thumb.width
                 file_inline['height'] = thumb.height
                 file_inline['thumb_inline'] = thumb.to_base64()
 
         return await self(
@@ -641,14 +657,21 @@
         time: str = None,
         width: int = None,
         height: int = None,
         reply_to_message_id: str = None,
         *args,
         **kwargs,
     ):
+        if cv2 == None and numpy == None:
+            thumb, time, width, height = (thumbnail.thumb,
+                                          thumbnail.time,
+                                          thumbnail.width,
+                                          thumbnail.height
+            )
+
         if object_guid.lower() in ('me', 'self', 'cloud'):
             object_guid = self._guid
 
         if type(video) != bytes:
             async with aiofiles.open(video, 'rb') as file:
                 file_name = os.path.basename(video)
                 kwargs['file_name'] = kwargs.get('file_name', file_name)
@@ -656,22 +679,21 @@
                 await file.close()
         else:
             kwargs['file_name'] = kwargs.get('file_name', file_name)
 
         file_inline = await self.upload(video, *args, **kwargs)
         file_inline['type'] = 'Video'
 
-        thumb = thumbnail.MakeThumbnail.from_video(video)
-
-        if thumb and width and height and time != None:
+        if cv2 == None and numpy == None:
             file_inline['width'] = width
             file_inline['height'] = height
             file_inline['thumb_inline'] = thumb
             file_inline['time'] = time
         else:
+            thumb = thumbnail.MakeThumbnail.from_video(video)
             if isinstance(thumb, thumbnail.Thumbnail):
                 file_inline['time'] = thumb.seconds
                 file_inline['width'] = thumb.width
                 file_inline['height'] = thumb.height
                 file_inline['thumb_inline'] = thumb.to_base64()
 
         return await self(
@@ -902,14 +924,25 @@
 
     async def channel_preview_by_join_link(self, link: str):
         return await self(methods.channels.ChannelPreviewByJoinLink(link))
 
     async def get_channel_all_members(self, channel_guid: str, search_text: str = None, start_id: int = None):
         return await self(methods.channels.GetChannelAllMembers(channel_guid, search_text, start_id))
 
+    async def check_join(self, channel_guid: str, username: str) -> bool:
+        result = await self.get_channel_all_members(channel_guid, username.replace('@', ''))
+        in_chat_members: dict = result['in_chat_members']
+        for member in in_chat_members:
+            if username in member.values():
+                return True
+            else:
+                continue
+        else:
+            return False
+
     async def get_channel_admin_members(self, channel_guid: str, start_id: int = None):
         return await self(methods.channels.GetChannelAdminMembers(channel_guid, start_id))
 
     async def update_channel_username(self, channel_guid: str, username: str):
         return await self(methods.channels.UpdateChannelUsername(channel_guid, username))
 
     async def get_channel_link(self, channel_guid: str):
```

### Comparing `rubpy-6.2.4/rubpy/crypto/crypto.py` & `rubpy-6.2.5/rubpy/crypto/crypto.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/gadgets/classino.py` & `rubpy-6.2.5/rubpy/gadgets/classino.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/gadgets/exceptions.py` & `rubpy-6.2.5/rubpy/gadgets/exceptions.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/gadgets/grouping.py` & `rubpy-6.2.5/rubpy/gadgets/grouping.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/gadgets/methods.py` & `rubpy-6.2.5/rubpy/gadgets/methods.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/network/connection.py` & `rubpy-6.2.5/rubpy/network/connection.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/network/proxies.py` & `rubpy-6.2.5/rubpy/network/proxies.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/sessions/sqliteSession.py` & `rubpy-6.2.5/rubpy/sessions/sqliteSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/sessions/stringSession.py` & `rubpy-6.2.5/rubpy/sessions/stringSession.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/structs/handlers.py` & `rubpy-6.2.5/rubpy/structs/handlers.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/structs/models.py` & `rubpy-6.2.5/rubpy/structs/models.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/structs/results.py` & `rubpy-6.2.5/rubpy/structs/results.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy/structs/struct.py` & `rubpy-6.2.5/rubpy/structs/struct.py`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/rubpy.egg-info/PKG-INFO` & `rubpy-6.2.5/rubpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubpy
-Version: 6.2.4
+Version: 6.2.5
 Summary: This is an unofficial library and fastest library for deploying robots on Rubika accounts.
 Home-page: https://github.com/shayanheidari01/rubika
 Author: Shayan Heidari
 Author-email: contact@shayanheidari.info
 Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rubpy Version: 6.2.4 Summary: This is an unofficial
+Metadata-Version: 2.1 Name: rubpy Version: 6.2.5 Summary: This is an unofficial
 library and fastest library for deploying robots on Rubika accounts. Home-page:
 https://github.com/shayanheidari01/rubika Author: Shayan Heidari Author-email:
 contact@shayanheidari.info Keywords: rubika,rubpy,chat,bot,robot,asyncio
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `rubpy-6.2.4/rubpy.egg-info/SOURCES.txt` & `rubpy-6.2.5/rubpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rubpy-6.2.4/setup.py` & `rubpy-6.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiohttp', 'pycryptodome', 'aiofiles']
 
 with open("README.md", encoding="UTF-8") as f:
     readme = f.read()
 
 setup(
     name = 'rubpy',
-    version = '6.2.4',
+    version = '6.2.5',
     author='Shayan Heidari',
     author_email = 'contact@shayanheidari.info',
     description = 'This is an unofficial library and fastest library for deploying robots on Rubika accounts.',
     keywords = ['rubika', 'rubpy', 'chat', 'bot', 'robot', 'asyncio'],
     long_description = readme,
     python_requires="~=3.7",
     long_description_content_type = 'text/markdown',
```

