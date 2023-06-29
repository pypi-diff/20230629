# Comparing `tmp/pytest-mypy-plugins-1.9.3.tar.gz` & `tmp/pytest-mypy-plugins-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mypy-plugins-1.9.3.tar", last modified: Tue Jan 11 12:44:07 2022, max compression
+gzip compressed data, was "pytest-mypy-plugins-2.0.0.tar", last modified: Thu Jun 29 07:14:44 2023, max compression
```

## Comparing `pytest-mypy-plugins-1.9.3.tar` & `pytest-mypy-plugins-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,34 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.602709 pytest-mypy-plugins-1.9.3/
--rw-r--r--   0 sobolev    (501) staff       (20)     1054 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.3/LICENSE
--rw-r--r--   0 sobolev    (501) staff       (20)     8228 2022-01-11 12:44:07.602046 pytest-mypy-plugins-1.9.3/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)     7489 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.3/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)      115 2021-12-25 08:11:40.000000 pytest-mypy-plugins-1.9.3/pyproject.toml
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.595543 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)     7182 2021-12-25 08:11:40.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/collect.py
--rw-r--r--   0 sobolev    (501) staff       (20)    14746 2022-01-11 12:36:28.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/item.py
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/py.typed
--rw-r--r--   0 sobolev    (501) staff       (20)    12431 2021-10-19 09:40:34.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/utils.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.601156 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)     8228 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      450 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       62 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/entry_points.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       96 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       20 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       38 2022-01-11 12:44:07.602907 pytest-mypy-plugins-1.9.3/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)     1319 2022-01-11 12:37:14.000000 pytest-mypy-plugins-1.9.3/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.534921 pytest-mypy-plugins-2.0.0/
+-rw-r--r--   0 sobolev    (501) staff       (20)     1054 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/LICENSE
+-rw-r--r--   0 sobolev    (501) staff       (20)       68 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/MANIFEST.in
+-rw-r--r--   0 sobolev    (501) staff       (20)     8316 2023-06-29 07:14:44.534748 pytest-mypy-plugins-2.0.0/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)     7535 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      313 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/mypy.ini
+-rw-r--r--   0 sobolev    (501) staff       (20)      115 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pyproject.toml
+-rw-r--r--   0 sobolev    (501) staff       (20)      125 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest.ini
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.532066 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     7257 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/collect.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    14684 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/item.py
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/py.typed
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.533996 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.534409 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/
+-rw-r--r--   0 sobolev    (501) staff       (20)      824 2023-06-29 07:07:03.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/reveal_type_hook.cpython-311.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)    11558 2023-06-29 07:07:03.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/__pycache__/test_utils.cpython-311-pytest-7.4.0.pyc
+-rw-r--r--   0 sobolev    (501) staff       (20)      354 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/reveal_type_hook.py
+-rw-r--r--   0 sobolev    (501) staff       (20)      183 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-extension.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1242 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-parametrized.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)      338 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-paths-from-env.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1179 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-regex_assertions.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     1987 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test-simple-cases.yml
+-rw-r--r--   0 sobolev    (501) staff       (20)     8631 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/tests/test_utils.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    12670 2023-06-29 06:58:38.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/utils.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2023-06-29 07:14:44.532972 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)     8316 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      960 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       61 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       64 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       20 2023-06-29 07:14:44.000000 pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2023-06-29 07:14:44.534968 pytest-mypy-plugins-2.0.0/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)     1365 2023-06-29 07:14:33.000000 pytest-mypy-plugins-2.0.0/setup.py
```

### Comparing `pytest-mypy-plugins-1.9.3/LICENSE` & `pytest-mypy-plugins-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-1.9.3/PKG-INFO` & `pytest-mypy-plugins-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 1.9.3
+Version: 2.0.0
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
+Maintainer: Nikita Sobolev
+Maintainer-email: mail@sobolevn.me
 License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
 
 # pytest plugin for testing mypy types, stubs, and plugins
 
@@ -70,15 +71,15 @@
 - case: mypy_path_from_env
   main: |
     from pair import Pair
 
     instance: Pair
     reveal_type(instance)  # N: Revealed type is 'pair.Pair'
   env:
-    - MYPYPATH=./pytest_mypy_plugins/tests/fixtures
+    - MYPYPATH=../fixtures
 ```
 
 
 ### What is a test case?
 
 In general each test case is just an element in an array written in a properly formatted `YAML` file.
 On top of that, each case must comply to following types:
@@ -142,17 +143,22 @@
 - case: with_params
   parametrized:
     - val: 1
       rt: builtins.int
     - val: 1.0
       rt: builtins.float
   main: |
-    reveal_type({[ val }})  # N: Revealed type is '{{ rt }}'
+    reveal_type({{ val }})  # N: Revealed type is '{{ rt }}'
 ```
 
