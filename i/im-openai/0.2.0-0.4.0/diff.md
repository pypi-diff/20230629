# Comparing `tmp/im_openai-0.2.0.tar.gz` & `tmp/im_openai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.2.0.tar", last modified: Tue Jun 27 22:35:32 2023, max compression
+gzip compressed data, was "im_openai-0.4.0.tar", last modified: Thu Jun 29 18:23:45 2023, max compression
```

## Comparing `im_openai-0.2.0.tar` & `im_openai-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-27 22:35:32.829151 im_openai-0.2.0/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.2.0/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.2.0/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.2.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.2.0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2635 2023-06-27 22:35:32.829688 im_openai-0.2.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.2.0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-27 22:35:32.784802 im_openai-0.2.0/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.2.0/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.2.0/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-27 22:35:32.800505 im_openai-0.2.0/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.2.0/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2341 2023-06-27 22:34:00.000000 im_openai-0.2.0/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2498 2023-06-27 22:33:34.000000 im_openai-0.2.0/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.2.0/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-27 22:35:32.821306 im_openai-0.2.0/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2635 2023-06-27 22:35:32.000000 im_openai-0.2.0/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      531 2023-06-27 22:35:32.000000 im_openai-0.2.0/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-27 22:35:32.000000 im_openai-0.2.0/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-27 22:35:32.000000 im_openai-0.2.0/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-27 22:35:32.000000 im_openai-0.2.0/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-27 22:35:32.831410 im_openai-0.2.0/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-26 18:47:51.000000 im_openai-0.2.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-27 22:35:32.827367 im_openai-0.2.0/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.2.0/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.2.0/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 18:23:45.442528 im_openai-0.4.0/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.4.0/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.4.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.4.0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2799 2023-06-29 18:23:45.443127 im_openai-0.4.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.4.0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 18:23:45.400786 im_openai-0.4.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.4.0/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.4.0/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 18:23:45.414792 im_openai-0.4.0/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-06-23 16:59:08.000000 im_openai-0.4.0/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3872 2023-06-29 18:15:38.000000 im_openai-0.4.0/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2812 2023-06-29 18:15:40.000000 im_openai-0.4.0/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.4.0/im_openai/template.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 18:23:45.432034 im_openai-0.4.0/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2799 2023-06-29 18:23:45.000000 im_openai-0.4.0/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      531 2023-06-29 18:23:45.000000 im_openai-0.4.0/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 18:23:45.000000 im_openai-0.4.0/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-29 18:23:45.000000 im_openai-0.4.0/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-06-29 18:23:45.000000 im_openai-0.4.0/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-06-29 18:23:45.445274 im_openai-0.4.0/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-06-29 18:22:09.000000 im_openai-0.4.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-29 18:23:45.440644 im_openai-0.4.0/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.4.0/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.4.0/tests/test_im_openai.py
```

### Comparing `im_openai-0.2.0/CONTRIBUTING.rst` & `im_openai-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/LICENSE` & `im_openai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/PKG-INFO` & `im_openai-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.2.0
+Version: 0.4.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -92,7 +92,15 @@
 ## 0.1.2 (2023-06-23)
 
 -   add support for original template too
 
 ## 0.2.0 (2023-06-26)
 
 - add explicit support for passing the "prompt template text"
+
+## 0.3.0 (2023-06-28)
+
+- add support for chat templates (as objects instead of arrays)
+
+## 0.4.0 (2023-06-29)
+
+- switch event reporting to be async / non-blocking
```

### Comparing `im_openai-0.2.0/README.md` & `im_openai-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/docs/Makefile` & `im_openai-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/docs/conf.py` & `im_openai-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/docs/installation.rst` & `im_openai-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/docs/make.bat` & `im_openai-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/im_openai/client.py` & `im_openai-0.4.0/im_openai/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,62 +1,73 @@
 import os
 import time
 import uuid
-from contextlib import contextmanager
+from contextlib import asynccontextmanager
+from typing import List
+import asyncio
+import aiohttp
+import warnings
 
-import requests
 
