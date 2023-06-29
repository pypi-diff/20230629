# Comparing `tmp/xia_coder-0.0.5-cp39-none-win_amd64.whl.zip` & `tmp/xia_coder-0.0.6-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 135590 bytes, number of entries: 7
--rw-r--r--  2.0 unx       84 b- defN 23-Jun-26 18:29 xia_coder/__init__.py
--rw-r--r--  2.0 unx   329728 b- defN 23-Jun-26 18:33 xia_coder/coder.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:33 xia_coder-0.0.5.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      634 b- defN 23-Jun-26 18:33 xia_coder-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:33 xia_coder-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-26 18:33 xia_coder-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      567 b- defN 23-Jun-26 18:33 xia_coder-0.0.5.dist-info/RECORD
-7 files, 331273 bytes uncompressed, 134580 bytes compressed:  59.4%
+Zip file size: 3888 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-29 20:39 xia_coder/__init__.py
+-rw-r--r--  2.0 unx     6257 b- defN 23-Jun-29 17:18 xia_coder/coder.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:41 xia_coder-0.0.6.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      634 b- defN 23-Jun-29 20:41 xia_coder-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:41 xia_coder-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-29 20:41 xia_coder-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      549 b- defN 23-Jun-29 20:41 xia_coder-0.0.6.dist-info/RECORD
+7 files, 7783 bytes uncompressed, 2910 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_coder/__init__.py
 Comment: 
 
-Filename: xia_coder/coder.cp39-win_amd64.pyd
+Filename: xia_coder/coder.py
 Comment: 
 
-Filename: xia_coder-0.0.5.dist-info/LICENSE.txt
+Filename: xia_coder-0.0.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_coder-0.0.5.dist-info/METADATA
+Filename: xia_coder-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: xia_coder-0.0.5.dist-info/WHEEL
+Filename: xia_coder-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: xia_coder-0.0.5.dist-info/top_level.txt
+Filename: xia_coder-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_coder-0.0.5.dist-info/RECORD
+Filename: xia_coder-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_coder/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_coder.coder import Coder
 
 __all__ = [
     "Coder"
 ]
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
```

## Comparing `xia_coder-0.0.5.dist-info/METADATA` & `xia_coder-0.0.6.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-coder
-Version: 0.0.5
+Version: 0.0.6
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-coder/0.0.5/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-coder/0.0.6/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

