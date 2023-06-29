# Comparing `tmp/lemon-ai-0.1.3.tar.gz` & `tmp/lemon-ai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon-ai-0.1.3.tar", last modified: Mon Jun 26 13:28:02 2023, max compression
+gzip compressed data, was "lemon-ai-0.1.4.tar", last modified: Tue Jun 27 16:25:06 2023, max compression
```

## Comparing `lemon-ai-0.1.3.tar` & `lemon-ai-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 13:28:02.791198 lemon-ai-0.1.3/
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1076 2023-06-22 18:20:13.000000 lemon-ai-0.1.3/LICENSE
--rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-26 13:28:02.786204 lemon-ai-0.1.3/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)        0 2023-06-26 10:11:43.000000 lemon-ai-0.1.3/README.md
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 13:28:02.625977 lemon-ai-0.1.3/lemon_ai/
--rw-r--r--   0 aah120    (1000) aah120    (1000)      109 2023-06-26 13:27:02.000000 lemon-ai-0.1.3/lemon_ai/__init__.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1741 2023-06-23 11:04:03.000000 lemon-ai-0.1.3/lemon_ai/cito_api_wrapper.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      840 2023-06-23 09:17:19.000000 lemon-ai-0.1.3/lemon_ai/cito_tool.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     5309 2023-06-23 11:35:50.000000 lemon-ai-0.1.3/lemon_ai/cito_toolkit.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      609 2023-06-23 08:27:59.000000 lemon-ai-0.1.3/lemon_ai/cito_workflow.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1564 2023-06-26 13:26:00.000000 lemon-ai-0.1.3/lemon_ai/execute_workflow.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      822 2023-06-23 08:58:16.000000 lemon-ai-0.1.3/lemon_ai/get_integrations.py
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-26 13:28:02.742604 lemon-ai-0.1.3/lemon_ai.egg-info/
--rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-26 13:28:01.000000 lemon-ai-0.1.3/lemon_ai.egg-info/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)      366 2023-06-26 13:28:01.000000 lemon-ai-0.1.3/lemon_ai.egg-info/SOURCES.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-26 13:28:01.000000 lemon-ai-0.1.3/lemon_ai.egg-info/dependency_links.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-26 13:28:01.000000 lemon-ai-0.1.3/lemon_ai.egg-info/requires.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-26 13:28:01.000000 lemon-ai-0.1.3/lemon_ai.egg-info/top_level.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-26 13:28:02.792206 lemon-ai-0.1.3/setup.cfg
--rw-r--r--   0 aah120    (1000) aah120    (1000)      852 2023-06-26 13:27:10.000000 lemon-ai-0.1.3/setup.py
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.591953 lemon-ai-0.1.4/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     3077 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/.gitignore
+-rw-r--r--   0 aah120    (1000) aah120    (1000)    11357 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/LICENSE
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-27 16:55:30.588947 lemon-ai-0.1.4/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     6436 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/README.md
+-rw-r--r--   0 aah120    (1000) aah120    (1000)    33634 2023-06-27 16:44:44.000000 lemon-ai-0.1.4/heatmap.ipynb
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.451950 lemon-ai-0.1.4/lemon_ai/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      109 2023-06-27 16:55:19.000000 lemon-ai-0.1.4/lemon_ai/__init__.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1741 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/cito_api_wrapper.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      840 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/cito_tool.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     5161 2023-06-27 16:39:55.000000 lemon-ai-0.1.4/lemon_ai/cito_toolkit.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      457 2023-06-27 16:39:55.000000 lemon-ai-0.1.4/lemon_ai/cito_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1411 2023-06-27 16:41:20.000000 lemon-ai-0.1.4/lemon_ai/execute_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      822 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/get_integrations.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       16 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/requirements.txt
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.569743 lemon-ai-0.1.4/lemon_ai.egg-info/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      417 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/requires.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/top_level.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-27 16:55:30.592948 lemon-ai-0.1.4/setup.cfg
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      852 2023-06-27 16:55:12.000000 lemon-ai-0.1.4/setup.py
```

### Comparing `lemon-ai-0.1.3/PKG-INFO` & `lemon-ai-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon-ai
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling
 Home-page: https://github.com/feliciori/lemon-ai-client-python
 Author: Felix Brockmeier
 Author-email: felix@citodata.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lemon-ai-0.1.3/lemon_ai/cito_api_wrapper.py` & `lemon-ai-0.1.4/lemon_ai/cito_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.3/lemon_ai/cito_tool.py` & `lemon-ai-0.1.4/lemon_ai/cito_tool.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.3/lemon_ai/cito_toolkit.py` & `lemon-ai-0.1.4/lemon_ai/cito_toolkit.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         
         for key in access_token_dict:
             if key in action_id:
                 access_token = access_token_dict[key]
     
         return api_key, access_token
     
