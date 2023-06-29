# Comparing `tmp/xia_compiler_openapi-0.1.18-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_openapi-0.1.19-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 211765 bytes, number of entries: 7
--rw-r--r--  2.0 unx      127 b- defN 23-Jun-26 05:43 xia_compiler_openapi/__init__.py
--rw-r--r--  2.0 unx   600064 b- defN 23-Jun-26 05:46 xia_compiler_openapi/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 05:46 xia_compiler_openapi-0.1.18.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      697 b- defN 23-Jun-26 05:46 xia_compiler_openapi-0.1.18.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 05:46 xia_compiler_openapi-0.1.18.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-26 05:46 xia_compiler_openapi-0.1.18.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      653 b- defN 23-Jun-26 05:46 xia_compiler_openapi-0.1.18.dist-info/RECORD
-7 files, 601812 bytes uncompressed, 210585 bytes compressed:  65.0%
+Zip file size: 9021 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      126 b- defN 23-Jun-29 20:40 xia_compiler_openapi/__init__.py
+-rw-r--r--  2.0 unx    38580 b- defN 23-Jun-29 20:40 xia_compiler_openapi/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      697 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      636 b- defN 23-Jun-29 20:42 xia_compiler_openapi-0.1.19.dist-info/RECORD
+7 files, 40310 bytes uncompressed, 7873 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_openapi/__init__.py
 Comment: 
 
-Filename: xia_compiler_openapi/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_openapi/compiler.py
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.18.dist-info/LICENSE.txt
+Filename: xia_compiler_openapi-0.1.19.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.18.dist-info/METADATA
+Filename: xia_compiler_openapi-0.1.19.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.18.dist-info/WHEEL
+Filename: xia_compiler_openapi-0.1.19.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.18.dist-info/top_level.txt
+Filename: xia_compiler_openapi-0.1.19.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_openapi-0.1.18.dist-info/RECORD
+Filename: xia_compiler_openapi-0.1.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_openapi/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_openapi.compiler import XiaCompilerOpenapi
 
 
 __all__ = [
     "XiaCompilerOpenapi",
 ]
 
-__version__ = "0.1.18"
+__version__ = "0.1.19"
```

## Comparing `xia_compiler_openapi-0.1.18.dist-info/METADATA` & `xia_compiler_openapi-0.1.19.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-openapi
-Version: 0.1.18
+Version: 0.1.19
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.18/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-openapi/0.1.19/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_compiler_openapi-0.1.18.dist-info/RECORD` & `xia_compiler_openapi-0.1.19.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_compiler_openapi/__init__.py,sha256=lDxzrGiCPsua7IwZJZ7vAJXxXefh6RsCoN7dzj9Z1qg,127
-xia_compiler_openapi/compiler.cp39-win_amd64.pyd,sha256=CNwBCgu-agGu-Oz8AOAshpO1r-DwDmeyUQuBkLDqW-g,600064
-xia_compiler_openapi-0.1.18.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_compiler_openapi-0.1.18.dist-info/METADATA,sha256=5ScR74uQYOTxCZcG0ZbN1WA6gdEEJ_gxBC6Wg0bHhH0,697
-xia_compiler_openapi-0.1.18.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_compiler_openapi-0.1.18.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
-xia_compiler_openapi-0.1.18.dist-info/RECORD,,
+xia_compiler_openapi/__init__.py,sha256=6er_biek0yxH-9w7OlvA-BOaIEmU9ZIb8miBCdvRJMU,126
+xia_compiler_openapi/compiler.py,sha256=eYWb4yMzaeDsYyf8UyaV0Dv7gWn4kBvX3clv2LfxurM,38580
+xia_compiler_openapi-0.1.19.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_compiler_openapi-0.1.19.dist-info/METADATA,sha256=c52rbUDrCExKBdtBxU5Th_ehJWUbICh2ob5MGoHkwxc,697
+xia_compiler_openapi-0.1.19.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_compiler_openapi-0.1.19.dist-info/top_level.txt,sha256=l-dHwHri9HVBghJIDfyblbK8E8exERfi3dhMi7vW3bE,21
+xia_compiler_openapi-0.1.19.dist-info/RECORD,,
```

