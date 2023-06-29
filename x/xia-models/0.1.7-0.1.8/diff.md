# Comparing `tmp/xia_models-0.1.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_models-0.1.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 329586 bytes, number of entries: 8
--rw-r--r--  2.0 unx      239 b- defN 23-Jun-26 14:15 xia_models/__init__.py
--rw-r--r--  2.0 unx   432640 b- defN 23-Jun-26 14:18 xia_models/address.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   452096 b- defN 23-Jun-26 14:21 xia_models/model.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 14:21 xia_models-0.1.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      638 b- defN 23-Jun-26 14:21 xia_models-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 14:21 xia_models-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 14:21 xia_models-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      671 b- defN 23-Jun-26 14:21 xia_models-0.1.7.dist-info/RECORD
-8 files, 886545 bytes uncompressed, 328412 bytes compressed:  63.0%
+Zip file size: 9857 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      238 b- defN 23-Jun-29 20:56 xia_models/__init__.py
+-rw-r--r--  2.0 unx    18354 b- defN 23-Jun-29 20:56 xia_models/address.py
+-rw-r--r--  2.0 unx    16070 b- defN 23-Jun-29 20:56 xia_models/model.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      638 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      637 b- defN 23-Jun-29 20:57 xia_models-0.1.8.dist-info/RECORD
+8 files, 36198 bytes uncompressed, 8747 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: xia_models/__init__.py
 Comment: 
 
-Filename: xia_models/address.cp39-win_amd64.pyd
+Filename: xia_models/address.py
 Comment: 
 
-Filename: xia_models/model.cp39-win_amd64.pyd
+Filename: xia_models/model.py
 Comment: 
 
-Filename: xia_models-0.1.7.dist-info/LICENSE.txt
+Filename: xia_models-0.1.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_models-0.1.7.dist-info/METADATA
+Filename: xia_models-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_models-0.1.7.dist-info/WHEEL
+Filename: xia_models-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_models-0.1.7.dist-info/top_level.txt
+Filename: xia_models-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_models-0.1.7.dist-info/RECORD
+Filename: xia_models-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_models/__init__.py

```diff
@@ -2,8 +2,8 @@
 from xia_models.address import DataAddress, TableAddress, TableCatalog
 
 __all__ = [
     "DataModel", "DataField",
     "DataAddress", "TableAddress", "TableCatalog"
 ]
 
-__version__ = "0.1.7"
+__version__ = "0.1.8"
```

## Comparing `xia_models-0.1.7.dist-info/METADATA` & `xia_models-0.1.8.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-models
-Version: 0.1.7
+Version: 0.1.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-models/0.1.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-models/0.1.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

