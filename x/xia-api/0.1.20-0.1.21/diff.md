# Comparing `tmp/xia_api-0.1.20-cp39-none-win_amd64.whl.zip` & `tmp/xia_api-0.1.21-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 386111 bytes, number of entries: 9
--rw-r--r--  2.0 unx      498 b- defN 23-Jun-26 08:24 xia_api/__init__.py
--rw-r--r--  2.0 unx   259072 b- defN 23-Jun-26 08:26 xia_api/auth_client.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   313856 b- defN 23-Jun-26 08:28 xia_api/message.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   416768 b- defN 23-Jun-26 08:30 xia_api/rest.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 08:30 xia_api-0.1.20.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      677 b- defN 23-Jun-26 08:30 xia_api-0.1.20.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 08:30 xia_api-0.1.20.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-26 08:30 xia_api-0.1.20.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 23-Jun-26 08:30 xia_api-0.1.20.dist-info/RECORD
-9 files, 991876 bytes uncompressed, 384825 bytes compressed:  61.2%
+Zip file size: 7953 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      497 b- defN 23-Jun-29 20:33 xia_api/__init__.py
+-rw-r--r--  2.0 unx     1577 b- defN 23-Jun-29 20:33 xia_api/auth_client.py
+-rw-r--r--  2.0 unx     2329 b- defN 23-Jun-29 20:33 xia_api/message.py
+-rw-r--r--  2.0 unx    18688 b- defN 23-Jun-29 20:33 xia_api/rest.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      677 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      694 b- defN 23-Jun-29 20:37 xia_api-0.1.21.dist-info/RECORD
+9 files, 24720 bytes uncompressed, 6763 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_api/__init__.py
 Comment: 
 
-Filename: xia_api/auth_client.cp39-win_amd64.pyd
+Filename: xia_api/auth_client.py
 Comment: 
 
-Filename: xia_api/message.cp39-win_amd64.pyd
+Filename: xia_api/message.py
 Comment: 
 
-Filename: xia_api/rest.cp39-win_amd64.pyd
+Filename: xia_api/rest.py
 Comment: 
 
-Filename: xia_api-0.1.20.dist-info/LICENSE.txt
+Filename: xia_api-0.1.21.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_api-0.1.20.dist-info/METADATA
+Filename: xia_api-0.1.21.dist-info/METADATA
 Comment: 
 
-Filename: xia_api-0.1.20.dist-info/WHEEL
+Filename: xia_api-0.1.21.dist-info/WHEEL
 Comment: 
 
-Filename: xia_api-0.1.20.dist-info/top_level.txt
+Filename: xia_api-0.1.21.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_api-0.1.20.dist-info/RECORD
+Filename: xia_api-0.1.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_api/__init__.py

```diff
@@ -7,8 +7,8 @@
 __all__ = [
     "AuthClient",
     "RestApi", "error_handle",
     "XiaCollectionDeleteMsg", "XiaDocumentDeleteMsg", "XiaFileMsg", "XiaRecordBook", "XiaRecordItem",
     "XiaErrorMessage", "XiaActionResult"
 ]
 
-__version__ = "0.1.20"
+__version__ = "0.1.21"
```

## Comparing `xia_api-0.1.20.dist-info/METADATA` & `xia_api-0.1.21.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-api
-Version: 0.1.20
+Version: 0.1.21
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.20/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-api/0.1.21/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

