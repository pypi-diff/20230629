# Comparing `tmp/xia_logger_gcp-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_logger_gcp-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 107657 bytes, number of entries: 7
--rw-r--r--  2.0 unx       98 b- defN 23-Jun-26 17:57 xia_logger_gcp/__init__.py
--rw-r--r--  2.0 unx   261120 b- defN 23-Jun-26 17:59 xia_logger_gcp/logger.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:59 xia_logger_gcp-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      690 b- defN 23-Jun-26 17:59 xia_logger_gcp-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:59 xia_logger_gcp-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-26 17:59 xia_logger_gcp-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      603 b- defN 23-Jun-26 17:59 xia_logger_gcp-0.1.1.dist-info/RECORD
-7 files, 262776 bytes uncompressed, 106575 bytes compressed:  59.4%
+Zip file size: 2347 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-29 20:52 xia_logger_gcp/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 23-Jun-29 20:52 xia_logger_gcp/logger.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      690 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      584 b- defN 23-Jun-29 20:55 xia_logger_gcp-0.1.2.dist-info/RECORD
+7 files, 2185 bytes uncompressed, 1297 bytes compressed:  40.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_logger_gcp/__init__.py
 Comment: 
 
-Filename: xia_logger_gcp/logger.cp39-win_amd64.pyd
+Filename: xia_logger_gcp/logger.py
 Comment: 
 
-Filename: xia_logger_gcp-0.1.1.dist-info/LICENSE.txt
+Filename: xia_logger_gcp-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.1.dist-info/METADATA
+Filename: xia_logger_gcp-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_logger_gcp-0.1.1.dist-info/WHEEL
+Filename: xia_logger_gcp-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_logger_gcp-0.1.1.dist-info/top_level.txt
+Filename: xia_logger_gcp-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_logger_gcp-0.1.1.dist-info/RECORD
+Filename: xia_logger_gcp-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_logger_gcp/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_logger_gcp.logger import GcpLogger
 
 __all__ = [
     "GcpLogger"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_logger_gcp-0.1.1.dist-info/METADATA` & `xia_logger_gcp-0.1.2.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-logger-gcp
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-logger-gcp/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-logger-gcp/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_logger_gcp-0.1.1.dist-info/RECORD` & `xia_logger_gcp-0.1.2.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_logger_gcp/__init__.py,sha256=5YBHqys4zwRXxMtmsMB-RW-yiVN5JfqZIu4c9g_Ri2I,98
-xia_logger_gcp/logger.cp39-win_amd64.pyd,sha256=ncyHBZe41b-AS3BgWjFS27OSiUQfOH8DdNhPKRZS1xw,261120
-xia_logger_gcp-0.1.1.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_logger_gcp-0.1.1.dist-info/METADATA,sha256=qwGbfcBlC4BRBGz3Swfg6gkDDCclm188BHIY2bYoLsc,690
-xia_logger_gcp-0.1.1.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_logger_gcp-0.1.1.dist-info/top_level.txt,sha256=c5S6Io75CGyFOYz1y3f4z_covUMj-YmHjiiIOd_Fdm8,15
-xia_logger_gcp-0.1.1.dist-info/RECORD,,
+xia_logger_gcp/__init__.py,sha256=lhUKucqLN-vKwbidjiyjtF0ZG1SHtTaSS5af5YhYUrM,97
+xia_logger_gcp/logger.py,sha256=sz-E3pDHuTURtUfhhGqluuIxIqP3DI1MISpdNIhF4-E,549
+xia_logger_gcp-0.1.2.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_logger_gcp-0.1.2.dist-info/METADATA,sha256=zLAvOKTB5nB-60xrxEqtP7VaksHLMCYxu2O0pcwF-0A,690
+xia_logger_gcp-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_logger_gcp-0.1.2.dist-info/top_level.txt,sha256=c5S6Io75CGyFOYz1y3f4z_covUMj-YmHjiiIOd_Fdm8,15
+xia_logger_gcp-0.1.2.dist-info/RECORD,,
```

