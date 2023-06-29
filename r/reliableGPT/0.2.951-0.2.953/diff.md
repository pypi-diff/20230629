# Comparing `tmp/reliableGPT-0.2.951.tar.gz` & `tmp/reliableGPT-0.2.953.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.951.tar", last modified: Thu Jun 29 00:36:07 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.953.tar", last modified: Thu Jun 29 21:45:46 2023, max compression
```

## Comparing `reliableGPT-0.2.951.tar` & `reliableGPT-0.2.953.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-29 00:36:07.184575 reliableGPT-0.2.951/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.951/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-29 00:36:07.184465 reliableGPT-0.2.951/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7112 2023-06-28 20:45:06.000000 reliableGPT-0.2.951/README.md
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      497 2023-06-28 20:45:06.000000 reliableGPT-0.2.951/pyproject.toml
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-29 00:36:07.183417 reliableGPT-0.2.951/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-29 00:36:07.000000 reliableGPT-0.2.951/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      450 2023-06-29 00:36:07.000000 reliableGPT-0.2.951/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-29 00:36:07.000000 reliableGPT-0.2.951/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       54 2023-06-29 00:36:07.000000 reliableGPT-0.2.951/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-29 00:36:07.000000 reliableGPT-0.2.951/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-29 00:36:07.184322 reliableGPT-0.2.951/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4210 2023-06-28 20:45:06.000000 reliableGPT-0.2.951/reliablegpt/APICallHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3120 2023-06-28 23:12:14.000000 reliableGPT-0.2.951/reliablegpt/Alerting.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4407 2023-06-28 20:45:06.000000 reliableGPT-0.2.951/reliablegpt/CustomQueue.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9965 2023-06-29 00:33:01.000000 reliableGPT-0.2.951/reliablegpt/IndividualRequest.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      753 2023-06-28 20:45:06.000000 reliableGPT-0.2.951/reliablegpt/Model.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     5170 2023-06-29 00:34:47.000000 reliableGPT-0.2.951/reliablegpt/RateLimitHandler.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      247 2023-06-28 23:12:17.000000 reliableGPT-0.2.951/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     3723 2023-06-29 00:34:09.000000 reliableGPT-0.2.951/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-29 00:36:07.184610 reliableGPT-0.2.951/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      398 2023-06-29 00:35:03.000000 reliableGPT-0.2.951/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.247001 reliableGPT-0.2.953/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-06-23 13:49:22.000000 reliableGPT-0.2.953/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-06-29 21:45:46.246870 reliableGPT-0.2.953/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     7112 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/README.md
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      497 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/pyproject.toml
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.245261 reliableGPT-0.2.953/reliableGPT.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      156 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      450 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       54 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       12 2023-06-29 21:45:46.000000 reliableGPT-0.2.953/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-06-29 21:45:46.246549 reliableGPT-0.2.953/reliablegpt/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4210 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/APICallHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3120 2023-06-29 21:36:46.000000 reliableGPT-0.2.953/reliablegpt/Alerting.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     4407 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/CustomQueue.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11224 2023-06-29 21:28:36.000000 reliableGPT-0.2.953/reliablegpt/IndividualRequest.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1286 2023-06-29 21:07:50.000000 reliableGPT-0.2.953/reliablegpt/Model.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     5195 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/RateLimitHandler.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      247 2023-06-29 02:51:34.000000 reliableGPT-0.2.953/reliablegpt/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     3921 2023-06-29 21:41:17.000000 reliableGPT-0.2.953/reliablegpt/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-06-29 21:45:46.247062 reliableGPT-0.2.953/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      398 2023-06-29 21:45:22.000000 reliableGPT-0.2.953/setup.py
```

### Comparing `reliableGPT-0.2.951/LICENSE` & `reliableGPT-0.2.953/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.951/README.md` & `reliableGPT-0.2.953/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.951/reliablegpt/APICallHandler.py` & `reliableGPT-0.2.953/reliablegpt/APICallHandler.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.951/reliablegpt/Alerting.py` & `reliableGPT-0.2.953/reliablegpt/Alerting.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.951/reliablegpt/CustomQueue.py` & `reliableGPT-0.2.953/reliablegpt/CustomQueue.py`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.951/reliablegpt/IndividualRequest.py` & `reliableGPT-0.2.953/reliablegpt/IndividualRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from termcolor import colored
 import requests
 import copy
-import openai
 import posthog
-
-
+import importlib
+import openai
+from openai import ChatCompletion
+import traceback
 
 class IndividualRequest:
   """A brief description of the class."""
 
   def __init__(self,
                model=None,
                fallback_strategy=[
@@ -16,67 +17,86 @@
                  'text-davinci-002'
                ],
                graceful_string="Sorry, the OpenAI API is currently down",
                user_email="",
                user_token="",
                send_notification=False,
                logging_fn=None,
+               backup_openai_key="",
                verbose=False):
     # Initialize instance variables
     self.model = model
     self.model_function = model.get_model_function()
     self.verbose = verbose
     self.graceful_string = graceful_string
     self.fallback_strategy = fallback_strategy
     self.user_email = user_email
     self.user_token = user_token
     self.save_request = logging_fn
+    self.backup_openai_key = backup_openai_key
 
     self.print_verbose(f"INIT fallback strategy {self.fallback_strategy}")
 
   def print_verbose(self, print_statement):
     if self.verbose:
       print(colored("Individual Request: " + print_statement, "blue"))
 
   ## Code that handles / wraps openai calls
   def __call__(self, *args, **kwargs):
     try:
       self.print_verbose(f"calling model function: {self.model_function}")
       self.print_verbose(f"these are the kwargs: {kwargs}")
-      try:
-        # this should never block running the openai call
-        self.save_request(
-            user_email=self.user_email,
-            graceful_string=self.graceful_string,
-            posthog_event='reliableGPT.request',
-        )
-      except:
-        print("ReliableGPT error occured during saving request")
+      self.print_verbose(f"this is the openai api base: {openai.api_base}")
       result = self.model_function(*args, **kwargs)
       self.print_verbose(f"This is the result: {str(result)[:500]}")
       return result
     except Exception as e:
       self.print_verbose("catches the error")
       return self.handle_exception(args, kwargs, e)
 
   def fallback_request(self, args, kwargs, fallback_strategy):
-    result = None
-    for model in fallback_strategy:
+    try: 
+      self.print_verbose("In fallback request")
+      result = None
       new_kwargs = copy.deepcopy(kwargs)  # Create a deep copy of kwargs
-      new_kwargs['model'] = model  # Update the model
-      result = self.make_LLM_request(new_kwargs)
-      if result != None:
-        return result
-    return None
+      if self.backup_openai_key and len(self.backup_openai_key) > 0: # user passed in a backup key for the raw openai endpoint
+        # switch to the raw openai model instead of using azure. 
+        new_kwargs["openai2"] = openai.__dict__.copy() # preserve the azure endpoint details
+        if "Embedding" in str(self.model_function):
+          fallback_strategy = ["text-embedding-ada-002"]
+
+      for model in fallback_strategy:
+        new_kwargs['model'] = model  # Update the model
+        result = self.make_LLM_request(new_kwargs)
+        if result != None:
+          return result
+      return None
+    except:
+      self.print_verbose(traceback.format_exc())
+      return None
 
   def make_LLM_request(self, new_kwargs):
     embedding_model = self.model.get_original_embeddings()
     chat_model = self.model.get_original_chat()
     completion_model = self.model.get_original_completion()
     try:
+      self.print_verbose(f"{new_kwargs.keys()}")
+      if "openai2" in new_kwargs:
+        openai.api_type = "openai"
+        openai.api_base = "https://api.openai.com/v1"
+        openai.api_version = None
+        openai.api_key = self.backup_openai_key
+        new_kwargs_except_openai_attributes = {k: v for k, v in new_kwargs.items() if k != "openai2"}
+        new_kwargs_except_engine = {k: v for k, v in new_kwargs_except_openai_attributes.items() if k != "engine"}
+        completion = self.model_function(**new_kwargs_except_engine)
+        openai.api_type = new_kwargs["openai2"]["api_type"]
+        openai.api_base = new_kwargs["openai2"]["api_base"]
+        openai.api_version = new_kwargs["openai2"]["api_version"]
+        openai.api_key = new_kwargs["openai2"]["api_key"]
+        return completion
       if "embedding" in str(self.model_function):
         # retry embedding with diff key
         print(colored(f"ReliableGPT: Retrying Embedding request", "blue"))
         return embedding_model(**new_kwargs)
 
       model = str(new_kwargs['model'])
       print(
```

