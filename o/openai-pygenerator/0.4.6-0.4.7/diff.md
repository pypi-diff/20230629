# Comparing `tmp/openai-pygenerator-0.4.6.tar.gz` & `tmp/openai-pygenerator-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-pygenerator-0.4.6.tar", last modified: Tue Jun 20 10:07:20 2023, max compression
+gzip compressed data, was "openai-pygenerator-0.4.7.tar", last modified: Thu Jun 29 19:34:55 2023, max compression
```

## Comparing `openai-pygenerator-0.4.6.tar` & `openai-pygenerator-0.4.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.770730 openai-pygenerator-0.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/mypy-tests.ini
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-20 10:07:20.778730 openai-pygenerator-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.770730 openai-pygenerator-0.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/src/openai_pygenerator/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/src/openai_pygenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/src/openai_pygenerator/example.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/src/openai_pygenerator/openai_pygenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/src/openai_pygenerator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 10:07:20.000000 openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:07:20.774731 openai-pygenerator-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-20 10:07:04.000000 openai-pygenerator-0.4.6/tests/test_gpt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.837877 openai-pygenerator-0.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.833877 openai-pygenerator-0.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.833877 openai-pygenerator-0.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-29 19:34:55.837877 openai-pygenerator-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/mypy-tests.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-29 19:34:55.837877 openai-pygenerator-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.833877 openai-pygenerator-0.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.833877 openai-pygenerator-0.4.7/src/openai_pygenerator/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/src/openai_pygenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/src/openai_pygenerator/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/src/openai_pygenerator/openai_pygenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/src/openai_pygenerator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.837877 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 19:34:55.000000 openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:34:55.837877 openai-pygenerator-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-06-29 19:34:45.000000 openai-pygenerator-0.4.7/tests/test_gpt.py
```

### Comparing `openai-pygenerator-0.4.6/.github/workflows/python-package.yml` & `openai-pygenerator-0.4.7/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/.github/workflows/python-publish.yml` & `openai-pygenerator-0.4.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/.pre-commit-config.yaml` & `openai-pygenerator-0.4.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/.pylintrc` & `openai-pygenerator-0.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/LICENSE.txt` & `openai-pygenerator-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/PKG-INFO` & `openai-pygenerator-0.4.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.6
+Version: 0.4.7
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # openai-pygenerator
 
-[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-generator/actions/workflows/continouos-integration.yml)
+[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/phelps-sg/openai-pygenerator)
 ![GitHub](https://img.shields.io/github/license/phelps-sg/openai-pygenerator?color=blue)
 
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
 
 ## Installation
```

### Comparing `openai-pygenerator-0.4.6/README.md` & `openai-pygenerator-0.4.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # openai-pygenerator
 
-[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-generator/actions/workflows/continouos-integration.yml)
+[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/phelps-sg/openai-pygenerator)
 ![GitHub](https://img.shields.io/github/license/phelps-sg/openai-pygenerator?color=blue)
 
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
 
 ## Installation
```

### Comparing `openai-pygenerator-0.4.6/pyproject.toml` & `openai-pygenerator-0.4.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/src/openai_pygenerator/example.py` & `openai-pygenerator-0.4.7/src/openai_pygenerator/example.py`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/src/openai_pygenerator/openai_pygenerator.py` & `openai-pygenerator-0.4.7/src/openai_pygenerator/openai_pygenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import time
 from enum import Enum, auto
 from typing import Callable, Dict, Iterable, Iterator, List, NewType, Optional, TypeVar
 
 import openai
 from openai.error import APIError, RateLimitError, ServiceUnavailableError
+from urllib3.exceptions import ReadTimeoutError
 
 Completion = Dict[str, str]
 Seconds = NewType("Seconds", int)
 Completions = Iterator[Completion]
 History = Iterable[Completion]
 Completer = Callable[[History, int], Completions]
 T = TypeVar("T")
@@ -84,15 +85,15 @@
             max_tokens=max_tokens,
             n=n,
             temperature=temperature,
         )
         logger.debug("response = %s", result)
         for choice in result.choices:
             yield choice.message
-    except (RateLimitError, APIError, ServiceUnavailableError) as err:
+    except (ReadTimeoutError, RateLimitError, APIError, ServiceUnavailableError) as err:
         if isinstance(err, APIError) and not (err.http_status in [524, 502]):
             raise
         logger.warning("Error returned from openai API: %s", err)
         logger.debug("retries = %d", retries)
         if retries < max_retries:
             logger.info("Retrying... ")
             time.sleep(retry_base + retry_exponent**retries)
```

### Comparing `openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/PKG-INFO` & `openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openai-pygenerator
-Version: 0.4.6
+Version: 0.4.7
 Summary: Simple generator wrapper for OpenAI Python API with retry
 Author-email: Steve Phelps <sphelps@sphelps.net>
 Project-URL: Homepage, https://github.com/phelps-sg/openai-pygenerator
 Project-URL: Bug Tracker, https://github.com/phelps-sg/openai-pygenerator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # openai-pygenerator
 
-[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-generator/actions/workflows/continouos-integration.yml)
+[![GitHub Workflow Status](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml/badge.svg)](https://github.com/phelps-sg/openai-pygenerator/actions/workflows/python-package.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/phelps-sg/openai-pygenerator)
 ![GitHub](https://img.shields.io/github/license/phelps-sg/openai-pygenerator?color=blue)
 
 This is a simple wrapper around the OpenAI Python API which provides
 type annotations, retry functionality and a generator over completions.
 
 ## Installation
```

### Comparing `openai-pygenerator-0.4.6/src/openai_pygenerator.egg-info/SOURCES.txt` & `openai-pygenerator-0.4.7/src/openai_pygenerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai-pygenerator-0.4.6/tests/test_gpt.py` & `openai-pygenerator-0.4.7/tests/test_gpt.py`

 * *Files identical despite different names*

