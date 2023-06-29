# Comparing `tmp/rubika-6.0.7.tar.gz` & `tmp/rubika-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubika-6.0.7.tar", last modified: Fri May 19 13:02:02 2023, max compression
+gzip compressed data, was "rubika-6.6.6.tar", last modified: Thu Jun 29 17:57:52 2023, max compression
```

## Comparing `rubika-6.0.7.tar` & `rubika-6.6.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwx---   0 root         (0)     9997        0 2023-05-19 13:02:02.410000 rubika-6.0.7/
--rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.0.7/LICENSE
--rw-rw----   0 root         (0)     9997     4193 2023-05-19 13:02:02.410000 rubika-6.0.7/PKG-INFO
--rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.0.7/README.md
-drwxrwx---   0 root         (0)     9997        0 2023-05-19 13:02:02.400000 rubika-6.0.7/rubika/
--rw-rw----   0 root         (0)     9997     4724 2023-05-19 12:59:33.000000 rubika-6.0.7/rubika/Types.py
--rw-rw----   0 root         (0)     9997      137 2023-05-19 13:00:20.000000 rubika-6.0.7/rubika/__init__.py
--rw-rw----   0 root         (0)     9997    38565 2023-05-19 12:58:01.000000 rubika-6.0.7/rubika/client.py
--rw-rw----   0 root         (0)     9997     6735 2023-05-19 13:01:25.000000 rubika-6.0.7/rubika/configs.py
--rw-rw----   0 root         (0)     9997     1022 2023-04-07 14:31:47.000000 rubika-6.0.7/rubika/encryption.py
--rw-rw----   0 root         (0)     9997      147 2023-04-07 14:31:47.000000 rubika-6.0.7/rubika/exceptions.py
--rw-rw----   0 root         (0)     9997     4631 2023-05-19 12:58:14.000000 rubika-6.0.7/rubika/fileIO.py
--rw-rw----   0 root         (0)     9997     5060 2023-04-07 14:31:47.000000 rubika-6.0.7/rubika/filters.py
--rw-rw----   0 root         (0)     9997     6344 2023-05-19 12:58:56.000000 rubika-6.0.7/rubika/rubino.py
--rw-rw----   0 root         (0)     9997     7014 2023-05-19 12:59:55.000000 rubika-6.0.7/rubika/tools.py
-drwxrwx---   0 root         (0)     9997        0 2023-05-19 13:02:02.410000 rubika-6.0.7/rubika.egg-info/
--rw-rw----   0 root         (0)     9997     4193 2023-05-19 13:02:02.000000 rubika-6.0.7/rubika.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      394 2023-05-19 13:02:02.000000 rubika-6.0.7/rubika.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2023-05-19 13:02:02.000000 rubika-6.0.7/rubika.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.0.7/rubika.egg-info/not-zip-safe
--rw-rw----   0 root         (0)     9997       73 2023-05-19 13:02:02.000000 rubika-6.0.7/rubika.egg-info/requires.txt
--rw-rw----   0 root         (0)     9997        7 2023-05-19 13:02:02.000000 rubika-6.0.7/rubika.egg-info/top_level.txt
--rw-rw----   0 root         (0)     9997       79 2023-05-19 13:02:02.410000 rubika-6.0.7/setup.cfg
--rw-rw----   0 root         (0)     9997     4580 2023-05-19 13:01:03.000000 rubika-6.0.7/setup.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/
+-rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.6.6/LICENSE
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 17:57:52.630000 rubika-6.6.6/PKG-INFO
+-rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.6.6/README.md
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/rubika/
+-rw-rw----   0 root         (0)     9997     5307 2023-06-29 17:52:20.000000 rubika-6.6.6/rubika/Types.py
+-rw-rw----   0 root         (0)     9997      116 2023-06-19 10:36:07.000000 rubika-6.6.6/rubika/__init__.py
+-rw-rw----   0 root         (0)     9997    42801 2023-06-29 17:49:59.000000 rubika-6.6.6/rubika/client.py
+-rw-rw----   0 root         (0)     9997     6535 2023-06-29 17:50:36.000000 rubika-6.6.6/rubika/configs.py
+-rw-rw----   0 root         (0)     9997     3771 2023-06-29 17:49:51.000000 rubika-6.6.6/rubika/encryption.py
+-rw-rw----   0 root         (0)     9997      170 2023-06-13 09:40:35.000000 rubika-6.6.6/rubika/exceptions.py
+-rw-rw----   0 root         (0)     9997     5458 2023-06-29 17:50:51.000000 rubika-6.6.6/rubika/fileIO.py
+-rw-rw----   0 root         (0)     9997     5469 2023-06-09 08:44:46.000000 rubika-6.6.6/rubika/filters.py
+-rw-rw----   0 root         (0)     9997     6444 2023-06-29 17:51:07.000000 rubika-6.6.6/rubika/rubino.py
+-rw-rw----   0 root         (0)     9997     4580 2023-06-29 17:53:02.000000 rubika-6.6.6/rubika/setup.py
+-rw-rw----   0 root         (0)     9997     6944 2023-06-29 17:52:00.000000 rubika-6.6.6/rubika/tools.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 17:57:52.630000 rubika-6.6.6/rubika.egg-info/
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/PKG-INFO
+-rw-rw----   0 root         (0)     9997      410 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0)     9997        1 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.6.6/rubika.egg-info/not-zip-safe
+-rw-rw----   0 root         (0)     9997       82 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/requires.txt
+-rw-rw----   0 root         (0)     9997        7 2023-06-29 17:57:52.000000 rubika-6.6.6/rubika.egg-info/top_level.txt
+-rw-rw----   0 root         (0)     9997       79 2023-06-29 17:57:52.640000 rubika-6.6.6/setup.cfg
+-rw-rw----   0 root         (0)     9997     2484 2023-06-13 10:32:27.000000 rubika-6.6.6/setup.py
```

### Comparing `rubika-6.0.7/LICENSE` & `rubika-6.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rubika-6.0.7/PKG-INFO` & `rubika-6.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.0.7
+Version: 6.6.6
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
@@ -35,15 +35,14 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 <p align="center">
     <a href="https://github.com/bahman-ahmadi/rubika">
         <img src="https://rubikalib.github.io/assets/logo.png" alt="RUBIKA" width="128">
     </a>
     <br>
     <b>Rubika Bot Self Library for Python</b>
     <br>
