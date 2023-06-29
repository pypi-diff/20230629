# Comparing `tmp/aicodebot-0.6.1.1.tar.gz` & `tmp/aicodebot-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aicodebot-0.6.1.1.tar", last modified: Thu Jun 29 15:20:34 2023, max compression
+gzip compressed data, was "aicodebot-0.6.2.tar", last modified: Thu Jun 29 19:43:30 2023, max compression
```

## Comparing `aicodebot-0.6.1.1.tar` & `aicodebot-0.6.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.050724 aicodebot-0.6.1.1/aicodebot/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/.aicodebot.template
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/aicodebot/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/alignment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/commit_message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/fun_fact.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/aicodebot/prompts/review.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:20:34.050724 aicodebot-0.6.1.1/aicodebot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 15:20:34.000000 aicodebot-0.6.1.1/aicodebot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:20:34.054724 aicodebot-0.6.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 15:20:06.000000 aicodebot-0.6.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-29 19:43:05.000000 aicodebot-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-29 19:43:30.361267 aicodebot-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-06-29 19:43:05.000000 aicodebot-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/.aicodebot.template
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13229 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/alignment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/commit_message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/fun_fact.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-29 19:43:05.000000 aicodebot-0.6.2/aicodebot/prompts/review.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:43:30.361267 aicodebot-0.6.2/aicodebot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-29 19:43:30.000000 aicodebot-0.6.2/aicodebot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-29 19:43:05.000000 aicodebot-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:43:30.361267 aicodebot-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-29 19:43:05.000000 aicodebot-0.6.2/setup.py
```

### Comparing `aicodebot-0.6.1.1/LICENSE` & `aicodebot-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/PKG-INFO` & `aicodebot-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.6.1.1
+Version: 0.6.2
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -47,27 +47,17 @@
 
 ### AI-Assisted Debugging
 
 `aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
 ### AI-Assisted Code Creation (Work in Progress)
 
-`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
 
-1. **Task Understanding**: The bot collects your task instructions.
-2. **Planning**: It devises a plan based on your task.
-3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
-4. **Clarification**: It asks questions if any aspect of the task is unclear.
-5. **Code Generation**: It generates code consistent with your codebase style.
-6. **Self-Review**: It reviews and improves the generated code.
-7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
-8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
-9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
-
-This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
+This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
```

### Comparing `aicodebot-0.6.1.1/README.md` & `aicodebot-0.6.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -30,27 +30,17 @@
 
 ### AI-Assisted Debugging
 
 `aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
 ### AI-Assisted Code Creation (Work in Progress)
 
-`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
 
-1. **Task Understanding**: The bot collects your task instructions.
-2. **Planning**: It devises a plan based on your task.
-3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
-4. **Clarification**: It asks questions if any aspect of the task is unclear.
-5. **Code Generation**: It generates code consistent with your codebase style.
-6. **Self-Review**: It reviews and improves the generated code.
-7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
-8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
-9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
-
-This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
+This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
```

### Comparing `aicodebot-0.6.1.1/aicodebot/cli.py` & `aicodebot-0.6.2/aicodebot/cli.py`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/aicodebot/helpers.py` & `aicodebot-0.6.2/aicodebot/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         file_status = exec_and_get_output(["git", "diff", diff_type, "--name-status"]).splitlines()
 
         diffs = []
         for status in file_status:
             status_code, file_name = status.split("\t")
             if status_code == "A":
                 # If the file is new, include the entire file content
-                contents = Path.read_text(file_name)
+                contents = Path(file_name).read_text()
                 diffs.append(f"## New file added: {file_name}")
                 diffs.append(contents)
             else:
                 # If the file is not new, get the diff
                 diffs.append(f"## File changed: {file_name}")
                 diffs.append(exec_and_get_output(base_git_diff + [diff_type, "--", file_name]))
```

### Comparing `aicodebot-0.6.1.1/aicodebot/prompts/alignment.yaml` & `aicodebot-0.6.2/aicodebot/prompts/alignment.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/aicodebot/prompts/commit_message.yaml` & `aicodebot-0.6.2/aicodebot/prompts/commit_message.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/aicodebot/prompts/review.yaml` & `aicodebot-0.6.2/aicodebot/prompts/review.yaml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/aicodebot.egg-info/PKG-INFO` & `aicodebot-0.6.2/aicodebot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aicodebot
-Version: 0.6.1.1
+Version: 0.6.2
 Summary: Your AI-powered coding companion: AI Code Bot 🤖
 Home-page: https://github.com/novara_ai/aicodebot
 Author: Nick Sullivan
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -47,27 +47,17 @@
 
 ### AI-Assisted Debugging
 
 `aicodebot debug $command` will run the command and capture the log message. It will pass the error message, stack trace, comand output, etc. to the AI and respond with some suggestions on how to fix it. It saves a trip to stackoverflow in a separate window, allowing you to stay in terminal with all the context.
 
 ### AI-Assisted Code Creation (Work in Progress)
 
-`aicodebot code` is a feature designed to automate coding tasks based on your instructions. It's a work in progress, but here's how it works:
+The aicodebot code feature is an AI-powered tool that automates coding tasks. It understands your task, formulates a plan, learns necessary information, and generates code that fits your codebase style. It also reviews its own work, modifies the local code, and creates unit tests. This feature is designed to streamline your coding process and boost productivity. In the future, we plan to enhance its performance through a continuous learning system based on user feedback and interaction outcomes.
 
-1. **Task Understanding**: The bot collects your task instructions.
-2. **Planning**: It devises a plan based on your task.
-3. **Learning**: It learns necessary information by searching the internet, reading the local codebase, and researching libraries/APIs.
-4. **Clarification**: It asks questions if any aspect of the task is unclear.
-5. **Code Generation**: It generates code consistent with your codebase style.
-6. **Self-Review**: It reviews and improves the generated code.
-7. **Code Modification**: It modifies the local code, allowing you to review changes before committing.
-8. **Test Creation**: It writes and runs unit tests for the new code, modifying the code until all tests pass.
-9. **Continuous Learning (v2)**: We plan to implement a system where the bot learns from each interaction, improving its performance over time based on feedback like code acceptance, compilation success, and test results.
-
-This feature is a work in progress, and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
+This feature is a work in progress, and it's more thoroughly documented [here](docs/code_agent.md) and we're excited about its potential to boost developer productivity. If you'd like to help, see [CONTRIBUTING](CONTRIBUTING.md).
 
 ## Getting Started
 
 [![PyPI version](https://badge.fury.io/py/aicodebot.svg)](https://badge.fury.io/py/aicodebot)
 
 To install AICodeBot, run:
```

### Comparing `aicodebot-0.6.1.1/aicodebot.egg-info/SOURCES.txt` & `aicodebot-0.6.2/aicodebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/pyproject.toml` & `aicodebot-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aicodebot-0.6.1.1/setup.py` & `aicodebot-0.6.2/setup.py`

 * *Files identical despite different names*

