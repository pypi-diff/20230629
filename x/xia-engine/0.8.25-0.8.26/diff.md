# Comparing `tmp/xia_engine-0.8.25-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine-0.8.26-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 1220154 bytes, number of entries: 12
--rw-r--r--  2.0 unx     1514 b- defN 23-Jun-26 06:59 xia_engine/__init__.py
--rw-r--r--  2.0 unx   458240 b- defN 23-Jun-26 07:04 xia_engine/acl.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   588288 b- defN 23-Jun-26 07:02 xia_engine/base.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   787968 b- defN 23-Jun-26 07:09 xia_engine/document.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   875520 b- defN 23-Jun-26 07:07 xia_engine/engine.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   282624 b- defN 23-Jun-26 07:09 xia_engine/exception.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   462336 b- defN 23-Jun-26 07:05 xia_engine/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 07:09 xia_engine-0.8.25.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      747 b- defN 23-Jun-26 07:09 xia_engine-0.8.25.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 07:09 xia_engine-0.8.25.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-26 07:09 xia_engine-0.8.25.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1057 b- defN 23-Jun-26 07:09 xia_engine-0.8.25.dist-info/RECORD
-12 files, 3458555 bytes uncompressed, 1218378 bytes compressed:  64.8%
+Zip file size: 36959 bytes, number of entries: 12
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jun-29 20:44 xia_engine/__init__.py
+-rw-r--r--  2.0 unx    14239 b- defN 23-Jun-29 20:44 xia_engine/acl.py
+-rw-r--r--  2.0 unx    35369 b- defN 23-Jun-29 20:44 xia_engine/base.py
+-rw-r--r--  2.0 unx    52305 b- defN 23-Jun-29 20:44 xia_engine/document.py
+-rw-r--r--  2.0 unx    43611 b- defN 23-Jun-29 20:44 xia_engine/engine.py
+-rw-r--r--  2.0 unx      961 b- defN 23-Jun-29 20:44 xia_engine/exception.py
+-rw-r--r--  2.0 unx    15335 b- defN 23-Jun-29 20:44 xia_engine/fields.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:44 xia_engine-0.8.26.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      747 b- defN 23-Jun-29 20:44 xia_engine-0.8.26.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:44 xia_engine-0.8.26.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 20:44 xia_engine-0.8.26.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      954 b- defN 23-Jun-29 20:44 xia_engine-0.8.26.dist-info/RECORD
+12 files, 165304 bytes uncompressed, 35375 bytes compressed:  78.6%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
 Filename: xia_engine/__init__.py
 Comment: 
 
-Filename: xia_engine/acl.cp39-win_amd64.pyd
+Filename: xia_engine/acl.py
 Comment: 
 
-Filename: xia_engine/base.cp39-win_amd64.pyd
+Filename: xia_engine/base.py
 Comment: 
 
-Filename: xia_engine/document.cp39-win_amd64.pyd
+Filename: xia_engine/document.py
 Comment: 
 
-Filename: xia_engine/engine.cp39-win_amd64.pyd
+Filename: xia_engine/engine.py
 Comment: 
 
-Filename: xia_engine/exception.cp39-win_amd64.pyd
+Filename: xia_engine/exception.py
 Comment: 
 
-Filename: xia_engine/fields.cp39-win_amd64.pyd
+Filename: xia_engine/fields.py
 Comment: 
 
-Filename: xia_engine-0.8.25.dist-info/LICENSE.txt
+Filename: xia_engine-0.8.26.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine-0.8.25.dist-info/METADATA
+Filename: xia_engine-0.8.26.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine-0.8.25.dist-info/WHEEL
+Filename: xia_engine-0.8.26.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine-0.8.25.dist-info/top_level.txt
+Filename: xia_engine-0.8.26.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine-0.8.25.dist-info/RECORD
+Filename: xia_engine-0.8.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine/__init__.py