@@ -113,8 +112,8 @@
 - Join the official channel at https://t.me/rubikalib and stay tuned for news, updates and announcements.
 
 ### License
 rubika library is licensed under [GPLv3 license](https://github.com/bahman-ahmadi/rubika/blob/main/LICENSE)
 
 This is not an official rubika product. It is not affiliated with nor endorsed by rubika Inc.
 
-© 2023 Bahman Ahmadi
+© 2022 Bahman Ahmadi
```

### Comparing `rubika-6.0.7/README.md` & `rubika-6.6.6/README.md`

 * *Files identical despite different names*

### Comparing `rubika-6.0.7/rubika/Types.py` & `rubika-6.6.6/rubika/Types.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,97 +1,106 @@
 from rubika.exceptions import InvalidInput
 from rubika.configs import makeData
 from rubika.tools import Tools
 
+
 class DictToClass:
-	def __init__(self, message):
-		assert type(message) == dict
-		[setattr(self, key, [DictToClass(x) if type(x) == dict else x for x in val]) if type(val) in (list, tuple) else setattr(self, key, DictToClass(val) if type(val) == dict else val) for key,val in message.items()]
+    def __init__(self, message):
+        assert type(message) == dict
+        [setattr(self, key, [DictToClass(x) if type(x) == dict else x for x in val]) if type(val) in (
+            list, tuple) else setattr(self, key, DictToClass(val) if type(val) == dict else val) for key, val in message.items()]
+
 
 def ClassToDict(dictToClassObject, result={}):
-	for key,val in dictToClassObject.__dict__.items():
-		if type(val) not in [DictToClass, dict]: result.setdefault(key, val)
-		else:
-			if type(val) == DictToClass: result[key] = val.__dict__
-			else: result[key] = val
-	return result
+    for key, val in dictToClassObject.__dict__.items():
+        if type(val) not in [DictToClass, dict]:
+            result.setdefault(key, val)
+        else:
+            if type(val) == DictToClass:
+                result[key] = val.__dict__
+            else:
+                result[key] = val
+    return result
+
 
 class Message:
-	def __init__(self, auth:str, message:dict, **kwargs):
-		self.auth    = auth
-		self.chat_id = kwargs.get("chat_id")
-		self.bot     = kwargs.get("bot")
+    def __init__(self, auth: str, message: dict, **kwargs):
+        self.auth = auth
+        self.chat_id = kwargs.get("chat_id")
+        self.bot = kwargs.get("bot")
 
-		if type(message) != dict:
-			try:
-				from rubika.client import Bot
-				self.bot = self.bot or Bot("", self.auth)
-				message = self.bot.getMessagesInfo(self.chat_id, [str(message)])[0]
-			except IndexError:
-				raise InvalidInput("the auth/entered message id/chat id is incorrect")
+        if type(message) != dict:
+            try:
+                from rubika.client import Bot
+                self.bot = self.bot or Bot("", self.auth)
+                message = self.bot.getMessagesInfo(
+                    self.chat_id, [str(message)])[0]
+            except IndexError:
+                raise InvalidInput(
+                    "the auth/entered message id/chat id is incorrect")
 
-		self.data = DictToClass(message)
+        self.data = DictToClass(message)
 
-	def edit(self, newText:str, metadata:list = [], parseMode:str = None) -> dict:
-		return self.bot.editMessage(self.data.message_id, self.chat_id, newText, metadata, parseMode)
+    def edit(self, newText: str, metadata: list = [], parseMode: str = None) -> dict:
+        return self.bot.editMessage(self.data.message_id, self.chat_id, newText, metadata, parseMode)
 
-	def forward(self, to:str) -> dict:
-		return self.bot.forwardMessages(self.chat_id, [str(self.data.message_id)], to)
+    def forward(self, to: str) -> dict:
+        return self.bot.forwardMessages(self.chat_id, [str(self.data.message_id)], to)
 
-	def resend(self, to:str, **kwargs) -> dict:
-		return self.bot.resendMessage(self.chat_id, self.data.message_id, to, **kwargs)
+    def resend(self, to: str, **kwargs) -> dict:
+        return self.bot.resendMessage(self.chat_id, self.data.message_id, to, **kwargs)
 
-	def getInfo(self) -> dict:
-		return self.bot.getMessagesInfo(self.chat_id, [str(self.data.message_id)])[0]
+    def getInfo(self) -> dict:
+        return self.bot.getMessagesInfo(self.chat_id, [str(self.data.message_id)])[0]
 
-	def getPollStatus(self) -> dict:
-		return self.bot.getPollStatus(self.data.message.poll_id)
+    def getPollStatus(self) -> dict:
+        return self.bot.getPollStatus(self.data.message.poll_id)
 
-	def getPollOptionVoters(self, option_index:int, start_id=None):
-		return self.bot.getPollOptionVoters(self.data.message.poll_id, int(option_index), start_id)
+    def getPollOptionVoters(self, option_index: int, start_id=None):
+        return self.bot.getPollOptionVoters(self.data.message.poll_id, int(option_index), start_id)
 
-	def show(self) -> dict:
-		try:
-			from rich import print as Print
-			Print(ClassToDict(self.data))
-		except MoudleNotFoundError:
-			print(ClassToDict(self.data))
+    def show(self) -> dict:
+        try:
+            from rich import print as Print
+            Print(ClassToDict(self.data))
+        except MoudleNotFoundError:
+            print(ClassToDict(self.data))
 
-	def reply(self, text:str, metadata:list=[], parseMode:str=None) -> dict:
-		return self.bot.sendMessage(self.chat_id, str(text), metadata, parseMode, message_id=self.data.message_id)
+    def reply(self, text: str, metadata: list = [], parseMode: str = None) -> dict:
+        return self.bot.sendMessage(self.chat_id, str(text), metadata, parseMode, message_id=self.data.message_id)
 
-	def reply_photo(self, photo:str, caption:str=None, metadata:list=[], parseMode:str=None, thumbnail:str=None, size:list=[], uresponse:list=None) -> dict:
-		return self.bot.sendPhoto(self.chat_id, photo, size, thumbnail, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_photo(self, photo: str, caption: str = None, metadata: list = [], parseMode: str = None, thumbnail: str = None, size: list = [], uresponse: list = None) -> dict:
+        return self.bot.sendPhoto(self.chat_id, photo, size, thumbnail, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
 
-	def reply_video(self, video:str, caption:str=None, metadata:list=[], parseMode:str=None, thumbnail:str=None, size:list=[], uresponse:list=None) -> dict:
-		return self.bot.sendVideo(self.chat_id, video, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_video(self, video: str, caption: str = None, metadata: list = [], parseMode: str = None, thumbnail: str = None, size: list = [], uresponse: list = None) -> dict:
+        return self.bot.sendVideo(self.chat_id, video, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
 
-	def reply_music(self, music:str, caption:str=None, metadata:list=[], parseMode:str=None, uresponse:list=None) -> dict:
-		return self.bot.sendMusic(self.chat_id, music, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_music(self, music: str, caption: str = None, metadata: list = [], parseMode: str = None, uresponse: list = None) -> dict:
+        return self.bot.sendMusic(self.chat_id, music, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
 
-	def reply_voice(self, voice:str, caption:str, time:int=None, metadata:list=[], parseMode:str=None, uresponse:list=None) -> dict:
-		return self.bot.sendVoice(self.chat_id, voice, time, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_voice(self, voice: str, caption: str, time: int = None, metadata: list = [], parseMode: str = None, uresponse: list = None) -> dict:
+        return self.bot.sendVoice(self.chat_id, voice, time, metadata, parseMode, caption, message_id=self.data.message_id, uresponse=uresponse)
 
-	def reply_document(self, file:str, caption:str, metadata:list=[], parseMode:str=None, uresponse:list=None) -> dict:
-		return self.bot.sendDocument(self.chat_id, file, caption, metadata, parseMode, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_document(self, file: str, caption: str, metadata: list = [], parseMode: str = None, uresponse: list = None) -> dict:
+        return self.bot.sendDocument(self.chat_id, file, caption, metadata, parseMode, message_id=self.data.message_id, uresponse=uresponse)
 
-	def reply_location(self, x:float, y:float) -> dict:
-		return self.bot.sendLocation(self.chat_id, [x,y], message_id=self.data.message_id)
+    def reply_location(self, x: float, y: float) -> dict:
+        return self.bot.sendLocation(self.chat_id, [x, y], message_id=self.data.message_id)
 
-	def reply_gif(self, video:str, caption:str, width:int, height:int, time:int=None, metadata:list=[], parseMode:str=None, thumbnail:str=None, uresponse:list=None) -> dict:
-		return self.bot.sendGIF(self.chat_id, video, width, height, time, metadata, parseMode, thumbnail, caption, message_id=self.data.message_id, uresponse=uresponse)
+    def reply_gif(self, video: str, caption: str, width: int, height: int, time: int = None, metadata: list = [], parseMode: str = None, thumbnail: str = None, uresponse: list = None) -> dict:
+        return self.bot.sendGIF(self.chat_id, video, width, height, time, metadata, parseMode, thumbnail, caption, message_id=self.data.message_id, uresponse=uresponse)
 
-	def delete(self, *args) -> dict:
-		#args can set for delete other message (out of current message)
-		return self.bot.deleteMessages(self.chat_id, [str(self.data.message_id), *args])
+    def delete(self, *args) -> dict:
+        # args can set for delete other message (out of current message)
+        return self.bot.deleteMessages(self.chat_id, [str(self.data.message_id), *args])
 
-	def ban(self) -> dict:
-		return self.bot.banMember(self.chat_id, self.data.author_object_guid)
+    def ban(self) -> dict:
+        return self.bot.banMember(self.chat_id, self.data.author_object_guid)
 
-	def block(self) -> dict:
-		return self.bot.block(self.data.author_object_guid)
+    def block(self) -> dict:
+        return self.bot.block(self.data.author_object_guid)
 
-	def unblock(self) -> dict:
-		return self.bot.unblock(self.data.author_object_guid)
+    def unblock(self) -> dict:
+        return self.bot.unblock(self.data.author_object_guid)
 
-	def download(self, saveAs:str=None) -> bytes :
-		return self.bot.download(self.chat_id, self.data.message_id, saveAs=saveAs)
+    def download(self, saveAs: str = None) -> bytes:
+        return self.bot.download(self.chat_id, self.data.message_id, saveAs=saveAs)
```

### Comparing `rubika-6.0.7/rubika/client.py` & `rubika-6.6.6/rubika/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,290 +1,583 @@
-from os         import path
-from threading  import Thread
-from datetime   import datetime
-from sys        import exc_info
-from json       import loads, dumps
-from random     import randint, choice
-from requests   import get as GET, exceptions
-
-from rubika.fileIO     import *
-from rubika.filters    import *
-from rubika.tools      import Tools
+from os import path
+from sys import exc_info
+from base64 import b64decode
+from threading import Thread
+from datetime import datetime
+from json import loads, dumps
+from random import randint, choice
+from requests import get as GET, exceptions
+
+from rubika.fileIO import *
+from rubika.filters import *
+from rubika.tools import Tools
+from rubika.exceptions import InvalidAuth
 from rubika.encryption import encryption
-from rubika.configs    import makeData, makeTmpData, defaultDevice, _getURL, welcome, __version__, __license__, __copyright__
+from rubika.configs import makeData, makeTmpData, defaultDevice, _getURL, welcome, __version__, __license__, __copyright__
 
 welcome(f"rubika library version {__version__}\n{__copyright__}\n→ docs : https://rubikalib.github.io\n")
 
 class Bot:
     downloadURL, DCsURL, getDCsURL, wsURL = "https://messengerX.iranlms.ir/GetFile.ashx", "https://messengerg2cX.iranlms.ir/", "https://getdcmess.iranlms.ir", "wss://msocket1.iranlms.ir:80"
 
-    def __init__(self, appName:str, auth:str=None, phoneNumber:str=None, wantRegister:bool=True, reconnect:bool=False, reconnectFunc:callable=lambda msg: ..., device:dict=defaultDevice, appType="rubika"):
-        self.appName, self.appType = appName, appType.lower()
-        if self.appType.lower() == "shad": Bot.setAsShad(self)
-
-        if auth is not None and len(auth) == 32 : self.auth = auth
-        else :
-            fileExist   = path.exists(f"{self.appName}.json")
-            phoneNumber = phoneNumber if not fileExist and phoneNumber is not None and len(phoneNumber) == 11 else input("please enter your phone number (e.g. 09123456789) : ")
-            account     = loads(open(f"{self.appName}.json").read()) if fileExist else Bot.signIn(phoneNumber, Bot.sendCode(phoneNumber)["data"]["phone_code_hash"], input("please enter activation code : "))
-            self.auth   = account["data"]["auth"]
-            if not fileExist and wantRegister :
-                Bot.registerDevice(self.auth, device=device)
-                open(f"{self.appName}.json", "w").write(dumps(account, indent=4, ensure_ascii=True))
-
-        self.enc  = encryption(self.auth)
-        if reconnect:
-            def keepingAlive():
-                soc = Socket(self.auth)
-                @soc.handler()
-                def reconnect(message): reconnectFunc(message)
-            Thread(target=keepingAlive).start()
-
-    #_getURL    = lambda dc_id=None: _getURL(Bot.DCsURL, Bot.getDCsURL, dc_id)
-    addContact = lambda self, first_name, last_name, phone: Bot._create(4, self.auth, "addAddressBook", {"first_name": first_name, "last_name": last_name, "phone": phone})
-    addGroup   = lambda self, title, users_chat_id: Bot._create(5, self.auth, "addGroup", {"title": title, "member_guids": users_chat_id})
-    addChannel = lambda self, title, channelType="Public", users_chat_id=None: Bot._create(5, self.auth, "addChannel", {"channel_type": channelType, "title": title, "member_guids": users_chat_id or []})
-    addFolder  = lambda self, name, exclude_chat_types=[], exclude_object_guids=[], include_chat_types=[], include_object_guids=[], is_add_to_top=True, folder_id="": Bot._create(5, self.auth, "addFolder", dict(exclude_object_guids=exclude_object_guids, include_object_guids=include_object_guids, exclude_chat_types=exclude_chat_types, include_chat_types=include_chat_types, folder_id=folder_id, is_add_to_top=is_add_to_top, name=name), clients.android)
-
-    banMember  = lambda self, chat_id, member_id: Bot._create(5, self.auth, f"ban{Bot._chatDetection(chat_id)}Member", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guid": member_id, "action":"Set"})
-    block      = lambda self, chat_id: Bot._create(5, self.auth, "setBlockUser", {"action": "Block","user_guid": chat_id})
-
-    _create        = lambda api_version, auth, method, data, client=None: makeData(int(api_version), auth, method, dict(data), client or clients.web if api_version == 5 else clients.android, url=_getURL(DCsURL=Bot.DCsURL , getDCsURL=Bot.getDCsURL , dc_id=None))
-    _createTMP     = lambda method, data: makeTmpData(method, dict(data), url=_getURL(DCsURL=Bot.DCsURL , getDCsURL=Bot.getDCsURL , dc_id=None))
-    _chatDetection = lambda chat_id: Tools.chatDetection(chat_id)
-    changeLink     = lambda self, chat_id: Bot._create(4, self.auth, f"set{Bot._chatDetection(chat_id)}Link", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id})
-    changePassword = lambda self, hint, newPass, oldPass: Bot._create(4, self.auth, "changePassword", {"new_hint": hint, "new_password": newPass, "password": oldPass})
-    checkPassword  = lambda self, password: Bot._create(4, self.auth, "checkTwoStepPasscode", {"password": password}).get("data").get("is_vaild")
-
-    deleteMessages    = lambda self, chat_id, message_ids: Bot._create(5, self.auth, "deleteMessages", {"object_guid":chat_id,"message_ids":list(message_ids),"type":"Global"})
-    deleteAdmin       = lambda self, chat_id, member_id: Bot._create(5, self.auth, f"set{Bot._chatDetection(chat_id)}Admin", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "action": "UnsetAdmin", "member_guid": member_id})
-    deleteAvatar      = lambda self, chat_id, avatar_id: Bot._create(5, self.auth, "deleteAvatar", {"object_guid": chat_id,"avatar_id": avatar_id})
-    deleteChatHistory = lambda self, chat_id, lastMessageId: Bot._create(4, self.auth, "deleteChatHistory", {"object_guid": chat_id,"last_message_id": lastMessageId})
-    deleteFolder      = lambda self, folder_id: Bot._create(5, self.auth, "deleteFolder", dict(folder_id=folder_id), clients.android)
-    deleteUserChat    = lambda self, chat_id, lastMessageID: Bot._create(5, self.auth, "deleteUserChat", {"last_deleted_message_id": lastMessageID, "user_guid": chat_id})
-    download          = lambda self, chat_id, message_id, save=True, saveAs=None, logging=True: download(self, chat_id, message_id, save, saveAs, logging)
-    disablePassword   = lambda self, password: Bot._create(4, self.auth, "turnOffTwoStep", {"password": password})
+    def __init__(self, appName:str, auth:str=None, privateKey:str=None, \
+                 b64decodePrivate:bool=True, userAgent:str="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0", \
+                 wantRegister:bool=True, device:dict=defaultDevice):
+        
+        # Setting basic variables
+        self.appName, self.enc = appName, encryption
+    
+        # Config the account
+        if auth is not None and len(auth) == 32:
+            self.auth = auth
+        else:
+            fileName = f"{self.appName}.json"
+            fileExists = path.exists(fileName)
+            if fileExists:
+                self.auth = loads(open(fileName).read())["auth"]
+                privateKey = loads(open(fileName).read())["private"]
+                b64decodePrivate = False
+            else:
+                phoneNumber = input(">>> Enter the Phone number (e.g. 09123456789): ")
+                sendCodeResp = Bot.sendCode(phoneNumber)
+                
+                if sendCodeResp.get('data') is None:
+                    raise InvalidAuth('Unfortunately, your account has been suspended!')
+                elif sendCodeResp['data']['status'] == 'SendPassKey':
+                    passKey = input(f">>> Enter your 2FA pass key{'(' + sendCodeResp['data'].get('hint_pass_key') + ')' if sendCodeResp['data'].get('hint_pass_key') is not None else ''}: ")
+                    sendCodeResp = Bot.sendCode(phoneNumber, passKey=passKey)
+                    while sendCodeResp['data']['status'] == "InvalidPassKey":
+                        passKey = input(f">>> Re-Enter your 2FA pass key{'(' + sendCodeResp['data'].get('hint_pass_key') + ')' if sendCodeResp['data'].get('hint_pass_key') is not None else ''}: ")
+                        sendCodeResp = Bot.sendCode(phoneNumber, passKey=passKey)
+                else:
+                    tmp, codeHash = sendCodeResp['tmp'], sendCodeResp["data"]["phone_code_hash"]
+                    otp = input(">>> Enter activation code: ")
+                    account = Bot.signIn(tmp, phoneNumber, codeHash, otp)
+                    while account['data']['status'] == 'CodeIsInvalid':
+                        otp = input(">>> Re-Enter activation code: ")
+                        account = Bot.signIn(tmp, phoneNumber, codeHash, otp)
+                
+                    self.auth = account['auth']
+                    Bot.privateKey = privateKey = account['private']
+                    open(f"{self.appName}.json", "w").write(dumps(account, indent=4, ensure_ascii=True))
+                    
+                    if wantRegister:
+                        Bot.registerDevice(self.auth, device=device)
+        
+        # No matter that login is manually or automatically, this block will run anyway
+        if b64decodePrivate:
+            privateKey = loads(b64decode(privateKey).decode('utf-8'))['d']
+     
+        Bot.privateKey = self.privateKey = privateKey
+        Bot.enc = self.enc = self.enc(self.enc.changeAuthType(self.auth), private_key=privateKey)
+
+    def __enter__(self): return self
+    def __exit__(self, exc_type, exc_value, exc_tb): return self
+
+
+    # _getURL    = lambda dc_id=None: _getURL(Bot.DCsURL, Bot.getDCsURL, dc_id)
+    def addContact(self, first_name, last_name, phone):
+        return Bot._create(self.auth, "addAddressBook", {"first_name": first_name, "last_name": last_name, "phone": phone})
+
+    def addGroup(self, title, users_chat_id):
+        return Bot._create(self.auth, "addGroup", {"title": title, "member_guids": users_chat_id})
+
+    def addChannel(self, title, channelType="Public", users_chat_id=None):
+        return Bot._create(self.auth, "addChannel", {"channel_type": channelType, "title": title, "member_guids": users_chat_id or []})
+
+    def addFolder(self, name, exclude_chat_types=[], exclude_object_guids=[], include_chat_types=[], include_object_guids=[], is_add_to_top=True, folder_id=""):
+        return Bot._create(self.auth, "addFolder", dict(exclude_object_guids=exclude_object_guids, include_object_guids=include_object_guids, exclude_chat_types=exclude_chat_types, include_chat_types=include_chat_types, folder_id=folder_id, is_add_to_top=is_add_to_top, name=name))
 
-    def editMessage(self, message_id, chat_id:str, newText:str, metadata:list=None, parse_mode:str=None) -> dict:
+
+    def banMember(self, chat_id, member_id):
+        return Bot._create(self.auth, f"ban{Bot._chatDetection(chat_id)}Member", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guid": member_id, "action": "Set"})
+
+    def block(self, chat_id):
+        return Bot._create(self.auth, "setBlockUser", {"action": "Block", "user_guid": chat_id})
+
+
+    @staticmethod
+    def _create(auth, method, data, client=clients.web):
+        print(auth, Bot.privateKey)
+        return makeData(auth, encryption(encryption.changeAuthType(auth), private_key=Bot.privateKey), method, dict(data))
+
+    @staticmethod
+    def _createTMP(method, data, tmp=None):
+        return makeTmpData(method, dict(data), tmp=tmp, url=_getURL(DCsURL=Bot.DCsURL, getDCsURL=Bot.getDCsURL, dc_id=None))
+
+    @staticmethod
+    def _chatDetection(chat_id):
+        return Tools.chatDetection(chat_id)
+
+    def changeLink(self, chat_id):
+        return Bot._create(self.auth, f"set{Bot._chatDetection(chat_id)}Link", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id})
+
+    def changePassword(self, hint, newPass, oldPass):
+        return Bot._create(self.auth, "changePassword", {"new_hint": hint, "new_password": newPass, "password": oldPass})
+
+    def checkPassword(self, password):
+        return Bot._create(self.auth, "checkTwoStepPasscode", {"password": password}).get("data").get("is_vaild")
+
+
+    def deleteContact(self, chat_id):
+        return Bot._create(self.auth, "deleteContact", {"user_guid": chat_id})
+
+    def deleteMessages(self, chat_id, message_ids):
+        return Bot._create(self.auth, "deleteMessages", {"object_guid": chat_id, "message_ids": list(message_ids), "type": "Global"})
+
+    def deleteAdmin(self, chat_id, member_id):
+        return Bot._create(self.auth, f"set{Bot._chatDetection(chat_id)}Admin", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "action": "UnsetAdmin", "member_guid": member_id})
+
+    def deleteAvatar(self, chat_id, avatar_id):
+        return Bot._create(self.auth, "deleteAvatar", {"object_guid": chat_id, "avatar_id": avatar_id})
+
+    def deleteChatHistory(self, chat_id, lastMessageId):
+        return Bot._create(self.auth, "deleteChatHistory", {"object_guid": chat_id, "last_message_id": lastMessageId})
+
+    def deleteFolder(self, folder_id):
+        return Bot._create(self.auth, "deleteFolder", dict(folder_id=folder_id))
+
+    def deleteUserChat(self, chat_id, lastMessageID):
+        return Bot._create(self.auth, "deleteUserChat", {"last_deleted_message_id": lastMessageID, "user_guid": chat_id})
+
+    def download(self, chat_id, message_id, save=True, saveAs=None, logging=True):
+        return download(self, chat_id, message_id, save, saveAs, logging)
+
+    def disablePassword(self, password):
+        return Bot._create(self.auth, "turnOffTwoStep", {"password": password})
+
+
+    def editMessage(self, message_id, chat_id: str, newText: str, metadata: list = None, parse_mode: str = None) -> dict:
         metadata, newText = Bot.loadMetadata(metadata, parse_mode, newText)
-        return Bot._create(5, self.auth, "editMessage", {"message_id": message_id, "object_guid": chat_id, "text": newText, "metadata": metadata})
+        return Bot._create(self.auth, "editMessage", {"message_id": message_id, "object_guid": chat_id, "text": newText, "metadata": metadata})
+
     def editFolder(self, **kwargs):
         '''
         exclude_chat_types: (list) types that should never apply
         include_chat_types: (list) types that should always apply
         exclude_object_guids: (list) items that should never apply
         include_object_guids: (list) items that should always apply
         folder_id: (str) id of the target folder
         name: (str) name of the target folder
         '''
         kwargs["update_parameters"] = [i for i in kwargs.keys() if "clude" in i]
-        return Bot._create(5, self.auth, "editFolder", kwargs, clients.android)
-    editVoiceChat = lambda self, chat_id, voice_chat_id, title: Bot._create(5, self.auth, f"set{Bot._chatDetection(chat_id)}VoiceChatSetting", {f"{Bot._chatDetection(chat_id).lower()}_guid":chat_id, "voice_chat_id" : voice_chat_id, "title" : title, "updated_parameters": ["title"]})
+        return Bot._create(self.auth, "editFolder", kwargs)
+
+    def editVoiceChat(self, chat_id, voice_chat_id, title):
+        return Bot._create(self.auth, f"set{Bot._chatDetection(chat_id)}VoiceChatSetting", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "voice_chat_id": voice_chat_id, "title": title, "updated_parameters": ["title"]})
+
     def editChatInfo(self, chat_id, **kwargs):
         chat = Bot._chatDetection(chat_id)
         data, result = {f"{chat.lower()}_guid": chat_id}, []
         if "username" in list(kwargs.keys()):
-            result.append(Bot._create(4, self.auth, "updateChannelUsername", {"channel_guid": chat_id, "username": kwargs.get("username").replace("@", ""), "updated_parameters":["username"]}))
+            result.append(Bot._create(self.auth, "updateChannelUsername", {"channel_guid": chat_id, "username": kwargs.get(
+                "username").replace("@", ""), "updated_parameters": ["username"]}))
             kwargs.pop("username")
         if kwargs != {} and not 'username' in kwargs.keys():
-            for k,v in kwargs.items(): data[k] = v
-            result.append(Bot._create(5, self.auth, f"edit{chat}Info", dict(channel_guid=chat_id, **kwargs, updated_parameters=list(kwargs.keys()))))
+            for k, v in kwargs.items():
+                data[k] = v
+            result.append(Bot._create(self.auth, f"edit{chat}Info", dict(
+                channel_guid=chat_id, **kwargs, updated_parameters=list(kwargs.keys()))))
         return result
-    def editProfile(self, **kwargs) -> list :
-        result:list = []
+
+    def editProfile(self, **kwargs) -> list:
+        result: list = []
         if "username" in list(kwargs.keys()):
-            result.append(Bot._create(4, self.auth, "updateUsername", {"username": kwargs.get("username"), "updated_parameters":["username"]}))
+            result.append(Bot._create(self.auth, "updateUsername", {
+                          "username": kwargs.get("username"), "updated_parameters": ["username"]}))
             kwargs.pop("username")
-        if kwargs != {} and not 'username' in kwargs.keys(): result.append(Bot._create(4, self.auth, "updateProfile", {"first_name": kwargs.get("first_name"),"last_name": kwargs.get("last_name"),"bio": kwargs.get("bio"),"updated_parameters":list(kwargs.keys())}))
+        if kwargs != {} and not 'username' in kwargs.keys():
+            result.append(Bot._create(self.auth, "updateProfile", {"first_name": kwargs.get("first_name"), "last_name": kwargs.get(
+                "last_name"), "bio": kwargs.get("bio"), "updated_parameters": list(kwargs.keys())}))
         return result
 
-    forwardMessages = lambda self, From, message_ids, to: Bot._create(5, self.auth, "forwardMessages", {"from_object_guid": From,"message_ids": message_ids,"rnd": f"{randint(100000,999999999)}","to_object_guid": to})
-    finishVoiceChat = lambda self, chat_id, voice_chat_id: Bot._create(5, self.auth, f"discard{Bot._chatDetection(chat_id)}VoiceChat", {f"{Bot._chatDetection(chat_id).lower()}_guid":chat_id, "voice_chat_id" : voice_chat_id})
 
-    getMe                      = lambda self, myGuid=None: Bot.getInfo(self, myGuid or loads(open(self.appName+".json","rt").read()).get("data").get("user").get("user_guid"))
-    getChats                   = lambda self, start_id=None: Bot._create(5, self.auth, "getChats", {"start_id": start_id})
-    getMessages                = lambda self, chat_id, min_id, start_id=None: Bot._create(5, self.auth, "getMessagesInterval", {"object_guid": chat_id,"middle_message_id": min_id,"start_id": start_id}).get("data").get("messages")
-    getLastMessage             = lambda self, chat_id:                Bot.getMessages(self, chat_id, Bot.getInfo(self, chat_id)["chat"]["last_message"]["message_id"])[-1] # it isn't a server method , is a shortcut
-    getInfoByUsername          = lambda self, username:               Bot._create(5, self.auth, "getObjectByUsername", {"username": username.replace("@","")})
-    getBlacklist               = lambda self, chat_id, start_id=None: Bot._create(5, self.auth, f"getBanned{Bot._chatDetection(chat_id)}Members", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "start_id":start_id}).get("data")
-    getMyBlacklist             = lambda self, start_id=None:          Bot._create(4, self.auth, "getBlockedUsers", {"start_id": start_id})
-    getAdmins                  = lambda self, chat_id, start_id=None: Bot._create(5, self.auth, f"get{Bot._chatDetection(chat_id)}AdminMembers", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "start_id":start_id})
-    getMessagesInfo            = lambda self, chat_id, message_ids:   Bot._create(5, self.auth, "getMessagesByID", {"object_guid": chat_id,"message_ids": list(message_ids)}).get("data").get("messages")
-    getMembers                 = lambda self, chat_id, search_text=None, start_id=None: Bot._create(5, self.auth, f"get{Bot._chatDetection(chat_id)}AllMembers", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "search_text": search_text, "start_id": start_id})
-    getInfo                    = lambda self, chat_id: Bot._create(5, self.auth, f"get{Bot._chatDetection(chat_id)}Info", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id}).get("data")
-    getLink                    = lambda self, chat_id: Bot._create(5, self.auth, f"get{Bot._chatDetection(chat_id)}Link", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id}).get("data").get("join_link")
-    getPreviewByJoinLink       = lambda self, link:    Bot._create(5, self.auth, f"{'group' if 'joing' in link else 'channel'}PreviewByJoinLink", {"hash_link": link.split("/")[-1]})
-    getChatAds                 = lambda self:          Bot._create(5, self.auth, "getChatAds", {"state": round(datetime.today().timestamp()) - 200 }).get("data")
-    getChatsUpdate             = lambda :              Bot._create(5, self.auth, "getChatsUpdates", {"state": round(datetime.today().timestamp()) - 200 }).get("data")
-    getChatUpdate              = lambda self, chat_id: Bot._create(5, self.auth, "getMessagesUpdates", {"object_guid":chat_id,"state": round(datetime.today().timestamp()) - 200 })
-    getMyStickerSet            = lambda self:          Bot._create(5, self.auth, "getMyStickerSets", {})
-    getAvatars                 = lambda self, chat_id: Bot._create(5, self.auth, "getAvatars", {"object_guid": chat_id})
-    getPollStatus              = lambda self, poll_id: Bot._create(5, self.auth, "getPollStatus", {"poll_id":str(poll_id)})
-    getPollOptionVoters        = lambda self, poll_id, option_index, start_id=None: Bot._create(5, self.auth, "getPollOptionVoters", {"poll_id":poll_id,"selection_index": option_index,"start_id": start_id})
-    getPostByLink              = lambda self, link:    Bot._create(5, self.auth, "getLinkFromAppUrl", {"app_url": link})["data"]["link"]["open_chat_data"]
-    getUserCommonGroups        = lambda self, chat_id: Bot._create(4, self.auth, "getCommonGroups", {"user_guid": chat_id})
-    getGroupOnlineMembersCount = lambda self, chat_id: Bot._create(4, self.auth, "getGroupOnlineCount", {"group_guid": chat_id}).get("online_count")
-    getTwoPasscodeStatus       = lambda self:          Bot._create(4, self.auth, "getTwoPasscodeStatus", {})
-    getPrivacySetting          = lambda self:          Bot._create(4, self.auth, "getPrivacySetting", {})
-    getNotificationSetting     = lambda self:          Bot._create(4, self.auth, "getNotificationSetting", {}).get("notification_setting")
-    getSuggestedFolders        = lambda self:          Bot._create(4, self.auth, "getSuggestedFolders", {}, clients.android)
-    getFolders                 = lambda self:          Bot._create(4, self.auth, "getFolders", {}, clients.android).get("folders")
-    getOwning                  = lambda self, chat_id: Bot._create(4, self.auth, "getPendingObjectOwner", {"object_guid": chat_id})
-    getMySessions              = lambda self:          Bot._create(5, self.auth, "getMySessions", {})
-    getContacts                = lambda self:          Bot._create(5, self.auth, "getContacts", {})
+    def forwardMessages(self, From, message_ids, to):
+        return Bot._create(self.auth, "forwardMessages", {"from_object_guid": From, "message_ids": message_ids, "rnd": f"{randint(100000,999999999)}", "to_object_guid": to})
+
+    def finishVoiceChat(self, chat_id, voice_chat_id):
+        return Bot._create(self.auth, f"discard{Bot._chatDetection(chat_id)}VoiceChat", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "voice_chat_id": voice_chat_id})
+
+
+    def getMe(self):
+        return Bot.getInfo(self)
+
+    def getChats(self, start_id=None):
+        return Bot._create(self.auth, "getChats", {"start_id": start_id})
+
+    def getMessages(self, chat_id, min_id, start_id=None):
+        return Bot._create(self.auth, "getMessagesInterval", {"object_guid": chat_id, "middle_message_id": min_id, "start_id": start_id}).get("data").get("messages")
+
+    def getLastMessage(self, chat_id):
+        return Bot.getMessages(self, chat_id, Bot.getInfo(self, chat_id)["chat"]["last_message"]["message_id"])[-1]  # it isn't a server method , is a shortcut
+
+    def getInfoByUsername(self, username):
+        return Bot._create(self.auth, "getObjectByUsername", {"username": username.replace("@", "")})
+
+    def getBlacklist(self, chat_id, start_id=None):
+        return Bot._create(self.auth, f"getBanned{Bot._chatDetection(chat_id)}Members", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "start_id": start_id}).get("data")
+
+    def getContactsUpdates(self):
+        return Bot._create(self.auth, "getContactsUpdates", {"state": round(datetime.today().timestamp()) - 200})
+
+    def getMyBlacklist(self, start_id=None):
+        return Bot._create(self.auth, "getBlockedUsers", {"start_id": start_id})
+
+    def getAbsObjects(self, chat_ids):
+        return Bot._create(self.auth, "getAbsObjects", {"object_guids": chat_ids})
+
+    def getAdmins(self, chat_id, start_id=None):
+        return Bot._create(self.auth, f"get{Bot._chatDetection(chat_id)}AdminMembers", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "start_id": start_id})
+
+    def getAdminAccesses(self, chat_id, admin_guid):
+        return Bot._create(self.auth, f"get{Bot._chatDetection(chat_id)}AdminAccessList", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guid": admin_guid})
+
+    def getMessagesInfo(self, chat_id, message_ids):
+        return Bot._create(self.auth, "getMessagesByID", {"object_guid": chat_id, "message_ids": list(message_ids)}).get("data").get("messages")
+
+    def getMembers(self, chat_id, search_text=None, start_id=None):
+        return Bot._create(self.auth, f"get{Bot._chatDetection(chat_id)}AllMembers", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "search_text": search_text, "start_id": start_id})
+
+    def getInfo(self, chat_id=None):
+        return Bot._create(self.auth, f"get{'User' if chat_id is None else Bot._chatDetection(chat_id)}Info", {} if chat_id is None else {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id}).get("data")
+
+    def getLink(self, chat_id):
+        return Bot._create(self.auth, f"get{Bot._chatDetection(chat_id)}Link", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id}).get("data").get("join_link")
+
+    def getPreviewByJoinLink(self, link):
+        return Bot._create(self.auth, f"{'group' if 'joing' in link else 'channel'}PreviewByJoinLink", {"hash_link": link.split("/")[-1]})
+
+    def getChatAds(self):
+        return Bot._create(self.auth, "getChatAds", {"state": round(datetime.today().timestamp()) - 200}).get("data")
+
+    def getChatsUpdate(self):
+        return Bot._create(self.auth, "getChatsUpdates", {"state": round(datetime.today().timestamp()) - 200}).get("data")
+
+    def getChatUpdate(self, chat_id):
+        return Bot._create(self.auth, "getMessagesUpdates", {"object_guid": chat_id, "state": round(datetime.today().timestamp()) - 200})
+
+    def getGroupMentionList(self, group_guid, mention_text):
+        return Bot._create(self.auth, "getGroupMentionList", {"group_guid": group_guid, "search_mention": mention_text})
+
+    def getGroupDefaultAccess(self, group_guid):
+        return Bot._create(self.auth, "getGroupDefaultAccess", {"group_guid": group_guid})
+
+    def getMyStickerSet(self):
+        return Bot._create(self.auth, "getMyStickerSets", {})
+
+    def getAvatars(self, chat_id):
+        return Bot._create(self.auth, "getAvatars", {"object_guid": chat_id})
+
+    def getPollStatus(self, poll_id):
+        return Bot._create(self.auth, "getPollStatus", {"poll_id": str(poll_id)})
+
+    def getPollOptionVoters(self, poll_id, option_index, start_id=None):
+        return Bot._create(self.auth, "getPollOptionVoters", {"poll_id": poll_id, "selection_index": option_index, "start_id": start_id})
+
+    def getPostByLink(self, link):
+        return Bot._create(self.auth, "getLinkFromAppUrl", {"app_url": link})["data"]["link"]["open_chat_data"]
+
+    def getUserCommonGroups(self, chat_id):
+        return Bot._create(self.auth, "getCommonGroups", {"user_guid": chat_id})
+
+    def getGroupOnlineMembersCount(self, chat_id):
+        return Bot._create(self.auth, "getGroupOnlineCount", {"group_guid": chat_id}).get("online_count")
+
+    def getTwoPasscodeStatus(self):
+        return Bot._create(self.auth, "getTwoPasscodeStatus", {})
 
