# Comparing `tmp/symbex-0.7.tar.gz` & `tmp/symbex-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbex-0.7.tar", last modified: Fri Jun 23 03:28:43 2023, max compression
+gzip compressed data, was "symbex-1.0.tar", last modified: Thu Jun 29 18:31:56 2023, max compression
```

## Comparing `symbex-0.7.tar` & `symbex-1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 03:28:26.000000 symbex-0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-23 03:28:43.516857 symbex-0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-23 03:28:26.000000 symbex-0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 03:28:43.516857 symbex-0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-23 03:28:26.000000 symbex-0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/symbex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:26.000000 symbex-0.7/symbex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-23 03:28:26.000000 symbex-0.7/symbex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-06-23 03:28:26.000000 symbex-0.7/symbex/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-23 03:28:26.000000 symbex-0.7/symbex/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/symbex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 03:28:43.000000 symbex-0.7/symbex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 03:28:43.516857 symbex-0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_symbex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-23 03:28:26.000000 symbex-0.7/tests/test_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.649236 symbex-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-29 18:31:42.000000 symbex-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-29 18:31:56.649236 symbex-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-06-29 18:31:42.000000 symbex-1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 18:31:56.649236 symbex-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-29 18:31:42.000000 symbex-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/symbex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:42.000000 symbex-1.0/symbex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 18:31:42.000000 symbex-1.0/symbex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12476 2023-06-29 18:31:42.000000 symbex-1.0/symbex/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-06-29 18:31:42.000000 symbex-1.0/symbex/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/symbex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 18:31:56.000000 symbex-1.0/symbex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 18:31:56.645236 symbex-1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_replace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7588 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_symbex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-29 18:31:42.000000 symbex-1.0/tests/test_symbols.py
```

### Comparing `symbex-0.7/LICENSE` & `symbex-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `symbex-0.7/PKG-INFO` & `symbex-1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: symbex
-Version: 0.7
-Summary: Find the Python code for specified symbols
-Home-page: https://github.com/simonw/symbex
-Author: Simon Willison
-License: Apache License, Version 2.0
-Project-URL: Issues, https://github.com/simonw/symbex/issues
-Project-URL: CI, https://github.com/simonw/symbex/actions
-Project-URL: Changelog, https://github.com/simonw/symbex/releases
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -138,15 +123,15 @@
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
 Here's the output of the command:
-```
+```python
 # File: setup.py Line: 5
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
         return fp.read()
@@ -309,14 +294,60 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Replacing a matched symbol
+
+The `--replace` option can be used to replace a single matched symbol with content piped in to standard input.
+
+Given a file called `my_code.py` with the following content:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function():
+    # This will be replaced
+    pass
+```
+Run the following:
+```bash
+echo "def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+" | symbex second_function --replace
+```
+The result will be an updated-in-place `my_code.py` containing the following:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+```
+This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
+
+You can use this with `llm` like so:
+
+```bash
+symbex second_function -n \
+  | llm --system 'add type hints, remove docstring' \
+  | symbex second_function --replace
+```
+When I ran this the result was a `second_function` definition like this:
+```python
+def second_function(a: int, b: int) -> int:
+    return a + b + 3
+```
+
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
@@ -360,14 +391,20 @@
 
       # View signatures for all async functions with type definitions
       symbex --async --typed -s
 
       # Count the number of --async functions in the project
       symbex --async --count
 
+      # Replace my_function with a new implementation:
+      echo "def my_function(a, b):
+          # This is a replacement implementation
+          return a + b + 3
+      " | symbex my_function --replace
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -384,14 +421,15 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --replace                  Replace matching symbol with text from stdin
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.7/README.md` & `symbex-1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: symbex
+Version: 1.0
+Summary: Find the Python code for specified symbols
+Home-page: https://github.com/simonw/symbex
+Author: Simon Willison
+License: Apache License, Version 2.0
+Project-URL: Issues, https://github.com/simonw/symbex/issues
+Project-URL: CI, https://github.com/simonw/symbex/actions
+Project-URL: Changelog, https://github.com/simonw/symbex/releases
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # symbex
 
 [![PyPI](https://img.shields.io/pypi/v/symbex.svg)](https://pypi.org/project/symbex/)
 [![Changelog](https://img.shields.io/github/v/release/simonw/symbex?include_prereleases&label=changelog)](https://github.com/simonw/symbex/releases)
 [![Tests](https://github.com/simonw/symbex/workflows/Test/badge.svg)](https://github.com/simonw/symbex/actions?query=workflow%3ATest)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/simonw/symbex/blob/master/LICENSE)
 
@@ -123,15 +138,15 @@
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
 Here's the output of the command:
-```
+```python
 # File: setup.py Line: 5
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
         return fp.read()
@@ -294,14 +309,60 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Replacing a matched symbol
+
+The `--replace` option can be used to replace a single matched symbol with content piped in to standard input.
+
+Given a file called `my_code.py` with the following content:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function():
+    # This will be replaced
+    pass
+```
+Run the following:
+```bash
+echo "def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+" | symbex second_function --replace
+```
+The result will be an updated-in-place `my_code.py` containing the following:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+```
+This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
+
+You can use this with `llm` like so:
+
+```bash
+symbex second_function -n \
+  | llm --system 'add type hints, remove docstring' \
+  | symbex second_function --replace
+```
+When I ran this the result was a `second_function` definition like this:
+```python
+def second_function(a: int, b: int) -> int:
+    return a + b + 3
+```
+
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
@@ -345,14 +406,20 @@
 
       # View signatures for all async functions with type definitions
       symbex --async --typed -s
 
       # Count the number of --async functions in the project
       symbex --async --count
 
+      # Replace my_function with a new implementation:
+      echo "def my_function(a, b):
+          # This is a replacement implementation
+          return a + b + 3
+      " | symbex my_function --replace
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -369,14 +436,15 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --replace                  Replace matching symbol with text from stdin
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.7/setup.py` & `symbex-1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 import os
 
-VERSION = "0.7"
+VERSION = "1.0"
 
 
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
@@ -28,10 +28,10 @@
     version=VERSION,
     packages=["symbex"],
     entry_points="""
         [console_scripts]
         symbex=symbex.cli:cli
     """,
     install_requires=["click"],
-    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp"]},
+    extras_require={"test": ["pytest", "pytest-icdiff", "cogapp", "PyYAML"]},
     python_requires=">=3.8",
 )
```