```diff
@@ -20,8 +20,8 @@
     "MetaEngine", "MetaRamEngine", "MetaCache", "MirrorClient", "MirrorEngine",
     "Acl", "AclItem",
     "XiaError", 'AuthorizationError', 'AuthenticationError', "OutOfQuotaError", "OutOfScopeError",
     'NotFoundError', 'ConflictError', 'BadRequestError', "UnprocessableError",
     "ServerError"
 ]
 
-__version__ = "0.8.25"
+__version__ = "0.8.26"
```

## Comparing `xia_engine-0.8.25.dist-info/METADATA` & `xia_engine-0.8.26.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine
-Version: 0.8.25
+Version: 0.8.26
 Summary: X-I-A Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.25/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine/0.8.26/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine-0.8.25.dist-info/RECORD` & `xia_engine-0.8.26.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-xia_engine/__init__.py,sha256=ad19BhBuHas6OHHb_yH5dQCpHk4CuOsRtc_9AE4sEwQ,1514
-xia_engine/acl.cp39-win_amd64.pyd,sha256=QmClMMTwCwRfGzuDxdIHwMbIfaZaxdqd-f2OlEJHQwc,458240
-xia_engine/base.cp39-win_amd64.pyd,sha256=CADQWBIFC_gi2MzkNw7nNIYkJbmEq8oKYHr78P1RcpA,588288
-xia_engine/document.cp39-win_amd64.pyd,sha256=UwZv_IEkwMnIHSfap8uh2JjTJ8BfCb_hVHemXYoxiW0,787968
-xia_engine/engine.cp39-win_amd64.pyd,sha256=wjZu9Hg5yvH1I8U06_IU3uKEktWJyfZES7M3dSVlhI4,875520
-xia_engine/exception.cp39-win_amd64.pyd,sha256=z1b_JJ4Lvn6rgdJUNO4X_-9K7G2RCbElilGYjbxmpHs,282624
-xia_engine/fields.cp39-win_amd64.pyd,sha256=vQAo0iP6Uj4H0etrSjmJI4AK5ngx9G7Y_oLgKrjckEs,462336
-xia_engine-0.8.25.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_engine-0.8.25.dist-info/METADATA,sha256=F1ZAQyjrgksqXLLrRB_jYz_vZ900cJLMkjjAIkH7Xq0,747
-xia_engine-0.8.25.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine-0.8.25.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
-xia_engine-0.8.25.dist-info/RECORD,,
+xia_engine/__init__.py,sha256=zNzNMNFLjmd1TDTPRSMSLvUgSAkiPosDacnoEzmj9_8,1513
+xia_engine/acl.py,sha256=Ro7FDlS7bxTriLP3dz4laYvl7t8nnqN1dN7FTAuRXGM,14239
+xia_engine/base.py,sha256=5YT455WiN8UjNTzcH1ulYBdPfodkFdEWsedZ5irBlPc,35369
+xia_engine/document.py,sha256=0HRwF65iqt0ePCwiQ2BF6Rk1pMKocQhygAT5MiV6YaA,52305
+xia_engine/engine.py,sha256=o4AkyE0d-TqctNXk4TjPFswUQMNA9iLc8veWfNAu9GI,43611
+xia_engine/exception.py,sha256=3OpfXYqwsnVxTU2Jz2vyFNvKdTfA-_nWMOnBbz_PRTk,961
+xia_engine/fields.py,sha256=h8veDRJLZHX2jmgUvms0iacxMlMAMVvjNvXkP3DBwUY,15335
+xia_engine-0.8.26.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine-0.8.26.dist-info/METADATA,sha256=kFkCnB2me4ZRN8fAgJsNsbZ0qmcCMGNcFmgUQYh_ZQU,747
+xia_engine-0.8.26.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_engine-0.8.26.dist-info/top_level.txt,sha256=Q896WUzHNHm14oiEaw7BbLcGbvHkKPKEQOBa8Z06dbk,11
+xia_engine-0.8.26.dist-info/RECORD,,
```

