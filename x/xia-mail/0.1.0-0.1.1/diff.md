# Comparing `tmp/xia_mail-0.1.0-cp39-none-win_amd64.whl.zip` & `tmp/xia_mail-0.1.1-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 120427 bytes, number of entries: 7
--rw-r--r--  2.0 unx      139 b- defN 23-Jun-26 18:45 xia_mail/__init__.py
--rw-r--r--  2.0 unx   297472 b- defN 23-Jun-26 18:47 xia_mail/mail.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:47 xia_mail-0.1.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      721 b- defN 23-Jun-26 18:47 xia_mail-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:47 xia_mail-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-26 18:47 xia_mail-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      559 b- defN 23-Jun-26 18:47 xia_mail-0.1.0.dist-info/RECORD
-7 files, 299150 bytes uncompressed, 119433 bytes compressed:  60.1%
+Zip file size: 2951 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      138 b- defN 23-Jun-29 20:53 xia_mail/__init__.py
+-rw-r--r--  2.0 unx     2683 b- defN 23-Jun-29 20:12 xia_mail/mail.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:57 xia_mail-0.1.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      721 b- defN 23-Jun-29 20:57 xia_mail-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:57 xia_mail-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-29 20:57 xia_mail-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      541 b- defN 23-Jun-29 20:57 xia_mail-0.1.1.dist-info/RECORD
+7 files, 4342 bytes uncompressed, 1989 bytes compressed:  54.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_mail/__init__.py
 Comment: 
 
-Filename: xia_mail/mail.cp39-win_amd64.pyd
+Filename: xia_mail/mail.py
 Comment: 
 
-Filename: xia_mail-0.1.0.dist-info/LICENSE.txt
+Filename: xia_mail-0.1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_mail-0.1.0.dist-info/METADATA
+Filename: xia_mail-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: xia_mail-0.1.0.dist-info/WHEEL
+Filename: xia_mail-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: xia_mail-0.1.0.dist-info/top_level.txt
+Filename: xia_mail-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_mail-0.1.0.dist-info/RECORD
+Filename: xia_mail-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_mail/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_mail.mail import MailField, MailAttachment, Mail
 
 
 __all__ = [
     "MailField", "MailAttachment", "Mail"
 ]
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## Comparing `xia_mail-0.1.0.dist-info/METADATA` & `xia_mail-0.1.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-mail
-Version: 0.1.0
+Version: 0.1.1
 Summary: X-I-A Mail Standard
-Home-page: https://develop.x-i-a.com/docs/xia-mail/0.1.0/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-mail/0.1.1/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

