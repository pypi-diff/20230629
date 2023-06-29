# Comparing `tmp/xia_git-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_git-0.1.3-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 130653 bytes, number of entries: 7
--rw-r--r--  2.0 unx       76 b- defN 23-Jun-29 05:29 xia_git/__init__.py
--rw-r--r--  2.0 unx   327168 b- defN 23-Jun-29 05:32 xia_git/git.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 05:32 xia_git-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      625 b- defN 23-Jun-29 05:32 xia_git-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 05:32 xia_git-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 05:32 xia_git-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      550 b- defN 23-Jun-29 05:32 xia_git-0.1.2.dist-info/RECORD
-7 files, 328677 bytes uncompressed, 129675 bytes compressed:  60.5%
+Zip file size: 3431 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       75 b- defN 23-Jun-29 20:50 xia_git/__init__.py
+-rw-r--r--  2.0 unx     5437 b- defN 23-Jun-29 20:50 xia_git/git.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:50 xia_git-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      625 b- defN 23-Jun-29 20:50 xia_git-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:50 xia_git-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-29 20:50 xia_git-0.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      533 b- defN 23-Jun-29 20:50 xia_git-0.1.3.dist-info/RECORD
+7 files, 6937 bytes uncompressed, 2485 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_git/__init__.py
 Comment: 
 
-Filename: xia_git/git.cp39-win_amd64.pyd
+Filename: xia_git/git.py
 Comment: 
 
-Filename: xia_git-0.1.2.dist-info/LICENSE.txt
+Filename: xia_git-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_git-0.1.2.dist-info/METADATA
+Filename: xia_git-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_git-0.1.2.dist-info/WHEEL
+Filename: xia_git-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_git-0.1.2.dist-info/top_level.txt
+Filename: xia_git-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_git-0.1.2.dist-info/RECORD
+Filename: xia_git-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_git/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_git.git import Git
 
 __all__ = [
     "Git"
 ]
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_git-0.1.2.dist-info/METADATA` & `xia_git-0.1.3.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-git
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-git/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-git/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

