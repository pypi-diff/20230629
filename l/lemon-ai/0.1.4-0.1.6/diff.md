# Comparing `tmp/lemon-ai-0.1.4.tar.gz` & `tmp/lemon-ai-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lemon-ai-0.1.4.tar", last modified: Tue Jun 27 16:25:06 2023, max compression
+gzip compressed data, was "lemon-ai-0.1.6.tar", last modified: Thu Jun 29 10:21:02 2023, max compression
```

## Comparing `lemon-ai-0.1.4.tar` & `lemon-ai-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.591953 lemon-ai-0.1.4/
--rw-r--r--   0 aah120    (1000) aah120    (1000)     3077 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/.gitignore
--rw-r--r--   0 aah120    (1000) aah120    (1000)    11357 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/LICENSE
--rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-27 16:55:30.588947 lemon-ai-0.1.4/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)     6436 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/README.md
--rw-r--r--   0 aah120    (1000) aah120    (1000)    33634 2023-06-27 16:44:44.000000 lemon-ai-0.1.4/heatmap.ipynb
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.451950 lemon-ai-0.1.4/lemon_ai/
--rw-r--r--   0 aah120    (1000) aah120    (1000)      109 2023-06-27 16:55:19.000000 lemon-ai-0.1.4/lemon_ai/__init__.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1741 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/cito_api_wrapper.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      840 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/cito_tool.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     5161 2023-06-27 16:39:55.000000 lemon-ai-0.1.4/lemon_ai/cito_toolkit.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      457 2023-06-27 16:39:55.000000 lemon-ai-0.1.4/lemon_ai/cito_workflow.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)     1411 2023-06-27 16:41:20.000000 lemon-ai-0.1.4/lemon_ai/execute_workflow.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)      822 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/get_integrations.py
--rw-r--r--   0 aah120    (1000) aah120    (1000)       16 2023-06-27 12:26:22.000000 lemon-ai-0.1.4/lemon_ai/requirements.txt
-drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-27 16:55:30.569743 lemon-ai-0.1.4/lemon_ai.egg-info/
--rw-r--r--   0 aah120    (1000) aah120    (1000)      724 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/PKG-INFO
--rw-r--r--   0 aah120    (1000) aah120    (1000)      417 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/SOURCES.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/dependency_links.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/requires.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-27 16:55:30.000000 lemon-ai-0.1.4/lemon_ai.egg-info/top_level.txt
--rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-27 16:55:30.592948 lemon-ai-0.1.4/setup.cfg
--rw-r--r--   0 aah120    (1000) aah120    (1000)      852 2023-06-27 16:55:12.000000 lemon-ai-0.1.4/setup.py
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-29 10:21:02.529645 lemon-ai-0.1.6/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     3077 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/.gitignore
+-rw-r--r--   0 aah120    (1000) aah120    (1000)    11357 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/LICENSE
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     6529 2023-06-29 10:21:02.520588 lemon-ai-0.1.6/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     5762 2023-06-29 10:09:16.000000 lemon-ai-0.1.6/README.md
+-rw-r--r--   0 aah120    (1000) aah120    (1000)    33634 2023-06-29 09:58:01.000000 lemon-ai-0.1.6/heatmap.ipynb
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-29 10:21:02.319577 lemon-ai-0.1.6/lemon_ai/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      109 2023-06-29 10:20:44.000000 lemon-ai-0.1.6/lemon_ai/__init__.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1741 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/lemon_ai/cito_api_wrapper.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      840 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/lemon_ai/cito_tool.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     5161 2023-06-27 16:39:55.000000 lemon-ai-0.1.6/lemon_ai/cito_toolkit.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      457 2023-06-27 16:39:55.000000 lemon-ai-0.1.6/lemon_ai/cito_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1411 2023-06-27 16:41:20.000000 lemon-ai-0.1.6/lemon_ai/execute_workflow.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      822 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/lemon_ai/get_integrations.py
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       16 2023-06-27 12:26:22.000000 lemon-ai-0.1.6/lemon_ai/requirements.txt
+drwxr-xr-x   0 aah120    (1000) aah120    (1000)        0 2023-06-29 10:21:02.481687 lemon-ai-0.1.6/lemon_ai.egg-info/
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     6529 2023-06-29 10:21:01.000000 lemon-ai-0.1.6/lemon_ai.egg-info/PKG-INFO
+-rw-r--r--   0 aah120    (1000) aah120    (1000)      417 2023-06-29 10:21:01.000000 lemon-ai-0.1.6/lemon_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        1 2023-06-29 10:21:01.000000 lemon-ai-0.1.6/lemon_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       17 2023-06-29 10:21:01.000000 lemon-ai-0.1.6/lemon_ai.egg-info/requires.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)        9 2023-06-29 10:21:01.000000 lemon-ai-0.1.6/lemon_ai.egg-info/top_level.txt
+-rw-r--r--   0 aah120    (1000) aah120    (1000)       38 2023-06-29 10:21:02.529645 lemon-ai-0.1.6/setup.cfg
+-rw-r--r--   0 aah120    (1000) aah120    (1000)     1039 2023-06-29 10:20:35.000000 lemon-ai-0.1.6/setup.py
```

### Comparing `lemon-ai-0.1.4/.gitignore` & `lemon-ai-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/LICENSE` & `lemon-ai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/README.md` & `lemon-ai-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,34 +44,30 @@
 Airtable (baseId: {airtable_base_id}, tableId: {airtable_table_id}). Only write the fields "username", "karma"
 and "created_at_i". Please make sure that Airtable does NOT automatically convert the field types.
 """
 
 # Initialise your model before passing it into the execute_workflow() function
 model = OpenAI(temperature=0)
 
-execute_workflow(model=model, prompt_string=prompt)
+execute_workflow(llm=model, prompt_string=prompt)
 ```
 
 It is crucial to ensure the parameters are specified in the prompt otherwise the execution will fail.
 
 ### Lemon AI Functions - Solve Tasks Based on Predefined Workflows
 
 Similar to [OpenAI's functions](https://openai.com/blog/function-calling-and-other-api-updates), Lemon AI provides the option to define workflows as reusable functions. Specific workflows can be defined in a separate lemonai.json:
 
 ```json
-// lemonai.json
-
 [
   {
     "name": "Hackernews Airtable User Workflow",
     "description": "retrieves user data from Hackernews and appends it to a table in Airtable",
     "tools": ["hackernews-get-user", "airtable-append-data"]
   }
-
-  //...
 ]
 ```
 
 In addition to Lemon AI's common set of tools, those workflow functions will also be provided to the model. Workflow functions can help to solve tasks in a specific way. This is especially helpful in situations where more deterministic model behavior is needed.
 
 Please make sure to provide a proper workflow 'description' and provide the 'tools' in the right order to allow the correct execution of the workflow '['tool to be used first', ...]'.
 
@@ -95,26 +91,26 @@
 and tableId {airtable_table_id}. Only write the fields 'username', 'karma' and 'created_at_i' to the Airtable
 table. Please make sure that Airtable does NOT automatically convert the field types."
 """
 
 # Initialise your model before passing it into the execute_workflow() function
 model = OpenAI(temperature=0)
 
