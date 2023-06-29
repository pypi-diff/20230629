# Comparing `tmp/cmflib-0.0.3.tar.gz` & `tmp/cmflib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmflib-0.0.3.tar", last modified: Fri May 12 20:03:53 2023, max compression
+gzip compressed data, was "cmflib-0.0.4.tar", last modified: Thu Jun 29 20:44:41 2023, max compression
```

## Comparing `cmflib-0.0.3.tar` & `cmflib-0.0.4.tar`

### file list

```diff
@@ -1,67 +1,70 @@
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/
--rw-r--r--   0 royann   (121683555) users      (100)    11356 2023-03-01 22:34:14.000000 cmflib-0.0.3/LICENSE
--rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-05-12 20:03:53.688822 cmflib-0.0.3/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)    10154 2023-04-25 18:07:06.000000 cmflib-0.0.3/README.md
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-03-01 22:34:14.000000 cmflib-0.0.3/cmflib/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/bin/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/bin/__init__.py
--rwxr-xr-x   0 royann   (121683555) users      (100)      214 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/bin/cmf
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/cli/
--rw-r--r--   0 royann   (121683555) users      (100)     1665 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)      910 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/command.py
--rw-r--r--   0 royann   (121683555) users      (100)     2912 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/parser.py
--rw-r--r--   0 royann   (121683555) users      (100)     2148 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cli/utils.py
--rw-r--r--   0 royann   (121683555) users      (100)    57153 2023-05-12 17:30:36.000000 cmflib-0.0.3/cmflib/cmf.py
--rw-r--r--   0 royann   (121683555) users      (100)     6341 2023-05-12 17:24:33.000000 cmflib-0.0.3/cmflib/cmf_merger.py
--rw-r--r--   0 royann   (121683555) users      (100)    16923 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/cmfquery.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/artifact/
--rw-r--r--   0 royann   (121683555) users      (100)     1450 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     9043 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/pull.py
--rw-r--r--   0 royann   (121683555) users      (100)     1612 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/artifact/push.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/init/
--rw-r--r--   0 royann   (121683555) users      (100)     1543 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/init/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     5163 2023-05-12 17:25:32.000000 cmflib-0.0.3/cmflib/commands/init/amazonS3.py
--rw-r--r--   0 royann   (121683555) users      (100)     4610 2023-05-12 17:25:48.000000 cmflib-0.0.3/cmflib/commands/init/local.py
--rw-r--r--   0 royann   (121683555) users      (100)     5496 2023-05-12 17:26:14.000000 cmflib-0.0.3/cmflib/commands/init/minioS3.py
--rw-r--r--   0 royann   (121683555) users      (100)     2094 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/init/show.py
--rw-r--r--   0 royann   (121683555) users      (100)     5403 2023-05-12 17:25:12.000000 cmflib-0.0.3/cmflib/commands/init/sshremote.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/commands/metadata/
--rw-r--r--   0 royann   (121683555) users      (100)     1444 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     4131 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/pull.py
--rw-r--r--   0 royann   (121683555) users      (100)     4830 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/commands/metadata/push.py
--rw-r--r--   0 royann   (121683555) users      (100)    15584 2023-04-25 19:37:49.000000 cmflib-0.0.3/cmflib/dvc_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    20186 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/graph_wrapper.py
--rw-r--r--   0 royann   (121683555) users      (100)    19118 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/metadata_helper.py
--rw-r--r--   0 royann   (121683555) users      (100)      179 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/mlmd_objects.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib/server_interface/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/server_interface/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)      657 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/server_interface/server_interface.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/cmflib/storage_backends/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     1713 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/amazonS3_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     1793 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/local_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     1779 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/minio_artifacts.py
--rw-r--r--   0 royann   (121683555) users      (100)     2166 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/storage_backends/sshremote_artifacts.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/cmflib/utils/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     1477 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/cmf_config.py
--rw-r--r--   0 royann   (121683555) users      (100)     1300 2023-04-25 18:07:06.000000 cmflib-0.0.3/cmflib/utils/dvc_config.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.684822 cmflib-0.0.3/cmflib.egg-info/
--rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/PKG-INFO
--rw-r--r--   0 royann   (121683555) users      (100)     1409 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/SOURCES.txt
--rw-r--r--   0 royann   (121683555) users      (100)        1 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/dependency_links.txt
--rw-r--r--   0 royann   (121683555) users      (100)      113 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/requires.txt
--rw-r--r--   0 royann   (121683555) users      (100)       14 2023-05-12 20:03:53.000000 cmflib-0.0.3/cmflib.egg-info/top_level.txt
--rw-r--r--   0 royann   (121683555) users      (100)      433 2023-05-12 19:54:35.000000 cmflib-0.0.3/pyproject.toml
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/server/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/__init__.py
-drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-05-12 20:03:53.688822 cmflib-0.0.3/server/app/
--rw-r--r--   0 royann   (121683555) users      (100)        0 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/__init__.py
--rw-r--r--   0 royann   (121683555) users      (100)     1966 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/get_data.py
--rw-r--r--   0 royann   (121683555) users      (100)     6573 2023-05-12 17:24:33.000000 cmflib-0.0.3/server/app/main.py
--rw-r--r--   0 royann   (121683555) users      (100)     1413 2023-04-25 18:07:06.000000 cmflib-0.0.3/server/app/query_visualization.py
--rw-r--r--   0 royann   (121683555) users      (100)      103 2023-05-12 20:03:53.688822 cmflib-0.0.3/setup.cfg
--rw-r--r--   0 royann   (121683555) users      (100)     1106 2023-04-25 18:07:06.000000 cmflib-0.0.3/setup.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.778371 cmflib-0.0.4/
+-rw-r--r--   0 royann   (121683555) users      (100)    11356 2023-06-29 20:39:18.000000 cmflib-0.0.4/LICENSE
+-rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-06-29 20:44:41.778371 cmflib-0.0.4/PKG-INFO
+-rw-r--r--   0 royann   (121683555) users      (100)    10154 2023-06-29 20:39:18.000000 cmflib-0.0.4/README.md
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.770371 cmflib-0.0.4/cmflib/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.770371 cmflib-0.0.4/cmflib/bin/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/bin/__init__.py
+-rwxr-xr-x   0 royann   (121683555) users      (100)      214 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/bin/cmf
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/cli/
+-rw-r--r--   0 royann   (121683555) users      (100)     1665 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cli/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)      910 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cli/command.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2912 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cli/parser.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2148 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cli/utils.py
+-rw-r--r--   0 royann   (121683555) users      (100)    64863 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cmf.py
+-rw-r--r--   0 royann   (121683555) users      (100)     6755 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cmf_merger.py
+-rw-r--r--   0 royann   (121683555) users      (100)    18141 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/cmfquery.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/commands/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/commands/artifact/
+-rw-r--r--   0 royann   (121683555) users      (100)     1450 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/artifact/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     9043 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/artifact/pull.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1612 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/artifact/push.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/commands/init/
+-rw-r--r--   0 royann   (121683555) users      (100)     1543 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5163 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/amazonS3.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4610 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/local.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5496 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/minioS3.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2094 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/show.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5403 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/init/sshremote.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/commands/metadata/
+-rw-r--r--   0 royann   (121683555) users      (100)     1444 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/metadata/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4131 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/metadata/pull.py
+-rw-r--r--   0 royann   (121683555) users      (100)     4998 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/commands/metadata/push.py
+-rw-r--r--   0 royann   (121683555) users      (100)    15572 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/dvc_wrapper.py
+-rw-r--r--   0 royann   (121683555) users      (100)    20186 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/graph_wrapper.py
+-rw-r--r--   0 royann   (121683555) users      (100)    19237 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/metadata_helper.py
+-rw-r--r--   0 royann   (121683555) users      (100)      197 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/mlmd_objects.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/server_interface/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/server_interface/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)      657 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/server_interface/server_interface.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/storage_backends/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/storage_backends/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1713 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/storage_backends/amazonS3_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1793 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/storage_backends/local_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1779 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/storage_backends/minio_artifacts.py
+-rw-r--r--   0 royann   (121683555) users      (100)     2166 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/storage_backends/sshremote_artifacts.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.774371 cmflib-0.0.4/cmflib/utils/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/utils/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1477 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/utils/cmf_config.py
+-rw-r--r--   0 royann   (121683555) users      (100)     1300 2023-06-29 20:39:18.000000 cmflib-0.0.4/cmflib/utils/dvc_config.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.770371 cmflib-0.0.4/cmflib.egg-info/
+-rw-r--r--   0 royann   (121683555) users      (100)    10629 2023-06-29 20:44:41.000000 cmflib-0.0.4/cmflib.egg-info/PKG-INFO
+-rw-r--r--   0 royann   (121683555) users      (100)     1472 2023-06-29 20:44:41.000000 cmflib-0.0.4/cmflib.egg-info/SOURCES.txt
+-rw-r--r--   0 royann   (121683555) users      (100)        1 2023-06-29 20:44:41.000000 cmflib-0.0.4/cmflib.egg-info/dependency_links.txt
+-rw-r--r--   0 royann   (121683555) users      (100)      113 2023-06-29 20:44:41.000000 cmflib-0.0.4/cmflib.egg-info/requires.txt
+-rw-r--r--   0 royann   (121683555) users      (100)       14 2023-06-29 20:44:41.000000 cmflib-0.0.4/cmflib.egg-info/top_level.txt
+-rw-r--r--   0 royann   (121683555) users      (100)      433 2023-06-29 20:41:38.000000 cmflib-0.0.4/pyproject.toml
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.778371 cmflib-0.0.4/server/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/__init__.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.778371 cmflib-0.0.4/server/app/
+-rw-r--r--   0 royann   (121683555) users      (100)        0 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)     5809 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/get_data.py
+-rw-r--r--   0 royann   (121683555) users      (100)     3839 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/main.py
+-rw-r--r--   0 royann   (121683555) users      (100)     3154 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/query_visualization.py
+drwxr-xr-x   0 royann   (121683555) users      (100)        0 2023-06-29 20:44:41.778371 cmflib-0.0.4/server/app/schemas/
+-rw-r--r--   0 royann   (121683555) users      (100)        1 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/schemas/__init__.py
+-rw-r--r--   0 royann   (121683555) users      (100)      188 2023-06-29 20:39:18.000000 cmflib-0.0.4/server/app/schemas/dataframe.py
+-rw-r--r--   0 royann   (121683555) users      (100)      103 2023-06-29 20:44:41.778371 cmflib-0.0.4/setup.cfg
+-rw-r--r--   0 royann   (121683555) users      (100)     1106 2023-06-29 20:42:13.000000 cmflib-0.0.4/setup.py
```

### Comparing `cmflib-0.0.3/LICENSE` & `cmflib-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/PKG-INFO` & `cmflib-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
 Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cmflib-0.0.3/README.md` & `cmflib-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/cli/__init__.py` & `cmflib-0.0.4/cmflib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/cli/command.py` & `cmflib-0.0.4/cmflib/cli/command.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/cli/parser.py` & `cmflib-0.0.4/cmflib/cli/parser.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/cli/utils.py` & `cmflib-0.0.4/cmflib/cli/utils.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/cmf.py` & `cmflib-0.0.4/cmflib/cmf.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,16 +181,16 @@
         if not check_git_repo():
             print(
                 "*** Not a git repo, Please do the following ***\n"
                 "*** Run Command cmf init ***"
             )
             sys.exit(1)
 
