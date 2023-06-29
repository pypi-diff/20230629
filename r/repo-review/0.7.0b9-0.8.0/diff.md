# Comparing `tmp/repo_review-0.7.0b9.tar.gz` & `tmp/repo_review-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Jun 12 21:33:23 2023, max compression
+gzip compressed data, last modified: Thu Jun 29 13:59:05 2023, max compression
```

## Comparing `repo_review-0.7.0b9.tar` & `repo_review-0.8.0.tar`

### file list

```diff
@@ -1,55 +1,57 @@
--rw-r--r--   0        0        0      125 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.git_archival.txt
--rw-r--r--   0        0        0       32 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.gitattributes
--rw-r--r--   0        0        0     2061 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      187 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0      399 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.readthedocs.yml
--rw-r--r--   0        0        0     1216 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/action.yml
--rw-r--r--   0        0        0     3197 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/noxfile.py
--rw-r--r--   0        0        0      359 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     2544 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      162 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/matchers/pylint.json
--rw-r--r--   0        0        0      669 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2356 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.github/workflows/ci.yml
--rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/.nojekyll
--rw-r--r--   0        0        0     4836 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/checks.md
--rw-r--r--   0        0        0      990 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/cli.md
--rw-r--r--   0        0        0      925 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/conf.py
--rw-r--r--   0        0        0     1236 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/families.md
--rw-r--r--   0        0        0     2023 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/fixtures.md
--rw-r--r--   0        0        0     1917 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/index.html
--rw-r--r--   0        0        0      243 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/index.md
--rw-r--r--   0        0        0     2244 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/intro.md
--rw-r--r--   0        0        0     2746 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/plugins.md
--rw-r--r--   0        0        0    10216 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/webapp.js
--rw-r--r--   0        0        0     1770 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/webapp.md
--rw-r--r--   0        0        0     1033 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/docs/api/repo_review.rst
--rw-r--r--   0        0        0      230 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/__init__.py
--rw-r--r--   0        0        0     7353 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/__main__.py
--rw-r--r--   0        0        0      162 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_version.py
--rw-r--r--   0        0        0      118 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_version.pyi
--rw-r--r--   0        0        0     2741 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/checks.py
--rw-r--r--   0        0        0     1055 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/families.py
--rw-r--r--   0        0        0     3156 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/fixtures.py
--rw-r--r--   0        0        0     6010 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/ghpath.py
--rw-r--r--   0        0        0     2301 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/html.py
--rw-r--r--   0        0        0     6278 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/processor.py
--rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/py.typed
--rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/__init__.py
--rw-r--r--   0        0        0      233 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/tomllib.py
--rw-r--r--   0        0        0      246 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/typing.py
--rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/resources/__init__.py
--rw-r--r--   0        0        0      256 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/src/repo_review/_compat/importlib/resources/abc.py
--rw-r--r--   0        0        0     4393 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_checks.py
--rw-r--r--   0        0        0      904 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_cmd.py
--rw-r--r--   0        0        0     2460 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_fixtures.py
--rw-r--r--   0        0        0      598 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_package.py
--rw-r--r--   0        0        0     2185 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_self.py
--rw-r--r--   0        0        0     3981 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_utilities/pyproject.py
--rw-r--r--   0        0        0      333 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/tests/test_utilities/pyproject.toml
--rw-r--r--   0        0        0     2086 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/.gitignore
--rw-r--r--   0        0        0     1525 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/LICENSE
--rw-r--r--   0        0        0     6104 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/README.md
--rw-r--r--   0        0        0     5190 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/pyproject.toml
--rw-r--r--   0        0        0     8326 2023-06-12 21:33:23.000000 repo_review-0.7.0b9/PKG-INFO
+-rw-r--r--   0        0        0      125 2023-06-29 13:59:05.000000 repo_review-0.8.0/.git_archival.txt
+-rw-r--r--   0        0        0       32 2023-06-29 13:59:05.000000 repo_review-0.8.0/.gitattributes
+-rw-r--r--   0        0        0     2061 2023-06-29 13:59:05.000000 repo_review-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      187 2023-06-29 13:59:05.000000 repo_review-0.8.0/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0      400 2023-06-29 13:59:05.000000 repo_review-0.8.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     1216 2023-06-29 13:59:05.000000 repo_review-0.8.0/action.yml
+-rw-r--r--   0        0        0     3242 2023-06-29 13:59:05.000000 repo_review-0.8.0/noxfile.py
+-rw-r--r--   0        0        0      359 2023-06-29 13:59:05.000000 repo_review-0.8.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     2527 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      162 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      669 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2356 2023-06-29 13:59:05.000000 repo_review-0.8.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/.nojekyll
+-rw-r--r--   0        0        0      217 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/changelog.md
+-rw-r--r--   0        0        0     5910 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/checks.md
+-rw-r--r--   0        0        0      990 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/cli.md
+-rw-r--r--   0        0        0     1009 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0     1236 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/families.md
+-rw-r--r--   0        0        0     2243 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/fixtures.md
+-rw-r--r--   0        0        0     1919 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/index.html
+-rw-r--r--   0        0        0      253 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/index.md
+-rw-r--r--   0        0        0     2248 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/intro.md
+-rw-r--r--   0        0        0     2746 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/plugins.md
+-rw-r--r--   0        0        0     2801 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/programmatic.md
+-rw-r--r--   0        0        0    10215 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/webapp.js
+-rw-r--r--   0        0        0     1770 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/webapp.md
+-rw-r--r--   0        0        0     1033 2023-06-29 13:59:05.000000 repo_review-0.8.0/docs/api/repo_review.rst
+-rw-r--r--   0        0        0      230 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/__init__.py
+-rw-r--r--   0        0        0     7626 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/__main__.py
+-rw-r--r--   0        0        0      160 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_version.py
+-rw-r--r--   0        0        0      118 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_version.pyi
+-rw-r--r--   0        0        0     3576 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/checks.py
+-rw-r--r--   0        0        0     1591 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/families.py
+-rw-r--r--   0        0        0     3607 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/fixtures.py
+-rw-r--r--   0        0        0     6010 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/ghpath.py
+-rw-r--r--   0        0        0     2315 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/html.py
+-rw-r--r--   0        0        0     7410 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/processor.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/py.typed
+-rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/__init__.py
+-rw-r--r--   0        0        0      233 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/tomllib.py
+-rw-r--r--   0        0        0      246 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/typing.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/resources/__init__.py
+-rw-r--r--   0        0        0      256 2023-06-29 13:59:05.000000 repo_review-0.8.0/src/repo_review/_compat/importlib/resources/abc.py
+-rw-r--r--   0        0        0     4393 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_checks.py
+-rw-r--r--   0        0        0      904 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_cmd.py
+-rw-r--r--   0        0        0     2460 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_fixtures.py
+-rw-r--r--   0        0        0      598 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_package.py
+-rw-r--r--   0        0        0     2185 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_self.py
+-rw-r--r--   0        0        0     3981 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_utilities/pyproject.py
+-rw-r--r--   0        0        0      333 2023-06-29 13:59:05.000000 repo_review-0.8.0/tests/test_utilities/pyproject.toml
+-rw-r--r--   0        0        0     2086 2023-06-29 13:59:05.000000 repo_review-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1525 2023-06-29 13:59:05.000000 repo_review-0.8.0/LICENSE
+-rw-r--r--   0        0        0     6123 2023-06-29 13:59:05.000000 repo_review-0.8.0/README.md
+-rw-r--r--   0        0        0     5262 2023-06-29 13:59:05.000000 repo_review-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     8397 2023-06-29 13:59:05.000000 repo_review-0.8.0/PKG-INFO
```

### Comparing `repo_review-0.7.0b9/.pre-commit-config.yaml` & `repo_review-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/action.yml` & `repo_review-0.8.0/action.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/noxfile.py` & `repo_review-0.8.0/noxfile.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,26 +88,27 @@
         "-b", dest="builder", default="html", help="Build target (default: html)"
     )
     args, posargs = parser.parse_known_args(session.posargs)
 
     if args.builder != "html" and args.serve:
         session.error("Must not specify non-HTML builder with --serve")
 
