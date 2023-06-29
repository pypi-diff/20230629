# Comparing `tmp/archytas-1.0.1.tar.gz` & `tmp/archytas-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archytas-1.0.1.tar", max compression
+gzip compressed data, was "archytas-1.0.2.tar", max compression
```

## Comparing `archytas-1.0.1.tar` & `archytas-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    32472 2023-06-01 14:07:03.452519 archytas-1.0.1/LICENSE
--rw-r--r--   0        0        0     2088 2023-06-01 14:07:03.452519 archytas-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/__init__.py
--rw-r--r--   0        0        0     9054 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/agent.py
--rw-r--r--   0        0        0     9746 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/demo_tools.py
--rw-r--r--   0        0        0     4129 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/prompt.py
--rw-r--r--   0        0        0     3166 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/python.py
--rw-r--r--   0        0        0     7630 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/react.py
--rw-r--r--   0        0        0     1462 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/repl.py
--rw-r--r--   0        0        0    18506 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/tool_utils.py
--rw-r--r--   0        0        0     4586 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/tools.py
--rw-r--r--   0        0        0     1251 2023-06-01 14:07:03.452519 archytas-1.0.1/archytas/utils.py
--rw-r--r--   0        0        0      780 2023-06-01 14:07:03.512519 archytas-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-06-29 16:09:47.604117 archytas-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2088 2023-06-29 16:09:47.604117 archytas-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/__init__.py
+-rw-r--r--   0        0        0     9054 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/agent.py
+-rw-r--r--   0        0        0     9746 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/demo_tools.py
+-rw-r--r--   0        0        0     4129 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/prompt.py
+-rw-r--r--   0        0        0     3166 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/python.py
+-rw-r--r--   0        0        0     8513 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/react.py
+-rw-r--r--   0        0        0     1462 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/repl.py
+-rw-r--r--   0        0        0    18506 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/tool_utils.py
+-rw-r--r--   0        0        0     4586 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/tools.py
+-rw-r--r--   0        0        0     1251 2023-06-29 16:09:47.604117 archytas-1.0.2/archytas/utils.py
+-rw-r--r--   0        0        0      780 2023-06-29 16:09:47.644118 archytas-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2923 1970-01-01 00:00:00.000000 archytas-1.0.2/PKG-INFO
```

### Comparing `archytas-1.0.1/LICENSE` & `archytas-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/README.md` & `archytas-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/agent.py` & `archytas-1.0.2/archytas/agent.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/demo_tools.py` & `archytas-1.0.2/archytas/demo_tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/prompt.py` & `archytas-1.0.2/archytas/prompt.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/python.py` & `archytas-1.0.2/archytas/python.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/react.py` & `archytas-1.0.2/archytas/react.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,20 @@
 from archytas.prompt import build_prompt, build_all_tool_names
 from archytas.tools import ask_user
 from archytas.tool_utils import make_tool_dict
 import json
 import pdb
 import sys
 import logging
+import typing
 
 logger = logging.Logger('archytas')
 
+class Undefined: ...
+
 class FailedTaskError(Exception): ...
 
 
 class LoopController:
     PROCEED = 0
     STOP_SUCCESS = 1
     STOP_FATAL = 2
@@ -24,36 +27,54 @@
 
     def set_state(self, new_value):
         self.state = new_value
 
     def reset(self):
         self.state = 0
 
-
 class ReActAgent(Agent):