+Properties that you can parametrize:
+- `main`
+- `mypy_config`
+- `out`
+
 #### 3. Longer type expectations
 
 ```yaml
 - case: with_out
   main: |
     reveal_type('abc')
   out: |
@@ -199,9 +205,7 @@
 ## Further reading
 
 - [Testing mypy stubs, plugins, and types](https://sobolevn.me/2019/08/testing-mypy-types)
 
 ## License
 
 [MIT](https://github.com/typeddjango/pytest-mypy-plugins/blob/master/LICENSE)
-
-
```

### Comparing `pytest-mypy-plugins-1.9.3/README.md` & `pytest-mypy-plugins-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 - case: mypy_path_from_env
   main: |
     from pair import Pair
 
     instance: Pair
     reveal_type(instance)  # N: Revealed type is 'pair.Pair'
   env:
-    - MYPYPATH=./pytest_mypy_plugins/tests/fixtures
+    - MYPYPATH=../fixtures
 ```
 
 
 ### What is a test case?
 
 In general each test case is just an element in an array written in a properly formatted `YAML` file.
 On top of that, each case must comply to following types:
@@ -121,17 +121,22 @@
 - case: with_params
   parametrized:
     - val: 1
       rt: builtins.int
     - val: 1.0
       rt: builtins.float
   main: |
-    reveal_type({[ val }})  # N: Revealed type is '{{ rt }}'
+    reveal_type({{ val }})  # N: Revealed type is '{{ rt }}'
 ```
 
+Properties that you can parametrize:
+- `main`
+- `mypy_config`
+- `out`
+
 #### 3. Longer type expectations
 
 ```yaml
 - case: with_out
   main: |
     reveal_type('abc')
   out: |
```

### Comparing `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/collect.py` & `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import os
 import pathlib
 import platform
 import sys
 import tempfile
-from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Mapping, Optional, Set
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Hashable,
+    Iterator,
+    List,
+    Mapping,
+    Optional,
+    Set,
+)
 
-import pkg_resources
+import py.path
 import pytest
 import yaml
 from _pytest.config.argparsing import Parser
 from _pytest.nodes import Node
-from py._path.local import LocalPath
+from packaging.version import Version
 
 from pytest_mypy_plugins import utils
 
 if TYPE_CHECKING:
     from pytest_mypy_plugins.item import YamlTestItem
 
 
@@ -59,19 +69,19 @@
             )
         parsed_params.append({k: v for k, v in param.items() if not k.startswith("__")})
 
     return parsed_params
 
 
 class SafeLineLoader(yaml.SafeLoader):
-    def construct_mapping(self, node: yaml.Node, deep: bool = False) -> None:
+    def construct_mapping(self, node: yaml.MappingNode, deep: bool = False) -> Dict[Hashable, Any]:
         mapping = super().construct_mapping(node, deep=deep)
         # Add 1 so line numbering starts at 1
         starting_line = node.start_mark.line + 1
-        for (title_node, contents_node) in node.value:
+        for title_node, contents_node in node.value:
             if title_node.value == "main":
                 starting_line = title_node.start_mark.line + 1
         mapping["__line__"] = starting_line
         return mapping
 
 
 class YamlTestFile(pytest.File):
@@ -117,15 +127,15 @@
 
                 starting_lineno = raw_test["__line__"]
                 extra_environment_variables = parse_environment_variables(raw_test.get("env", []))
                 disable_cache = raw_test.get("disable_cache", False)
                 expected_output.extend(
                     utils.extract_output_matchers_from_out(raw_test.get("out", ""), params, regex=regex)
                 )
-                additional_mypy_config = raw_test.get("mypy_config", "")
+                additional_mypy_config = utils.render_template(template=raw_test.get("mypy_config", ""), data=params)
 
                 skip = self._eval_skip(str(raw_test.get("skip", "False")))
                 if not skip:
                     yield YamlTestItem.from_parent(
                         self,
                         name=test_name,
                         files=test_files,
@@ -138,24 +148,24 @@
                         expect_fail=expect_fail,
                     )
 
     def _eval_skip(self, skip_if: str) -> bool:
         return eval(skip_if, {"sys": sys, "os": os, "pytest": pytest, "platform": platform})
 
 