-    session.install(".[docs]")
+    session.install("-e.[docs]")
     session.chdir("docs")
 
     if args.builder == "linkcheck":
         session.run(
             "sphinx-build", "-b", "linkcheck", ".", "_build/linkcheck", *posargs
         )
         return
 
     session.run(
         "sphinx-build",
         "-n",  # nitpicky mode
+        "--keep-going",  # show all errors
         "-T",  # full tracebacks
         "-b",
         args.builder,
         ".",
         f"_build/{args.builder}",
         *posargs,
     )
```

### Comparing `repo_review-0.7.0b9/.github/CONTRIBUTING.md` & `repo_review-0.8.0/.github/CONTRIBUTING.md`

 * *Files 8% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 To use, run `nox`. This will lint and test using every installed version of
 Python on your system, skipping ones that are not installed. You can also run
 specific jobs:
 
 ```console
 $ nox -s lint  # Lint only
-$ nox -s tests-3.9  # Python 3.9 tests only
-$ nox -s docs -- serve  # Build and serve the docs
+$ nox -s tests # Tests
+$ nox -s docs -- --serve  # Build and serve the docs
 $ nox -s build  # Make an SDist and wheel
 ```
 
 Nox handles everything for you, including setting up an temporary virtual
 environment for each run.
 
 You can also use `nox -s run -- .` to run an example set of checks on a repo.
@@ -73,15 +73,15 @@
 ```bash
 nox -s docs
 ```
 
 You can see a preview with:
 
 ```bash
-nox -s docs -- serve
+nox -s docs -- --serve
 ```
 
 ## Pre-commit
 
 This project uses pre-commit for all style checking. While you can run it with
 nox, this is such an important tool that it deserves to be installed on its
 own. Install pre-commit and run:
```

