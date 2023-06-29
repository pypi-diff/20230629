# Comparing `tmp/xia_broadcast_fastapi-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_broadcast_fastapi-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 134725 bytes, number of entries: 7
--rw-r--r--  2.0 unx      130 b- defN 23-Jun-26 17:37 xia_broadcast_fastapi/__init__.py
--rw-r--r--  2.0 unx   333312 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi/broadcaster.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      900 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      658 b- defN 23-Jun-26 17:40 xia_broadcast_fastapi-0.1.0.dist-info/RECORD
-7 files, 335272 bytes uncompressed, 133535 bytes compressed:  60.2%
+Zip file size: 3840 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      129 b- defN 23-Jun-29 20:33 xia_broadcast_fastapi/__init__.py
+-rw-r--r--  2.0 unx     4771 b- defN 23-Jun-29 20:33 xia_broadcast_fastapi/broadcaster.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      900 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      640 b- defN 23-Jun-29 20:37 xia_broadcast_fastapi-0.1.1.dist-info/RECORD
+7 files, 6712 bytes uncompressed, 2682 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_broadcast_fastapi/__init__.py
 Comment: 
 
-Filename: xia_broadcast_fastapi/broadcaster.cp39-win_amd64.pyd
+Filename: xia_broadcast_fastapi/broadcaster.py
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.0.dist-info/LICENSE.txt
+Filename: xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.0.dist-info/METADATA
+Filename: xia_broadcast_fastapi-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.0.dist-info/WHEEL
+Filename: xia_broadcast_fastapi-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.0.dist-info/top_level.txt
+Filename: xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_broadcast_fastapi-0.1.0.dist-info/RECORD
+Filename: xia_broadcast_fastapi-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_broadcast_fastapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_broadcast_fastapi.broadcaster import BroadcasterFastapi
 
 
 __all__ = [
     "BroadcasterFastapi",
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_broadcast_fastapi-0.1.0.dist-info/METADATA` & `xia_broadcast_fastapi-0.1.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-broadcast-fastapi
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A Broadcast
-Home-page: https://develop.x-i-a.com/docs/xia-broadcast-fastapi/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-broadcast-fastapi/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_broadcast_fastapi-0.1.0.dist-info/RECORD` & `xia_broadcast_fastapi-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_broadcast_fastapi/__init__.py,sha256=7_k2J-tJuVMFRDLo_sv8OT5BGMUuVutg6zZlhZgFgOM,130
-xia_broadcast_fastapi/broadcaster.cp39-win_amd64.pyd,sha256=x3UjmaIjFuAu8wFxC2N6Ye0Az2T5KGV_sGhJhiCJwAw,333312
-xia_broadcast_fastapi-0.1.0.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_broadcast_fastapi-0.1.0.dist-info/METADATA,sha256=togAoTuYkvHcF08Z3knBEksT_jx2HoG-Q2OBy30py_4,900
-xia_broadcast_fastapi-0.1.0.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_broadcast_fastapi-0.1.0.dist-info/top_level.txt,sha256=t1WhzbP6ZYMQR5rAS86UFjQkSu3TvquMHCAklcm7YlA,22
-xia_broadcast_fastapi-0.1.0.dist-info/RECORD,,
+xia_broadcast_fastapi/__init__.py,sha256=ywMWnVZ5GvlYc8VZNp-A8muh_tz1-Khasx-ReGL9WWk,129
+xia_broadcast_fastapi/broadcaster.py,sha256=eGRCKnE6Elx2QArLCgLadsOvjeyeGQ6EUK9xbV6W4hk,4771
+xia_broadcast_fastapi-0.1.1.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_broadcast_fastapi-0.1.1.dist-info/METADATA,sha256=pjJmYF6D3fvCfUFec_9WmhgKNJZ9EkNexVqai5perg8,900
+xia_broadcast_fastapi-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_broadcast_fastapi-0.1.1.dist-info/top_level.txt,sha256=t1WhzbP6ZYMQR5rAS86UFjQkSu3TvquMHCAklcm7YlA,22
+xia_broadcast_fastapi-0.1.1.dist-info/RECORD,,
```

