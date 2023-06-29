# Comparing `tmp/revChatGPT-6.5.0.tar.gz` & `tmp/revChatGPT-6.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-6.5.0.tar", last modified: Mon Jun 26 15:53:05 2023, max compression
+gzip compressed data, was "revChatGPT-6.6.0.tar", last modified: Thu Jun 29 09:02:39 2023, max compression
```

## Comparing `revChatGPT-6.5.0.tar` & `revChatGPT-6.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.690529 revChatGPT-6.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.690529 revChatGPT-6.5.0/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    57017 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    24598 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/src/revChatGPT/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-26 15:53:05.000000 revChatGPT-6.5.0/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:53:05.694529 revChatGPT-6.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-26 15:52:29.000000 revChatGPT-6.5.0/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.598651 revChatGPT-6.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    58293 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24824 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/src/revChatGPT/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 09:02:39.000000 revChatGPT-6.6.0/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:02:39.602651 revChatGPT-6.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-29 09:02:07.000000 revChatGPT-6.6.0/tests/test_recipient.py
```

### Comparing `revChatGPT-6.5.0/LICENSE` & `revChatGPT-6.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/PKG-INFO` & `revChatGPT-6.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.5.0
+Version: 6.6.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.5.0/README.md` & `revChatGPT-6.6.0/README.md`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/setup.py` & `revChatGPT-6.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "httpx[socks]",
         "async_tio",
         "prompt-toolkit",
         "tiktoken>=0.3.0",
         "openai",
         "curl_cffi",
         "rich",
+        "tls_client>=0.2.1",
     ],
     classifiers=[
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
         "Intended Audience :: Developers",
         "Intended Audience :: End Users/Desktop",
         "Natural Language :: English",
         "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `revChatGPT-6.5.0/src/revChatGPT/V1.py` & `revChatGPT-6.6.0/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from pathlib import Path
 from typing import AsyncGenerator
 from typing import Generator
 from typing import NoReturn
 
 import httpx
 import requests
-import urllib
+import tls_client
 from httpx import AsyncClient
 from OpenAIAuth import Auth0 as Authenticator
 from rich.live import Live
 from rich.markdown import Markdown
 
 from . import __version__
 from . import typings as t
@@ -106,14 +106,43 @@
     return decorator
 
 
 BASE_URL = environ.get("CHATGPT_BASE_URL") or "https://bypass.churchless.tech/"
 
 bcolors = t.Colors()
 
+session = tls_client.Session(
+    client_identifier="firefox110", random_tls_extension_order=True
+)
+
+
+def get_arkose_token() -> str:
+    form_data = session.get(BASE_URL + "arkose").json().get("form")
+    resp: dict = session.post(
+        "https://tcr9i.chat.openai.com/fc/gt2/public_key/35536E1E-65B4-4D96-9D97-6ADB7EFF8147",
+        data=form_data,
+        headers={
+            "Host": "tcr9i.chat.openai.com",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:114.0) Gecko/20100101 Firefox/114.0",
+            "Accept": "*/*",
+            "Accept-Language": "en-US,en;q=0.5",
+            "Accept-Encoding": "gzip, deflate, br",
+            "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
+            "Origin": "https://tcr9i.chat.openai.com",
+            "DNT": "1",
+            "Connection": "keep-alive",
+            "Referer": "https://tcr9i.chat.openai.com/v2/1.5.2/enforcement.64b3a4e29686f93d52816249ecbf9857.html",
+            "Sec-Fetch-Dest": "empty",
+            "Sec-Fetch-Mode": "cors",
+            "Sec-Fetch-Site": "same-origin",
+            "TE": "trailers",
+        },
+    ).json()
+    return resp.get("token")
+
 
 class Chatbot:
     """
     Chatbot class for ChatGPT
     """
 
     @logger(is_timed=True)
@@ -380,14 +409,17 @@
         data: dict,
         auto_continue: bool = False,
         timeout: float = 360,
         **kwargs,
     ) -> Generator[dict, None, None]:
         log.debug("Sending the payload")
 
