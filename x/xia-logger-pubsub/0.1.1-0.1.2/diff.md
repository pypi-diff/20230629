# Comparing `tmp/xia_logger_pubsub-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_pubsub-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 142053 bytes, number of entries: 7
--rw-r--r--  2.0 unx      107 b- defN 23-Jun-26 17:55 xia_logger_pubsub/__init__.py
--rw-r--r--  2.0 unx   361472 b- defN 23-Jun-26 17:58 xia_logger_pubsub/logger.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:58 xia_logger_pubsub-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      701 b- defN 23-Jun-26 17:58 xia_logger_pubsub-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:58 xia_logger_pubsub-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-26 17:58 xia_logger_pubsub-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      625 b- defN 23-Jun-26 17:58 xia_logger_pubsub-0.1.1.dist-info/RECORD
-7 files, 363173 bytes uncompressed, 140929 bytes compressed:  61.2%
+Zip file size: 3989 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      106 b- defN 23-Jun-29 20:50 xia_logger_pubsub/__init__.py
+-rw-r--r--  2.0 unx     8477 b- defN 23-Jun-29 20:12 xia_logger_pubsub/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      701 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      607 b- defN 23-Jun-29 20:55 xia_logger_pubsub-0.1.2.dist-info/RECORD
+7 files, 10159 bytes uncompressed, 2897 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_pubsub/__init__.py
 Comment: 
 
-Filename: xia_logger_pubsub/logger.cp39-win_amd64.pyd
+Filename: xia_logger_pubsub/logger.py
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.1.dist-info/LICENSE.txt
+Filename: xia_logger_pubsub-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.1.dist-info/METADATA
+Filename: xia_logger_pubsub-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.1.dist-info/WHEEL
+Filename: xia_logger_pubsub-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.1.dist-info/top_level.txt
+Filename: xia_logger_pubsub-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_pubsub-0.1.1.dist-info/RECORD
+Filename: xia_logger_pubsub-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_pubsub/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_pubsub.logger import PubsubLogger
 
 __all__ = [
     "PubsubLogger"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_logger_pubsub-0.1.1.dist-info/METADATA` & `xia_logger_pubsub-0.1.2.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-logger-pubsub
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-logger-pubsub/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-logger-pubsub/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

