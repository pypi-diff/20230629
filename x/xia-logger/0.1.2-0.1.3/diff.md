# Comparing `tmp/xia_logger-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 147077 bytes, number of entries: 7
--rw-r--r--  2.0 unx      160 b- defN 23-Jun-26 13:25 xia_logger/__init__.py
--rw-r--r--  2.0 unx   393216 b- defN 23-Jun-26 13:27 xia_logger/logger.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:27 xia_logger-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-26 13:27 xia_logger-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:27 xia_logger-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 13:27 xia_logger-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      576 b- defN 23-Jun-26 13:27 xia_logger-0.1.2.dist-info/RECORD
-7 files, 394939 bytes uncompressed, 146051 bytes compressed:  63.0%
+Zip file size: 4879 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      159 b- defN 23-Jun-29 20:49 xia_logger/__init__.py
+-rw-r--r--  2.0 unx    11135 b- defN 23-Jun-29 17:32 xia_logger/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      559 b- defN 23-Jun-29 20:54 xia_logger-0.1.3.dist-info/RECORD
+7 files, 12840 bytes uncompressed, 3885 bytes compressed:  69.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger/__init__.py
 Comment: 
 
-Filename: xia_logger/logger.cp39-win_amd64.pyd
+Filename: xia_logger/logger.py
 Comment: 
 
-Filename: xia_logger-0.1.2.dist-info/LICENSE.txt
+Filename: xia_logger-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger-0.1.2.dist-info/METADATA
+Filename: xia_logger-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger-0.1.2.dist-info/WHEEL
+Filename: xia_logger-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger-0.1.2.dist-info/top_level.txt
+Filename: xia_logger-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger-0.1.2.dist-info/RECORD
+Filename: xia_logger-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger.logger import Logger, HttpLogger, JsonLogger, DataLog
 
 __all__ = [
     "Logger", "HttpLogger", "JsonLogger", "DataLog"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_logger-0.1.2.dist-info/METADATA` & `xia_logger-0.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-logger
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-logger/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-logger/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

