# Comparing `tmp/xia_token_flask-0.1.12-cp39-none-win_amd64.whl.zip` & `tmp/xia_token_flask-0.1.13-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 144932 bytes, number of entries: 7
--rw-r--r--  2.0 unx      103 b- defN 23-Jun-26 17:25 xia_token_flask/__init__.py
--rw-r--r--  2.0 unx   382976 b- defN 23-Jun-26 17:28 xia_token_flask/token.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 17:28 xia_token_flask-0.1.12.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      702 b- defN 23-Jun-26 17:28 xia_token_flask-0.1.12.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 17:28 xia_token_flask-0.1.12.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-26 17:28 xia_token_flask-0.1.12.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      615 b- defN 23-Jun-26 17:28 xia_token_flask-0.1.12.dist-info/RECORD
-7 files, 384662 bytes uncompressed, 143828 bytes compressed:  62.6%
+Zip file size: 5385 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      102 b- defN 23-Jun-29 21:02 xia_token_flask/__init__.py
+-rw-r--r--  2.0 unx    17714 b- defN 23-Jun-29 21:02 xia_token_flask/token.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 21:02 xia_token_flask-0.1.13.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      702 b- defN 23-Jun-29 21:02 xia_token_flask-0.1.13.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 21:02 xia_token_flask-0.1.13.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 21:02 xia_token_flask-0.1.13.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      599 b- defN 23-Jun-29 21:02 xia_token_flask-0.1.13.dist-info/RECORD
+7 files, 19392 bytes uncompressed, 4313 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_token_flask/__init__.py
 Comment: 
 
-Filename: xia_token_flask/token.cp39-win_amd64.pyd
+Filename: xia_token_flask/token.py
 Comment: 
 
-Filename: xia_token_flask-0.1.12.dist-info/LICENSE.txt
+Filename: xia_token_flask-0.1.13.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.12.dist-info/METADATA
+Filename: xia_token_flask-0.1.13.dist-info/METADATA
 Comment: 
 
-Filename: xia_token_flask-0.1.12.dist-info/WHEEL
+Filename: xia_token_flask-0.1.13.dist-info/WHEEL
 Comment: 
 
-Filename: xia_token_flask-0.1.12.dist-info/top_level.txt
+Filename: xia_token_flask-0.1.13.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_token_flask-0.1.12.dist-info/RECORD
+Filename: xia_token_flask-0.1.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_token_flask/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_token_flask.token import FlaskToken
 
 
 __all__ = [
     "FlaskToken",
 ]
 
-__version__ = "0.1.12"
+__version__ = "0.1.13"
```

## Comparing `xia_token_flask-0.1.12.dist-info/METADATA` & `xia_token_flask-0.1.13.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-token-flask
-Version: 0.1.12
+Version: 0.1.13
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.12/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-token-flask/0.1.13/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

