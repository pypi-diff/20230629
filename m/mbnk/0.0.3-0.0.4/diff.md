# Comparing `tmp/mbnk-0.0.3.tar.gz` & `tmp/mbnk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbnk-0.0.3.tar", max compression
+gzip compressed data, was "mbnk-0.0.4.tar", max compression
```

## Comparing `mbnk-0.0.3.tar` & `mbnk-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,18 @@
--rw-r--r--   0        0        0      692 2023-05-05 16:01:16.349631 mbnk-0.0.3/README.md
--rw-r--r--   0        0        0      274 2023-05-05 15:36:44.885277 mbnk-0.0.3/mbnk/__init__.py
--rw-r--r--   0        0        0     5766 2023-05-05 15:32:04.238740 mbnk-0.0.3/mbnk/__main__.py
--rw-r--r--   0        0        0       26 2023-05-05 14:23:55.019901 mbnk-0.0.3/mbnk/decorators/__init__.py
--rw-r--r--   0        0        0      182 2023-05-05 14:36:37.206163 mbnk-0.0.3/mbnk/decorators/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1529 2023-05-05 14:44:43.017405 mbnk-0.0.3/mbnk/decorators/__pycache__/decorators.cpython-38.pyc
--rw-r--r--   0        0        0     1469 2023-05-05 15:32:04.446739 mbnk-0.0.3/mbnk/decorators/decorators.py
--rw-r--r--   0        0        0       26 2023-05-05 14:20:51.246996 mbnk-0.0.3/mbnk/exceptions/__init__.py
--rw-r--r--   0        0        0      182 2023-05-05 14:36:37.210162 mbnk-0.0.3/mbnk/exceptions/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      425 2023-05-05 14:44:06.921880 mbnk-0.0.3/mbnk/exceptions/__pycache__/exceptions.cpython-38.pyc
--rw-r--r--   0        0        0      101 2023-05-05 14:44:02.081946 mbnk-0.0.3/mbnk/exceptions/exceptions.py
--rw-r--r--   0        0        0       24 2023-05-05 14:27:50.660629 mbnk-0.0.3/mbnk/instances/__init__.py
--rw-r--r--   0        0        0      180 2023-05-05 14:36:37.302160 mbnk-0.0.3/mbnk/instances/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1764 2023-05-05 15:25:26.044824 mbnk-0.0.3/mbnk/instances/__pycache__/instances.cpython-38.pyc
--rw-r--r--   0        0        0     1027 2023-05-05 15:24:33.653100 mbnk-0.0.3/mbnk/instances/instances.py
--rw-r--r--   0        0        0       25 2023-05-05 14:29:09.728795 mbnk-0.0.3/mbnk/responses/__init__.py
--rw-r--r--   0        0        0      180 2023-05-05 14:36:37.302160 mbnk-0.0.3/mbnk/responses/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1234 2023-05-05 15:21:17.118137 mbnk-0.0.3/mbnk/responses/__pycache__/responses.cpython-38.pyc
--rw-r--r--   0        0        0      554 2023-05-05 15:32:04.350739 mbnk-0.0.3/mbnk/responses/responses.py
--rw-r--r--   0        0        0      104 2023-05-05 14:19:51.878618 mbnk-0.0.3/mbnk/utils/__init__.py
--rw-r--r--   0        0        0      246 2023-05-05 14:36:37.218162 mbnk-0.0.3/mbnk/utils/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      430 2023-05-05 14:36:37.218162 mbnk-0.0.3/mbnk/utils/__pycache__/builders.cpython-38.pyc
--rw-r--r--   0        0        0      404 2023-05-05 14:44:59.013201 mbnk-0.0.3/mbnk/utils/__pycache__/is_exception.cpython-38.pyc
--rw-r--r--   0        0        0      399 2023-05-05 14:36:37.218162 mbnk-0.0.3/mbnk/utils/__pycache__/to_camel_case.cpython-38.pyc
--rw-r--r--   0        0        0      262 2023-05-05 15:32:04.398739 mbnk-0.0.3/mbnk/utils/builders.py
--rw-r--r--   0        0        0      220 2023-05-05 14:44:57.937215 mbnk-0.0.3/mbnk/utils/is_exception.py
--rw-r--r--   0        0        0      140 2023-05-05 14:18:28.037997 mbnk-0.0.3/mbnk/utils/to_camel_case.py
--rw-r--r--   0        0        0      307 2023-05-05 16:01:32.433547 mbnk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 mbnk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      692 2023-05-05 16:01:16.349631 mbnk-0.0.4/README.md
+-rw-r--r--   0        0        0      290 2023-06-29 11:51:13.889758 mbnk-0.0.4/mbnk/__init__.py
+-rw-r--r--   0        0        0      108 2023-06-26 17:49:44.968379 mbnk-0.0.4/mbnk/asyncio/__init__.py
+-rw-r--r--   0        0        0     5334 2023-06-29 11:43:17.215861 mbnk-0.0.4/mbnk/asyncio/mbnk.py
+-rw-r--r--   0        0        0     2014 2023-06-26 20:24:53.337731 mbnk-0.0.4/mbnk/decorators.py
+-rw-r--r--   0        0        0     1031 2023-06-26 19:21:25.551426 mbnk-0.0.4/mbnk/enums.py
+-rw-r--r--   0        0        0        0 2023-06-26 17:26:19.588213 mbnk-0.0.4/mbnk/exceptions.py
+-rw-r--r--   0        0        0       24 2023-05-05 14:27:50.660629 mbnk-0.0.4/mbnk/instances/__init__.py
+-rw-r--r--   0        0        0     1027 2023-05-05 15:24:33.653100 mbnk-0.0.4/mbnk/instances/instances.py
+-rw-r--r--   0        0        0     6498 2023-06-26 17:52:49.728848 mbnk-0.0.4/mbnk/monobank.py
+-rw-r--r--   0        0        0      554 2023-05-05 15:32:04.350739 mbnk-0.0.4/mbnk/responses.py
+-rw-r--r--   0        0        0      104 2023-05-05 14:19:51.878618 mbnk-0.0.4/mbnk/utils/__init__.py
+-rw-r--r--   0        0        0      276 2023-06-26 19:48:53.018019 mbnk-0.0.4/mbnk/utils/builders.py
+-rw-r--r--   0        0        0      152 2023-06-26 16:15:25.376467 mbnk-0.0.4/mbnk/utils/is_exception.py
+-rw-r--r--   0        0        0      141 2023-06-26 16:51:30.107547 mbnk-0.0.4/mbnk/utils/to_camel_case.py
+-rw-r--r--   0        0        0      505 2023-05-01 23:52:09.567523 mbnk-0.0.4/mbnk/utils/webhook_authentication.py
+-rw-r--r--   0        0        0      313 2023-06-29 11:50:31.722997 mbnk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 mbnk-0.0.4/PKG-INFO
```

### Comparing `mbnk-0.0.3/README.md` & `mbnk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.3/mbnk/instances/instances.py` & `mbnk-0.0.4/mbnk/instances/instances.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.3/mbnk/responses/responses.py` & `mbnk-0.0.4/mbnk/responses.py`

 * *Files identical despite different names*

### Comparing `mbnk-0.0.3/PKG-INFO` & `mbnk-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mbnk
-Version: 0.0.3
-Summary: Sync version monobank api
+Version: 0.0.4
+Summary: Sync/Async version monobank api
 License: MIT
 Author: yeghorkikhai
 Author-email: yeghorkikhai@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

