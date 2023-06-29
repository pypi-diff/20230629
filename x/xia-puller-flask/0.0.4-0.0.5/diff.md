# Comparing `tmp/xia_puller_flask-0.0.4-cp39-none-win_amd64.whl.zip` & `tmp/xia_puller_flask-0.0.5-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 111131 bytes, number of entries: 7
--rw-r--r--  2.0 unx       97 b- defN 23-Jun-26 18:04 xia_puller_flask/__init__.py
--rw-r--r--  2.0 unx   269312 b- defN 23-Jun-26 18:06 xia_puller_flask/api.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:06 xia_puller_flask-0.0.4.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      714 b- defN 23-Jun-26 18:06 xia_puller_flask-0.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:06 xia_puller_flask-0.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-26 18:06 xia_puller_flask-0.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      614 b- defN 23-Jun-26 18:06 xia_puller_flask-0.0.4.dist-info/RECORD
-7 files, 271004 bytes uncompressed, 110027 bytes compressed:  59.4%
+Zip file size: 2551 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       97 b- defN 23-Jun-29 08:52 xia_puller_flask/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-Jun-26 18:04 xia_puller_flask/api.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 08:52 xia_puller_flask-0.0.5.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      714 b- defN 23-Jun-29 08:52 xia_puller_flask-0.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 08:52 xia_puller_flask-0.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-29 08:52 xia_puller_flask-0.0.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      596 b- defN 23-Jun-29 08:52 xia_puller_flask-0.0.5.dist-info/RECORD
+7 files, 2778 bytes uncompressed, 1479 bytes compressed:  46.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_puller_flask/__init__.py
 Comment: 
 
-Filename: xia_puller_flask/api.cp39-win_amd64.pyd
+Filename: xia_puller_flask/api.py
 Comment: 
 
-Filename: xia_puller_flask-0.0.4.dist-info/LICENSE.txt
+Filename: xia_puller_flask-0.0.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.4.dist-info/METADATA
+Filename: xia_puller_flask-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: xia_puller_flask-0.0.4.dist-info/WHEEL
+Filename: xia_puller_flask-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: xia_puller_flask-0.0.4.dist-info/top_level.txt
+Filename: xia_puller_flask-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_puller_flask-0.0.4.dist-info/RECORD
+Filename: xia_puller_flask-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_puller_flask/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_puller_flask.api import PullerApi
 
 __all__ = [
     "PullerApi"
 ]
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
```

## Comparing `xia_puller_flask-0.0.4.dist-info/METADATA` & `xia_puller_flask-0.0.5.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-puller-flask
-Version: 0.0.4
+Version: 0.0.5
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-puller-flask/0.0.4/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-puller-flask/0.0.5/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_puller_flask-0.0.4.dist-info/RECORD` & `xia_puller_flask-0.0.5.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_puller_flask/__init__.py,sha256=ezd8G8ZLdLa2nDCkAALLlhV34mo0QlTn5kQIzJftdAc,97
-xia_puller_flask/api.cp39-win_amd64.pyd,sha256=Iczs9qy25iR-LNTskuxsbibakcy_IoGHHK78X020dCM,269312
-xia_puller_flask-0.0.4.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_puller_flask-0.0.4.dist-info/METADATA,sha256=e9ZIn1nmaAsEXzo82d6siV79mewJLtCi1rG8pvG---o,714
-xia_puller_flask-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_puller_flask-0.0.4.dist-info/top_level.txt,sha256=1L3f8B1GOTeCgn915g1myzSBbN-3IeHhv_zU2W0cmrE,17
-xia_puller_flask-0.0.4.dist-info/RECORD,,
+xia_puller_flask/__init__.py,sha256=LM-K852mAuZp2bWhFAMN2z1PcDXq-jD1p5oUCt4HXvk,97
+xia_puller_flask/api.py,sha256=f8wnWHHisVLGbyzHs1v3EvLdMgS9CfTG9013xtX--4k,1104
+xia_puller_flask-0.0.5.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_puller_flask-0.0.5.dist-info/METADATA,sha256=d3zpMEM6vvWq1k3juowkhAWo3QOFUdytkCS5iOONZGA,714
+xia_puller_flask-0.0.5.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_puller_flask-0.0.5.dist-info/top_level.txt,sha256=1L3f8B1GOTeCgn915g1myzSBbN-3IeHhv_zU2W0cmrE,17
+xia_puller_flask-0.0.5.dist-info/RECORD,,
```

