# Comparing `tmp/aioredisorm-0.1.1.tar.gz` & `tmp/aioredisorm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioredisorm-0.1.1.tar", max compression
+gzip compressed data, was "aioredisorm-0.1.2.tar", max compression
```

## Comparing `aioredisorm-0.1.1.tar` & `aioredisorm-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1082 2023-06-27 15:42:37.968974 aioredisorm-0.1.1/LICENSE
--rw-r--r--   0        0        0       49 2023-06-27 14:42:54.674318 aioredisorm-0.1.1/aioredisorm/__init__.py
--rw-r--r--   0        0        0     4413 2023-06-27 15:33:22.348494 aioredisorm-0.1.1/aioredisorm/aioredisorm.py
--rw-r--r--   0        0        0      625 2023-06-29 06:32:18.798652 aioredisorm-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      688 2023-06-29 06:34:42.245121 aioredisorm-0.1.1/setup.py
--rw-r--r--   0        0        0      568 2023-06-29 06:34:42.245376 aioredisorm-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-27 15:42:37.968974 aioredisorm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2487 2023-06-27 15:42:37.968974 aioredisorm-0.1.2/README.md
+-rw-r--r--   0        0        0       49 2023-06-27 14:42:54.674318 aioredisorm-0.1.2/aioredisorm/__init__.py
+-rw-r--r--   0        0        0     4413 2023-06-27 15:33:22.348494 aioredisorm-0.1.2/aioredisorm/aioredisorm.py
+-rw-r--r--   0        0        0      643 2023-06-29 06:37:23.917174 aioredisorm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3367 2023-06-29 06:37:31.691780 aioredisorm-0.1.2/setup.py
+-rw-r--r--   0        0        0     3094 2023-06-29 06:37:31.692093 aioredisorm-0.1.2/PKG-INFO
```

### Comparing `aioredisorm-0.1.1/LICENSE` & `aioredisorm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aioredisorm-0.1.1/aioredisorm/aioredisorm.py` & `aioredisorm-0.1.2/aioredisorm/aioredisorm.py`

 * *Files identical despite different names*

### Comparing `aioredisorm-0.1.1/pyproject.toml` & `aioredisorm-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "aioredisorm"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python class for interacting with Redis using asyncio and aioredis."
 authors = ["fadedreams7 <fadedreams7@gmail.com>"]
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.3"
 aioredis = "^2.0.1"
 
 [tool.poetry.dev-dependencies]
@@ -20,9 +21,9 @@
 classifiers = [
     "Operating System :: OS Independent",
     "Environment :: Console",
     "Topic :: Utilities"
 ]
 
 [tool.poetry.urls]
-repository = "https://github.com/your-username/aioredisorm"
+repository = "https://github.com/fadedreams/aioredisorm"
```