-    def __del__(self):
-        git_commit(self.execution.id)
+    def finalize(self):
+        git_commit(self.execution_name)
         if self.graph:
             self.driver.close()
 
     def create_context(
         self, pipeline_stage: str, custom_properties: t.Optional[t.Dict] = None
     ) -> mlpb.Context:
         """Create's a  context(stage).
@@ -325,27 +325,33 @@
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
         git_start_commit = git_get_commit()
         cmd = str(sys.argv) if cmd is None else cmd
         self.execution = create_new_execution_in_existing_run_context(
             store=self.store,
             # Type field when re-using executions
-            execution_type_name=self.child_context.name+'_'+str(uuid.uuid1()),
+            execution_type_name=self.child_context.name,
             execution_name=execution_type, 
             #Name field if we are re-using executions
             #Type field , if creating new executions always 
             context_id=self.child_context.id,
             execution=cmd,
             pipeline_id=self.parent_context.id,
             pipeline_type=self.parent_context.name,
             git_repo=git_repo,
             git_start_commit=git_start_commit,
             custom_properties=custom_props,
             create_new_execution=create_new_execution,
         )
+        uuids = self.execution.properties["Execution_uuid"].string_value
+        if uuids:
+            self.execution.properties["Execution_uuid"].string_value = uuids+","+str(uuid.uuid1())
+        else:
+            self.execution.properties["Execution_uuid"].string_value = str(uuid.uuid1())            
+        self.store.put_executions([self.execution])
         self.execution_name = str(self.execution.id) + "," + execution_type
         self.execution_command = cmd
         for k, v in custom_props.items():
             k = re.sub("-", "_", k)
             self.execution_label_props[k] = v
         self.execution_label_props["Execution_Name"] = (
             execution_type + ":" + str(self.execution.id)
@@ -368,15 +374,15 @@
         """Updates an existing execution.
         The custom properties can be updated after creation of the execution.
         The new custom properties is merged with earlier custom properties.
         """
         self.execution = self.store.get_executions_by_id([execution_id])[0]
         if self.execution is None:
             print("Error - no execution id")
-            sys.exit(1)
+            return
         execution_type = self.store.get_execution_types_by_id([self.execution.type_id])[
             0
         ]
 
         if custom_properties:
             for key, value in custom_properties.items():
                 if isinstance(value, int):
@@ -419,44 +425,65 @@
 
     def merge_created_execution(
         self,
         execution_type: str,
         execution_cmd: str,
         properties: t.Optional[t.Dict] = None,
         custom_properties: t.Optional[t.Dict] = None,
+        orig_execution_name:str = "",
+        create_new_execution:bool = True
     ) -> mlpb.Execution:
         # Initializing the execution related fields
         properties = {} if properties is None else properties
         self.metrics = {}
         self.input_artifacts = []
         self.execution_label_props = {}
         custom_props = {} if custom_properties is None else custom_properties
         # print(custom_props)
         git_repo = properties.get("Git_Repo", "")
         git_start_commit = properties.get("Git_Start_Commit", "")
-        name = properties.get("Name", "")
+        #name = properties.get("Name", "")
         create_new_execution = True
         execution_name = execution_type
-        if name != "":
+        #exe.name property is passed as the orig_execution_name.
+        #if name is not an empty string then we are re-using executions
+        if orig_execution_name != "":
             create_new_execution = False
-            execution_name = name
+            execution_name = orig_execution_name
 
         self.execution = create_new_execution_in_existing_run_context(
             store=self.store,
-            execution_type_name=execution_type,
-            execution_name=execution_name,
+            execution_type_name=execution_type, # Type field when re-using executions
+            execution_name=execution_name, #Name field if we are re-using executionsname
+                                           #Type field , if creating new executions always
             context_id=self.child_context.id,
             execution=execution_cmd,
             pipeline_id=self.parent_context.id,
             pipeline_type=self.parent_context.name,
             git_repo=git_repo,
             git_start_commit=git_start_commit,
             custom_properties=custom_props,
             create_new_execution=create_new_execution
         )
+
+        uuids = ""
+
+        if "Execution_uuid" in self.execution.properties:
+            uuids = self.execution.properties["Execution_uuid"].string_value
+            if uuids:
+                self.execution.properties["Execution_uuid"].string_value = uuids +\
+                    ","+properties["Execution_uuid"]
+            else:
+                self.execution.properties["Execution_uuid"].string_value =\
+                    properties["Execution_uuid"]
+        else:
+            self.execution.properties["Execution_uuid"].string_value = str(uuid.uuid1())
+
+        
+        self.store.put_executions([self.execution])
         self.execution_name = str(self.execution.id) + "," + execution_type
         self.execution_command = execution_cmd
         for k, v in custom_props.items():
             k = re.sub("-", "_", k)
             self.execution_label_props[k] = v
         self.execution_label_props["Execution_Name"] = (
             execution_type + ":" + str(self.execution.id)
@@ -499,14 +526,19 @@
         Args:
              url: The path to the dataset.
              event: Takes arguments `INPUT` OR `OUTPUT`.
              custom_properties: Dataset properties (key/value pairs).
         Returns:
             Artifact object from ML Metadata library associated with the new dataset artifact.
         """
