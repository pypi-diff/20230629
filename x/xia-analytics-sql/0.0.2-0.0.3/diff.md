# Comparing `tmp/xia_analytics_sql-0.0.2-cp39-none-win_amd64.whl.zip` & `tmp/xia_analytics_sql-0.0.3-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 108493 bytes, number of entries: 7
--rw-r--r--  2.0 unx      106 b- defN 23-Jun-26 18:31 xia_analytics_sql/__init__.py
--rw-r--r--  2.0 unx   263680 b- defN 23-Jun-26 18:33 xia_analytics_sql/analyzer.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-26 18:33 xia_analytics_sql-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      691 b- defN 23-Jun-26 18:33 xia_analytics_sql-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Jun-26 18:33 xia_analytics_sql-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-Jun-26 18:33 xia_analytics_sql-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      627 b- defN 23-Jun-26 18:33 xia_analytics_sql-0.0.2.dist-info/RECORD
-7 files, 265372 bytes uncompressed, 107365 bytes compressed:  59.5%
+Zip file size: 2606 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      105 b- defN 23-Jun-29 20:32 xia_analytics_sql/__init__.py
+-rw-r--r--  2.0 unx     1186 b- defN 23-Jun-29 20:32 xia_analytics_sql/analyzer.py
+-rw-rw-rw-  2.0 unx      151 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      691 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      609 b- defN 23-Jun-29 20:36 xia_analytics_sql-0.0.3.dist-info/RECORD
+7 files, 2859 bytes uncompressed, 1510 bytes compressed:  47.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: xia_analytics_sql/__init__.py
 Comment: 
 
-Filename: xia_analytics_sql/analyzer.cp39-win_amd64.pyd
+Filename: xia_analytics_sql/analyzer.py
 Comment: 
 
-Filename: xia_analytics_sql-0.0.2.dist-info/LICENSE.txt
+Filename: xia_analytics_sql-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_analytics_sql-0.0.2.dist-info/METADATA
+Filename: xia_analytics_sql-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xia_analytics_sql-0.0.2.dist-info/WHEEL
+Filename: xia_analytics_sql-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xia_analytics_sql-0.0.2.dist-info/top_level.txt
+Filename: xia_analytics_sql-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_analytics_sql-0.0.2.dist-info/RECORD
+Filename: xia_analytics_sql-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_analytics_sql/__init__.py

```diff
@@ -1,7 +1,7 @@
 from xia_analytics_sql.analyzer import SqlAnalyzer
 
 __all__ = [
    "SqlAnalyzer"
 ]
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
```

## Comparing `xia_analytics_sql-0.0.2.dist-info/METADATA` & `xia_analytics_sql-0.0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: xia-analytics-sql
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-analytics-sql/0.0.2/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-analytics-sql/0.0.3/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

## Comparing `xia_analytics_sql-0.0.2.dist-info/RECORD` & `xia_analytics_sql-0.0.3.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-xia_analytics_sql/__init__.py,sha256=O25MyTSWMgxgJx3AnwHP2xK1IEBSQgp00s26-tFvWvE,106
-xia_analytics_sql/analyzer.cp39-win_amd64.pyd,sha256=XW1JGlKqRd7T_8yD6P18IkHQtX3n9YliWL12Criw4ak,263680
-xia_analytics_sql-0.0.2.dist-info/LICENSE.txt,sha256=FU8wWPH4eLlGEUQT4o0vgpnW66Olgbnc_Oe1tvF5lek,151
-xia_analytics_sql-0.0.2.dist-info/METADATA,sha256=j4qFvFs8e0ssm79GDP2LqsLULGv6Dzf19QmkVLM8iOk,691
-xia_analytics_sql-0.0.2.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
-xia_analytics_sql-0.0.2.dist-info/top_level.txt,sha256=mrVMNrm-BLTdC4PUEQWdzBiSd47TAqlb99m7t0MdLok,18
-xia_analytics_sql-0.0.2.dist-info/RECORD,,
+xia_analytics_sql/__init__.py,sha256=5cDXOmPpQYudRBFwFsfEyL0rARKbwPjgNkZPUNV-Jeg,105
+xia_analytics_sql/analyzer.py,sha256=s4PHmL_pTleAht4y_9X2mFMqB8MW10iBeMs4oB5F_jc,1186
+xia_analytics_sql-0.0.3.dist-info/LICENSE.txt,sha256=8eGGd5uTzfYM5wAFddxevOMkV57kCpaehAvbSNQebDE,151
+xia_analytics_sql-0.0.3.dist-info/METADATA,sha256=28Wt8A7J0ArnSkgUfakJTDTgI-Wb25Ni10wl6T4aO9Q,691
+xia_analytics_sql-0.0.3.dist-info/WHEEL,sha256=rotlO1fPkO19RolFJ8zxn0hURh38g88DeuJ659l3xAc,99
+xia_analytics_sql-0.0.3.dist-info/top_level.txt,sha256=mrVMNrm-BLTdC4PUEQWdzBiSd47TAqlb99m7t0MdLok,18
+xia_analytics_sql-0.0.3.dist-info/RECORD,,
```

