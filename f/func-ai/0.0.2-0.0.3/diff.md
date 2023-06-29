# Comparing `tmp/func_ai-0.0.2.tar.gz` & `tmp/func_ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.2.tar", max compression
+gzip compressed data, was "func_ai-0.0.3.tar", max compression
```

## Comparing `func_ai-0.0.2.tar` & `func_ai-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.2/LICENSE
--rw-r--r--   0        0        0      881 2023-06-29 17:44:19.322109 func_ai-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.2/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.2/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.2/func_ai/utils/__init__.py
--rw-r--r--   0        0        0     9504 2023-06-29 17:43:21.938646 func_ai-0.0.2/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0     2242 2023-06-29 09:45:30.583696 func_ai-0.0.2/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3392 2023-06-29 09:04:33.935006 func_ai-0.0.2/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-06-29 15:06:55.283947 func_ai-0.0.2/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      889 2023-06-29 16:09:54.454177 func_ai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1914 1970-01-01 00:00:00.000000 func_ai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-28 17:45:39.671843 func_ai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1036 2023-06-29 18:08:36.509794 func_ai-0.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 16:40:13.608045 func_ai-0.0.3/func_ai/__init__.py
+-rw-r--r--   0        0        0     4082 2023-06-28 17:47:54.691621 func_ai-0.0.3/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-06-28 17:11:55.264886 func_ai-0.0.3/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0    10240 2023-06-29 18:00:21.930012 func_ai-0.0.3/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0     2242 2023-06-29 09:45:30.583696 func_ai-0.0.3/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3392 2023-06-29 09:04:33.935006 func_ai-0.0.3/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-06-29 15:06:55.283947 func_ai-0.0.3/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      889 2023-06-29 18:06:04.015344 func_ai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2069 1970-01-01 00:00:00.000000 func_ai-0.0.3/PKG-INFO
```

### Comparing `func_ai-0.0.2/LICENSE` & `func_ai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.2/README.md` & `func_ai-0.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -41,8 +41,14 @@
 
 def test_user_openai_schema():
     print(User.from_prompt(prompt="Create a user with id 100 and name Jimmy", llm_interface=OpenAIInterface()).json())
     """
     Returns: {"id": 100, "name": "Jimmy"}
     """
 
-```
+```
+
+## Inspiration
+
+- https://github.com/jxnl/openai_function_call
+- https://github.com/rizerphe/openai-functions
+- https://github.com/aurelio-labs/funkagent
```

### Comparing `func_ai-0.0.2/func_ai/function_indexer.py` & `func_ai-0.0.3/func_ai/function_indexer.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.2/func_ai/utils/llm_tools.py` & `func_ai-0.0.3/func_ai/utils/llm_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import os
 import traceback
 from abc import abstractmethod
+from enum import Enum
 from typing import Any
 
 import openai
 from tenacity import retry, wait_fixed, stop_after_attempt
 
 from pydantic import BaseModel, Field
 
@@ -230,37 +231,54 @@
         Returns a string representation of a field definition
 
         :param name:
         :param field_info:
         :return:
         """
 
-        default = f"Default value: {field_info.default}" if not field_info.required else ""
+        default = f". Default value: {str(field_info.default)}" if not field_info.required else ""
         description = field_info.field_info.description
         if description:
             description = description.replace("\n", " ")
         else:
             description = ""
+        _enum_values = ""
+        if issubclass(field_info.outer_type_, Enum):
+            _enum_values = ". Enum: " + ",".join([f"{_enum.name}" for _enum in field_info.outer_type_])
         return {
-            "description": f"{description}. {default}",
+            "description": f"{description}{default}{_enum_values}",
             "type": type_mapping(field_info.outer_type_)
         }
 
     @classmethod
     def from_response(cls, completion, throw_error=True):
+        """
+        Returns an instance of the class from LLM completion response
 
+        :param completion: completion response from LLM
+        :param throw_error:  whether to throw error if function call is not present
+        :return:
+        """
         if throw_error:
             assert "function_call" in completion, "No function call detected"
             assert (
                     completion["function_call"]["name"] == cls.openai_schema["name"]
             ), "Function name does not match"
 
         function_call = completion["function_call"]
         arguments = json.loads(function_call["arguments"])
         return cls(**arguments)
 
     @classmethod
     def from_prompt(cls, prompt: str, llm_interface: LLMInterface, throw_error=True):
+        """
+        Returns an instance of the class from LLM prompt
+
+        :param prompt: User prompt
+        :param llm_interface: LLM interface
+        :param throw_error: whether to throw error if function call is not present
+        :return:
+        """
         completion = llm_interface.send(prompt, functions=[cls.openai_schema])
         # print(llm_interface.get_conversation())
         # TODO add crud interface functions here
         return cls.from_response(completion, throw_error)
```

### Comparing `func_ai-0.0.2/func_ai/utils/openapi_function_parser.py` & `func_ai-0.0.3/func_ai/utils/openapi_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.2/func_ai/utils/py_function_parser.py` & `func_ai-0.0.3/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.2/func_ai/workflow_creator.py` & `func_ai-0.0.3/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.2/pyproject.toml` & `func_ai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.2"
+version = "0.0.3"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
```

### Comparing `func_ai-0.0.2/PKG-INFO` & `func_ai-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func-ai
-Version: 0.0.2
+Version: 0.0.3
 Summary: AI Functional Catalog - OpenAI functions on steriods
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -68,7 +68,13 @@
 def test_user_openai_schema():
     print(User.from_prompt(prompt="Create a user with id 100 and name Jimmy", llm_interface=OpenAIInterface()).json())
     """
     Returns: {"id": 100, "name": "Jimmy"}
     """
 
 ```
+
+## Inspiration
+
+- https://github.com/jxnl/openai_function_call
+- https://github.com/rizerphe/openai-functions
+- https://github.com/aurelio-labs/funkagent
```

