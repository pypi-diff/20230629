# Comparing `tmp/ollama-0.0.3.tar.gz` & `tmp/ollama-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.3.tar", max compression
+gzip compressed data, was "ollama-0.0.4.tar", max compression
```

## Comparing `ollama-0.0.3.tar` & `ollama-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.3/LICENSE
--rw-r--r--   0        0        0     1870 2023-06-29 18:34:52.656897 ollama-0.0.3/README.md
--rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.3/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.3/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.3/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     2816 2023-06-29 18:34:52.658295 ollama-0.0.3/ollama/cmd/cli.py
--rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.3/ollama/cmd/server.py
--rw-r--r--   0        0        0     1495 2023-06-29 19:06:47.735287 ollama-0.0.3/ollama/engine.py
--rw-r--r--   0        0        0     3892 2023-06-29 19:06:47.735430 ollama-0.0.3/ollama/model.py
--rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.3/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.3/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.3/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.3/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.3/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.3/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.3/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.3/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.3/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.3/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      490 2023-06-29 19:06:58.735866 ollama-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 ollama-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 21:19:19.222162 ollama-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1870 2023-06-29 14:42:40.514873 ollama-0.0.4/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 21:06:55.414148 ollama-0.0.4/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:49:14.157072 ollama-0.0.4/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 20:49:24.964439 ollama-0.0.4/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     3269 2023-06-29 20:42:43.077175 ollama-0.0.4/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     2123 2023-06-29 14:42:40.516389 ollama-0.0.4/ollama/cmd/server.py
+-rw-r--r--   0        0        0     1682 2023-06-29 20:22:30.476717 ollama-0.0.4/ollama/engine.py
+-rw-r--r--   0        0        0     3905 2023-06-29 19:09:36.124508 ollama-0.0.4/ollama/model.py
+-rw-r--r--   0        0        0      618 2023-06-29 19:36:57.583354 ollama-0.0.4/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 19:41:40.782502 ollama-0.0.4/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782730 ollama-0.0.4/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 19:41:40.782903 ollama-0.0.4/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 19:41:40.783102 ollama-0.0.4/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 19:41:40.783315 ollama-0.0.4/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 19:41:40.783509 ollama-0.0.4/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 19:41:40.783707 ollama-0.0.4/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 19:41:40.783935 ollama-0.0.4/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 19:41:40.784222 ollama-0.0.4/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      508 2023-06-29 20:53:13.348101 ollama-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 ollama-0.0.4/PKG-INFO
```

### Comparing `ollama-0.0.3/LICENSE` & `ollama-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.3/README.md` & `ollama-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ollama-0.0.3/ollama/cmd/server.py` & `ollama-0.0.4/ollama/cmd/server.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.3/ollama/engine.py` & `ollama-0.0.4/ollama/engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -41,18 +41,21 @@
         stored_model_path = os.path.join(models_home, model, ".bin")
         if os.path.exists(stored_model_path):
             model_path = stored_model_path
         else:
             # try loading this as a path to a model, rather than a model name
             model_path = os.path.abspath(model)
 
-        # suppress LLM's output
-        with suppress_stderr():
-            llm = LLM(model_path, verbose=False)
-            llms.update({model: llm})
-
+        try:
+            # suppress LLM's output
+            with suppress_stderr():
+                llm = LLM(model_path, verbose=False)
+                llms.update({model: llm})
+        except Exception as e:
+            # e is sent to devnull, so create a generic exception
+            raise Exception(f"Failed to load model: {model}")
     return llm
 
 
 def unload(model, llms={}):
     if model in llms:
         llms.pop(model)
```

### Comparing `ollama-0.0.3/ollama/model.py` & `ollama-0.0.4/ollama/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     print(f'Pulling {os.path.basename(location)}...')
 
     header = {'Range': f'bytes={first_byte}-'} if first_byte != 0 else {}
 
     response = requests.get(download_url, headers=header, stream=True)
     response.raise_for_status()
 
-    total_size = int(response.headers.get('content-length', 0))
+    total_size = int(response.headers.get('content-length', 0)) + first_byte
 
     with open(local_filename, 'ab' if first_byte else 'wb') as file, tqdm(
         total=total_size,
         unit='iB',
         unit_scale=True,
         unit_divisor=1024,
         initial=first_byte,
```

### Comparing `ollama-0.0.3/ollama/prompt.py` & `ollama-0.0.4/ollama/prompt.py`

 * *Files identical despite different names*

### Comparing `ollama-0.0.3/PKG-INFO` & `ollama-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.0.3
+Version: 0.0.4
 Summary: Run ai models locally
 Author: ollama team
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -12,14 +12,15 @@
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: aiohttp-cors (>=0.7.0,<0.8.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: llama-cpp-python (>=0.1.66,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: validators (>=0.20.0,<0.21.0)
+Requires-Dist: yaspin (>=2.3.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Ollama
 
 Run ai models locally.
 
 > _Note: this project is a work in progress. The features below are still in development_
```

