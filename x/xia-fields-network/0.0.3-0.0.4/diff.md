# Comparing `tmp/xia_fields_network-0.0.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_fields_network-0.0.4-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 113453 bytes, number of entries: 7
--rw-r--r--  2.0 unx      172 b- defN 23-Jun-26 18:36 xia_fields_network/__init__.py
--rw-r--r--  2.0 unx   280576 b- defN 23-Jun-26 18:38 xia_fields_network/fields.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:38 xia_fields_network-0.0.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      670 b- defN 23-Jun-26 18:38 xia_fields_network-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:38 xia_fields_network-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-Jun-26 18:38 xia_fields_network-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      632 b- defN 23-Jun-26 18:38 xia_fields_network-0.0.3.dist-info/RECORD
-7 files, 282319 bytes uncompressed, 112315 bytes compressed:  60.2%
+Zip file size: 2714 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      171 b- defN 23-Jun-29 20:47 xia_fields_network/__init__.py
+-rw-r--r--  2.0 unx     2344 b- defN 23-Jun-29 20:47 xia_fields_network/fields.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      670 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      614 b- defN 23-Jun-29 20:51 xia_fields_network-0.0.4.dist-info/RECORD
+7 files, 4068 bytes uncompressed, 1608 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_fields_network/__init__.py
 Comment: 
 
-Filename: xia_fields_network/fields.cp39-win_amd64.pyd
+Filename: xia_fields_network/fields.py
 Comment: 
 
-Filename: xia_fields_network-0.0.3.dist-info/LICENSE.txt
+Filename: xia_fields_network-0.0.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_fields_network-0.0.3.dist-info/METADATA
+Filename: xia_fields_network-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_fields_network-0.0.3.dist-info/WHEEL
+Filename: xia_fields_network-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_fields_network-0.0.3.dist-info/top_level.txt
+Filename: xia_fields_network-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_fields_network-0.0.3.dist-info/RECORD
+Filename: xia_fields_network-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_fields_network/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_fields_network.fields import EmailField, IpField, IpV6Field, MacField
 
 
 __all__ = [
     "EmailField", "IpField", "IpV6Field", "MacField",
 ]
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

## Comparing `xia_fields_network-0.0.3.dist-info/METADATA` & `xia_fields_network-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-fields-network
-Version: 0.0.3
+Version: 0.0.4
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-fields-network/0.0.3/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-fields-network/0.0.4/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_fields_network-0.0.3.dist-info/RECORD` & `xia_fields_network-0.0.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_fields_network/__init__.py,sha256=G8ijcyTp4cHp6szS1z9e9FTAiQ4xQ4PZatyR-FdUuoo,172
-xia_fields_network/fields.cp39-win_amd64.pyd,sha256=_iT0Dp1AMY17z7mj5ogfB1GZ-IMt6w8JmV3RaDHyDs0,280576
-xia_fields_network-0.0.3.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_fields_network-0.0.3.dist-info/METADATA,sha256=dijx-9GluquYRYN0Ys2U3GnjEuK6-H-HLn_STKSfaOg,670
-xia_fields_network-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_fields_network-0.0.3.dist-info/top_level.txt,sha256=r_frVEKNN4Myp21gIzqk-TlQReQN_JQRxkBPOA3XPlc,19
-xia_fields_network-0.0.3.dist-info/RECORD,,
+xia_fields_network/__init__.py,sha256=7ECzh_QD-VDmaCKgsj5rulPn6e3jyNSsAaH9o9KylTA,171
+xia_fields_network/fields.py,sha256=lVx-M4Du8-aBK2F2WSuCuDZ7_QWE-J81MVbkXSMoDmU,2344
+xia_fields_network-0.0.4.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_fields_network-0.0.4.dist-info/METADATA,sha256=zXWkwoZt6ENEYY7p2RAzItCIHo3qCxdaS8A0mA_13I4,670
+xia_fields_network-0.0.4.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_fields_network-0.0.4.dist-info/top_level.txt,sha256=r_frVEKNN4Myp21gIzqk-TlQReQN_JQRxkBPOA3XPlc,19
+xia_fields_network-0.0.4.dist-info/RECORD,,
```

