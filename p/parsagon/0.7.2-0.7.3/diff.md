# Comparing `tmp/parsagon-0.7.2.tar.gz` & `tmp/parsagon-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsagon-0.7.2.tar", last modified: Tue Jun 27 10:13:26 2023, max compression
+gzip compressed data, was "parsagon-0.7.3.tar", last modified: Thu Jun 29 19:42:29 2023, max compression
```

## Comparing `parsagon-0.7.2.tar` & `parsagon-0.7.3.tar`

### file list

```diff
@@ -1,23 +1,28 @@
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.074568 parsagon-0.7.2/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-27 10:13:26.074024 parsagon-0.7.2/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.2/README.md
--rw-r--r--   0 amsuh    (10002)    18010      935 2023-06-27 10:04:55.000000 parsagon-0.7.2/pyproject.toml
--rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-27 10:13:26.074711 parsagon-0.7.2/setup.cfg
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.063509 parsagon-0.7.2/src/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.2/src/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.068215 parsagon-0.7.2/src/parsagon/
--rw-r--r--   0 amsuh    (10002)    18010       46 2023-06-26 21:26:23.000000 parsagon-0.7.2/src/parsagon/__init__.py
--rw-r--r--   0 amsuh    (10002)    18010     3678 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/api.py
--rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.2/src/parsagon/custom_function.py
--rw-r--r--   0 amsuh    (10002)    18010    10517 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/executor.py
--rw-r--r--   0 amsuh    (10002)    18010     7100 2023-06-27 10:04:55.000000 parsagon-0.7.2/src/parsagon/main.py
--rw-r--r--   0 amsuh    (10002)    18010     1085 2023-06-18 04:18:36.000000 parsagon-0.7.2/src/parsagon/settings.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.073542 parsagon-0.7.2/src/parsagon/tests/
--rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.2/src/parsagon/tests/__init__.py
-drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-27 10:13:26.072877 parsagon-0.7.2/src/parsagon.egg-info/
--rw-r--r--   0 amsuh    (10002)    18010     1424 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/PKG-INFO
--rw-r--r--   0 amsuh    (10002)    18010      437 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/SOURCES.txt
--rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/dependency_links.txt
--rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/entry_points.txt
--rw-r--r--   0 amsuh    (10002)    18010      209 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/requires.txt
--rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-27 10:13:26.000000 parsagon-0.7.2/src/parsagon.egg-info/top_level.txt
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.775278 parsagon-0.7.3/
+-rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-29 19:42:29.774702 parsagon-0.7.3/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010     1054 2023-06-20 20:10:33.000000 parsagon-0.7.3/README.md
+-rw-r--r--   0 amsuh    (10002)    18010     1026 2023-06-29 19:41:23.000000 parsagon-0.7.3/pyproject.toml
+-rw-r--r--   0 amsuh    (10002)    18010       38 2023-06-29 19:42:29.775469 parsagon-0.7.3/setup.cfg
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.759590 parsagon-0.7.3/src/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.3/src/__init__.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.766466 parsagon-0.7.3/src/parsagon/
+-rw-r--r--   0 amsuh    (10002)    18010       54 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     4355 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/api.py
+-rw-r--r--   0 amsuh    (10002)    18010      770 2023-06-19 04:58:01.000000 parsagon-0.7.3/src/parsagon/custom_function.py
+-rw-r--r--   0 amsuh    (10002)    18010      879 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/exceptions.py
+-rw-r--r--   0 amsuh    (10002)    18010    10517 2023-06-27 10:04:55.000000 parsagon-0.7.3/src/parsagon/executor.py
+-rw-r--r--   0 amsuh    (10002)    18010     6885 2023-06-29 19:39:03.000000 parsagon-0.7.3/src/parsagon/main.py
+-rw-r--r--   0 amsuh    (10002)    18010     1570 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/settings.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.773783 parsagon-0.7.3/src/parsagon/tests/
+-rw-r--r--   0 amsuh    (10002)    18010        0 2023-06-07 21:22:25.000000 parsagon-0.7.3/src/parsagon/tests/__init__.py
+-rw-r--r--   0 amsuh    (10002)    18010     3127 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/api_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      327 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/cli_mocks.py
+-rw-r--r--   0 amsuh    (10002)    18010      428 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/conftest.py
+-rw-r--r--   0 amsuh    (10002)    18010     1089 2023-06-29 05:25:58.000000 parsagon-0.7.3/src/parsagon/tests/test_pipeline_operations.py
+drwxr-xr-x   0 amsuh    (10002)    18010        0 2023-06-29 19:42:29.769867 parsagon-0.7.3/src/parsagon.egg-info/
+-rw-r--r--   0 amsuh    (10002)    18010     1444 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/PKG-INFO
+-rw-r--r--   0 amsuh    (10002)    18010      606 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/SOURCES.txt
+-rw-r--r--   0 amsuh    (10002)    18010        1 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/dependency_links.txt
+-rw-r--r--   0 amsuh    (10002)    18010       48 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/entry_points.txt
+-rw-r--r--   0 amsuh    (10002)    18010      250 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/requires.txt
+-rw-r--r--   0 amsuh    (10002)    18010       18 2023-06-29 19:42:29.000000 parsagon-0.7.3/src/parsagon.egg-info/top_level.txt
```

### Comparing `parsagon-0.7.2/PKG-INFO` & `parsagon-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # parsagon
 
 Parsagon allows you to create browser automations with natural language. You can create automations that fill out forms, scrape web pages, and much more, all without writing code. Here's a brief overview of how to get started:
 
 ## Requirements
