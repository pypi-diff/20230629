# Comparing `tmp/ag_llama_api-0.0.6.tar.gz` & `tmp/ag_llama_api-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama_api-0.0.6.tar", last modified: Thu Jun 29 13:54:38 2023, max compression
+gzip compressed data, was "dist\ag_llama_api-0.0.7.tar", last modified: Thu Jun 29 13:58:49 2023, max compression
```

## Comparing `ag_llama_api-0.0.6.tar` & `ag_llama_api-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 13:54:38.356058 ag_llama_api-0.0.6/
--rw-rw-rw-   0        0        0      764 2023-06-29 13:54:38.355065 ag_llama_api-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 13:54:38.334728 ag_llama_api-0.0.6/ag_llama_api/
--rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.6/ag_llama_api/__init__.py
--rw-rw-rw-   0        0        0     9159 2023-06-29 13:31:25.000000 ag_llama_api-0.0.6/ag_llama_api/__main__.py
--rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/ag_llama_api/choice.py
--rw-rw-rw-   0        0        0    13780 2023-06-28 17:04:18.000000 ag_llama_api-0.0.6/ag_llama_api/model.py
--rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/ag_llama_api/tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:54:38.344154 ag_llama_api-0.0.6/ag_llama_api.egg-info/
--rw-rw-rw-   0        0        0      764 2023-06-29 13:54:38.000000 ag_llama_api-0.0.6/ag_llama_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-06-29 13:54:38.000000 ag_llama_api-0.0.6/ag_llama_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 13:54:38.000000 ag_llama_api-0.0.6/ag_llama_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      290 2023-06-29 13:54:38.000000 ag_llama_api-0.0.6/ag_llama_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-29 13:54:38.000000 ag_llama_api-0.0.6/ag_llama_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 13:54:38.356559 ag_llama_api-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2567 2023-06-29 13:52:31.000000 ag_llama_api-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:54:38.349608 ag_llama_api-0.0.6/tests/
--rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api-0.0.6/tests/test_choice.py
--rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/tests/test_model.py
--rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/tests/test_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-06-29 13:54:38.353082 ag_llama_api-0.0.6/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api-0.0.6/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:58:49.885042 ag_llama_api-0.0.7/
+-rw-rw-rw-   0        0        0      764 2023-06-29 13:58:49.883584 ag_llama_api-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 13:58:49.863218 ag_llama_api-0.0.7/ag_llama_api/
+-rw-rw-rw-   0        0        0     2186 2023-06-27 12:34:01.000000 ag_llama_api-0.0.7/ag_llama_api/__init__.py
+-rw-rw-rw-   0        0        0     9143 2023-06-29 13:58:28.000000 ag_llama_api-0.0.7/ag_llama_api/__main__.py
+-rw-rw-rw-   0        0        0     2011 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/ag_llama_api/choice.py
+-rw-rw-rw-   0        0        0    13780 2023-06-28 17:04:18.000000 ag_llama_api-0.0.7/ag_llama_api/model.py
+-rw-rw-rw-   0        0        0     1850 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/ag_llama_api/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:58:49.872641 ag_llama_api-0.0.7/ag_llama_api.egg-info/
+-rw-rw-rw-   0        0        0      764 2023-06-29 13:58:49.000000 ag_llama_api-0.0.7/ag_llama_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-06-29 13:58:49.000000 ag_llama_api-0.0.7/ag_llama_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 13:58:49.000000 ag_llama_api-0.0.7/ag_llama_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      290 2023-06-29 13:58:49.000000 ag_llama_api-0.0.7/ag_llama_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-29 13:58:49.000000 ag_llama_api-0.0.7/ag_llama_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 13:58:49.885042 ag_llama_api-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2567 2023-06-29 13:52:31.000000 ag_llama_api-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:58:49.877600 ag_llama_api-0.0.7/tests/
+-rw-rw-rw-   0        0        0     1121 2023-06-28 17:09:17.000000 ag_llama_api-0.0.7/tests/test_choice.py
+-rw-rw-rw-   0        0        0     2982 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/tests/test_model.py
+-rw-rw-rw-   0        0        0     1945 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/tests/test_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 13:58:49.881569 ag_llama_api-0.0.7/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama_api-0.0.7/utils/render.py
```

### Comparing `ag_llama_api-0.0.6/PKG-INFO` & `ag_llama_api-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama_api
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_api Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api-0.0.6/ag_llama_api/__init__.py` & `ag_llama_api-0.0.7/ag_llama_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/ag_llama_api/__main__.py` & `ag_llama_api-0.0.7/ag_llama_api/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,13 +278,12 @@
         app,
         host=HOST,
         port=PORT,
         threads=SERVER_THREADS,
         ident=SERVER_IDENTITY,
         connection_limit=SERVER_CONNECTION_LIMIT,
         channel_timeout=SERVER_CHANNEL_TIMEOUT,
-        backlog
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ag_llama_api-0.0.6/ag_llama_api/choice.py` & `ag_llama_api-0.0.7/ag_llama_api/choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/ag_llama_api/model.py` & `ag_llama_api-0.0.7/ag_llama_api/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/ag_llama_api/tokenizer.py` & `ag_llama_api-0.0.7/ag_llama_api/tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/ag_llama_api.egg-info/PKG-INFO` & `ag_llama_api-0.0.7/ag_llama_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama-api
-Version: 0.0.6
+Version: 0.0.7
 Summary: ag_llama_api Test Package for Somthing
 Author: AA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ag_llama_api-0.0.6/setup.py` & `ag_llama_api-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/tests/test_choice.py` & `ag_llama_api-0.0.7/tests/test_choice.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/tests/test_model.py` & `ag_llama_api-0.0.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/tests/test_tokenizer.py` & `ag_llama_api-0.0.7/tests/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/utils/download.py` & `ag_llama_api-0.0.7/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama_api-0.0.6/utils/render.py` & `ag_llama_api-0.0.7/utils/render.py`

 * *Files identical despite different names*

