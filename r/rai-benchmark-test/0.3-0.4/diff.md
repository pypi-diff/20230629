# Comparing `tmp/rai_benchmark_test-0.3.tar.gz` & `tmp/rai_benchmark_test-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\rai_benchmark_test-0.3.tar", last modified: Thu Jun 29 18:12:26 2023, max compression
+gzip compressed data, was "dist\rai_benchmark_test-0.4.tar", last modified: Thu Jun 29 18:16:40 2023, max compression
```

## Comparing `rai_benchmark_test-0.3.tar` & `rai_benchmark_test-0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 18:12:26.785543 rai_benchmark_test-0.3/
--rw-rw-rw-   0        0        0       63 2023-06-29 18:12:26.773526 rai_benchmark_test-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 18:12:26.738272 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/
--rw-rw-rw-   0        0        0       63 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       55 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-29 18:12:26.000000 rai_benchmark_test-0.3/rai_benchmark_test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-29 18:12:26.785543 rai_benchmark_test-0.3/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-06-29 17:30:55.000000 rai_benchmark_test-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-29 18:12:26.773526 rai_benchmark_test-0.3/src/
--rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.3/src/__init__.py
--rw-rw-rw-   0        0        0      891 2023-06-29 16:18:37.000000 rai_benchmark_test-0.3/src/aml_auth.py
--rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.3/src/aml_fetch_data.py
--rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.3/src/assessment_flow.py
--rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.3/src/constants.py
--rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.3/src/data_prep.py
--rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.3/src/e2e_exp.py
--rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.3/src/evaluation.py
--rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.3/src/job.py
--rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.3/src/job_manager.py
--rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.3/src/prompt_builder.py
--rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.3/src/prompt_data.py
--rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.3/src/request.py
--rw-rw-rw-   0        0        0     1420 2023-06-29 16:01:28.000000 rai_benchmark_test-0.3/src/run.py
--rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.3/src/tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:16:40.885042 rai_benchmark_test-0.4/
+-rw-rw-rw-   0        0        0       63 2023-06-29 18:16:40.885042 rai_benchmark_test-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-29 18:16:40.845070 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/
+-rw-rw-rw-   0        0        0       63 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-29 18:16:40.000000 rai_benchmark_test-0.4/rai_benchmark_test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-29 18:16:40.885042 rai_benchmark_test-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      379 2023-06-29 18:16:35.000000 rai_benchmark_test-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-29 18:16:40.885042 rai_benchmark_test-0.4/src/
+-rw-rw-rw-   0        0        0        0 2023-06-29 17:25:37.000000 rai_benchmark_test-0.4/src/__init__.py
+-rw-rw-rw-   0        0        0      891 2023-06-29 16:18:37.000000 rai_benchmark_test-0.4/src/aml_auth.py
+-rw-rw-rw-   0        0        0      537 2023-06-27 17:41:58.000000 rai_benchmark_test-0.4/src/aml_fetch_data.py
+-rw-rw-rw-   0        0        0     2749 2023-06-29 16:26:57.000000 rai_benchmark_test-0.4/src/assessment_flow.py
+-rw-rw-rw-   0        0        0       96 2023-06-22 00:15:34.000000 rai_benchmark_test-0.4/src/constants.py
+-rw-rw-rw-   0        0        0     2651 2023-06-26 19:04:32.000000 rai_benchmark_test-0.4/src/data_prep.py
+-rw-rw-rw-   0        0        0     4059 2023-06-29 16:33:55.000000 rai_benchmark_test-0.4/src/e2e_exp.py
+-rw-rw-rw-   0        0        0     1916 2023-06-27 17:14:37.000000 rai_benchmark_test-0.4/src/evaluation.py
+-rw-rw-rw-   0        0        0     1512 2023-06-22 00:03:28.000000 rai_benchmark_test-0.4/src/job.py
+-rw-rw-rw-   0        0        0     7806 2023-06-26 21:31:22.000000 rai_benchmark_test-0.4/src/job_manager.py
+-rw-rw-rw-   0        0        0     7076 2023-06-27 00:10:20.000000 rai_benchmark_test-0.4/src/prompt_builder.py
+-rw-rw-rw-   0        0        0      424 2023-06-21 23:17:39.000000 rai_benchmark_test-0.4/src/prompt_data.py
+-rw-rw-rw-   0        0        0     4938 2023-06-22 00:16:24.000000 rai_benchmark_test-0.4/src/request.py
+-rw-rw-rw-   0        0        0     1420 2023-06-29 16:01:28.000000 rai_benchmark_test-0.4/src/run.py
+-rw-rw-rw-   0        0        0      493 2023-06-22 00:16:34.000000 rai_benchmark_test-0.4/src/tokenizer.py
```

### Comparing `rai_benchmark_test-0.3/rai_benchmark_test.egg-info/SOURCES.txt` & `rai_benchmark_test-0.4/rai_benchmark_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/aml_auth.py` & `rai_benchmark_test-0.4/src/aml_auth.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/aml_fetch_data.py` & `rai_benchmark_test-0.4/src/aml_fetch_data.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/assessment_flow.py` & `rai_benchmark_test-0.4/src/assessment_flow.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/data_prep.py` & `rai_benchmark_test-0.4/src/data_prep.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/e2e_exp.py` & `rai_benchmark_test-0.4/src/e2e_exp.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/evaluation.py` & `rai_benchmark_test-0.4/src/evaluation.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/job.py` & `rai_benchmark_test-0.4/src/job.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/job_manager.py` & `rai_benchmark_test-0.4/src/job_manager.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/prompt_builder.py` & `rai_benchmark_test-0.4/src/prompt_builder.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/request.py` & `rai_benchmark_test-0.4/src/request.py`

 * *Files identical despite different names*

### Comparing `rai_benchmark_test-0.3/src/run.py` & `rai_benchmark_test-0.4/src/run.py`

 * *Files identical despite different names*

