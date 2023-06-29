# Comparing `tmp/xia_engine_terraform-0.1.16-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform-0.1.17-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 201618 bytes, number of entries: 7
--rw-r--r--  2.0 unx      646 b- defN 23-Jun-26 08:30 xia_engine_terraform/__init__.py
--rw-r--r--  2.0 unx   562688 b- defN 23-Jun-26 08:33 xia_engine_terraform/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 08:33 xia_engine_terraform-0.1.16.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      726 b- defN 23-Jun-26 08:33 xia_engine_terraform-0.1.16.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 08:33 xia_engine_terraform-0.1.16.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Jun-26 08:33 xia_engine_terraform-0.1.16.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      651 b- defN 23-Jun-26 08:33 xia_engine_terraform-0.1.16.dist-info/RECORD
-7 files, 564982 bytes uncompressed, 200442 bytes compressed:  64.5%
+Zip file size: 7652 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      645 b- defN 23-Jun-29 20:43 xia_engine_terraform/__init__.py
+-rw-r--r--  2.0 unx    28900 b- defN 23-Jun-29 20:43 xia_engine_terraform/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      726 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      634 b- defN 23-Jun-29 20:48 xia_engine_terraform-0.1.17.dist-info/RECORD
+7 files, 31176 bytes uncompressed, 6508 bytes compressed:  79.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform/engine.py
 Comment: 
 
-Filename: xia_engine_terraform-0.1.16.dist-info/LICENSE.txt
+Filename: xia_engine_terraform-0.1.17.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.16.dist-info/METADATA
+Filename: xia_engine_terraform-0.1.17.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform-0.1.16.dist-info/WHEEL
+Filename: xia_engine_terraform-0.1.17.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform-0.1.16.dist-info/top_level.txt
+Filename: xia_engine_terraform-0.1.17.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform-0.1.16.dist-info/RECORD
+Filename: xia_engine_terraform-0.1.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform/__init__.py

```diff
@@ -6,8 +6,8 @@
 __all__ = [
     "TerraformEngine", "TerraformConnectParam", "TerraformClient",
     "TerraformLocalEngine", "TerraformLocalConnectParam", "TerraformLocalClient",
     "ScwTerraformLocalEngine", "ScwTerraformLocalConnectParam",
     "TerraformConfigFactory"
 ]
 
-__version__ = "0.1.16"
+__version__ = "0.1.17"
```

## Comparing `xia_engine_terraform-0.1.16.dist-info/METADATA` & `xia_engine_terraform-0.1.17.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform
-Version: 0.1.16
+Version: 0.1.17
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.16/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform/0.1.17/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_engine_terraform-0.1.16.dist-info/RECORD` & `xia_engine_terraform-0.1.17.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_engine_terraform/__init__.py,sha256=fHys81Xq0hog_yiAieSIQgeZz-qG0SRA6VzH0-L6h1I,646
-xia_engine_terraform/engine.cp39-win_amd64.pyd,sha256=F8Z2lu0kQ9IF42Q66flKcEczacyrkzw5C9wdMf90WS4,562688
-xia_engine_terraform-0.1.16.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_engine_terraform-0.1.16.dist-info/METADATA,sha256=_tPTXudxeOJ5eDbJ_-4p6Vtstf3RGCItEfgLBZ_DqmE,726
-xia_engine_terraform-0.1.16.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_engine_terraform-0.1.16.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
-xia_engine_terraform-0.1.16.dist-info/RECORD,,
+xia_engine_terraform/__init__.py,sha256=lbHSuM05IgT6HWK9STpnk1tbMySmlRRZh-1DWrcweUU,645
+xia_engine_terraform/engine.py,sha256=_t4Xbj18HeoKX2369qDMO_9P_qy_PYqdeceEGLCLqo4,28900
+xia_engine_terraform-0.1.17.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_engine_terraform-0.1.17.dist-info/METADATA,sha256=80GlsVwfekxqs_QBOMpy0JAwVrmHz8BiqnqiZ04hYsc,726
+xia_engine_terraform-0.1.17.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_engine_terraform-0.1.17.dist-info/top_level.txt,sha256=9T86e-QQo91fnAOB3rD5xeM_4EPL7Edk_oOlmR_xquQ,21
+xia_engine_terraform-0.1.17.dist-info/RECORD,,
```