+                ### To Do : Technical Debt. 
+        # If the dataset already exist , then we just link the existing dataset to the execution
+        # We do not update the dataset properties . 
+        # We need to append the new properties to the existing dataset properties
+
         custom_props = {} if custom_properties is None else custom_properties
         git_repo = git_get_repo()
         name = re.split("/", url)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
         if event.lower() == "input":
             event_type = mlpb.Event.Type.INPUT
@@ -776,14 +808,18 @@
             model_framework: Framework used to create the model.
             model_type: Type of model algorithm used.
             model_name: Name of the algorithm used.
             custom_properties: The model properties.
         Returns:
             Artifact object from ML Metadata library associated with the new model artifact.
         """
+        # To Do : Technical Debt. 
+        # If the model already exist , then we just link the existing model to the execution
+        # We do not update the model properties . 
+        # We need to append the new properties to the existing model properties
 
         if custom_properties is None:
             custom_properties = {}
         custom_props = {} if custom_properties is None else custom_properties
         # name = re.split('/', path)[-1]
         event_type = mlpb.Event.Type.OUTPUT
         existing_artifact = []
@@ -806,15 +842,14 @@
             existing_artifact.extend(self.store.get_artifacts_by_uri(uri))
         else:
             raise RuntimeError("Model commit failed, Model uri empty")
 
         if (
             existing_artifact
             and len(existing_artifact) != 0
-            and event_type == mlpb.Event.Type.INPUT
         ):
             # update url for existing artifact
             existing_artifact = self.update_model_url(
                 existing_artifact, url_with_pipeline
             )
             artifact = link_execution_to_artifact(
                 store=self.store,
@@ -851,14 +886,15 @@
                     "url": mlpb.STRING,
                 },
                 custom_properties=custom_props,
                 milliseconds_since_epoch=int(time.time() * 1000),
             )
         # custom_properties["Commit"] = model_commit
         self.execution_label_props["Commit"] = model_commit
+        #To DO model nodes should be similar to dataset nodes when we create neo4j
         if self.graph:
             self.driver.create_model_node(
                 model_uri,
                 uri,
                 event,
                 self.execution.id,
                 self.parent_context,
@@ -956,15 +992,14 @@
             existing_artifact.extend(self.store.get_artifacts_by_uri(uri))
         else:
             raise RuntimeError("Model commit failed, Model uri empty")
 
         if (
             existing_artifact
             and len(existing_artifact) != 0
-            and event_type == mlpb.Event.Type.INPUT
         ):
             # update url for existing artifact
             existing_artifact = self.update_model_url(existing_artifact, url)
             artifact = link_execution_to_artifact(
                 store=self.store,
                 execution_id=self.execution.id,
                 uri=c_hash,
@@ -1039,14 +1074,75 @@
                 }
                 self.driver.create_artifact_relationships(
                     self.input_artifacts, child_artifact, self.execution_label_props
                 )
 
         return artifact
 
+    def log_execution_metrics_from_client(self, metrics_name: str,
+                                         custom_properties: t.Optional[t.Dict] = None) -> mlpb.Artifact:
+        metrics = None
+        custom_props = {} if custom_properties is None else custom_properties
+        existing_artifact = []
+        name_tokens = metrics_name.split(":")
+        if name_tokens and len(name_tokens) > 2:
+            name = name_tokens[0]
+            uri = name_tokens[1]
+            execution_id = name_tokens[2]
+        else:
+            print(f"Error : metrics name {metrics_name} is not in the correct format")
+            return 
+
+        #we need to add the execution id to the metrics name
+        new_metrics_name = f"{name}:{uri}:{str(self.execution.id)}"
+        existing_artifacts = self.store.get_artifacts_by_uri(uri)
+
+        existing_artifact = existing_artifacts[0] if existing_artifacts else None
+        if not existing_artifact or \
+           ((existing_artifact) and not
+            (existing_artifact.name == new_metrics_name)):  #we need to add the artifact otherwise its already there 
+            metrics = create_new_artifact_event_and_attribution(
+            store=self.store,
+            execution_id=self.execution.id,
+            context_id=self.child_context.id,
+            uri=uri,
+            name=new_metrics_name,
+            type_name="Metrics",
+            event_type=mlpb.Event.Type.OUTPUT,
+            properties={"metrics_name": metrics_name},
+            artifact_type_properties={"metrics_name": mlpb.STRING},
+            custom_properties=custom_props,
+            milliseconds_since_epoch=int(time.time() * 1000),
+        )
+            if self.graph:
+                # To do create execution_links
+                self.driver.create_metrics_node(
+                    metrics_name,
+                    uri,
+                    "output",
+                    self.execution.id,
+                    self.parent_context,
+                    custom_props,
+                )
+                child_artifact = {
+                    "Name": metrics_name,
+                    "URI": uri,
+                    "Event": "output",
+                    "Execution_Name": self.execution_name,
+                    "Type": "Metrics",
+                    "Execution_Command": self.execution_command,
+                    "Pipeline_Id": self.parent_context.id,
+                    "Pipeline_Name": self.parent_context.name,
+                }
+                self.driver.create_artifact_relationships(
+                    self.input_artifacts, child_artifact, self.execution_label_props
+                )
+        return metrics
+
+
     def log_execution_metrics(
         self, metrics_name: str, custom_properties: t.Optional[t.Dict] = None
     ) -> mlpb.Artifact:
         """Log the metadata associated with the execution (coarse-grained tracking).
         It is stored as a metrics artifact. This does not have a backing physical file, unlike other artifacts that we
         have.
         Example:
