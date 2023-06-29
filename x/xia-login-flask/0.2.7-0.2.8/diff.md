# Comparing `tmp/xia_login_flask-0.2.7-cp39-none-win_amd64.whl.zip` & `tmp/xia_login_flask-0.2.8-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 199653 bytes, number of entries: 7
--rw-r--r--  2.0 unx      109 b- defN 23-Jun-26 05:39 xia_login_flask/__init__.py
--rw-r--r--  2.0 unx   560128 b- defN 23-Jun-26 05:43 xia_login_flask/account.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 05:43 xia_login_flask-0.2.7.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      739 b- defN 23-Jun-26 05:43 xia_login_flask-0.2.7.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 05:43 xia_login_flask-0.2.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-26 05:43 xia_login_flask-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 23-Jun-26 05:43 xia_login_flask-0.2.7.dist-info/RECORD
-7 files, 561854 bytes uncompressed, 198555 bytes compressed:  64.7%
+Zip file size: 7403 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:52 xia_login_flask/__init__.py
+-rw-r--r--  2.0 unx    25032 b- defN 23-Jun-29 20:52 xia_login_flask/account.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      739 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      595 b- defN 23-Jun-29 20:56 xia_login_flask-0.2.8.dist-info/RECORD
+7 files, 26740 bytes uncompressed, 6337 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_login_flask/__init__.py
 Comment: 
 
-Filename: xia_login_flask/account.cp39-win_amd64.pyd
+Filename: xia_login_flask/account.py
 Comment: 
 
-Filename: xia_login_flask-0.2.7.dist-info/LICENSE.txt
+Filename: xia_login_flask-0.2.8.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.7.dist-info/METADATA
+Filename: xia_login_flask-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: xia_login_flask-0.2.7.dist-info/WHEEL
+Filename: xia_login_flask-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: xia_login_flask-0.2.7.dist-info/top_level.txt
+Filename: xia_login_flask-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_login_flask-0.2.7.dist-info/RECORD
+Filename: xia_login_flask-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_login_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_login_flask.account import XiaLoginFlask
 
 __all__ = [
     "XiaLoginFlask",
 ]
 
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

## Comparing `xia_login_flask-0.2.7.dist-info/METADATA` & `xia_login_flask-0.2.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-login-flask
-Version: 0.2.7
+Version: 0.2.8
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.7/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-login-flask/0.2.8/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

