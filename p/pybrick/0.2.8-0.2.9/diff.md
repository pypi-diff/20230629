# Comparing `tmp/pybrick-0.2.8-py3-none-any.whl.zip` & `tmp/pybrick-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6368 bytes, number of entries: 7
+Zip file size: 6423 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jun-30 13:40 pybrick/__init__.py
--rw-rw-rw-  2.0 fat       25 b- defN 23-Jun-28 15:42 pybrick/ptest.csv
+-rw-rw-rw-  2.0 fat       88 b- defN 23-Jun-29 01:19 pybrick/ptest.csv
 -rw-rw-rw-  2.0 fat    14953 b- defN 23-Jun-29 01:27 pybrick/pybrick.py
--rw-rw-rw-  2.0 fat      321 b- defN 23-Jun-29 01:30 pybrick-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 01:30 pybrick-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-29 01:30 pybrick-0.2.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      517 b- defN 23-Jun-29 01:30 pybrick-0.2.8.dist-info/RECORD
-7 files, 15916 bytes uncompressed, 5450 bytes compressed:  65.8%
+-rw-rw-rw-  2.0 fat      321 b- defN 23-Jun-29 01:34 pybrick-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 01:34 pybrick-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-29 01:34 pybrick-0.2.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      517 b- defN 23-Jun-29 01:34 pybrick-0.2.9.dist-info/RECORD
+7 files, 15979 bytes uncompressed, 5505 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pybrick/ptest.csv
 Comment: 
 
 Filename: pybrick/pybrick.py
 Comment: 
 
-Filename: pybrick-0.2.8.dist-info/METADATA
+Filename: pybrick-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: pybrick-0.2.8.dist-info/WHEEL
+Filename: pybrick-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: pybrick-0.2.8.dist-info/top_level.txt
+Filename: pybrick-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pybrick-0.2.8.dist-info/RECORD
+Filename: pybrick-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pybrick/ptest.csv

```diff
@@ -1,3 +1,8 @@
 A,B
-1,adsf
-3.14159,aelh
+1.0,one point zero
+2,two
+3.14159,pi
+4,four
+5,five
+6,six
+7.8,seven point eight
```

