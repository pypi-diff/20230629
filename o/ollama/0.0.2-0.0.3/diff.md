# Comparing `tmp/ollama-0.0.2.tar.gz` & `tmp/ollama-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama-0.0.2.tar", max compression
+gzip compressed data, was "ollama-0.0.3.tar", max compression
```

## Comparing `ollama-0.0.2.tar` & `ollama-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2023-06-26 21:49:18.368771 ollama-0.0.2/LICENSE
--rw-r--r--   0        0        0     2016 2023-06-28 19:40:37.104272 ollama-0.0.2/README.md
--rw-r--r--   0        0        0      152 2023-06-27 20:27:59.113927 ollama-0.0.2/ollama/__init__.py
--rw-r--r--   0        0        0       70 2023-06-27 21:45:02.867694 ollama-0.0.2/ollama/__main__.py
--rw-r--r--   0        0        0        0 2023-06-27 21:25:07.935115 ollama-0.0.2/ollama/cmd/__init__.py
--rw-r--r--   0        0        0     2351 2023-06-28 22:48:04.582988 ollama-0.0.2/ollama/cmd/cli.py
--rw-r--r--   0        0        0     2075 2023-06-28 22:48:04.583723 ollama-0.0.2/ollama/cmd/server.py
--rw-r--r--   0        0        0     1471 2023-06-28 22:48:04.584352 ollama-0.0.2/ollama/engine.py
--rw-r--r--   0        0        0     2596 2023-06-28 19:46:56.507243 ollama-0.0.2/ollama/model.py
--rw-r--r--   0        0        0      607 2023-06-28 22:48:04.585093 ollama-0.0.2/ollama/prompt.py
--rw-r--r--   0        0        0      154 2023-06-28 18:51:43.063656 ollama-0.0.2/ollama/templates/alpaca.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:51:43.063962 ollama-0.0.2/ollama/templates/gpt4.prompt
--rw-r--r--   0        0        0       46 2023-06-28 18:51:43.064096 ollama-0.0.2/ollama/templates/hermes.prompt
--rw-r--r--   0        0        0       13 2023-06-28 18:51:43.064273 ollama-0.0.2/ollama/templates/oasst.prompt
--rw-r--r--   0        0        0      141 2023-06-28 22:03:18.518503 ollama-0.0.2/ollama/templates/orca.prompt
--rw-r--r--   0        0        0       39 2023-06-28 18:51:43.064711 ollama-0.0.2/ollama/templates/qlora.prompt
--rw-r--r--   0        0        0       16 2023-06-28 18:51:43.064890 ollama-0.0.2/ollama/templates/tulu.prompt
--rw-r--r--   0        0        0      186 2023-06-28 18:51:43.065060 ollama-0.0.2/ollama/templates/vicuna.prompt
--rw-r--r--   0        0        0       27 2023-06-28 18:51:43.065261 ollama-0.0.2/ollama/templates/wizardlm.prompt
--rw-r--r--   0        0        0      812 2023-06-28 22:47:59.898795 ollama-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 ollama-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1058 2023-06-26 19:56:14.979617 ollama-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1870 2023-06-29 18:34:52.656897 ollama-0.0.3/README.md
+-rw-r--r--   0        0        0      152 2023-06-28 18:43:09.587198 ollama-0.0.3/ollama/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-28 14:57:23.288184 ollama-0.0.3/ollama/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-27 21:07:07.679438 ollama-0.0.3/ollama/cmd/__init__.py
+-rw-r--r--   0        0        0     2816 2023-06-29 18:34:52.658295 ollama-0.0.3/ollama/cmd/cli.py
+-rw-r--r--   0        0        0     2123 2023-06-29 18:34:52.658544 ollama-0.0.3/ollama/cmd/server.py
+-rw-r--r--   0        0        0     1495 2023-06-29 19:06:47.735287 ollama-0.0.3/ollama/engine.py
+-rw-r--r--   0        0        0     3892 2023-06-29 19:06:47.735430 ollama-0.0.3/ollama/model.py
+-rw-r--r--   0        0        0      618 2023-06-29 19:06:47.735551 ollama-0.0.3/ollama/prompt.py
+-rw-r--r--   0        0        0      154 2023-06-28 18:57:14.634245 ollama-0.0.3/ollama/templates/alpaca.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634372 ollama-0.0.3/ollama/templates/gpt4.prompt
+-rw-r--r--   0        0        0       46 2023-06-28 18:57:14.634451 ollama-0.0.3/ollama/templates/hermes.prompt
+-rw-r--r--   0        0        0       13 2023-06-28 18:57:14.634568 ollama-0.0.3/ollama/templates/oasst.prompt
+-rw-r--r--   0        0        0      141 2023-06-28 18:57:14.634683 ollama-0.0.3/ollama/templates/orca.prompt
+-rw-r--r--   0        0        0       39 2023-06-28 18:57:14.634794 ollama-0.0.3/ollama/templates/qlora.prompt
+-rw-r--r--   0        0        0       16 2023-06-28 18:57:14.634913 ollama-0.0.3/ollama/templates/tulu.prompt
+-rw-r--r--   0        0        0      186 2023-06-28 18:57:14.635053 ollama-0.0.3/ollama/templates/vicuna.prompt
+-rw-r--r--   0        0        0       27 2023-06-28 18:57:14.635179 ollama-0.0.3/ollama/templates/wizardlm.prompt
+-rw-r--r--   0        0        0      490 2023-06-29 19:06:58.735866 ollama-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 ollama-0.0.3/PKG-INFO
```

### Comparing `ollama-0.0.2/LICENSE` & `ollama-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama-0.0.2/README.md` & `ollama-0.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -16,29 +16,20 @@
 
 ## Install
 
 ```
 pip install ollama
 ```
 
