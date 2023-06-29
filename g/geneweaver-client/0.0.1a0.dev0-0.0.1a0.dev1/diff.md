# Comparing `tmp/geneweaver_client-0.0.1a0.dev0.tar.gz` & `tmp/geneweaver_client-0.0.1a0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_client-0.0.1a0.dev0.tar", max compression
+gzip compressed data, was "geneweaver_client-0.0.1a0.dev1.tar", max compression
```

## Comparing `geneweaver_client-0.0.1a0.dev0.tar` & `geneweaver_client-0.0.1a0.dev1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11356 2023-06-29 12:40:34.692952 geneweaver_client-0.0.1a0.dev0/LICENSE
--rw-r--r--   0        0        0        2 2023-06-26 23:35:00.771148 geneweaver_client-0.0.1a0.dev0/README.md
--rw-r--r--   0        0        0     1126 2023-06-29 21:38:53.158036 geneweaver_client-0.0.1a0.dev0/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-28 18:15:46.077427 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/__init__.py
--rw-r--r--   0        0        0       37 2023-06-29 12:46:46.688012 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/__init__.py
--rw-r--r--   0        0        0       70 2023-06-26 23:35:00.775445 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/auth.py
--rw-r--r--   0        0        0      238 2023-06-28 18:06:18.299347 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/exc.py
--rw-r--r--   0        0        0     1454 2023-06-29 12:45:06.212514 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/genesets.py
--rw-r--r--   0        0        0     2033 2023-06-29 16:22:14.199284 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/legacy.py
--rw-r--r--   0        0        0     1356 2023-06-29 16:16:12.508098 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/utils.py
--rw-r--r--   0        0        0       66 2023-06-29 16:15:01.097656 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/batch/__init__.py
--rw-r--r--   0        0        0       48 2023-06-29 16:24:20.097633 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/cli/__init__.py
--rw-r--r--   0        0        0      704 2023-06-29 19:25:08.024792 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/cli/main.py
--rw-r--r--   0        0        0     1552 2023-06-29 16:31:43.842718 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/cli/parser.py
--rw-r--r--   0        0        0     3112 2023-06-29 16:11:53.517604 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/config.py
--rw-r--r--   0        0        0      699 2023-06-29 13:51:51.654691 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/exceptions.py
--rw-r--r--   0        0        0       55 2023-06-29 16:07:27.581298 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/__init__.py
--rw-r--r--   0        0        0     6080 2023-06-29 12:45:06.228269 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/csv.py
--rw-r--r--   0        0        0     3332 2023-06-29 20:09:30.754509 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/general.py
--rw-r--r--   0        0        0     1374 2023-06-29 20:39:58.278826 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/utils.py
--rw-r--r--   0        0        0     7619 2023-06-29 13:46:46.600190 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/xlsx.py
--rw-r--r--   0        0        0      194 2023-06-28 19:49:38.153124 geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/types.py
--rw-r--r--   0        0        0     1205 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev0/setup.py
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-29 12:40:34.692952 geneweaver_client-0.0.1a0.dev1/LICENSE
+-rw-r--r--   0        0        0      568 2023-06-29 21:51:24.356766 geneweaver_client-0.0.1a0.dev1/README.md
+-rw-r--r--   0        0        0     1127 2023-06-29 21:51:27.895618 geneweaver_client-0.0.1a0.dev1/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-28 18:15:46.077427 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-29 12:46:46.688012 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-26 23:35:00.775445 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/auth.py
+-rw-r--r--   0        0        0      238 2023-06-28 18:06:18.299347 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/exc.py
+-rw-r--r--   0        0        0     1454 2023-06-29 12:45:06.212514 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/genesets.py
+-rw-r--r--   0        0        0     2033 2023-06-29 16:22:14.199284 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/legacy.py
+-rw-r--r--   0        0        0     1356 2023-06-29 16:16:12.508098 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/utils.py
+-rw-r--r--   0        0        0       66 2023-06-29 16:15:01.097656 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/batch/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-29 16:24:20.097633 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/__init__.py
+-rw-r--r--   0        0        0      704 2023-06-29 19:25:08.024792 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/main.py
+-rw-r--r--   0        0        0     1552 2023-06-29 16:31:43.842718 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/parser.py
+-rw-r--r--   0        0        0     3112 2023-06-29 16:11:53.517604 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/config.py
+-rw-r--r--   0        0        0      699 2023-06-29 13:51:51.654691 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/exceptions.py
+-rw-r--r--   0        0        0       55 2023-06-29 16:07:27.581298 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/__init__.py
+-rw-r--r--   0        0        0     6080 2023-06-29 12:45:06.228269 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/csv.py
+-rw-r--r--   0        0        0     3332 2023-06-29 20:09:30.754509 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/general.py
+-rw-r--r--   0        0        0     1374 2023-06-29 20:39:58.278826 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/utils.py
+-rw-r--r--   0        0        0     7619 2023-06-29 13:46:46.600190 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/xlsx.py
+-rw-r--r--   0        0        0      194 2023-06-28 19:49:38.153124 geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/types.py
+-rw-r--r--   0        0        0     1805 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev1/setup.py
+-rw-r--r--   0        0        0     1587 1970-01-01 00:00:00.000000 geneweaver_client-0.0.1a0.dev1/PKG-INFO
```

### Comparing `geneweaver_client-0.0.1a0.dev0/LICENSE` & `geneweaver_client-0.0.1a0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/pyproject.toml` & `geneweaver_client-0.0.1a0.dev1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-client"
-version = "0.0.1a0-dev"
+version = "0.0.1a0-dev1"
 description = "A Python Client for the Geneweaver API"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://bergsalex.github.io/geneweaver-docs/"
 repository = "https://bitbucket.org/jacksonlaboratory/geneweaver-client/"
 packages = [
```

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/genesets.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/genesets.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/legacy.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/legacy.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/api/utils.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/api/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/cli/main.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/main.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/cli/parser.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/cli/parser.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/config.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/config.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/exceptions.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/csv.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/csv.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/general.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/general.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/utils.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_client-0.0.1a0.dev0/src/geneweaver/client/parser/xlsx.py` & `geneweaver_client-0.0.1a0.dev1/src/geneweaver/client/parser/xlsx.py`

 * *Files identical despite different names*

