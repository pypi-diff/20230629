# Comparing `tmp/xia_engine_sql-0.2.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_sql-0.2.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 281603 bytes, number of entries: 7
--rw-r--r--  2.0 unx      171 b- defN 23-Jun-26 08:27 xia_engine_sql/__init__.py
--rw-r--r--  2.0 unx   823808 b- defN 23-Jun-26 08:31 xia_engine_sql/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 08:31 xia_engine_sql-0.2.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      669 b- defN 23-Jun-26 08:31 xia_engine_sql-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 08:31 xia_engine_sql-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-26 08:31 xia_engine_sql-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      604 b- defN 23-Jun-26 08:31 xia_engine_sql-0.2.1.dist-info/RECORD
-7 files, 825517 bytes uncompressed, 280521 bytes compressed:  66.0%
+Zip file size: 11046 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      170 b- defN 23-Jun-29 20:44 xia_engine_sql/__init__.py
+-rw-r--r--  2.0 unx    41248 b- defN 23-Jun-29 20:07 xia_engine_sql/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:47 xia_engine_sql-0.2.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      669 b- defN 23-Jun-29 20:47 xia_engine_sql-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:47 xia_engine_sql-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:47 xia_engine_sql-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      587 b- defN 23-Jun-29 20:47 xia_engine_sql-0.2.2.dist-info/RECORD
+7 files, 42939 bytes uncompressed, 9996 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_sql/__init__.py
 Comment: 
 
-Filename: xia_engine_sql/engine.cp39-win_amd64.pyd
+Filename: xia_engine_sql/engine.py
 Comment: 
 
-Filename: xia_engine_sql-0.2.1.dist-info/LICENSE.txt
+Filename: xia_engine_sql-0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_sql-0.2.1.dist-info/METADATA
+Filename: xia_engine_sql-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_sql-0.2.1.dist-info/WHEEL
+Filename: xia_engine_sql-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_sql-0.2.1.dist-info/top_level.txt
+Filename: xia_engine_sql-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_sql-0.2.1.dist-info/RECORD
+Filename: xia_engine_sql-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_sql/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_engine_sql.engine import SqlEngine, SqliteEngine, SqliteConnectParam
 
 
 __all__ = [
     "SqlEngine", "SqliteEngine", "SqliteConnectParam"
 ]
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
```

## Comparing `xia_engine_sql-0.2.1.dist-info/METADATA` & `xia_engine_sql-0.2.2.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-sql
-Version: 0.2.1
+Version: 0.2.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.2.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-sql/0.2.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_sql-0.2.1.dist-info/RECORD` & `xia_engine_sql-0.2.2.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_sql/__init__.py,sha256=mih4WNRNpUxraZA3m3WDD4cS_iqbQ00UTdxLr9N9L1Y,171
-xia_engine_sql/engine.cp39-win_amd64.pyd,sha256=PWaltOhF5d8XHk6uz2-UN7nFV666DjApFdo9V4-UOj8,823808
-xia_engine_sql-0.2.1.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_engine_sql-0.2.1.dist-info/METADATA,sha256=Xvt5VJ9Hl0Xblf8JVcz78nUvjOrdlJill0MekJ5UaP4,669
-xia_engine_sql-0.2.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_sql-0.2.1.dist-info/top_level.txt,sha256=h1_hqTerPqRAQlyzQJgg61c-xJeOvLMmlDjskvb4uVA,15
-xia_engine_sql-0.2.1.dist-info/RECORD,,
+xia_engine_sql/__init__.py,sha256=EFj4Vrql410lKnRZZcv9JSpg-HFdEXgOCly2jZRVtoY,170
+xia_engine_sql/engine.py,sha256=u8mNY1Ku9yKHmNsqp51uXUIXNF38LI3QP5vmPH2HJIY,41248
+xia_engine_sql-0.2.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_sql-0.2.2.dist-info/METADATA,sha256=uFaMArT1qmhUcMfWkGGQKqEPga4vKPNNJdpBjacfozA,669
+xia_engine_sql-0.2.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_sql-0.2.2.dist-info/top_level.txt,sha256=h1_hqTerPqRAQlyzQJgg61c-xJeOvLMmlDjskvb4uVA,15
+xia_engine_sql-0.2.2.dist-info/RECORD,,
```

