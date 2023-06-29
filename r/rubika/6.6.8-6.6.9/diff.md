# Comparing `tmp/rubika-6.6.8.tar.gz` & `tmp/rubika-6.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubika-6.6.8.tar", last modified: Thu Jun 29 20:49:30 2023, max compression
+gzip compressed data, was "rubika-6.6.9.tar", last modified: Thu Jun 29 20:54:58 2023, max compression
```

## Comparing `rubika-6.6.8.tar` & `rubika-6.6.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:49:30.910000 rubika-6.6.8/
--rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.6.8/LICENSE
--rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:49:30.910000 rubika-6.6.8/PKG-INFO
--rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.6.8/README.md
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:49:30.900000 rubika-6.6.8/rubika/
--rw-rw----   0 root         (0)     9997     5307 2023-06-29 17:52:20.000000 rubika-6.6.8/rubika/Types.py
--rw-rw----   0 root         (0)     9997      138 2023-06-29 20:48:13.000000 rubika-6.6.8/rubika/__init__.py
--rw-rw----   0 root         (0)     9997    42801 2023-06-29 17:49:59.000000 rubika-6.6.8/rubika/client.py
--rw-rw----   0 root         (0)     9997     6535 2023-06-29 17:50:36.000000 rubika-6.6.8/rubika/configs.py
--rw-rw----   0 root         (0)     9997     3771 2023-06-29 17:49:51.000000 rubika-6.6.8/rubika/encryption.py
--rw-rw----   0 root         (0)     9997      170 2023-06-13 09:40:35.000000 rubika-6.6.8/rubika/exceptions.py
--rw-rw----   0 root         (0)     9997     5458 2023-06-29 17:50:51.000000 rubika-6.6.8/rubika/fileIO.py
--rw-rw----   0 root         (0)     9997     5469 2023-06-09 08:44:46.000000 rubika-6.6.8/rubika/filters.py
--rw-rw----   0 root         (0)     9997     6444 2023-06-29 17:51:07.000000 rubika-6.6.8/rubika/rubino.py
--rw-rw----   0 root         (0)     9997     4580 2023-06-29 17:53:02.000000 rubika-6.6.8/rubika/setup.py
--rw-rw----   0 root         (0)     9997     6944 2023-06-29 17:52:00.000000 rubika-6.6.8/rubika/tools.py
-drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:49:30.910000 rubika-6.6.8/rubika.egg-info/
--rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:49:30.000000 rubika-6.6.8/rubika.egg-info/PKG-INFO
--rw-rw----   0 root         (0)     9997      410 2023-06-29 20:49:30.000000 rubika-6.6.8/rubika.egg-info/SOURCES.txt
--rw-rw----   0 root         (0)     9997        1 2023-06-29 20:49:30.000000 rubika-6.6.8/rubika.egg-info/dependency_links.txt
--rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.6.8/rubika.egg-info/not-zip-safe
--rw-rw----   0 root         (0)     9997       82 2023-06-29 20:49:30.000000 rubika-6.6.8/rubika.egg-info/requires.txt
--rw-rw----   0 root         (0)     9997        7 2023-06-29 20:49:30.000000 rubika-6.6.8/rubika.egg-info/top_level.txt
--rw-rw----   0 root         (0)     9997       79 2023-06-29 20:49:30.910000 rubika-6.6.8/setup.cfg
--rw-rw----   0 root         (0)     9997     2501 2023-06-29 20:48:38.000000 rubika-6.6.8/setup.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:54:58.580000 rubika-6.6.9/
+-rw-rw----   0 root         (0)     9997    35148 2023-04-07 14:31:47.000000 rubika-6.6.9/LICENSE
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:54:58.580000 rubika-6.6.9/PKG-INFO
+-rw-rw----   0 root         (0)     9997     2205 2023-04-07 14:31:47.000000 rubika-6.6.9/README.md
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:54:58.570000 rubika-6.6.9/rubika/
+-rw-rw----   0 root         (0)     9997     5307 2023-06-29 17:52:20.000000 rubika-6.6.9/rubika/Types.py
+-rw-rw----   0 root         (0)     9997      138 2023-06-29 20:48:13.000000 rubika-6.6.9/rubika/__init__.py
+-rw-rw----   0 root         (0)     9997    42765 2023-06-29 20:54:25.000000 rubika-6.6.9/rubika/client.py
+-rw-rw----   0 root         (0)     9997     6474 2023-06-29 20:54:05.000000 rubika-6.6.9/rubika/configs.py
+-rw-rw----   0 root         (0)     9997     3771 2023-06-29 17:49:51.000000 rubika-6.6.9/rubika/encryption.py
+-rw-rw----   0 root         (0)     9997      170 2023-06-13 09:40:35.000000 rubika-6.6.9/rubika/exceptions.py
+-rw-rw----   0 root         (0)     9997     5458 2023-06-29 17:50:51.000000 rubika-6.6.9/rubika/fileIO.py
+-rw-rw----   0 root         (0)     9997     5469 2023-06-09 08:44:46.000000 rubika-6.6.9/rubika/filters.py
+-rw-rw----   0 root         (0)     9997     6444 2023-06-29 17:51:07.000000 rubika-6.6.9/rubika/rubino.py
+-rw-rw----   0 root         (0)     9997     4580 2023-06-29 17:53:02.000000 rubika-6.6.9/rubika/setup.py
+-rw-rw----   0 root         (0)     9997     6944 2023-06-29 17:52:00.000000 rubika-6.6.9/rubika/tools.py
+drwxrwx---   0 root         (0)     9997        0 2023-06-29 20:54:58.580000 rubika-6.6.9/rubika.egg-info/
+-rw-rw----   0 root         (0)     9997     4192 2023-06-29 20:54:58.000000 rubika-6.6.9/rubika.egg-info/PKG-INFO
+-rw-rw----   0 root         (0)     9997      410 2023-06-29 20:54:58.000000 rubika-6.6.9/rubika.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0)     9997        1 2023-06-29 20:54:58.000000 rubika-6.6.9/rubika.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0)     9997        1 2023-04-07 14:31:47.000000 rubika-6.6.9/rubika.egg-info/not-zip-safe
+-rw-rw----   0 root         (0)     9997       82 2023-06-29 20:54:58.000000 rubika-6.6.9/rubika.egg-info/requires.txt
+-rw-rw----   0 root         (0)     9997        7 2023-06-29 20:54:58.000000 rubika-6.6.9/rubika.egg-info/top_level.txt
+-rw-rw----   0 root         (0)     9997       79 2023-06-29 20:54:58.580000 rubika-6.6.9/setup.cfg
+-rw-rw----   0 root         (0)     9997     2501 2023-06-29 20:54:41.000000 rubika-6.6.9/setup.py
```

### Comparing `rubika-6.6.8/LICENSE` & `rubika-6.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/PKG-INFO` & `rubika-6.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.6.8
+Version: 6.6.9
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
```

### Comparing `rubika-6.6.8/README.md` & `rubika-6.6.9/README.md`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/Types.py` & `rubika-6.6.9/rubika/Types.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/client.py` & `rubika-6.6.9/rubika/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
 
     def block(self, chat_id):
         return Bot._create(self.auth, "setBlockUser", {"action": "Block", "user_guid": chat_id})
 
 
     @staticmethod
     def _create(auth, method, data, client=clients.web):
-        print(auth, Bot.privateKey)
         return makeData(auth, encryption(encryption.changeAuthType(auth), private_key=Bot.privateKey), method, dict(data))
 
     @staticmethod
     def _createTMP(method, data, tmp=None):
         return makeTmpData(method, dict(data), tmp=tmp, url=_getURL(DCsURL=Bot.DCsURL, getDCsURL=Bot.getDCsURL, dc_id=None))
 
     @staticmethod
```