-    invite = lambda self, chat_id, user_ids: Bot._create(5, self.auth, f"add{Bot._chatDetection(chat_id)}Members", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guids": user_ids})
+    def getPrivacySetting(self):
+        return Bot._create(self.auth, "getPrivacySetting", {})
 
-    join   = lambda self, value: Bot._create(5, self.auth, "joinChannelAction", {"action": "Join","channel_guid": value}) if value.startswith("c") else Bot._create(5, self.auth, "joinGroup", {"hash_link": value.split("/")[-1]})
+    def getNotificationSetting(self):
+        return Bot._create(self.auth, "getNotificationSetting", {}).get("notification_setting")
+
+    def getSuggestedFolders(self):
+        return Bot._create(self.auth, "getSuggestedFolders", {})
+
+    def getFolders(self):
+        return Bot._create(self.auth, "getFolders", {}).get("folders")
+
+    def getOwning(self, chat_id):
+        return Bot._create(self.auth, "getPendingObjectOwner", {"object_guid": chat_id})
+
+    def getMySessions(self):
+        return Bot._create(self.auth, "getMySessions", {})
+
+    def getContacts(self, start_id=None):
+        return Bot._create(self.auth, "getContacts", {"start_id": start_id})
+
+
+    def invite(self, chat_id, user_ids):
+        return Bot._create(self.auth, f"add{Bot._chatDetection(chat_id)}Members", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guids": user_ids})
+
+
+    def join(self, value):
+        return Bot._create(self.auth, "joinChannelAction", {"action": "Join", "channel_guid": value}) if value.startswith("c") else Bot._create(self.auth, "joinGroup", {"hash_link": value.split("/")[-1]})
+
+
+    def logout(self):
+        return Bot._create(self.auth, "logout", {})
+
+    def leave(self, chat_id):
+        return Bot._create(self.auth, "joinChannelAction", {"action": "Leave", "channel_guid": chat_id}) if chat_id.startswith("c") else Bot._create(self.auth, "leaveGroup", {"group_guid": chat_id})
 
-    logout = lambda self: Bot._create(5, self.auth, "logout", {})
-    leave  = lambda self, chat_id: Bot._create(5, self.auth, "joinChannelAction", {"action": "Leave","channel_guid": chat_id}) if chat_id.startswith("c") else Bot._create(5, self.auth, "leaveGroup", {"group_guid": chat_id})
     @staticmethod
     def loadMetadata(metadata, parse_mode, text) -> tuple:
-        if metadata is not None : metadata = {"meta_data_parts":metadata}
-        if parse_mode is not None :
+        if metadata is not None:
+            metadata = {"meta_data_parts": metadata}
+        if parse_mode is not None:
             parsedResult = Tools.parse(parse_mode, text)
-            metadata, text = {"meta_data_parts": parsedResult["metadata"]}, parsedResult["realText"]
+            metadata, text = {
+                "meta_data_parts": parsedResult["metadata"]}, parsedResult["realText"]
         return metadata if metadata != {"meta_data_parts": []} else None, text
 
-    muteChat = lambda self, chat_id: Bot._create(5, self.auth, "setActionChat", {"action": "Mute", "object_guid": chat_id})
 
-    pin = lambda self, chat_id, message_id: Bot._create(4, self.auth, "setPinMessage", {"action":"Pin","message_id": message_id,"object_guid": chat_id})
+    def muteChat(self, chat_id):
+        return Bot._create(self.auth, "setActionChat", {"action": "Mute", "object_guid": chat_id})
+
+
+    def pin(self, chat_id, message_id):
+        return Bot._create(self.auth, "setPinMessage", {"action": "Pin", "message_id": message_id, "object_guid": chat_id})
+
+    @staticmethod
+    def registerDevice(auth, device=defaultDevice):
+        return Bot._create(auth, "registerDevice", device)
+
+    def reportChat(self, chat_id, reportType=106, description=None):
+        return Bot._create(self.auth, "reportObject", {"object_guid": chat_id, "report_description": description, "report_type": reportType, "report_type_object": "Object"})
+
+    def removeChat(self, chat_id):
+        return Bot._create(self.auth, f"remove{Bot._chatDetection(chat_id)}", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id})
+
+    def requestSendFile(self, file, size=None):
+        return requestSendFile(self, file, int(size))
 
-    registerDevice  = lambda auth, device=defaultDevice: Bot._create(5, auth, "registerDevice", device)
-    reportChat      = lambda self, chat_id, reportType=106, description=None: Bot._create(4, self.auth, "reportObject", {"object_guid": chat_id, "report_description": description, "report_type": reportType, "report_type_object": "Object"})
-    removeChat      = lambda self, chat_id: Bot._create(4, self.auth, f"remove{Bot._chatDetection(chat_id)}", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id})
-    requestSendFile = lambda self, file, size=None: requestSendFile(self, file, int(size))
     def resendMessage(self, From, message_id, To, **kwargs):
         message = Bot.getMessagesInfo(self, From, [str(message_id)])[0]
-        for key,value in kwargs.items(): message[key] = value
-        return Bot._create(5, self.auth, "sendMessage", dict(object_guid=To, rnd=str(randint(100000,999999999)), **message))
+        for key, value in kwargs.items():
+            message[key] = value
+        return Bot._create(self.auth, "sendMessage", dict(object_guid=To, rnd=str(randint(100000, 999999999)), **message))
 
