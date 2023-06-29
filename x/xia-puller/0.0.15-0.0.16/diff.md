# Comparing `tmp/xia_puller-0.0.15-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller-0.0.16-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 114793 bytes, number of entries: 7
--rw-r--r--  2.0 unx       89 b- defN 23-Jun-29 13:27 xia_puller/__init__.py
--rw-r--r--  2.0 unx   278528 b- defN 23-Jun-29 13:29 xia_puller/puller.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 13:29 xia_puller-0.0.15.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 13:29 xia_puller-0.0.15.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 13:29 xia_puller-0.0.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 13:29 xia_puller-0.0.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      580 b- defN 23-Jun-29 13:29 xia_puller-0.0.15.dist-info/RECORD
+-rw-r--r--  2.0 unx       89 b- defN 23-Jun-29 13:29 xia_puller/__init__.py
+-rw-r--r--  2.0 unx   278528 b- defN 23-Jun-29 13:31 xia_puller/puller.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 13:31 xia_puller-0.0.16.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 13:31 xia_puller-0.0.16.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 13:31 xia_puller-0.0.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-29 13:31 xia_puller-0.0.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      580 b- defN 23-Jun-29 13:31 xia_puller-0.0.16.dist-info/RECORD
 7 files, 280149 bytes uncompressed, 113757 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller/__init__.py
 Comment: 
 
 Filename: xia_puller/puller.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_puller-0.0.15.dist-info/LICENSE.txt
+Filename: xia_puller-0.0.16.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller-0.0.15.dist-info/METADATA
+Filename: xia_puller-0.0.16.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller-0.0.15.dist-info/WHEEL
+Filename: xia_puller-0.0.16.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller-0.0.15.dist-info/top_level.txt
+Filename: xia_puller-0.0.16.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller-0.0.15.dist-info/RECORD
+Filename: xia_puller-0.0.16.dist-info/RECORD
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
 
-__version__ = "0.0.15"
+__version__ = "0.0.16"
```

## Comparing `xia_puller-0.0.15.dist-info/METADATA` & `xia_puller-0.0.16.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-puller
-Version: 0.0.15
+Version: 0.0.16
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-puller/0.0.15/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-puller/0.0.16/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_puller-0.0.15.dist-info/RECORD` & `xia_puller-0.0.16.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_puller/__init__.py,sha256=1T9wTanGGyqzb7eJenskUP0jin91t87uoRY-2LZyF_s,89
-xia_puller/puller.cp39-win_amd64.pyd,sha256=NurkRsDJUx7tkYXrYcx6HT-jk-pvIVf-Li4WAG_i2To,278528
-xia_puller-0.0.15.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
-xia_puller-0.0.15.dist-info/METADATA,sha256=EQIMee8ySO1cwFrGlIWhbsa64KcgI1auOcjz8LPFeSA,691
-xia_puller-0.0.15.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_puller-0.0.15.dist-info/top_level.txt,sha256=KwFMsBZetO5LVySeImHzwv2JRXsPMNsvbYgFiOGaNAE,11
-xia_puller-0.0.15.dist-info/RECORD,,
+xia_puller/__init__.py,sha256=qjfslTo326rKSynODmeOwUUhD3n9sgHkpOljXWDFP-A,89
+xia_puller/puller.cp39-win_amd64.pyd,sha256=6B6r75mL9GRxX2rthfon-agBWtAN_fMf0HDIjQaWndc,278528
+xia_puller-0.0.16.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_puller-0.0.16.dist-info/METADATA,sha256=GdkANqLjJjQrkJVSHSgAsrWJhsm8H4-TkguNwjlDpiA,691
+xia_puller-0.0.16.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_puller-0.0.16.dist-info/top_level.txt,sha256=KwFMsBZetO5LVySeImHzwv2JRXsPMNsvbYgFiOGaNAE,11
+xia_puller-0.0.16.dist-info/RECORD,,
```