-if pkg_resources.parse_version(pytest.__version__) >= pkg_resources.parse_version("7.0.0rc1"):
+if Version(pytest.__version__) >= Version("7.0.0rc1"):
 
     def pytest_collect_file(file_path: pathlib.Path, parent: Node) -> Optional[YamlTestFile]:
         if file_path.suffix in {".yaml", ".yml"} and file_path.name.startswith(("test-", "test_")):
             return YamlTestFile.from_parent(parent, path=file_path, fspath=None)
         return None
 
 else:
 
-    def pytest_collect_file(path: LocalPath, parent: Node) -> Optional[YamlTestFile]:  # type: ignore[misc]
+    def pytest_collect_file(path: py.path.local, parent: Node) -> Optional[YamlTestFile]:  # type: ignore[misc]
         if path.ext in {".yaml", ".yml"} and path.basename.startswith(("test-", "test_")):
             return YamlTestFile.from_parent(parent, fspath=path)
         return None
 
 
 def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("mypy-tests")
```

### Comparing `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/item.py` & `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
 class ReturnCodes:
     SUCCESS = 0
     FAIL = 1
     FATAL_ERROR = 2
 
 
-def run_mypy_typechecking(cmd_options: List[str]) -> int:
+def run_mypy_typechecking(cmd_options: List[str]) -> Optional[Union[str, int]]:
     fscache = FileSystemCache()
     sources, options = process_options(cmd_options, fscache=fscache)
 
     error_messages = []
 
     def flush_errors(new_messages: List[str], serious: bool) -> None:
         error_messages.extend(new_messages)
@@ -211,15 +211,15 @@
         )
         captured_stdout = completed.stdout.decode()
         captured_stderr = completed.stderr.decode()
         return completed.returncode, (captured_stdout, captured_stderr)
 
     def typecheck_in_same_process(
         self, execution_path: Path, mypy_cmd_options: List[Any]
-    ) -> Tuple[int, Tuple[str, str]]:
+    ) -> Tuple[Optional[Union[str, int]], Tuple[str, str]]:
         with utils.temp_environ(), utils.temp_path(), utils.temp_sys_modules():
             # add custom environment variables
             for key, val in self.environment_variables.items():
                 os.environ[key] = val
 
             # add current directory to path
             sys.path.insert(0, str(execution_path))
@@ -237,15 +237,14 @@
         extension_hook(self)
 
     def runtest(self) -> None:
         try:
             temp_dir = tempfile.TemporaryDirectory(prefix="pytest-mypy-", dir=self.root_directory)
 
         except (FileNotFoundError, PermissionError, NotADirectoryError) as e:
-
             raise TypecheckAssertionError(
                 error_message=f"Testing base directory {self.root_directory} must exist and be writable"
             ) from e
 
         try:
             execution_path = Path(temp_dir.name)
 
@@ -380,15 +379,13 @@
 
     def _collect_mypy_path(self, rootdir: Optional[Path]) -> None:
         mypy_path_parts = []
 
         existing_mypy_path = os.environ.get("MYPYPATH")
         if existing_mypy_path:
             mypy_path_parts.append(existing_mypy_path)
-        if self.base_ini_fpath:
-            mypy_path_parts.append(os.path.dirname(self.base_ini_fpath))
         mypy_path_key = self.environment_variables.get("MYPYPATH")
         if mypy_path_key:
             mypy_path_parts.append(maybe_to_abspath(mypy_path_key, rootdir))
             mypy_path_parts.append(mypy_path_key)
 
         self.environment_variables["MYPYPATH"] = ":".join(mypy_path_parts)
```

### Comparing `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/utils.py` & `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,20 @@
 import re
 import sys
 from dataclasses import dataclass
 from itertools import zip_longest
 from pathlib import Path
 from typing import Any, Callable, Dict, Iterator, List, Mapping, Optional, Tuple, Union
 
-import chevron
+import jinja2
 import regex
 from decorator import contextmanager
 
+_rendering_env = jinja2.Environment()
+
 
 @contextmanager
 def temp_environ() -> Iterator[None]:
     """Allow the ability to set os.environ temporarily"""
     environ = dict(os.environ)
     try:
         yield
@@ -140,14 +142,16 @@
     if len(s1) < 4:
         return error_message
 
     maxw = 72  # Maximum number of characters shown
 
     error_message += "Alignment of first line difference:\n"
 
+    assert s1 != s2
+
     trunc = False
     while s1[:30] == s2[:30]:
         s1 = s1[10:]
         s2 = s2[10:]
         trunc = True
 
     if trunc:
@@ -256,15 +260,17 @@
                 expected_message_lines.append("  ...")
                 actual_message_lines.append("  ...")
 
         error_message = "Actual:\n{}\nExpected:\n{}\n".format(
             format_error_lines(actual_message_lines), format_error_lines(expected_message_lines)
         )
 
-        if (
+        if expected_line and expected_line.regex:
+            error_message += "The actual output does not match the expected regex."
+        elif (
             first_diff_actual is not None
             and first_diff_expected is not None
             and (
                 len(first_diff_actual) >= MIN_LINE_LENGTH_FOR_ALIGNMENT
                 or len(str(first_diff_expected)) >= MIN_LINE_LENGTH_FOR_ALIGNMENT
             )
         ):
@@ -344,15 +350,16 @@
                     col=col,
                 )
             )
     return matchers
 
 
 def render_template(template: str, data: Mapping[str, Any]) -> str:
-    return chevron.render(template=template, data={k: v if v is not None else "None" for k, v in data.items()})
+    t: jinja2.environment.Template = _rendering_env.from_string(template)
+    return t.render({k: v if v is not None else "None" for k, v in data.items()})
 
 
 def get_func_first_lnum(attr: Callable[..., None]) -> Optional[Tuple[int, List[str]]]:
     lines, _ = inspect.getsourcelines(attr)
     for lnum, line in enumerate(lines):
         no_space_line = line.strip()
         if f"def {attr.__name__}" in no_space_line:
```

### Comparing `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/PKG-INFO` & `pytest-mypy-plugins-2.0.0/pytest_mypy_plugins.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 1.9.3
+Version: 2.0.0
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
+Maintainer: Nikita Sobolev
+Maintainer-email: mail@sobolevn.me
 License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="http://mypy-lang.org/static/mypy_light.svg" alt="mypy logo" width="300px"/>
 
 # pytest plugin for testing mypy types, stubs, and plugins
 
@@ -70,15 +71,15 @@
 - case: mypy_path_from_env
   main: |
     from pair import Pair
 
     instance: Pair
     reveal_type(instance)  # N: Revealed type is 'pair.Pair'
   env:
-    - MYPYPATH=./pytest_mypy_plugins/tests/fixtures
+    - MYPYPATH=../fixtures
 ```
 
 
 ### What is a test case?
 
 In general each test case is just an element in an array written in a properly formatted `YAML` file.
 On top of that, each case must comply to following types:
@@ -142,17 +143,22 @@
 - case: with_params
   parametrized:
     - val: 1
       rt: builtins.int
     - val: 1.0
       rt: builtins.float
   main: |
-    reveal_type({[ val }})  # N: Revealed type is '{{ rt }}'
+    reveal_type({{ val }})  # N: Revealed type is '{{ rt }}'
 ```
 
+Properties that you can parametrize:
+- `main`
+- `mypy_config`
+- `out`
+
 #### 3. Longer type expectations
 
 ```yaml
 - case: with_out
   main: |
     reveal_type('abc')
   out: |
@@ -199,9 +205,7 @@
 ## Further reading
 
 - [Testing mypy stubs, plugins, and types](https://sobolevn.me/2019/08/testing-mypy-types)
 
 ## License
 
 [MIT](https://github.com/typeddjango/pytest-mypy-plugins/blob/master/LICENSE)
-
-
```

### Comparing `pytest-mypy-plugins-1.9.3/setup.py` & `pytest-mypy-plugins-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     readme = f.read()
 
 dependencies = [
-    "pytest>=6.0.0",
-    "mypy>=0.900",
+    "pytest>=7.0.0",
+    "mypy>=1.3",
     "decorator",
     "pyyaml",
-    "chevron",
+    "Jinja2",
     "regex",
-    "dataclasses ; python_version<'3.7'",
+    "packaging",
 ]
 
 setup(
     name="pytest-mypy-plugins",
-    version="1.9.3",
+    version="2.0.0",
     description="pytest plugin for writing tests for mypy plugins",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/TypedDjango/pytest-mypy-plugins",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
+    maintainer="Nikita Sobolev",
+    maintainer_email="mail@sobolevn.me",
     packages=["pytest_mypy_plugins"],
     # the following makes a plugin available to pytest
     entry_points={"pytest11": ["pytest-mypy-plugins = pytest_mypy_plugins.collect"]},
     install_requires=dependencies,
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     package_data={
         "pytest_mypy_plugins": ["py.typed"],
     },
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