-    sendCode = lambda phoneNumber: Bot._createTMP("sendCode", {"phone_number":f"98{phoneNumber[1:]}", "send_type":"SMS"})
-    signIn   = lambda phoneNumber, phone_code_hash, phone_code: Bot._createTMP("signIn", { "phone_number": f"98{phoneNumber[1:]}", "phone_code_hash": phone_code_hash, "phone_code": phone_code })
+    @staticmethod
+    def sendCode(phoneNumber, passKey=None, Type="SMS"):
+        return Bot._createTMP("sendCode", {"phone_number": f"98{phoneNumber[1:]}", "pass_key": passKey, "send_type": Type})
 
-    def setAsShad(self): clients.web["app_version"], clients.web["package"], clients.android["package"], Bot.wsURL, Bot.DCsURL, Bot.getDCsURL, Bot.downloadURL = "3.2.2", "web.shad.ir", "ir.medu.shad", "wss://shsocket1.iranlms.ir:80", "https://shadmessengerX.iranlms.ir/", "https://shgetdcmess.iranlms.ir", "https://shstX.iranlms.ir/GetFile.ashx"
+    @staticmethod
+    def signIn(tmp, phoneNumber, phone_code_hash, phone_code):
+        public, private = encryption.rsaKeyGenerate()
+        resp = Bot._createTMP("signIn", {"phone_number": f"98{phoneNumber[1:]}", "phone_code_hash": phone_code_hash, "phone_code": phone_code, "public_key": public}, tmp=tmp)
+        if resp['status'] == "OK" and resp['data']['status'] == "OK":
+            resp['auth'] = encryption.decryptRsaOaep(private, resp['data']['auth'])
+            resp['private'] = private
+        return resp
 
-    def sendMessage(self, chat_id:str, text:str, metadata:list=None, parse_mode:str=None, message_id=None) -> dict:
+    def sendMessage(self, chat_id: str, text: str, metadata: list = None, parse_mode: str = None, message_id=None) -> dict:
         metadata, text = Bot.loadMetadata(metadata, parse_mode, text)
-        return Bot._create(5, self.auth, "sendMessage", {"object_guid":chat_id,"rnd":f"{randint(100000,999999999)}","text":text, "metadata":metadata,"reply_to_message_id":message_id})
+        return Bot._create(self.auth, "sendMessage", {"object_guid": chat_id, "rnd": f"{randint(100000,999999999)}", "text": text, "metadata": metadata, "reply_to_message_id": message_id})
 
-    def sendPhoto(self, chat_id:str, file:str, size:list=None, thumbnail:str="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", metadata:list=None, parse_mode:str=None, caption:str=None, message_id=None, uresponse:list=None) -> dict :
+    def sendPhoto(self, chat_id: str, file: str, size: list = None, thumbnail: str = "iVBORw0KGgoAAAANSUhEUgAAABwAAAAoCAYAAADt5povAAAAAXNSR0IArs4c6QAACmpJREFUWEfNVwl0U1Ua/u57ycuetGmatOneJt0prWUpYEVBkB0dQFkcGQRRYZwB5AyLy3gAHSgqjqgjokg944oiCiguI6ioFbpQSimFlkK3hO5p0uzv3TkJTaciwsyZOZ6557yTd/Lu/b97/+X7v0vwKw/yK+Ph/xowsLnBT8g5AgDa/1zXYdc7YQggYChg+FqD6f94TfBrAYYMBICY+CHQxMch1WBAMsSItHhBHS60e7pQZ7Wi3laF7n7A0CavusGrAQ4syJloUAzPtRVk3uBdlGgWbtGoEe0lhJzpJWjsoyCEAjz87l5YeprwVWMpir/bha/73Ruw87PTXgkYBJsDkNwnkrKSRrhWac3dcyjvlfs9QKcLtLaH+m0eCCwDuCEibqJkfIxcRMUS8IKiu6sj+kBtif6llu1vlvTHPHDwAHBwDAYMgi3NV2nnptH5eaOFVfXDnAnnJRA4P/ztHrC1Lpa1IBItJBdNfBY6fFFw+pXUB4kfrIRCJmWIXiViFeJmtqL6ec+KzS+gudk9KLYDgAEw5pmbYBytx+qCFDzUlQpUZoLvlhLSzrPsjw69UNmR333OktFgd6ic4MQM4rUGkmyMITqNXBCDgvoovELgIYRle0lL29+FxY89gro6ewh0IM2fGA79bUl4aGQM1nnDCG3PA62Mp0yrn3F9eVx2/JtDxmJrGVOGTns3XK1NQQMmk0QplSZHJedOjkkZ+luanjj0fIqUt8RJBF7GssRPeklj2+vCsg3rcPq0P+Da4MkmGiArmoA7h4TjBV4EqS+V0LpsypSKcGHvO3j64B7sRiucMA6PA8+bcan8cH84BpIiT55nNEVmLkuIzf69PS1MWTFS7aseGcH0acVWlFRuxZ2rXgxgBU94bgFGqiXkpQglzaVK8H15YEq1qC4qxprP38Cn/e7gxIaZeUSpm8aLXRX8mbc+vKIMqE6nU+Sop842q5KKYjmZtsso9laO1QvnM1QnOoqeW+o4fLiaLDUadQvT2QdGJbg28MoOgYknxJJAzz7yBf5cvBPvA2BVKqPmxtvmLJw6Y/baEQXDdA2W5q4P93/27jsvPLkFbsvFwQyk1ZoUqZHjFiRpkp5JZgin8VO4ROhpE2yvvnhs83pSkTp2eHi4d3tswqVhQlyD4IqB/bSP7hy1BusDYMCI2El3zluz5L7bl44x29HTx/McQ5kezkg3f9773Z6181bCVlYxKONJetTNcRpV6toEbfrSBJGHalgR8fL+kv11ex8jlVk33ZOp4XbQyIsSJuMctUWTktm76NLDlagJAkrGxWeNmvRo/vS5C10RBqGqRcTGaCk1GQThZEPniR82zVuB7iPfBeKDAA1c/iUPZC8pdDOq112S6ASzROBZUGuTrelrcjRrzLYCteqPft1FwZd6pu+CnO4eshErBiWFFJEb5yK2cCfyC1koCIVHALzdvbCU7Man01f3F3aIxIOJuDHOlKhUmB7tVd6wsIYJEzIlgt8nCN3k1NDC/ely1WSfxiL0mqob32r1blq5F8X9O73Mh0pDJGdYeD8S71jPJ+VwqkgOUVxrl6V0317X969t93afPHUFkZD88HDV03FJi/TylKLt3gwfOIU8SQxKmnPHVhgkihyfsktwxNdU/anKtmp3aZAPA64JABKoJpmhLXwcKXPuQnoyYRQMI2MFKvG4qNR50WLmviwu3/3YNrvd3jnIM6LKQtPMeFHEayfs6eLXiYkoRTIpaRg2/lQ8y2X4xU449BeOLa66+OC+c6gctBDQry5gwsw75Lnjs0VmHbU51Yxe6qOpkk7UtzBEkUQ702yHdh7YsuiRQTRGTszUTojyad+Qd6VqD/sNfftpHMi6YQ+Xz+DsWfm0Hr2KnoolDWXL99WjfBAgo4yank5U+U+p0sdNl2cbhDq3mZWIKI2gF7uEH49YOyNuyVAMlZV6d81Y7mw6VtbvHXryXtwW7da/EdGYrfP7ON4J4iVTctaW5Ck1+TNR600Qztc9bq1Zs+NC++f9gMFemHdv8USX2/Dq+eaoaK85FdBKAIEKcF+qx6F1r4IkhkNfMB3tHz2LczsC8ScmE0TvTcRvMhnNLrY6Uyo4tJRhfYSMz/zDnhhl/B154j6+kD9rrb1UtnVBw5kgDV2OYaxUfNebc8AlvULrLRI+KoYiKRoEVAB/qZ4c2bqBP/Hch4BUD4gdQDCOzM35CH90BO67RaN40ldqBrHFgLC8QG5MW7bJoEpar2N5ZIqdzhTX6bemlb2/HECAbAODw5SjsyDSF6OpUUQ0OtCMbAqOoXBaK3Bw/gq0Hvl+kAQJlsXfFiNjiI48NUrMTfWVJQukPdntoW4LmZCx8g6pJOI1jmXCYiUiIZJ4Th6q/2DVUeuJf2Vq5O+GgjrmQVD1MQmz7gu/cWyMMVFCu9s6jze/PHU5bOUBpgkVPjEB4veKMM2kILvkDSKlUJdAXc2mC9/2WvaRkUn35Khk+i1qqWEiQ7xCDMd6xbxjz9PHNj2IQFO/PIIdWz/77dF5QxJemTIpP7Ozo8/n77tUVrRy8cP+lu8Hd3dmw0pkjDBiywQNmcSfYASmw0hcDRlfza8pXUF0ujRVRtTku7WymO2Mxw0pyyKMo229zvrn36zatTlEVQFQpSFFN+butUuih83Y0OnVMFG89dDOe4cuAGw9l3kXdNw0RM25FStnpWGVthwCbSFwuxXWqpMxfx1dWrs16G/lxNWZjDziL1qJYWpsaztvcPBMGPW3tjtqtn1c9/bz/RwZMIi8yfenRg4t2GDIGjbSWvLZzi9eXF0EwBeYkzMZsZOmYcX04ViRexZEfgrgbRA8DP4x5QAWfXsR1lDHF2HBtluhitghgig2vMfOx3a5GaPd2+vurP+o+sKXW63euuqQENJqtWqn0xnudrsDrQlIhDRvlGhkwXh+zbjhdHJaB2h6FSjOg/b5Sc07FXTdgz/g4EADDi6KzFSg8O67SFTKsxSCCpTnxX6B0booI+3tbrNfOn3A1l75Cd/edArE0Q51HKDWxMuzo28wj+iYPmbI6fGjozqVei+laY2UxlYCrjbSVN5Ki276GC+H6jqk2i6fNDlfhSFT55LotE2UMhHw+QRwIkApY6FWAWEyIFzkh4Z1ctJeJoY7Jc9gDzJZOIosro+Gi8Gr+0Dya8DSalw4VoeiCQcHwIJy5GcyEYmJnCR91ljGnPk4MUeOhpEIjBw+MeeiMrGdUaOFNfhPs0a+FGH+ehrJUr9JDaoWExZiyho9jDfuW/bH99+lTz50zB9irAHtczUhHCyDnAdG62OyHfOj09uXySQ2M/F6QLw8GH+QfihlgGgFIWlhBCqZAMoQoc8uOl9bzu34oIjZXXb2J53jqkI4lBM/Ech5MxAdZsbthgxMURtIDisjBk5MuCQZhUlOPX0OamltRGXtSXxa9g0+Of4NAhLyF+8X17rMXLmIRGZCIZXBwBCoFYFa8MDWY0VbezscVyq4X7q+Xe+6FrAT1CiDZMRgT4TeQ3NCMuNqc4L//TuAV7p6cGaHkmEgRr+IdIUGud68/9n3//SE/zXwrw74T3XSTDJjBhdXAAAAAElFTkSuQmCC", metadata: list = None, parse_mode: str = None, caption: str = None, message_id=None, uresponse: list = None) -> dict:
         # size = [width:int, height:int]
         uresponse = uresponse or Bot.uploadFile(self, file)
-        if "."  in thumbnail: thumbnail = str(Tools.getThumbInline(open(file,"rb").read() if not "http" in file else GET(file).content))
-        if size is None: size = Tools.getImageSize(open(file,"rb").read() if not "http" in file else GET(file).content)
+        if "." in thumbnail:
+            thumbnail = str(Tools.getThumbInline(open(file, "rb").read() if path.isfile(file) else len(file) if not "http" in file else GET(file).content))
+        if size is None:
+            size = Tools.getImageSize(open(file, "rb").read() if path.isfile(file) else len(file) if not "http" in file else GET(file).content)
         metadata, caption = Bot.loadMetadata(metadata, parse_mode, caption)
-        return Bot._create(5, self.auth, "sendMessage", {"file_inline": {"dc_id": uresponse[0]["dc_id"],"file_id": uresponse[0]["id"],"type":"Image","file_name": file.split("/")[-1],"size": str(len(GET(file).content if "http" in file else open(file,"rb").read())),"mime": file.split(".")[-1],"access_hash_rec": uresponse[1],"width": size[0],"height": size[1],"thumb_inline": thumbnail},"object_guid": chat_id, "text": caption, "metadata": metadata,"rnd": f"{randint(100000,999999999)}","reply_to_message_id": message_id})
+        return Bot._create(self.auth, "sendMessage", {"file_inline": {"dc_id": uresponse[0]["dc_id"], "file_id": uresponse[0]["id"], "type": "Image", "file_name": file.split("/")[-1], "size": str(len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file))), "mime": file.split(".")[-1], "access_hash_rec": uresponse[1], "width": size[0], "height": size[1], "thumb_inline": thumbnail}, "object_guid": chat_id, "text": caption, "metadata": metadata, "rnd": f"{randint(100000,999999999)}", "reply_to_message_id": message_id})
 
-    def sendVideo(self, chat_id:str, file:str, width:int=720, height:int=720, metadata:list=None, parse_mode:str=None, caption=None, message_id=None, uresponse:list=None):
-        from tinytag import TinyTag # pip install tinytag
+    def sendVideo(self, chat_id: str, file: str, width: int = 720, height: int = 720, metadata: list = None, parse_mode: str = None, caption=None, message_id=None, uresponse: list = None):
+        from tinytag import TinyTag  # pip install tinytag
         uresponse, metadata, caption = uresponse or Bot.uploadFile(self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
-        return Bot._create(4, self.auth, "sendMessage", {"file_inline":{"access_hash_rec":uresponse[1],"auto_play":False,"dc_id":uresponse[0]["dc_id"],"file_id":str(uresponse[0]["id"]),"file_name":file.split("/")[-1],"height":height,"mime":file.split(".")[-1],"size":str(len(GET(file).content if "http" in file else open(file,"rb").read())),"thumb_inline":file,"time":round(TinyTag.get(file).duration * 1000),"type":"Video","width":width},"is_mute":False,"object_guid":chat_id, "text": caption, "metadata": metadata, "rnd":str(randint(100000,999999999)), "reply_to_message_id":message_id})
+        return Bot._create(self.auth, "sendMessage", {"file_inline": {"access_hash_rec": uresponse[1], "auto_play": False, "dc_id": uresponse[0]["dc_id"], "file_id": str(uresponse[0]["id"]), "file_name": file.split("/")[-1], "height": height, "mime": file.split(".")[-1], "size": str(len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file))), "thumb_inline": file, "time": round(TinyTag.get(file).duration * 1000), "type": "Video", "width": width}, "is_mute": False, "object_guid": chat_id, "text": caption, "metadata": metadata, "rnd": str(randint(100000, 999999999)), "reply_to_message_id": message_id})
 
-    def sendMusic(self, chat_id:str, file:str, metadata:list=None, parse_mode:str=None, caption=None, message_id=None, uresponse:list=None):
-        from tinytag import TinyTag # pip install tinytag
+    def sendMusic(self, chat_id: str, file: str, metadata: list = None, parse_mode: str = None, caption=None, message_id=None, uresponse: list = None):
+        from tinytag import TinyTag  # pip install tinytag
         uresponse, metadata, caption = uresponse or Bot.uploadFile(self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
-        return Bot._create(4, self.auth, "sendMessage", {"file_inline":{"access_hash_rec":uresponse[1], "auto_play":False, "dc_id":uresponse[0]["dc_id"], "file_id":str(uresponse[0]["id"]),"file_name":file.split("/")[-1],"height":0.0,"mime":file.split(".")[-1],"music_performer": str(TinyTag.get(file).artist),"size": len(GET(file).content if "http" in file else open(file,"rb").read()),"time": round(TinyTag.get(file).duration),"type":"Music","width":0.0},"is_mute":False,"object_guid":chat_id, "text": caption, "metadata": metadata,"rnd":randint(100000,999999999),"reply_to_message_id":message_id})
+        return Bot._create(self.auth, "sendMessage", {"file_inline": {"access_hash_rec": uresponse[1], "auto_play": False, "dc_id": uresponse[0]["dc_id"], "file_id": str(uresponse[0]["id"]), "file_name": file.split("/")[-1], "height": 0.0, "mime": file.split(".")[-1], "music_performer": str(TinyTag.get(file).artist), "size": len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file)), "time": round(TinyTag.get(file).duration), "type": "Music", "width": 0.0}, "is_mute": False, "object_guid": chat_id, "text": caption, "metadata": metadata, "rnd": randint(100000, 999999999), "reply_to_message_id": message_id})
 
