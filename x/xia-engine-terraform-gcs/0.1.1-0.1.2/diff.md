# Comparing `tmp/xia_engine_terraform_gcs-0.1.1-cp39-none-win_amd64.whl.zip` & `tmp/xia_engine_terraform_gcs-0.1.2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 127104 bytes, number of entries: 7
--rw-r--r--  2.0 unx      378 b- defN 23-Jun-26 13:18 xia_engine_terraform_gcs/__init__.py
--rw-r--r--  2.0 unx   313856 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs-0.1.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      762 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs-0.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs-0.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      674 b- defN 23-Jun-26 13:20 xia_engine_terraform_gcs-0.1.1.dist-info/RECORD
-7 files, 315945 bytes uncompressed, 125882 bytes compressed:  60.2%
+Zip file size: 3601 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      377 b- defN 23-Jun-29 20:44 xia_engine_terraform_gcs/__init__.py
+-rw-r--r--  2.0 unx     4325 b- defN 23-Jun-29 14:52 xia_engine_terraform_gcs/engine.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:49 xia_engine_terraform_gcs-0.1.2.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      762 b- defN 23-Jun-29 20:49 xia_engine_terraform_gcs-0.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:49 xia_engine_terraform_gcs-0.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-Jun-29 20:49 xia_engine_terraform_gcs-0.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jun-29 20:49 xia_engine_terraform_gcs-0.1.2.dist-info/RECORD
+7 files, 6395 bytes uncompressed, 2411 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_engine_terraform_gcs/__init__.py
 Comment: 
 
-Filename: xia_engine_terraform_gcs/engine.cp39-win_amd64.pyd
+Filename: xia_engine_terraform_gcs/engine.py
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.1.dist-info/LICENSE.txt
+Filename: xia_engine_terraform_gcs-0.1.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.1.dist-info/METADATA
+Filename: xia_engine_terraform_gcs-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.1.dist-info/WHEEL
+Filename: xia_engine_terraform_gcs-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.1.dist-info/top_level.txt
+Filename: xia_engine_terraform_gcs-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_engine_terraform_gcs-0.1.1.dist-info/RECORD
+Filename: xia_engine_terraform_gcs-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_engine_terraform_gcs/__init__.py

```diff
@@ -3,8 +3,8 @@
 
 
 __all__ = [
     "TerraformGcsEngine", "TerraformGcsConnectParam", "TerraformGcsClient",
     "ScwTerraformGcsEngine", "ScwTerraformGcsConnectParam"
 ]
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## Comparing `xia_engine_terraform_gcs-0.1.1.dist-info/METADATA` & `xia_engine_terraform_gcs-0.1.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-engine-terraform-gcs
-Version: 0.1.1
+Version: 0.1.2
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.1.1/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-engine-terraform-gcs/0.1.2/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

