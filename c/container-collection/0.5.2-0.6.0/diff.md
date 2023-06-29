# Comparing `tmp/container_collection-0.5.2.tar.gz` & `tmp/container_collection-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "container_collection-0.5.2.tar", max compression
+gzip compressed data, was "container_collection-0.6.0.tar", max compression
```

## Comparing `container_collection-0.5.2.tar` & `container_collection-0.6.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1519 2023-03-30 00:44:27.092081 container_collection-0.5.2/LICENSE
--rw-r--r--   0        0        0      772 2023-03-30 00:44:27.092081 container_collection-0.5.2/README.md
--rw-r--r--   0        0        0     1910 2023-03-30 00:44:27.092081 container_collection-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/__init__.py
--rw-r--r--   0        0        0       52 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/__main__.py
--rw-r--r--   0        0        0      561 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/__init__.py
--rw-r--r--   0        0        0     1087 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/check_batch_job.py
--rw-r--r--   0        0        0      829 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/get_batch_logs.py
--rw-r--r--   0        0        0      738 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/make_batch_job.py
--rw-r--r--   0        0        0      682 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/register_batch_job.py
--rw-r--r--   0        0        0      561 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/submit_batch_job.py
--rw-r--r--   0        0        0      214 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/batch/terminate_batch_job.py
--rw-r--r--   0        0        0      880 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/__init__.py
--rw-r--r--   0        0        0      677 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/check_docker_job.py
--rw-r--r--   0        0        0      302 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/clean_docker_job.py
--rw-r--r--   0        0        0      299 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/create_docker_volume.py
--rw-r--r--   0        0        0      510 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/get_docker_logs.py
--rw-r--r--   0        0        0      321 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/make_docker_job.py
--rw-r--r--   0        0        0      108 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/remove_docker_volume.py
--rw-r--r--   0        0        0      637 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/run_docker_command.py
--rw-r--r--   0        0        0      462 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/submit_docker_job.py
--rw-r--r--   0        0        0      189 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/docker/terminate_docker_job.py
--rw-r--r--   0        0        0      540 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/fargate/__init__.py
--rw-r--r--   0        0        0     1151 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/fargate/check_fargate_task.py
--rw-r--r--   0        0        0     1250 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/fargate/make_fargate_task.py
--rw-r--r--   0        0        0      727 2023-03-30 00:44:27.092081 container_collection-0.5.2/src/container_collection/fargate/register_fargate_task.py
--rw-r--r--   0        0        0      997 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/fargate/submit_fargate_task.py
--rw-r--r--   0        0        0      205 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/fargate/terminate_fargate_task.py
--rw-r--r--   0        0        0      495 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/manifest/__init__.py
--rw-r--r--   0        0        0     1894 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/manifest/filter_manifest_files.py
--rw-r--r--   0        0        0      921 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/manifest/find_missing_conditions.py
--rw-r--r--   0        0        0     1363 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/manifest/summarize_manifest_files.py
--rw-r--r--   0        0        0      989 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/manifest/update_manifest_contents.py
--rw-r--r--   0        0        0        0 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/py.typed
--rw-r--r--   0        0        0      144 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/template/__init__.py
--rw-r--r--   0        0        0      319 2023-03-30 00:44:27.096081 container_collection-0.5.2/src/container_collection/template/generate_input_contents.py
--rw-r--r--   0        0        0     1571 1970-01-01 00:00:00.000000 container_collection-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-06-29 20:59:21.273187 container_collection-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2550 2023-06-29 20:59:21.273187 container_collection-0.6.0/README.md
+-rw-r--r--   0        0        0     1926 2023-06-29 20:59:21.277187 container_collection-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/__init__.py
+-rw-r--r--   0        0        0       52 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/__main__.py
+-rw-r--r--   0        0        0      561 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/__init__.py
+-rw-r--r--   0        0        0     1087 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/check_batch_job.py
+-rw-r--r--   0        0        0      829 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/get_batch_logs.py
+-rw-r--r--   0        0        0      650 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/make_batch_job.py
+-rw-r--r--   0        0        0      682 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/register_batch_job.py
+-rw-r--r--   0        0        0      561 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/submit_batch_job.py
+-rw-r--r--   0        0        0      214 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/batch/terminate_batch_job.py
+-rw-r--r--   0        0        0      880 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/docker/__init__.py
+-rw-r--r--   0        0        0      677 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/docker/check_docker_job.py
+-rw-r--r--   0        0        0      302 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/docker/clean_docker_job.py
+-rw-r--r--   0        0        0      299 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/docker/create_docker_volume.py
+-rw-r--r--   0        0        0      510 2023-06-29 20:59:21.277187 container_collection-0.6.0/src/container_collection/docker/get_docker_logs.py
+-rw-r--r--   0        0        0      321 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/docker/make_docker_job.py
+-rw-r--r--   0        0        0      108 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/docker/remove_docker_volume.py
+-rw-r--r--   0        0        0      637 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/docker/run_docker_command.py
+-rw-r--r--   0        0        0      462 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/docker/submit_docker_job.py
+-rw-r--r--   0        0        0      189 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/docker/terminate_docker_job.py
+-rw-r--r--   0        0        0      540 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/__init__.py
+-rw-r--r--   0        0        0     1151 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/check_fargate_task.py
+-rw-r--r--   0        0        0     1250 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/make_fargate_task.py
+-rw-r--r--   0        0        0      727 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/register_fargate_task.py
+-rw-r--r--   0        0        0      997 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/submit_fargate_task.py
+-rw-r--r--   0        0        0      205 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/fargate/terminate_fargate_task.py
+-rw-r--r--   0        0        0      495 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/manifest/__init__.py
+-rw-r--r--   0        0        0     1894 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/manifest/filter_manifest_files.py
+-rw-r--r--   0        0        0      921 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/manifest/find_missing_conditions.py
+-rw-r--r--   0        0        0     1363 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/manifest/summarize_manifest_files.py
+-rw-r--r--   0        0        0      989 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/manifest/update_manifest_contents.py
+-rw-r--r--   0        0        0        0 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/py.typed
+-rw-r--r--   0        0        0      144 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/template/__init__.py
+-rw-r--r--   0        0        0      319 2023-06-29 20:59:21.281187 container_collection-0.6.0/src/container_collection/template/generate_input_contents.py
+-rw-r--r--   0        0        0     3349 1970-01-01 00:00:00.000000 container_collection-0.6.0/PKG-INFO
```

### Comparing `container_collection-0.5.2/LICENSE` & `container_collection-0.6.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, Bagheri Lab
+Copyright (c) 2023, Bagheri Lab
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `container_collection-0.5.2/pyproject.toml` & `container_collection-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "container-collection"
-version = "0.5.2"
+version = "0.6.0"
 description = "Collection of tasks for running containerized models."
 authors = [
     "Jessica S. Yu <jesyu@uw.edu>"
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -17,23 +17,24 @@
 docker = "^6.0.1"
 deepdiff = "^5.8.1"
 tabulate = "^0.9.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
 isort = "^5.12.0"
-mypy = "^0.991"
+mypy = "^1.3.0"
 pylint = "^2.16.2"
-pytest = "^7.2.0"
+pytest = "^7.3.0"
 pytest-cov = "^4.0.0"
-pytest-subtests = "^0.8.0"
-Sphinx = "^5.3.0"
-sphinx-rtd-theme = "^1.2.0"
-sphinx_mdinclude = "^0.5.3"
-tox = "^3.26.0"
+pytest-subtests = "^0.11.0"
+sphinx = "^7.0.1"
+furo = "^2023.5.20"
+myst-parser = "^2.0.0"
+sphinx-copybutton = "^0.5.2"
+tox = "^4.5.1"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `container_collection-0.5.2/src/container_collection/batch/__init__.py` & `container_collection-0.6.0/src/container_collection/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/batch/check_batch_job.py` & `container_collection-0.6.0/src/container_collection/batch/check_batch_job.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/batch/get_batch_logs.py` & `container_collection-0.6.0/src/container_collection/batch/get_batch_logs.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/batch/register_batch_job.py` & `container_collection-0.6.0/src/container_collection/batch/register_batch_job.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/batch/submit_batch_job.py` & `container_collection-0.6.0/src/container_collection/batch/submit_batch_job.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/docker/__init__.py` & `container_collection-0.6.0/src/container_collection/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/docker/check_docker_job.py` & `container_collection-0.6.0/src/container_collection/docker/check_docker_job.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/docker/run_docker_command.py` & `container_collection-0.6.0/src/container_collection/docker/run_docker_command.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/fargate/__init__.py` & `container_collection-0.6.0/src/container_collection/fargate/__init__.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/fargate/check_fargate_task.py` & `container_collection-0.6.0/src/container_collection/fargate/check_fargate_task.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/fargate/make_fargate_task.py` & `container_collection-0.6.0/src/container_collection/fargate/make_fargate_task.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/fargate/register_fargate_task.py` & `container_collection-0.6.0/src/container_collection/fargate/register_fargate_task.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/fargate/submit_fargate_task.py` & `container_collection-0.6.0/src/container_collection/fargate/submit_fargate_task.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/manifest/filter_manifest_files.py` & `container_collection-0.6.0/src/container_collection/manifest/filter_manifest_files.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/manifest/find_missing_conditions.py` & `container_collection-0.6.0/src/container_collection/manifest/find_missing_conditions.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/manifest/summarize_manifest_files.py` & `container_collection-0.6.0/src/container_collection/manifest/summarize_manifest_files.py`

 * *Files identical despite different names*

### Comparing `container_collection-0.5.2/src/container_collection/manifest/update_manifest_contents.py` & `container_collection-0.6.0/src/container_collection/manifest/update_manifest_contents.py`

 * *Files identical despite different names*