-    def sendVoice(self, chat_id:str, file:str, time:int=None, metadata:list=None, parse_mode:str=None, caption:str=None, message_id=None, uresponse:list=None) -> dict :
+    def sendVoice(self, chat_id: str, file: str, time: int = None, metadata: list = None, parse_mode: str = None, caption: str = None, message_id=None, uresponse: list = None) -> dict:
         # file's format must be ogg. time must be ms (type: float).
-        uresponse, metadata, caption = uresponse or Bot.uploadFile(self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
+        uresponse, metadata, caption = uresponse or Bot.uploadFile(
+            self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
         if time is None:
-            from tinytag import TinyTag # pip install tinytag
+            from tinytag import TinyTag  # pip install tinytag
             time = round(TinyTag.get(file).duration)
-        return Bot._create(5, self.auth, "sendMessage", {"file_inline": {"dc_id": str(uresponse[0]["dc_id"]),"file_id": uresponse[0]["id"],"type":"Voice","file_name": file.split("/")[-1],"size": len(GET(file).content if "http" in file else open(file,"rb").read()),"time": float(time),"mime": file.split(".")[-1],"access_hash_rec": str(uresponse[1])},"object_guid":chat_id, "text": caption, "metadata": metadata, "rnd":f"{randint(100000,999999999)}","reply_to_message_id":message_id})
+        return Bot._create(self.auth, "sendMessage", {"file_inline": {"dc_id": str(uresponse[0]["dc_id"]), "file_id": uresponse[0]["id"], "type": "Voice", "file_name": file.split("/")[-1], "size": len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file)), "time": float(time), "mime": file.split(".")[-1], "access_hash_rec": str(uresponse[1])}, "object_guid": chat_id, "text": caption, "metadata": metadata, "rnd": f"{randint(100000,999999999)}", "reply_to_message_id": message_id})
 
-    def sendDocument(self, chat_id:str, file:str, caption:str=None, metadata:list=None, parse_mode:str = None, message_id=None, uresponse:list=None) -> dict :
+    def sendDocument(self, chat_id: str, file: str, caption: str = None, metadata: list = None, parse_mode: str = None, message_id=None, uresponse: list = None) -> dict:
         # Bot.sendDocument("guid","./file.txt", caption="anything", message_id="12345678")
-        uresponse, metadata, caption = uresponse or Bot.uploadFile(self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
-        return Bot._create(5, self.auth, "sendMessage", {"object_guid":chat_id, "metadata": metadata, "text": caption, "reply_to_message_id":message_id,"rnd":f"{randint(100000,999999999)}","file_inline":{"dc_id":str(uresponse[0]["dc_id"]),"file_id":str(uresponse[0]["id"]),"type":"File","file_name":file.split("/")[-1],"size":len(GET(file).content if "http" in file else open(file,"rb").read()),"mime":file.split(".")[-1],"access_hash_rec":uresponse[1]}})
-
-    sendLocation = lambda self, chat_id, location, message_id: Bot._create(4, self.auth, "sendMessage", {"is_mute": False,"object_guid":chat_id,"rnd":f"{randint(100000,999999999)}","location":{"latitude": location[0],"longitude": location[1]},"reply_to_message_id":message_id})
-
-    def sendGIF(self, chat_id:str, file:str, width:int, height:int, time:int=None, metadata:list=None, parse_mode:str=None, thumbnail:str=r"/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDACAWGBwYFCAcGhwkIiAmMFA0MCwsMGJGSjpQdGZ6eHJm\ncG6AkLicgIiuim5woNqirr7EztDOfJri8uDI8LjKzsb/2wBDASIkJDAqMF40NF7GhHCExsbGxsbG\nxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsb/wAARCAAyADIDASIA\nAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQA\nAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3\nODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWm\np6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEA\nAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSEx\nBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElK\nU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3\nuLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDXqCXo\nasVXk70DKwHNSBaRRzUgrnZqMUfMKtkcCq24KcmntdxgDmtIEyJ8UVB9ti9aKskmB4qJ/uk1L2qC\nZtsZpiII5P3hB6VDLOySZ7UyVJDEWWoXLGD5uoqFHQtvUnln3rkVB5bv3qqk3Y1filUKM09kCV2R\nfZ39aKtectFK7K5URwagzrila4klcJiqdtbsrA5q+jLE4ZhVXsyErq5bCFYAMVQuVYKVC9av/akc\ncGmy4ZeKaIaZgeWVlANX1jDKKbdRYYNQJQqdamRpAk8pfWiq/n+9FSWPtifM61LcdKKKctyIbEMJ\nO4c1oj7lFFUiWQXH+qNZLmiihjiNzRRRUlH/2Q==\n", caption:str=None, message_id:int=None, uresponse:list=None) -> dict :
-        uresponse, metadata, caption = uresponse or Bot.uploadFile(self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
-        if time is None :
-            from tinytag import TinyTag # pip install TinyTag
+        uresponse, metadata, caption = uresponse or Bot.uploadFile(
+            self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
+        return Bot._create(self.auth, "sendMessage", {"object_guid": chat_id, "metadata": metadata, "text": caption, "reply_to_message_id": message_id, "rnd": f"{randint(100000,999999999)}", "file_inline": {"dc_id": str(uresponse[0]["dc_id"]), "file_id": str(uresponse[0]["id"]), "type": "File", "file_name": file.split("/")[-1], "size": len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file)), "mime": file.split(".")[-1], "access_hash_rec": uresponse[1]}})
+
+    def sendLocation(self, chat_id, location, message_id):
+        return Bot._create(self.auth, "sendMessage", {"is_mute": False, "object_guid": chat_id, "rnd": f"{randint(100000,999999999)}", "location": {"latitude": location[0], "longitude": location[1]}, "reply_to_message_id": message_id})
+
+    def sendGIF(self, chat_id: str, file: str, width: int, height: int, time: int = None, metadata: list = None, parse_mode: str = None, thumbnail: str = r"/9j/4AAQSkZJRgABAQAAAQABAAD/2wBDACAWGBwYFCAcGhwkIiAmMFA0MCwsMGJGSjpQdGZ6eHJm\ncG6AkLicgIiuim5woNqirr7EztDOfJri8uDI8LjKzsb/2wBDASIkJDAqMF40NF7GhHCExsbGxsbG\nxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsbGxsb/wAARCAAyADIDASIA\nAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQA\nAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3\nODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWm\np6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEA\nAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSEx\nBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElK\nU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3\nuLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwDXqCXo\nasVXk70DKwHNSBaRRzUgrnZqMUfMKtkcCq24KcmntdxgDmtIEyJ8UVB9ti9aKskmB4qJ/uk1L2qC\nZtsZpiII5P3hB6VDLOySZ7UyVJDEWWoXLGD5uoqFHQtvUnln3rkVB5bv3qqk3Y1filUKM09kCV2R\nfZ39aKtectFK7K5URwagzrila4klcJiqdtbsrA5q+jLE4ZhVXsyErq5bCFYAMVQuVYKVC9av/akc\ncGmy4ZeKaIaZgeWVlANX1jDKKbdRYYNQJQqdamRpAk8pfWiq/n+9FSWPtifM61LcdKKKctyIbEMJ\nO4c1oj7lFFUiWQXH+qNZLmiihjiNzRRRUlH/2Q==\n", caption: str = None, message_id: int = None, uresponse: list = None) -> dict:
+        uresponse, metadata, caption = uresponse or Bot.uploadFile(
+            self, file), *Bot.loadMetadata(metadata, parse_mode, caption)
+        if time is None:
+            from tinytag import TinyTag  # pip install TinyTag
             time = round(TinyTag.get(file).duration * 1000)
-        return Bot._create(4, self.auth, "sendMessage", {"object_guid": chat_id,"is_mute": False,"rnd": randint(100000,999999999),"file_inline": {"access_hash_rec": str(uresponse[1]),"dc_id": str(uresponse[0]["dc_id"]),"file_id": int(uresponse[0]["id"]),"auto_play": False,"file_name": file.split("/")[-1],"width": width,"height": height,"mime": file.split(".")[-1],"size": len(GET(file).content if "http" in file else open(file,"rb").read()),"thumb_inline": thumbnail, "time": time, "type": "Gif"},"text": caption, "metadata": metadata, "reply_to_message_id": message_id})
+        return Bot._create(self.auth, "sendMessage", {"object_guid": chat_id, "is_mute": False, "rnd": randint(100000, 999999999), "file_inline": {"access_hash_rec": str(uresponse[1]), "dc_id": str(uresponse[0]["dc_id"]), "file_id": int(uresponse[0]["id"]), "auto_play": False, "file_name": file.split("/")[-1], "width": width, "height": height, "mime": file.split(".")[-1], "size": len(GET(file).content if "http" in file else open(file, "rb").read() if path.isfile(file) else len(file)), "thumb_inline": thumbnail, "time": time, "type": "Gif"}, "text": caption, "metadata": metadata, "reply_to_message_id": message_id})
 
-    def sendContact(self, chat_id:str, user_guid:str, phone:str, firstName:str, lastName:str=None, avatarFile:str=None, uresponse:list=None) -> dict:
+    def sendContact(self, chat_id: str, user_guid: str, phone: str, firstName: str, lastName: str = None, avatarFile: str = None, uresponse: list = None) -> dict:
         '''
         chat_id: destination guid for sending the contact
         user_guid: contact's guid
         phone: contact's phone number
         first_name: contact's first name
         '''
-        uresponse = Bot.uploadFile(self, avatarFile) if avatarFile is not None else uresponse or [{"dc_id": "702", "id": 2521972095}, "5653363141731050515439840306092021010915"]
-        avatar = {"access_hash_rec": str(uresponse[1]), "file_id": int(uresponse[0]["id"]),"auto_play": False,"dc_id": str(uresponse[0]["dc_id"]),"height": 0,"mime": "none","size": 10025 if uresponse[0]["id"] == 2521972095 else len(GET(avatarFile).content if "http" in avatarFile else open(avatarFile,"rb").read()),"time": 5,"type": "File","width": 0}
-        return Bot._create(4, self.auth, "sendMessage", {"is_mute": False, "message_contact": {"contactAbsObject": {"avatar_thumbnail": avatar,"first_name": firstName,"last_name": lastName or "","is_deleted": False,"is_verified": False,"object_guid": user_guid,"type": "User"},"first_name": firstName,"last_name": lastName or "","phone_number": "+98"+phone[1:],"user_guid": user_guid,"vcard": f"BEGIN:VCARD\nVERSION:3.0\nFN:{firstName}\nTEL;MOBILE:+98{phone[1:]}\nEND:VCARD"}, "object_guid": chat_id, "rnd": randint(100000, 999999999)})
-
-    setMembersAccess    = lambda self, chat_id, access_list: Bot._create(4, self.auth, "setGroupDefaultAccess", {"access_list": access_list, "group_guid": chat_id})
-    setGroupTimer       = lambda self, chat_id, time: Bot._create(5, self.auth, "editGroupInfo", {"group_guid": chat_id,"slow_mode": time,"updated_parameters":["slow_mode"]})
-    setAdmin            = lambda self, chat_id, member_id, access_list=None: Bot._create(5, self.auth, f"set{Bot._chatDetection(chat_id)}Admin", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "access_list": access_list or [], "action": "SetAdmin", "member_guid": member_id})
-    seenChats           = lambda self, seenList: Bot._create(5, self.auth, "seenChats", {"seen_list": dict(seenList)})
-    sendChatAction      = lambda self, chat_id, action: Bot._create(5, self.auth, "sendChatActivity", {"activity": action,"object_guid": chat_id}) #every some seconds before sending message this request should send. action can be : Typing, Recording, Uploading
-    sendPoll            = lambda self, chat_id, allows_multiple_answers, is_anonymous, options, question, Type="Regular", message_id=None: Bot._create(4, self.auth, "createPoll", {"allows_multiple_answers": bool(allows_multiple_answers), "is_anonymous": bool(is_anonymous), "object_guid": chat_id, "options": list(options), "question": question, "rnd": str(randint(100000, 999999999)), "type": Type, "reply_to_message_id": message_id})
-    sendQuiz            = lambda self, chat_id, correct_option_index, is_anonymous, options, question, Type="Quiz", message_id=None: Bot._create(4, self.auth, "createPoll", {"correct_option_index": int(correct_option_index), "is_anonymous": bool(is_anonymous), "object_guid": chat_id, "options": list(options), "question": question, "rnd": str(randint(100000, 999999999)), "type": Type, "reply_to_message_id": message_id})
-    searchGlobalObjects = lambda self, text, start_id=None: Bot._create(4, self.auth, "searchGlobalObjects", {"search_text":text, "start_id": start_id})
-    setPhoneVisibility  = lambda self, mode="Nobody": Bot._create(4, self.auth, "setSetting", {"settings": {"show_my_phone_number": mode}, "update_parameters": ["show_my_phone_number"]}) #mode = Nobody/Everybody/MyContacts
-    setOnlineVisibility = lambda self, mode="Everybody": Bot._create(4, self.auth, "setSetting", {"settings": {"show_my_last_online": mode}, "update_parameters": ["show_my_last_online"]}) #mode = Nobody/Everybody/MyContacts
-    setAvatarVisibility = lambda self, mode="Everybody": Bot._create(4, self.auth, "setSetting", {"settings": {"show_my_profile_photo": mode}, "update_parameters": ["show_my_profile_photo"]}) #mode = Everybody/MyContacts
-    setCallableBy       = lambda self, mode="MyContacts": Bot._create(4, self.auth, "setSetting", {"settings": {"can_called_by": mode}, "update_parameters": ["can_called_by"]}) #mode = Everybody/MyContacts
-    setForwardableBy    = lambda self, mode="Everybody": Bot._create(4, self.auth, "setSetting", {"settings": {"link_forward_message": mode}, "update_parameters": ["link_forward_message"]}) #mode = Nobody/Everybody/MyContacts
-    setJoinableBy       = lambda self, mode="MyContacts": Bot._create(4, self.auth, "setSetting", {"settings": {"can_join_chat_by": mode}, "update_parameters": ["can_join_chat_by"]}) #mode = Everybody/MyContacts
-    setMyAutoDeleteTime = lambda self, time=24: Bot._create(4, self.auth, "setSetting", {"settings": {"delete_account_not_active_months": str(time)}, "update_parameters": ["show_my_phone_number"]}) #time = 3/6/12/24 , type: str/int, duration: months
-    setNotifications    = lambda self, user_message_preview=True, group_message_preview=False, channel_message_preview=False, in_app_sound=True, new_contacts=False, user_notification=True, group_notification=False, channel_notification=False, update_parameters=["user_message_preview", "in_app_sound", "user_notification"] : Bot._create(4, self.auth, "setSetting", {"settings": {"user_message_preview": user_message_preview, "user_notification": user_notification, "group_message_preview": group_message_preview, "group_notification": group_notification, "channel_message_preview": channel_message_preview, "channel_notification": channel_notification, "in_app_sound": in_app_sound, "new_contacts": new_contacts}, "update_parameters": update_parameters})
-    setOwning           = lambda self, chat_id, newOwnerGuid: Bot._create(4, self.auth, "requestChangeObjectOwner", {"object_guid": chat_id, "new_owner_user_guid": newOwnerGuid})
-    startVoiceChat      = lambda self, chat_id: Bot._create(5, self.auth, f"create{Bot._chatDetection(chat_id)}VoiceChat", {"object_guid": chat_id})
-
-    terminateOtherSessions = lambda self: Bot._create(5, self.auth, "terminateOtherSessions", {})
-
-    unbanMember  = lambda self, chat_id, member_id: Bot._create(5, self.auth, f"ban{Bot._chatDetection(chat_id)}Member", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guid": member_id, "action":"Unset"})
-    unpin        = lambda self, chat_id, message_id: Bot._create(4, self.auth, "setPinMessage", {"action":"Unpin","message_id": message_id,"object_guid": chat_id})
-    unblock      = lambda self, chat_id: Bot._create(5, self.auth, "setBlockUser", {"action": "Unblock","user_guid": chat_id})
-    unmuteChat   = lambda self, chat_id: Bot._create(5, self.auth, "setActionChat", {"action": "Unmute", "object_guid": chat_id})
-    uploadAvatar = lambda self, chat_id, main, thumbnail="": Bot._create(5, self.auth, "uploadAvatar", {"object_guid": chat_id, "thumbnail_file_id": str(Bot.uploadFile(self, thumbnail or main)[0]["id"]), "main_file_id": str(Bot.uploadFile(self, main)[0]["id"])})
-    uploadFile   = lambda self, file, frequest=None, logging=False: uploadFile(self, file, frequest, logging)
+        uresponse = Bot.uploadFile(self, avatarFile) if avatarFile is not None else uresponse or [
+            {"dc_id": "702", "id": 2521972095}, "5653363141731050515439840306092021010915"]
+        avatar = {"access_hash_rec": str(uresponse[1]), "file_id": int(uresponse[0]["id"]), "auto_play": False, "dc_id": str(uresponse[0]["dc_id"]), "height": 0, "mime": "none", "size": 10025 if str(uresponse[0]["id"]) == "2521972095" else len(GET(avatarFile).content if "http" in avatarFile else open(avatarFile, "rb").read() if path.isfile(avatarFile) else len(avatarFile)), "time": 0, "type": "File", "width": 0}
+        return Bot._create(self.auth, "sendMessage", {"is_mute": False, "message_contact": {"contactAbsObject": {"avatar_thumbnail": avatar, "first_name": firstName, "last_name": lastName or "", "is_deleted": False, "is_verified": False, "object_guid": user_guid, "type": "User"}, "first_name": firstName, "last_name": lastName or "", "phone_number": "+98"+phone[1:], "user_guid": user_guid, "vcard": f"BEGIN:VCARD\nVERSION:3.0\nFN:{firstName}\nTEL;MOBILE:+98{phone[1:]}\nEND:VCARD"}, "object_guid": chat_id, "rnd": randint(100000, 999999999)})
+
+    def setMembersAccess(self, chat_id, access_list):
+        return Bot._create(self.auth, "setGroupDefaultAccess", {"access_list": access_list, "group_guid": chat_id})
+
+    def setGroupTimer(self, chat_id, time):
+        return Bot._create(self.auth, "editGroupInfo", {"group_guid": chat_id, "slow_mode": time, "updated_parameters": ["slow_mode"]})
+
+    def setAdmin(self, chat_id, member_id, access_list=None):
+        return Bot._create(self.auth, f"set{Bot._chatDetection(chat_id)}Admin", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "access_list": access_list or [], "action": "SetAdmin", "member_guid": member_id})
 
