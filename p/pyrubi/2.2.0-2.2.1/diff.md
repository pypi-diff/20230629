# Comparing `tmp/pyrubi-2.2.0.tar.gz` & `tmp/pyrubi-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrubi-2.2.0.tar", last modified: Tue Jun 27 14:34:12 2023, max compression
+gzip compressed data, was "pyrubi-2.2.1.tar", last modified: Thu Jun 29 17:54:50 2023, max compression
```

## Comparing `pyrubi-2.2.0.tar` & `pyrubi-2.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.288563 pyrubi-2.2.0/
--rw-rw-rw-   0        0        0     2156 2023-06-27 14:34:12.288563 pyrubi-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1316 2023-06-27 14:31:50.000000 pyrubi-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.232560 pyrubi-2.2.0/pyrubi/
--rw-rw-rw-   0        0        0      246 2023-06-27 14:18:29.000000 pyrubi-2.2.0/pyrubi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.250135 pyrubi-2.2.0/pyrubi/cryption/
--rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.2.0/pyrubi/cryption/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.251134 pyrubi-2.2.0/pyrubi/handler/
--rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.2.0/pyrubi/handler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.259333 pyrubi-2.2.0/pyrubi/maker/
--rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.2.0/pyrubi/maker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.261333 pyrubi-2.2.0/pyrubi/message/
--rw-rw-rw-   0        0        0     4009 2023-06-27 13:19:11.000000 pyrubi-2.2.0/pyrubi/message/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.271329 pyrubi-2.2.0/pyrubi/methods/
--rw-rw-rw-   0        0        0    45760 2023-06-27 13:43:21.000000 pyrubi-2.2.0/pyrubi/methods/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.284752 pyrubi-2.2.0/pyrubi/servers/
--rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.2.0/pyrubi/servers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.286028 pyrubi-2.2.0/pyrubi/sessions/
--rw-rw-rw-   0        0        0      690 2023-06-27 12:19:25.000000 pyrubi-2.2.0/pyrubi/sessions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.287560 pyrubi-2.2.0/pyrubi/tools/
--rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.2.0/pyrubi/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-27 14:34:12.249184 pyrubi-2.2.0/pyrubi.egg-info/
--rw-rw-rw-   0        0        0     2156 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-27 14:34:12.000000 pyrubi-2.2.0/pyrubi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-27 14:34:12.288563 pyrubi-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1109 2023-06-27 14:32:51.000000 pyrubi-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.234609 pyrubi-2.2.1/
+-rw-rw-rw-   0        0        0     2251 2023-06-29 17:54:50.234609 pyrubi-2.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2023-06-29 17:51:32.000000 pyrubi-2.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.194502 pyrubi-2.2.1/pyrubi/
+-rw-rw-rw-   0        0        0      205 2023-06-29 16:41:57.000000 pyrubi-2.2.1/pyrubi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.212496 pyrubi-2.2.1/pyrubi/cryption/
+-rw-rw-rw-   0        0        0     3932 2023-06-27 09:26:51.000000 pyrubi-2.2.1/pyrubi/cryption/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.220494 pyrubi-2.2.1/pyrubi/handler/
+-rw-rw-rw-   0        0        0     1142 2023-06-27 09:30:29.000000 pyrubi-2.2.1/pyrubi/handler/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.221493 pyrubi-2.2.1/pyrubi/maker/
+-rw-rw-rw-   0        0        0     3399 2023-06-27 13:42:47.000000 pyrubi-2.2.1/pyrubi/maker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.228611 pyrubi-2.2.1/pyrubi/message/
+-rw-rw-rw-   0        0        0     3439 2023-06-29 17:42:57.000000 pyrubi-2.2.1/pyrubi/message/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.230611 pyrubi-2.2.1/pyrubi/methods/
+-rw-rw-rw-   0        0        0    45811 2023-06-29 17:47:51.000000 pyrubi-2.2.1/pyrubi/methods/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.231611 pyrubi-2.2.1/pyrubi/servers/
+-rw-rw-rw-   0        0        0      357 2023-06-27 08:13:23.000000 pyrubi-2.2.1/pyrubi/servers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.232610 pyrubi-2.2.1/pyrubi/sessions/
+-rw-rw-rw-   0        0        0      672 2023-06-29 17:23:20.000000 pyrubi-2.2.1/pyrubi/sessions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.233610 pyrubi-2.2.1/pyrubi/tools/
+-rw-rw-rw-   0        0        0     7297 2023-06-26 11:48:21.000000 pyrubi-2.2.1/pyrubi/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 17:54:50.211497 pyrubi-2.2.1/pyrubi.egg-info/
+-rw-rw-rw-   0        0        0     2251 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-29 17:54:50.000000 pyrubi-2.2.1/pyrubi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 17:54:50.234609 pyrubi-2.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1109 2023-06-29 17:48:53.000000 pyrubi-2.2.1/setup.py
```

### Comparing `pyrubi-2.2.0/PKG-INFO` & `pyrubi-2.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.2.0
+Version: 2.2.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,28 +13,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.2.0</h1>
+<h1>Pyrubi 2.2.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+
 **The Pyrubi library is compatible with version 6 of the Rubik's API**
 
 <hr>
 
 ## Install or Update:
 
 ``` bash
@@ -44,15 +46,15 @@
 <hr>
 
 ## Example:
 
 ``` python
 from pyrubi import Bot
 