-## Install From Source
-
-```
-git clone git@github.com:jmorganca/ollama ollama
-cd ollama
-pip install -r requirements.txt
-pip install -e .
-```
-
 ## Quickstart
 
 ```
 % ollama run huggingface.co/TheBloke/orca_mini_3B-GGML
 Pulling huggingface.co/TheBloke/orca_mini_3B-GGML...
-Downloading [================>          ] 66.67% (2/3) 30.2MB/s
+Downloading [================           ] 66.67% 11.8MiB/s
 
 ...
 ...
 ...
 
 > Hello
```

### Comparing `ollama-0.0.2/ollama/cmd/cli.py` & `ollama-0.0.3/ollama/cmd/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 import sys
-import json
 from pathlib import Path
 from argparse import ArgumentParser
 
 from ollama import model, engine
 from ollama.cmd import server
 
 
@@ -25,17 +24,22 @@
     generate_parser.set_defaults(fn=generate)
 
     add_parser = subparsers.add_parser("add")
     add_parser.add_argument("model")
     add_parser.set_defaults(fn=add)
 
     pull_parser = subparsers.add_parser("pull")
-    pull_parser.add_argument("remote")
+    pull_parser.add_argument("model")
     pull_parser.set_defaults(fn=pull)
 
+    pull_parser = subparsers.add_parser("run")
+    pull_parser.add_argument("model")
+    pull_parser.add_argument("prompt", nargs="?")
+    pull_parser.set_defaults(fn=run)
+
     args = parser.parse_args()
     args = vars(args)
 
     try:
         fn = args.pop("fn")
         fn(**args)
     except KeyboardInterrupt:
@@ -48,47 +52,62 @@
 
 def list_models(*args, **kwargs):
     for m in model.models(*args, **kwargs):
         print(m)
 
 
 def generate(*args, **kwargs):
-    if prompt := kwargs.get('prompt'):
-        print('>>>', prompt, flush=True)
-        print(flush=True)
+    if prompt := kwargs.get("prompt"):
+        print(">>>", prompt, flush=True)
         generate_oneshot(*args, **kwargs)
-        print(flush=True)
         return
 
-    return generate_interactive(*args, **kwargs)
+    if sys.stdin.isatty():
+        return generate_interactive(*args, **kwargs)
+
+    return generate_batch(*args, **kwargs)
 
 
 def generate_oneshot(*args, **kwargs):
+    print(flush=True)
+
     for output in engine.generate(*args, **kwargs):
-        output = json.loads(output)
         choices = output.get("choices", [])
         if len(choices) > 0:
             print(choices[0].get("text", ""), end="", flush=True)
 
     # end with a new line
-    print()
+    print(flush=True)
+    print(flush=True)
 
 
 def generate_interactive(*args, **kwargs):
-    print('>>> ', end='', flush=True)
-    for line in sys.stdin:
-        if not sys.stdin.isatty():
-            print(line, end='')
+    while True:
+        print(">>> ", end="", flush=True)
+        line = next(sys.stdin)
+        if not line:
+            return
+
+        kwargs.update({"prompt": line})
+        generate_oneshot(*args, **kwargs)
+
 
-        print(flush=True)
-        kwargs.update({'prompt': line})
+def generate_batch(*args, **kwargs):
+    for line in sys.stdin:
+        print(">>> ", line, end="", flush=True)
+        kwargs.update({"prompt": line})
         generate_oneshot(*args, **kwargs)