-    votePoll     = lambda self, poll_id, option_index: Bot._create(4, self.auth, "votePoll", {"poll_id": poll_id,"selection_index": option_index})
+    def seenChats(self, seenList):
+        return Bot._create(self.auth, "seenChats", {"seen_list": dict(seenList)})
+
+    def sendChatAction(self, chat_id, action):
+        # every some seconds before sending message this request should send. action can be : Typing, Recording, Uploading
+        return Bot._create(self.auth, "sendChatActivity", {"activity": action, "object_guid": chat_id})
+
+    def sendPoll(self, chat_id, allows_multiple_answers, is_anonymous, options, question, Type="Regular", message_id=None):
+        return Bot._create(self.auth, "createPoll", {"allows_multiple_answers": bool(allows_multiple_answers), "is_anonymous": bool(is_anonymous), "object_guid": chat_id, "options": list(options), "question": question, "rnd": str(randint(100000, 999999999)), "type": Type, "reply_to_message_id": message_id})
+
+    def sendQuiz(self, chat_id, correct_option_index, is_anonymous, options, question, Type="Quiz", message_id=None):
+        return Bot._create(self.auth, "createPoll", {"correct_option_index": int(correct_option_index), "is_anonymous": bool(is_anonymous), "object_guid": chat_id, "options": list(options), "question": question, "rnd": str(randint(100000, 999999999)), "type": Type, "reply_to_message_id": message_id})
+
+    def searchGlobalObjects(self, text, start_id=None):
+        return Bot._create(self.auth, "searchGlobalObjects", {"search_text": text, "start_id": start_id})
+
+    def searchChatMessages(self, chat_id, search_text):
+        return Bot._create(self.auth, "searchChatMessages", {"object_guid": chat_id, "search_text": search_text})
+
+    def setPhoneVisibility(self, mode="Nobody"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"show_my_phone_number": mode}, "update_parameters": ["show_my_phone_number"]})  # mode = Nobody/Everybody/MyContacts
+
+    def setOnlineVisibility(self, mode="Everybody"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"show_my_last_online": mode}, "update_parameters": ["show_my_last_online"]})  # mode = Nobody/Everybody/MyContacts
+
+    def setAvatarVisibility(self, mode="Everybody"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"show_my_profile_photo": mode}, "update_parameters": ["show_my_profile_photo"]})  # mode = Everybody/MyContacts
+
+    def setCallableBy(self, mode="MyContacts"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"can_called_by": mode}, "update_parameters": ["can_called_by"]})  # mode = Everybody/MyContacts
+
+    def setForwardableBy(self, mode="Everybody"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"link_forward_message": mode}, "update_parameters": ["link_forward_message"]})  # mode = Nobody/Everybody/MyContacts
+
+    def setJoinableBy(self, mode="MyContacts"):
+        return Bot._create(self.auth, "setSetting", {"settings": {"can_join_chat_by": mode}, "update_parameters": ["can_join_chat_by"]})  # mode = Everybody/MyContacts
+
+    def setMyAutoDeleteTime(self, time=24):
+        return Bot._create(self.auth, "setSetting", {"settings": {"delete_account_not_active_months": str(time)}, "update_parameters": ["show_my_phone_number"]})  # time = 3/6/12/24 , type: str/int, duration: months
+
+    def setNotifications(self, user_message_preview=True, group_message_preview=False, channel_message_preview=False, in_app_sound=True, new_contacts=False, user_notification=True, group_notification=False, channel_notification=False, update_parameters=["user_message_preview", "in_app_sound", "user_notification"]):
+        return Bot._create(self.auth, "setSetting", {"settings": {"user_message_preview": user_message_preview, "user_notification": user_notification, "group_message_preview": group_message_preview, "group_notification": group_notification, "channel_message_preview": channel_message_preview, "channel_notification": channel_notification, "in_app_sound": in_app_sound, "new_contacts": new_contacts}, "update_parameters": update_parameters})
+
+    def setOwning(self, chat_id, newOwnerGuid):
+        return Bot._create(self.auth, "requestChangeObjectOwner", {"object_guid": chat_id, "new_owner_user_guid": newOwnerGuid})
+
+    def startVoiceChat(self, chat_id):
+        return Bot._create(self.auth, f"create{Bot._chatDetection(chat_id)}VoiceChat", {"object_guid": chat_id})
+
+
+    def terminateOtherSessions(self):
+        return Bot._create(self.auth, "terminateOtherSessions", {})
+
+
+    def unbanMember(self, chat_id, member_id):
+        return Bot._create(self.auth, f"ban{Bot._chatDetection(chat_id)}Member", {f"{Bot._chatDetection(chat_id).lower()}_guid": chat_id, "member_guid": member_id, "action": "Unset"})
+
+    def unpin(self, chat_id, message_id):
+        return Bot._create(self.auth, "setPinMessage", {"action": "Unpin", "message_id": message_id, "object_guid": chat_id})
+
+    def unblock(self, chat_id):
+        return Bot._create(self.auth, "setBlockUser", {"action": "Unblock", "user_guid": chat_id})
+
+    def unmuteChat(self, chat_id):
+        return Bot._create(self.auth, "setActionChat", {"action": "Unmute", "object_guid": chat_id})
+
+    def uploadAvatar(self, chat_id, main, thumbnail=""):
+        return Bot._create(self.auth, "uploadAvatar", {"object_guid": chat_id, "thumbnail_file_id": str(Bot.uploadFile(self, thumbnail or main)[0]["id"]), "main_file_id": str(Bot.uploadFile(self, main)[0]["id"])})
+
+    def uploadFile(self, file, frequest=None, logging=False):
+        return uploadFile(self, file, frequest, logging)
+
+
+    def votePoll(self, poll_id, option_index):
+        return Bot._create(self.auth, "votePoll", {"poll_id": poll_id, "selection_index": option_index})
 
 class Socket:
-    appliedFilters, chats, noChats, filtersType, func = *[[]]*3, "all", lambda msg: ...
+    appliedFilters, chats, noChats, filtersType, func = * \
+        [[]]*3, "all", lambda msg: ...
+
+    def __init__(self, auth, privateKey, proxy: str = None, logging: bool = False):
+        self.auth, self.privateKey, self.enc, self.proxy, self.logging = auth, privateKey, oldEncryption(auth), proxy, logging
 
-    def __init__(self, auth, proxy:str=None, logging:bool=False): self.auth, self.enc, self.proxy, self.logging = auth, encryption(auth), proxy, logging
+    def __enter__(self): return self
+    def __exit__(self, exc_type, exc_value, exc_tb): return self
 
     def on_open(self, ws):
-        Thread(target=ws.send(dumps({"api_version": "4","auth": self.auth,"data_enc": "","method": "handShake"})), args=()).start()
+        ws.send({"api_version": "5", "auth": self.auth, "data_enc": "", "method": "handShake"})
+
+    def on_error(self, ws, error):
+        print(error) if self.logging else None
+
+    def on_close(self, ws, code, msg):
+        print({"code": code, "message": msg}) if self.logging else None
+
+    def on_ping(self, ws, msg):
+        print("ping", ws.send(dumps({}))) if self.logging else ws.send(dumps({}))
 
-    on_error = lambda self, ws, error:     print(error) if self.logging else None
-    on_close = lambda self, ws, code, msg: print({"code": code, "message": msg}) if self.logging else None
-    on_ping  = lambda self, ws, msg :      print("ping") if self.logging else None
-    on_pong  = lambda self, ws, msg :      print("pong") if self.logging else None
+    def on_pong(self, ws, msg):
+        print("pong", msg) if self.logging else None
 
     def on_message(self, ws, message):
         try:
-            from Types import Message
-            bot, update, conditions = Bot("", self.auth), loads(self.enc.decrypt(loads(message)["data_enc"])), []
-            if self.logging: print(update)
-            parsedMessage = Message(self.auth, update["message_updates"][-1], chat_id=update["message_updates"][-1]["object_guid"], bot=bot)
-            [conditions.append(condition(bot, update)) for condition in Socket.appliedFilters]
+            from rubika.Types import Message
+            bot, update, conditions = Bot("", auth=self.auth, privateKey=self.privateKey), loads(self.enc.decrypt(loads(message)["data_enc"])) if loads(message).get("data_enc") != None else {}, []
+            if self.logging:
+                print(update)
+            parsedMessage = Message(
+                self.auth, update["message_updates"][-1], chat_id=update["message_updates"][-1]["object_guid"], bot=bot)
+            [conditions.append(condition(bot, update))
+             for condition in Socket.appliedFilters]
             if (Socket.chats == [] or (Socket.chats != [] and parsedMessage.chat_id in Socket.chats)) and (Socket.noChats == [] or (Socket.noChats != [] and not parsedMessage.chat_id in Socket.noChats)):
-                if   Socket.filtersType == "any" and any(conditions):        Thread(target=Socket.func, args=(parsedMessage,)).start()
-                elif Socket.filtersType == "invert" and not all(conditions): Thread(target=Socket.func, args=(parsedMessage,)).start()
-                elif all(conditions):                                        Thread(target=Socket.func, args=(parsedMessage,)).start()
-        except IndexError: pass
-        except Exception as e: print("\n✘ ERROR at line : ", exc_info()[2].tb_lineno, "\n    ",e) if self.logging else None
+                if Socket.filtersType == "any" and any(conditions):
+                    Thread(target=Socket.func, args=(parsedMessage,)).start()
+                elif Socket.filtersType == "invert" and not all(conditions):
+                    Thread(target=Socket.func, args=(parsedMessage,)).start()
+                elif all(conditions):
+                    Thread(target=Socket.func, args=(parsedMessage,)).start()
+        except IndexError:
+            pass
+        except Exception as e:
+            print("\n✘ ERROR at line : ", exc_info()[2].tb_lineno, "\n    ", e)
 
     def handler(self, *args, **kwargs):
         def wrapper(func):
             import websocket
 
-            Socket.func, Socket.appliedFilters, Socket.filtersType, Socket.chats, Socket.noChats = func, args, kwargs.get("Type") or types.ALL, kwargs.get("chats") or [], kwargs.get("blacklist") or []
-            try: Bot.wsURL = _getURL(key='default_sockets')
-            except exceptions.ConnectionError: ...
-            ws = websocket.WebSocketApp(Bot.wsURL, on_open = Socket(self.auth).on_open, on_message = Socket(self.auth).on_message, on_error = Socket(self.auth).on_error, on_close = Socket(self.auth).on_close, on_ping = Socket(self.auth).on_ping, on_pong = Socket(self.auth).on_pong)
+            Socket.func, Socket.appliedFilters, Socket.filtersType, Socket.chats, Socket.noChats = func, args, kwargs.get(
+                "Type") or types.ALL, kwargs.get("chats") or [], kwargs.get("blacklist") or []
+            try:
+                Bot.wsURL = _getURL(key='default_sockets')
+            except exceptions.ConnectionError:
+                ...
+            ws = websocket.WebSocketApp(Bot.wsURL, on_open=self.on_open, on_message=self.on_message, on_error=self.on_error, on_close=self.on_close, on_ping=self.on_ping, on_pong=self.on_pong)
             websocket.enableTrace(self.logging)
-            ws.run_forever(http_proxy_host = self.proxy[0] if self.proxy is not None else None, http_proxy_port = self.proxy[1] if self.proxy is not None else None, ping_interval=30, ping_timeout=10)
+            Thread(target=ws.run_forever, kwargs=dict(http_proxy_host=self.proxy[0] if self.proxy is not None else None,
+                   http_proxy_port=self.proxy[1] if self.proxy is not None else None, ping_interval=30, ping_timeout=5, host="web.rubika.ir")).start()
 
         return wrapper
```

### Comparing `rubika-6.0.7/rubika/configs.py` & `rubika-6.6.6/rubika/configs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,169 +1,186 @@
-from asyncio  import run
-from random   import sample, choice
-from json     import loads, dumps, decoder
+from re import findall
 from datetime import datetime
-from aiohttp  import ClientSession, client_exceptions
-from string   import ascii_lowercase, ascii_uppercase, digits
+from requests import get, post
+from random import sample, choice
+from json import loads, dumps, decoder
+from requests.exceptions import ConnectionError
+from aiohttp import ClientSession, client_exceptions
+from string import ascii_lowercase, ascii_uppercase, digits
 
 from rubika.encryption import encryption
 from rubika.exceptions import *
 
-__version__ , __license__ , __copyright__ = "6.0.7" , "GPLv3 license" , f"Copyright (C) {datetime.now().year} Bahman Ahmadi <github.com/Bahman-Ahmadi>"
+__version__, __license__, __copyright__ = "6.6.6", "GPLv3 license", f"Copyright (C) {datetime.now().year} Bahman Ahmadi <github.com/Bahman-Ahmadi>"
+
 
 class accesses:
     class admin:
-        pin               = "PinMessages"
-        newAdmin          = "SetAdmin"
-        editInfo          = "ChangeInfo"
-        banMember         = "BanMember"
-        changeLink        = "SetJoinLink"
+        pin = "PinMessages"
+        newAdmin = "SetAdmin"
+        editInfo = "ChangeInfo"
+        banMember = "BanMember"
+        changeLink = "SetJoinLink"
         editMembersAccess = "SetMemberAccess"
-        deleteMessages    = "DeleteGlobalAllMessages"
+        deleteMessages = "DeleteGlobalAllMessages"
 
     class user:
         viewMembers = "ViewMembers"
-        viewAdmins  = "ViewAdmins"
+        viewAdmins = "ViewAdmins"
         sendMessage = "SendMessages"
-        addMember   = "AddMember"
+        addMember = "AddMember"
+
 
 class clients:
     pwa = {
-        "app_name"    : "Main",
-        "app_version" : "1.2.1",
-        "platform"    : "PWA",
-        "package"     : "m.rubika.ir",
-        "lang_code"   : "fa"
+        "app_name": "Main",
+        "app_version": "1.2.1",
+        "platform": "PWA",
+        "package": "m.rubika.ir",
+        "lang_code": "fa"
     }
     web = {
-        "app_name"    : "Main",
-        "app_version" : "4.0.7",
-        "platform"    : "Web",
-        "package"     : "web.ir",
-        "lang_code"   : "fa"
-    }
+		"app_name": "Main",
+		"app_version": "4.3.3",
+		"platform": "Web",
+		"package": "web.rubika.ir",
+		"lang_code": "fa"
+	}
     android = {
-        "app_name"    : "Main",
-        "app_version" : "2.9.8",
-        "platform"    : "Android",
-        "package"     : "app.rbmain.a",
-        "lang_code"   : "fa"
+        "app_name": "Main",
+        "app_version": "2.9.8",
+        "platform": "Android",
+        "package": "app.rbmain.a",
+        "lang_code": "fa"
     }
 
+
 class reports:
-    OTHER       = 100
-    VIOLENCE    = 101
-    SPAM        = 102
+    OTHER = 100
+    VIOLENCE = 101
+    SPAM = 102
     PORNOGRAPHY = 103
     CHILD_ABUSE = 104
