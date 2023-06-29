# Comparing `tmp/blockit-0.0.0.tar.gz` & `tmp/blockit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockit-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "blockit-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `blockit-0.0.0.tar` & `blockit-0.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.0/.dockerignore
--rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.0/.gitignore
--rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.0/Dockerfile
--rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.0/Hillciph.pdf
--rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.0/LICENSE
--rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.0/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.0/README.md
--rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.0/ascii-table.png
--rw-r--r--   0        0        0       22 2023-06-27 16:52:55.122478 blockit-0.0.0/blockit/__init__.py
--rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.0/blockit/__main__.py
--rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.0/blockit/cli.py
--rw-r--r--   0        0        0    22306 2023-06-29 13:56:53.891309 blockit-0.0.0/blockit/crypto_algorithms.py
--rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.0/docker-compose.yml
--rw-r--r--   0        0        0     2268 2023-06-29 09:28:04.386191 blockit-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-06-29 09:17:08.018647 blockit-0.0.0/requirements.txt
--rw-r--r--   0        0        0      185 2023-06-27 15:09:15.863495 blockit-0.0.0/setup.cfg
--rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.0/test_build.py
--rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 blockit-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       44 2023-06-27 15:20:25.653377 blockit-0.0.1/.dockerignore
+-rw-r--r--   0        0        0     3076 2023-06-27 16:50:58.027428 blockit-0.0.1/.gitignore
+-rw-r--r--   0        0        0      465 2023-06-29 01:22:18.465157 blockit-0.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      910 2023-06-27 16:52:36.399243 blockit-0.0.1/Dockerfile
+-rw-r--r--   0        0        0   164426 2023-06-28 16:05:24.794108 blockit-0.0.1/Hillciph.pdf
+-rw-r--r--   0        0        0     1069 2023-02-18 13:26:33.609851 blockit-0.0.1/LICENSE
+-rw-r--r--   0        0        0      345 2023-06-27 15:12:38.873798 blockit-0.0.1/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 15:16:06.343611 blockit-0.0.1/README.md
+-rw-r--r--   0        0        0    26493 2023-06-27 15:33:57.322371 blockit-0.0.1/ascii-table.png
+-rw-r--r--   0        0        0       22 2023-06-29 14:07:35.157325 blockit-0.0.1/blockit/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-29 13:55:17.133147 blockit-0.0.1/blockit/__main__.py
+-rw-r--r--   0        0        0      947 2023-06-29 13:55:16.589155 blockit-0.0.1/blockit/cli.py
+-rw-r--r--   0        0        0    22306 2023-06-29 13:56:53.891309 blockit-0.0.1/blockit/crypto_algorithms.py
+-rw-r--r--   0        0        0       46 2023-06-27 16:50:58.483408 blockit-0.0.1/docker-compose.yml
+-rw-r--r--   0        0        0     2269 2023-06-29 14:06:17.584638 blockit-0.0.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-06-29 09:17:08.018647 blockit-0.0.1/requirements.txt
+-rw-r--r--   0        0        0      186 2023-06-29 14:06:28.417329 blockit-0.0.1/setup.cfg
+-rw-r--r--   0        0        0      107 2023-06-27 15:09:15.915495 blockit-0.0.1/test_build.py
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 blockit-0.0.1/PKG-INFO
```

### Comparing `blockit-0.0.0/.gitignore` & `blockit-0.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/Dockerfile` & `blockit-0.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/Hillciph.pdf` & `blockit-0.0.1/Hillciph.pdf`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/LICENSE` & `blockit-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/ascii-table.png` & `blockit-0.0.1/ascii-table.png`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/blockit/cli.py` & `blockit-0.0.1/blockit/cli.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/blockit/crypto_algorithms.py` & `blockit-0.0.1/blockit/crypto_algorithms.py`

 * *Files identical despite different names*

### Comparing `blockit-0.0.0/pyproject.toml` & `blockit-0.0.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 ]
 requires-python = ">=3.9"
 dependencies = [
     "typer >= 0.9.0",
 ]
 
 [project.scripts]
-appins = "blockit.cli:app"
+blockit = "blockit.cli:app"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "isort",
     "black",
     "mypy",
```

### Comparing `blockit-0.0.0/PKG-INFO` & `blockit-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockit
-Version: 0.0.0
+Version: 0.0.1
 Summary: blockit - cli tool for encrypting and decrypting strings
 Author-email: 0xsirsaif <sirsaif99@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