@@ -1182,14 +1278,51 @@
                 "Pipeline_Id": self.parent_context.id,
             }
             self.driver.create_artifact_relationships(
                 self.input_artifacts, child_artifact, self.execution_label_props
             )
         return metrics
 
+    def commit_existing_metrics(self, metrics_name: str, uri: str, custom_properties: t.Optional[t.Dict] = None):
+        custom_props =  {} if custom_properties is None else custom_properties
+        metrics = create_new_artifact_event_and_attribution(
+            store=self.store,
+            execution_id=self.execution.id,
+            context_id=self.child_context.id,
+            uri=uri,
+            name=metrics_name,
+            type_name="Step_Metrics",
+            event_type=mlpb.Event.Type.OUTPUT,
+            custom_properties=custom_props,
+            milliseconds_since_epoch=int(time.time() * 1000),
+        )
+        if self.graph:
+            self.driver.create_metrics_node(
+                metrics_name,
+                uri,
+                "output",
+                self.execution.id,
+                self.parent_context,
+                custom_props,
+            )
+            child_artifact = {
+                "Name": metrics_name,
+                "URI": uri,
+                "Event": "output",
+                "Execution_Name": self.execution_name,
+                "Type": "Metrics",
+                "Execution_Command": self.execution_command,
+                "Pipeline_Id": self.parent_context.id,
+            }
+            self.driver.create_artifact_relationships(
+                self.input_artifacts, child_artifact, self.execution_label_props
+            )
+        return metrics
+
+
     def log_validation_output(
         self, version: str, custom_properties: t.Optional[t.Dict] = None
     ) -> object:
         uri = str(uuid.uuid1())
         return create_new_artifact_event_and_attribution(
             store=self.store,
             execution_id=self.execution.id,
@@ -1365,14 +1498,48 @@
                 )
             if self.writer.graph:
                 self.writer.driver.create_dataslice_node(
                     self.name, self.name + ":" + c_hash, c_hash, self.data_parent, props
                 )
             return slice
 
+        def commit_existing(self, uri: str, custom_properties: t.Optional[t.Dict] = None) -> None:
+            custom_props = {} if custom_properties is None else custom_properties
+            c_hash = uri
+            dataslice_commit = c_hash
+            existing_artifact = []
+            if c_hash and c_hash.strip():
+                existing_artifact.extend(
+                    self.writer.store.get_artifacts_by_uri(c_hash))
+            if existing_artifact and len(existing_artifact) != 0:
+                print("Adding to existing data slice")
+                slice = link_execution_to_input_artifact(
+                    store=self.writer.store,
+                    execution_id=self.writer.execution.id,
+                    uri=c_hash,
+                    input_name=self.name
+                )
+            else:
+                slice = create_new_artifact_event_and_attribution(
+                    store=self.writer.store,
+                    execution_id=self.writer.execution.id,
+                    context_id=self.writer.child_context.id,
+                    uri=c_hash,
+                    name=self.name,
+                    type_name="Dataslice",
+                    event_type=mlpb.Event.Type.OUTPUT,
+                    custom_properties=custom_properties,
+                    milliseconds_since_epoch=int(time.time() * 1000),
+                )
+            if self.writer.graph:
+                self.writer.driver.create_dataslice_node(
+                    self.name, self.name, c_hash, self.data_parent, custom_properties
+                )
+            return slice
+
 
 #        """Temporary code"""
 #
 #        def materialize(self, name):
 #            slicedir = name + "-" + "dir"
 #            os.mkdir(slicedir)
 #            df = pd.read_parquet(name)
```

### Comparing `cmflib-0.0.3/cmflib/cmf_merger.py` & `cmflib-0.0.4/cmflib/cmf_merger.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             custom_properties = stage["custom_properties"],
             )
             _ = cmf_class.merge_created_execution(
                 execution["properties"]["Context_Type"],
                 execution["properties"]["Execution"],
                 execution["properties"],
                 execution["custom_properties"],
+                execution["name"]
             )
             for event in execution["events"]:  # Iterates over all the events
                 artifact_type = event["artifact"]["type"]
                 event_type = event["type"]
                 artifact_name = (event["artifact"]["name"].split(":"))[0]
                 custom_props = event["artifact"]["custom_properties"]
                 props = event["artifact"]["properties"]
@@ -101,15 +102,20 @@
                         event="output",
                         props=props,
                         custom_properties=props,
                     )
                 elif artifact_type == "Metrics":
                     # print(props,'parse')
                     # cmf_class.log_execution_metrics_with_uuid(props, custom_props)
-                    cmf_class.log_execution_metrics(artifact_name, custom_props)
+                    cmf_class.log_execution_metrics_from_client(event["artifact"]["name"], custom_props)
+                elif artifact_type == "Dataslice":
+                    dataslice = cmf_class.create_dataslice(event["artifact"]["name"])
+                    dataslice.commit_existing(uri, custom_props)
+                elif artifact_type == "Step_Metrics":
+                    cmf_class.commit_existing_metrics(event["artifact"]["name"], uri, custom_props)
                 else:
                     pass
 
 
 # create_time_since_epoch is appended to mlmd pushed to cmf-server as original_create_time_since_epoch
 def create_original_time_since_epoch(mlmd_data):
     stages = []