-    COPYRIGHT   = 105
-    FISHING     = 106
+    COPYRIGHT = 105
+    FISHING = 106
+
 
 class visibility:
-    EVERYBODY  = "Everybody"
+    EVERYBODY = "Everybody"
     MYCONTACTS = "MyContacts"
-    NOBODY     = "Nobody"
+    NOBODY = "Nobody"
 
-randStr = lambda length, choices=[*ascii_lowercase, *ascii_uppercase, *digits, *"-_"]: "".join([choice(choices) for i in range(length)])
+
+randStr = lambda length, choices=[*ascii_lowercase, *ascii_uppercase,
+                                  *digits, *"-_"]: "".join([choice(choices) for i in range(length)])
+
+defaultUserAgent = "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0"
 
 defaultDevice = {
-    "app_version"      : "MA_2.9.8",
-    "device_hash"      : randStr(32, [*ascii_uppercase, *digits]),
-    "device_model"     : "rubikalib",
-    "is_multi_account" : False,
-    "lang_code"        : "fa",
-    "system_version"   : "SDK 22",
-    "token"            : f"{randStr(22, [*ascii_lowercase, *ascii_uppercase, *digits])}:{randStr(140)}",
-    "token_type"       : "Firebase"
+	"token_type": "Web",
+	"token": "",
+	"app_version": "WB_4.3.3",
+	"lang_code": "fa",
+	"system_version": "Windows 10",
+	"device_model": "Firefox 113",
+	"device_hash" : "2"+''.join(findall(r'\d+', defaultUserAgent))
 }
 
-def post(json:dict, method, url:str=None, platform="rubika", enc:encryption=None, isEncrypted:bool=True) -> dict:
-    async def POST(url, data):
-        while 1:
-            try:
-                async with ClientSession() as session:
-                    async with session.post(url, json=data) as response:
-                        response = await response.text()
-                        response = loads(str(enc.decrypt(loads(response).get("data_enc")))) if "data_enc" in loads(response).keys() and isEncrypted else loads(response)
-                        if "status" in response.keys() and response.get("status") != "OK":
-                            if response.get("status_det") == "NOT_REGISTERED":
-                                raise NotRegistered("the auth is incorrect. please sure about your account's health then login again.")
-                            elif response.get("status_det") == "INVALID_INPUT" :
-                                print(url)
-                                raise InvalidInput(f"the inserted argument(s) is invaild in the {platform}/{method}. if you're sure about your argument(s), please report this message.")
-                            elif response.get("status_det") == "TOO_REQUESTS" :
-                                raise TooRequests(f"the {platform}/{method} method has been limited. please try again later.")
-                            elif response.get("status_det") == 'INVALID_AUTH':
-                                raise InvaildAuth(f"the inserted argument(s) in {platform}/{method} is vaild but is not related to other argument(s) or maybe for other reasons, anyway now this method can't run on server. please don't enter fake argument(s) and fix anything can return this exception")
-                        else:
-                            return response
-            except decoder.JSONDecodeError: ...
-            except client_exceptions.ClientConnectorError: url = _getURL(dc_id=64)
-    return run(POST(url or _getURL(), json))
+def POST(json: dict, method, url: str = None, platform="web.rubika.ir", enc: encryption = None, isEncrypted: bool = True) -> dict:
+    while 1:
+        try:
+            response = post(url=url, json=json, headers={
+                    'Origin': 'https://'+platform,
+					'Referer': f'https://{platform}/',
+					'Host': url.replace("https://","").replace("/",""),
+					'User-Agent': defaultUserAgent
+            }).text
+            response = loads(str(enc.decrypt(loads(response).get("data_enc")))) if "data_enc" in loads(response).keys() and isEncrypted else loads(response)
+            if "status" in response.keys() and response.get("status") != "OK":
+                print(json, method, url, platform, response)
+                if response.get("status_det") == "NOT_REGISTERED":
+                    raise NotRegistered("the auth is incorrect. please sure about your account's health then login again.")
+                elif response.get("status_det") == "INVALID_INPUT":
+                    raise InvalidInput(f"the inserted argument(s) is invaild in the {platform}/{method}. if you're sure about your argument(s), please report this message.")
+                elif response.get("status_det") == "TOO_REQUESTS":
+                    raise TooRequests(f"the {platform}/{method} method has been limited. please try again later.")
+                elif response.get("status_det") == 'INVALID_AUTH':
+                    raise InvalidAuth(f"the inserted argument(s) in {platform}/{method} is vaild but is not related to other argument(s) or maybe for other reasons, anyway now this method can't run on server. please don't enter fake argument(s) and fix anything can return this exception")
+            else:
+                return response
+        except decoder.JSONDecodeError:
+                ...
+        except ConnectionError:
+                url = _getURL(dc_id=64)
 
 retries = 0
-def _getURL(key="default_api_urls", DCsURL:str="https://messengerg2cX.iranlms.ir/", getDCsURL:str="https://getdcmess.iranlms.ir", dc_id:int=None):
-    import requests
+def _getURL(key="default_api_urls", DCsURL: str = "https://messengerg2cX.iranlms.ir/", getDCsURL: str = "https://getdcmess.iranlms.ir", dc_id: int = None):
+    global retries
     while 1:
         try:
-            res = requests.post(json={"api_version": 4, "client": clients.pwa, "method": "getDCs"}, url=getDCsURL).json().get("data").get(key)
+            res = post(json={"api_version": 4, "client": clients.pwa, "method": "getDCs"}, url=getDCsURL).json().get("data").get(key)
             return DCsURL.replace('X', dc_id) if dc_id is not None else choice(list(res))
         except requests.exceptions.ConnectionError:
             retries += 1
             if retries == 3:
                 retries = 0
                 break
 
-def makeData(api_version:int, auth:str, method:str, data:dict, client:dict, url:str=None) -> dict :
-    url, enc = url or _getURL(), encryption(auth)
-    outerJson = {
-        "api_version" : str(api_version),
-        "auth"        : auth,
-        "data_enc"    : enc.encrypt(dumps({
-            "method"  : method,
-            "input"   : data,
-            "client"  : client
-        }))
-    }
 
-    if int(api_version) == 4:
-        outerJson["data_enc"] = enc.encrypt(dumps(data))
-        outerJson["client"]   = client
-        outerJson["method"]   = method
+def makeData(auth:str, enc:encryption, method:str, data:dict, client:dict=clients.web, url:str = None) -> dict:
+    url = url or _getURL()
+    outerJson = {
+        "api_version": "6",
+        "auth": auth,
+        "data_enc": {
+            "method": method,
+            "input": data,
+            "client": client
+        }
+    }
+    print(outerJson)
+    outerJson["data_enc"] = enc.encrypt(dumps(outerJson["data_enc"]))
+    outerJson["sign"] = enc.makeSignFromData(outerJson["data_enc"])
+    return POST(outerJson, url=url, platform=client.get('package'), method=method, enc=enc)
 
-    return post(outerJson, url=url, platform=client.get('package'), method=method, enc=enc)
 
