# Comparing `tmp/xia_mail_sender-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_mail_sender-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 104102 bytes, number of entries: 7
--rw-r--r--  2.0 unx      101 b- defN 23-Jun-28 05:27 xia_mail_sender/__init__.py
--rw-r--r--  2.0 unx   252416 b- defN 23-Jun-28 05:30 xia_mail_sender/sender.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-28 05:30 xia_mail_sender-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      714 b- defN 23-Jun-28 05:30 xia_mail_sender-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-28 05:30 xia_mail_sender-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-28 05:30 xia_mail_sender-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      611 b- defN 23-Jun-28 05:30 xia_mail_sender-0.1.0.dist-info/RECORD
-7 files, 254108 bytes uncompressed, 103006 bytes compressed:  59.5%
+Zip file size: 2609 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      100 b- defN 23-Jun-29 20:53 xia_mail_sender/__init__.py
+-rw-r--r--  2.0 unx     1333 b- defN 23-Jun-29 20:53 xia_mail_sender/sender.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      714 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      593 b- defN 23-Jun-29 20:56 xia_mail_sender-0.1.1.dist-info/RECORD
+7 files, 3006 bytes uncompressed, 1545 bytes compressed:  48.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_mail_sender/__init__.py
 Comment: 
 
-Filename: xia_mail_sender/sender.cp39-win_amd64.pyd
+Filename: xia_mail_sender/sender.py
 Comment: 
 
-Filename: xia_mail_sender-0.1.0.dist-info/LICENSE.txt
+Filename: xia_mail_sender-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.0.dist-info/METADATA
+Filename: xia_mail_sender-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_mail_sender-0.1.0.dist-info/WHEEL
+Filename: xia_mail_sender-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_mail_sender-0.1.0.dist-info/top_level.txt
+Filename: xia_mail_sender-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_mail_sender-0.1.0.dist-info/RECORD
+Filename: xia_mail_sender-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_mail_sender/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_mail_sender.sender import MailSender
 
 __all__ = [
     "MailSender"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_mail_sender-0.1.0.dist-info/METADATA` & `xia_mail_sender-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-mail-sender
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A Mail Sender
-Home-page: https://develop.x-i-a.com/docs/xia-mail-sender/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-mail-sender/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