### Comparing `rubika-6.6.8/rubika/configs.py` & `rubika-6.6.9/rubika/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,14 @@
                     'Origin': 'https://'+platform,
 					'Referer': f'https://{platform}/',
 					'Host': url.replace("https://","").replace("/",""),
 					'User-Agent': defaultUserAgent
             }).text
             response = loads(str(enc.decrypt(loads(response).get("data_enc")))) if "data_enc" in loads(response).keys() and isEncrypted else loads(response)
             if "status" in response.keys() and response.get("status") != "OK":
-                print(json, method, url, platform, response)
                 if response.get("status_det") == "NOT_REGISTERED":
                     raise NotRegistered("the auth is incorrect. please sure about your account's health then login again.")
                 elif response.get("status_det") == "INVALID_INPUT":
                     raise InvalidInput(f"the inserted argument(s) is invaild in the {platform}/{method}. if you're sure about your argument(s), please report this message.")
                 elif response.get("status_det") == "TOO_REQUESTS":
                     raise TooRequests(f"the {platform}/{method} method has been limited. please try again later.")
                 elif response.get("status_det") == 'INVALID_AUTH':
```

### Comparing `rubika-6.6.8/rubika/encryption.py` & `rubika-6.6.9/rubika/encryption.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/fileIO.py` & `rubika-6.6.9/rubika/fileIO.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/filters.py` & `rubika-6.6.9/rubika/filters.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/rubino.py` & `rubika-6.6.9/rubika/rubino.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/setup.py` & `rubika-6.6.9/rubika/setup.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika/tools.py` & `rubika-6.6.9/rubika/tools.py`

 * *Files identical despite different names*

### Comparing `rubika-6.6.8/rubika.egg-info/PKG-INFO` & `rubika-6.6.9/rubika.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubika
-Version: 6.6.8
+Version: 6.6.9
 Summary: this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that
 Home-page: https://github.com/bahman-ahmadi/rubika
 Download-URL: https://github.com/bahman-ahmadi/rubika/releases/latest
 Author: Bahman Ahmadi
 Author-email: bahmanahmadi.mail@gmail.com
 License: LGPLv3
 Project-URL: Tracker, https://github.com/bahman-ahmadi/rubika/issues
```

### Comparing `rubika-6.6.8/setup.py` & `rubika-6.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from sys import argv
 from requests import get
 from setuptools import setup, find_packages
 
 requires = ["requests", "pycryptodome==3.10.1", "urllib3",
             "tqdm", "aiohttp", "rich", "websocket-client", "schedule"]
-version = "6.6.8"
+version = "6.6.9"
 readme = get(
     "https://raw.githubusercontent.com/Bahman-Ahmadi/rubika/main/README.md").text
 
 setup(
     name="rubika",
     version=version,
     description="this is an unofficial library for making bots in rubika. using this library you can make your own rubika bot and control that",
```