-def makeTmpData(method:str, data:dict, url:str=None) -> dict:
-    url, tmp = url or _getURL(), tmpGeneration()
+def makeTmpData(method: str, data: dict, url: str = None, tmp:str=None) -> dict:
+    url, tmp = url or _getURL(), encryption.changeAuthType(tmp or tmpGeneration())
     enc = encryption(tmp)
     outerJson = {
-        "api_version": "5",
+        "api_version": "6",
         "tmp_session": tmp,
-        "data_enc"   : enc.encrypt(dumps({
-            "method" : method,
-            "input"  : data,
-            "client" : clients.web
+        "data_enc": enc.encrypt(dumps({
+            "method": method,
+            "input": data,
+            "client": clients.web
         }))
     }
-    
-    return post(outerJson, method, url=url, platform=clients.web.get("package"), enc=enc)
 
-def makeRubinoData(auth:str, method:str, data:dict) -> dict:
+    resp = POST(outerJson, method, url=url, platform=clients.web.get("package"), enc=enc)
+    resp['tmp'] = tmp
+    return resp
+
+
+def makeRubinoData(auth: str, method: str, data: dict) -> dict:
     outerJson = {
         "api_version": "0",
-        "auth"   : auth,
-        "client" : clients.android,
-        "data"   : data,
-        "method" : method
+        "auth": auth,
+        "client": clients.android,
+        "data": data,
+        "method": method
     }
-    return post(outerJson, method, url="https://rubino12.iranlms.ir/", platform="rubino", isEncrypted=False)
+    return POST(outerJson, method, url="https://rubino12.iranlms.ir/", platform=clients.web.get('package'), isEncrypted=False)
+
+
+def tmpGeneration():
+    return randStr(32, [*ascii_lowercase, *digits])
 
-tmpGeneration = lambda: randStr(32, [*ascii_lowercase, *digits])
 
-def welcome(text, time:float=0.035):
+def welcome(text, time: float = 0.035):
     from time import sleep
     try:
         from rich import print as Print
         Print(text)
     except ModuleNotFoundError:
         for char in text:
             print(char, end='', flush=True)
```

### Comparing `rubika-6.0.7/rubika/rubino.py` & `rubika-6.6.6/rubika/rubino.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,90 @@
 from pathlib import Path
-from random  import randint
+from random import randint
 
 from rubika.fileIO import uploadFile
 from rubika.configs import makeRubinoData, welcome, __version__, __license__, __copyright__
 
+
 class Rubino:
-    def __init__(self, auth:str):
+    def __init__(self, auth: str):
         self.auth = auth
-        self.profileID = [i['id'] for i in self.getProfileList().get("data").get("profiles") if i['is_default']][0]
-        welcome(f"rubika library version {__version__}\n{__copyright__}\n→ docs : https://rubikalib.github.io\n\nswitching rubino...")
+        #self.profileID = [i['id'] for i in self.getProfileList().get(
+        #    "data").get("profiles") if i['is_default']][0]
+        welcome(
+            f"rubika library version {__version__}\n{__copyright__}\n→ docs : https://rubikalib.github.io\n\nswitching rubino...")
 
-    def addPost(self, file:str, caption:str=None, isMultiFile:bool=None, postType:str="Picture"):
-        uresponse:list = self.fileUpload(file, Type=postType)
+    def addPost(self, file: str, caption: str = None, isMultiFile: bool = None, postType: str = "Picture"):
+        uresponse: list = self.fileUpload(file, Type=postType)
         return makeRubinoData(self.auth, "addPost", {"caption": caption, "file_id": uresponse[0]['file_id'], "hash_file_receive": uresponse[1], "height": "800", "width": "800", "is_multi_file": isMultiFile, "post_type": postType, "rnd": randint(100000, 999999999), "thumbnail_file_id": uresponse[0]['file_id'], "thumbnail_hash_file_receive": uresponse[1], "profile_id": self.profileID})
 
-    def addStory(self, duration, width, height, storyType="Picture"):
-        uresponse:list = self.fileUpload(file, Type=storyType)
+    def addStory(self, file: str, duration, width, height, storyType="Picture"):
+        uresponse: list = self.fileUpload(file, Type=storyType)
         return makeRubinoData(self.auth, "addStory", {"duration": duration, "file_id": uresponse[0]['file_id'], "hash_file_receive": uresponse[1], "height": height, "profile_id": self.profileID, "rnd": randint(100000, 999999999), "story_type": storyType, "thumbnail_file_id": uresponse[0]['file_id'], "thumbnail_hash_file_receive": uresponse[1], "width": width})
 
-    bookmark          = lambda self, postID, postProfileID       : makeRubinoData(self.auth, "postBookmarkAction", {"action_type": "Bookmark","post_id": postID,"post_profile_id": postProfileID,"profile_id": self.profileID})
+    def bookmark(self, postID, postProfileID): return makeRubinoData(self.auth, "postBookmarkAction", {
+        "action_type": "Bookmark", "post_id": postID, "post_profile_id": postProfileID, "profile_id": self.profileID})
+
+    def createPage(self, name, username, bio=None): return makeRubinoData(
+        self.auth, "createPage", {"bio": bio, "name": name, "username": username})
+
+    def comment(self, text, postID, postProfileID): return makeRubinoData(self.auth, "addComment", {
+        "content": text, "post_id": postID, "post_profile_id": postProfileID, "rnd": str(randint(100000, 999999999)), "profile_id": self.profileID})
+
+    fileUpload = lambda self, file, Type="Picture": uploadFile(
+        self, file, rubino=True, rubinoFType=Type, rubinoFRequest=self.requestUploadFile)
+
+    def follow(self, followee_id): return makeRubinoData(self.auth, "requestFollow", {
+        "f_type": "Follow", "followee_id": followee_id, "profile_id": self.profileID})
+
+    getComments = lambda self, postID, postProfileID, limit=50, sort="FromMax": makeRubinoData(self.auth, "getComments", {
+                                                                                               "equal": False, "limit": limit, "sort": sort, "post_id": postID, "profile_id": self.profileID, "post_profile_id": postProfileID})
+
+    def getMyProfileInfo(self): return makeRubinoData(
+        self.auth, "getMyProfileInfo", {"profile_id": self.profileID})
+
+    def getPostByShareLink(self, shareString): return makeRubinoData(self.auth, "getPostByShareLink", {
+        "share_string": shareString.replace('https://rubika.ir/post/', ''), "profile_id": self.profileID})
+    getProfileList = lambda self, equal=False, limit=10, sort="FromMax": makeRubinoData(
+        self.auth, "getProfileList", {"equal": equal, "limit": limit, "sort": sort})
+    getProfilePosts = lambda self, targetProfileID, limit=51, sort="FromMax": makeRubinoData(self.auth, "getProfilePosts", {
+                                                                                             "equal": False, "limit": limit, "sort": sort, "target_profile_id": targetProfileID, "profile_id": self.profileID})
+    getRecentPosts = lambda self, equal=False, limit=30, sort="FromMax": makeRubinoData(
+        self.auth, "getRecentFollowingPosts", {"equal": equal, "limit": limit, "sort": sort, "profile_id": self.profileID})
+
+    def getShareLink(self, postID, postProfileID): return makeRubinoData(self.auth, "getShareLink", {
+        "post_id": postID, "post_profile_id": postProfileID, "profile_id": self.profileID})
+
+    def getStories(self, targetProfileID, limit=100): return makeRubinoData(
+        self.auth, "getProfileStories", {"limit": limit, "profile_id": targetProfileID})
+
+    def getStoryIds(self, targetProfileID): return makeRubinoData(self.auth, "getStoryIds", {
+        "profile_id": self.profileID, "target_profile_id": targetProfileID})
+
+    def isExist(self, username): return makeRubinoData(
+        self.auth, "isExistUsername", {"username": username.replace('@', '')})
+
+    def like(self, post_id, post_profile_id): return makeRubinoData(self.auth, "likePostAction", {
+        "action_type": "Like", "post_id": post_id, "post_profile_id": post_profile_id, "profile_id": self.profileID})
+
+    def reloadProfile(self): return makeRubinoData(self.auth, "updateProfile", {
+        "profile_id": self.profileID, "profile_status": "Public"})
+    requestUploadFile = lambda self, file, size=None, Type="Picture": makeRubinoData(self.auth, "requestUploadFile", {"file_name": file.split(
+        "/")[-1], "file_size": size or Path(file).stat().st_size, "file_type": Type, "profile_id": self.profileID})
+
+    def unbookmark(self, postID, postProfileID): return makeRubinoData(self.auth, "postBookmarkAction", {
+        "action_type": "Unbookmark", "post_id": postID, "post_profile_id": postProfileID, "profile_id": self.profileID})
+
+    def unfollow(self, followee_id): return makeRubinoData(self.auth, "requestFollow", {
+        "f_type": "Unfollow", "followee_id": followee_id, "profile_id": self.profileID})
+
+    def unlike(self, post_id, post_profile_id): return makeRubinoData(self.auth, "likePostAction", {
+        "action_type": "Unlike", "post_id": post_id, "post_profile_id": post_profile_id, "profile_id": self.profileID})
+
+    def updateProfile(self, name=None, bio=None, email=None): return makeRubinoData(
+        self.auth, "updateProfile", {"name": name, "bio": bio, "email": email})
 
-    createPage        = lambda self, name, username, bio=None    : makeRubinoData(self.auth, "createPage", {"bio": bio,"name": name,"username": username})
-    comment           = lambda self, text, postID, postProfileID : makeRubinoData(self.auth, "addComment", {"content": text,"post_id": postID, "post_profile_id": postProfileID, "rnd": str(randint(100000,999999999)) ,"profile_id": self.profileID})
+    def viewPost(self, post_id, post_profile_id): return makeRubinoData(
+        self.auth, "addPostViewCount", {"post_id": post_id, "post_profile_id": post_profile_id})
 
-    fileUpload        = lambda self, file, Type="Picture": uploadFile(self, file, rubino=True, rubinoFType=Type, rubinoFRequest=self.requestUploadFile)
-    follow            = lambda self, followee_id: makeRubinoData(self.auth, "requestFollow", {"f_type": "Follow", "followee_id": followee_id, "profile_id": self.profileID})
-    
-    getComments        = lambda self, postID, postProfileID, limit=50, sort="FromMax" : makeRubinoData(self.auth, "getComments", {"equal": False, "limit": limit, "sort": sort, "post_id": postID, "profile_id": self.profileID, "post_profile_id": postProfileID})
-    getMyProfileInfo   = lambda self                                                  : makeRubinoData(self.auth, "getMyProfileInfo", {"profile_id": self.profileID})
-    getPostByShareLink = lambda self, shareString                                     : makeRubinoData(self.auth, "getPostByShareLink", {"share_string": shareString.replace('https://rubika.ir/post/', ''), "profile_id": self.profileID})
-    getProfileList     = lambda self, equal=False, limit=10, sort="FromMax"           : makeRubinoData(self.auth, "getProfileList", {"equal": equal,"limit": limit,"sort": sort})
-    getProfilePosts    = lambda self, targetProfileID, limit=51, sort="FromMax"       : makeRubinoData(self.auth, "getProfilePosts", {"equal": False, "limit": limit, "sort": sort, "target_profile_id": targetProfileID, "profile_id": self.profileID})
-    getRecentPosts     = lambda self, equal=False, limit=30, sort="FromMax"           : makeRubinoData(self.auth, "getRecentFollowingPosts", {"equal": equal, "limit": limit, "sort": sort, "profile_id": self.profileID})
-    getShareLink       = lambda self, postID, postProfileID                           : makeRubinoData(self.auth, "getShareLink", {"post_id": postID, "post_profile_id": postProfileID, "profile_id": self.profileID})
-    getStories         = lambda self, targetProfileID, limit=100                      : makeRubinoData(self.auth, "getProfileStories", {"limit": limit, "profile_id": targetProfileID})
-    getStoryIds        = lambda self, targetProfileID                                 : makeRubinoData(self.auth, "getStoryIds", {"profile_id": self.profileID, "target_profile_id": targetProfileID})
-
-    isExist           = lambda self, username: makeRubinoData(self.auth, "isExistUsername", {"username": username.replace('@','')})
-
-    like              = lambda self, post_id, post_profile_id: makeRubinoData(self.auth, "likePostAction", {"action_type": "Like", "post_id": post_id, "post_profile_id": post_profile_id, "profile_id": self.profileID})
-
-    reloadProfile     = lambda self                                  : makeRubinoData(self.auth, "updateProfile", {"profile_id": self.profileID, "profile_status": "Public"})
-    requestUploadFile = lambda self, file, size=None, Type="Picture" : makeRubinoData(self.auth, "requestUploadFile", {"file_name": file.split("/")[-1], "file_size": size or Path(file).stat().st_size, "file_type": Type, "profile_id": self.profileID})
-
-    unbookmark        = lambda self, postID, postProfileID : makeRubinoData(self.auth, "postBookmarkAction", {"action_type": "Unbookmark","post_id": postID,"post_profile_id": postProfileID,"profile_id": self.profileID})
-    unfollow          = lambda self, followee_id: makeRubinoData(self.auth, "requestFollow", {"f_type": "Unfollow", "followee_id": followee_id, "profile_id": self.profileID})
-    unlike            = lambda self, post_id, post_profile_id: makeRubinoData(self.auth, "likePostAction", {"action_type": "Unlike", "post_id": post_id, "post_profile_id": post_profile_id, "profile_id": self.profileID})
-    updateProfile     = lambda self, name=None, bio=None, email=None: makeRubinoData(self.auth, "updateProfile", {"name": name, "bio": bio, "email": email})
-    
-    viewPost          = lambda self, post_id, post_profile_id   : makeRubinoData(self.auth, "addPostViewCount", {"post_id": post_id, "post_profile_id": post_profile_id})
-    viewStories         = lambda self, storyIds, storyProfileID : makeRubinoData(self.auth, "addViewStory", {"profile_id": self.profileID, "story_ids": storyIds, "story_profile_id": storyProfileID})
+    def viewStories(self, storyIds, storyProfileID): return makeRubinoData(self.auth, "addViewStory", {
+        "profile_id": self.profileID, "story_ids": storyIds, "story_profile_id": storyProfileID})
```

### Comparing `rubika-6.0.7/rubika/tools.py` & `rubika-6.6.6/rubika/tools.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,193 @@
+import re
 from re import findall
 from rich import print
 from threading import Thread
 from datetime import datetime
 
 bot = None
 socket = None
 lockTime = None
 unlockTime = None
 
+
 class Tools:
     def __init__(self, auth):
         from rubika.client import Bot, Socket
         bot = Bot("", auth=auth)
         socket = Socket(auth)
 
     def hasInsult(self, msg):
         return any(word in open("dontReadMe.txt").read().split("\n") for word in msg.split())
-    
+
     def hasAD(self, msg):
         result = False
-        links = list(map(lambda ID: ID.strip()[1:],findall(r"@[\w|_|\d]+", msg))) + list(map(lambda link:link.split("/")[-1],findall(r"rubika\.ir/\w+",msg)))
+        links = list(map(lambda ID: ID.strip()[1:], findall(r"@[\w|_|\d]+", msg))) + list(
+            map(lambda link: link.split("/")[-1], findall(r"rubika\.ir/\w+", msg)))
         joincORjoing = "joing" in msg or "joinc" in msg
-    
-        if joincORjoing: result = True
+
+        if joincORjoing:
+            result = True
         else:
             for link in links:
                 try:
-                    Type = bot.getInfoByUsername(link)["data"]["chat"]["abs_object"]["type"]
-                    if Type == "Channel": result = True
-                except KeyError: result = False
+                    Type = bot.getInfoByUsername(
+                        link)["data"]["chat"]["abs_object"]["type"]
+                    if Type == "Channel":
+                        result = True
+                except KeyError:
+                    result = False
 
         return result
 
     def hasSpam(self, messages):
-        result, beforeIter = {"isExist":False, "spams":[]}, 0
-        for Iter in range(0,len(messages)):
+        result, beforeIter = {"isExist": False, "spams": []}, 0
+        for Iter in range(0, len(messages)):
             if messages[beforeIter] == messages[Iter] and Iter != beforeIter:
                 result["isExist"] = True
                 result["spams"].append([beforeIter, Iter])
             beforeIter = Iter
         return result
 
     class lockSchedule:
         def __init__(self): pass
 
         def setLockTime(self, h, m):
             global lockTime
             lockTime = f"{h}:{m}"
-    
+
         def setUnlockTime(self, h, m):
             global unlockTime
             unlockTime = f"{h}:{m}"
 
         def getLockTime(self):
             global lockTime
             return lockTime
 
         def getUnlockTime(self):
             global unlockTime
             return unlockTime
-    
+
         def checkLockTime(self, guid, accesses=[]):
             global lockTime
             if datetime.now().strftime("%H:%M") == lockTime:
                 bot.setMembersAccess(guid, accesses)
-    
-        def checkUnlockTime(self, guid, accesses=["ViewMembers","ViewAdmins","SendMessages","AddMember"]):
+
+        def checkUnlockTime(self, guid, accesses=["ViewMembers", "ViewAdmins", "SendMessages", "AddMember"]):
             global lockTime
             if datetime.now().strftime("%H:%M") == lockTime:
                 bot.setMembersAccess(guid, accesses)
 
-    def commandHandler(self, message, command, method:callable):
-        if message == command: method()
-
-    def isJoin(self, user_guid:str, channel_guid:str) -> bool:
-        userInfo       = bot.getInfo(user_guid)
-        haveUserName   = 'username' in userInfo.keys()
-        channelMembers = lambda keyword : bot.getMembers(channel_guid, search_text=keyword) if keyword != None else []
-
-        if haveUserName: result = [True for i in channelMembers(userInfo.get('username'))     if i['member_guid'] == user_guid][0]
+    def commandHandler(self, message, command, method: callable):
+        if message == command:
+            method()
+
+    def isJoin(self, user_guid: str, channel_guid: str) -> bool:
+        userInfo = bot.getInfo(user_guid)
+        haveUserName = 'username' in userInfo.keys()
+        def channelMembers(keyword): return bot.getMembers(
+            channel_guid, search_text=keyword) if keyword != None else []
+
+        if haveUserName:
+            result = [True for i in channelMembers(userInfo.get(
+                'username')) if i['member_guid'] == user_guid][0]
         else:
-            result = [True for i in channelMembers(userInfo.get('first_name'))   if i['member_guid'] == user_guid][0]
-            result = [True for i in channelMembers(userInfo.get('last_name'))    if i['member_guid'] == user_guid][0]
+            result = [True for i in channelMembers(userInfo.get(
+                'first_name')) if i['member_guid'] == user_guid][0]
+            result = [True for i in channelMembers(userInfo.get(
+                'last_name')) if i['member_guid'] == user_guid][0]
 
         return result == True
 
-    def faster(self, controller):
-        def get(): socket.handle()
-        def use(): controller(socket.data)
-        
-        while True:
-            Thread(target=get).start()
-            Thread(target=use).start()
-
-    loadTime = lambda timestamp, func=__import__("datetime").datetime.fromtimestamp: func(int(timestamp)) # func can be __import__("jdatetime").datetime.fromtimestamp THEN you must install jdatetime using `pip install jdatetime`
+    # func can be __import__("jdatetime").datetime.fromtimestamp THEN you must install jdatetime using `pip install jdatetime`
+    loadTime = lambda timestamp, func=__import__(
+        "datetime").datetime.fromtimestamp: func(int(timestamp))
 
     @staticmethod
-    def chatDetection(chat_id:str) -> str:
+    def chatDetection(chat_id: str) -> str:
         return "Group" if chat_id.startswith("g") else "Channel" if chat_id.startswith("c") else "User" if chat_id.startswith("u") else "Bot" if chat_id.startswith("b") else "Service"
 
     @staticmethod
     def parse(mode, text):
-        results = []
-        
-        replaces = ["**", "__", "`", "[", "]", "(", ")", "~~", "--"] if mode.lower() == "markdown" else ["<b>", "<i>", "<pre>", "<s>", "<u>", "<link href='", "<a href='", "'>", "</a>", "</link>", "</u>", "</s>", "</pre>", "</i>", "</b>"] # the symbols
-        realText = text
-        for i in replaces:
-            if i in text: realText = realText.replace(i, '')
-        bolds    = findall(r"\*\*(.*?)\*\*",text) if mode.lower() == "markdown" else findall("<b>(.*?)</b>",text)
-        italics  = findall(r"\_\_(.*?)\_\_",text) if mode.lower() == "markdown" else findall("<i>(.*?)</i>",text)
-        monos    = findall(r"\`(.*?)\`",text) if mode.lower() == "markdown" else findall("<pre>(.*?)</pre>",text)
-        strikes  = findall(r"\~\~(.*?)\~\~",text) if mode.lower() == "markdown" else findall("<s>(.*?)</s>",text)
-        unders   = findall(r"\-\-(.*?)\-\-",text) if mode.lower() == "markdown" else findall("<u>(.*?)</u>",text)
-        Mentions = findall(r"\[(.*?)\]\((.*?)\)", text) if mode.lower() == "markdown" else findall("<a href='(.*?)'>(.*?)</a>", text)
-
-        bResult = [realText.index(i) for i in bolds]
-        iResult = [realText.index(i) for i in italics]
-        mResult = [realText.index(i) for i in monos]
-        sResult = [realText.index(i) for i in strikes]
-        uResult = [realText.index(i) for i in unders]
-
-        for m in Mentions: realText = realText.replace(m[0], "") # removing guids & links from orginal text
-        MResult = [realText.index(i[1]) for i in Mentions]
-        
-        for indexes,words,Types in ((bResult, bolds, ["Bold"]*len(bolds)), (iResult, italics, ["Italic"]*len(italics)), (mResult, monos, ["Mono"]*len(monos)), (sResult, strikes, ["Strike"]), (uResult, unders, ["Underline"]), (MResult, Mentions, ["MentionText"]*len(Mentions))):
-            if indexes != [] and words != []:
-                for index, word, Type in zip(indexes, words, Types):
-                    result = {"from_index": index,"length": len(word if Type != "MentionText" else word[1]),"type": Type}
-                    if Type == "MentionText":
-                        if word[0].startswith('http'): result["type"], result["link"] = "Link", {"hyperlink_data": {"url": word[0]}, "type": "hyperlink"}
-                        else: result["mention_text_object_guid"], result["mention_text_object_type"] = word[0], Tools.chatDetection(word[0])
-                    results.append(result)
+        pattern = r'`(.*)`|\*\*(.*)\*\*|__(.*)__|\[(.*)\]\((\S+)\)'
+        conflict = 0
+        meta_data_parts = []
+        for markdown in re.finditer(pattern, value):
+            span = markdown.span()
+            if markdown.group(0).startswith('`'):
+                value = re.sub(pattern, r'\1', value, count=1)
+                meta_data_parts.append(
+                    {
+                        'type': 'Mono',
+                        'from_index': span[0] - conflict,
+                        'length': span[1] - span[0] - 2
+                    }
+                )
+                conflict += 2
+
+            elif markdown.group(0).startswith('**'):
+                value = re.sub(pattern, r'\2', value, count=1)
+                meta_data_parts.append(
+                    {
+                        'type': 'Bold',
+                        'from_index': span[0] - conflict,
+                        'length': span[1] - span[0] - 4
+                    }
+                )
+                conflict += 4
+
+            elif markdown.group(0).startswith('__'):
+                value = re.sub(pattern, r'\3', value, count=1)
+                meta_data_parts.append(
+                    {
+                        'type': 'Italic',
+                        'from_index': span[0] - conflict,
+                        'length': span[1] - span[0] - 4
+                    }
+                )
+                conflict += 4
+
+            else:
+                value = re.sub(pattern, r'\4', value, count=1)
+
+                mention_text_object_type = 'User'
+                mention_text_object_guid = markdown.group(5)
+                if mention_text_object_guid.startswith('g'):
+                    mention_text_object_type = 'Group'
+
+                elif mention_text_object_guid.startswith('c'):
+                    mention_text_object_type = 'Channel'
+
+                meta_data_parts.append(
+                    {
+                        'type': 'MentionText',
+                        'from_index': span[0] - conflict,
+                        'length': len(markdown.group(4)),
+                        'mention_text_object_guid': mention_text_object_guid,
+                        'mention_text_object_type': mention_text_object_type
+                    }
+                )
+                conflict += 4 + len(mention_text_object_guid)
 
-        return dict(metadata=results, realText=realText)
+        return dict(realText=value, metadata=dict(meta_data_parts=meta_data_parts))
 
     @staticmethod
-    def getThumbInline(image_bytes:bytes) -> str:
-        import io, base64, PIL.Image
+    def getThumbInline(image_bytes: bytes) -> str:
+        import io
+        import base64
+        import PIL.Image
         im, output = PIL.Image.open(io.BytesIO(image_bytes)), io.BytesIO()
         width, height = im.size
         im.save(output, format='PNG')
         im_data = output.getvalue()
         image_data = base64.b64encode(im_data)
-        if not isinstance(image_data, str): image_data = image_data.decode()
+        if not isinstance(image_data, str):
+            image_data = image_data.decode()
         return image_data
 
     @staticmethod
-    def getImageSize(image_bytes:bytes) -> list:
-        import io, PIL.Image
+    def getImageSize(image_bytes: bytes) -> list:
+        import io
+        import PIL.Image
         im = PIL.Image.open(io.BytesIO(image_bytes))
         width, height = im.size
-        return [width , height]
+        return [width, height]
```

### Comparing `rubika-6.0.7/rubika.egg-info/PKG-INFO` & `rubika-6.6.6/rubika.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.0.7
+Version: 6.6.6
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
@@ -35,15 +35,14 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: ~=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-
 <p align="center">
     <a href="https://github.com/bahman-ahmadi/rubika">
         <img src="https://rubikalib.github.io/assets/logo.png" alt="RUBIKA" width="128">
     </a>
     <br>
     <b>Rubika Bot Self Library for Python</b>
     <br>
@@ -113,8 +112,8 @@
 - Join the official channel at https://t.me/rubikalib and stay tuned for news, updates and announcements.
 
 ### License
 rubika library is licensed under [GPLv3 license](https://github.com/bahman-ahmadi/rubika/blob/main/LICENSE)
 
 This is not an official rubika product. It is not affiliated with nor endorsed by rubika Inc.
 
-© 2023 Bahman Ahmadi
+© 2022 Bahman Ahmadi
```

### Comparing `rubika-6.0.7/setup.py` & `rubika-6.6.6/rubika/setup.py`

 * *Files identical despite different names*