```

### Comparing `parsagon-0.7.2/README.md` & `parsagon-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.2/pyproject.toml` & `parsagon-0.7.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.black]
 line-length = 120
 
 [project]
 name = "parsagon"
-version = "0.7.2"
+version = "0.7.3"
 description = "Allows you to create browser automations with natural language"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
   { name="Sandy Suh", email="sandy@parsagon.io" },
 ]
 classifiers = [
@@ -34,12 +34,18 @@
     'cssselect==1.1.0',
     'undetected-chromedriver==3.1.5.post4',
     'jsonpath-ng==1.5.3',
     'usaddress==0.5.10',
     'simplejson==3.19.1',
 ]
 
+[project.optional-dependencies]
+dev = [
+    "pytest==7.3.2",
+    "pytest-mock==3.11.1",
+]
+
 [project.urls]
 "Homepage" = "https://parsagon.io"
 
 [project.scripts]
 parsagon = "parsagon.main:main"
```

### Comparing `parsagon-0.7.2/src/parsagon/api.py` & `parsagon-0.7.3/src/parsagon/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,52 @@
+import contextlib
 import json
 from json import JSONDecodeError
 
 import httpx
 
 from parsagon import settings
+from parsagon.exceptions import ParsagonException, APIException, ProgramNotFoundException
 
 environment = "PANDAS_1.x"
 
 
-class APIException(Exception):
-    @property
-    def value(self):
-        return self.args[0]
+class RaiseProgramNotFound:
+    def __init__(self, program_name):
+        self.program_name = program_name
+
+    def __enter__(self):
+        pass
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        if exc_type is not None and issubclass(exc_type, APIException):
+            if exc_value.status_code == 404:
+                raise ProgramNotFoundException(self.program_name)
+        return False
 
 
 def _request_to_exception(response):
-    if response.status_code == 500:
-        raise APIException("A server error occurred. Please notify Parsagon.")
-    if response.status_code in (502, 503, 504):
-        raise APIException("Lost connection to server.")
+    status_code = response.status_code
+    if status_code == 500:
+        raise APIException("A server error occurred. Please notify Parsagon.", status_code)
+    if status_code in (502, 503, 504):
+        raise APIException("Lost connection to server.", status_code)
     try:
         errors = response.json()
         if "non_field_errors" in errors:
-            raise APIException(errors["non_field_errors"])
+            raise APIException(errors["non_field_errors"], status_code)
         else:
-            raise APIException(errors)
+            raise APIException(errors, status_code)
     except JSONDecodeError:
-        raise APIException("Could not parse response.")
+        raise APIException("Could not parse response.", status_code)
 
 
 def _api_call(httpx_func, endpoint, **kwargs):
-    api_key = settings.API_KEY
-    api_endpoint = f"{settings.API_BASE}/api{endpoint}"
+    api_key = settings.get_api_key()
+    api_endpoint = f"{settings.get_api_base()}/api{endpoint}"
     headers = {"Authorization": f"Token {api_key}"}
     r = httpx_func(api_endpoint, headers=headers, timeout=None, **kwargs)
     if not r.is_success:
         _request_to_exception(r)
     else:
         try:
             return r.json()
@@ -76,15 +87,17 @@
     :param schema: Schema of the data to scrape, in the format
     :return: Scraped data, with lists truncated.
     """
     return _api_call(httpx.post, "/transformers/get-custom-data/", json={"html": html, "schema": schema})
 
 
 def create_pipeline(name, description, program_sketch):
-    return _api_call(httpx.post, "/pipelines/", json={"name": name, "description": description, "program_sketch": program_sketch})
+    return _api_call(
+        httpx.post, "/pipelines/", json={"name": name, "description": description, "program_sketch": program_sketch}
+    )
 
 
 def delete_pipeline(pipeline_id):
     return _api_call(httpx.delete, f"/pipelines/{pipeline_id}/")
 
 
 def create_custom_function(pipeline_id, call_id, custom_function):
@@ -92,27 +105,29 @@
         httpx.post,
         "/transformers/custom-function/",
         json={"pipeline": pipeline_id, "call_id": call_id, **custom_function.to_json()},
     )
 
 
 def get_pipeline(pipeline_name):
-    return _api_call(
-        httpx.get,
-        f"/pipelines/name/{pipeline_name}/",
-    )
+    with RaiseProgramNotFound(pipeline_name):
+        return _api_call(
+            httpx.get,
+            f"/pipelines/name/{pipeline_name}/",
+        )
 
 
 def get_pipelines():
     return _api_call(httpx.get, f"/pipelines/")
 
 
 def get_pipeline_code(pipeline_name, variables, environment, headless):
-    return _api_call(
-        httpx.post,
-        f"/pipelines/name/{pipeline_name}/code/",
-        json={
-            "variables": variables,
-            "environment": environment,
-            "headless": headless,
-        },
-    )
+    with RaiseProgramNotFound(pipeline_name):
+        return _api_call(
+            httpx.post,
+            f"/pipelines/name/{pipeline_name}/code/",
+            json={
+                "variables": variables,
+                "environment": environment,
+                "headless": headless,
+            },
+        )
```

### Comparing `parsagon-0.7.2/src/parsagon/custom_function.py` & `parsagon-0.7.3/src/parsagon/custom_function.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.2/src/parsagon/executor.py` & `parsagon-0.7.3/src/parsagon/executor.py`

 * *Files identical despite different names*

### Comparing `parsagon-0.7.2/src/parsagon/main.py` & `parsagon-0.7.3/src/parsagon/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,44 +10,44 @@
     delete_pipeline,
     create_custom_function,
     get_pipeline,
     get_pipelines,
     get_pipeline_code,
     APIException,
 )
+from parsagon.exceptions import ParsagonException
 from parsagon.executor import Executor, custom_functions_to_descriptions
 
 logger = logging.getLogger(__name__)
 
 
 def configure_logging(verbose):
     logging.config.dictConfig(settings.get_logging_config("DEBUG" if verbose else "INFO"))
 
 
-def main():
+def get_args():
     parser = argparse.ArgumentParser(
         prog="parsagon", description="Scrapes and interacts with web pages based on natural language.", add_help=False
     )
     parser.add_argument("-v", "--verbose", action="store_true", help="run the task in verbose mode")
     subparsers = parser.add_subparsers()
 
     # Create
     parser_create = subparsers.add_parser("create", description="Creates a program.")
     parser_create.add_argument(
-        "task",
-        metavar="task",
+        "--task",
+        dest="task",
         type=str,
-        help="natural language description of the task to run, optionally with numbered steps.",
+        help="natural language description of the task to run",
     )
     parser_create.add_argument(
-        "-p",
         "--program",
         dest="program_name",
         type=str,
-        help="the name of the program to create (otherwise user input is required)",
+        help="the name of the program to create",
     )
     parser_create.add_argument(
         "--headless",
         action="store_true",
         help="run the browser in headless mode",
     )
     parser_create.set_defaults(func=create)
@@ -96,29 +96,40 @@
     )
     parser_delete.add_argument(
         "program_name",
         type=str,
         help="the name of the program to run",
     )
     parser_delete.set_defaults(func=delete)
-
     args = parser.parse_args()
     kwargs = vars(args)
+    return kwargs, parser
+
+
+def main():
+    kwargs, parser = get_args()
     func = kwargs.pop("func")
     verbose = kwargs["verbose"]
     configure_logging(verbose)
 
     if func:
-        return func(**kwargs)
+        try:
+            return func(**kwargs)
+        except ParsagonException as e:
+            error_message = "Error:\n" + e.to_string(verbose)
+            logger.error(error_message)
     else:
         parser.print_help()
 
 
-def create(task, program_name=None, headless=False, verbose=False):
-    logger.info("Launched with task description:\n%s", task)
+def create(task=None, program_name=None, headless=False, verbose=False):
+    if task:
+        logger.info("Launched with task description:\n%s", task)
+    else:
+        task = input("Type what you want to do: ")
 
     logger.info("Analyzing task description...")
     program_sketches = get_program_sketches(task)
 
     full_program = program_sketches["full"]
     abridged_program = program_sketches["abridged"]
     logger.debug("Program:\n%s", abridged_program)
@@ -178,42 +189,28 @@
 
 
 def run(program_name, variables={}, environment="LOCAL", headless=False, verbose=False):
     """
     Executes pipeline code
     """
     logger.info("Preparing to run program %s", program_name)
-    try:
-        code = get_pipeline_code(program_name, variables, environment, headless)["code"]
-    except APIException as e:
-        if isinstance(e.value, dict) and e.value.get("detail") == "Not found.":
-            logger.error("Error: A program with this name does not exist.")
-            return
-        else:
-            raise e
+    code = get_pipeline_code(program_name, variables, environment, headless)["code"]
 
     logger.info("Running program...")
-    globals_locals = {"PARSAGON_API_KEY": settings.API_KEY}
+    globals_locals = {"PARSAGON_API_KEY": settings.get_api_key()}
     try:
         exec(code, globals_locals, globals_locals)
     finally:
         if "driver" in globals_locals:
             globals_locals["driver"].quit()
         if "display" in globals_locals:
             globals_locals["display"].stop()
     logger.info("Done.")
     return globals_locals["output"]
 
 
 def delete(program_name, verbose=False):
     logger.info("Preparing to delete program %s", program_name)
-    try:
-        pipeline_id = get_pipeline(program_name)["id"]
-    except APIException as e:
-        if isinstance(e.value, dict) and e.value.get("detail") == "Not found.":
-            logger.error("Error: A program with this name does not exist.")
-            return
-        else:
-            raise e
+    pipeline_id = get_pipeline(program_name)["id"]
     logger.info("Deleting program...")
     delete_pipeline(pipeline_id)
     logger.info("Done.")
```

### Comparing `parsagon-0.7.2/src/parsagon.egg-info/PKG-INFO` & `parsagon-0.7.3/src/parsagon.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: parsagon
-Version: 0.7.2
+Version: 0.7.3
 Summary: Allows you to create browser automations with natural language
 Author-email: Sandy Suh <sandy@parsagon.io>
 Project-URL: Homepage, https://parsagon.io
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 
 # parsagon
 
 Parsagon allows you to create browser automations with natural language. You can create automations that fill out forms, scrape web pages, and much more, all without writing code. Here's a brief overview of how to get started:
 
 ## Requirements
```