-bot = Bot("session")
+bot = Bot("sessionName")
 
 for update in bot.on_message():
     if update.text() == 'hello':
         bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.2.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.2.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
 markdown
-****** Pyrubi 2.2.0 ******
+****** Pyrubi 2.2.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.0]
+                            [Pyrubi Library 2.2.1]
                              GitHub â¢ Documents
-**The Pyrubi library is compatible with version 6 of the Rubik's API**
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
+project/pyrubi) **The Pyrubi library is compatible with version 6 of the
+Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
-in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
-(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
-library.__", update.message_id()) ```
+## Example: ``` python from pyrubi import Bot bot = Bot("sessionName") for
+update in bot.on_message(): if update.text() == 'hello': bot.send_text
+(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is
+from the Pyrubi library.__", update.message_id()) ```
 ===============================================================================
 ## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
 ## Social Media: ### Rubika
```

### Comparing `pyrubi-2.2.0/README.md` & `pyrubi-2.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-<h1>Pyrubi 2.2.0</h1>
+<h1>Pyrubi 2.2.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+
 **The Pyrubi library is compatible with version 6 of the Rubik's API**
 
 <hr>
 
 ## Install or Update:
 
 ``` bash
@@ -25,15 +27,15 @@
 <hr>
 
 ## Example:
 
 ``` python
 from pyrubi import Bot
 
-bot = Bot("session")
+bot = Bot("sessionName")
 
 for update in bot.on_message():
     if update.text() == 'hello':
         bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-****** Pyrubi 2.2.0 ******
+****** Pyrubi 2.2.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.0]
+                            [Pyrubi Library 2.2.1]
                              GitHub â¢ Documents
-**The Pyrubi library is compatible with version 6 of the Rubik's API**
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
+project/pyrubi) **The Pyrubi library is compatible with version 6 of the
+Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
-in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
-(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
-library.__", update.message_id()) ```
+## Example: ``` python from pyrubi import Bot bot = Bot("sessionName") for
+update in bot.on_message(): if update.text() == 'hello': bot.send_text
+(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is
+from the Pyrubi library.__", update.message_id()) ```
 ===============================================================================
 ## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
 ## Social Media: ### Rubika
```

### Comparing `pyrubi-2.2.0/pyrubi/cryption/__init__.py` & `pyrubi-2.2.1/pyrubi/cryption/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.0/pyrubi/handler/__init__.py` & `pyrubi-2.2.1/pyrubi/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.0/pyrubi/maker/__init__.py` & `pyrubi-2.2.1/pyrubi/maker/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.0/pyrubi/methods/__init__.py` & `pyrubi-2.2.1/pyrubi/methods/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,17 @@
 from random import choice, randint
 from time import time
 from pathlib import Path
 
 class methods:
 
     def __init__(self, session:str):
-        if sessions.cheack_session(session):
-            self.session_data = sessions.session_data(session)
+        self.sessions = sessions()
+        if self.sessions.cheack_session(session):
+            self.session_data = self.sessions.session_data(session)
         else:
             self.method = maker(None, cryption6).method
             self.session_data = self.create_session(session, input("Enter the phone number: "))
 
         self.crypto = cryption6(self.session_data['auth'], self.session_data['private_key'])
         self.hs = handler(self.session_data['auth']).hand_shake
         self.method = maker(cryption6.changeAuthType(self.session_data['auth']), self.crypto).method
@@ -43,15 +44,15 @@
 
             session_data = {
                 'auth': cryption6.decryptRsaOaep(sign_in_data[1], sign_in_data[0]['auth']),
                 'private_key': sign_in_data[1],
                 'user': sign_in_data[0]['user'],
             }
 
-            sessions.create_session(session_name, session_data)
+            self.sessions.create_session(session_name, session_data)
 
             methods(session_name).register_device(
                 "Windows 10",
                 f"Pyrubi Library | {session_name}",
                 "25010064641090201001011130"
             )
```

### Comparing `pyrubi-2.2.0/pyrubi/tools/__init__.py` & `pyrubi-2.2.1/pyrubi/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrubi-2.2.0/pyrubi.egg-info/PKG-INFO` & `pyrubi-2.2.1/pyrubi.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrubi
-Version: 2.2.0
+Version: 2.2.1
 Summary: This is a powerful and easy library for building self Bots in Rubika
 Home-page: https://github.com/AliGanji1/pyrubi
 Author: Ali Ganji zadeh
 Author-email: ali.ganji.za@gmail.com
 Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -13,28 +13,30 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.6
 Description-Content-Type: text/markdown
 
-<h1>Pyrubi 2.2.0</h1>
+<h1>Pyrubi 2.2.1</h1>
 
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
 
 <p align='center'>
-    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.0' width='356' class="image">
+    <img src='https://iili.io/HIjPRS9.jpg' alt='Pyrubi Library 2.2.1' width='356' class="image">
 </p>
 
 <p align='center'>
     <a href='https://github.com/AliGanji1/pyrubi'>GitHub</a>
     •
     <a href='https://rubika.ir/pyrubika'>Documents</a>
 </p>
 
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/project/pyrubi)
+
 **The Pyrubi library is compatible with version 6 of the Rubik's API**
 
 <hr>
 
 ## Install or Update:
 
 ``` bash
@@ -44,15 +46,15 @@
 <hr>
 
 ## Example:
 
 ``` python
 from pyrubi import Bot
 
-bot = Bot("session")
+bot = Bot("sessionName")
 
 for update in bot.on_message():
     if update.text() == 'hello':
         bot.send_text(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi library.__", update.message_id())
 ```
 
 <hr>
```

#### html2text {}

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 2.1 Name: pyrubi Version: 2.2.0 Summary: This is a powerful
+Metadata-Version: 2.1 Name: pyrubi Version: 2.2.1 Summary: This is a powerful
 and easy library for building self Bots in Rubika Home-page: https://
 github.com/AliGanji1/pyrubi Author: Ali Ganji zadeh Author-email:
 ali.ganji.za@gmail.com Keywords: rubika,rubika-bot,pyrubi,rubx,rubino,rubika.ir
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: ~=3.6 Description-Content-Type: text/
 markdown
-****** Pyrubi 2.2.0 ******
+****** Pyrubi 2.2.1 ******
 > Pyrubi is a powerful and easy library for building self Bots in Rubika
-                            [Pyrubi Library 2.2.0]
+                            [Pyrubi Library 2.2.1]
                              GitHub â¢ Documents
-**The Pyrubi library is compatible with version 6 of the Rubik's API**
+[![Downloads](https://static.pepy.tech/badge/pyrubi)](https://pepy.tech/
+project/pyrubi) **The Pyrubi library is compatible with version 6 of the
+Rubik's API**
 ===============================================================================
 ## Install or Update: ``` bash pip install -U pyrubi ```
 ===============================================================================
-## Example: ``` python from pyrubi import Bot bot = Bot("session") for update
-in bot.on_message(): if update.text() == 'hello': bot.send_text(update.chat_id
-(), f"**Hello** ``{update.author_title()}``. __This message is from the Pyrubi
-library.__", update.message_id()) ```
+## Example: ``` python from pyrubi import Bot bot = Bot("sessionName") for
+update in bot.on_message(): if update.text() == 'hello': bot.send_text
+(update.chat_id(), f"**Hello** ``{update.author_title()}``. __This message is
+from the Pyrubi library.__", update.message_id()) ```
 ===============================================================================
 ## Features: - **Fast** : *The requests are very fast.* - **Easy** : *All
 methods and features are designed as easy and optimal as possible* -
 **Powerful** : *While the library is simple, it has high speed and features
 that make your work easier and faster*
 ===============================================================================
 ## Social Media: ### Rubika
```

### Comparing `pyrubi-2.2.0/setup.py` & `pyrubi-2.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'pyrubi',
-    version = '2.2.0',
+    version = '2.2.1',
     author='Ali Ganji zadeh',
     author_email = 'ali.ganji.za@gmail.com',
     description = 'This is a powerful and easy library for building self Bots in Rubika',
     keywords = ['rubika', 'rubika-bot', 'pyrubi', 'rubx', 'rubino', 'rubika.ir'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

