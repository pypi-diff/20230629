# Comparing `tmp/neulab-0.0.30-py3-none-any.whl.zip` & `tmp/neulab-0.0.31-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9526 bytes, number of entries: 11
+Zip file size: 9564 bytes, number of entries: 11
 -rw-r--r--  2.0 unx        0 b- defN 22-Apr-28 12:23 neulab/__init__.py
 -rw-r--r--  2.0 unx    10293 b- defN 23-Feb-22 15:09 neulab/clusters.py
 -rw-r--r--  2.0 unx     3712 b- defN 23-Feb-21 20:54 neulab/discover.py
 -rw-r--r--  2.0 unx     1123 b- defN 23-Feb-21 23:24 neulab/normalization.py
 -rw-r--r--  2.0 unx     5893 b- defN 23-Feb-22 01:09 neulab/outliers.py
 -rw-r--r--  2.0 unx     8076 b- defN 23-Feb-21 21:05 neulab/recover.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/LICENSE
--rw-r--r--  2.0 unx      786 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      836 b- defN 23-Feb-22 18:00 neulab-0.0.30.dist-info/RECORD
-11 files, 31890 bytes uncompressed, 8126 bytes compressed:  74.5%
+-rw-r--r--  2.0 unx     1072 b- defN 23-Jun-29 00:41 neulab-0.0.31.dist-info/LICENSE
+-rw-r--r--  2.0 unx      878 b- defN 23-Jun-29 00:41 neulab-0.0.31.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 00:41 neulab-0.0.31.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Jun-29 00:41 neulab-0.0.31.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      836 b- defN 23-Jun-29 00:41 neulab-0.0.31.dist-info/RECORD
+11 files, 31982 bytes uncompressed, 8164 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: neulab/outliers.py
 Comment: 
 
 Filename: neulab/recover.py
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/LICENSE
+Filename: neulab-0.0.31.dist-info/LICENSE
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/METADATA
+Filename: neulab-0.0.31.dist-info/METADATA
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/WHEEL
+Filename: neulab-0.0.31.dist-info/WHEEL
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/top_level.txt
+Filename: neulab-0.0.31.dist-info/top_level.txt
 Comment: 
 
-Filename: neulab-0.0.30.dist-info/RECORD
+Filename: neulab-0.0.31.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `neulab-0.0.30.dist-info/LICENSE` & `neulab-0.0.31.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `neulab-0.0.30.dist-info/METADATA` & `neulab-0.0.31.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: neulab
-Version: 0.0.30
+Version: 0.0.31
 Summary: Tool for data preprocess in ML.
 Home-page: https://github.com/kndahl/neulab
 Author: Roman Fitzjalen
 Author-email: romaactor@gmail.com
 License: MIT
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: scipy
 Requires-Dist: networkx
 Requires-Dist: matplotlib
+Requires-Dist: jinja2
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
 
 # neulab
 Tool for data preprocess in ML.
 
 [![Downloads](https://pepy.tech/badge/neulab)](https://pepy.tech/project/neulab)
 # Installation
 ```
 pip install neulab
 ```
 # Description
 The library contains several blocks: data analysis, data recovery methods, data normalization, outlier detection, clustering. A detailed description and instructions can be found on Github: https://github.com/kndahl/neulab
+
```

## Comparing `neulab-0.0.30.dist-info/RECORD` & `neulab-0.0.31.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 neulab/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 neulab/clusters.py,sha256=HiGD0nBSVY0m0BvGlv8Nij4Y-DzB7AmKFfmr5k8ECoU,10293
 neulab/discover.py,sha256=MqTuzm9jCLXodssP3e1Q7OP-srhI2KhBzdtRds-882E,3712
 neulab/normalization.py,sha256=Fuk4CaocSZQKbdCKxeIb4Cl7UU7thE9YQG-SGh1-PBs,1123
 neulab/outliers.py,sha256=VFo4WSp7bI4Rk2ILuq_x4dLyNcPSqwO7pLtAweGsU8U,5893
 neulab/recover.py,sha256=GmwEixJ57aNi7aE9m8wJ27PnYpD6nbsD970Q2Jr0ups,8076
-neulab-0.0.30.dist-info/LICENSE,sha256=O8fgY-KCD2vIUoSpKXwlNSnqy_XJRKWVxWUfJzi6M0k,1072
-neulab-0.0.30.dist-info/METADATA,sha256=gR0-3di3Mcr8X5xGGYsJDIfb08vG3ipUHuoSVZQRVZs,786
-neulab-0.0.30.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-neulab-0.0.30.dist-info/top_level.txt,sha256=WoV2_jqLKem7Qa9WbZrt45w8snBf5lekIsmrQo94FvY,7
-neulab-0.0.30.dist-info/RECORD,,
+neulab-0.0.31.dist-info/LICENSE,sha256=O8fgY-KCD2vIUoSpKXwlNSnqy_XJRKWVxWUfJzi6M0k,1072
+neulab-0.0.31.dist-info/METADATA,sha256=yL_4N2CiXX0hRitVBPg93peqS5tHvrFnyHnPZw7adqc,878
+neulab-0.0.31.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+neulab-0.0.31.dist-info/top_level.txt,sha256=WoV2_jqLKem7Qa9WbZrt45w8snBf5lekIsmrQo94FvY,7
+neulab-0.0.31.dist-info/RECORD,,
```

