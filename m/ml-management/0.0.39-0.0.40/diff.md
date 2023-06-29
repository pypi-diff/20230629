# Comparing `tmp/ml-management-0.0.39.tar.gz` & `tmp/ml-management-0.0.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ml-management-0.0.39.tar", last modified: Mon Jun 26 13:30:57 2023, max compression
+gzip compressed data, was "ml-management-0.0.40.tar", last modified: Thu Jun 29 11:20:50 2023, max compression
```

## Comparing `ml-management-0.0.39.tar` & `ml-management-0.0.40.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.366889 ml-management-0.0.39/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       18 2022-11-15 15:35:02.000000 ml-management-0.0.39/MANIFEST.in
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      120 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1092 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      456 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1318 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/collectors.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/dummy/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      463 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.358888 ml-management-0.0.39/ML_management/collectors/s3/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    10609 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/collectors/topic_markers/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)   331440 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3167 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/dataset_loader_template/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2407 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/executor_template/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/executor_template/default_executors/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      895 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      843 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      869 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     4566 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      402 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      334 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/mlmanagement/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      581 2022-09-29 11:08:30.000000 ml-management-0.0.39/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3392 2023-03-13 16:12:20.000000 ml-management-0.0.39/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     5054 2023-03-13 16:12:20.000000 ml-management-0.0.39/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    13677 2023-06-23 15:20:18.000000 ml-management-0.0.39/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)    10260 2023-06-23 15:20:18.000000 ml-management-0.0.39/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      201 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     5001 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      316 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/models/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/models/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      949 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/models/patterns/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     4202 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      561 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      445 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      457 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/registry/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-08-01 13:04:47.000000 ml-management-0.0.39/ML_management/registry/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2566 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/registry/exceptions.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     7556 2023-05-15 09:28:39.000000 ml-management-0.0.39/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/tests/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2022-12-07 10:58:45.000000 ml-management-0.0.39/ML_management/tests/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     3361 2022-12-07 10:58:45.000000 ml-management-0.0.39/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     9275 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.362888 ml-management-0.0.39/ML_management/uploader_data/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        0 2023-05-31 08:55:31.000000 ml-management-0.0.39/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1694 2023-06-15 09:26:35.000000 ml-management-0.0.39/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-26 13:30:57.366889 ml-management-0.0.39/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       56 2022-08-01 13:04:47.000000 ml-management-0.0.39/README.md
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        7 2023-06-26 13:30:41.000000 ml-management-0.0.39/VERSION
-drwxrwxr-x   0 boeing    (1000) boeing    (1000)        0 2023-06-26 13:30:57.366889 ml-management-0.0.39/ml_management.egg-info/
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      312 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     2449 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)        1 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)      153 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/requires.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       14 2023-06-26 13:30:57.000000 ml-management-0.0.39/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 boeing    (1000) boeing    (1000)       38 2023-06-26 13:30:57.366889 ml-management-0.0.39/setup.cfg
--rw-rw-r--   0 boeing    (1000) boeing    (1000)     1052 2023-06-23 15:20:18.000000 ml-management-0.0.39/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/
+-rw-rw-r--   0 denis     (1000) denis     (1000)       18 2023-05-30 08:20:16.000000 ml-management-0.0.40/MANIFEST.in
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-08 12:48:25.000000 ml-management-0.0.40/ML_management/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      120 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1092 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      456 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1318 2023-06-08 08:02:27.000000 ml-management-0.0.40/ML_management/collectors/collectors.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/dummy/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      463 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.502761 ml-management-0.0.40/ML_management/collectors/s3/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10609 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)   331440 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3167 2023-06-05 06:12:04.000000 ml-management-0.0.40/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/dataset_loader_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2407 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/executor_template/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      895 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      843 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      869 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4566 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      402 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      334 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/mlmanagement/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      737 2023-06-29 10:47:21.000000 ml-management-0.0.40/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3392 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5054 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    14229 2023-06-29 10:47:21.000000 ml-management-0.0.40/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)    10260 2023-06-26 13:36:25.000000 ml-management-0.0.40/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      201 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     5001 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      316 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/models/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      949 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/models/patterns/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     4202 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      561 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      445 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      457 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/registry/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2566 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/exceptions.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     7556 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/tests/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/tests/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     3361 2023-05-30 08:20:16.000000 ml-management-0.0.40/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     9275 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ML_management/uploader_data/
+-rw-rw-r--   0 denis     (1000) denis     (1000)        0 2023-06-05 06:12:01.000000 ml-management-0.0.40/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1694 2023-06-21 07:06:27.000000 ml-management-0.0.40/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      394 2023-06-29 11:20:50.506761 ml-management-0.0.40/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)       56 2023-05-30 08:20:16.000000 ml-management-0.0.40/README.md
+-rw-rw-r--   0 denis     (1000) denis     (1000)        7 2023-06-29 11:15:02.000000 ml-management-0.0.40/VERSION
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-06-29 11:20:50.506761 ml-management-0.0.40/ml_management.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)      394 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2449 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)      153 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       14 2023-06-29 11:20:50.000000 ml-management-0.0.40/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       38 2023-06-29 11:20:50.506761 ml-management-0.0.40/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1052 2023-06-26 13:36:25.000000 ml-management-0.0.40/setup.py
```

### Comparing `ml-management-0.0.39/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.40/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/collectors/collectors.py` & `ml-management-0.0.40/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.40/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.40/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.40/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.40/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.40/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.40/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.40/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.40/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.40/ML_management/mlmanagement/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,12 @@
 set_tag = mlmanagement.set_tag
 autolog = mlmanagement.autolog
 load_model = mlmanagement.load_model
 save_model = mlmanagement.save_model
 active_run = mlmanagement.active_run
 get_run = mlmanagement.get_run
 end_run = mlmanagement.end_run
+log_artifact = mlmanagement.log_artifact
+log_artifacts = mlmanagement.log_artifacts
+log_param = mlmanagement.log_param
+log_params = mlmanagement.log_params
 MlflowClient = mlmanagement.MlflowClient
```

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.40/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.40/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.40/ML_management/mlmanagement/mlmanagement.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,34 @@
 
     If no run is active, this method will create a new active run.
     """
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
+def log_param(key: str, value: Any) -> Any:
+    """
+    Log a parameter (e.g. model hyperparameter) under the current run.
+
+    If no run is active, this method will create a new active run.
+    """
+    start_run_if_not_exist()
+    return request_for_function(inspect.currentframe())
+
+
+def log_params(params: Dict[str, Any]) -> None:
+    """
+    Log a batch of params for the current run.
+
+    If no run is active, this method will create a new active run.
+    """
+    start_run_if_not_exist()
+    return request_for_function(inspect.currentframe())
+
+
 def set_tag(key: str, value: Any) -> None:
     """Set a tag under the current run. If no run is active, this method will create a new active run."""
     start_run_if_not_exist()
     return request_for_function(inspect.currentframe())
 
 
 def autolog(
```

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.40/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.40/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.40/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.40/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.40/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/registry/exceptions.py` & `ml-management-0.0.40/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/registry/registry_manager.py` & `ml-management-0.0.40/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.40/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.40/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.40/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.40/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.39/setup.py` & `ml-management-0.0.40/setup.py`

 * *Files identical despite different names*

