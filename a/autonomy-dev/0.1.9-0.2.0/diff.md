# Comparing `tmp/autonomy_dev-0.1.9.tar.gz` & `tmp/autonomy_dev-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomy_dev-0.1.9.tar", max compression
+gzip compressed data, was "autonomy_dev-0.2.0.tar", max compression
```

## Comparing `autonomy_dev-0.1.9.tar` & `autonomy_dev-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0      578 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/LICENSE
--rw-r--r--   0        0        0      368 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/README.md
--rw-r--r--   0        0        0        0 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/__init__.py
--rw-r--r--   0        0        0     2569 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/base.py
--rw-r--r--   0        0        0      242 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/cli.py
--rw-r--r--   0        0        0     2758 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/cli_executor.py
--rw-r--r--   0        0        0     3318 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/augment.py
--rw-r--r--   0        0        0     1890 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/fmt.py
--rw-r--r--   0        0        0     2151 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/lint.py
--rw-r--r--   0        0        0     5195 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/repo.py
--rw-r--r--   0        0        0    10945 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/scaffold.py
--rw-r--r--   0        0        0     1450 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/commands/test.py
--rw-r--r--   0        0        0      515 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/constants.py
--rw-r--r--   0        0        0      173 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/mermaid.py
--rw-r--r--   0        0        0      642 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/pylama.ini
--rw-r--r--   0        0        0      532 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/data/repo/templates/python/readme.py
--rw-r--r--   0        0        0     2027 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/fmt.py
--rw-r--r--   0        0        0      464 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/lint.py
--rw-r--r--   0        0        0      438 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/test.py
--rw-r--r--   0        0        0     1585 2023-06-26 02:33:37.494932 autonomy_dev-0.1.9/auto_dev/utils.py
--rw-r--r--   0        0        0     2595 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      455 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/conftest.py
--rw-r--r--   0        0        0     1634 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_augmenter.py
--rw-r--r--   0        0        0     1108 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_cli.py
--rw-r--r--   0        0        0     2488 2023-06-26 02:33:37.498932 autonomy_dev-0.1.9/tests/test_contracts.py
--rw-r--r--   0        0        0     2619 1970-01-01 00:00:00.000000 autonomy_dev-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/LICENSE
+-rw-r--r--   0        0        0      368 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/__init__.py
+-rw-r--r--   0        0        0     2569 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/base.py
+-rw-r--r--   0        0        0      242 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/cli.py
+-rw-r--r--   0        0        0     2758 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/cli_executor.py
+-rw-r--r--   0        0        0     3335 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/augment.py
+-rw-r--r--   0        0        0     1890 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/fmt.py
+-rw-r--r--   0        0        0     2144 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/lint.py
+-rw-r--r--   0        0        0     5195 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/repo.py
+-rw-r--r--   0        0        0    10945 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/scaffold.py
+-rw-r--r--   0        0        0     1450 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/commands/test.py
+-rw-r--r--   0        0        0      515 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/constants.py
+-rw-r--r--   0        0        0      173 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/mermaid.py
+-rw-r--r--   0        0        0      642 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/pylama.ini
+-rw-r--r--   0        0        0      532 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/data/repo/templates/python/readme.py
+-rw-r--r--   0        0        0     2027 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/fmt.py
+-rw-r--r--   0        0        0      464 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/lint.py
+-rw-r--r--   0        0        0     2153 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/local_fork.py
+-rw-r--r--   0        0        0      470 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/test.py
+-rw-r--r--   0        0        0     1585 2023-06-29 10:49:13.957270 autonomy_dev-0.2.0/auto_dev/utils.py
+-rw-r--r--   0        0        0     2613 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      455 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1634 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_augmenter.py
+-rw-r--r--   0        0        0     1108 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_cli.py
+-rw-r--r--   0        0        0     2488 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_contracts.py
+-rw-r--r--   0        0        0     1562 2023-06-29 10:49:13.961270 autonomy_dev-0.2.0/tests/test_local_fork.py
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 autonomy_dev-0.2.0/PKG-INFO
```

### Comparing `autonomy_dev-0.1.9/LICENSE` & `autonomy_dev-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/base.py` & `autonomy_dev-0.2.0/auto_dev/base.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/cli_executor.py` & `autonomy_dev-0.2.0/auto_dev/cli_executor.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/augment.py` & `autonomy_dev-0.2.0/auto_dev/commands/augment.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         return logging_config
 
     def scaffold(self, handlers: list):
         """Scaffold logging."""
         path = "aea-config.yaml"
         if not Path(path).exists():
             raise FileNotFoundError(f"File {path} not found")