```

### Comparing `cmflib-0.0.3/cmflib/cmfquery.py` & `cmflib-0.0.4/cmflib/cmfquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,52 +15,56 @@
 ###
 
 import pandas as pd
 from ml_metadata.metadata_store import metadata_store
 from ml_metadata.proto import metadata_store_pb2 as mlpb
 from cmflib.mlmd_objects import CONTEXT_LIST
 import json
+import typing as t
+
 
 
 class CmfQuery(object):
     def __init__(self, filepath: str = "mlmd"):
         config = mlpb.ConnectionConfig()
         config.sqlite.filename_uri = filepath
         self.store = metadata_store.MetadataStore(config)
 
     def _transform_to_dataframe(self, node):
+        #d = CmfQuery.__get_node_properties(node)
         d = {"id": node.id}
+        d["name"] = getattr(node, "name", "")        
         for k, v in node.properties.items():
-            if v.HasField('string_value'):
-                d[k] = v.string_value
-            elif v.HasField('int_value'):
-                d[k] = v.int_value
-            else:
-                d[k] = v.double_value
+             if v.HasField('string_value'):
+                 d[k] = v.string_value
+             elif v.HasField('int_value'):
+                 d[k] = v.int_value
+             else:
+                 d[k] = v.double_value
 
         for k, v in node.custom_properties.items():
-            if v.HasField('string_value'):
-                d[k] = v.string_value
-            elif v.HasField('int_value'):
-                d[k] = v.int_value
-            else:
-                d[k] = v.double_value
+             if v.HasField('string_value'):
+                 d[k] = v.string_value
+             elif v.HasField('int_value'):
+                 d[k] = v.int_value
+             else:
+                 d[k] = v.double_value
 
         df = pd.DataFrame(d, index=[0, ])
         return df
 
     def get_pipeline_id(self, pipeline_name: str) -> int:
         contexts = self.store.get_contexts_by_type("Parent_Context")
         for ctx in contexts:
             if ctx.name == pipeline_name:
                 return ctx.id
-
         return -1
 
-    def get_pipeline_names(self) -> []:
+
+    def get_pipeline_names(self) -> t.List:
         names = []
         contexts = self.store.get_contexts_by_type("Parent_Context")
         for ctx in contexts:
             names.append(ctx.name)
         return names
 
     def get_pipeline_stages(self, pipeline_name: str) -> []:
@@ -69,14 +73,26 @@
         for ctx in contexts:
             if ctx.name == pipeline_name:
                 child_contexts = self.store.get_children_contexts_by_context(ctx.id)
                 for cc in child_contexts:
                     stages.append(cc.name)
         return stages
 
+    def get_all_exe_in_stage(self, stage_name: str) -> []:
+        df = pd.DataFrame()
+        contexts = self.store.get_contexts_by_type("Parent_Context")
+        executions = None
+        for ctx in contexts:
+            child_contexts = self.store.get_children_contexts_by_context(ctx.id)
+            for cc in child_contexts:
+                if cc.name == stage_name:
+                    executions = self.store.get_executions_by_context(cc.id)
+        return executions
+
+
     def get_all_executions_in_stage(self, stage_name: str) -> pd.DataFrame:
         df = pd.DataFrame()
         contexts = self.store.get_contexts_by_type("Parent_Context")
         for ctx in contexts:
             child_contexts = self.store.get_children_contexts_by_context(ctx.id)
             for cc in child_contexts:
                 if cc.name == stage_name:
@@ -105,14 +121,22 @@
             elif v.HasField('int_value'):
                 d[k] = v.int_value
             else:
                 d[k] = v.double_value
         df = pd.DataFrame(d, index=[0, ])
         return df
 
+    def get_all_artifacts(self) -> t.List:
+        artifact_list = []
+        artifacts = self.store.get_artifacts()
+        for art in artifacts:
+            name = art.name
+            artifact_list.append(name)
+        return artifact_list
+
     def get_artifact(self, name: str):
         artifact = None
         artifacts = self.store.get_artifacts()
         for art in artifacts:
             if art.name == name:
                 artifact = art
                 break
@@ -310,17 +334,16 @@
                 if attr == "properties":
                     node_dict["properties"] = CmfQuery.__get_properties(node)
                 elif attr == "custom_properties":
                     node_dict["custom_properties"] = CmfQuery.__get_customproperties(
                         node
                     )
                 else:
-                    node_dict[attr] = node.__getattribute__(attr)
+                    node_dict[attr] = getattr(node, attr, "")
 
-        # print(node_dict)
         return node_dict
 
     @staticmethod
     def __get_properties(node) -> dict:
         prop_dict = {}
         for k, v in node.properties.items():
             if v.HasField("string_value"):
@@ -331,14 +354,16 @@
                 prop_dict[k] = v.double_value
         return prop_dict
 
     @staticmethod
     def __get_customproperties(node) -> dict:
         prop_dict = {}
         for k, v in node.custom_properties.items():
+            if k == "type":
+                k = "user_type"
             if v.HasField("string_value"):
                 prop_dict[k] = v.string_value
             elif v.HasField("int_value"):
                 prop_dict[k] = v.int_value
             else:
                 prop_dict[k] = v.double_value
         return prop_dict
@@ -366,16 +391,19 @@
                     else:
                         return "Invalid execution id given."
                     for exe in list_executions:
                         exe_dict = CmfQuery.__get_node_properties(exe)
                         exe_type = self.store.get_execution_types_by_id([exe.type_id])
                         exe_dict["type"] = exe_type[0].name
                         exe_dict["events"] = []