+        if data.get("model", "").startswith("gpt-4"):
+            data["arkose_token"] = get_arkose_token()
+
         cid, pid = data["conversation_id"], data["parent_message_id"]
         message = ""
 
         self.conversation_id_prev_queue.append(cid)
         self.parent_id_prev_queue.append(pid)
         response = self.session.post(
             url=f"{self.base_url}conversation",
```

### Comparing `revChatGPT-6.5.0/src/revChatGPT/V3.py` & `revChatGPT-6.6.0/src/revChatGPT/V3.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,17 @@
 
     # https://github.com/openai/openai-cookbook/blob/main/examples/How_to_count_tokens_with_tiktoken.ipynb
     def get_token_count(self, convo_id: str = "default") -> int:
         """
         Get token count
         """
         if self.engine not in ENGINES:
-            raise NotImplementedError(f"Engine {self.engine} is not supported. Select from {ENGINES}")
+            raise NotImplementedError(
+                f"Engine {self.engine} is not supported. Select from {ENGINES}"
+            )
         tiktoken.model.MODEL_TO_ENCODING["gpt-4"] = "cl100k_base"
 
         encoding = tiktoken.encoding_for_model(self.engine)
 
         num_tokens = 0
         for message in self.conversation[convo_id]:
             # every message follows <im_start>{role/name}\n{content}<im_end>\n
@@ -192,18 +194,26 @@
         if convo_id not in self.conversation:
             self.reset(convo_id=convo_id, system_prompt=self.system_prompt)
         self.add_to_conversation(prompt, "user", convo_id=convo_id)
         self.__truncate_conversation(convo_id=convo_id)
         # Get response
         if os.environ.get("API_URL") and os.environ.get("MODEL_NAME"):
             # https://learn.microsoft.com/en-us/azure/cognitive-services/openai/chatgpt-quickstart?tabs=command-line&pivots=rest-api
-            url = os.environ.get("API_URL") + "openai/deployments/" + os.environ.get("MODEL_NAME") +"/chat/completions?api-version=2023-05-15"
+            url = (
+                os.environ.get("API_URL")
+                + "openai/deployments/"
+                + os.environ.get("MODEL_NAME")
+                + "/chat/completions?api-version=2023-05-15"
+            )
             headers = {"Content-Type": "application/json", "api-key": self.api_key}
         else:
-            url = "https://api.openai.com/v1/chat/completions"
+            url = (
+                os.environ.get("API_URL")
+                or "https://api.openai.com/v1/chat/completions"
+            )
             headers = {"Authorization": f"Bearer {kwargs.get('api_key', self.api_key)}"}
         response = self.session.post(
             url,
             headers=headers,
             json={
                 "model": os.environ.get("MODEL_NAME") or model or self.engine,
                 "messages": self.conversation[convo_id] if pass_history else [prompt],
@@ -310,15 +320,15 @@
                 if not line:
                     continue
                 # Remove "data: "
                 line = line[6:]
                 if line == "[DONE]":
                     break
                 resp: dict = json.loads(line)
-                if 'error' in resp:
+                if "error" in resp:
                     raise t.ResponseError(f"{resp['error']}")
                 choices = resp.get("choices")
                 if not choices:
                     continue
                 delta: dict[str, str] = choices[0].get("delta")
                 if not delta:
                     continue
@@ -689,15 +699,18 @@
             )
         except KeyboardInterrupt:
             print("\nExiting...")
             sys.exit()
         if prompt.startswith("!"):
             try:
                 chatbot.handle_commands(prompt)
-            except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as err:
+            except (
+                requests.exceptions.Timeout,
+                requests.exceptions.ConnectionError,
+            ) as err:
                 print(f"Error: {err}")
                 continue
             continue
         print()
         print("ChatGPT: ", flush=True)
         if args.enable_internet:
             query = chatbot.ask(
@@ -739,8 +752,7 @@
     try:
         main()
     except Exception as exc:
         raise t.CLIError("Command line program unknown error") from exc
     except KeyboardInterrupt:
         print("\nExiting...")
         sys.exit()
-
```

### Comparing `revChatGPT-6.5.0/src/revChatGPT/__init__.py` & `revChatGPT-6.6.0/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/src/revChatGPT/__main__.py` & `revChatGPT-6.6.0/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/src/revChatGPT/config/enable_internet.json` & `revChatGPT-6.6.0/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/src/revChatGPT/typings.py` & `revChatGPT-6.6.0/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/src/revChatGPT/utils.py` & `revChatGPT-6.6.0/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-6.5.0/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-6.6.0/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 6.5.0
+Version: 6.6.0
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
```

### Comparing `revChatGPT-6.5.0/tests/test_recipient.py` & `revChatGPT-6.6.0/tests/test_recipient.py`

 * *Files identical despite different names*

