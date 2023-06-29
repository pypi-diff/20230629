# Comparing `tmp/xia_puller-0.0.11-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller-0.0.12-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 114790 bytes, number of entries: 7
--rw-r--r--  2.0 unx       89 b- defN 23-Jun-27 21:12 xia_puller/__init__.py
--rw-r--r--  2.0 unx   278528 b- defN 23-Jun-27 21:15 xia_puller/puller.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-27 21:15 xia_puller-0.0.11.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-27 21:15 xia_puller-0.0.11.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-27 21:15 xia_puller-0.0.11.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-27 21:15 xia_puller-0.0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      580 b- defN 23-Jun-27 21:15 xia_puller-0.0.11.dist-info/RECORD
-7 files, 280149 bytes uncompressed, 113754 bytes compressed:  59.4%
+Zip file size: 87113 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-29 08:00 xia_puller/__init__.py
+-rw-r--r--  2.0 unx   234960 b- defN 23-Jun-29 08:00 xia_puller/puller.cpython-39-darwin.so
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 08:00 xia_puller-0.0.12.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 08:00 xia_puller-0.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 08:00 xia_puller-0.0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 08:00 xia_puller-0.0.12.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-Jun-29 08:00 xia_puller-0.0.12.dist-info/RECORD
+7 files, 236593 bytes uncompressed, 86073 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller/__init__.py
 Comment: 
 
-Filename: xia_puller/puller.cp39-win_amd64.pyd
+Filename: xia_puller/puller.cpython-39-darwin.so
 Comment: 
 
-Filename: xia_puller-0.0.11.dist-info/LICENSE.txt
+Filename: xia_puller-0.0.12.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller-0.0.11.dist-info/METADATA
+Filename: xia_puller-0.0.12.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller-0.0.11.dist-info/WHEEL
+Filename: xia_puller-0.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller-0.0.11.dist-info/top_level.txt
+Filename: xia_puller-0.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller-0.0.11.dist-info/RECORD
+Filename: xia_puller-0.0.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_puller/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_puller.puller import Puller
 
 __all__ = [
     "Puller"
 ]
 
-__version__ = "0.0.11"
+__version__ = "0.0.12"
```