-        print(flush=True)
-        print('>>> ', end='', flush=True)
 
 
 def add(model, models_home):
     os.rename(model, Path(models_home) / Path(model).name)
 
 
 def pull(*args, **kwargs):
     model.pull(*args, **kwargs)
+
+
+def run(*args, **kwargs):
+    name = model.pull(*args, **kwargs)
+    kwargs.update({"model": name})
+    print(f"Running {name}...")
+    generate(*args, **kwargs)
```

### Comparing `ollama-0.0.2/ollama/cmd/server.py` & `ollama-0.0.3/ollama/cmd/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from aiohttp import web
+import json
 import aiohttp_cors
+from aiohttp import web
 
 from ollama import engine
 
 
 def set_parser(parser):
     parser.add_argument("--host", default="127.0.0.1")
     parser.add_argument("--port", default=7734)
@@ -85,11 +86,12 @@
 
     kwargs = {
         "llms": request.app.get("llms"),
         "models_home": request.app.get("models_home"),
     }
 
     for output in engine.generate(model, prompt, **kwargs):
-        await response.write(output.encode("utf-8"))
+        output = json.dumps(output).encode('utf-8')
+        await response.write(output)
         await response.write(b"\n")
 
     return response
```

### Comparing `ollama-0.0.2/ollama/engine.py` & `ollama-0.0.3/ollama/engine.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,38 +18,36 @@
     os.dup2(stderr, sys.stderr.fileno())
 
 
 def generate(model, prompt, models_home=".", llms={}, *args, **kwargs):
     llm = load(model, models_home=models_home, llms=llms)
 
     prompt = ollama.prompt.template(model, prompt)
-
     if "max_tokens" not in kwargs:
         kwargs.update({"max_tokens": 16384})
 
     if "stop" not in kwargs:
         kwargs.update({"stop": ["Q:"]})
 
     if "stream" not in kwargs:
         kwargs.update({"stream": True})
 
     for output in llm(prompt, *args, **kwargs):
-        yield json.dumps(output)
+        yield output
 
 
 def load(model, models_home=".", llms={}):
     llm = llms.get(model, None)
     if not llm:
-        model_path = {
-            name: path for name, path in ollama.model.models(models_home)
-        }.get(model, None)
-
-        if not model_path:
+        stored_model_path = os.path.join(models_home, model, ".bin")
+        if os.path.exists(stored_model_path):
+            model_path = stored_model_path
+        else:
             # try loading this as a path to a model, rather than a model name
-            model_path = model
+            model_path = os.path.abspath(model)
 
         # suppress LLM's output
         with suppress_stderr():
             llm = LLM(model_path, verbose=False)
             llms.update({model: llm})
 
     return llm
```

### Comparing `ollama-0.0.2/ollama/prompt.py` & `ollama-0.0.3/ollama/prompt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from os import path
+import os
 from difflib import SequenceMatcher
 from jinja2 import Environment, PackageLoader
 
 
 def template(model, prompt):
     best_ratio = 0
     best_template = ''
 
     environment = Environment(loader=PackageLoader(__name__, 'templates'))
     for template in environment.list_templates():
-        base, _ = path.splitext(template)
-        ratio = SequenceMatcher(None, model.lower(), base).ratio()
+        base, _ = os.path.splitext(template)
+        ratio = SequenceMatcher(None, os.path.basename(model.lower()), base).ratio()
         if ratio > best_ratio:
             best_ratio = ratio
             best_template = template
 
     template = environment.get_template(best_template)
     return template.render(prompt=prompt)
```

### Comparing `ollama-0.0.2/PKG-INFO` & `ollama-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: ollama
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run ai models locally
 Author: ollama team
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: server
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0) ; extra == "server"
-Requires-Dist: aiohttp-cors (>=0.7.0,<0.8.0) ; extra == "server"
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: aiohttp-cors (>=0.7.0,<0.8.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: llama-cpp-python (>=0.1.66,<0.2.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
 Description-Content-Type: text/markdown
 
 # Ollama
 
 Run ai models locally.
 
 > _Note: this project is a work in progress. The features below are still in development_
@@ -33,29 +36,20 @@
 
 ## Install
 
 ```
 pip install ollama
 ```
 
-## Install From Source
-
-```
-git clone git@github.com:jmorganca/ollama ollama
-cd ollama
-pip install -r requirements.txt
-pip install -e .
-```
-
 ## Quickstart
 
 ```
 % ollama run huggingface.co/TheBloke/orca_mini_3B-GGML
 Pulling huggingface.co/TheBloke/orca_mini_3B-GGML...
-Downloading [================>          ] 66.67% (2/3) 30.2MB/s
+Downloading [================           ] 66.67% 11.8MiB/s
 
 ...
 ...
 ...
 
 > Hello
```

