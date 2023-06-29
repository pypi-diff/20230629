# Comparing `tmp/xia_analytics-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 101226 bytes, number of entries: 7
--rw-r--r--  2.0 unx       96 b- defN 23-Jun-27 19:40 xia_analytics/__init__.py
--rw-r--r--  2.0 unx   245760 b- defN 23-Jun-27 19:42 xia_analytics/analyzer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      663 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      598 b- defN 23-Jun-27 19:42 xia_analytics-0.0.4.dist-info/RECORD
-7 files, 247381 bytes uncompressed, 100154 bytes compressed:  59.5%
+Zip file size: 2367 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       95 b- defN 23-Jun-29 20:32 xia_analytics/__init__.py
+-rw-r--r--  2.0 unx      750 b- defN 23-Jun-29 20:32 xia_analytics/analyzer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:36 xia_analytics-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      663 b- defN 23-Jun-29 20:36 xia_analytics-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:36 xia_analytics-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-29 20:36 xia_analytics-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      579 b- defN 23-Jun-29 20:36 xia_analytics-0.0.5.dist-info/RECORD
+7 files, 2351 bytes uncompressed, 1327 bytes compressed:  43.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics/__init__.py
 Comment: 
 
-Filename: xia_analytics/analyzer.cp39-win_amd64.pyd
+Filename: xia_analytics/analyzer.py
 Comment: 
 
-Filename: xia_analytics-0.0.4.dist-info/LICENSE.txt
+Filename: xia_analytics-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics-0.0.4.dist-info/METADATA
+Filename: xia_analytics-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics-0.0.4.dist-info/WHEEL
+Filename: xia_analytics-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics-0.0.4.dist-info/top_level.txt
+Filename: xia_analytics-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics-0.0.4.dist-info/RECORD
+Filename: xia_analytics-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_analytics/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_analytics.analyzer import Analyzer
 
 __all__ = [
    "Analyzer"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_analytics-0.0.4.dist-info/METADATA` & `xia_analytics-0.0.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-analytics
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-analytics/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