### Comparing `reliableGPT-0.2.951/reliablegpt/RateLimitHandler.py` & `reliableGPT-0.2.953/reliablegpt/RateLimitHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import uuid
 import time
 import traceback
 
 
 ## Dev Imports 
 # from IndividualRequest import IndividualRequest
-# from APICallHandler import APICallHandler
+# from RateLimitHandler_helpers.APICallHandler import APICallHandler
 
 ## Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.APICallHandler import APICallHandler
 
 
 class RateLimitHandler:
```

### Comparing `reliableGPT-0.2.951/reliablegpt/main.py` & `reliableGPT-0.2.953/reliablegpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# Prod Imports
+# # Prod Imports
 from reliablegpt.IndividualRequest import IndividualRequest
 from reliablegpt.RateLimitHandler import RateLimitHandler
 from reliablegpt.Model import Model
-from reliablegpt.alerting import Alerting
+from reliablegpt.Alerting import Alerting
 
 # # Dev Imports
 # from IndividualRequest import IndividualRequest
 # from RateLimitHandler import RateLimitHandler
 # from Model import Model
-# from alerting import Alerting
+# from Alerting import Alerting
 
 from posthog import Posthog
 
 posthog = Posthog(
   project_api_key='phc_yZ30KsPzRXd3nYaET3VFDmquFKtMZwMTuFKVOei6viB',
   host='https://app.posthog.com')
 