-    def __init__(self, *, model:str='gpt-4', api_key:str|None=None, tools:list=None, allow_ask_user:bool=True, max_errors:int|None=3, max_react_steps:int|None=None, verbose:bool=False, **kwargs):
+    def __init__(
+        self,
+        *,
+        model: str = "gpt-4",
+        api_key: str | None = None,
+        tools: list = None,
+        allow_ask_user: bool = True,
+        max_errors: int | None = 3,
+        max_react_steps: int | None = None,
+        verbose: bool = False,
+        thought_handler: typing.Callable | None = Undefined,
+        **kwargs,
+    ):
         """
         Create a ReAct agent
 
         Args:
             model (str): The model to use. Defaults to 'gpt-4'. Recommended not to change this. gpt-3.5-turbo doesn't follow the prompt format.
             api_key (str, optional): The OpenAI API key to use. If not set, defaults to reading the API key from the OPENAI_API_KEY environment variable.
             tools (list): A list of tools to use. Defaults to None. If None, only the system tools (final_answer, fail_task) will be used.
             allow_ask_user (bool): Whether to include the ask_user tool, which allows the model to ask the user for clarification. Defaults to True.
             max_errors (int, optional): The maximum number of errors to allow during a task. Defaults to 3.
             max_react_steps (int, optional): The maximum number of steps to allow during a task. Defaults to infinity.
             verbose (bool, optional): Whether to print the agent's thoughts and observations. Defaults to False.
+            thought_handler (function, optional): Hook to control logging/output of the thoughts made in the middle of a react loop. Set to None to disable, or leave default of Undefined to 
+                    print to terminal. Otherwise expects a callable function with the signature of `func(thought: str, tool_name: str, tool_input: str) -> None`.
         """
 
         # create a dictionary for looking up tools by name
         tools = tools or []
         if allow_ask_user:
             tools.append(ask_user)
         self.tools = make_tool_dict(tools)
 
+        if thought_handler is Undefined:
+            self.thought_handler = self.thought_callback
+        else:
+            self.thought_handler = thought_handler
+
         #check that the tools dict keys match the list of generated tool names
         names, keys = sorted(build_all_tool_names(tools)), sorted([*self.tools.keys()])
         assert names == keys, f'Internal Error: tools dict keys does not match list of generated tool names. {names} != {keys}'
 
         # create the prompt with the tools, and initialize the agent
         self.prompt = build_prompt(tools)
         super().__init__(model=model, prompt=self.prompt, api_key=api_key, **kwargs)
@@ -67,14 +88,20 @@
         self.errors = 0
         self.steps = 0
 
         # keep track of the last tool used (for error messages)
         self.last_tool_name = ''
 
 
+    def thought_callback(self, thought: str, tool_name: str, tool_input: str) -> None:
+        if self.verbose:
+            #TODO: better coloring
+            self.print(f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n")
+
+
     def react(self, query:str) -> str:
         # reset error and steps counter
         self.errors = 0
         self.steps = 0
 
         # run the initial user query
         action_str = self.query(query)
@@ -98,18 +125,16 @@
                 thought, tool_name, tool_input = self.extract_action(action)
                 logger.debug(f"\nThought: {thought}\nTool name: {tool_name}\nTool input: {tool_input}")
                 self.last_tool_name = tool_name # keep track of the last tool used
             except AssertionError as e:
                 action_str = self.error(str(e))
                 continue
 
-            # print action
-            if self.verbose:
-                #TODO: better coloring
-                self.print(f"thought: {thought}\ntool: {tool_name}\ntool_input: {tool_input}\n")
+            if self.thought_handler:
+                self.thought_handler(thought, tool_name, tool_input)
 
             # exit ReAct loop if agent says final_answer or fail_task
             if tool_name == 'final_answer':
                 return tool_input
             if tool_name == 'fail_task':
                 raise FailedTaskError(tool_input)
```

### Comparing `archytas-1.0.1/archytas/repl.py` & `archytas-1.0.2/archytas/repl.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/tool_utils.py` & `archytas-1.0.2/archytas/tool_utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/tools.py` & `archytas-1.0.2/archytas/tools.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/archytas/utils.py` & `archytas-1.0.2/archytas/utils.py`

 * *Files identical despite different names*

### Comparing `archytas-1.0.1/pyproject.toml` & `archytas-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "archytas"
-version = "1.0.1"
+version = "1.0.2"
 description = "A library for pairing LLM agents with tools so they perform open ended tasks"
 authors = ["David Andrew Samson <david.andrew.engineer@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 
 [project.urls]
 "Homepage" = "https://github.com/jataware/archytas"
```

### Comparing `archytas-1.0.1/PKG-INFO` & `archytas-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archytas
-Version: 1.0.1
+Version: 1.0.2
 Summary: A library for pairing LLM agents with tools so they perform open ended tasks
 License: GPL-3.0-or-later
 Author: David Andrew Samson
 Author-email: david.andrew.engineer@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

