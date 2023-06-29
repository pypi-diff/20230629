# Comparing `tmp/xia_engine_rest-0.1.11-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_rest-0.1.12-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 149091 bytes, number of entries: 7
--rw-r--r--  2.0 unx      141 b- defN 23-Jun-26 14:17 xia_engine_rest/__init__.py
--rw-r--r--  2.0 unx   381440 b- defN 23-Jun-26 14:21 xia_engine_rest/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 14:21 xia_engine_rest-0.1.11.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      684 b- defN 23-Jun-26 14:21 xia_engine_rest-0.1.11.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 14:21 xia_engine_rest-0.1.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-26 14:21 xia_engine_rest-0.1.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      616 b- defN 23-Jun-26 14:21 xia_engine_rest-0.1.11.dist-info/RECORD
-7 files, 383147 bytes uncompressed, 147985 bytes compressed:  61.4%
+Zip file size: 4023 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      140 b- defN 23-Jun-29 20:43 xia_engine_rest/__init__.py
+-rw-r--r--  2.0 unx     7322 b- defN 23-Jun-29 17:29 xia_engine_rest/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      684 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      598 b- defN 23-Jun-29 20:46 xia_engine_rest-0.1.12.dist-info/RECORD
+7 files, 9010 bytes uncompressed, 2949 bytes compressed:  67.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_rest/__init__.py
 Comment: 
 
-Filename: xia_engine_rest/engine.cp39-win_amd64.pyd
+Filename: xia_engine_rest/engine.py
 Comment: 
 
-Filename: xia_engine_rest-0.1.11.dist-info/LICENSE.txt
+Filename: xia_engine_rest-0.1.12.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.11.dist-info/METADATA
+Filename: xia_engine_rest-0.1.12.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_rest-0.1.11.dist-info/WHEEL
+Filename: xia_engine_rest-0.1.12.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_rest-0.1.11.dist-info/top_level.txt
+Filename: xia_engine_rest-0.1.12.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_rest-0.1.11.dist-info/RECORD
+Filename: xia_engine_rest-0.1.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_rest/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_rest.engine import RestEngine, RestConnectParam
 
 
 __all__ = [
     "RestEngine", "RestConnectParam"
 ]
 
-__version__ = "0.1.11"
+__version__ = "0.1.12"
```

## Comparing `xia_engine_rest-0.1.11.dist-info/METADATA` & `xia_engine_rest-0.1.12.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-rest
-Version: 0.1.11
+Version: 0.1.12
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-rest/0.1.11/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-rest/0.1.12/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_rest-0.1.11.dist-info/RECORD` & `xia_engine_rest-0.1.12.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_rest/__init__.py,sha256=MjIfMjPQhfKZLm63r4v6XsVvdEdY60ukCHctfjNZibo,141
-xia_engine_rest/engine.cp39-win_amd64.pyd,sha256=3aUwcTyZpdglggoHr7HLO0aTn8tKpjh1nOiXFWOh2Lk,381440
-xia_engine_rest-0.1.11.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_engine_rest-0.1.11.dist-info/METADATA,sha256=ZjPQiDlzE-QYbkLavntnBKJ40ub847amFrFJfoHbalg,684
-xia_engine_rest-0.1.11.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_rest-0.1.11.dist-info/top_level.txt,sha256=Y6M8ui9-spd32kpo6unwoI0veR6mPHw-V7WRkhbl74g,16
-xia_engine_rest-0.1.11.dist-info/RECORD,,
+xia_engine_rest/__init__.py,sha256=UPXJD1nvpX-nlj7UT1ynBn7rRvn1fRAjGlRQyBrf5b4,140
+xia_engine_rest/engine.py,sha256=inDcFQMgT9zTNdkwZrzNjj-6KvSTUI1daD-rjcF4yyY,7322
+xia_engine_rest-0.1.12.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_rest-0.1.12.dist-info/METADATA,sha256=i2ft2BsWRXw7ybprEErRCON6VyFzxisLG-dazCfJZA0,684
+xia_engine_rest-0.1.12.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_rest-0.1.12.dist-info/top_level.txt,sha256=Y6M8ui9-spd32kpo6unwoI0veR6mPHw-V7WRkhbl74g,16
+xia_engine_rest-0.1.12.dist-info/RECORD,,
```

