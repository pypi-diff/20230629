# Comparing `tmp/rai_benchmark_test-0.6.tar.gz` & `tmp/rai_benchmark_test-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-0.6.tar", last modified: Thu Jun 29 18:53:33 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-0.7.tar", last modified: Thu Jun 29 20:13:37 2023, max compression
```

## Comparing `rai_benchmark_test-0.6.tar` & `rai_benchmark_test-0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:53:33.809881 rai_benchmark_test-0.6/
--rw-rw-rw-   0        0        0       63 2023-06-29 18:53:33.809881 rai_benchmark_test-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 18:53:33.778636 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 18:53:33.000000 rai_benchmark_test-0.6/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 18:53:33.809881 rai_benchmark_test-0.6/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-29 18:53:01.000000 rai_benchmark_test-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:53:33.809881 rai_benchmark_test-0.6/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.6/src/__init__.py
--rw-rw-rw-   0        0        0      878 2023-06-29 18:27:50.000000 rai_benchmark_test-0.6/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.6/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.6/src/assessment_flow.py
--rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.6/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.6/src/data_prep.py
--rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.6/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.6/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.6/src/job.py
--rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.6/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.6/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.6/src/prompt_data.py
--rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.6/src/request.py
--rw-rw-rw-   0        0        0     1532 2023-06-29 18:52:56.000000 rai_benchmark_test-0.6/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.6/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:13:37.360386 rai_benchmark_test-0.7/
+-rw-rw-rw-   0        0        0       63 2023-06-29 20:13:37.360386 rai_benchmark_test-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 20:13:37.329740 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 20:13:37.000000 rai_benchmark_test-0.7/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:13:37.360386 rai_benchmark_test-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-29 20:13:32.000000 rai_benchmark_test-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:13:37.360386 rai_benchmark_test-0.7/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.7/src/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-0.7/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.7/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.7/src/assessment_flow.py
+-rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.7/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.7/src/data_prep.py
+-rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.7/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.7/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.7/src/job.py
+-rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.7/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.7/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.7/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.7/src/request.py
+-rw-rw-rw-   0        0        0     1532 2023-06-29 18:52:56.000000 rai_benchmark_test-0.7/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.7/src/tokenizer.py
```

### Comparing `rai_benchmark_test-0.6/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-0.7/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/aml_auth.py` & `rai_benchmark_test-0.7/src/aml_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     return ml_client
 
 
 def get_aml_workspace():
     ws = Workspace(
         subscription_id="e0fd569c-e34a-4249-8c24-e8d723c7f054",
         resource_group="benchmark",
-        workspace_name="ziqitest",
-        auth=DefaultAzureCredential() #get_service_pr_auth()
+        workspace_name="ziqitest"#,
+        #get_service_pr_auth()
     )
     return ws
 
 
 def start_mlflow_experiment(exp_name):
     ws = get_aml_workspace()
     mlflow.set_tracking_uri(ws.get_mlflow_tracking_uri())
```

### Comparing `rai_benchmark_test-0.6/src/aml_fetch_data.py` & `rai_benchmark_test-0.7/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/assessment_flow.py` & `rai_benchmark_test-0.7/src/assessment_flow.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/data_prep.py` & `rai_benchmark_test-0.7/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/e2e_exp.py` & `rai_benchmark_test-0.7/src/e2e_exp.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/evaluation.py` & `rai_benchmark_test-0.7/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/job.py` & `rai_benchmark_test-0.7/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/job_manager.py` & `rai_benchmark_test-0.7/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/prompt_builder.py` & `rai_benchmark_test-0.7/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/request.py` & `rai_benchmark_test-0.7/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.6/src/run.py` & `rai_benchmark_test-0.7/src/run.py`

 * *Files identical despite different names*

