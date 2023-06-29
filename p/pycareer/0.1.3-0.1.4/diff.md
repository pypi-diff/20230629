# Comparing `tmp/pycareer-0.1.3.tar.gz` & `tmp/pycareer-0.1.4.tar.gz`

## Comparing `pycareer-0.1.3.tar` & `pycareer-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   108324 2020-02-02 00:00:00.000000 pycareer-0.1.3/poetry.lock
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pycareer-0.1.3/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/cli.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/formatter.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/models.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/request.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycareer-0.1.3/.gitignore
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycareer-0.1.3/README.md
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pycareer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pycareer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0   108324 2020-02-02 00:00:00.000000 pycareer-0.1.4/poetry.lock
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pycareer-0.1.4/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pycareer-0.1.4/pycareer/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pycareer-0.1.4/pycareer/cli.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pycareer-0.1.4/pycareer/formatter.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pycareer-0.1.4/pycareer/models.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pycareer-0.1.4/pycareer/request.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycareer-0.1.4/.gitignore
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycareer-0.1.4/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 pycareer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pycareer-0.1.4/PKG-INFO
```

### Comparing `pycareer-0.1.3/poetry.lock` & `pycareer-0.1.4/poetry.lock`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.3/pycareer/cli.py` & `pycareer-0.1.4/pycareer/cli.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.3/pycareer/formatter.py` & `pycareer-0.1.4/pycareer/formatter.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.3/pycareer/request.py` & `pycareer-0.1.4/pycareer/request.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.3/.gitignore` & `pycareer-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.3/pyproject.toml` & `pycareer-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 [project.urls]
 Homepage = "https://pycareer.io"
 Documentation = "https://github.com/tadasgedgaudas/pycareer/README.md"
 Repository = "https://github.com/tadasgedgaudas/pycareer"
 
 [tool.poetry]
 name = "pycareer"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
-authors = ["Your Name <you@example.com>"]
+authors = ["Tadas Gedgaudas <tadasgedgaudas@0xw.app>"]
 readme = "README.md"
 packages = [{include = "pycareer"}]
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.9.0"
@@ -41,15 +41,15 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.poetry.scripts]
-pycareer = "cli:main"
+pycareer = "pycareer.cli:main"
 
 [tool.hatch.version]
 path = "pycareer/__init__.py"
 
 [build-system]
-requires = ["hatchling >= 1.13.0"]
+requires = ["hatchling >= 1.7.0"]
 build-backend = "hatchling.build"
```

