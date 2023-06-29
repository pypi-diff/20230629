# Comparing `tmp/edwh_bundler_plugin-0.1.6.tar.gz` & `tmp/edwh_bundler_plugin-0.1.7.tar.gz`

## Comparing `edwh_bundler_plugin-0.1.6.tar` & `edwh_bundler_plugin-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/CHANGELOG.md
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/__about__.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/__init__.py
--rw-r--r--   0        0        0    20248 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/bundler_plugin.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/css.py
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/js.py
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/shared.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/.gitignore
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/README.md
--rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/CHANGELOG.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/bundle.yaml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/__about__.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/__init__.py
+-rw-r--r--   0        0        0    20717 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/bundler_plugin.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/css.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/js.py
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/shared.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/README.md
+-rw-r--r--   0        0        0     4087 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 edwh_bundler_plugin-0.1.7/PKG-INFO
```

### Comparing `edwh_bundler_plugin-0.1.6/CHANGELOG.md` & `edwh_bundler_plugin-0.1.7/CHANGELOG.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.1.7 (2023-06-29)
+### Fix
+* Don't crash if the output folder doesn't exist yet ([`630342d`](https://github.com/educationwarehouse/edwh-bundler-plugin/commit/630342dd149a0120cd003c6c09d7f1238797d3a5))
+
 ## v0.1.6 (2023-05-31)
 
 
 ## v0.1.5 (2023-04-17)
 
 
 ## v0.1.4 (2023-04-17)
```

### Comparing `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/bundler_plugin.py` & `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/bundler_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 
 import io
 import os
 import re
 import sqlite3
 import sys
 import typing
+import warnings
 from contextlib import contextmanager
+from dataclasses import dataclass
 from datetime import datetime
+from pathlib import Path
 
 import invoke
 import yaml
 from invoke import task, Context
 from dotenv import load_dotenv
 from shutil import rmtree
 
@@ -55,18 +58,23 @@
     Open a temp buffer file in append mode and first remove old version if that exists
     """
     if isinstance(temp, io.IOBase):
         # already writable like io.StringIO or sys.stdout
         yield temp
         return
 
-    if os.path.exists(temp):
-        os.remove(temp)
+    path = Path(temp)
 
-    f = open(temp, "a")
+    if path.exists():
+        path.unlink()
+
+    # ensure the path to the file exists:
+    path.parent.mkdir(parents=True, exist_ok=True)
+
+    f = path.open("a")
     try:
         yield f
     finally:
         f.close()
 
 
 def cli_or_config(
@@ -212,15 +220,15 @@
     Build the JS bundle (cli only)
     """
     config = load_config(input)
 
     files = files or config.get("js")
 
     if not files:
-        raise ValueError("Please specify either --files or the js key in a config yaml (e.g. bundle.yaml)")
+        raise NotFound("js")
 
     settings = config.get("config", {})
 
     minify = cli_or_config(minify, settings, "minify")
     cache = cli_or_config(cache, settings, "cache", default=True)
     output = sys.stdout if stdout else cli_or_config(output, settings, "output_js", bool=False) or DEFAULT_OUTPUT_JS
 
@@ -275,14 +283,22 @@
     if not isinstance(output, io.StringIO):
         return output
 
     output.seek(0)
     return output.read()
 
 
+@dataclass
+class NotFound(Exception):
+    type: typing.Literal["js", "css"]
+
+    def __str__(self):
+        return f"Please specify either --files or the {self.type} key in a config yaml (e.g. bundle.yaml)"
+
+
 @task(iterable=["files"])
 def build_css(
     c,
     files=None,
     input=DEFAULT_INPUT,
     verbose=False,
     # overrule config:
@@ -302,15 +318,15 @@
     cache = cli_or_config(cache, settings, "cache", default=True)
 
     settings["version"] = cli_or_config(version, settings, "version", bool=False, default="latest")
 
     output = sys.stdout if stdout else cli_or_config(output, settings, "output_css", bool=False) or DEFAULT_OUTPUT_CSS
 
     if not (files := (files or config.get("css"))):
-        raise ValueError("Please specify either --files or the css key in a config yaml (e.g. bundle.yaml)")
+        raise NotFound("css")
 
     return _handle_files(
         files,
         extract_contents_for_css,
         output,
         verbose=verbose,
         cache=cache,
@@ -377,18 +393,29 @@
     Build the JS and CSS bundle
     """
     # invoke build
 
     # second argument of build_ is None, so files will be loaded from config.
     # --files can be supplied for the build-js or build-css methods, but not for normal build
     # since it would be too ambiguous to determine whether the files should be compiled as JS or CSS.
-    return (
-        build_js(c, None, input, verbose, output_js, minify, cache, version),
-        build_css(c, None, input, verbose, output_css, minify, cache, version),
-    )
+    result = []
+    try:
+        result.append(build_js(c, None, input, verbose, output_js, minify, cache, version))
+    except NotFound as e:
+        warnings.warn(str(e), source=e)
+
+    try:
+        result.append(
+            build_css(c, None, input, verbose, output_css, minify, cache, version),
+        )
+    except NotFound as e:
+        warnings.warn(str(e), source=e)
+
+    print(result)
+    return result
 
 
 def XOR(first, *extra):
     result = bool(first)
     for item in extra:
         result ^= bool(item)
```

### Comparing `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/css.py` & `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/css.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/js.py` & `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/js.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/src/edwh_bundler_plugin/shared.py` & `edwh_bundler_plugin-0.1.7/src/edwh_bundler_plugin/shared.py`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/LICENSE.txt` & `edwh_bundler_plugin-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/README.md` & `edwh_bundler_plugin-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/pyproject.toml` & `edwh_bundler_plugin-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edwh_bundler_plugin-0.1.6/PKG-INFO` & `edwh_bundler_plugin-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edwh-bundler-plugin
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python-only static file (js, css) bundler for `edwh`
 Project-URL: Documentation, https://github.com/educationwarehouse/edwh-bundler-plugin#readme
 Project-URL: Issues, https://github.com/educationwarehouse/edwh-bundler-plugin/issues
 Project-URL: Source, https://github.com/educationwarehouse/edwh-bundler-plugin
 Author-email: Robin van der Noord <robin.vdn@educationwarehouse.nl>, Remco Boerma <remco.b@educationwarehouse.nl>
 License-Expression: MIT
 License-File: LICENSE.txt
```

