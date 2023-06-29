# Comparing `tmp/xia_engine_test-0.1.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_test-0.1.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 339670 bytes, number of entries: 9
--rw-r--r--  2.0 unx      308 b- defN 23-Jun-25 21:12 xia_engine_test/__init__.py
--rw-r--r--  2.0 unx   305152 b- defN 23-Jun-25 21:19 xia_engine_test/document_example.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   293888 b- defN 23-Jun-25 21:17 xia_engine_test/field_test.cp39-win_amd64.pyd
--rw-r--r--  2.0 unx   265728 b- defN 23-Jun-25 21:15 xia_engine_test/models.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 21:19 xia_engine_test-0.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      853 b- defN 23-Jun-25 21:19 xia_engine_test-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 21:19 xia_engine_test-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-25 21:19 xia_engine_test-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      825 b- defN 23-Jun-25 21:19 xia_engine_test-0.1.2.dist-info/RECORD
-9 files, 867020 bytes uncompressed, 338230 bytes compressed:  61.0%
+Zip file size: 4264 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      307 b- defN 23-Jun-29 20:47 xia_engine_test/__init__.py
+-rw-r--r--  2.0 unx     2338 b- defN 23-Jun-29 20:09 xia_engine_test/document_example.py
+-rw-r--r--  2.0 unx     6563 b- defN 23-Jun-29 20:09 xia_engine_test/field_test.py
+-rw-r--r--  2.0 unx      627 b- defN 23-Jun-29 20:09 xia_engine_test/models.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      853 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      770 b- defN 23-Jun-29 20:50 xia_engine_test-0.1.3.dist-info/RECORD
+9 files, 11724 bytes uncompressed, 2920 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
 Filename: xia_engine_test/__init__.py
 Comment: 
 
-Filename: xia_engine_test/document_example.cp39-win_amd64.pyd
+Filename: xia_engine_test/document_example.py
 Comment: 
 
-Filename: xia_engine_test/field_test.cp39-win_amd64.pyd
+Filename: xia_engine_test/field_test.py
 Comment: 
 
-Filename: xia_engine_test/models.cp39-win_amd64.pyd
+Filename: xia_engine_test/models.py
 Comment: 
 
-Filename: xia_engine_test-0.1.2.dist-info/LICENSE.txt
+Filename: xia_engine_test-0.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.2.dist-info/METADATA
+Filename: xia_engine_test-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_test-0.1.2.dist-info/WHEEL
+Filename: xia_engine_test-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_test-0.1.2.dist-info/top_level.txt
+Filename: xia_engine_test-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_test-0.1.2.dist-info/RECORD
+Filename: xia_engine_test-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_test/__init__.py

```diff
@@ -5,8 +5,8 @@
 __all__ = [
     "FieldTest",
     "MessageHello", "DocumentSimple", "External",
     "DocumentBasic"
 ]
 
 
-__version__ = "0.1.2"
+__version__ = "0.1.3"
```

## Comparing `xia_engine_test-0.1.2.dist-info/METADATA` & `xia_engine_test-0.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-test
-Version: 0.1.2
+Version: 0.1.3
 Summary: X-I-A Engine Test Suite
-Home-page: https://develop.x-i-a.com/docs/xia-engine-test/0.1.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-test/0.1.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_test-0.1.2.dist-info/RECORD` & `xia_engine_test-0.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-xia_engine_test/__init__.py,sha256=LUTQ0V9l2HXag_IgFpnh0h8bXouCdyUfuRGsYUJuIvk,308
-xia_engine_test/document_example.cp39-win_amd64.pyd,sha256=nLqdZkli5sS4CodKbCEQNvQCj9oNi6L3QTh-J61wxRQ,305152
-xia_engine_test/field_test.cp39-win_amd64.pyd,sha256=MLh_IpUz9YsIif779nPE3HCSw0OyOIm_UeAYEiDRqaM,293888
-xia_engine_test/models.cp39-win_amd64.pyd,sha256=SiGUuOIlWEjjqn1BQGzwdd-cj1Xx0Q9dh-1-aRBRv48,265728
-xia_engine_test-0.1.2.dist-info/LICENSE.txt,sha256=YN4tZxdLShKEJg_dqPpbMkiYPRURlsJaFLM0qCep1yU,151
-xia_engine_test-0.1.2.dist-info/METADATA,sha256=-ZUbajdGbqzaVKyFJPefNMia0igeFRDVuik8hlr6atg,853
-xia_engine_test-0.1.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_test-0.1.2.dist-info/top_level.txt,sha256=lNzim7ax9-cnURpBE9M4WcBlHouRrTJJeqeGcQEemxE,16
-xia_engine_test-0.1.2.dist-info/RECORD,,
+xia_engine_test/__init__.py,sha256=qs1HJPHUJXXlo8xOMu-jDTkYeUNFZPfATssDj8WfwTw,307
+xia_engine_test/document_example.py,sha256=sA-t9d452ltCG6JuVpflJ8jcgwcPZpy6L1Aw6fYXkDg,2338
+xia_engine_test/field_test.py,sha256=2AHygYE8p1RJptKq2PpOvEBJKTB7nO7hLLpJuEpXJck,6563
+xia_engine_test/models.py,sha256=-1aik7CVjvi_N_zg33rfGWIZGOoWRvzOyqyI1xxoow8,627
+xia_engine_test-0.1.3.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_test-0.1.3.dist-info/METADATA,sha256=ChiowJvr4l4OE5YgsKlXZI5vCdkIMtdd5fkJ4FOIe9M,853
+xia_engine_test-0.1.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_test-0.1.3.dist-info/top_level.txt,sha256=lNzim7ax9-cnURpBE9M4WcBlHouRrTJJeqeGcQEemxE,16
+xia_engine_test-0.1.3.dist-info/RECORD,,
```