-execute_workflow(model=model, prompt_string=prompt)
+execute_workflow(llm=model, prompt_string=prompt)
 ```
 
-The console output should show the intermediate steps taken by the Langchain agent to execute your prompt as well as the final answer. There will also be an output.log file which will log all tools/workflows used in each session and the final result of execution.
+## Traceability
+
+To allow you to gain full transparency on how your model interacted with your Lemon AI tools to solve the given task, we are writing all decisions made, tools used and operations performed to a local output.log file.
 
 ```log
-2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User -
-2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table -
-2023-06-26T11:50:45.792924+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - I read the user information for 'kimburgess' from Hackernews and wrote it to Airtable. The result was a record with the fields 'username', 'karma' and 'created_at_i' with the values 'kimburgess', 2454 and 1362302320 respectively.
-2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User -
-2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table -
-2023-06-26T11:58:52.504537+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - I read the user information for 'kimburgess' from Hackernews and wrote it to Airtable. The result was a record with the fields 'username', 'karma' and 'created_at_i' with the values 'kimburgess', 2454 and 1362302320 respectively.
+2023-06-26T11:50:27.708785+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - HackerNews: Get User
+2023-06-26T11:50:39.624035+0100 - b5f91c59-8487-45c2-800a-156eac0c7dae - Airtable: Append the data to a table
+2023-06-26T11:58:32.925228+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - HackerNews: Get User
+2023-06-26T11:58:43.988788+0100 - 5efe603c-9898-4143-b99a-55b50007ed9d - Airtable: Append the data to a table
 ```
 
 ## Supported Tools
 
 Below is a list of all supported tools by Lemon AI and their ids (for use in the lemonai.json workflow file):
 
 #### HackerNews:
```

### Comparing `lemon-ai-0.1.4/heatmap.ipynb` & `lemon-ai-0.1.6/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/lemon_ai/cito_api_wrapper.py` & `lemon-ai-0.1.6/lemon_ai/cito_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/lemon_ai/cito_tool.py` & `lemon-ai-0.1.6/lemon_ai/cito_tool.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/lemon_ai/cito_toolkit.py` & `lemon-ai-0.1.6/lemon_ai/cito_toolkit.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/lemon_ai/execute_workflow.py` & `lemon-ai-0.1.6/lemon_ai/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/lemon_ai/get_integrations.py` & `lemon-ai-0.1.6/lemon_ai/get_integrations.py`

 * *Files identical despite different names*

### Comparing `lemon-ai-0.1.4/setup.py` & `lemon-ai-0.1.6/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from setuptools import setup
 
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name='lemon-ai',
-    version='0.1.4',    
+    version='0.1.6',    
     description='A Python client that enables Langchain agents to design and execute workflow automations targeting internal tooling',
     author='Felix Brockmeier',
     author_email='felix@citodata.com',
-    url="https://github.com/feliciori/lemon-ai-client-python",
-    license='MIT',
+    url="https://github.com/feliciori/lemonai-py-client",
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    license='Apache License 2.0',
     packages=['lemon_ai'],
     python_requires='>=3.8.1',
     install_requires=[
         'langchain',
         'loguru'
     ],
     classifiers=[
```

