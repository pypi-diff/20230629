# Comparing `tmp/SilverStreamingApplication-1.1.tar.gz` & `tmp/SilverStreamingApplication-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SilverStreamingApplication-1.1.tar", last modified: Tue Jun  6 06:12:42 2023, max compression
+gzip compressed data, was "SilverStreamingApplication-1.2.tar", last modified: Thu Jun 29 13:44:38 2023, max compression
```

## Comparing `SilverStreamingApplication-1.1.tar` & `SilverStreamingApplication-1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/
--rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-06 06:12:42.000000 SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/com/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.052880 SilverStreamingApplication-1.1/com/phida/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/com/phida/main/
--rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/Maintenance.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12292 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/Operations.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16891 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/PartitionAnalyzer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3967 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/PerfAnalyzer.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11680 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/SilverMerge.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14662 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/WorkflowBuilder.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1374 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/logging.py
--rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/sparksession.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1831 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/main/utilsDatabricksAPI.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/com/phida/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)     5765 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/OperationsTest.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/main_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/com/phida/tests/utils_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-06 06:12:42.056880 SilverStreamingApplication-1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      247 2023-06-06 06:12:35.000000 SilverStreamingApplication-1.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      181 2023-06-29 13:44:38.000000 SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      702 2023-06-29 13:44:38.000000 SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-29 13:44:38.000000 SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-29 13:44:38.000000 SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/com/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/com/phida/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/com/phida/main/
+-rw-r--r--   0 vsts      (1001) docker     (123)      759 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/Maintenance.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12292 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/Operations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16891 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/PartitionAnalyzer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3967 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/PerfAnalyzer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11801 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/SilverMerge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14662 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/WorkflowBuilder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1374 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      160 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/sparksession.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1831 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1247 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/main/utilsDatabricksAPI.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/com/phida/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5765 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/tests/OperationsTest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/tests/main_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/com/phida/tests/utils_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-06-29 13:44:38.159734 SilverStreamingApplication-1.2/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)      247 2023-06-29 13:44:30.000000 SilverStreamingApplication-1.2/setup.py
```

### Comparing `SilverStreamingApplication-1.1/SilverStreamingApplication.egg-info/SOURCES.txt` & `SilverStreamingApplication-1.2/SilverStreamingApplication.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/Maintenance.py` & `SilverStreamingApplication-1.2/com/phida/main/Maintenance.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/Operations.py` & `SilverStreamingApplication-1.2/com/phida/main/Operations.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/PartitionAnalyzer.py` & `SilverStreamingApplication-1.2/com/phida/main/PartitionAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/PerfAnalyzer.py` & `SilverStreamingApplication-1.2/com/phida/main/PerfAnalyzer.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/SilverMerge.py` & `SilverStreamingApplication-1.2/com/phida/main/SilverMerge.py`

 * *Files 2% similar despite different names*

```diff
@@ -217,28 +217,31 @@
 
         example:
             N/A - see method streamIntoDeltaTarget() for usage
 
         tip:
             N/A
         """
+         
+        microBatchOutputDF = microBatchOutputDF.filter("source_operation in (0,1,2,3)")
+
         windowSpec = Window.partitionBy(self.keyColsList).orderBy(col("src_commit_time").desc(),
                                                                   col("hvr_integ_key").desc())
 
         microBatchOutputDF = microBatchOutputDF.withColumn("latest_record", row_number().over(windowSpec)).filter(
             "latest_record == 1").drop("latest_record")
 
         tgtDeltaTable = DeltaTable.forName(spark, self.tgtDatabaseName + "." + self.tgtTableName)
 
         tgtDeltaTable.alias("t").merge(microBatchOutputDF.alias("s"), self.condition) \
-            .whenMatchedDelete("s.source_operation = 0") \
-            .whenMatchedUpdate(condition="s.source_operation != 0", set=self.columnsDict) \
-            .whenNotMatchedInsert(condition="s.source_operation != 0", values=self.columnsDict) \
+            .whenMatchedDelete("s.source_operation in (0,3)") \
+            .whenMatchedUpdate(condition="s.source_operation not in (0,3)", set=self.columnsDict) \
+            .whenNotMatchedInsert(condition="s.source_operation not in (0,3)", values=self.columnsDict) \
             .execute()
-
+ 
     def streamIntoDeltaTarget(self):
         """
         desc:
             A Function for writing the given streaming dataframe into Delta Target table with foreachBatch merge
             Main layer the triggers/kicks off the entire process of reading from Bronze and merging into silver.
         args:
             None
```

### Comparing `SilverStreamingApplication-1.1/com/phida/main/WorkflowBuilder.py` & `SilverStreamingApplication-1.2/com/phida/main/WorkflowBuilder.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/logging.py` & `SilverStreamingApplication-1.2/com/phida/main/logging.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/utils.py` & `SilverStreamingApplication-1.2/com/phida/main/utils.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/main/utilsDatabricksAPI.py` & `SilverStreamingApplication-1.2/com/phida/main/utilsDatabricksAPI.py`

 * *Files identical despite different names*

### Comparing `SilverStreamingApplication-1.1/com/phida/tests/OperationsTest.py` & `SilverStreamingApplication-1.2/com/phida/tests/OperationsTest.py`

 * *Files identical despite different names*

