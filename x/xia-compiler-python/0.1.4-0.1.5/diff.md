# Comparing `tmp/xia_compiler_python-0.1.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_compiler_python-0.1.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 152592 bytes, number of entries: 7
--rw-r--r--  2.0 unx      116 b- defN 23-Jun-26 05:22 xia_compiler_python/__init__.py
--rw-r--r--  2.0 unx   390656 b- defN 23-Jun-26 05:25 xia_compiler_python/compiler.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 05:25 xia_compiler_python-0.1.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      674 b- defN 23-Jun-26 05:25 xia_compiler_python-0.1.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 05:25 xia_compiler_python-0.1.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jun-26 05:25 xia_compiler_python-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 23-Jun-26 05:25 xia_compiler_python-0.1.4.dist-info/RECORD
-7 files, 392357 bytes uncompressed, 151436 bytes compressed:  61.4%
+Zip file size: 5202 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      115 b- defN 23-Jun-29 20:40 xia_compiler_python/__init__.py
+-rw-r--r--  2.0 unx    14558 b- defN 23-Jun-29 14:55 xia_compiler_python/compiler.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      674 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      624 b- defN 23-Jun-29 20:44 xia_compiler_python-0.1.5.dist-info/RECORD
+7 files, 16241 bytes uncompressed, 4078 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_compiler_python/__init__.py
 Comment: 
 
-Filename: xia_compiler_python/compiler.cp39-win_amd64.pyd
+Filename: xia_compiler_python/compiler.py
 Comment: 
 
-Filename: xia_compiler_python-0.1.4.dist-info/LICENSE.txt
+Filename: xia_compiler_python-0.1.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.4.dist-info/METADATA
+Filename: xia_compiler_python-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_compiler_python-0.1.4.dist-info/WHEEL
+Filename: xia_compiler_python-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_compiler_python-0.1.4.dist-info/top_level.txt
+Filename: xia_compiler_python-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_compiler_python-0.1.4.dist-info/RECORD
+Filename: xia_compiler_python-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_compiler_python/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_compiler_python.compiler import PythonCompiler
 
 
 __all__ = [
     "PythonCompiler"
 ]
 
-__version__ = "0.1.4"
+__version__ = "0.1.5"
```

## Comparing `xia_compiler_python-0.1.4.dist-info/METADATA` & `xia_compiler_python-0.1.5.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-compiler-python
-Version: 0.1.4
+Version: 0.1.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-compiler-python/0.1.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-compiler-python/0.1.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

