# Comparing `tmp/pycareer-0.1.2.tar.gz` & `tmp/pycareer-0.1.3.tar.gz`

## Comparing `pycareer-0.1.2.tar` & `pycareer-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0   108324 2020-02-02 00:00:00.000000 pycareer-0.1.2/poetry.lock
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pycareer-0.1.2/.github/workflows/ci-cd.yml
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pycareer-0.1.2/pycareer/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pycareer-0.1.2/pycareer/cli.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pycareer-0.1.2/pycareer/formatter.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pycareer-0.1.2/pycareer/models.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pycareer-0.1.2/pycareer/request.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycareer-0.1.2/.gitignore
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycareer-0.1.2/README.md
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 pycareer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pycareer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0   108324 2020-02-02 00:00:00.000000 pycareer-0.1.3/poetry.lock
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 pycareer-0.1.3/.github/workflows/ci-cd.yml
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/cli.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/formatter.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/models.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pycareer-0.1.3/pycareer/request.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pycareer-0.1.3/.gitignore
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pycareer-0.1.3/README.md
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 pycareer-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 pycareer-0.1.3/PKG-INFO
```

### Comparing `pycareer-0.1.2/poetry.lock` & `pycareer-0.1.3/poetry.lock`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.2/pycareer/cli.py` & `pycareer-0.1.3/pycareer/cli.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.2/pycareer/formatter.py` & `pycareer-0.1.3/pycareer/formatter.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.2/pycareer/request.py` & `pycareer-0.1.3/pycareer/request.py`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.2/.gitignore` & `pycareer-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pycareer-0.1.2/pyproject.toml` & `pycareer-0.1.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [project.urls]
 Homepage = "https://pycareer.io"
 Documentation = "https://github.com/tadasgedgaudas/pycareer/README.md"
 Repository = "https://github.com/tadasgedgaudas/pycareer"
 
 [tool.poetry]
 name = "pycareer"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "pycareer"}]
 
 
 [tool.poetry.dependencies]
@@ -41,15 +41,15 @@
 line-length = 120
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.poetry.scripts]
-pycareer = "pycareer_cli.pycareer.cli:main"
+pycareer = "cli:main"
 
 [tool.hatch.version]
 path = "pycareer/__init__.py"
 
 [build-system]
 requires = ["hatchling >= 1.13.0"]
 build-backend = "hatchling.build"
```

