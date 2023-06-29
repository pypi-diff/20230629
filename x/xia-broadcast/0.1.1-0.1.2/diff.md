# Comparing `tmp/xia_broadcast-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast-0.1.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 133198 bytes, number of entries: 7
--rw-r--r--  2.0 unx      132 b- defN 23-Jun-26 17:47 xia_broadcast/__init__.py
--rw-r--r--  2.0 unx   328704 b- defN 23-Jun-26 17:50 xia_broadcast/broadcast.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:50 xia_broadcast-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      840 b- defN 23-Jun-26 17:50 xia_broadcast-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:50 xia_broadcast-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-26 17:50 xia_broadcast-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-26 17:50 xia_broadcast-0.1.1.dist-info/RECORD
-7 files, 330540 bytes uncompressed, 132124 bytes compressed:  60.0%
+Zip file size: 4302 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      131 b- defN 23-Jun-29 20:35 xia_broadcast/__init__.py
+-rw-r--r--  2.0 unx     7587 b- defN 23-Jun-29 20:35 xia_broadcast/broadcast.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:35 xia_broadcast-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      840 b- defN 23-Jun-29 20:35 xia_broadcast-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:35 xia_broadcast-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-29 20:35 xia_broadcast-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-Jun-29 20:35 xia_broadcast-0.1.2.dist-info/RECORD
+7 files, 9414 bytes uncompressed, 3260 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast/__init__.py
 Comment: 
 
-Filename: xia_broadcast/broadcast.cp39-win_amd64.pyd
+Filename: xia_broadcast/broadcast.py
 Comment: 
 
-Filename: xia_broadcast-0.1.1.dist-info/LICENSE.txt
+Filename: xia_broadcast-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.1.dist-info/METADATA
+Filename: xia_broadcast-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast-0.1.1.dist-info/WHEEL
+Filename: xia_broadcast-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast-0.1.1.dist-info/top_level.txt
+Filename: xia_broadcast-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast-0.1.1.dist-info/RECORD
+Filename: xia_broadcast-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast.broadcast import AuthClient, Broadcaster
 
 
 __all__ = [
     "AuthClient", "Broadcaster",
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_broadcast-0.1.1.dist-info/METADATA` & `xia_broadcast-0.1.2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-broadcast
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A Broadcast
-Home-page: https://develop.x-i-a.com/docs/xia-broadcast/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-broadcast/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

