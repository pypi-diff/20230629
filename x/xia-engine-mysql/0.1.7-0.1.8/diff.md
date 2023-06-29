# Comparing `tmp/xia_engine_mysql-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_mysql-0.1.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 137362 bytes, number of entries: 7
--rw-r--r--  2.0 unx      144 b- defN 23-Jun-26 16:48 xia_engine_mysql/__init__.py
--rw-r--r--  2.0 unx   349184 b- defN 23-Jun-26 16:50 xia_engine_mysql/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 16:50 xia_engine_mysql-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      715 b- defN 23-Jun-26 16:50 xia_engine_mysql-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 16:50 xia_engine_mysql-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 16:50 xia_engine_mysql-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      618 b- defN 23-Jun-26 16:50 xia_engine_mysql-0.1.7.dist-info/RECORD
-7 files, 350928 bytes uncompressed, 136252 bytes compressed:  61.2%
+Zip file size: 4148 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-29 20:44 xia_engine_mysql/__init__.py
+-rw-r--r--  2.0 unx     6756 b- defN 23-Jun-29 20:07 xia_engine_mysql/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      600 b- defN 23-Jun-29 20:46 xia_engine_mysql-0.1.8.dist-info/RECORD
+7 files, 8481 bytes uncompressed, 3070 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_mysql/__init__.py
 Comment: 
 
-Filename: xia_engine_mysql/engine.cp39-win_amd64.pyd
+Filename: xia_engine_mysql/engine.py
 Comment: 
 
-Filename: xia_engine_mysql-0.1.7.dist-info/LICENSE.txt
+Filename: xia_engine_mysql-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.7.dist-info/METADATA
+Filename: xia_engine_mysql-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_mysql-0.1.7.dist-info/WHEEL
+Filename: xia_engine_mysql-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_mysql-0.1.7.dist-info/top_level.txt
+Filename: xia_engine_mysql-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_mysql-0.1.7.dist-info/RECORD
+Filename: xia_engine_mysql-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_mysql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_engine_mysql.engine import MysqlEngine, MysqlConnectParam
 
 __all__ = [
     "MysqlEngine", "MysqlConnectParam"
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_engine_mysql-0.1.7.dist-info/METADATA` & `xia_engine_mysql-0.1.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-mysql
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-mysql/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-mysql/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

