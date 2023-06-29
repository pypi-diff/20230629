# Comparing `tmp/efcamdat-0.0.4.tar.gz` & `tmp/efcamdat-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efcamdat-0.0.4.tar", max compression
+gzip compressed data, was "efcamdat-0.0.5.tar", max compression
```

## Comparing `efcamdat-0.0.4.tar` & `efcamdat-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-06-28 11:18:03.859806 efcamdat-0.0.4/LICENSE
--rw-r--r--   0        0        0      209 2023-06-28 11:17:36.112139 efcamdat-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-28 11:11:07.423621 efcamdat-0.0.4/efcamdat/__init__.py
--rw-r--r--   0        0        0      290 2023-06-28 15:31:55.837660 efcamdat-0.0.4/efcamdat/cli.py
--rw-r--r--   0        0        0       80 2023-06-28 15:31:57.111424 efcamdat-0.0.4/efcamdat/transform.py
--rw-r--r--   0        0        0      651 2023-06-28 15:36:43.747455 efcamdat-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 efcamdat-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-28 11:18:03.859806 efcamdat-0.0.5/LICENSE
+-rw-r--r--   0        0        0      209 2023-06-28 11:17:36.112139 efcamdat-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-28 11:11:07.423621 efcamdat-0.0.5/efcamdat/__init__.py
+-rw-r--r--   0        0        0     5719 2023-06-29 20:59:33.855189 efcamdat-0.0.5/efcamdat/cli.py
+-rw-r--r--   0        0        0       80 2023-06-28 15:31:57.111424 efcamdat-0.0.5/efcamdat/transform.py
+-rw-r--r--   0        0        0      704 2023-06-29 20:17:17.326576 efcamdat-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 efcamdat-0.0.5/PKG-INFO
```

### Comparing `efcamdat-0.0.4/LICENSE` & `efcamdat-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `efcamdat-0.0.4/pyproject.toml` & `efcamdat-0.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 [tool.poetry]
 name = "EFCAMDAT"
-version = "0.0.4"
+version = "0.0.5"
 authors = [ "Bernardo Stearns <bernardo.stearns@gmail.com>" ]
 description = "A library for doing all preprocessing related to EFCAMDAT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 typer = {extras = ["all"], version = "^0.1.0"}
+pydantic = "^1.10.9"
+pyyaml = "^6.0"
+nltk = "^3.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 twine = "^4.0.2"
 
 [tool.poetry.scripts]
 efcamdat_cli = "efcamdat.cli:app"
```

### Comparing `efcamdat-0.0.4/PKG-INFO` & `efcamdat-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: efcamdat
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for doing all preprocessing related to EFCAMDAT
 Author: Bernardo Stearns
 Author-email: bernardo.stearns@gmail.com
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nltk (>=3.8.1,<4.0.0)
+Requires-Dist: pydantic (>=1.10.9,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer[all] (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 # The EFCAMDAT dataset preprocessing Package
 
 This is a simple package to preprocessing tasks in the EFCAMDAT dataset. You can see the docs here 
 [DOCS](https://guides.github.com/features/mastering-markdown/)
```

