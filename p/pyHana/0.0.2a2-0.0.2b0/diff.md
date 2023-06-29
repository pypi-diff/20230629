# Comparing `tmp/pyHana-0.0.2a2-py3-none-any.whl.zip` & `tmp/pyHana-0.0.2b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 35082 bytes, number of entries: 30
+Zip file size: 35101 bytes, number of entries: 30
 -rw-rw-rw-  2.0 fat       85 b- defN 23-Jun-25 16:00 pyHana/__init__.py
 -rw-rw-rw-  2.0 fat       28 b- defN 23-Jun-04 13:58 pyHana/analysis/__init__.py
 -rw-rw-rw-  2.0 fat    16752 b- defN 23-Jun-28 14:17 pyHana/analysis/stockEcoIndex.py
 -rw-rw-rw-  2.0 fat       48 b- defN 23-Jun-09 22:21 pyHana/common/__init__.py
 -rw-rw-rw-  2.0 fat     2827 b- defN 23-Jun-29 12:26 pyHana/common/code.py
 -rw-rw-rw-  2.0 fat      624 b- defN 23-Jun-24 14:46 pyHana/common/conf.py
 -rw-rw-rw-  2.0 fat     1535 b- defN 23-Jun-26 14:01 pyHana/common/dataProc.py
@@ -21,12 +21,12 @@
 -rw-rw-rw-  2.0 fat     5646 b- defN 23-Jun-29 03:45 pyHana/innerIO/stockInfo.py
 -rw-rw-rw-  2.0 fat       72 b- defN 23-Jun-24 12:59 pyHana/outerIO/__init__.py
 -rw-rw-rw-  2.0 fat     5465 b- defN 23-Jun-25 05:55 pyHana/outerIO/dart.py
 -rw-rw-rw-  2.0 fat    15300 b- defN 23-Jun-28 14:01 pyHana/outerIO/ebest.py
 -rw-rw-rw-  2.0 fat     1840 b- defN 23-Jun-18 12:21 pyHana/outerIO/ecoIndex.py
 -rw-rw-rw-  2.0 fat     6535 b- defN 23-Jun-25 04:27 pyHana/outerIO/kind.py
 -rw-rw-rw-  2.0 fat     1800 b- defN 23-Jun-24 12:01 pyHana/outerIO/marketIndex.py
--rw-rw-rw-  2.0 fat      659 b- defN 23-Jun-29 14:49 pyHana-0.0.2a2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 14:49 pyHana-0.0.2a2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-29 14:49 pyHana-0.0.2a2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     2440 b- defN 23-Jun-29 14:49 pyHana-0.0.2a2.dist-info/RECORD
-30 files, 98898 bytes uncompressed, 31176 bytes compressed:  68.5%
+-rw-rw-rw-  2.0 fat      704 b- defN 23-Jun-29 14:19 pyHana-0.0.2b0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 14:19 pyHana-0.0.2b0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-29 14:19 pyHana-0.0.2b0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2440 b- defN 23-Jun-29 14:19 pyHana-0.0.2b0.dist-info/RECORD
+30 files, 98943 bytes uncompressed, 31195 bytes compressed:  68.5%
```

## zipnote {}

```diff
@@ -72,20 +72,20 @@
 
 Filename: pyHana/outerIO/kind.py
 Comment: 
 
 Filename: pyHana/outerIO/marketIndex.py
 Comment: 
 
-Filename: pyHana-0.0.2a2.dist-info/METADATA
+Filename: pyHana-0.0.2b0.dist-info/METADATA
 Comment: 
 
-Filename: pyHana-0.0.2a2.dist-info/WHEEL
+Filename: pyHana-0.0.2b0.dist-info/WHEEL
 Comment: 
 
-Filename: pyHana-0.0.2a2.dist-info/top_level.txt
+Filename: pyHana-0.0.2b0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyHana-0.0.2a2.dist-info/RECORD
+Filename: pyHana-0.0.2b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyHana-0.0.2a2.dist-info/RECORD` & `pyHana-0.0.2b0.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 pyHana/innerIO/stockInfo.py,sha256=XZOVfNjd6GwbYuxgLx4oUj5pyABOm9kOYjsvse3GFfg,5646
 pyHana/outerIO/__init__.py,sha256=4ov-xPtJCVADhp1TQ39PBaHJ_Md213hsMzRnGG5qWmE,72
 pyHana/outerIO/dart.py,sha256=MaIz73wzOp8oVSI-OQPKVSOuVBV0advwB6ZJDrbBE8w,5465
 pyHana/outerIO/ebest.py,sha256=RfxR_BwK7RBuHgIsc7_tp_Vi2eLd3OIXh-DpWdUCGEA,15300
 pyHana/outerIO/ecoIndex.py,sha256=Lbu9VrbWYy2Yo57iisfTi6dJlHUkbH1tDcBGeE5xC-c,1840
 pyHana/outerIO/kind.py,sha256=ZunqvWQpG0s1nTv8QpdoXm1GKyh5VekIoVZVMcJUXsc,6535
 pyHana/outerIO/marketIndex.py,sha256=i6AUpzo8kuSM1TDogLV5uqv877DEVa00PtT6uCHUlaY,1800
-pyHana-0.0.2a2.dist-info/METADATA,sha256=AMqdcP0rIeJZxUkfvx_8VzTo-dKzdlG9byu5m608Pdw,659
-pyHana-0.0.2a2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyHana-0.0.2a2.dist-info/top_level.txt,sha256=HB0jmziPuwk5hJlWnvEbaS8QkKv84NPwX8F6le7Tm1Y,7
-pyHana-0.0.2a2.dist-info/RECORD,,
+pyHana-0.0.2b0.dist-info/METADATA,sha256=gvIL5KulmYYvEPvtTqlB78wCAt_SgSvBje3kcYHR2ZU,704
+pyHana-0.0.2b0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyHana-0.0.2b0.dist-info/top_level.txt,sha256=HB0jmziPuwk5hJlWnvEbaS8QkKv84NPwX8F6le7Tm1Y,7
+pyHana-0.0.2b0.dist-info/RECORD,,
```

