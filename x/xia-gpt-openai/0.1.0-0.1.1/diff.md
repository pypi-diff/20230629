# Comparing `tmp/xia_gpt_openai-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_gpt_openai-0.1.1-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 114275 bytes, number of entries: 7
--rw-r--r--  2.0 unx       95 b- defN 23-Jun-25 20:28 xia_gpt_openai/__init__.py
--rw-r--r--  2.0 unx   279040 b- defN 23-Jun-25 20:31 xia_gpt_openai/gpt.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-25 20:31 xia_gpt_openai-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      673 b- defN 23-Jun-25 20:31 xia_gpt_openai-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-25 20:31 xia_gpt_openai-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Jun-25 20:31 xia_gpt_openai-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      600 b- defN 23-Jun-25 20:31 xia_gpt_openai-0.1.0.dist-info/RECORD
-7 files, 280673 bytes uncompressed, 113199 bytes compressed:  59.7%
+Zip file size: 2769 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       94 b- defN 23-Jun-29 20:51 xia_gpt_openai/__init__.py
+-rw-r--r--  2.0 unx     1724 b- defN 23-Jun-29 20:51 xia_gpt_openai/gpt.py
+-rw-r--r--  2.0 unx      151 b- defN 23-Jun-29 20:51 xia_gpt_openai-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      673 b- defN 23-Jun-29 20:51 xia_gpt_openai-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-Jun-29 20:51 xia_gpt_openai-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Jun-29 20:51 xia_gpt_openai-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      583 b- defN 23-Jun-29 20:51 xia_gpt_openai-0.1.1.dist-info/RECORD
+7 files, 3348 bytes uncompressed, 1725 bytes compressed:  48.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_gpt_openai/__init__.py
 Comment: 
 
-Filename: xia_gpt_openai/gpt.cp39-win_amd64.pyd
+Filename: xia_gpt_openai/gpt.py
 Comment: 
 
-Filename: xia_gpt_openai-0.1.0.dist-info/LICENSE.txt
+Filename: xia_gpt_openai-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.0.dist-info/METADATA
+Filename: xia_gpt_openai-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_gpt_openai-0.1.0.dist-info/WHEEL
+Filename: xia_gpt_openai-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_gpt_openai-0.1.0.dist-info/top_level.txt
+Filename: xia_gpt_openai-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_gpt_openai-0.1.0.dist-info/RECORD
+Filename: xia_gpt_openai-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_gpt_openai/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_gpt_openai.gpt import OpenaiGpt
 
 __all__ = [
     "OpenaiGpt"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_gpt_openai-0.1.0.dist-info/METADATA` & `xia_gpt_openai-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-gpt-openai
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-gpt-openai/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-gpt-openai/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_gpt_openai-0.1.0.dist-info/RECORD` & `xia_gpt_openai-0.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_gpt_openai/__init__.py,sha256=FOvrnU3nI17GQygwdFT2c2W7OCfYWyY7K3bMBkllGc8,95
-xia_gpt_openai/gpt.cp39-win_amd64.pyd,sha256=3y-3TggjFgga6pt1b7ZHFEfIAQ1ARfl5gQVy-3VwoEA,279040
-xia_gpt_openai-0.1.0.dist-info/LICENSE.txt,sha256=YN4tZxdLShKEJg_dqPpbMkiYPRURlsJaFLM0qCep1yU,151
-xia_gpt_openai-0.1.0.dist-info/METADATA,sha256=mIFceQtyUs5udp1T00CO2c2e8vU7JFKoRJLd9_gKIks,673
-xia_gpt_openai-0.1.0.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_gpt_openai-0.1.0.dist-info/top_level.txt,sha256=jfjlRNwHE1wgDClmy0nje2mJka0SPlg7iN9E3IKxRGM,15
-xia_gpt_openai-0.1.0.dist-info/RECORD,,
+xia_gpt_openai/__init__.py,sha256=oqHUBTWIK_HXsZ35qA8OkcE5XvdvJ8Vm76ueg-8dNqg,94
+xia_gpt_openai/gpt.py,sha256=CkS_FLsUXn_c7HG1tr81Sv9Ci43eNmWDDlRI5g36Cso,1724
+xia_gpt_openai-0.1.1.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_gpt_openai-0.1.1.dist-info/METADATA,sha256=rcIqToF_2kQsYfg4A7cG6zOpnGCAoo1sMrzhui3559U,673
+xia_gpt_openai-0.1.1.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_gpt_openai-0.1.1.dist-info/top_level.txt,sha256=jfjlRNwHE1wgDClmy0nje2mJka0SPlg7iN9E3IKxRGM,15
+xia_gpt_openai-0.1.1.dist-info/RECORD,,
```