-        aea_config = yaml.safe_load(Path(path).read_text(encoding=DEFAULT_ENCODING))
+        aea_config = list(yaml.safe_load_all(Path(path).read_text(encoding=DEFAULT_ENCODING))).pop(0)
         logging_config = self.generate(handlers)
         aea_config.update(logging_config)
         write(path, aea_config)
         return logging_config
 
 
 @cli.group()
```

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/fmt.py` & `autonomy_dev-0.2.0/auto_dev/commands/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/lint.py` & `autonomy_dev-0.2.0/auto_dev/commands/lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         results = single_thread_lint(paths, verbose, logger)
     passed = sum(results.values())
     failed = len(results) - passed
     logger.info(f"Linting completed with {passed} passed and {failed} failed")
     if failed > 0:
         for file_path, result in results.items():
             if not result:
-                logger.error(f"Linting failed for {paths[file_path]}")
+                logger.error(f"Linting failed for {file_path}")
     if failed > 0:
         raise click.ClickException("Linting failed!")
 
 
 def single_thread_lint(paths, verbose, logger):
     """Run the linting in a single thread."""
     results = {}
```

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/repo.py` & `autonomy_dev-0.2.0/auto_dev/commands/repo.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/scaffold.py` & `autonomy_dev-0.2.0/auto_dev/commands/scaffold.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/commands/test.py` & `autonomy_dev-0.2.0/auto_dev/commands/test.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/constants.py` & `autonomy_dev-0.2.0/auto_dev/constants.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/data/pylama.ini` & `autonomy_dev-0.2.0/auto_dev/data/pylama.ini`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/data/repo/templates/python/readme.py` & `autonomy_dev-0.2.0/auto_dev/data/repo/templates/python/readme.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/fmt.py` & `autonomy_dev-0.2.0/auto_dev/fmt.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/auto_dev/utils.py` & `autonomy_dev-0.2.0/auto_dev/utils.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/pyproject.toml` & `autonomy_dev-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "autonomy_dev"
-version = "0.1.9"
+version = "0.2.0"
 homepage = "https://github.com/8ball030/auto_dev"
 description = "A collection of tooling to enable open source development of autonomy tools"
 authors = ["8Baller <8ball030@gmail.com>"]
 readme = "README.md"
 license =  "Apache-2.0"
 classifiers=[
     'Development Status :: 2 - Pre-Alpha',
@@ -49,14 +49,15 @@
 mkdocstrings-python = "^0.10.0"
 isort = "~5"
 pylint = "~2"
 open-aea = "^1.35.0"
 open-aea-cli-ipfs = "^1.35.0"
 web3 = "~5"
 responses = "^0.23.1"
+docker = "^6.1.3"
 
 [tool.poetry.dev-dependencies]
 
 
 [tool.poetry.extras]
 all = [
     "pytest",
```

### Comparing `autonomy_dev-0.1.9/tests/test_augmenter.py` & `autonomy_dev-0.2.0/tests/test_augmenter.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/tests/test_cli.py` & `autonomy_dev-0.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/tests/test_contracts.py` & `autonomy_dev-0.2.0/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `autonomy_dev-0.1.9/PKG-INFO` & `autonomy_dev-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomy-dev
-Version: 0.1.9
+Version: 0.2.0
 Summary: A collection of tooling to enable open source development of autonomy tools
 Home-page: https://github.com/8ball030/auto_dev
 License: Apache-2.0
 Author: 8Baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.7.2,<=3.11
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,14 +19,15 @@
 Provides-Extra: all
 Provides-Extra: dev
 Provides-Extra: doc
 Requires-Dist: GitPython (>=3.1.27,<4.0.0)
 Requires-Dist: black (>=22.6.0,<23.0.0) ; extra == "all"
 Requires-Dist: bump2version (>=1.0.1,<2.0.0) ; extra == "dev"
 Requires-Dist: click (==8.0.2)
+Requires-Dist: docker (>=6.1.3,<7.0.0)
 Requires-Dist: install (>=1.3.5,<2.0.0)
 Requires-Dist: isort (>=5,<6) ; extra == "all"
 Requires-Dist: mkdocs (>=1.3.1,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=3.6.1,<4.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=8.4.0,<9.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0)
```

