# Comparing `tmp/xia_storer_gcs-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_storer_gcs-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 128519 bytes, number of entries: 7
--rw-r--r--  2.0 unx       84 b- defN 23-Jun-26 18:48 xia_storer_gcs/__init__.py
--rw-r--r--  2.0 unx   318976 b- defN 23-Jun-26 18:51 xia_storer_gcs/storer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:51 xia_storer_gcs-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-26 18:51 xia_storer_gcs-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:51 xia_storer_gcs-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-26 18:51 xia_storer_gcs-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      603 b- defN 23-Jun-26 18:51 xia_storer_gcs-0.0.3.dist-info/RECORD
-7 files, 320654 bytes uncompressed, 127437 bytes compressed:  60.3%
+Zip file size: 2961 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       83 b- defN 23-Jun-29 20:59 xia_storer_gcs/__init__.py
+-rw-r--r--  2.0 unx     2653 b- defN 23-Jun-29 20:59 xia_storer_gcs/storer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      585 b- defN 23-Jun-29 21:02 xia_storer_gcs-0.0.4.dist-info/RECORD
+7 files, 4312 bytes uncompressed, 1911 bytes compressed:  55.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_storer_gcs/__init__.py
 Comment: 
 
-Filename: xia_storer_gcs/storer.cp39-win_amd64.pyd
+Filename: xia_storer_gcs/storer.py
 Comment: 
 
-Filename: xia_storer_gcs-0.0.3.dist-info/LICENSE.txt
+Filename: xia_storer_gcs-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.3.dist-info/METADATA
+Filename: xia_storer_gcs-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_storer_gcs-0.0.3.dist-info/WHEEL
+Filename: xia_storer_gcs-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_storer_gcs-0.0.3.dist-info/top_level.txt
+Filename: xia_storer_gcs-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_storer_gcs-0.0.3.dist-info/RECORD
+Filename: xia_storer_gcs-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_storer_gcs/__init__.py

```diff
@@ -1,8 +1,8 @@
 from storer import GcsStorer
 
 __all__ = [
     "GcsStorer"
 ]
 
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_storer_gcs-0.0.3.dist-info/METADATA` & `xia_storer_gcs-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-storer-gcs
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-storer-gcs/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-storer-gcs/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

