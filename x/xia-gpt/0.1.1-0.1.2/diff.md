# Comparing `tmp/xia_gpt-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt-0.1.2-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 100471 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-25 20:33 xia_gpt/__init__.py
--rw-r--r--  2.0 unx   245248 b- defN 23-Jun-25 20:35 xia_gpt/gpt.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 20:35 xia_gpt-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      600 b- defN 23-Jun-25 20:35 xia_gpt-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 20:35 xia_gpt-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-25 20:35 xia_gpt-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 23-Jun-25 20:35 xia_gpt-0.1.1.dist-info/RECORD
-7 files, 246732 bytes uncompressed, 99493 bytes compressed:  59.7%
+Zip file size: 2400 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-29 20:50 xia_gpt/__init__.py
+-rw-r--r--  2.0 unx     1049 b- defN 23-Jun-29 20:50 xia_gpt/gpt.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:50 xia_gpt-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      600 b- defN 23-Jun-29 20:50 xia_gpt-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:50 xia_gpt-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:50 xia_gpt-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      533 b- defN 23-Jun-29 20:50 xia_gpt-0.1.2.dist-info/RECORD
+7 files, 2524 bytes uncompressed, 1454 bytes compressed:  42.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt/__init__.py
 Comment: 
 
-Filename: xia_gpt/gpt.cp39-win_amd64.pyd
+Filename: xia_gpt/gpt.py
 Comment: 
 
-Filename: xia_gpt-0.1.1.dist-info/LICENSE.txt
+Filename: xia_gpt-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt-0.1.1.dist-info/METADATA
+Filename: xia_gpt-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt-0.1.1.dist-info/WHEEL
+Filename: xia_gpt-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt-0.1.1.dist-info/top_level.txt
+Filename: xia_gpt-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt-0.1.1.dist-info/RECORD
+Filename: xia_gpt-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt.gpt import Gpt
 
 __all__ = [
     "Gpt"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

