# Comparing `tmp/gitease-0.0.6.tar.gz` & `tmp/gitease-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitease-0.0.6.tar", last modified: Tue Jun 27 12:57:16 2023, max compression
+gzip compressed data, was "gitease-0.0.7.tar", last modified: Wed Jun 28 14:51:08 2023, max compression
```

## Comparing `gitease-0.0.6.tar` & `gitease-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.285625 gitease-0.0.6/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.6/.gitattributes
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4161 2023-06-19 19:56:47.000000 gitease-0.0.6/.gitignore
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1068 2023-06-19 20:28:50.000000 gitease-0.0.6/LICENSE
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4564 2023-06-27 12:57:16.285250 gitease-0.0.6/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3287 2023-06-27 12:55:55.000000 gitease-0.0.6/README.md
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.279565 gitease-0.0.6/docs/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      634 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/Makefile
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1134 2023-06-27 12:55:55.000000 gitease-0.0.6/docs/conf.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.279940 gitease-0.0.6/docs/images/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)   174135 2023-06-19 20:35:34.000000 gitease-0.0.6/docs/images/logo.png
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     2152 2023-06-27 10:53:24.000000 gitease-0.0.6/docs/index.rst
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      800 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/make.bat
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.281206 gitease-0.0.6/docs/markdowns/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      260 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/markdowns/quickstart.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     9780 2023-06-27 12:55:55.000000 gitease-0.0.6/docs/markdowns/usage.md
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       60 2023-06-19 19:56:47.000000 gitease-0.0.6/docs/requirements.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.282638 gitease-0.0.6/gitease/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.6/gitease/__init__.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4628 2023-06-27 10:53:24.000000 gitease-0.0.6/gitease/automations.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     6250 2023-06-27 12:55:55.000000 gitease-0.0.6/gitease/cli.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4765 2023-06-27 12:55:55.000000 gitease-0.0.6/gitease/git_helper.py
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     3140 2023-06-19 18:15:11.000000 gitease-0.0.6/gitease/llm_helper.py
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.284688 gitease-0.0.6/gitease/prompts/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      947 2023-06-13 08:49:13.000000 gitease-0.0.6/gitease/prompts/prompt_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      823 2023-06-13 08:49:13.000000 gitease-0.0.6/gitease/prompts/refine_template.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.6/gitease/prompts/undo_template.txt
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.283988 gitease-0.0.6/gitease.egg-info/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     4564 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/PKG-INFO
--rw-r--r--   0 yonatanalexander   (501) staff       (20)      641 2023-06-27 12:57:16.000000 gitease-0.0.6/gitease.egg-info/SOURCES.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/dependency_links.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/entry_points.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       94 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/requires.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-27 12:57:12.000000 gitease-0.0.6/gitease.egg-info/top_level.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)     1555 2023-06-27 12:55:55.000000 gitease-0.0.6/pyproject.toml
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.6/requirements.txt
--rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-27 12:57:16.285698 gitease-0.0.6/setup.cfg
-drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-27 12:57:16.284879 gitease-0.0.6/tests/
--rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.6/tests/__init__.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.750462 gitease-0.0.7/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       79 2023-06-07 11:21:02.000000 gitease-0.0.7/.gitattributes
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4174 2023-06-28 13:30:52.000000 gitease-0.0.7/.gitignore
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      708 2023-06-27 15:09:45.000000 gitease-0.0.7/.readthedocs.yaml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1068 2023-06-27 15:09:45.000000 gitease-0.0.7/LICENSE
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4565 2023-06-28 14:51:08.750064 gitease-0.0.7/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     3288 2023-06-28 14:49:02.000000 gitease-0.0.7/README.md
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.743811 gitease-0.0.7/docs/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      634 2023-06-19 19:56:47.000000 gitease-0.0.7/docs/Makefile
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1131 2023-06-27 15:18:05.000000 gitease-0.0.7/docs/conf.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.744210 gitease-0.0.7/docs/images/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)   173327 2023-06-28 14:36:04.000000 gitease-0.0.7/docs/images/logo.png
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2153 2023-06-27 15:17:54.000000 gitease-0.0.7/docs/index.rst
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      800 2023-06-19 19:56:47.000000 gitease-0.0.7/docs/make.bat
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.744980 gitease-0.0.7/docs/markdowns/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      261 2023-06-27 15:09:45.000000 gitease-0.0.7/docs/markdowns/quickstart.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     9780 2023-06-27 15:09:45.000000 gitease-0.0.7/docs/markdowns/usage.md
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       90 2023-06-27 15:09:45.000000 gitease-0.0.7/docs/requirements.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.746383 gitease-0.0.7/gitease/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        2 2023-06-14 15:01:01.000000 gitease-0.0.7/gitease/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     6146 2023-06-28 14:12:53.000000 gitease-0.0.7/gitease/cli.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4420 2023-06-28 13:30:52.000000 gitease-0.0.7/gitease/git_helper.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2772 2023-06-28 13:30:52.000000 gitease-0.0.7/gitease/llm_helper.py
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.748105 gitease-0.0.7/gitease/prompts/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      956 2023-06-28 13:30:52.000000 gitease-0.0.7/gitease/prompts/prompt_template.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      157 2023-06-15 11:21:54.000000 gitease-0.0.7/gitease/prompts/undo_template.txt
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.747711 gitease-0.0.7/gitease.egg-info/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     4565 2023-06-28 14:51:05.000000 gitease-0.0.7/gitease.egg-info/PKG-INFO
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      703 2023-06-28 14:51:08.000000 gitease-0.0.7/gitease.egg-info/SOURCES.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        1 2023-06-28 14:51:05.000000 gitease-0.0.7/gitease.egg-info/dependency_links.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       39 2023-06-28 14:51:05.000000 gitease-0.0.7/gitease.egg-info/entry_points.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      111 2023-06-28 14:51:05.000000 gitease-0.0.7/gitease.egg-info/requires.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        8 2023-06-28 14:51:05.000000 gitease-0.0.7/gitease.egg-info/top_level.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     1579 2023-06-28 14:39:36.000000 gitease-0.0.7/pyproject.toml
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       64 2023-06-12 19:37:45.000000 gitease-0.0.7/requirements.txt
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)       38 2023-06-28 14:51:08.750569 gitease-0.0.7/setup.cfg
+drwxr-xr-x   0 yonatanalexander   (501) staff       (20)        0 2023-06-28 14:51:08.749598 gitease-0.0.7/tests/
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)        0 2023-06-07 11:21:27.000000 gitease-0.0.7/tests/__init__.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2505 2023-06-28 13:30:52.000000 gitease-0.0.7/tests/cli_test.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)     2478 2023-06-28 13:30:52.000000 gitease-0.0.7/tests/git_helper_test.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      754 2023-06-28 13:30:52.000000 gitease-0.0.7/tests/llm_helper_test.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      208 2023-06-28 13:30:52.000000 gitease-0.0.7/tests/util_tests.py
+-rw-r--r--   0 yonatanalexander   (501) staff       (20)      423 2023-06-28 13:30:52.000000 gitease-0.0.7/tests/utils.py
```

### Comparing `gitease-0.0.6/.gitignore` & `gitease-0.0.7/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -262,8 +262,9 @@
 # (https://github.com/github/gitignore/pull/2483#issue-259490424)
 /gitllm.egg-info/
 **.egg-info/**
 **/**/**.pyc
 dist/*
 docs/_build/*
 docs/_static
-docs/_templates
+docs/_templates
+docs/_images
```

### Comparing `gitease-0.0.6/LICENSE` & `gitease-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gitease-0.0.6/PKG-INFO` & `gitease-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -27,14 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
+
 # GitEase
 [![Version](https://img.shields.io/pypi/v/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Python](https://img.shields.io/pypi/pyversions/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![License](https://img.shields.io/github/license/xetdata/gitease?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
 [![Downloads](https://img.shields.io/pypi/dm/gitease?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Documentation Status](https://readthedocs.org/projects/gitease/badge/?version=latest)](https://gitease.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gitease-0.0.6/README.md` & `gitease-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 <p align="center">
    <img src="https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
+
 # GitEase
 [![Version](https://img.shields.io/pypi/v/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Python](https://img.shields.io/pypi/pyversions/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![License](https://img.shields.io/github/license/xetdata/gitease?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
 [![Downloads](https://img.shields.io/pypi/dm/gitease?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Documentation Status](https://readthedocs.org/projects/gitease/badge/?version=latest)](https://gitease.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gitease-0.0.6/docs/Makefile` & `gitease-0.0.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gitease-0.0.6/docs/conf.py` & `gitease-0.0.7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,12 @@
 
 extensions = ["myst_parser", "sphinx.ext.autodoc", "sphinx.ext.napoleon", "sphinx.ext.viewcode", "sphinx_rtd_theme",
               "sphinx_book_theme"]
 
 templates_path = ['_templates']
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', 'docs', '.venv']
 
-
-
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "sphinx_book_theme"
-html_static_path = ['_static']
+html_static_path = ['_static']
```

### Comparing `gitease-0.0.6/docs/index.rst` & `gitease-0.0.7/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.. image:: https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png
+.. figure:: https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png
   :width: 250
   :alt: gitease-logo
 
 
 Welcome to GitEase's documentation!
 ===================================
```

### Comparing `gitease-0.0.6/docs/make.bat` & `gitease-0.0.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gitease-0.0.6/docs/markdowns/usage.md` & `gitease-0.0.7/docs/markdowns/usage.md`

 * *Files identical despite different names*

### Comparing `gitease-0.0.6/gitease/cli.py` & `gitease-0.0.7/gitease/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         console.print("No changes files to add", style=Style(color="red", blink=True, bold=True))
 
     if not is_valid(message):
         message = get_message(helper, quiet, y)
 
     if is_valid(message):
         helper.commit(message)
-        console.print(f"Committed with message: {message}")
+        console.print(f"Committed with message: {message}", style=Style(color="green", blink=True, bold=True))
     if is_valid(staged_at_start):  # cleanup
         helper.unstage(add)
         helper.stage(staged_at_start)
 
 
 @cli.command()
 def share(add: add_annotation = None,
@@ -114,40 +114,35 @@
           y: y_annotation = False):
     """Share to remote: add, commit and push to git"""
     save(add=add, message=message, quiet=quiet, y=y)
     GitHelper(verbose=not quiet).push()
     console.print("Pushed changes to the cloud", style=Style(color="green", blink=True, bold=True))
 
 
-
 @cli.command()
 def load():
     """Pull recent updates from git"""
-    GitHelper().pull()
+    console.print(GitHelper().pull(), style=Style(color="yellow", blink=True, bold=True))
 
 
 @cli.command()
 def message(quiet: quiet_annotation = False,
             copy: Annotated[bool, typer.Option("--copy", "-c", help="Copy to clipboard")] = False):
     """Generate commit message from diff using AI"""
     if not OPENAI_API_KEY:
         console.print(f"OPENAI_API_KEY not set", style=Style(color="red", blink=True, bold=True))
         return False
     diff = GitHelper(verbose=not quiet).get_diff(staged=True)
     message = LanguageModel(verbose=not quiet).summarize(diff).lstrip()
     console.print("Commit message:\n", style=Style(color="red", blink=True, bold=True))
     console.print(message)
     if copy:
-        try:
-            import clipboard
-            console.print("Copied to clipboard", style=Style(color="green"))
-            clipboard.copy(message)
-        except ImportError:
-            console.print("Install clipboard to copy to clipboard: 'pip install clipboard'",
-                          style=Style(color="red", blink=True, bold=True))
+        import pyperclip
+        pyperclip.copy(message)
+        console.print("Copied to clipboard", style=Style(color="green"))
 
 
 @cli.command()
 def undo():
     """Undo last git action"""
     llm = LanguageModel()
     reflog = "\n".join(GitHelper().reflog().split("\n")[0])
```

### Comparing `gitease-0.0.6/gitease/git_helper.py` & `gitease-0.0.7/gitease/git_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -37,38 +37,42 @@
     def get_diff(self, staged: bool = False):
         """
         Returns the Git diff of the repository.
          :param staged: Whether to return the staged diff.
          :return: The Git diff.
         """
         if staged:
-            staged = '--staged'
-        return self.repo.git.diff(staged)
+            return self.repo.git.diff('--staged')
+        return self.repo.git.diff()
 
-    def push(self):
+    def push(self, force: bool = False):
         """
         Pushes the repository to the remote.
          :return: The Git push output.
         """
-
+        if force:
+            return self.repo.git.push('--force')
         return self.repo.git.push()
 
     def pull(self):
         """
         Pulls the repository from the remote.
          :return: The Git pull output.
         """
         return self.repo.git.pull()
 
     def get_staged(self):
         """
         Returns the staged files.
          :return: The staged files.
         """
-        return self.repo.git.diff('--staged', '--name-only').split('\n')
+        staged = self.repo.git.diff('--staged', '--name-only').split('\n')
+        if staged == ['']:
+            staged = []
+        return staged
 
     def stage(self, files: List[str] = None):
         """
         Stages the files.
          :param files: The files to stage.
         """
         if not files:
@@ -100,54 +104,49 @@
         status = self.get_status()
         for line in status.split('\n'):
             if line.startswith('??') or line.strip().startswith('M'):
                 files.append(line[3:])
 
         return files
 
-    def add_commit(self, files: List[str] = None, message: str = None):
-        """
-        Adds and commits changes to the repository.
-         :param files: The list of files to add and commit. If None, all changes will be added and committed.
-         :param message: The commit message.
-        :return: True if changes were added and committed, False otherwise.
-        """
-        if not files:
-            new_files, changed_files = self.get_changes()
-            files = new_files + changed_files
-        if not files:
-            print("No changes found")
-            return False
-
-        if message is None:
-            message = self.summarize_diff(staged=True)
-            message = message + f"\n{self._join_files(files)}"
-        if self.verbose:
-            print(f"Adding files to git: {files}")
-        self.repo.index.add(files)
-        if self.verbose:
-            print(message)
-        self.repo.index.commit(message)
-        return True
-
     def summarize_diff(self, staged: bool = False):
         """
         Summarizes the Git diff of the repository.
          :param staged: Whether to summarize the staged diff.
         :return: The summarized diff.
         """
         if os.getenv("OPENAI_API_KEY") is None:
             raise RuntimeError(
                 f"OPENAI_API_KEY not set - please set it in your environment variables or provide a commit message manually.")
         with contextlib.suppress(openai.error.InvalidRequestError):
-            return LanguageModel(verbose=self.verbose).summarize(self.get_diff(staged=staged))
+            diff = self.get_diff(staged=staged)
+            if diff:
+                diff = LanguageModel(verbose=self.verbose).summarize(diff)
+            return diff
+
         return "Diff too long to summarize."
 
     def reflog(self):
         return self.repo.git.reflog('show')
 
-    def restore(self, files: List[str] = None):
+
+    def reset(self, hard: bool = False, commit:str=None ):
+        args =[]
+        if hard:
+            args.append('--hard')
+        if commit:
+            args.append(commit)
+        return self.repo.git.reset(*args)
+
+    def remove(self, files: List[str] = None, commit:str=None):
+        """
+        Removes the files.
+         :param files: The files to remove.
+         :param commit: The commit message.
+        """
         if not files:
             return False
-        command = f"(cd {self.repo.working_tree_dir} && git restore --staged {' '.join(files)})"
-        subprocess.run(command, shell=True)
+        commit = commit or f"Removed files - {files}"
+        self.repo.index.remove(files)
+        self.repo.index.commit(commit)
         return True
+
```

### Comparing `gitease-0.0.6/gitease/llm_helper.py` & `gitease-0.0.7/gitease/llm_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,50 +19,45 @@
     """
 
     def __init__(self, verbose: bool = True, temperature=0):
         """
         Initializes the Summarizer class with a text splitter and a summarize chain.
          :param verbose: A boolean indicating whether to print verbose output.
         """
-        prompt_path = os.path.join(os.path.dirname(__file__), 'prompts/prompt_template.txt')
-        summarize_template = PromptTemplate(template=Path(prompt_path).read_text(),
-                                            input_variables=["text"])
+
+        summarize_template = PromptTemplate(
+            template=Path(os.path.join(os.path.dirname(__file__), 'prompts/prompt_template.txt')).read_text(),
+            input_variables=["text"])
         self.llm = OpenAI(temperature=temperature)
         self.text_splitter = RecursiveCharacterTextSplitter(
             chunk_size=4000,
             chunk_overlap=20,
             length_function=len,
         )
         self.summarize_chain = load_summarize_chain(llm=self.llm,
                                                     chain_type="map_reduce",
                                                     map_prompt=summarize_template,
                                                     combine_prompt=summarize_template,
                                                     verbose=verbose)
         self.parser = PydanticOutputParser(pydantic_object=RevertCommand)
-        prompt_path = os.path.join(os.path.dirname(__file__), 'prompts/undo_template.txt')
+
         self.undo_template = PromptTemplate(
-            template=Path(prompt_path).read_text(),
+            template=Path(os.path.join(os.path.dirname(__file__), 'prompts/undo_template.txt')).read_text(),
             input_variables=["reflog"],
             partial_variables={"format_instructions": self.parser.get_format_instructions()}
         )
 
     def summarize(self, text: str):
         """
         Summarizes the given text using OpenAI's language model.
          :param text: The text to be summarized.
         :return: The summarized text.
         """
-        try:
-            texts = self.text_splitter.create_documents([text])
-            return self.summarize_chain.run(texts)
-        except openai.error.InvalidRequestError as e:
-            print(f"Invalid request error: {e}")
-        except Exception as e:
-            print(f"Error summarizing text: {e}")
-        raise RuntimeError("Summarization failed - try to add a single file")
+        texts = self.text_splitter.create_documents([text])
+        return self.summarize_chain.run(texts)
 
     def get_git_undo(self, reflog: str):
         """
         Returns the last git action and the command to undo it.
         :return: The undo command.
         """
         # TODO explicit maybe? """https://github.blog/2015-06-08-how-to-undo-almost-anything-with-git/"""
```

### Comparing `gitease-0.0.6/gitease/prompts/prompt_template.txt` & `gitease-0.0.7/gitease/prompts/prompt_template.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Generate an clear and elaborate git commit message written in present tense for the following code diff with the given specifications below:
+Generate a clear and elaborate git commit message written in present tense for the following code diff with the given specifications below:
 Your entire response will be passed directly into git commit.
-Include a concise summary of the change from each file in the diff.
+Include a concise and short summary of the change from each file in the diff.
 Pick one of the following titles:
 
 TITLES:
 docs: Documentation only changes
 style: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc),
 refactor: A code change that neither fixes a bug nor adds a feature
 perf: A code change that improves performance
```

### Comparing `gitease-0.0.6/gitease.egg-info/PKG-INFO` & `gitease-0.0.7/gitease.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitease
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to simplfy git operations
 Maintainer-email: XetHub <contact@xethub.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://xethub.com/xdssio/gitease
 Keywords: ai,llm,openai,developer-tools,git,nlp
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -27,14 +27,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
    <img src="https://xethub.com/xdssio/gitease/raw/branch/main/docs/images/logo.png" alt="logo" width="400" />
 </p>
 
+
 # GitEase
 [![Version](https://img.shields.io/pypi/v/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Python](https://img.shields.io/pypi/pyversions/gitease.svg?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![License](https://img.shields.io/github/license/xetdata/gitease?style=flat)](https://xethub.com/xdssio/gitease/src/branch/main/LICENSE)
 [![Downloads](https://img.shields.io/pypi/dm/gitease?style=flat)](https://pypi.python.org/pypi/gitease/)
 [![Documentation Status](https://readthedocs.org/projects/gitease/badge/?version=latest)](https://gitease.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `gitease-0.0.6/gitease.egg-info/SOURCES.txt` & `gitease-0.0.7/gitease.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 .gitattributes
 .gitignore
+.readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/requirements.txt
 docs/images/logo.png
 docs/markdowns/quickstart.md
 docs/markdowns/usage.md
 gitease/__init__.py
-gitease/automations.py
 gitease/cli.py
 gitease/git_helper.py
 gitease/llm_helper.py
 gitease.egg-info/PKG-INFO
 gitease.egg-info/SOURCES.txt
 gitease.egg-info/dependency_links.txt
 gitease.egg-info/entry_points.txt
 gitease.egg-info/requires.txt
 gitease.egg-info/top_level.txt
 gitease/prompts/prompt_template.txt
-gitease/prompts/refine_template.txt
 gitease/prompts/undo_template.txt
-tests/__init__.py
+tests/__init__.py
+tests/cli_test.py
+tests/git_helper_test.py
+tests/llm_helper_test.py
+tests/util_tests.py
+tests/utils.py
```

### Comparing `gitease-0.0.6/pyproject.toml` & `gitease-0.0.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gitease"
-version = "0.0.6"
+version = "0.0.7"
 description = "A tool to simplfy git operations"
 readme = "README.md"
 keywords = [
     "ai",
     "llm",
     "openai",
     "developer-tools",
@@ -39,15 +39,16 @@
 ]
 dependencies = [
     "openai>=0.27.7",
     "typer>=0.9.0",
     "rich>=13.4.2",
     "langchain>=0.0.191",
     "GitPython>=3.1.31",
-    "tiktoken>=0.4.0"
+    "tiktoken>=0.4.0",
+    "pyperclip>=1.8.2"
 ]
 
 [project.urls]
 Homepage = "https://xethub.com/xdssio/gitease"
 
 
 [project.scripts]
```

