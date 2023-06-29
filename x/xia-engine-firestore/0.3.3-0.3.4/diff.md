# Comparing `tmp/xia_engine_firestore-0.3.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_firestore-0.3.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 4305 bytes, number of entries: 7
--rw-r--r--  2.0 unx      117 b- defN 23-Jun-29 12:53 xia_engine_firestore/__init__.py
--rw-r--r--  2.0 unx     9905 b- defN 23-Jun-29 12:53 xia_engine_firestore/engine.py
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 12:54 xia_engine_firestore-0.3.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      817 b- defN 23-Jun-29 12:54 xia_engine_firestore-0.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 12:54 xia_engine_firestore-0.3.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 12:54 xia_engine_firestore-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      628 b- defN 23-Jun-29 12:54 xia_engine_firestore-0.3.3.dist-info/RECORD
+-rw-r--r--  2.0 unx      117 b- defN 23-Jun-29 14:06 xia_engine_firestore/__init__.py
+-rw-r--r--  2.0 unx     9905 b- defN 23-Jun-29 12:54 xia_engine_firestore/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 14:06 xia_engine_firestore-0.3.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      817 b- defN 23-Jun-29 14:06 xia_engine_firestore-0.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 14:06 xia_engine_firestore-0.3.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 14:06 xia_engine_firestore-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      628 b- defN 23-Jun-29 14:06 xia_engine_firestore-0.3.4.dist-info/RECORD
 7 files, 11738 bytes uncompressed, 3171 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_firestore/__init__.py
 Comment: 
 
 Filename: xia_engine_firestore/engine.py
 Comment: 
 
-Filename: xia_engine_firestore-0.3.3.dist-info/LICENSE.txt
+Filename: xia_engine_firestore-0.3.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.3.dist-info/METADATA
+Filename: xia_engine_firestore-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_firestore-0.3.3.dist-info/WHEEL
+Filename: xia_engine_firestore-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_firestore-0.3.3.dist-info/top_level.txt
+Filename: xia_engine_firestore-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_firestore-0.3.3.dist-info/RECORD
+Filename: xia_engine_firestore-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_firestore/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_firestore.engine import FirestoreEngine
 
 
 __all__ = [
     "FirestoreEngine"
 ]
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
```

## Comparing `xia_engine_firestore-0.3.3.dist-info/METADATA` & `xia_engine_firestore-0.3.4.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-firestore
-Version: 0.3.3
+Version: 0.3.4
 Summary: X-I-A Firestore Engine
-Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.3.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-firestore/0.3.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_firestore-0.3.3.dist-info/RECORD` & `xia_engine_firestore-0.3.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_firestore/__init__.py,sha256=VpQ32yBvJIWo1SX9bD98dJh6S1cnlwpwmRS1_bUoCGQ,117
+xia_engine_firestore/__init__.py,sha256=VPDqwU88LgsaK3n3yGvbvbG_5dN3a8bSsarQZEh-OmU,117
 xia_engine_firestore/engine.py,sha256=BewFLUI81p_T4SXsj3IAYa3LGCrtpNa9nviBaWj5fzI,9905
-xia_engine_firestore-0.3.3.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_engine_firestore-0.3.3.dist-info/METADATA,sha256=oTz7q_1f01jhaKf4w727bsjo_IgVBi2TCTXP1AE0erE,817
-xia_engine_firestore-0.3.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_firestore-0.3.3.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
-xia_engine_firestore-0.3.3.dist-info/RECORD,,
+xia_engine_firestore-0.3.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_firestore-0.3.4.dist-info/METADATA,sha256=3WDxgCEbIlrZmxCnK8RSGzrFix6hXVm8fRHeUiZ_Ffg,817
+xia_engine_firestore-0.3.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_firestore-0.3.4.dist-info/top_level.txt,sha256=NUY0_anDQ8KVQ1TnPs_SCf-78KqRmu8_ARIL_J5agrg,21
+xia_engine_firestore-0.3.4.dist-info/RECORD,,
```