### Comparing `repo_review-0.7.0b9/.github/matchers/pylint.json` & `repo_review-0.8.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/.github/workflows/cd.yml` & `repo_review-0.8.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/.github/workflows/ci.yml` & `repo_review-0.8.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/docs/checks.md` & `repo_review-0.8.0/docs/checks.md`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 You need to implement `family`, which is a string indicating which family it is
 grouped under, and `check()`, which can take [](./fixtures.md), and returns `True` if
 the check passes, or `False` if the check fails. If you want a dynamic error
 explanation instead of the `check()` docstring, you can return a non-empty
 string from the check instead of `False`. Returning `None` makes a check
 "skipped". Docstrings/error messages can access their own object with `{self}`
-and check name with `{name}` (these are processed with `.format`, so escape `{}`
+and check name with `{name}` (these are processed with `.format()`, so escape `{}`
 as `{{}}`). The error message is in markdown format.
 
 If the check named in `requires` does not pass, the check is skipped.
 
 A suggested convention for easily writing checks is as follows:
 
 ```python
@@ -97,15 +97,15 @@
 ```python
 def repo_review_checks() -> dict[str, General | PyProject]:
     general = {p.__name__: p() for p in General.__subclasses__()}
     pyproject = {p.__name__: p() for p in PyProject.__subclasses__()}
     return general | pyproject
 ```
 
-You tell repo review to use this function via an entry-point:
+You tell repo-review to use this function via an entry-point:
 
 ```toml
 [project.entry-points."repo_review.checks"]
 general_pyproject = "my_plugin_package.my_checks_module:repo_review_checks"
 ```
 
 The entry-point name doesn't matter.
@@ -150,7 +150,40 @@
     }
     match pyproject:
         case {"build-system": {"build-backend": str(x)}} if x in backends:
             return {"PP003": PP003(name=backends[x])}
         case _:
             return {}
 ```
+
+### Handling empty generation
+
+If repo-review is listing all checks, a
+{class}`repo_review.ghpath.EmptyTraversable` is passed for `root` and
+`package`. This will appear to be a directory with no contents. If you have
+conditional checks, you should handle this case to support being listed as a
+possible check. As a helper for this case, a
+{func}`~repo_review.fixtures.list_all` fixture is provided that returns {obj}`True`
+only if a list-all operation is being performed. The above can then be written:
+
+```python
+def repo_review_checks(
+    list_all: bool, pyproject: dict[str, Any]
+) -> dict[str, PyProject]:
+    backends = {
+        "setuptools.build_api": "setuptools",
+        "scikit_build_core.build": "scikit-build",
+    }
+
+    if list_all:
+        return {"PP003": PP003(name="<backend>")}
+
+    match pyproject:
+        case {"build-system": {"build-backend": str(x)}} if x in backends:
+            return {"PP003": PP003(name=backends[x])}
+        case _:
+            return {}
+```
+
+```{versionadded} 0.8
+The {func}`~repo_review.fixtures.list_all` fixture.
+```
```

### Comparing `repo_review-0.7.0b9/docs/cli.md` & `repo_review-0.8.0/docs/cli.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/docs/conf.py` & `repo_review-0.8.0/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import importlib.metadata
+import os
 
 project = "repo-review"
 copyright = "2022, Henry Schreiner"
 author = "Henry Schreiner"
-release = importlib.metadata.version("repo-review").split("+")[0]
-version = ".".join(release.split(".")[:2])
+version = importlib.metadata.version("repo-review").split("+")[0]
+release = version
 
 extensions = [
     "myst_parser",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx_autodoc_typehints",
     "sphinx_copybutton",
     "sphinxcontrib.programoutput",
+    "sphinx_github_changelog",
     "sphinxext.opengraph",
 ]
 
 source_suffix = [".rst", ".md"]
 
 exclude_patterns = [
     "_build",
@@ -41,7 +43,9 @@
 nitpick_ignore = [
     ("py:class", "_io.StringIO"),
     ("py:class", "_io.BytesIO"),
     ("py:class", "repo_review.fixtures.T"),
 ]
 
 always_document_param_types = True
+
+sphinx_github_changelog_token = os.environ.get("GITHUB_API_TOKEN")
```

### Comparing `repo_review-0.7.0b9/docs/families.md` & `repo_review-0.8.0/docs/families.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/docs/fixtures.md` & `repo_review-0.8.0/docs/fixtures.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Fixtures
 
-Like pytest fixtures, fixtures in repo-review are requested by name. There are three built-in fixtures:
+Like pytest fixtures, fixtures in repo-review are requested by name. There are four built-in fixtures:
 
-- `root: Traversable` - The repository path. All checks or fixtures that depend on the root of the repository should use this.
-- `package: Traversable` - The path to the package directory. This is the same as `root` unless `--package-dir` is passed.
-- `pyproject: dict[str, Any]` - The `pyproject.toml` in the package if it exists, an empty dict otherwise.
+- `root`: {class}`~importlib.resources.abc.Traversable` - The repository path. All checks or fixtures that depend on the root of the repository should use this.
+- `package`: `~importlib.resources.abc.Traversable` - The path to the package directory. This is the same as `root` unless `--package-dir` is passed.
+- {func}`~repo_review.fixtures.pyproject`: `dict[str, Any]` - The `pyproject.toml` in the package if it exists, an empty dict otherwise.
+- {func}`~repo_review.fixtures.list_all`: `bool` - returns True if repo-review is just trying to collect all checks to list them.
 
 Repo-review doesn't necessarily assume any form or language for your repository,
 but since it already looks for configuration in `pyproject.toml`, this fixture
 is provided.
 
 ## Writing a fixture
```

### Comparing `repo_review-0.7.0b9/docs/index.html` & `repo_review-0.8.0/docs/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   <head>
     <meta
       charset="utf-8"
       name="viewport"
       content="initial-scale=1, width=device-width"
     />
     <script
-      src="https://cdn.jsdelivr.net/pyodide/v0.23.2/full/pyodide.js"
+      src="https://cdn.jsdelivr.net/pyodide/v0.23.3/full/pyodide.js"
       crossorigin
     ></script>
     <!-- Production -->
     <script
       src="https://unpkg.com/react@18/umd/react.production.min.js"
       crossorigin
     ></script>
@@ -59,13 +59,13 @@
   <body>
     <div id="root">Loading...</div>
     <script type="text/babel">
       const root = ReactDOM.createRoot(document.getElementById("root"));
       root.render(
         <App
           header={true}
-          deps={["sp_repo_review==2023.06.07", "repo-review==0.7.0b8"]}
+          deps={["sp-repo-review==2023.06.17", "repo-review>=0.7,<=0.9"]}
         />,
       );
     </script>
   </body>
 </html>
```

### Comparing `repo_review-0.7.0b9/docs/intro.md` & `repo_review-0.8.0/docs/intro.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 Though check your favorite plugin, which might directly support running from
 pre-commit, and then pre-commit's pinning system will pin on your plugin,
 rather than the framework (repo-review).
 
 ## GitHub Actions
 
-```
+```yaml
 - uses: scientific-python/repo-review@<version>
   with:
     plugins: sp-repo-review
 ```
 
 (Insert the current version above, optionally pin the plugin version, as long
 as you have a way to auto-update it.)
```

### Comparing `repo_review-0.7.0b9/docs/plugins.md` & `repo_review-0.8.0/docs/plugins.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/docs/webapp.js` & `repo_review-0.8.0/docs/webapp.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -352,15 +352,15 @@
             }
             console.log(families);
             for (const val of results_list) {
                 results[val.family].push({
                     name: val.name.toString(),
                     description: val.description.toString(),
                     state: val.result,
-                    err_msg: val.err_markdown().toString(),
+                    err_msg: val.err_as_html().toString(),
                     url: val.url.toString(),
                 });
             }
 
             this.setState({
                 results: results,
                 families: families,
```

### Comparing `repo_review-0.7.0b9/docs/webapp.md` & `repo_review-0.8.0/docs/webapp.md`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/docs/api/repo_review.rst` & `repo_review-0.8.0/docs/api/repo_review.rst`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/src/repo_review/__main__.py` & `repo_review-0.8.0/src/repo_review/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,18 +22,19 @@
 import rich.text
 import rich.traceback
 import rich.tree
 
 from . import __version__
 from ._compat.importlib.resources.abc import Traversable
 from ._compat.typing import assert_never
-from .families import Family
-from .ghpath import EmptyTraversable, GHPath
+from .checks import get_check_description, get_check_url
+from .families import Family, get_family_name
+from .ghpath import GHPath
 from .html import to_html
-from .processor import Result, _collect_all, as_simple_dict, process
+from .processor import Result, as_simple_dict, collect_all, process
 
 __all__ = ["main"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
@@ -41,23 +42,30 @@
 rich.traceback.install(suppress=[click, rich, orig_click], show_locals=True, width=None)
 
 
 def list_all(ctx: click.Context, _param: click.Parameter, value: bool) -> None:
     if not value or ctx.resilient_parsing:
         return
 
-    _, checks, families = _collect_all(EmptyTraversable())
-    if len(checks) == 0:
+    collected = collect_all()
+    if len(collected.checks) == 0:
         msg = "No checks registered. Please install a repo-review plugin."
         raise click.ClickException(msg)
 
-    for family, grp in itertools.groupby(checks.items(), key=lambda x: x[1].family):
-        rich.print(f'  [dim]# {families[family].get("name", family)}')
+    for family, grp in itertools.groupby(
+        collected.checks.items(), key=lambda x: x[1].family
+    ):
+        rich.print(f"  [dim]# {get_family_name(collected.families, family)}")
         for code, check in grp:
-            rich.print(f'  "{code}",  [dim]# {check.__doc__}')
+            url = get_check_url(code, check)
+            doc = get_check_description(code, check)
+            link = f"[link={url}]{code}[/link]" if url else code
+            comment = f" [dim]# {doc}" if doc else ""
+            rich.print(f'  "{link}",{comment}')
+
     ctx.exit()
 
 
 def rich_printer(
     families: Mapping[str, Family],
     processed: list[Result],
     *,
@@ -66,15 +74,15 @@
     color: bool = True,
 ) -> None:
     console = rich.console.Console(
         record=svg, quiet=svg, stderr=stderr, color_system="auto" if color else None
     )
 
     for family, results_list in itertools.groupby(processed, lambda r: r.family):
-        family_name = families[family].get("name", family)
+        family_name = get_family_name(families, family)
         tree = rich.tree.Tree(f"[bold]{family_name}[/bold]:")
         for result in results_list:
             style = (
                 "yellow"
                 if result.result is None
                 else "green"
                 if result.result
@@ -202,16 +210,16 @@
 ) -> None:
     """
     Pass in a local Path or gh:org/repo@branch.
     """
     ignore_list = {x.strip() for x in ignore.split(",") if x}
     select_list = {x.strip() for x in select.split(",") if x}
 
-    _, checks, _ = _collect_all(package, subdir=package_dir)
-    if len(checks) == 0:
+    collected = collect_all(package, subdir=package_dir)
+    if len(collected.checks) == 0:
         msg = "No checks registered. Please install a repo-review plugin."
         raise click.ClickException(msg)
 
     if str(package).startswith("gh:"):
         _, org_repo_branch, *p = str(package).split(":", maxsplit=2)
         org_repo, branch = org_repo_branch.split("@", maxsplit=1)
         package = GHPath(repo=org_repo, branch=branch, path=p[0] if p else "")
```

### Comparing `repo_review-0.7.0b9/src/repo_review/checks.py` & `repo_review-0.8.0/src/repo_review/checks.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import importlib.metadata
 from collections.abc import Mapping, Set
 from typing import Any, Protocol
 
 from .fixtures import apply_fixtures
 
-__all__ = ["Check", "collect_checks", "is_allowed"]
+__all__ = ["Check", "collect_checks", "is_allowed", "get_check_url"]
 
 
 class Check(Protocol):
     """
     This is the check Protocol. Since Python doesn't support optional Protocol
     members, the two optional members are required if you want to use this
     Protocol in a type checker. The members can be specified as class
@@ -79,7 +79,35 @@
     :return: True if this check is allowed, False otherwise.
     """
     if select and name not in select and name.rstrip("0123456789") not in select:
         return False
     if name in ignore or name.rstrip("0123456789") in ignore:
         return False
     return True
+
+
+def get_check_url(name: str, check: Check) -> str:
+    """
+    Get the url from a check instance. Will return an empty string if missing.
+    Will process string via format.
+
+    :param name: The name of the check (letters and number)
+    :param check: The check to process.
+    :return: The final URL.
+
+    .. versionadded:: 0.8
+    """
+    return getattr(check, "url", "").format(self=check, name=name)
+
+
+def get_check_description(name: str, check: Check) -> str:
+    """
+    Get the doc from a check instance. Will return an empty string if missing.
+    Will process string via format.
+
+    :param name: The name of the check (letters and number)
+    :param check: The check to process.
+    :return: The final doc.
+
+    .. versionadded:: 0.8
+    """
+    return (check.__doc__ or "").format(self=check, name=name)
```

### Comparing `repo_review-0.7.0b9/src/repo_review/families.py` & `repo_review-0.8.0/src/repo_review/families.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import importlib.metadata
 import typing
+from collections.abc import Mapping
 
-__all__ = ["Family", "collect_families"]
+__all__ = ["Family", "collect_families", "get_family_name"]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
 class Family(typing.TypedDict, total=False):
@@ -32,7 +33,21 @@
     :class:`Family`'s.
     """
     return {
         name: family
         for ep in importlib.metadata.entry_points(group="repo_review.families")
         for name, family in ep.load()().items()
     }
+
+
+def get_family_name(families: Mapping[str, Family], family: str) -> str:
+    """
+    Returns the "nice" family name if there is one, otherwise the (input)
+    family short name.
+
+    :param families: A dict of family short names to :class:`.Family`'s.
+    :param family: The short name of a family.
+    :return: The nice family name if there is one, otherwise the short name is returned.
+
+    .. versionadded:: 0.8
+    """
+    return families.get(family, {}).get("name", family)
```

### Comparing `repo_review-0.7.0b9/src/repo_review/fixtures.py` & `repo_review-0.8.0/src/repo_review/fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 import inspect
 import typing
 from collections.abc import Callable, Mapping, Set
 from typing import Any
 
 from ._compat import tomllib
 from ._compat.importlib.resources.abc import Traversable
+from .ghpath import EmptyTraversable
 
 __all__ = [
     "pyproject",
+    "list_all",
     "compute_fixtures",
     "apply_fixtures",
     "collect_fixtures",
 ]
 
 
 def __dir__() -> list[str]:
@@ -24,22 +26,38 @@
 
 def pyproject(package: Traversable) -> dict[str, Any]:
     """
     Fixture: The ``pyproject.toml`` structure from the package. Returned an
     empty dict if no pyproject.toml found.
 
     :param package: The package fixture.
+
+    :return: The pyproject.toml dict or an empty dict if no file found.
     """
     pyproject_path = package.joinpath("pyproject.toml")
     if pyproject_path.is_file():
         with pyproject_path.open("rb") as f:
             return tomllib.load(f)
     return {}
 
 
+def list_all(root: Traversable) -> bool:
+    """
+    Fixture: Is True when this is trying to produce a list of all checks.
+
+    :param root: The root fixture.
+
+    :return: True only if trying to make a list of all checks/fixtures/families.
+
+    .. versionadded:: 0.8
+    """
+
+    return isinstance(root, EmptyTraversable)
+
+
 def compute_fixtures(
     root: Traversable,
     package: Traversable,
     unevaluated_fixtures: Mapping[str, Callable[..., Any]],
 ) -> dict[str, Any]:
     """
     Given the repo ``root`` Traversable, the ``package`` Traversable, and the dict
```

### Comparing `repo_review-0.7.0b9/src/repo_review/ghpath.py` & `repo_review-0.8.0/src/repo_review/ghpath.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/src/repo_review/html.py` & `repo_review-0.8.0/src/repo_review/html.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import functools
 import io
 import itertools
 from collections.abc import Mapping
 
 import markdown_it
 
-from .families import Family
+from .families import Family, get_family_name
 from .processor import Result
 
 __all__ = ["to_html"]
 
 
 def __dir__() -> list[str]:
     return __all__
@@ -26,15 +26,15 @@
     :param processed: The list of processed results.
     """
     out = io.StringIO()
     print = functools.partial(builtins.print, file=out)
     md = markdown_it.MarkdownIt()
 
     for family, results_list in itertools.groupby(processed, lambda r: r.family):
-        family_name = families[family].get("name", family)
+        family_name = get_family_name(families, family)
         print(f"<h2>{family_name}</h2>")
         print("<table>")
         print("<tr><th>?</th><th>Name</th><th>Description</th></tr>")
         for result in results_list:
             color = (
                 "orange"
                 if result.result is None
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations import builtins import functools import io
 import itertools from collections.abc import Mapping import markdown_it from
-.families import Family from .processor import Result __all__ = ["to_html"] def
-__dir__() -> list[str]: return __all__ def to_html(families: Mapping[str,
-Family], processed: list[Result]) -> str: """ Convert the results of a repo
-review (``families``, ``processed``) to HTML. :param families: The family
-mapping. :param processed: The list of processed results. """ out = io.StringIO
-() print = functools.partial(builtins.print, file=out) md =
+.families import Family, get_family_name from .processor import Result __all__
+= ["to_html"] def __dir__() -> list[str]: return __all__ def to_html(families:
+Mapping[str, Family], processed: list[Result]) -> str: """ Convert the results
+of a repo review (``families``, ``processed``) to HTML. :param families: The
+family mapping. :param processed: The list of processed results. """ out =
+io.StringIO() print = functools.partial(builtins.print, file=out) md =
 markdown_it.MarkdownIt() for family, results_list in itertools.groupby
-(processed, lambda r: r.family): family_name = families[family].get("name",
+(processed, lambda r: r.family): family_name = get_family_name(families,
 family) print(f"
 ***** {family_name} *****
 ") print("
 ?      Name          Description
 {icon} {result.name} {description} ") print(description) print("
                                    ") print(md.render(result.err_msg)) print("
 ") if len(processed) == 0: print('No checks ran.') return out.getvalue()
```

### Comparing `repo_review-0.7.0b9/src/repo_review/processor.py` & `repo_review-0.8.0/src/repo_review/processor.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,25 +6,27 @@
 import typing
 from collections.abc import Mapping, Set
 from typing import Any, TypeVar
 
 import markdown_it
 
 from ._compat.importlib.resources.abc import Traversable
-from .checks import Check, collect_checks, is_allowed
+from .checks import Check, collect_checks, get_check_url, is_allowed
 from .families import Family, collect_families
 from .fixtures import apply_fixtures, collect_fixtures, compute_fixtures, pyproject
+from .ghpath import EmptyTraversable
 
 __all__ = [
+    "CollectionReturn",
+    "ProcessReturn",
     "Result",
     "ResultDict",
-    "ProcessReturn",
-    "process",
     "as_simple_dict",
-    "_collect_all",
+    "collect_all",
+    "process",
 ]
 
 
 def __dir__() -> list[str]:
     return __all__
 
 
@@ -53,34 +55,50 @@
     family: str  #: The family string
     name: str  #: The name of the check
     description: str  #: The short description of what the check looks for
     result: bool | None  #: The result, None means skip
     err_msg: str = ""  #: The error message if the result is false, in markdown format
     url: str = ""  #: An optional URL (empty string if missing)
 
-    def err_markdown(self) -> str:
+    def err_as_html(self) -> str:
         """
         Produces HTML from the error message, assuming it is in markdown.
         """
         result: str = md.render(self.err_msg).strip()
         return result.removeprefix("<p>").removesuffix("</p>").strip()
 
 
 class ProcessReturn(typing.NamedTuple):
     """
     Return type for :func:`process`.
     """
 
-    families: dict[str, Family]  #: A mapping of family strings to Family info dicts
+    families: dict[
+        str, Family
+    ]  #: A mapping of family strings to :class:`.Family` info dicts
     results: list[Result]  #: The results list
 
 
+class CollectionReturn(typing.NamedTuple):
+    """
+    Return type for :func:`collect_all`.
+
+    .. versionadded:: 0.8
+    """
+
+    fixtures: dict[str, Any]  #: The computed fixtures, as a :class:`dict`
+    checks: dict[str, Check]  #: The checks dict, sorted by :class:`.Family`.
+    families: dict[
+        str, Family
+    ]  #: A mapping of family strings to :class:`.Family` info dicts
+
+
 class HasFamily(typing.Protocol):
     """
-    Simple Protocol to see if family property is present.
+    Simple :class:`~typing.Protocol` to see if family property is present.
     """
 
     @property
     def family(self) -> str:
         ...
 
 
@@ -94,17 +112,31 @@
         sorted(
             dict_has_family.items(),
             key=lambda x: (families[x[1].family].get("order", 0), x[1].family, x[0]),
         )
     )
 
 
-def _collect_all(
-    root: Traversable, subdir: str = ""
-) -> tuple[dict[str, Any], dict[str, Check], dict[str, Family]]:
+def collect_all(
+    root: Traversable = EmptyTraversable(),  # noqa: B008 (frozen dataclass OK)
+    subdir: str = "",
+) -> CollectionReturn:
+    """
+    Collect all checks. If ``root`` is not passed, then checks are collected
+    with a :class:`~repo_review.ghpath.EmptyTraversable`. Any checks that are
+    returned conditionally based on fixture results might not be collected
+    unless :func:`~repo_review.fixtures.list_all` is used.
+
+    :param root: If passed, this is the root of the repo (for fixture computation).
+    :param subdir: The subdirectory (for fixture computation).
+
+    :return: The collected fixtures, checks, and families.
+
+    .. versionadded:: 0.8
+    """
     package = root.joinpath(subdir) if subdir else root
 
     # Collect the fixtures
     fixture_functions = collect_fixtures()
     fixtures = compute_fixtures(root, package, fixture_functions)
 
     # Collect the checks
@@ -117,39 +149,38 @@
     for name in {c.family for c in checks.values()}:
         if name not in families:
             families[name] = Family()
 
     # Sort results
     checks = _sort_by_family(families, checks)
 
-    return fixtures, checks, families
+    return CollectionReturn(fixtures, checks, families)
 
 
 def process(
     root: Traversable,
     *,
     select: Set[str] = frozenset(),
     ignore: Set[str] = frozenset(),
     subdir: str = "",
 ) -> ProcessReturn:
     """
     Process the package and return a dictionary of results.
 
-    :param root: The Path(like) to the repository to process
-
-    :param ignore: A list of checks to ignore
-
+    :param root: The Traversable to the repository to process.
+    :param select: A list of checks to select. All checks selected if empty.
+    :param ignore: A list of checks to ignore.
     :param subdir: The path to the package in the subdirectory, if not at the
                    root of the repository.
 
     :return: A dictionary of check results.
     """
     package = root.joinpath(subdir) if subdir else root
 
-    fixtures, tasks, families = _collect_all(root, subdir)
+    fixtures, tasks, families = collect_all(root, subdir)
 
     # Collect our own config
     config = pyproject(package).get("tool", {}).get("repo-review", {})
     select_checks = select if select else set(config.get("select", ()))
     skip_checks = ignore if ignore else set(config.get("ignore", ()))
 
     # Make a graph of the check's interdependencies
@@ -184,15 +215,15 @@
         result_list.append(
             Result(
                 family=check.family,
                 name=task_name,
                 description=doc.format(self=check, name=task_name),
                 result=result,
                 err_msg=textwrap.dedent(err_msg.format(self=check, name=task_name)),
-                url=getattr(check, "url", "").format(self=check, name=task_name),
+                url=get_check_url(task_name, check),
             )
         )
 
     return ProcessReturn(families, result_list)
 
 
 def as_simple_dict(results: list[Result]) -> dict[str, ResultDict]:
```

### Comparing `repo_review-0.7.0b9/tests/test_checks.py` & `repo_review-0.8.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/tests/test_cmd.py` & `repo_review-0.8.0/tests/test_cmd.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/tests/test_fixtures.py` & `repo_review-0.8.0/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/tests/test_package.py` & `repo_review-0.8.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/tests/test_self.py` & `repo_review-0.8.0/tests/test_self.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/tests/test_utilities/pyproject.py` & `repo_review-0.8.0/tests/test_utilities/pyproject.py`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/.gitignore` & `repo_review-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/LICENSE` & `repo_review-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `repo_review-0.7.0b9/README.md` & `repo_review-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,19 @@
 So if you want to lint Python code, use Flake8 or Ruff. But if you want to
 check Flake8 or Ruff's configuration, use repo-review! Generally, repo-review
 plugins are more about requiring things to be present, like making use all your
 repos have some [pre-commit][] check.
 
 ## Development of repo-review and plugins
 
-This repository is intended to be fun and easy to develop - it requires and uses
-Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
-entirely conventional, but it enables very simple plugin development. It works
-locally, remotely, and in WebAssembly (using [Pyodide][]).
+This project is intended to be fun and easy to develop and design checks for -
+it requires and uses Python 3.10, and uses a lot of the new features in 3.9 and
+3.10. It's maybe not entirely conventional, but it enables very simple plugin
+development. It works locally, remotely, and in WebAssembly (using
+[Pyodide][]).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
```

### Comparing `repo_review-0.7.0b9/pyproject.toml` & `repo_review-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,16 @@
   "pyyaml",
   "tomli; python_version < '3.11'",
   "typing-extensions; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 cli = [
-  "click>=8",
-  "rich>=12.2",
+  "click >=8",
+  "rich >=12.2",
   "rich-click",
 ]
 test = [
   "pytest >=7",
   "sp-repo-review",
 ]
 dev = [
@@ -54,28 +54,30 @@
   "myst_parser >=0.13",
   "repo-review[cli]",
   "sphinx >=4.0",
   "sphinx-autodoc-typehints",
   "sphinx-copybutton",
   "sphinxcontrib-programoutput",
   "sphinxext-opengraph",
+  "sphinx-github-changelog",
 ]
 
 [project.urls]
 Changelog = "https://github.com/scientific-python/repo-review/releases"
 Demo = "https://scientific-python.github.io/repo-review"
-Documentation = "https://repo-review.readthedocs.io/"
-Homepage = "https://repo-review.readthedocs.io/"
+Documentation = "https://repo-review.readthedocs.io"
+Homepage = "https://repo-review.readthedocs.io"
 Source = "https://github.com/scientific-python/repo-review"
 
 [project.scripts]
 repo-review = "repo_review.__main__:main"
 
 [project.entry-points."repo_review.fixtures"]
 pyproject = "repo_review.fixtures:pyproject"
+list_all = "repo_review.fixtures:list_all"
 
 
 [tool.hatch]
 version.source = "vcs"
 build.hooks.vcs.version-file = "src/repo_review/_version.py"
```

### Comparing `repo_review-0.7.0b9/PKG-INFO` & `repo_review-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: repo_review
-Version: 0.7.0b9
+Version: 0.8.0
 Summary: Framework that can run checks on repos
 Project-URL: Changelog, https://github.com/scientific-python/repo-review/releases
 Project-URL: Demo, https://scientific-python.github.io/repo-review
-Project-URL: Documentation, https://repo-review.readthedocs.io/
-Project-URL: Homepage, https://repo-review.readthedocs.io/
+Project-URL: Documentation, https://repo-review.readthedocs.io
+Project-URL: Homepage, https://repo-review.readthedocs.io
 Project-URL: Source, https://github.com/scientific-python/repo-review
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: WebAssembly :: Emscripten
 Classifier: Intended Audience :: Developers
@@ -37,14 +37,15 @@
 Requires-Dist: repo-review[cli,test]; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: furo; extra == 'docs'
 Requires-Dist: myst-parser>=0.13; extra == 'docs'
 Requires-Dist: repo-review[cli]; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx-copybutton; extra == 'docs'
+Requires-Dist: sphinx-github-changelog; extra == 'docs'
 Requires-Dist: sphinx>=4.0; extra == 'docs'
 Requires-Dist: sphinxcontrib-programoutput; extra == 'docs'
 Requires-Dist: sphinxext-opengraph; extra == 'docs'
 Provides-Extra: test
 Requires-Dist: pytest>=7; extra == 'test'
 Requires-Dist: sp-repo-review; extra == 'test'
 Description-Content-Type: text/markdown
@@ -110,18 +111,19 @@
 So if you want to lint Python code, use Flake8 or Ruff. But if you want to
 check Flake8 or Ruff's configuration, use repo-review! Generally, repo-review
 plugins are more about requiring things to be present, like making use all your
 repos have some [pre-commit][] check.
 
 ## Development of repo-review and plugins
 
-This repository is intended to be fun and easy to develop - it requires and uses
-Python 3.10, and uses a lot of the new features in 3.9 and 3.10. It's maybe not
-entirely conventional, but it enables very simple plugin development. It works
-locally, remotely, and in WebAssembly (using [Pyodide][]).
+This project is intended to be fun and easy to develop and design checks for -
+it requires and uses Python 3.10, and uses a lot of the new features in 3.9 and
+3.10. It's maybe not entirely conventional, but it enables very simple plugin
+development. It works locally, remotely, and in WebAssembly (using
+[Pyodide][]).
 
 There are a few key designs that are very useful and make this possible. First,
 all paths are handled as Traversables. This allows a simple Traversable
 implementation based on `open_url` to provide a web interface for use in the
 webapp. It also would allow `zipfile.Path` to work just as well, too - no need
 to extract.
```