-
-def send_event(
+async def send_event(
+    session: aiohttp.ClientSession,
     project_key: str,
     api_name: str,
     prompt_event_id: str,
-    prompt_text: str,
+    prompt_template_text: str,
+    prompt_template_chat: List,
     prompt_params: dict = None,
     response: str = None,
     response_time: float = None,
 ):
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
         "projectKey": project_key,
         "apiName": api_name,
         "params": {},
         "prompt": {},
         "promptEventId": prompt_event_id,
     }
-    if prompt_text is not None:
-        # first default template to just the raw text
-        event["promptTemplateText"] = prompt_text
-
-        if prompt_params is None and getattr(prompt_text, "params", None):
-            # Can be TemplateString or any other
-            prompt_params = prompt_text.params
-
-        # If the original template is available, send it too
-        if getattr(prompt_text, "template", None):
-            event["promptTemplateText"] = prompt_text.template
+    if prompt_template_text is not None:
+        if isinstance(prompt_template_text, str):
+            # first default template to just the raw text
+            event["promptTemplateText"] = prompt_template_text
+            if prompt_params is None and getattr(prompt_template_text, "params", None):
+                # Can be TemplateString or any other
+                prompt_params = prompt_template_text.params
+
+            # If the original template is available, send it too
+            if getattr(prompt_template_text, "template", None):
+                event["promptTemplateText"] = prompt_template_text.template
+
+    elif prompt_template_chat is not None:
+        # We're going to assume that if a non-string was passed in, then it
+        # was probably a chat template, aka a chat message history
+
+        # TODO: figure out template extraction for chat templates
+        event["promptTemplateChat"] = prompt_template_chat
 
     if prompt_params is not None:
         event["params"] = prompt_params
     if response is not None:
         event["response"] = response
     if response_time is not None:
         event["responseTime"] = response_time
 
