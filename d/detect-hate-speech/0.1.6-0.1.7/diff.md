# Comparing `tmp/detect_hate_speech-0.1.6.tar.gz` & `tmp/detect_hate_speech-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "detect_hate_speech-0.1.6.tar", max compression
+gzip compressed data, was "detect_hate_speech-0.1.7.tar", max compression
```

## Comparing `detect_hate_speech-0.1.6.tar` & `detect_hate_speech-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-06-29 04:38:57.578859 detect_hate_speech-0.1.6/LICENSE
--rw-r--r--   0        0        0     3958 2023-06-29 04:38:57.578859 detect_hate_speech-0.1.6/README.md
--rw-r--r--   0        0        0      783 2023-06-29 04:38:57.627858 detect_hate_speech-0.1.6/detect_hate_speech/main.py
--rw-r--r--   0        0        0     4470 2023-06-29 04:38:57.627858 detect_hate_speech-0.1.6/detect_hate_speech/utils.py
--rw-r--r--   0        0        0      332 2023-06-29 04:39:09.022816 detect_hate_speech-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 detect_hate_speech-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-29 06:20:41.530578 detect_hate_speech-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3958 2023-06-29 06:20:41.530578 detect_hate_speech-0.1.7/README.md
+-rw-r--r--   0        0        0      783 2023-06-29 06:20:41.579578 detect_hate_speech-0.1.7/detect_hate_speech/main.py
+-rw-r--r--   0        0        0     4470 2023-06-29 06:20:41.579578 detect_hate_speech-0.1.7/detect_hate_speech/utils.py
+-rw-r--r--   0        0        0      332 2023-06-29 06:20:53.870436 detect_hate_speech-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4458 1970-01-01 00:00:00.000000 detect_hate_speech-0.1.7/PKG-INFO
```

### Comparing `detect_hate_speech-0.1.6/LICENSE` & `detect_hate_speech-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `detect_hate_speech-0.1.6/README.md` & `detect_hate_speech-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `detect_hate_speech-0.1.6/detect_hate_speech/main.py` & `detect_hate_speech-0.1.7/detect_hate_speech/main.py`

 * *Files identical despite different names*

### Comparing `detect_hate_speech-0.1.6/detect_hate_speech/utils.py` & `detect_hate_speech-0.1.7/detect_hate_speech/utils.py`

 * *Files identical despite different names*

### Comparing `detect_hate_speech-0.1.6/PKG-INFO` & `detect_hate_speech-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: detect-hate-speech
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Amanda Nobre
 Author-email: amandapnobre@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

