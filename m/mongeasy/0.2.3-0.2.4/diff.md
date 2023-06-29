# Comparing `tmp/mongeasy-0.2.3.tar.gz` & `tmp/mongeasy-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongeasy-0.2.3.tar", last modified: Thu Jun 29 09:29:07 2023, max compression
+gzip compressed data, was "mongeasy-0.2.4.tar", last modified: Thu Jun 29 09:40:08 2023, max compression
```

## Comparing `mongeasy-0.2.3.tar` & `mongeasy-0.2.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.272565 mongeasy-0.2.3/
--rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.3/LICENSE
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.232560 mongeasy-0.2.3/Mongeasy.egg-info/
--rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 09:29:07.000000 mongeasy-0.2.3/Mongeasy.egg-info/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)     1018 2023-06-29 09:29:07.000000 mongeasy-0.2.3/Mongeasy.egg-info/SOURCES.txt
--rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-29 09:29:07.000000 mongeasy-0.2.3/Mongeasy.egg-info/dependency_links.txt
--rw-r--r--   0 javv       (501) staff       (20)      822 2023-06-29 09:29:07.000000 mongeasy-0.2.3/Mongeasy.egg-info/requires.txt
--rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-29 09:29:07.000000 mongeasy-0.2.3/Mongeasy.egg-info/top_level.txt
--rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 09:29:07.272175 mongeasy-0.2.3/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)    21636 2023-06-29 09:27:38.000000 mongeasy-0.2.3/README.md
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.249321 mongeasy-0.2.3/mongeasy/
--rw-r--r--   0 javv       (501) staff       (20)      623 2023-06-22 13:22:39.000000 mongeasy-0.2.3/mongeasy/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/base_dict.py
--rw-r--r--   0 javv       (501) staff       (20)     3685 2023-06-26 05:55:43.000000 mongeasy-0.2.3/mongeasy/connection.py
--rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.3/mongeasy/core.py
--rw-r--r--   0 javv       (501) staff       (20)    14298 2023-06-29 07:09:12.000000 mongeasy-0.2.3/mongeasy/document.py
--rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.3/mongeasy/dynamics.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.260257 mongeasy-0.2.3/mongeasy/examples/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/examples/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/exceptions.py
--rw-r--r--   0 javv       (501) staff       (20)     1876 2023-06-29 07:08:47.000000 mongeasy-0.2.3/mongeasy/lazy_resultlist.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.262410 mongeasy-0.2.3/mongeasy/plugins/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.3/mongeasy/plugins/registry.py
--rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/resultlist.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.263849 mongeasy-0.2.3/mongeasy/utils/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/utils/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.3/mongeasy/utils/utils.py
--rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.3/pyproject.toml
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.269915 mongeasy-0.2.3/sample_plugins/
--rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/connection_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/delete_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/init_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/pydantic_validator.py
--rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/query_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/save_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.3/sample_plugins/validator_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-29 09:29:07.272650 mongeasy-0.2.3/setup.cfg
--rw-r--r--   0 javv       (501) staff       (20)     1206 2023-06-29 09:28:55.000000 mongeasy-0.2.3/setup.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:29:07.271585 mongeasy-0.2.3/tests/
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.3/tests/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)    14505 2023-06-29 07:29:00.000000 mongeasy-0.2.3/tests/test_mongeasy.py
--rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.3/tests/test_plugins.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.241855 mongeasy-0.2.4/
+-rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.4/LICENSE
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.221783 mongeasy-0.2.4/Mongeasy.egg-info/
+-rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 09:40:08.000000 mongeasy-0.2.4/Mongeasy.egg-info/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)     1018 2023-06-29 09:40:08.000000 mongeasy-0.2.4/Mongeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-29 09:40:08.000000 mongeasy-0.2.4/Mongeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 javv       (501) staff       (20)      821 2023-06-29 09:40:08.000000 mongeasy-0.2.4/Mongeasy.egg-info/requires.txt
+-rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-29 09:40:08.000000 mongeasy-0.2.4/Mongeasy.egg-info/top_level.txt
+-rw-r--r--   0 javv       (501) staff       (20)    22372 2023-06-29 09:40:08.241536 mongeasy-0.2.4/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)    21636 2023-06-29 09:39:26.000000 mongeasy-0.2.4/README.md
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.229497 mongeasy-0.2.4/mongeasy/
+-rw-r--r--   0 javv       (501) staff       (20)      623 2023-06-22 13:22:39.000000 mongeasy-0.2.4/mongeasy/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/base_dict.py
+-rw-r--r--   0 javv       (501) staff       (20)     3685 2023-06-26 05:55:43.000000 mongeasy-0.2.4/mongeasy/connection.py
+-rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.4/mongeasy/core.py
+-rw-r--r--   0 javv       (501) staff       (20)    14298 2023-06-29 07:09:12.000000 mongeasy-0.2.4/mongeasy/document.py
+-rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.4/mongeasy/dynamics.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.230960 mongeasy-0.2.4/mongeasy/examples/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/examples/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/exceptions.py
+-rw-r--r--   0 javv       (501) staff       (20)     1876 2023-06-29 07:08:47.000000 mongeasy-0.2.4/mongeasy/lazy_resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.232257 mongeasy-0.2.4/mongeasy/plugins/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.4/mongeasy/plugins/registry.py
+-rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.233437 mongeasy-0.2.4/mongeasy/utils/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/utils/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.4/mongeasy/utils/utils.py
+-rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.4/pyproject.toml
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.238391 mongeasy-0.2.4/sample_plugins/
+-rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/connection_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/delete_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/init_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/pydantic_validator.py
+-rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/query_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/save_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.4/sample_plugins/validator_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-29 09:40:08.241943 mongeasy-0.2.4/setup.cfg
+-rw-r--r--   0 javv       (501) staff       (20)     1206 2023-06-29 09:39:18.000000 mongeasy-0.2.4/setup.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-29 09:40:08.240859 mongeasy-0.2.4/tests/
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.4/tests/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)    14505 2023-06-29 07:29:00.000000 mongeasy-0.2.4/tests/test_mongeasy.py
+-rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.4/tests/test_plugins.py
```

### Comparing `mongeasy-0.2.3/LICENSE` & `mongeasy-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/Mongeasy.egg-info/PKG-INFO` & `mongeasy-0.2.4/Mongeasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.3?
+## What's new in version 0.2.4?
 ### Support for lazy queries
 The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
 User = create_document_class('User', 'users')
