# Comparing `tmp/xia_fields-0.3.11-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields-0.3.12-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 447580 bytes, number of entries: 9
--rw-r--r--  2.0 unx     1178 b- defN 23-Jun-25 20:45 xia_fields/__init__.py
--rw-r--r--  2.0 unx   376320 b- defN 23-Jun-25 20:50 xia_fields/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   419328 b- defN 23-Jun-25 20:52 xia_fields/fields.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   391680 b- defN 23-Jun-25 20:48 xia_fields/fields_ext.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 20:52 xia_fields-0.3.11.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3310 b- defN 23-Jun-25 20:52 xia_fields-0.3.11.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 20:52 xia_fields-0.3.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-25 20:52 xia_fields-0.3.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      775 b- defN 23-Jun-25 20:52 xia_fields-0.3.11.dist-info/RECORD
-9 files, 1192852 bytes uncompressed, 446244 bytes compressed:  62.6%
+Zip file size: 11493 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     1177 b- defN 23-Jun-29 20:50 xia_fields/__init__.py
+-rw-r--r--  2.0 unx    13346 b- defN 23-Jun-29 20:50 xia_fields/base.py
+-rw-r--r--  2.0 unx    13317 b- defN 23-Jun-29 20:50 xia_fields/fields.py
+-rw-r--r--  2.0 unx     9575 b- defN 23-Jun-29 20:50 xia_fields/fields_ext.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3310 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      723 b- defN 23-Jun-29 20:51 xia_fields-0.3.12.dist-info/RECORD
+9 files, 41709 bytes uncompressed, 10253 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_fields/__init__.py
 Comment: 
 
-Filename: xia_fields/base.cp39-win_amd64.pyd
+Filename: xia_fields/base.py
 Comment: 
 
-Filename: xia_fields/fields.cp39-win_amd64.pyd
+Filename: xia_fields/fields.py
 Comment: 
 
-Filename: xia_fields/fields_ext.cp39-win_amd64.pyd
+Filename: xia_fields/fields_ext.py
 Comment: 
 
-Filename: xia_fields-0.3.11.dist-info/LICENSE.txt
+Filename: xia_fields-0.3.12.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields-0.3.11.dist-info/METADATA
+Filename: xia_fields-0.3.12.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields-0.3.11.dist-info/WHEEL
+Filename: xia_fields-0.3.12.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields-0.3.11.dist-info/top_level.txt
+Filename: xia_fields-0.3.12.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields-0.3.11.dist-info/RECORD
+Filename: xia_fields-0.3.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields/__init__.py

```diff
@@ -14,8 +14,8 @@
     "JsonField", "DictField", "CompressedStringField",
     "Int64Field", "Int32Field", "SFixed64Field", "SFixed32Field",
     "UInt64Field", "UInt32Field", "Fixed64Field", "Fixed32Field",
     "DoubleField", "DateField", "TimestampField", "TimeField", "DateTimeField",
     "OsEnvironField"
 ]
 
-__version__ = "0.3.11"
+__version__ = "0.3.12"
```

## Comparing `xia_fields-0.3.11.dist-info/METADATA` & `xia_fields-0.3.12.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-fields
-Version: 0.3.11
+Version: 0.3.12
 Summary: X-I-A Field Protocol
-Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.11/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-fields/0.3.12/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

