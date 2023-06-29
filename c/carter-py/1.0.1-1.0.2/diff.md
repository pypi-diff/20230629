# Comparing `tmp/carter_py-1.0.1-py3-none-any.whl.zip` & `tmp/carter_py-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 8208 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       67 b- defN 23-Apr-15 11:17 carterpy/__init__.py
 -rw-rw-rw-  2.0 fat     3249 b- defN 23-Jun-10 19:44 carterpy/async_carter.py
 -rw-rw-rw-  2.0 fat     3161 b- defN 23-Jun-10 19:48 carterpy/carter.py
 -rw-rw-rw-  2.0 fat     2763 b- defN 23-Jun-10 19:49 carterpy/classes.py
--rw-rw-rw-  2.0 fat      466 b- defN 23-Jun-25 22:55 carterpy/utils.py
--rw-rw-rw-  2.0 fat     8919 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/license.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      779 b- defN 23-Jun-25 22:59 carter_py-1.0.1.dist-info/RECORD
-10 files, 20580 bytes uncompressed, 6884 bytes compressed:  66.6%
+-rw-rw-rw-  2.0 fat      467 b- defN 23-Jun-29 19:34 carterpy/utils.py
+-rw-rw-rw-  2.0 fat     8919 b- defN 23-Jun-29 19:37 carter_py-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 19:37 carter_py-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1075 b- defN 23-Jun-29 19:37 carter_py-1.0.2.dist-info/license.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-29 19:37 carter_py-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      779 b- defN 23-Jun-29 19:37 carter_py-1.0.2.dist-info/RECORD
+10 files, 20581 bytes uncompressed, 6884 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: carterpy/classes.py
 Comment: 
 
 Filename: carterpy/utils.py
 Comment: 
 
-Filename: carter_py-1.0.1.dist-info/METADATA
+Filename: carter_py-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: carter_py-1.0.1.dist-info/WHEEL
+Filename: carter_py-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: carter_py-1.0.1.dist-info/license.txt
+Filename: carter_py-1.0.2.dist-info/license.txt
 Comment: 
 
-Filename: carter_py-1.0.1.dist-info/top_level.txt
+Filename: carter_py-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: carter_py-1.0.1.dist-info/RECORD
+Filename: carter_py-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## carterpy/utils.py

```diff
@@ -1,11 +1,11 @@
 import datetime
 
 URLS = {
-    "say": "https://api.carterlabs.ai/api/say",
+    "say": "https://api.carterlabs.ai/api/chat",
     "opener": "https://api.carterlabs.ai/api/opener",
     "personalise": "https://api.carterlabs.ai/api/personalise",
 }
 
 def convert_to_string(variable_name, value):
     try:
         return str(value)
```

## Comparing `carter_py-1.0.1.dist-info/METADATA` & `carter_py-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carter-py
-Version: 1.0.1
+Version: 1.0.2
 Summary: A wrapper for the Carter API
 Home-page: https://github.com/LazyLyrics/carter-py
 Author: LazyLyrics
 Author-email: lazylyrics@icloud.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `carter_py-1.0.1.dist-info/license.txt` & `carter_py-1.0.2.dist-info/license.txt`

 * *Files identical despite different names*