```

### Comparing `mongeasy-0.2.3/Mongeasy.egg-info/SOURCES.txt` & `mongeasy-0.2.4/Mongeasy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/Mongeasy.egg-info/requires.txt` & `mongeasy-0.2.4/Mongeasy.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 docutils==0.19
 ghp-import==2.1.0
 idna==3.4
 import-string==0.1.0
 importlib-metadata==6.4.1
 iniconfig==2.0.0
 jaraco.classes==3.2.3
-Jinja2==2.11.3
 keyring==23.13.1
 Markdown==3.3.7
 markdown-it-py==2.2.0
 MarkupSafe==2.1.3
 mdurl==0.1.2
 mergedeep==1.3.4
 mkdocs==1.4.2
 more-itertools==9.1.0
 packaging==23.1
 pkginfo==1.9.6
+pluggy==1.2.0
 pydantic==1.10.9
 Pygments==2.15.0
 pymongo==4.3.3
 pyparsing==3.0.9
 pyproject_hooks==1.0.0
 pytest==7.3.1
 python-dateutil==2.8.2
```

### Comparing `mongeasy-0.2.3/PKG-INFO` & `mongeasy-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.3
+Version: 0.2.4
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.3?
+## What's new in version 0.2.4?
 ### Support for lazy queries
 The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
 User = create_document_class('User', 'users')
```

### Comparing `mongeasy-0.2.3/README.md` & `mongeasy-0.2.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ```bash
 pip install mongeasy
 ```
 
 ## Documentation
 The documentation can be found at [https://mongeasy.readthedocs.io](https://mongeasy.readthedocs.io)
 
-## What's new in version 0.2.3?
+## What's new in version 0.2.4?
 ### Support for lazy queries
 The find method now supports a lazy flag (defeault set to False) which when set to True, returns a lazy query object instead of a result list. This is useful when you want to iterate over a large number of documents without loading them all into memory at once.
 
 ```python
 from mongeasy import create_document_class
 
 User = create_document_class('User', 'users')
```

### Comparing `mongeasy-0.2.3/mongeasy/__init__.py` & `mongeasy-0.2.4/mongeasy/__init__.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/base_dict.py` & `mongeasy-0.2.4/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/connection.py` & `mongeasy-0.2.4/mongeasy/connection.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/core.py` & `mongeasy-0.2.4/mongeasy/core.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/document.py` & `mongeasy-0.2.4/mongeasy/document.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/dynamics.py` & `mongeasy-0.2.4/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/exceptions.py` & `mongeasy-0.2.4/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/lazy_resultlist.py` & `mongeasy-0.2.4/mongeasy/lazy_resultlist.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/plugins/registry.py` & `mongeasy-0.2.4/mongeasy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/resultlist.py` & `mongeasy-0.2.4/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/mongeasy/utils/utils.py` & `mongeasy-0.2.4/mongeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/sample_plugins/__init__.py` & `mongeasy-0.2.4/sample_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/sample_plugins/pydantic_validator.py` & `mongeasy-0.2.4/sample_plugins/pydantic_validator.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/setup.py` & `mongeasy-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="mongeasy",
-    version="0.2.3",
+    version="0.2.4",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `mongeasy-0.2.3/tests/test_mongeasy.py` & `mongeasy-0.2.4/tests/test_mongeasy.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.3/tests/test_plugins.py` & `mongeasy-0.2.4/tests/test_plugins.py`

 * *Files identical despite different names*