-                        if exe.name != "":
-                            exe_dict["Name"] = exe.name
+                        # name will be an empty string for executions that are created with 
+                        # create new execution as true(default)
+                        # In other words name property will there only for execution 
+                        # that are created with create new execution flag set to false(special case)
+                        exe_dict["name"] = exe.name if exe.name != "" else ""
                         events = self.store.get_events_by_execution_ids([exe.id])
                         for evt in events:
                             evt_dict = CmfQuery.__get_node_properties(evt)
                             artifact = self.store.get_artifacts_by_id([evt.artifact_id])
                             if artifact is not None:
                                 artifact_type = self.store.get_artifact_types_by_id(
                                     [artifact[0].type_id]
@@ -406,7 +434,8 @@
                git_repo = v
            elif (k == "Revision"):
                rev = v
            elif (remote == "Remote"):
                remote = v
        
        Cmf.materialize(path, git_repo, rev, remote)'''
+
```

### Comparing `cmflib-0.0.3/cmflib/commands/artifact/__init__.py` & `cmflib-0.0.4/cmflib/commands/artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/artifact/pull.py` & `cmflib-0.0.4/cmflib/commands/artifact/pull.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/artifact/push.py` & `cmflib-0.0.4/cmflib/commands/artifact/push.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/__init__.py` & `cmflib-0.0.4/cmflib/commands/init/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/amazonS3.py` & `cmflib-0.0.4/cmflib/commands/init/amazonS3.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/local.py` & `cmflib-0.0.4/cmflib/commands/init/local.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/minioS3.py` & `cmflib-0.0.4/cmflib/commands/init/minioS3.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/show.py` & `cmflib-0.0.4/cmflib/commands/init/show.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/init/sshremote.py` & `cmflib-0.0.4/cmflib/commands/init/sshremote.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/metadata/__init__.py` & `cmflib-0.0.4/cmflib/commands/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/metadata/pull.py` & `cmflib-0.0.4/cmflib/commands/metadata/pull.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/commands/metadata/push.py` & `cmflib-0.0.4/cmflib/commands/metadata/push.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,16 +80,18 @@
                             break
                 if execution_flag == 0:
                     return "Given execution is not found in mlmd."
             else:
                 exec_id = None
                 response = server_interface.call_mlmd_push(json_payload, url, exec_id)
             status_code = response.status_code
-            if status_code == 200:
+            if status_code == 200 and response.json()['status']=="success":
                 return "mlmd is successfully pushed."
+            elif status_code==200 and response.json()["status"]=="exists":
+                return "Executions already exists."
             elif status_code == 404:
                 return "ERROR: cmf-server is not available."
             elif status_code == 500:
                 return "ERROR: Internal server error."
             else:
                 return "ERROR: Status Code = {status_code}. Unable to push mlmd."
         else:
```

### Comparing `cmflib-0.0.3/cmflib/dvc_wrapper.py` & `cmflib-0.0.4/cmflib/dvc_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,21 +231,21 @@
     process = ""
     try:
         process = subprocess.Popen(['dvc', 'add', folder],
                                    stdout=subprocess.PIPE,
                                    universal_newlines=True)
 
         # To-Do : Parse the output and report if error
-        output, errs = process.communicate(timeout=60)
+        output, errs = process.communicate()
         commit = output.strip()
         process = subprocess.Popen(['git', 'add', folder + '.dvc'],
                                    stdout=subprocess.PIPE,
                                    universal_newlines=True)
         # To-Do : Parse the output and report if error
-        # _, _ = process.communicate(timeout=60)
+        _, _ = process.communicate(timeout=60)
         # process = subprocess.Popen(
         #     [
         #         'git',
         #         'commit',
         #         '-m ' +
         #         'commiting dvc metadata file for ' +
         #         str(folder) +
```

### Comparing `cmflib-0.0.3/cmflib/graph_wrapper.py` & `cmflib-0.0.4/cmflib/graph_wrapper.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/metadata_helper.py` & `cmflib-0.0.4/cmflib/metadata_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import typing as t
 from time import sleep
 from ml_metadata.proto import metadata_store_pb2
 from ml_metadata.metadata_store import metadata_store
 from ipaddress import ip_address, IPv4Address
 from typing import List
 import functools
+import uuid
 
 
 def value_to_mlmd_value(value) -> metadata_store_pb2.Value:
     if value is None:
         return metadata_store_pb2.Value()
     if isinstance(value, int):
         return metadata_store_pb2.Value(int_value=value)
@@ -147,25 +148,25 @@
     artifact.id = store.put_artifacts([artifact])[0]
     return artifact
 
 
 def create_execution_with_type(
         store,
         type_name: str,
-        name:str,
+        name: str,
         properties: dict = None,
         type_properties: dict = None,
         custom_properties: t.Optional[t.Dict] = None,
-        create_new_execution:bool = True
+        create_new_execution: bool = True
 ) -> metadata_store_pb2.Execution:
     if create_new_execution:
         execution_type = get_or_create_execution_type(
-        store=store,
-        type_name=name,
-        properties=type_properties,
+        store = store,
+        type_name = name,
+        properties = type_properties,
         )
         execution = metadata_store_pb2.Execution(
             type_id=execution_type.id,
             properties=properties,
             custom_properties=custom_properties,
         )
         execution.id = store.put_executions([execution])[0]
@@ -256,20 +257,20 @@
                 context_name, context_types[0].name, type_name))
     return context
 
 
 def create_new_execution_in_existing_context(
         store,
         execution_type_name: str,
-        execution_name:str,
+        execution_name: str,
         context_id: int,
         properties: dict = None,
         execution_type_properties: dict = None,
         custom_properties: dict = None,
-        create_new_execution:bool = True
+        create_new_execution: bool = True
 ) -> metadata_store_pb2.Execution:
     execution = create_execution_with_type(
         store=store,
         properties=properties,
         custom_properties=custom_properties,
         type_name=execution_type_name,
         name=execution_name,
@@ -307,15 +308,15 @@
 
 EXECUTION_REPO = "Git_Repo"
 EXECUTION_START_COMMIT = "Git_Start_Commit"
 EXECUTION_END_COMMIT = "Git_End_Commit"
 EXECUTION_PIPELINE_TYPE = "Pipeline_Type"
 
 EXECUTION_PIPELINE_ID = "Pipeline_id"
-
+EXECUTION_UNIQUE_ID = "Execution_uuid"
 
 def get_or_create_parent_context(
         store,
         pipeline: str,
         custom_properties: t.Optional[t.Dict] = None
 ) -> metadata_store_pb2.Context:
     mlmd_custom_properties = {}
@@ -391,28 +392,30 @@
     for property_name, property_value in (custom_properties or {}).items():
         mlmd_custom_properties[property_name] = value_to_mlmd_value(
             property_value)
 
     return create_new_execution_in_existing_context(
         store=store,
         execution_type_name=execution_type_name,
-        execution_name = execution_name,
+        execution_name=execution_name,
         context_id=context_id,
         execution_type_properties={
+            EXECUTION_UNIQUE_ID: metadata_store_pb2.STRING,
             EXECUTION_CONTEXT_NAME_PROPERTY_NAME: metadata_store_pb2.STRING,
             EXECUTION_CONTEXT_ID: metadata_store_pb2.INT,
             EXECUTION_EXECUTION: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_TYPE: metadata_store_pb2.STRING,
             EXECUTION_PIPELINE_ID: metadata_store_pb2.INT,
             EXECUTION_REPO: metadata_store_pb2.STRING,
             EXECUTION_START_COMMIT: metadata_store_pb2.STRING,
             EXECUTION_END_COMMIT: metadata_store_pb2.STRING,
         },
 
         properties={
+
             EXECUTION_CONTEXT_NAME_PROPERTY_NAME: metadata_store_pb2.Value(string_value=execution_type_name),
             # Mistakenly used for grouping in the UX
             EXECUTION_CONTEXT_ID: metadata_store_pb2.Value(int_value=context_id),
             EXECUTION_EXECUTION: metadata_store_pb2.Value(string_value=execution),
             EXECUTION_PIPELINE_TYPE: metadata_store_pb2.Value(string_value=pipeline_type),
             EXECUTION_PIPELINE_ID: metadata_store_pb2.Value(int_value=pipeline_id),
             EXECUTION_REPO: metadata_store_pb2.Value(string_value=git_repo),
```

### Comparing `cmflib-0.0.3/cmflib/server_interface/server_interface.py` & `cmflib-0.0.4/cmflib/server_interface/server_interface.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/storage_backends/amazonS3_artifacts.py` & `cmflib-0.0.4/cmflib/storage_backends/amazonS3_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/storage_backends/local_artifacts.py` & `cmflib-0.0.4/cmflib/storage_backends/local_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/storage_backends/minio_artifacts.py` & `cmflib-0.0.4/cmflib/storage_backends/minio_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/storage_backends/sshremote_artifacts.py` & `cmflib-0.0.4/cmflib/storage_backends/sshremote_artifacts.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/utils/cmf_config.py` & `cmflib-0.0.4/cmflib/utils/cmf_config.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib/utils/dvc_config.py` & `cmflib-0.0.4/cmflib/utils/dvc_config.py`

 * *Files identical despite different names*

### Comparing `cmflib-0.0.3/cmflib.egg-info/PKG-INFO` & `cmflib-0.0.4/cmflib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmflib
-Version: 0.0.3
+Version: 0.0.4
 Summary: Track metadata for AI pipeline
 Author: Hewlett Packard Enterprise
 Project-URL: Homepage, https://github.com/HewlettPackard/cmf
 Project-URL: Bug Tracker, https://github.com/HewlettPackard/cmf/issues
 Keywords: python,first package
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `cmflib-0.0.3/cmflib.egg-info/SOURCES.txt` & `cmflib-0.0.4/cmflib.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -45,8 +45,10 @@
 cmflib/utils/__init__.py
 cmflib/utils/cmf_config.py
 cmflib/utils/dvc_config.py
 server/__init__.py
 server/app/__init__.py
 server/app/get_data.py
 server/app/main.py
-server/app/query_visualization.py
+server/app/query_visualization.py
+server/app/schemas/__init__.py
+server/app/schemas/dataframe.py
```

### Comparing `cmflib-0.0.3/server/app/main.py` & `cmflib-0.0.4/server/app/get_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,175 +1,137 @@
-# cmf-server api's
-
-from fastapi import FastAPI, Request
 from cmflib import cmfquery, cmf_merger
-from fastapi.templating import Jinja2Templates
-from fastapi.responses import HTMLResponse
-from fastapi.staticfiles import StaticFiles
-from server.app.get_data import get_executions, get_artifacts
-from server.app.query_visualization import query_visualization
-from pathlib import Path
-
+import pandas as pd
+import json,glob
 import os
-import json
-
-app = FastAPI()
-
-BASE_PATH = Path(__file__).resolve().parent
-templates = Jinja2Templates(directory=str(BASE_PATH/"template"))
-app.mount("/cmf-server/data/static", StaticFiles(directory="/cmf-server/data/static"), name="static")
-server_store_path = "/cmf-server/data/mlmd"
-
+from server.app.query_visualization import query_visualization
+from fastapi.responses import FileResponse
 
-@app.get("/")
-def read_root(request: Request):
-    return templates.TemplateResponse(
-        "home.html", {'request': request}
-    )
+def get_executions(mlmdfilepath, pipeline_name):
+    query = cmfquery.CmfQuery(mlmdfilepath)
+    stages = query.get_pipeline_stages(pipeline_name)
+    df = pd.DataFrame()
+    for stage in stages:
+        executions = query.get_all_executions_in_stage(stage)
+        if str(executions.Pipeline_Type[0]) == pipeline_name:
+            df = pd.concat([df, executions], sort=True, ignore_index=True)
+    return df
+
+
+# This function fetches all the artifacts available in given mlmd
+def get_artifacts(mlmdfilepath, pipeline_name, data):  # get_artifacts return value (artifact_type or artifact_df) is 
+  # determined by a data variable().
+    query = cmfquery.CmfQuery(mlmdfilepath)
+    names = query.get_pipeline_names()  # getting all pipeline names in mlmd
+    identifiers = []
+    for name in names:
+        if name==pipeline_name:
+            stages = query.get_pipeline_stages(name)
+            for stage in stages:
+                executions = query.get_all_executions_in_stage(stage)
+                dict_executions = executions.to_dict("dict")  # converting it to dictionary
+                for id in dict_executions["id"].values():
+                    identifiers.append(id)
+                identifiers.append(dict_executions["id"][0])
+    name = []
+    url = []
+    df = pd.DataFrame()
+    for identifier in identifiers:
+        get_artifacts = query.get_all_artifacts_for_execution(
+            identifier
+        )  # getting all artifacts
+        df = pd.concat([df, get_artifacts], sort=True, ignore_index=True)
+    df['event'] = df.groupby('id')['event'].transform(lambda x: ', '.join(x))
+    df['name'] = df['name'].str.split(':').str[0]
+    df=df.drop_duplicates()
+    if data == "artifact_type":
+        tempout = list(set(df["type"]))
+    else:
+        df = df.loc[df["type"] == data]
+        result = df.to_json(orient="records")
+        tempout = json.loads(result)
+    return tempout
 
 
-# api to posAt mlmd file to cmf-server
-@app.post("/mlmd_push")
-async def mlmd_push(info: Request):
-    req_info = await info.json()
+def create_unique_executions(server_store_path, req_info):
     mlmd_data = json.loads(req_info["json_payload"])
     pipelines = mlmd_data["Pipeline"]
     pipeline = pipelines[0]
     pipeline_name = pipeline["name"]
     executions_server = []
     list_executions_exists = []
     if os.path.exists(server_store_path):
         query = cmfquery.CmfQuery(server_store_path)
         stages = query.get_pipeline_stages(pipeline_name)
         for stage in stages:
             executions = []
             executions = query.get_all_executions_in_stage(stage)
-            for i in executions.index:
-                executions_server.append(executions['Context_Type'][i])
-
-            executions_client = []
-            for i in mlmd_data['Pipeline'][0][
-                "stages"
-            ]:  # checks if given execution_id present in mlmd
-                for j in i["executions"]:
-                    executions_client.append(j['properties']['Context_Type'])
-            if executions_server != []:
-                list_executions_exists = list(set(executions_client).intersection(set(executions_server)))
+            #print(executions)
+            for i in executions.index:                
+                for uuid in executions['Execution_uuid'][i].split(","):
+                    executions_server.append(uuid)
+        executions_client = []
+        for i in mlmd_data['Pipeline'][0]["stages"]:  # checks if given execution_id present in mlmd
+            for j in i["executions"]:
+                if j['name'] != "":#If executions have name , they are reusable executions                        
+                    continue       #which needs to be merged in irrespective of whether already 
+                                   #present or not so that new artifacts associated with it gets in.
+                for uuid in j['properties']['Execution_uuid'].split(","):
+                    executions_client.append(uuid)
+        if executions_server != []:
+            list_executions_exists = list(set(executions_client).intersection(set(executions_server)))
         for i in mlmd_data["Pipeline"]:
             for stage in i['stages']:
-                for exec in stage['executions']:
-                    if exec["properties"]["Context_Type"] in list_executions_exists:
-                        stage['executions'].remove(exec)
+                for cmf_exec in stage['executions'][:]:
+                    uuids = cmf_exec["properties"]["Execution_uuid"].split(",")
+                    for uuid in uuids:
+                        if uuid in list_executions_exists:
+                            stage['executions'].remove(cmf_exec)
+
         for i in mlmd_data["Pipeline"]:
-            for stage in i['stages']:
-                if len(stage['executions']) == 0:
-                    i['stages'].remove(stage)
+            i['stages']=[stage for stage in i['stages'] if stage['executions']!=[]]
     for i in mlmd_data["Pipeline"]:
-        if len(i['stages']) == 0:
-            print("Executions already exists")
+        if len(i['stages']) == 0 :
+            status="exists"
         else:
             cmf_merger.parse_json_to_mlmd(
                 json.dumps(mlmd_data), "/cmf-server/data/mlmd", "push", req_info["id"]
             )
-    return {"status": "success", "data": req_info}
+            status='success'
+    return status
 
 
-# api to get mlmd file from cmf-server
-@app.get("/mlmd_pull/{pipeline_name}", response_class=HTMLResponse)
-async def mlmd_pull(info: Request, pipeline_name: str):
-    # checks if mlmd file exists on server
-    req_info = await info.json()
-    if os.path.exists(server_store_path):
-        query = cmfquery.CmfQuery(server_store_path)
-        execution_flag = 0
-        # checks if given execution_id present in mlmd
-        if (
-                pipeline_name in query.get_pipeline_names()
-        ):  # checks if pipeline name is available in mlmd
-            json_payload = query.dumptojson(pipeline_name, None)
-            mlmd_data = json.loads(json_payload)["Pipeline"]
-            if req_info["exec_id"] == None:
-                json_payload = query.dumptojson(pipeline_name, req_info["exec_id"])
-            else:
-                for stage in mlmd_data[0]["stages"]:
-                    for execution in stage["executions"]:
-                        if execution["id"] == int(req_info["exec_id"]):
-                            execution_flag = 1
-                            break
-                if execution_flag == 1:
-                    json_payload = query.dumptojson(pipeline_name, req_info["exec_id"])
-                else:
-                    json_payload = "no_exec_id"
-                    return json_payload
+def get_mlmd_from_server(server_store_path, pipeline_name, exec_id):
+    query = cmfquery.CmfQuery(server_store_path)
+    execution_flag = 0
+    # checks if given execution_id present in mlmd
+    if (
+        pipeline_name in query.get_pipeline_names()
+    ):  # checks if pipeline name is available in mlmd
+        json_payload = query.dumptojson(pipeline_name, None)
+        mlmd_data = json.loads(json_payload)["Pipeline"]
+        if exec_id == None:
+            json_payload = query.dumptojson(pipeline_name, exec_id)
         else:
-            json_payload = "NULL"
+            for stage in mlmd_data[0]["stages"]:
+                for execution in stage["executions"]:
+                    if execution["id"] == int(exec_id):
+                        execution_flag = 1
+                        break
+            if execution_flag == 1:
+                json_payload = query.dumptojson(pipeline_name, exec_id)
+            else:
+                json_payload = "no_exec_id"
+                return json_payload
     else:
-        print("No mlmd file submitted.")
-        json_payload = ""
+        json_payload = "NULL"
     return json_payload
 
-
-# api to display executions available in mlmd
-@app.get("/display_executions/{pipeline_name}", response_class=HTMLResponse)
-async def display_exec(request: Request, pipeline_name: str):
-    # checks if mlmd file exists on server
-
-    if os.path.exists(server_store_path):
-        execution_df = get_executions(server_store_path, pipeline_name)
-        exec_val = "true"
-
-    return templates.TemplateResponse(
-        "execution.html",
-        {"request": request, "exec_df": execution_df, "exec_val": exec_val},
-    )
-
-
-@app.get("/display_lineage/{pipeline_name}", response_class=HTMLResponse)
-async def display_lineage(request: Request, pipeline_name: str):
-    # checks if mlmd file exists on server
-    if os.path.exists(server_store_path):
-        query = cmfquery.CmfQuery(server_store_path)
-        if (pipeline_name in query.get_pipeline_names()):
-            query_visualization(server_store_path, pipeline_name)
-        else:
-            print("Pipeline name " + pipeline_name + " doesn't exist.")
-
-
-    else:
-        print('mlmd doesnt exist')
-    return templates.TemplateResponse(
-        "lineage.html", {"request": request},
-    )
-
-
-# api to display artifacts available in mlmd
-@app.get("/display_artifacts", response_class=HTMLResponse)
-async def display_artifact(request: Request):
-    # checks if mlmd file exists on server
-    if os.path.exists(server_store_path):
-        artifact_df = get_artifacts(server_store_path)
-        artifact_val = "true"
-    else:
-        artifact_val = "false"
-        artifact_df = ""
-    return templates.TemplateResponse(
-        "artifacts.html",
-        {"request": request, "artifact_df": artifact_df, "artifact_val": artifact_val},
-    )
-
-
-@app.get("/display_pipelines/{disp_val}", response_class=HTMLResponse)
-async def display_list_of_pipelines(request: Request,disp_val:str):
-    # checks if mlmd file exists on server
-    if os.path.exists(server_store_path):
-        query = cmfquery.CmfQuery(server_store_path)
-        pipeline_names = query.get_pipeline_names()
-        exec_val = 'True'
-    else:
-        print("No mlmd file submitted.")
-        pipeline_names = []
-        exec_val = "False"
-    return templates.TemplateResponse(
-        "list_of_pipelines.html",
-        {"request": request, "exec_val": exec_val, 'pipeline_names': pipeline_names,'disp_val':disp_val},
-    )
+def get_lineage_img_path(server_store_path,pipeline_name):
+    query = cmfquery.CmfQuery(server_store_path)
+    del_img = glob.glob("./data/static/*.png")
+    for img in del_img:
+        os.remove(img)
+    img_path = query_visualization(server_store_path, pipeline_name)
+    response = FileResponse(img_path,
+    media_type="image/png",)
+    return response
```

### Comparing `cmflib-0.0.3/setup.py` & `cmflib-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Metadata Python Package'
 LONG_DESCRIPTION = 'Metadata framework storing AI metadata into MLMD'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="cmflib",
```