-    response = requests.post(PROMPT_REPORTING_URL, json=event)
-    response.raise_for_status()
+    await session.post(PROMPT_REPORTING_URL, json=event)
 
 
-@contextmanager
-def event_session(
+@asynccontextmanager
+async def event_session(
     project_key: str,
     api_name: str,
-    prompt_text: str,
+    prompt_template_text: str,
+    prompt_template_chat: List,
     prompt_template_params: dict = None,
     prompt_event_id: str = None,
 ):
     """Context manager for sending an event to Imaginary Dev.
 
     Usage::
 
@@ -64,24 +75,47 @@
             # do something
             complete_event(response)
 
     """
     start = time.time()
     if prompt_event_id is None:
         prompt_event_id = str(uuid.uuid4())
-    send_event(
-        project_key, api_name, prompt_event_id, prompt_text, prompt_template_params
-    )
 
-    def complete_event(response):
-        response_time = (time.time() - start) * 1000
-        send_event(
+    async with aiohttp.ClientSession() as session:
+        pending_events_sent = []
+        first_event_sent = send_event(
+            session,
             project_key,
             api_name,
             prompt_event_id,
-            prompt_text,
+            prompt_template_text,
+            prompt_template_chat,
             prompt_template_params,
-            response,
-            response_time,
         )
+        pending_events_sent.append(first_event_sent)
 
-    yield complete_event
+        async def complete_event(response):
+            response_time = (time.time() - start) * 1000
+            second_event_sent = send_event(
+                session,
+                project_key,
+                api_name,
+                prompt_event_id,
+                prompt_template_text,
+                prompt_template_chat,
+                prompt_template_params,
+                response,
+                response_time,
+            )
+            pending_events_sent.append(second_event_sent)
+
+        yield complete_event
+        w = time.time()
+        pending_events_results = await asyncio.gather(
+            *pending_events_sent, return_exceptions=True
+        )
+        failed_events = [e for e in pending_events_results if isinstance(e, Exception)]
+        if failed_events:
+            warnings.warn(
+                f"Failed to report calls. {len(failed_events)} failure(s). First failure: {failed_events[0]}",
+                stacklevel=3,
+            )
```

### Comparing `im_openai-0.2.0/im_openai/patch.py` & `im_openai-0.4.0/im_openai/patch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 import os
 from typing import Callable
 
 from openai import ChatCompletion, Completion
 
 from .client import event_session
+import asyncio
 
 
-def patch_openai_class(cls, get_prompt_text: Callable, get_result: Callable):
+def patch_openai_class(cls, get_prompt_template: Callable, get_result: Callable):
     oldcreate = cls.create
 
-    def local_create(
+    async def local_create(
         cls,
         *args,
         ip_project_key=None,
         ip_api_name=None,
         ip_event_id=None,
         ip_template_text=None,
+        ip_template_chat=None,
         ip_template_params=None,
         **kwargs
     ):
         if ip_project_key is None:
             ip_project_key = os.environ.get("PROMPT_PROJECT_KEY")
         if ip_project_key is None:
             return oldcreate(*args, **kwargs)
-        if ip_template_text is None:
-            ip_template_text = get_prompt_text(*args, **kwargs)
 
-        with event_session(
+        if ip_template_text is None and ip_template_chat is None:
+            ip_template = get_prompt_template(*args, **kwargs)
+            if isinstance(ip_template, str):
+                ip_template_text = ip_template
+            elif isinstance(ip_template, list):
+                ip_template_chat = ip_template
+
+        async with event_session(
             ip_project_key,
             ip_api_name,
             ip_template_text,
+            ip_template_chat,
             ip_template_params,
             ip_event_id,
         ) as complete_event:
             response = oldcreate(*args, **kwargs)
-            complete_event(get_result(response))
+            await complete_event(get_result(response))
         return response
 
     oldacreate = cls.acreate
 
     async def local_create_async(cls, *args, template=None, **kwargs):
         # TODO: record the request and response with the template
         return oldacreate(*args, **kwargs)
 
     setattr(
         cls,
         "create",
-        classmethod(lambda cls, *args, **kwds: local_create(cls, *args, **kwds)),
+        classmethod(
+            lambda cls, *args, **kwds: asyncio.run(local_create(cls, *args, **kwds))
+        ),
     )
     setattr(
         cls,
         "acreate",
         classmethod(lambda cls, *args, **kwds: local_create_async(cls, *args, **kwds)),
     )
 
@@ -62,29 +72,29 @@
 
 
 def patch_openai():
     """Patch openai APIs to add logging capabilities.
 
     Returns a function which may be called to "unpatch" the APIs."""
 
-    def get_completion_prompt_text(*args, prompt=None, **kwargs):
+    def get_completion_prompt(*args, prompt=None, **kwargs):
         return prompt
 
     unpatch_completion = patch_openai_class(
-        Completion, get_completion_prompt_text, lambda x: x["choices"][0]["text"]
+        Completion, get_completion_prompt, lambda x: x["choices"][0]["text"]
     )
 
-    def get_chat_prompt_text(*args, messages=None, **kwargs):
+    def get_chat_prompt(*args, messages=None, **kwargs):
         # TODO: What should we be sending? For now we'll just send the last message
-        prompt_text = messages[-1]["content"]
+        prompt_text = messages
         return prompt_text
 
     unpatch_chat = patch_openai_class(
         ChatCompletion,
-        get_chat_prompt_text,
+        get_chat_prompt,
         lambda x: x["choices"][0]["message"]["content"],
     )
 
     def unpatch():
         unpatch_chat()
         unpatch_completion()
```

### Comparing `im_openai-0.2.0/im_openai.egg-info/PKG-INFO` & `im_openai-0.4.0/im_openai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.2.0
+Version: 0.4.0
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -92,7 +92,15 @@
 ## 0.1.2 (2023-06-23)
 
 -   add support for original template too
 
 ## 0.2.0 (2023-06-26)
 
 - add explicit support for passing the "prompt template text"
+
+## 0.3.0 (2023-06-28)
+
+- add support for chat templates (as objects instead of arrays)
+
+## 0.4.0 (2023-06-29)
+
+- switch event reporting to be async / non-blocking
```

### Comparing `im_openai-0.2.0/im_openai.egg-info/SOURCES.txt` & `im_openai-0.4.0/im_openai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `im_openai-0.2.0/setup.py` & `im_openai-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.2.0",
+    version="0.4.0",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.2.0/tests/test_im_openai.py` & `im_openai-0.4.0/tests/test_im_openai.py`

 * *Files identical despite different names*

