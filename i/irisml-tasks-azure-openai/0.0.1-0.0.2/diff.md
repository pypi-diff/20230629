# Comparing `tmp/irisml-tasks-azure-openai-0.0.1.tar.gz` & `tmp/irisml-tasks-azure-openai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irisml-tasks-azure-openai-0.0.1.tar", last modified: Thu May  4 04:53:17 2023, max compression
+gzip compressed data, was "irisml-tasks-azure-openai-0.0.2.tar", last modified: Thu Jun 29 21:23:14 2023, max compression
```

## Comparing `irisml-tasks-azure-openai-0.0.1.tar` & `irisml-tasks-azure-openai-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/
--rw-r--r--   0 shono     (1000) shono     (1000)     1141 2023-05-04 04:41:30.000000 irisml-tasks-azure-openai-0.0.1/LICENSE
--rw-r--r--   0 shono     (1000) shono     (1000)     1834 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)     1545 2023-05-04 04:44:24.000000 irisml-tasks-azure-openai-0.0.1/README.md
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/irisml/
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/irisml/tasks/
--rw-r--r--   0 shono     (1000) shono     (1000)     3828 2023-05-04 04:48:11.000000 irisml-tasks-azure-openai-0.0.1/irisml/tasks/call_azure_openai_completion.py
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/
--rw-r--r--   0 shono     (1000) shono     (1000)     1834 2023-05-04 04:53:17.000000 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/PKG-INFO
--rw-r--r--   0 shono     (1000) shono     (1000)      373 2023-05-04 04:53:17.000000 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/SOURCES.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        1 2023-05-04 04:53:17.000000 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/dependency_links.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       32 2023-05-04 04:53:17.000000 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/requires.txt
--rw-r--r--   0 shono     (1000) shono     (1000)        7 2023-05-04 04:53:17.000000 irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/top_level.txt
--rw-r--r--   0 shono     (1000) shono     (1000)       81 2023-05-04 04:41:34.000000 irisml-tasks-azure-openai-0.0.1/pyproject.toml
--rw-r--r--   0 shono     (1000) shono     (1000)      517 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/setup.cfg
-drwxr-xr-x   0 shono     (1000) shono     (1000)        0 2023-05-04 04:53:17.566610 irisml-tasks-azure-openai-0.0.1/test/
--rw-r--r--   0 shono     (1000) shono     (1000)     1057 2023-05-04 04:41:34.000000 irisml-tasks-azure-openai-0.0.1/test/test_call_azure_openai_completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:14.675830 irisml-tasks-azure-openai-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 21:23:14.675830 irisml-tasks-azure-openai-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:14.671829 irisml-tasks-azure-openai-0.0.2/irisml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:14.671829 irisml-tasks-azure-openai-0.0.2/irisml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/irisml/tasks/call_azure_openai_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/irisml/tasks/create_azure_openai_chat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/irisml/tasks/create_azure_openai_completion_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:14.675830 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 21:23:14.000000 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-29 21:23:14.000000 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 21:23:14.000000 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 21:23:14.000000 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 21:23:14.000000 irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-29 21:23:14.675830 irisml-tasks-azure-openai-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 21:23:14.675830 irisml-tasks-azure-openai-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/test/test_call_azure_openai_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/test/test_create_azure_openai_chat_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-06-29 21:20:46.000000 irisml-tasks-azure-openai-0.0.2/test/test_create_azure_openai_completion_model.py
```

### Comparing `irisml-tasks-azure-openai-0.0.1/LICENSE` & `irisml-tasks-azure-openai-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-openai-0.0.1/PKG-INFO` & `irisml-tasks-azure-openai-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Azure OpenAI tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-openai
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-openai-0.0.1/README.md` & `irisml-tasks-azure-openai-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `irisml-tasks-azure-openai-0.0.1/irisml/tasks/call_azure_openai_completion.py` & `irisml-tasks-azure-openai-0.0.2/irisml/tasks/call_azure_openai_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             except Exception:
                 logger.exception(f"Failed to generate text {i}. Skipping.")
                 result = ''
                 num_tokens = 0
 
             texts.append(result)
             total_tokens += num_tokens
-            logger.info(f"Generated text {i}: {result} (prompt='{t}', {num_tokens} tokens, {time.time() - start_time} seconds)")
+            logger.info(f"Generated text {i}: {repr(result)} (prompt={repr(t)}, {num_tokens} tokens, {time.time() - start_time} seconds)")
             time.sleep(self.config.requests_interval)
 
         logger.info(f"Generated {len(texts)} texts. ({total_tokens} tokens)")
         return self.Outputs(texts=texts, total_tokens=total_tokens)
 
     def dry_run(self, inputs):
         self._check_config()
```

### Comparing `irisml-tasks-azure-openai-0.0.1/irisml_tasks_azure_openai.egg-info/PKG-INFO` & `irisml-tasks-azure-openai-0.0.2/irisml_tasks_azure_openai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irisml-tasks-azure-openai
-Version: 0.0.1
+Version: 0.0.2
 Summary: Azure OpenAI tasks for IrisML
 Home-page: https://github.com/microsoft/irisml-tasks-azure-openai
 Author: irisdev
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `irisml-tasks-azure-openai-0.0.1/setup.cfg` & `irisml-tasks-azure-openai-0.0.2/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = irisml-tasks-azure-openai
-version = 0.0.1
+version = 0.0.2
 url = https://github.com/microsoft/irisml-tasks-azure-openai
 description = Azure OpenAI tasks for IrisML
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = irisdev
 license = MIT
 
@@ -12,14 +12,15 @@
 packages = find_namespace:
 python_requires = >= 3.8
 install_requires = 
 	irisml
 	Pillow
 	requests
 	tenacity
+	torchvision
 
 [options.packages.find]
 include = 
 	irisml.tasks
 
 [flake8]
 max-line-length = 200
```

### Comparing `irisml-tasks-azure-openai-0.0.1/test/test_call_azure_openai_completion.py` & `irisml-tasks-azure-openai-0.0.2/test/test_call_azure_openai_completion.py`

 * *Files identical despite different names*

