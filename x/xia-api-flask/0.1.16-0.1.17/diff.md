# Comparing `tmp/xia_api_flask-0.1.16-cp39-none-win_amd64.whl.zip` & `tmp/xia_api_flask-0.1.17-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 165026 bytes, number of entries: 7
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-26 07:13 xia_api_flask/__init__.py
--rw-r--r--  2.0 unx   445952 b- defN 23-Jun-26 07:17 xia_api_flask/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 07:17 xia_api_flask-0.1.16.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-Jun-26 07:17 xia_api_flask-0.1.16.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 07:17 xia_api_flask-0.1.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Jun-26 07:17 xia_api_flask-0.1.16.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      599 b- defN 23-Jun-26 07:17 xia_api_flask-0.1.16.dist-info/RECORD
-7 files, 447647 bytes uncompressed, 163952 bytes compressed:  63.4%
+Zip file size: 6053 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 20:34 xia_api_flask/__init__.py
+-rw-r--r--  2.0 unx    18246 b- defN 23-Jun-29 20:34 xia_api_flask/rest.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:36 xia_api_flask-0.1.17.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      739 b- defN 23-Jun-29 20:36 xia_api_flask-0.1.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:36 xia_api_flask-0.1.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-29 20:36 xia_api_flask-0.1.17.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      582 b- defN 23-Jun-29 20:36 xia_api_flask-0.1.17.dist-info/RECORD
+7 files, 19923 bytes uncompressed, 5011 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_api_flask/__init__.py
 Comment: 
 
-Filename: xia_api_flask/rest.cp39-win_amd64.pyd
+Filename: xia_api_flask/rest.py
 Comment: 
 
-Filename: xia_api_flask-0.1.16.dist-info/LICENSE.txt
+Filename: xia_api_flask-0.1.17.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.16.dist-info/METADATA
+Filename: xia_api_flask-0.1.17.dist-info/METADATA
 Comment: 
 
-Filename: xia_api_flask-0.1.16.dist-info/WHEEL
+Filename: xia_api_flask-0.1.17.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api_flask-0.1.16.dist-info/top_level.txt
+Filename: xia_api_flask-0.1.17.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api_flask-0.1.16.dist-info/RECORD
+Filename: xia_api_flask-0.1.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_api_flask.rest import Restful
 
 __all__ = [
     "Restful",
 ]
 
-__version__ = "0.1.16"
+__version__ = "0.1.17"
```

## Comparing `xia_api_flask-0.1.16.dist-info/METADATA` & `xia_api_flask-0.1.17.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api-flask
-Version: 0.1.16
+Version: 0.1.17
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.16/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api-flask/0.1.17/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

