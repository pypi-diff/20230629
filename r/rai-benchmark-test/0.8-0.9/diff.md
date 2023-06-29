# Comparing `tmp/rai_benchmark_test-0.8.tar.gz` & `tmp/rai_benchmark_test-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-0.8.tar", last modified: Thu Jun 29 20:22:30 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-0.9.tar", last modified: Thu Jun 29 20:45:14 2023, max compression
```

## Comparing `rai_benchmark_test-0.8.tar` & `rai_benchmark_test-0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 20:22:30.381959 rai_benchmark_test-0.8/
--rw-rw-rw-   0        0        0       63 2023-06-29 20:22:30.381959 rai_benchmark_test-0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 20:22:30.356555 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 20:22:30.000000 rai_benchmark_test-0.8/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 20:22:30.381959 rai_benchmark_test-0.8/setup.cfg
--rw-rw-rw-   0        0        0      385 2023-06-29 20:22:23.000000 rai_benchmark_test-0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 20:22:30.381959 rai_benchmark_test-0.8/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.8/src/__init__.py
--rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-0.8/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.8/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.8/src/assessment_flow.py
--rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.8/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.8/src/data_prep.py
--rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.8/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.8/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.8/src/job.py
--rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.8/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.8/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.8/src/prompt_data.py
--rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.8/src/request.py
--rw-rw-rw-   0        0        0     1571 2023-06-29 20:21:52.000000 rai_benchmark_test-0.8/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.8/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.586038 rai_benchmark_test-0.9/
+-rw-rw-rw-   0        0        0       63 2023-06-29 20:45:14.586038 rai_benchmark_test-0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.471437 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 20:45:14.000000 rai_benchmark_test-0.9/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 20:45:14.587037 rai_benchmark_test-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      385 2023-06-29 20:44:51.000000 rai_benchmark_test-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 20:45:14.583902 rai_benchmark_test-0.9/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.9/src/__init__.py
+-rw-rw-rw-   0        0        0      849 2023-06-29 20:12:05.000000 rai_benchmark_test-0.9/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.9/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.9/src/assessment_flow.py
+-rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.9/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.9/src/data_prep.py
+-rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.9/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.9/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.9/src/job.py
+-rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.9/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.9/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.9/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.9/src/request.py
+-rw-rw-rw-   0        0        0     1588 2023-06-29 20:44:33.000000 rai_benchmark_test-0.9/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.9/src/tokenizer.py
```

### Comparing `rai_benchmark_test-0.8/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-0.9/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/aml_auth.py` & `rai_benchmark_test-0.9/src/aml_auth.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/aml_fetch_data.py` & `rai_benchmark_test-0.9/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/assessment_flow.py` & `rai_benchmark_test-0.9/src/assessment_flow.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/data_prep.py` & `rai_benchmark_test-0.9/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/e2e_exp.py` & `rai_benchmark_test-0.9/src/e2e_exp.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/evaluation.py` & `rai_benchmark_test-0.9/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/job.py` & `rai_benchmark_test-0.9/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/job_manager.py` & `rai_benchmark_test-0.9/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/prompt_builder.py` & `rai_benchmark_test-0.9/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/request.py` & `rai_benchmark_test-0.9/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.8/src/run.py` & `rai_benchmark_test-0.9/src/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
       "--experiment_name",
       experiment_name,
       "--prompt_file",
       prompt_file,
       "--model_name",
       model_name
     ]
-    src = ScriptRunConfig(source_directory=path.dirname(__file__),
-                        script='e2e_exp.py',
+    src = ScriptRunConfig(source_directory="./",
+                        script=path.join(path.dirname(__file__), 'e2e_exp.py'),
                         compute_target='local',
                         environment=myenv,
                         arguments=script_params
                         )
 
     ws = get_aml_workspace()
     experiment = Experiment(workspace=ws, name=experiment_name)
```