### Comparing `symbex-0.7/symbex/cli.py` & `symbex-1.0/symbex/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import ast
 import click
 import importlib
 import inspect
 import pathlib
 import site
+import sys
 
 from .lib import (
     code_for_node,
     find_symbol_nodes,
     import_line_for_function,
     read_file,
     type_summary,
@@ -133,14 +134,19 @@
     help="Filter functions with full type annotations",
 )
 @click.option(
     "--no-init",
     is_flag=True,
     help="Filter to exclude any __init__ methods",
 )
+@click.option(
+    "--replace",
+    is_flag=True,
+    help="Replace matching symbol with text from stdin",
+)
 def cli(
     symbols,
     files,
     directories,
     stdlib,
     excludes,
     signatures,
@@ -157,14 +163,15 @@
     documented,
     undocumented,
     typed,
     untyped,
     partially_typed,
     fully_typed,
     no_init,
+    replace,
 ):
     """
     Find symbols in Python code and print the code for them.
 
     Example usage:
 
     \b
@@ -202,14 +209,21 @@
     \b
         # View signatures for all async functions with type definitions
         symbex --async --typed -s
 
     \b
         # Count the number of --async functions in the project
         symbex --async --count
+
+    \b
+        # Replace my_function with a new implementation:
+        echo "def my_function(a, b):
+            # This is a replacement implementation
+            return a + b + 3
+        " | symbex my_function --replace
     """
     if modules:
         module_dirs = []
         module_files = []
         for module in modules:
             try:
                 mod = importlib.import_module(module)
@@ -259,14 +273,19 @@
             no_init,
             modules,
         ]
     ):
         ctx = click.get_current_context()
         click.echo(ctx.get_help())
         ctx.exit()