@@ -22,14 +22,15 @@
 def save_request(user_email,
                  graceful_string,
                  posthog_event="",
                  result="",
                  posthog_metadata={},
                  errors=[]):
   try:
+    #metadata  = kwargs['metadata']
     if posthog_event != "":
       posthog.capture(user_email, posthog_event,
                       posthog_metadata)  # save posthog event
     if result == graceful_string or len(
         errors) == 2:  # returns a graceful string or got a 2nd exception
       # send an email and alert
       for error in errors:
@@ -44,15 +45,17 @@
              'gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'
            ],
            graceful_string="Sorry, the OpenAI API is currently down",
            user_email="",
            user_token="",
            send_notification=True,
            model_limits_dir={},
-           queue_requests=False):
+           backup_openai_key=None,
+           queue_requests=False, 
+           verbose=False):
   """Determine if an instantiation is calling the rate limit handler or the individual request wrapper directly and return the correct object"""
 
   primary_email = ""  # which api key management is mapped to
   ## Add email for alerting
   if isinstance(user_email, str):
     if user_email == "":
       raise ValueError("ReliableGPT Error: Please pass in a user email")
@@ -69,23 +72,25 @@
   if queue_requests == False:
     return IndividualRequest(model,
                              fallback_strategy=fallback_strategy,
                              graceful_string=graceful_string,
                              user_email=primary_email,
                              user_token=user_token,
                              logging_fn=save_request,
-                             send_notification=send_notification)
+                             send_notification=send_notification,
+                             backup_openai_key=backup_openai_key, 
+                             verbose=verbose)
   elif queue_requests == True:
     max_token_capacity = 40000
     max_request_capacity = 200
     ## [TODO]: Allow handling multiple model types (gpt-3.5-turbo AND gpt-4)
     if model_limits_dir and isinstance(model_limits_dir, dict):
-      keys = list(model_limits_dir.keys())
+      keys = model_limits_dir.keys()
       max_token_capacity = model_limits_dir[keys[0]]["max_token_capacity"]
-      max_request_capacity = model_limits_dir[keys[0]]["max_request_capacity"]
+      max_request_capacity = model_limits_dir["max_request_capacity"]
 
     return RateLimitHandler(model,
                             fallback_strategy=fallback_strategy,
                             graceful_string=graceful_string,
                             user_email=primary_email,
                             user_token=user_token,
                             send_notification=send_notification,
```