-    def _get_workflows_from_file(tools_list: List[CitoTool], logger: Logger, session_id: str) -> List[CitoWorkflow]:
+    def _get_workflows_from_file(tools_list: List[CitoTool]) -> List[CitoWorkflow]:
         workflows = []
 
-        with open("workflow.json", "r") as file:
+        with open("lemonai.json", "r") as file:
             data = json.load(file)
             tool_ids_list = [tool.id for tool in tools_list]
 
             for item in data:
                 required_tools = item["tools"]
                 tools_objs = []
                 ignore = False
@@ -47,16 +47,14 @@
                 if not ignore:
                     tool_names = [tool.name for tool in tools_objs]
                     workflows.append(
                         CitoWorkflow(
                             name=item["name"],
                             description=CitoToolkit._build_workflow_description(item["name"], item["description"], tool_names),
                             tools=tools_objs,
-                            logger=logger,
-                            session_id=session_id
                     ))
 
         return workflows
 
     def _build_workflow_description(name: str, description: str, tool_names: List[str]) -> str:
         return f"A wrapper around Lemon AI workflows. To run this workflow, run each tool in the workflow's tools list in the correct order to achieve the goal given by the workflow's description. You MUST take into account the params when executing each stage of the workflow. Sometimes, but not always, the output from a tool in the workflow may need to be used as the param for another tool in the workflow. For example, if the workflow's description is \"send the latest weather information in an email to mohammed@citodata.com\", first you would need to retrieve the latest weather information using one tool and then send that tool's output in an email to the given recipient, using the weather information as a param for the tool to send the email. You MUST use every tool that is given in the workflow's tools list once and in the same order as the list. Do not make up params, they will be explicitly specified in each tool's description. Do not use any tools that are not in this workflow's tools list. If you do not have enough information to fill in the params for a tool, just say 'not enough information provided in the instruction, missing <param>'. If you get a null or none response, STOP EXECUTION, do not try another tool! This workflow is named:{name} and has the goal:{description} and this workflow's tools list is: {tool_names}" 
 
@@ -94,15 +92,15 @@
                         api_wrapper=api_wrapper,
                         api_key=api_key,
                         access_token=access_token,
                         logger=logger,
                         session_id=session_id
                     ))
         
-        if os.path.exists("workflow.json"):
-            workflows = cls._get_workflows_from_file(cito_tools, logger, session_id)
+        if os.path.exists("lemonai.json"):
+            workflows = cls._get_workflows_from_file(cito_tools)
             cito_tools.extend(workflows)
 
         return cls(tools=cito_tools)
 
     def get_tools(self) -> List[CitoTool]:
         return self.tools
```

### Comparing `lemon-ai-0.1.3/lemon_ai/get_integrations.py` & `lemon-ai-0.1.4/lemon_ai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.3/lemon_ai.egg-info/PKG-INFO` & `lemon-ai-0.1.4/lemon_ai.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lemon-ai
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling
 Home-page: https://github.com/feliciori/lemon-ai-client-python
 Author: Felix Brockmeier
 Author-email: felix@citodata.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lemon-ai-0.1.3/setup.py` & `lemon-ai-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='lemon-ai',
-    version='0.1.3',    
+    version='0.1.4',    
     description='A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling',
     author='Felix Brockmeier',
     author_email='felix@citodata.com',
     url="https://github.com/feliciori/lemon-ai-client-python",
     license='MIT',
     packages=['lemon_ai'],
     python_requires='>=3.8.1',
```