+
+    if replace and signatures:
+        raise click.ClickException("--replace cannot be used with --signatures")
+    if replace:
+        no_file = True
     # Default to '*' if --signatures or filters are provided without symbols
     if (
         any(
             [
                 signatures,
                 async_,
                 function,
@@ -350,14 +369,15 @@
                 return False
             if fully_typed and not summary.fully:
                 return False
             return True
 
     pwd = pathlib.Path(".").resolve()
     num_matches = 0
+    replace_matches = []
     for file in iterate_files():
         try:
             code = read_file(file)
         except UnicodeDecodeError as ex:
             if not silent:
                 click.secho(f"# Unicode error in {file}: {ex}", err=True, fg="yellow")
             continue
@@ -376,14 +396,17 @@
             # If file is within pwd, print relative path
             if pwd in file.resolve().parents:
                 path = file.resolve().relative_to(pwd)
             else:
                 # else print absolute path
                 path = file.resolve()
             snippet, line_no = code_for_node(code, node, class_name, signatures, docs)
+            if replace:
+                replace_matches.append((file.resolve(), snippet, line_no))
+                continue
             if not no_file:
                 bits = ["# File:", path]
                 if class_name:
                     bits.extend(["Class:", class_name])
                 bits.extend(["Line:", line_no])
                 click.echo(" ".join(str(bit) for bit in bits))
             if imports:
@@ -397,14 +420,36 @@
                     )
                 click.echo("# " + import_line)
             click.echo(snippet)
             click.echo()
     if count:
         click.echo(num_matches)
 
+    if replace:
+        # Only works if we got a single match
+        if len(replace_matches) != 1:
+            raise click.ClickException(
+                "--replace only works with a single match, got {}".format(
+                    len(replace_matches)
+                )
+            )
+        filepath, to_replace = replace_matches[0][:2]
+        if sys.stdin.isatty():
+            raise click.ClickException(
+                "--replace only works with text piped to it on stdin"
+            )
+        new_lines = sys.stdin.readlines()
+        # Check if any lines were read
+        if len(new_lines) == 0:
+            raise click.ClickException("No input for --replace found on stdin")
+        replacement = "".join(new_lines)
+        old = filepath.read_text("utf-8")
+        new = old.replace(to_replace, replacement)
+        filepath.write_text(new, "utf-8")
+
 
 def is_subpath(path: pathlib.Path, parent: pathlib.Path) -> bool:
     try:
         path.relative_to(parent)
         return True
     except ValueError:
         return False
```

### Comparing `symbex-0.7/symbex/lib.py` & `symbex-1.0/symbex/lib.py`

 * *Files identical despite different names*

### Comparing `symbex-0.7/symbex.egg-info/PKG-INFO` & `symbex-1.0/symbex.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbex
-Version: 0.7
+Version: 1.0
 Summary: Find the Python code for specified symbols
 Home-page: https://github.com/simonw/symbex
 Author: Simon Willison
 License: Apache License, Version 2.0
 Project-URL: Issues, https://github.com/simonw/symbex/issues
 Project-URL: CI, https://github.com/simonw/symbex/actions
 Project-URL: Changelog, https://github.com/simonw/symbex/releases
@@ -138,15 +138,15 @@
 
 In a fresh checkout of [Datasette](https://github.com/simonw/datasette) I ran this command:
 
 ```bash
 symbex MessagesDebugView get_long_description
 ```
 Here's the output of the command:
-```
+```python
 # File: setup.py Line: 5
 def get_long_description():
     with open(
         os.path.join(os.path.dirname(os.path.abspath(__file__)), "README.md"),
         encoding="utf8",
     ) as fp:
         return fp.read()
@@ -309,14 +309,60 @@
 ```bash
 symbex Response | llm --system 'Explain this code, succinctly'
 ```
 And got back this:
 
 > This code defines a custom `Response` class with methods for returning HTTP responses. It includes methods for setting cookies, returning HTML, text, and JSON responses, and redirecting to a different URL. The `asgi_send` method sends the response to the client using the ASGI (Asynchronous Server Gateway Interface) protocol.
 
+## Replacing a matched symbol
+
+The `--replace` option can be used to replace a single matched symbol with content piped in to standard input.
+
+Given a file called `my_code.py` with the following content:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function():
+    # This will be replaced
+    pass
+```
+Run the following:
+```bash
+echo "def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+" | symbex second_function --replace
+```
+The result will be an updated-in-place `my_code.py` containing the following:
+```python
+def first_function():
+    # This will be ignored
+    pass
+
+def second_function(a, b):
+    # This is a replacement implementation
+    return a + b + 3
+```
+This feature should be used with care! I recommend only using this feature against code that is already checked into Git, so you can review changes it makes using `git diff` and revert them using `git checkout my_code.py`.
+
+You can use this with `llm` like so:
+
+```bash
+symbex second_function -n \
+  | llm --system 'add type hints, remove docstring' \
+  | symbex second_function --replace
+```
+When I ran this the result was a `second_function` definition like this:
+```python
+def second_function(a: int, b: int) -> int:
+    return a + b + 3
+```
+
 ## Similar tools
 
 - [pyastgrep](https://github.com/spookylukey/pyastgrep) by Luke Plant offers advanced capabilities for viewing and searching through Python ASTs using XPath.
 - [cq](https://github.com/fullstackio/cq) is a tool thet lets you "extract code snippets using CSS-like selectors", built using [Tree-sitter](https://tree-sitter.github.io/tree-sitter/) and primarily targetting JavaScript and TypeScript.
 
 ## symbex --help
 
@@ -360,14 +406,20 @@
 
       # View signatures for all async functions with type definitions
       symbex --async --typed -s
 
       # Count the number of --async functions in the project
       symbex --async --count
 
+      # Replace my_function with a new implementation:
+      echo "def my_function(a, b):
+          # This is a replacement implementation
+          return a + b + 3
+      " | symbex my_function --replace
+
 Options:
   --version                  Show the version and exit.
   -f, --file FILE            Files to search
   -d, --directory DIRECTORY  Directories to search
   --stdlib                   Search the Python standard library
   -x, --exclude DIRECTORY    Directories to exclude
   -s, --signatures           Show just function and class signatures
@@ -384,14 +436,15 @@
   --documented               Filter functions with docstrings
   --undocumented             Filter functions without docstrings
   --typed                    Filter functions with type annotations
   --untyped                  Filter functions without type annotations
   --partially-typed          Filter functions with partial type annotations
   --fully-typed              Filter functions with full type annotations
   --no-init                  Filter to exclude any __init__ methods
+  --replace                  Replace matching symbol with text from stdin
   --help                     Show this message and exit.
 
 ```
 <!-- [[[end]]] -->
 
 ## Development
```

### Comparing `symbex-0.7/tests/test_filters.py` & `symbex-1.0/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `symbex-0.7/tests/test_imports.py` & `symbex-1.0/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `symbex-0.7/tests/test_symbex.py` & `symbex-1.0/tests/test_symbex.py`

 * *Files identical despite different names*

### Comparing `symbex-0.7/tests/test_symbols.py` & `symbex-1.0/tests/test_symbols.py`

 * *Files identical despite different names*

