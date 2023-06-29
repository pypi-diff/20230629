# Comparing `tmp/xia_compiler_jsoneditor-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_jsoneditor-0.1.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 160446 bytes, number of entries: 7
--rw-r--r--  2.0 unx      135 b- defN 23-Jun-26 05:44 xia_compiler_jsoneditor/__init__.py
--rw-r--r--  2.0 unx   433664 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      687 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       24 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      669 b- defN 23-Jun-26 05:46 xia_compiler_jsoneditor-0.1.3.dist-info/RECORD
-7 files, 435429 bytes uncompressed, 159234 bytes compressed:  63.4%
+Zip file size: 6527 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      134 b- defN 23-Jun-29 20:38 xia_compiler_jsoneditor/__init__.py
+-rw-r--r--  2.0 unx    20330 b- defN 23-Jun-29 20:04 xia_compiler_jsoneditor/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      687 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       24 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      652 b- defN 23-Jun-29 20:42 xia_compiler_jsoneditor-0.1.4.dist-info/RECORD
+7 files, 22077 bytes uncompressed, 5347 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_jsoneditor/__init__.py
 Comment: 
 
-Filename: xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_jsoneditor/compiler.py
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.3.dist-info/LICENSE.txt
+Filename: xia_compiler_jsoneditor-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.3.dist-info/METADATA
+Filename: xia_compiler_jsoneditor-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.3.dist-info/WHEEL
+Filename: xia_compiler_jsoneditor-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.3.dist-info/top_level.txt
+Filename: xia_compiler_jsoneditor-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_jsoneditor-0.1.3.dist-info/RECORD
+Filename: xia_compiler_jsoneditor-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_jsoneditor/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_jsoneditor.compiler import XiaCompilerJsoneditor
 
 
 __all__ = [
     "XiaCompilerJsoneditor",
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_compiler_jsoneditor-0.1.3.dist-info/METADATA` & `xia_compiler_jsoneditor-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-jsoneditor
-Version: 0.1.3
+Version: 0.1.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.1.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-jsoneditor/0.1.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_jsoneditor-0.1.3.dist-info/RECORD` & `xia_compiler_jsoneditor-0.1.4.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_jsoneditor/__init__.py,sha256=ZXD-mhJFq7HFFKdIdEzbg-xR_pIa4_poiD_woId5_G0,135
-xia_compiler_jsoneditor/compiler.cp39-win_amd64.pyd,sha256=9805ujH3x3DvuvZG4GB6ybDlRS8UkisOP9P0jwZmh8o,433664
-xia_compiler_jsoneditor-0.1.3.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_compiler_jsoneditor-0.1.3.dist-info/METADATA,sha256=lfh8jzN2gOeylAZrtVKFqgG9F9pX2IFoP9kQYrUw5ec,687
-xia_compiler_jsoneditor-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_compiler_jsoneditor-0.1.3.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
-xia_compiler_jsoneditor-0.1.3.dist-info/RECORD,,
+xia_compiler_jsoneditor/__init__.py,sha256=GqP4j9yrvPK3Y4_gxMnpG0W1WKBZrB6oBoMedHY40QA,134
+xia_compiler_jsoneditor/compiler.py,sha256=K3ab4LCAp80HHH5Ui-5CdTeIfxQ4gCDrXTlofByvMyI,20330
+xia_compiler_jsoneditor-0.1.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_compiler_jsoneditor-0.1.4.dist-info/METADATA,sha256=E1Vtjn5ww41ajqGll25wT0bE8lqnSEmUq620AkY2BOM,687
+xia_compiler_jsoneditor-0.1.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_compiler_jsoneditor-0.1.4.dist-info/top_level.txt,sha256=oY6KydARRKWB_3q2LeXeIeKJVyZ1d54IIkH9htejhKA,24
+xia_compiler_jsoneditor-0.1.4.dist-info/RECORD,,
```

