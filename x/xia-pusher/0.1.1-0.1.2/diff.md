# Comparing `tmp/xia_pusher-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_pusher-0.1.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 112838 bytes, number of entries: 7
--rw-r--r--  2.0 unx       88 b- defN 23-Jun-26 13:22 xia_pusher/__init__.py
--rw-r--r--  2.0 unx   275456 b- defN 23-Jun-26 13:24 xia_pusher/pusher.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      689 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      575 b- defN 23-Jun-26 13:24 xia_pusher-0.1.1.dist-info/RECORD
-7 files, 277069 bytes uncompressed, 111812 bytes compressed:  59.6%
+Zip file size: 2639 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       87 b- defN 23-Jun-29 20:56 xia_pusher/__init__.py
+-rw-r--r--  2.0 unx     1743 b- defN 23-Jun-29 20:56 xia_pusher/pusher.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:56 xia_pusher-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      689 b- defN 23-Jun-29 20:56 xia_pusher-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:56 xia_pusher-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:56 xia_pusher-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      558 b- defN 23-Jun-29 20:56 xia_pusher-0.1.2.dist-info/RECORD
+7 files, 3347 bytes uncompressed, 1645 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_pusher/__init__.py
 Comment: 
 
-Filename: xia_pusher/pusher.cp39-win_amd64.pyd
+Filename: xia_pusher/pusher.py
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/LICENSE.txt
+Filename: xia_pusher-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/METADATA
+Filename: xia_pusher-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/WHEEL
+Filename: xia_pusher-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/top_level.txt
+Filename: xia_pusher-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_pusher-0.1.1.dist-info/RECORD
+Filename: xia_pusher-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_pusher/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_pusher.pusher import Pusher
 
 __all__ = [
     "Pusher"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_pusher-0.1.1.dist-info/METADATA` & `xia_pusher-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-pusher
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-pusher/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

