# Comparing `tmp/fastkafka-0.7.0rc2.tar.gz` & `tmp/fastkafka-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastkafka-0.7.0rc2.tar", last modified: Wed May 31 15:08:03 2023, max compression
+gzip compressed data, was "fastkafka-0.8.0rc0.tar", last modified: Thu Jun 29 13:54:24 2023, max compression
```

## Comparing `fastkafka-0.7.0rc2.tar` & `fastkafka-0.8.0rc0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12621 2023-05-19 13:11:05.000000 fastkafka-0.7.0rc2/CONTRIBUTING.md
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc2/LICENSE
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-03-14 07:16:19.000000 fastkafka-0.7.0rc2/MANIFEST.in
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24678 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    23250 2023-05-31 15:05:16.000000 fastkafka-0.7.0rc2/README.md
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.862865 fastkafka-0.7.0rc2/fastkafka/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/__init__.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.866865 fastkafka-0.7.0rc2/fastkafka/_application/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_application/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    39065 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_application/app.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    17537 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_application/tester.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5622 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli_docs.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_cli_testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_components/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4698 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/_subprocess.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13315 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/aiokafka_consumer_loop.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/asyncapi.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/benchmarking.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/docs_dependencies.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_components/encoder/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/avro.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_components/encoder/json.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/logger.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/meta.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7403 2023-05-31 15:02:33.000000 fastkafka-0.7.0rc2/fastkafka/_components/producer_decorator.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_components/task_streaming.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7992 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_components/test_dependencies.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    20426 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_docusaurus_helper.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51550 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_helpers.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    84393 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_modidx.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     8205 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/_server.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/fastkafka/_testing/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:02:35.000000 fastkafka-0.7.0rc2/fastkafka/_testing/__init__.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    22761 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/apache_kafka_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28873 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/in_memory_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12344 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/local_redpanda_broker.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4979 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/_testing/test_utils.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-05-31 15:02:34.000000 fastkafka-0.7.0rc2/fastkafka/encoder.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/executors.py
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-05-31 15:02:32.000000 fastkafka-0.7.0rc2/fastkafka/testing.py
-drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-05-31 15:08:03.866865 fastkafka-0.7.0rc2/fastkafka.egg-info/
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24678 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/PKG-INFO
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1410 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/SOURCES.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/dependency_links.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/entry_points.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-05-23 12:47:36.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/not-zip-safe
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/requires.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-05-31 15:08:03.000000 fastkafka-0.7.0rc2/fastkafka.egg-info/top_level.txt
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-05-31 14:46:47.000000 fastkafka-0.7.0rc2/settings.ini
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-05-31 15:08:03.870864 fastkafka-0.7.0rc2/setup.cfg
--rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-05-30 11:33:36.000000 fastkafka-0.7.0rc2/setup.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.333007 fastkafka-0.8.0rc0/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    12572 2023-06-29 13:51:03.000000 fastkafka-0.8.0rc0/CONTRIBUTING.md
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11357 2023-06-01 05:47:44.000000 fastkafka-0.8.0rc0/LICENSE
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      111 2023-06-01 05:47:44.000000 fastkafka-0.8.0rc0/MANIFEST.in
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24665 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    23237 2023-06-01 07:29:35.000000 fastkafka-0.8.0rc0/README.md
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      525 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      398 2023-06-29 13:51:30.000000 fastkafka-0.8.0rc0/fastkafka/_aiokafka_imports.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka/_application/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_application/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    40035 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_application/app.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13420 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_application/tester.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2108 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5764 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli_docs.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      996 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_cli_testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_components/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4981 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/_subprocess.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13656 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/aiokafka_consumer_loop.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    18656 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/asyncapi.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     2905 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/benchmarking.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     6991 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/docs_dependencies.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_components/encoder/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13910 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/avro.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1630 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_components/encoder/json.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4136 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     4730 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_components/logger.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    13150 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/meta.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7414 2023-06-29 13:51:32.000000 fastkafka-0.8.0rc0/fastkafka/_components/producer_decorator.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    11998 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_components/task_streaming.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    10312 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_components/test_dependencies.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    25289 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_docusaurus_helper.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    51560 2023-06-29 13:51:34.000000 fastkafka-0.8.0rc0/fastkafka/_helpers.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    87522 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_modidx.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     7313 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/_server.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.329007 fastkafka-0.8.0rc0/fastkafka/_testing/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:51:35.000000 fastkafka-0.8.0rc0/fastkafka/_testing/__init__.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28096 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/apache_kafka_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    28660 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/in_memory_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    14098 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/local_redpanda_broker.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     5428 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/_testing/test_utils.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      598 2023-06-29 13:51:33.000000 fastkafka-0.8.0rc0/fastkafka/encoder.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      454 2023-06-29 13:51:31.000000 fastkafka-0.8.0rc0/fastkafka/executors.py
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      858 2023-06-29 13:51:30.000000 fastkafka-0.8.0rc0/fastkafka/testing.py
+drwxrwxr-x   0 tvrtko    (1000) tvrtko    (1000)        0 2023-06-29 13:54:24.325007 fastkafka-0.8.0rc0/fastkafka.egg-info/
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)    24665 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/PKG-INFO
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1441 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/SOURCES.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/dependency_links.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      146 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/entry_points.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)        1 2023-06-01 08:53:21.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/not-zip-safe
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)      690 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/requires.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       10 2023-06-29 13:54:24.000000 fastkafka-0.8.0rc0/fastkafka.egg-info/top_level.txt
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     1231 2023-06-29 12:08:23.000000 fastkafka-0.8.0rc0/settings.ini
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)       38 2023-06-29 13:54:24.333007 fastkafka-0.8.0rc0/setup.cfg
+-rw-rw-r--   0 tvrtko    (1000) tvrtko    (1000)     3777 2023-06-29 13:51:03.000000 fastkafka-0.8.0rc0/setup.py
```

### Comparing `fastkafka-0.7.0rc2/CONTRIBUTING.md` & `fastkafka-0.8.0rc0/CONTRIBUTING.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Contributing to fastkafka
+# Contributing to FastKafka
 
 First off, thanks for taking the time to contribute! ❤️
 
 All types of contributions are encouraged and valued. See the [Table of Contents](#table-of-contents) for different ways to help and details about how this project handles them. Please make sure to read the relevant section before making your contribution. It will make it a lot easier for us maintainers and smooth out the experience for all involved. The community looks forward to your contributions. 🎉
 
 > And if you like the project, but just don't have time to contribute, that's fine. There are other easy ways to support the project and show your appreciation, which we would also be very happy about:
 > - Star the project
@@ -17,15 +17,14 @@
   - [Reporting Bugs](#reporting-bugs)
   - [Suggesting Enhancements](#suggesting-enhancements)
   - [Your First Code Contribution](#your-first-code-contribution)
 - [Development](#development)
     - [Prepare the dev environment](#prepare-the-dev-environment)
     - [Way of working](#way-of-working)
     - [Before a PR](#before-a-pr)
-- [Join The Project Team](#join-the-project-team)
 
 
 
 ## I Have a Question
 
 > If you want to ask a question, we assume that you have read the available [Documentation](https://fastkafka.airt.ai/docs).
 
@@ -48,15 +47,15 @@
 
 #### Before Submitting a Bug Report
 
 A good bug report shouldn't leave others needing to chase you up for more information. Therefore, we ask you to investigate carefully, collect information and describe the issue in detail in your report. Please complete the following steps in advance to help us fix any potential bug as fast as possible.
 
 - Make sure that you are using the latest version.
 - Determine if your bug is really a bug and not an error on your side e.g. using incompatible environment components/versions (Make sure that you have read the [documentation](https://fastkafka.airt.ai/docs). If you are looking for support, you might want to check [this section](#i-have-a-question)).
-- To see if other users have experienced (and potentially already solved) the same issue you are having, check if there is not already a bug report existing for your bug or error in the [bug tracker](https://github.com/airtai/fastkafkaissues?q=label%3Abug).
+- To see if other users have experienced (and potentially already solved) the same issue you are having, check if there is not already a bug report existing for your bug or error in the [bug tracker](https://github.com/airtai/fastkafka/issues?q=label%3Abug).
 - Also make sure to search the internet (including Stack Overflow) to see if users outside of the GitHub community have discussed the issue.
 - Collect information about the bug:
   - Stack trace (Traceback)
   - OS, Platform and Version (Windows, Linux, macOS, x86, ARM)
   - Python version
   - Possibly your input and the output
   - Can you reliably reproduce the issue? And can you also reproduce it with older versions?
@@ -74,15 +73,15 @@
 
 - The project team will label the issue accordingly.
 - A team member will try to reproduce the issue with your provided steps. If there are no reproduction steps or no obvious way to reproduce the issue, the team will ask you for those steps and mark the issue as `needs-repro`. Bugs with the `needs-repro` tag will not be addressed until they are reproduced.
 - If the team is able to reproduce the issue, it will be marked `needs-fix`, as well as possibly other tags (such as `critical`), and the issue will be left to be implemented.
 
 ### Suggesting Enhancements
 
-This section guides you through submitting an enhancement suggestion for fastkafka, **including completely new features and minor improvements to existing functionality**. Following these guidelines will help maintainers and the community to understand your suggestion and find related suggestions.
+This section guides you through submitting an enhancement suggestion for FastKafka, **including completely new features and minor improvements to existing functionality**. Following these guidelines will help maintainers and the community to understand your suggestion and find related suggestions.
 
 #### Before Submitting an Enhancement
 
 - Make sure that you are using the latest version.
 - Read the [documentation](https://fastkafka.airt.ai/docs) carefully and find out if the functionality is already covered, maybe by an individual configuration.
 - Perform a [search](https://github.com/airtai/fastkafka/issues) to see if the enhancement has already been suggested. If it has, add a comment to the existing issue instead of opening a new one.
 - Find out whether your idea fits with the scope and aims of the project. It's up to you to make a strong case to convince the project's developers of the merits of this feature. Keep in mind that we want features that will be useful to the majority of our users and not just a small subset. If you're just targeting a minority of users, consider writing an add-on/plugin library.
@@ -91,65 +90,65 @@
 #### How Do I Submit a Good Enhancement Suggestion?
 
 Enhancement suggestions are tracked as [GitHub issues](https://github.com/airtai/fastkafka/issues).
 
 - Use a **clear and descriptive title** for the issue to identify the suggestion.
 - Provide a **step-by-step description of the suggested enhancement** in as many details as possible.
 - **Describe the current behavior** and **explain which behavior you expected to see instead** and why. At this point you can also tell which alternatives do not work for you.
-- **Explain why this enhancement would be useful** to most fastkafka users. You may also want to point out the other projects that solved it better and which could serve as inspiration.
+- **Explain why this enhancement would be useful** to most FastKafka users. You may also want to point out the other projects that solved it better and which could serve as inspiration.
 
 ### Your First Code Contribution
 
 A great way to start contributing to FastKafka would be by solving an issue tagged with "good first issue". To find a list of issues that are tagged as "good first issue" and are suitable for newcomers, please visit the following link: [Good first issues](https://github.com/airtai/fastkafka/labels/good%20first%20issue)
 
 These issues are beginner-friendly and provide a great opportunity to get started with contributing to FastKafka. Choose an issue that interests you, follow the contribution process mentioned in [Way of working](#way-of-working) and [Before a PR](#before-a-pr), and help us make FastKafka even better!
 
 If you have any questions or need further assistance, feel free to reach out to us. Happy coding!
 
 ## Development
 
 ### Prepare the dev environment
 
-To start contributing to fastkafka, you first have to prepare the development environment.
+To start contributing to FastKafka, you first have to prepare the development environment.
 
-#### Clone the fastkafka repository
+#### Clone the FastKafka repository
 
 To clone the repository, run the following command in the CLI:
 
 ```shell
 git clone https://github.com/airtai/fastkafka.git
 ```
 
 #### Optional: create a virtual python environment
 
-To prevent library version clashes with you other projects, it is reccomended that you create a virtual python environment for your fastkafka project by running:
+To prevent library version clashes with you other projects, it is reccomended that you create a virtual python environment for your FastKafka project by running:
 
 ```shell
 python3 -m venv fastkafka-env
 ```
 
 And to activate your virtual environment run:
 
 ```shell
 source fastkafka-env/bin/activate
 ```
 
 To learn more about virtual environments, please have a look at [official python documentation](https://docs.python.org/3/library/venv.html#:~:text=A%20virtual%20environment%20is%20created,the%20virtual%20environment%20are%20available.)
 
-#### Install fastkafka
+#### Install FastKafka
 
-To install fastkafka, navigate to the root directory of the cloned fastkafka project and run:
+To install FastKafka, navigate to the root directory of the cloned FastKafka project and run:
 
 ```shell
 pip install fastkafka -e [."dev"]
 ```
 
 #### Install JRE and Kafka toolkit
 
-To be able to run tests and use all the functionalities of fastkafka, you have to have JRE and Kafka toolkit installed on your machine. To do this, you have two options:
+To be able to run tests and use all the functionalities of FastKafka, you have to have JRE and Kafka toolkit installed on your machine. To do this, you have two options:
 
 1. Use our `fastkafka testing install-deps` CLI command which will install JRE and Kafka toolkit for you in your .local folder
 OR
 2. Install JRE and Kafka manually.
    To do this, please refer to [JDK and JRE installation guide](https://docs.oracle.com/javase/9/install/toc.htm) and [Apache Kafka quickstart](https://kafka.apache.org/quickstart)
    
 #### Install npm
@@ -159,41 +158,41 @@
 1. Use our `fastkafka docs install_deps` CLI command which will install npm for you in your .local folder
 OR
 2. Install npm manually.
    To do this, please refer to [NPM installation guide](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm)
    
 #### Install docusaurus
 
-To generate the documentation, you need docusaurus. To install it run 'docusaurus/scripts/install_docusaurus_deps.sh' in the root of fastkafka project.
+To generate the documentation, you need docusaurus. To install it run 'docusaurus/scripts/install_docusaurus_deps.sh' in the root of FastKafka project.
 
 #### Check if everything works
 
-After installing fastkafka and all the necessary dependencies, run `nbdev_test` in the root of fastkafka project. This will take a couple of minutes as it will run all the tests on fastkafka project. If everythng is setup correctly, you will get a "Success." message in your terminal, otherwise please refer to previous steps.
+After installing FastKafka and all the necessary dependencies, run `nbdev_test` in the root of FastKafka project. This will take a couple of minutes as it will run all the tests on FastKafka project. If everythng is setup correctly, you will get a "Success." message in your terminal, otherwise please refer to previous steps.
 
 ### Way of working
 
-The development of fastkafka is done in Jupyter notebooks. Inside the `nbs` directory you will find all the source code of fastkafka, this is where you will implement your changes.
+The development of FastKafka is done in Jupyter notebooks. Inside the `nbs` directory you will find all the source code of FastKafka, this is where you will implement your changes.
 
-The testing, cleanup and exporting of the code is being handled by `nbdev`, please, before starting the work on fastkafka, get familiar with it by reading [nbdev documentation](https://nbdev.fast.ai/getting_started.html).
+The testing, cleanup and exporting of the code is being handled by `nbdev`, please, before starting the work on FastKafka, get familiar with it by reading [nbdev documentation](https://nbdev.fast.ai/getting_started.html).
 
-The general philosopy you should follow when writing code for fastkafka is:
+The general philosopy you should follow when writing code for FastKafka is:
 
 - Function should be an atomic functionality, short and concise
    - Good rule of thumb: your function should be 5-10 lines long usually
 - If there are more than 2 params, enforce keywording using *
    - E.g.: `def function(param1, *, param2, param3): ...`
 - Define typing of arguments and return value
    - If not, mypy tests will fail and a lot of easily avoidable bugs will go undetected
 - After the function cell, write test cells using the assert keyword
    - Whenever you implement something you should test that functionality immediately in the cells below 
 - Add Google style python docstrings when function is implemented and tested
 
 ### Before a PR
 
-After you have implemented your changes you will want to open a pull request to merge those changes into our main branch. To make this as smooth for you and us, please do the following before opening the request (all the commands are to be run in the root of fastkafka project):
+After you have implemented your changes you will want to open a pull request to merge those changes into our main branch. To make this as smooth for you and us, please do the following before opening the request (all the commands are to be run in the root of FastKafka project):
 
 1. Format your notebooks: `nbqa black nbs`
 2. Close, shutdown, and clean the metadata from your notebooks: `nbdev_clean`
 3. Export your code: `nbdev_export`
 4. Run the tests: `nbdev_test`
 5. Test code typing: `mypy fastkafka`
 6. Test code safety with bandit: `bandit -r fastkafka`
```

### Comparing `fastkafka-0.7.0rc2/LICENSE` & `fastkafka-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/PKG-INFO` & `fastkafka-0.8.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.7.0rc2
+Version: 0.8.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -81,15 +81,15 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on macOS, Linux, and most Unix-style operating systems.
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
 To install fastkafka with testing features please use:
@@ -250,15 +250,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
+[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -384,15 +384,17 @@
     return processed_data
 ```
 
 To run the service, use the FastKafka CLI command and pass the module
 (in this case, the file where the app implementation is located) and the
 app simbol to the command.
 
-`shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
+``` sh
+fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app
+```
 
 After running the command, you should see the following output in your
 command line:
 
     [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
     [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
```

### Comparing `fastkafka-0.7.0rc2/README.md` & `fastkafka-0.8.0rc0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on macOS, Linux, and most Unix-style operating systems.
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
 To install fastkafka with testing features please use:
@@ -220,15 +220,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
+[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -354,15 +354,17 @@
     return processed_data
 ```
 
 To run the service, use the FastKafka CLI command and pass the module
 (in this case, the file where the app implementation is located) and the
 app simbol to the command.
 
-`shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
+``` sh
+fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app
+```
 
 After running the command, you should see the following output in your
 command line:
 
     [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
     [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/__init__.py` & `fastkafka-0.8.0rc0/fastkafka/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0rc2"
+__version__ = "0.8.0rc0"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/010_Application_export.ipynb.
 
 # %% auto 0
 __all__ = ['dummy']
 
 # %% ../nbs/010_Application_export.ipynb 1
 from ._application.app import FastKafka
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_application/app.py` & `fastkafka-0.8.0rc0/fastkafka/_application/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from functools import wraps
 from inspect import signature
 from pathlib import Path
 from typing import *
 from unittest.mock import AsyncMock, MagicMock
 
 import anyio
-from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
 from fastkafka._components.aiokafka_consumer_loop import (
     aiokafka_consumer_loop,
     sanitize_kafka_config,
 )
@@ -32,14 +31,17 @@
     ConsumeCallable,
     ContactInfo,
     KafkaBroker,
     KafkaBrokers,
     KafkaServiceInfo,
     export_async_spec,
 )
+
+import fastkafka._aiokafka_imports
+from .._aiokafka_imports import AIOKafkaConsumer, AIOKafkaProducer
 from .._components.benchmarking import _benchmark
 from .._components.logger import get_logger
 from .._components.meta import delegates, export, filter_using_signature, patch
 from .._components.producer_decorator import ProduceCallable, producer_decorator
 from .._components.task_streaming import StreamExecutor
 from .._components.helpers import remove_suffix
 
@@ -47,31 +49,34 @@
 if TYPE_CHECKING:
     from fastapi import FastAPI
 
 # %% ../../nbs/015_FastKafka.ipynb 4
 logger = get_logger(__name__)
 
 # %% ../../nbs/015_FastKafka.ipynb 9
-@delegates(AIOKafkaConsumer, but=["bootstrap_servers_id"])
-@delegates(AIOKafkaProducer, but=["bootstrap_servers_id"], keep=True)
+@delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer, but=["bootstrap_servers"])
+@delegates(
+    fastkafka._aiokafka_imports.AIOKafkaProducer, but=["bootstrap_servers"], keep=True
+)
 def _get_kafka_config(
+    bootstrap_servers_id: str = "localhost",
     **kwargs: Any,
 ) -> Dict[str, Any]:
     """Get kafka config"""
     allowed_keys = set(signature(_get_kafka_config).parameters.keys())
     if not set(kwargs.keys()) <= allowed_keys:
         unallowed_keys = ", ".join(
             sorted([f"'{x}'" for x in set(kwargs.keys()).difference(allowed_keys)])
         )
         raise ValueError(f"Unallowed key arguments passed: {unallowed_keys}")
     retval = kwargs.copy()
 
     # todo: check this values
     config_defaults = {
-        "bootstrap_servers_id": "localhost",
+        "bootstrap_servers_id": bootstrap_servers_id,
         "auto_offset_reset": "earliest",
         "max_poll_records": 100,
     }
     for key, value in config_defaults.items():
         if key not in retval:
             retval[key] = value
 
@@ -189,15 +194,15 @@
                 the title will be set to empty string
             description: optional description for the documentation. If
                 None, the description will be set to empty string
             version: optional version for the documentation. If None,
                 the version will be set to empty string
             contact: optional contact for the documentation. If None, the
                 contact will be set to placeholder values:
-                name='Author' url=HttpUrl(' https://www.google.com ', ) email='noreply@gmail.com'
+                name='Author' url=HttpUrl('https://www.google.com', ) email='noreply@gmail.com'
             kafka_brokers: dictionary describing kafka brokers used for setting
                 the bootstrap server when running the applicationa and for
                 generating documentation. Defaults to
                     {
                         "localhost": {
                             "url": "localhost",
                             "description": "local kafka broker",
@@ -238,18 +243,17 @@
             }
 
         self._kafka_brokers = _get_kafka_brokers(kafka_brokers)
 
         self._override_brokers: List[KafkaBrokers] = []
 
         self._root_path = Path(".") if root_path is None else Path(root_path)
+        self._root_path.mkdir(exist_ok=True, parents=True)
 
         self._asyncapi_path = self._root_path / "asyncapi"
-        (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
-        (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
 
         # this is used as default parameters for creating AIOProducer and AIOConsumer objects
         self._kafka_config = _get_kafka_config(**kwargs)
 
         #
         self._consumers_store: Dict[
             str,
@@ -262,21 +266,21 @@
             ],
         ] = {}
 
         self._producers_store: Dict[  # type: ignore
             str,
             Tuple[
                 ProduceCallable,
-                AIOKafkaProducer,
+                fastkafka._aiokafka_imports.AIOKafkaProducer,
                 Optional[KafkaBrokers],
                 Dict[str, Any],
             ],
         ] = {}
 
-        self._producers_list: List[AIOKafkaProducer] = []  # type: ignore
+        self._producers_list: List[fastkafka._aiokafka_imports.AIOKafkaProducer] = []  # type: ignore
 
         self.benchmark_results: Dict[str, Dict[str, Any]] = {}
 
         # background tasks
         self._scheduled_bg_tasks: List[Callable[..., Coroutine[Any, Any, Any]]] = []
         self._bg_task_group_generator: Optional[anyio.abc.TaskGroup] = None
         self._bg_tasks_group: Optional[anyio.abc.TaskGroup] = None
@@ -297,14 +301,24 @@
         # testing functions
         self.AppMocks = None
         self.mocks = None
         self.awaited_mocks = None
 
     @property
     def is_started(self) -> bool:
+        """Property indicating whether the FastKafka object is started.
+
+        The is_started property indicates if the FastKafka object is currently
+        in a started state. This implies that all background tasks, producers,
+        and consumers have been initiated, and the object is successfully connected
+        to the Kafka broker.
+
+        Returns:
+            bool: True if the object is started, False otherwise.
+        """
         return self._is_started
 
     def set_kafka_broker(self, kafka_broker_name: str) -> None:
         """
         Sets the Kafka broker to start FastKafka with
 
         Args:
@@ -454,15 +468,15 @@
     while resolved_key in dictionary:
         i += 1
         resolved_key = f"{key}_{i}"
     return resolved_key
 
 # %% ../../nbs/015_FastKafka.ipynb 31
 @patch
-@delegates(AIOKafkaConsumer)
+@delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer)
 def consumes(
     self: FastKafka,
     topic: Optional[str] = None,
     decoder: Union[str, Callable[[bytes, ModelMetaclass], Any]] = "json",
     *,
     executor: Union[str, StreamExecutor, None] = None,
     brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None,
@@ -562,15 +576,15 @@
             )
         return avro_encoder
     else:
         raise ValueError(f"Unknown encoder - {encoder}")
 
 # %% ../../nbs/015_FastKafka.ipynb 36
 @patch
-@delegates(AIOKafkaProducer)
+@delegates(fastkafka._aiokafka_imports.AIOKafkaProducer)
 def produces(
     self: FastKafka,
     topic: Optional[str] = None,
     encoder: Union[str, Callable[[BaseModel], bytes]] = "json",
     *,
     prefix: str = "to_",
     brokers: Optional[Union[Dict[str, Any], KafkaBrokers]] = None,
@@ -699,15 +713,15 @@
 # %% ../../nbs/015_FastKafka.ipynb 45
 @patch
 def _populate_consumers(
     self: FastKafka,
     is_shutting_down_f: Callable[[], bool],
 ) -> None:
     default_config: Dict[str, Any] = filter_using_signature(
-        AIOKafkaConsumer, **self._kafka_config
+        fastkafka._aiokafka_imports.AIOKafkaConsumer, **self._kafka_config
     )
 
     bootstrap_server = self._kafka_config["bootstrap_servers_id"]
 
     self._kafka_consumer_tasks = [
         asyncio.create_task(
             aiokafka_consumer_loop(
@@ -751,16 +765,16 @@
 # TODO: Add passing of vars
 async def _create_producer(  # type: ignore
     *,
     callback: ProduceCallable,
     default_config: Dict[str, Any],
     override_config: Dict[str, Any],
     bootstrap_servers: Union[str, List[str]],
-    producers_list: List[AIOKafkaProducer],
-) -> AIOKafkaProducer:
+    producers_list: List[fastkafka._aiokafka_imports.AIOKafkaProducer],
+) -> fastkafka._aiokafka_imports.AIOKafkaProducer:
     """Creates a producer
 
     Args:
         callback: A callback function that is called when the producer is ready.
         producer: An existing producer to use.
         default_config: A dictionary of default configuration values.
         override_config: A dictionary of configuration values to override.
@@ -768,20 +782,24 @@
         producers_list: A list of producers to add the new producer to.
 
     Returns:
         A producer.
     """
 
     config = {
-        **filter_using_signature(AIOKafkaProducer, **default_config),
-        **filter_using_signature(AIOKafkaProducer, **override_config),
+        **filter_using_signature(
+            fastkafka._aiokafka_imports.AIOKafkaProducer, **default_config
+        ),
+        **filter_using_signature(
+            fastkafka._aiokafka_imports.AIOKafkaProducer, **override_config
+        ),
         **{"bootstrap_servers": bootstrap_servers},
     }
 
-    producer = AIOKafkaProducer(**config)
+    producer = fastkafka._aiokafka_imports.AIOKafkaProducer(**config)
     logger.info(
         f"_create_producer() : created producer using the config: '{sanitize_kafka_config(**config)}'"
     )
 
     await producer.start()
 
     producers_list.append(producer)
@@ -930,14 +948,16 @@
     Note:
         The asyncapi documentation is saved to the location specified by the `_asyncapi_path`
         attribute of the FastKafka instance.
 
     Returns:
         None
     """
+    (self._asyncapi_path / "docs").mkdir(exist_ok=True, parents=True)
+    (self._asyncapi_path / "spec").mkdir(exist_ok=True, parents=True)
     export_async_spec(
         consumers={
             remove_suffix(topic) if topic.endswith("_0") else topic: callback
             for topic, (callback, _, _, _, _) in self._consumers_store.items()
         },
         producers={
             remove_suffix(topic) if topic.endswith("_0") else topic: callback
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_application/tester.py` & `fastkafka-0.8.0rc0/fastkafka/_application/tester.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import collections
 import inspect
 from unittest.mock import AsyncMock, MagicMock
 import json
 from contextlib import asynccontextmanager
 from itertools import groupby
 from typing import *
+from types import ModuleType
 
 from pydantic import BaseModel
 
 from .. import KafkaEvent
 from .app import FastKafka, AwaitedMock, _get_kafka_brokers
 from .._components.asyncapi import KafkaBroker, KafkaBrokers
 from .._components.helpers import unwrap_list_type
@@ -43,24 +44,22 @@
     return KafkaBroker(url=url, port=port, description="", protocol="")
 
 # %% ../../nbs/016_Tester.ipynb 9
 @export("fastkafka.testing")
 class Tester(FastKafka):
     __test__ = False
 
-    @delegates(ApacheKafkaBroker.__init__)
     def __init__(
         self,
         app: Union[FastKafka, List[FastKafka]],
         *,
-        broker: Optional[
-            Union[ApacheKafkaBroker, LocalRedpandaBroker, InMemoryBroker]
-        ] = None,
+        use_in_memory_broker: bool = True,
+        patch_module: Optional[ModuleType] = None,
     ):
-        """Mirror-like object for testing a FastFafka application
+        """Mirror-like object for testing a FastKafka application
 
         Can be used as context manager
 
         Args:
             app: The FastKafka application to be tested.
             broker: An optional broker to start and to use for testing.
         """
@@ -68,80 +67,20 @@
 
         for app in self.apps:
             app.create_mocks()
 
         super().__init__()
         self.mirrors: Dict[Any, Any] = {}
         self._kafka_brokers = self.apps[0]._kafka_brokers
-        self._create_mirrors()
-        self.broker = broker
-        unique_broker_configs = []
-        for app in self.apps:
-            for broker_config in app._override_brokers:
-                if broker_config not in unique_broker_configs:
-                    unique_broker_configs.append(broker_config)
-        self.num_brokers = len(unique_broker_configs)
-
-        self.overriden_brokers: List[Union[ApacheKafkaBroker, LocalRedpandaBroker]] = []
-
-    @delegates(LocalRedpandaBroker.__init__)
-    def using_local_redpanda(self, **kwargs: Any) -> "Tester":
-        """Starts local Redpanda broker used by the Tester instance
-
-        Args:
-            listener_port: Port on which the clients (producers and consumers) can connect
-            tag: Tag of Redpanda image to use to start container
-            seastar_core: Core(s) to use byt Seastar (the framework Redpanda uses under the hood)
-            memory: The amount of memory to make available to Redpanda
-            mode: Mode to use to load configuration properties in container
-            default_log_level: Log levels to use for Redpanda
-            topics: List of topics to create after successful redpanda broker startup
-            retries: Number of retries to create redpanda service
-            apply_nest_asyncio: set to True if running in notebook
-            port allocation if the requested port was taken
-
-        Returns:
-            An instance of tester with Redpanda as broker
-        """
-        topics = set().union(*(app.get_topics() for app in self.apps))
-        kwargs["topics"] = (
-            topics.union(kwargs["topics"]) if "topics" in kwargs else topics
-        )
-        self.broker = LocalRedpandaBroker(**kwargs)
-        self.overriden_brokers = [
-            LocalRedpandaBroker(**kwargs) for _ in range(self.num_brokers)
-        ]
-        return self
-
-    @delegates(ApacheKafkaBroker.__init__)
-    def using_local_kafka(self, **kwargs: Any) -> "Tester":
-        """Starts local Kafka broker used by the Tester instance
-
-        Args:
-            data_dir: Path to the directory where the zookeeper instance will save data
-            zookeeper_port: Port for clients (Kafka brokers) to connect
-            listener_port: Port on which the clients (producers and consumers) can connect
-            topics: List of topics to create after successful Kafka broker startup
-            retries: Number of retries to create Kafka and zookeeper services using random
-            apply_nest_asyncio: set to True if running in notebook
-            port allocation if the requested port was taken
-
-        Returns:
-            An instance of tester with Kafka as broker
-        """
-        topics = set().union(*(app.get_topics() for app in self.apps))
-        kwargs["topics"] = (
-            topics.union(kwargs["topics"]) if "topics" in kwargs else topics
-        )
-        self.broker = ApacheKafkaBroker(**kwargs)
-        self.overriden_brokers = [
-            ApacheKafkaBroker(**kwargs) for _ in range(self.num_brokers)
+        self._kafka_config["bootstrap_servers_id"] = self.apps[0]._kafka_config[
+            "bootstrap_servers_id"
         ]
-
-        return self
+        self._create_mirrors()
+        self.use_in_memory_broker = use_in_memory_broker
+        self.patch_module = patch_module
 
     async def _start_tester(self) -> None:
         """Starts the Tester"""
         for app in self.apps:
             await app.__aenter__()
         self.create_mocks()
         self._arrange_mirrors()
@@ -158,65 +97,36 @@
         pass
 
     def _arrange_mirrors(self) -> None:
         pass
 
     @asynccontextmanager
     async def _create_ctx(self) -> AsyncGenerator["Tester", None]:
-        if self.broker is None:
-            topics = set().union(*(app.get_topics() for app in self.apps))
-            self.broker = InMemoryBroker()
-
-        broker_spec = _get_broker_spec(await self.broker._start())
-
-        try:
-            if isinstance(self.broker, (ApacheKafkaBroker, LocalRedpandaBroker)):
-                override_broker_configs = [
-                    list(grp)
-                    for k, grp in groupby(
-                        [
-                            broker_config
-                            for app in self.apps + [self]
-                            for broker_config in app._override_brokers
-                        ]
-                    )
-                ]
-
-                for override_brokers_config_groups, broker in zip(
-                    override_broker_configs, self.overriden_brokers
-                ):
-                    b_s = _get_broker_spec(await broker._start())
-                    for override_broker_config in override_brokers_config_groups:
-                        override_broker_config["fastkafka_tester_broker"] = b_s  # type: ignore
-
-                for app in self.apps + [self]:
-                    app._kafka_brokers.brokers["fastkafka_tester_broker"] = broker_spec
-                    app.set_kafka_broker("fastkafka_tester_broker")
-
-            else:
-                for app in self.apps + [self]:
-                    app.set_kafka_broker(list(self._kafka_brokers.brokers.keys())[0])
+        if self.use_in_memory_broker == True:
+            with InMemoryBroker(patch_module=self.patch_module):  # type: ignore
+                await self._start_tester()
+                try:
+                    yield self
+                finally:
+                    await self._stop_tester()
+        else:
             await self._start_tester()
             try:
                 yield self
             finally:
                 await self._stop_tester()
-        finally:
-            await self.broker._stop()
-            for broker in self.overriden_brokers:
-                await broker._stop()
 
     async def __aenter__(self) -> "Tester":
         self._ctx = self._create_ctx()
         return await self._ctx.__aenter__()
 
     async def __aexit__(self, *args: Any) -> None:
         await self._ctx.__aexit__(*args)
 
-# %% ../../nbs/016_Tester.ipynb 19
+# %% ../../nbs/016_Tester.ipynb 16
 def mirror_producer(
     topic: str, producer_f: Callable[..., Any], brokers: str, app: FastKafka
 ) -> Callable[..., Any]:
     """
     Decorator to create a mirrored producer function.
 
     Args:
@@ -253,15 +163,15 @@
         ]
     )
 
     mirror_func.__signature__ = sig  # type: ignore
 
     return mirror_func
 
-# %% ../../nbs/016_Tester.ipynb 22
+# %% ../../nbs/016_Tester.ipynb 19
 def mirror_consumer(
     topic: str, consumer_f: Callable[..., Any], brokers: str, app: FastKafka
 ) -> Callable[[BaseModel], Coroutine[Any, Any, BaseModel]]:
     """
     Decorator to create a mirrored consumer function.
 
     Args:
@@ -291,15 +201,15 @@
     sig = sig.replace(
         parameters=[msg_type], return_annotation=msg_type_unwrapped.annotation
     )
 
     mirror_func.__signature__ = sig  # type: ignore
     return mirror_func
 
-# %% ../../nbs/016_Tester.ipynb 24
+# %% ../../nbs/016_Tester.ipynb 21
 @patch
 def _create_mirrors(self: Tester) -> None:
     """
     Creates mirror functions for producers and consumers.
 
     Iterates over the FastKafka application and its producers and consumers. For each consumer, it creates a mirror
     consumer function using the `mirror_consumer` decorator. For each producer, it creates a mirror producer function
@@ -335,15 +245,15 @@
                 brokers=brokers,
             )(
                 mirror_f  # type: ignore
             )
             self.mirrors[producer_f] = mirror_f
             setattr(self, mirror_f.__name__, mirror_f)
 
-# %% ../../nbs/016_Tester.ipynb 29
+# %% ../../nbs/016_Tester.ipynb 25
 class AmbiguousWarning:
     """
     Warning class used for ambiguous topics.
 
     Args:
         topic: The ambiguous topic.
         functions: List of function names associated with the ambiguous topic.
@@ -359,15 +269,15 @@
         )
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         raise RuntimeError(
             f"Ambiguous topic: {self.topic}, for functions: {self.functions}\nUse Tester.mirrors[app.function] to resolve ambiguity"
         )
 
-# %% ../../nbs/016_Tester.ipynb 31
+# %% ../../nbs/016_Tester.ipynb 27
 def set_sugar(
     *,
     tester: Tester,
     prefix: str,
     topic_brokers: Dict[str, Tuple[List[str], List[str]]],
     topic: str,
     brokers: str,
@@ -397,15 +307,15 @@
     if len(brokers_for_topic) == 1:
         setattr(tester, f"{prefix}{topic}", function)
     else:
         setattr(
             tester, f"{prefix}{topic}", AmbiguousWarning(topic, functions_for_topic)
         )
 
-# %% ../../nbs/016_Tester.ipynb 32
+# %% ../../nbs/016_Tester.ipynb 28
 @patch
 def _arrange_mirrors(self: Tester) -> None:
     """
     Arranges the mirror functions.
 
     Iterates over the FastKafka application and its producers and consumers. For each consumer, it retrieves the mirror
     function from the `self.mirrors` dictionary and sets it as an attribute on the Tester instance. It also sets the
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_cli.py` & `fastkafka-0.8.0rc0/fastkafka/_cli.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_cli_docs.py` & `fastkafka-0.8.0rc0/fastkafka/_cli_docs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/024_CLI_Docs.ipynb.
 
 # %% auto 0
 __all__ = ['logger', 'docs_install_deps', 'generate_docs', 'serve_docs']
 
 # %% ../nbs/024_CLI_Docs.ipynb 1
 import asyncio
+import platform
 import signal
 import socketserver
 from http.server import SimpleHTTPRequestHandler
 from pathlib import Path
 from types import FrameType
 from typing import *
 
@@ -22,15 +23,15 @@
 from ._components.helpers import _import_from_string, change_dir
 from ._components.logger import get_logger
 
 # %% ../nbs/024_CLI_Docs.ipynb 5
 logger = get_logger(__name__)
 
 # %% ../nbs/024_CLI_Docs.ipynb 8
-_docs_app = typer.Typer(help="Commands for managing fastkafka app documentation")
+_docs_app = typer.Typer(help="Commands for managing FastKafka app documentation")
 
 # %% ../nbs/024_CLI_Docs.ipynb 9
 @_docs_app.command(
     "install_deps",
     help="Installs dependencies for FastKafka documentation generation",
 )
 def docs_install_deps() -> None:
@@ -142,14 +143,16 @@
             def sigint_handler(
                 signal: int, frame: Optional[FrameType], d: Dict[str, bool] = d
             ) -> None:
                 d["should_stop"] = True
 
             signal.signal(signal.SIGINT, sigint_handler)
             signal.signal(signal.SIGTERM, sigint_handler)
+            if platform.system() == "Windows":
+                signal.signal(signal.SIGBREAK, sigint_handler)  # type: ignore
 
             with socketserver.TCPServer(server_address, handler) as httpd:
                 httpd.timeout = 0.1
                 typer.secho(
                     f"Serving documentation on http://{server_address[0]}:{server_address[1]}"
                 )
                 while not d["should_stop"]:
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_cli_testing.py` & `fastkafka-0.8.0rc0/fastkafka/_cli_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ._components.logger import get_logger
 from ._components.test_dependencies import _install_testing_deps
 
 # %% ../nbs/025_CLI_Testing.ipynb 5
 logger = get_logger(__name__)
 
 # %% ../nbs/025_CLI_Testing.ipynb 8
-_testing_app = typer.Typer(help="Commands for managing fastkafka testing")
+_testing_app = typer.Typer(help="Commands for managing FastKafka testing")
 
 # %% ../nbs/025_CLI_Testing.ipynb 9
 @_testing_app.command(
     "install_deps",
     help="Installs dependencies for FastKafka app testing",
 )
 def testing_install_deps() -> None:
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/_subprocess.py` & `fastkafka-0.8.0rc0/fastkafka/_components/_subprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,18 +40,22 @@
     except asyncio.TimeoutError:
         pass
 
     for i in range(3):
         if platform.system() == "Windows":
             import psutil
 
-            parent = psutil.Process(p.pid)
-            children = parent.children(recursive=True)
-            for child in children:
-                child.kill()
+            try:
+                parent = psutil.Process(p.pid)
+                children = parent.children(recursive=True)
+                for child in children:
+                    child.kill()
+                p.send_signal(signal.CTRL_BREAK_EVENT)  # type: ignore
+            except psutil.NoSuchProcess:
+                pass
         else:
             p.terminate()
         try:
             await asyncio.wait_for(p.wait(), 10)
             logger.info(f"terminate_asyncio_process(): Process {p.pid} terminated.")
             return
         except asyncio.TimeoutError:
@@ -81,14 +85,16 @@
     """
     loop = asyncio.get_event_loop()
 
     HANDLED_SIGNALS = (
         signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
         signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
     )
+    if platform.system() == "Windows":
+        HANDLED_SIGNALS = (*HANDLED_SIGNALS, signal.SIGBREAK)  # type: ignore
 
     d = {"should_exit": False}
 
     def handle_windows_exit(
         signum: int, frame: Optional[FrameType], d: Dict[str, bool] = d
     ) -> None:
         d["should_exit"] = True
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/aiokafka_consumer_loop.py` & `fastkafka-0.8.0rc0/fastkafka/_components/aiokafka_consumer_loop.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 1
 from asyncio import iscoroutinefunction, Task  # do not use the version from inspect
 from typing import *
 from dataclasses import dataclass
 
 import asyncer
-from aiokafka import AIOKafkaConsumer
 from aiokafka.structs import ConsumerRecord
 from pydantic import BaseModel
 from pydantic.main import ModelMetaclass
 
+import fastkafka._aiokafka_imports
 from .logger import get_logger
 from .meta import delegates, export
 from .task_streaming import get_executor, StreamExecutor
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 5
 logger = get_logger(__name__)
 
@@ -137,30 +137,33 @@
         callback if iscoroutinefunction(callback) else asyncer.asyncify(callback)  # type: ignore
     )
     return _callback_parameters_wrapper(async_callback)
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 24
 def _get_single_msg_handlers(  # type: ignore
     *,
-    consumer: AIOKafkaConsumer,
+    consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     callback: AsyncConsumeMeta,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     msg_type: Type[BaseModel],
     **kwargs: Any,
 ) -> Tuple[
     Callable[
         [
             ConsumerRecord,
             AsyncConsumeMeta,
             Callable[[bytes, ModelMetaclass], Any],
             Type[BaseModel],
         ],
         Awaitable[None],
     ],
-    Callable[[AIOKafkaConsumer, Any], Awaitable[List[ConsumerRecord]]],
+    Callable[
+        [fastkafka._aiokafka_imports.AIOKafkaConsumer, Any],
+        Awaitable[List[ConsumerRecord]],
+    ],
 ]:
     """
     Retrieves the message handlers for consuming single messages from a Kafka topic.
 
     Args:
         consumer: The Kafka consumer instance.
         callback: The callback function to handle the consumed message.
@@ -180,40 +183,44 @@
     ) -> None:
         await callback(
             decoder_fn(record.value, msg_type),
             EventMetadata.create_event_metadata(record),
         )
 
     async def poll_consumer(  # type: ignore
-        consumer: AIOKafkaConsumer = consumer, kwargs: Any = kwargs
+        consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer = consumer,
+        kwargs: Any = kwargs,
     ) -> List[ConsumerRecord]:
         msgs = await consumer.getmany(**kwargs)
         return [msg for msg_group in msgs.values() for msg in msg_group]
 
     return handle_msg, poll_consumer
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 26
 def _get_batch_msg_handlers(  # type: ignore
     *,
-    consumer: AIOKafkaConsumer,
+    consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     callback: AsyncConsumeMeta,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     msg_type: Type[BaseModel],
     **kwargs: Any,
 ) -> Tuple[
     Callable[
         [
             List[ConsumerRecord],
             AsyncConsumeMeta,
             Callable[[bytes, ModelMetaclass], Any],
             Type[BaseModel],
         ],
         Awaitable[None],
     ],
-    Callable[[AIOKafkaConsumer, Any], Awaitable[List[List[ConsumerRecord]]]],
+    Callable[
+        [fastkafka._aiokafka_imports.AIOKafkaConsumer, Any],
+        Awaitable[List[List[ConsumerRecord]]],
+    ],
 ]:
     """
     Retrieves the message handlers for consuming messages in batches from a Kafka topic.
 
     Args:
         consumer: The Kafka consumer instance.
         callback: The callback function to handle the consumed messages.
@@ -233,25 +240,26 @@
     ) -> None:
         await callback(
             [decoder_fn(record.value, msg_type) for record in records],
             [EventMetadata.create_event_metadata(record) for record in records],
         )
 
     async def poll_consumer(  # type: ignore
-        consumer: AIOKafkaConsumer = consumer, kwargs: Any = kwargs
+        consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer = consumer,
+        kwargs: Any = kwargs,
     ) -> List[List[ConsumerRecord]]:
         msgs = await consumer.getmany(**kwargs)
         return [value for value in msgs.values() if len(value) > 0]
 
     return handle_msg, poll_consumer
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 28
-@delegates(AIOKafkaConsumer.getmany)
+@delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer.getmany)
 async def _aiokafka_consumer_loop(  # type: ignore
-    consumer: AIOKafkaConsumer,
+    consumer: fastkafka._aiokafka_imports.AIOKafkaConsumer,
     *,
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     callback: ConsumeCallable,
     max_buffer_size: int = 100_000,
     msg_type: Union[Type[List[BaseModel]], Type[BaseModel]],
     is_shutting_down_f: Callable[[], bool],
@@ -299,15 +307,15 @@
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 35
 def sanitize_kafka_config(**kwargs: Any) -> Dict[str, Any]:
     """Sanitize Kafka config"""
     return {k: "*" * len(v) if "pass" in k.lower() else v for k, v in kwargs.items()}
 
 # %% ../../nbs/011_ConsumerLoop.ipynb 37
-@delegates(AIOKafkaConsumer)
+@delegates(fastkafka._aiokafka_imports.AIOKafkaConsumer)
 @delegates(_aiokafka_consumer_loop, keep=True)
 async def aiokafka_consumer_loop(
     topic: str,
     decoder_fn: Callable[[bytes, ModelMetaclass], Any],
     *,
     timeout_ms: int = 100,
     max_buffer_size: int = 100_000,
@@ -327,15 +335,15 @@
         timeout_ms: Time to timeut the getmany request by the consumer
         max_buffer_size: Maximum number of unconsumed messages in the callback buffer
         msg_type: Type with `parse_json` method used for parsing a decoded message
         is_shutting_down_f: Function for controlling the shutdown of consumer loop
     """
     logger.info(f"aiokafka_consumer_loop() starting...")
     try:
-        consumer = AIOKafkaConsumer(
+        consumer = fastkafka._aiokafka_imports.AIOKafkaConsumer(
             **kwargs,
         )
         logger.info(
             f"aiokafka_consumer_loop(): Consumer created using the following parameters: {sanitize_kafka_config(**kwargs)}"
         )
 
         await consumer.start()
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/asyncapi.py` & `fastkafka-0.8.0rc0/fastkafka/_components/asyncapi.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/benchmarking.py` & `fastkafka-0.8.0rc0/fastkafka/_components/benchmarking.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/docs_dependencies.py` & `fastkafka-0.8.0rc0/fastkafka/_components/docs_dependencies.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/encoder/avro.py` & `fastkafka-0.8.0rc0/fastkafka/_components/encoder/avro.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/encoder/json.py` & `fastkafka-0.8.0rc0/fastkafka/_components/encoder/json.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/helpers.py` & `fastkafka-0.8.0rc0/fastkafka/_components/helpers.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/logger.py` & `fastkafka-0.8.0rc0/fastkafka/_components/logger.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/meta.py` & `fastkafka-0.8.0rc0/fastkafka/_components/meta.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/producer_decorator.py` & `fastkafka-0.8.0rc0/fastkafka/_components/producer_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import random
 import time
 from asyncio import iscoroutinefunction  # do not use the version from inspect
 from dataclasses import dataclass
 from inspect import Parameter
 from typing import *
 
-from aiokafka import AIOKafkaProducer
 from aiokafka.producer.message_accumulator import BatchBuilder
 from pydantic import BaseModel
 
+from .._aiokafka_imports import AIOKafkaProducer
 from .meta import export
 from .helpers import remove_suffix
 
 # %% ../../nbs/013_ProducerDecorator.ipynb 3
 BaseSubmodel = TypeVar("BaseSubmodel", bound=Union[List[BaseModel], BaseModel])
 BaseSubmodel
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_components/task_streaming.py` & `fastkafka-0.8.0rc0/fastkafka/_components/task_streaming.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/_docusaurus_helper.py` & `fastkafka-0.8.0rc0/fastkafka/_docusaurus_helper.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/096_Docusaurus_Helper.ipynb.
 
 # %% auto 0
-__all__ = ['fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar',
+__all__ = ['CustomNbdevLookup', 'fix_invalid_syntax_in_markdown', 'generate_markdown_docs', 'generate_sidebar',
            'delete_unused_markdown_files_from_sidebar']
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 2
 import itertools
 import re
 import ast
 import types
-from inspect import Signature, getmembers, isclass, isfunction, signature
+from inspect import (
+    Signature,
+    getmembers,
+    isclass,
+    isfunction,
+    signature,
+    ismethod,
+    getsource,
+)
 from pathlib import Path
 from typing import *
 from urllib.parse import urljoin
+from functools import lru_cache
 
 import typer
 from docstring_parser import parse
 from docstring_parser.common import DocstringParam, DocstringRaises, DocstringReturns
 from nbdev.config import get_config
+from nbdev.doclinks import NbdevLookup, patch_name, L, _find_mod
 from nbdev_mkdocs.mkdocs import (
     _add_all_submodules,
     _import_all_members,
     _import_functions_and_classes,
     _import_submodules,
 )
 
@@ -40,23 +50,39 @@
         The formatted docstring.
     """
     formatted_docstring = ""
     if len(items) > 0:
         formatted_docstring += f"**{keyword}**:\n"
         for item in items:
             if keyword == "Parameters":
-                formatted_docstring += f"- `{item.arg_name}`: {item.description}\n"  # type: ignore
+                formatted_docstring += f"- **{item.arg_name}**: {item.description}\n"  # type: ignore
             elif keyword == "Exceptions":
-                formatted_docstring += f"- `{item.type_name}`: {item.description}\n"
+                formatted_docstring += f"- **{item.type_name}**: {item.description}\n"
             else:
                 formatted_docstring += f"- {item.description}\n"
         formatted_docstring = f"{formatted_docstring}\n"
     return formatted_docstring
 
 # %% ../nbs/096_Docusaurus_Helper.ipynb 8
+def _format_free_links(s: str) -> str:
+    """Format free links in a given string by adding proper spacing around them.
+
+    Args:
+        s: The input string containing free links.
+
+    Returns:
+        The modified string with properly formatted free links.
+    """
+    pattern = r"([\"'])(https?:\/\/[^\s]+)([\"'])"
+    ret_val = re.sub(
+        pattern, lambda match: f"{match.group(1)} {match.group(2)} {match.group(3)}", s
+    )
+    return ret_val
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 10
 def _docstring_to_markdown(docstring: str) -> str:
     """Converts a docstring to a markdown-formatted string.
 
     Args:
         docstring: The docstring to convert.
 
     Returns:
@@ -75,17 +101,19 @@
     formatted_docstring += _format_docstring_sections(
         parsed_docstring.many_returns, "Returns"
     )
     formatted_docstring += _format_docstring_sections(
         parsed_docstring.raises, "Exceptions"
     )
 
-    return formatted_docstring
+    ret_val = _format_free_links(formatted_docstring)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 12
+    return ret_val
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 14
 def _get_submodules(module_name: str) -> List[str]:
     """Get a list of all submodules contained within the module.
 
     Args:
         module_name: The name of the module to retrieve submodules from
 
     Returns:
@@ -94,15 +122,15 @@
     members = _import_all_members(module_name)
     members_with_submodules = _add_all_submodules(members)
     members_with_submodules_str: List[str] = [
         x[:-1] if x.endswith(".") else x for x in members_with_submodules
     ]
     return members_with_submodules_str
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 14
+# %% ../nbs/096_Docusaurus_Helper.ipynb 16
 def _load_submodules(
     module_name: str, members_with_submodules: List[str]
 ) -> List[Union[types.FunctionType, Type[Any]]]:
     """Load the given submodules from the module.
 
     Args:
         module_name: The name of the module whose submodules to load
@@ -118,123 +146,242 @@
     names = [
         y
         for x, y in members
         if f"{y.__module__}.{y.__name__}" in members_with_submodules
     ]
     return names
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 16
-def _convert_union_to_optional(annotation_str: str) -> str:
-    """Convert the 'Union[Type1, Type2, ..., NoneType]' to 'Optional[Type1, Type2, ...]' in the given annotation string
+# %% ../nbs/096_Docusaurus_Helper.ipynb 18
+def _get_parameters(_signature: Signature) -> List[str]:
+    """Convert a function's signature into a string representation of its parameter list.
+
+    Args:
+        _signature: The signature object representing the function's signature.
+
+    Returns:
+        A list of strings representing the function's parameters, including their default values if applicable.
+    """
+    params = [param for param in _signature.parameters.values()]
+    ret_val = [
+        f"{param.name}"
+        if (param.default is param.empty)
+        else f"{param.name}='{param.default}'"
+        if isinstance(param.default, str)
+        else f"{param.name}={param.default}"
+        for param in params
+    ]
+    return ret_val
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 22
+def _format_symbol_definition(
+    symbol: Union[types.FunctionType, Type[Any]], params_list: List[str]
+) -> str:
+    """Format the given symbol parameters by adding a new line and indentation.
 
     Args:
-        annotation_str: The type annotation string to convert.
+        params_list: A string representation of the parameter list.
 
     Returns:
-        The converted type annotation string.
+        A formatted string representation of the parameters with new lines and indentation.
     """
-    pattern = r"Union\[(.*)?,\s*NoneType\s*\]"
-    match = re.search(pattern, annotation_str)
-    if match:
-        union_type = match.group(1)
-        optional_type = f"Optional[{union_type}]"
-        return re.sub(pattern, optional_type, annotation_str)
+    parameters = ", ".join(params_list)
+    if parameters == "":
+        return f"{symbol.__name__}()\n"
+    elif len(f"{symbol.__name__}({parameters})") <= 79:
+        return f"{symbol.__name__}(\n    {parameters}\n)\n"
     else:
-        return annotation_str
+        formatted_parameters = "".join([f"\n    {param}," for param in params_list])
+        return f"{symbol.__name__}({formatted_parameters}\n)\n"
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 18
-def _get_arg_list_with_signature(_signature: Signature) -> str:
-    """Converts a function's signature into a string representation of its argument list.
+# %% ../nbs/096_Docusaurus_Helper.ipynb 29
+def _get_exps(mod: str) -> Dict[str, str]:
+    mf = _find_mod(mod)
+    if not mf:
+        return {}
+    txt = mf.read_text()
+    _def_types = ast.FunctionDef, ast.AsyncFunctionDef, ast.ClassDef
+    d = {}
+    for tree in ast.parse(txt).body:
+        if isinstance(tree, _def_types):
+            for t in L(patch_name(tree)):
+                d[t] = f"{tree.lineno}-L{tree.end_lineno}"
+        if isinstance(tree, ast.ClassDef):
+            d.update(
+                {
+                    tree.name + "." + t2.name: f"{t2.lineno}-L{t2.end_lineno}"
+                    for t2 in tree.body
+                    if isinstance(t2, _def_types)
+                }
+            )
+    return d
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 31
+def _lineno(sym: str, fname: str) -> Optional[str]:
+    return _get_exps(fname).get(sym, None) if fname else None
+
+
+@lru_cache(None)
+class CustomNbdevLookup(NbdevLookup.__wrapped__):  # type: ignore
+    def __init__(
+        self,
+        strip_libs: Optional[str] = None,
+        incl_libs: Optional[str] = None,
+        skip_mods: Optional[str] = None,
+    ):
+        super().__init__(strip_libs, incl_libs, skip_mods)
+
+    def code(self, sym: str) -> Optional[str]:
+        "Link to source code for `sym`"
+        res = self[sym]
+        if not isinstance(res, tuple):
+            return None
+        _, py, gh = res
+        line = _lineno(sym, py)
+        return f"{gh}#L{line}"
+
+# %% ../nbs/096_Docusaurus_Helper.ipynb 34
+def _get_symbol_source_link(
+    symbol: Union[types.FunctionType, Type[Any]], lib_version: str
+) -> str:
+    """Returns the source code link for a given symbol.
 
     Args:
-        _signature (signature): The signature object for the function to convert.
+        symbol: The symbol to get the source code link for.
+        lib_version: The current version of the library.
 
     Returns:
-        str: A string representation of the function's argument list.
+        The source code link for the symbol.
     """
-    arg_list = []
-    for param in _signature.parameters.values():
-        arg_list.append(_convert_union_to_optional(str(param)))
+    symbol = symbol.fget if isinstance(symbol, property) else symbol  # type: ignore
+    source_link = CustomNbdevLookup().code(f"{symbol.__qualname__}")
 
-    return ", ".join(arg_list)
+    if source_link is None:
+        return ""
+
+    href = (
+        source_link.replace("/blob/main/", f"/blob/{lib_version}/")
+        if lib_version.replace(".", "").isdigit()
+        else source_link
+    )
+    return f'<a href="{href}" class="link-to-source" target="_blank">View source</a>'
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 21
-def _get_symbol_definition(symbol: Union[types.FunctionType, Type[Any]]) -> str:
+# %% ../nbs/096_Docusaurus_Helper.ipynb 38
+def _get_method_type(symbol: Union[types.FunctionType, Type[Any]]) -> str:
+    try:
+        source = getsource(symbol).strip()
+    except TypeError as e:
+        return ""
+
+    first_line = source.split("\n")[0]
+    return (
+        f"{first_line}\n"
+        if first_line
+        in ["@abstractmethod", "@staticmethod", "@classmethod", "@property"]
+        else ""
+    )
+
+
+def _get_symbol_definition(
+    symbol: Union[types.FunctionType, Type[Any]], header_level: int, lib_version: str
+) -> str:
     """Return the definition of a given symbol.
 
     Args:
         symbol: A function or method object to get the definition for.
+        header_level: The level of the markdown header to append.
+        lib_version: The current version of the library.
 
     Returns:
         A string representing the function definition
     """
+    if isclass(symbol):
+        return f"{'#'*(header_level - 1)} {symbol.__module__}.{symbol.__name__} {{#{symbol.__module__}.{symbol.__name__}}}\n\n{_get_symbol_source_link(symbol, lib_version)}\n\n"
+
+    if isinstance(symbol, property):
+        symbol = symbol.fget
+
+    symbol_anchor = (
+        f"{'#' * header_level} {symbol.__name__}"
+        + f" {{#{symbol.__module__}.{'.'.join([component.strip('_') for component in symbol.__qualname__.rsplit('.', 1)])}}}\n\n"
+    )
+
+    link_to_source = f"{_get_symbol_source_link(symbol, lib_version)}\n\n"
+
     _signature = signature(symbol)
-    arg_list = _get_arg_list_with_signature(_signature)
-    ret_val = ""
+    parameters = _get_parameters(_signature)
+    symbol_definition = f"```py\n{_get_method_type(symbol)}{_format_symbol_definition(symbol, parameters)}```\n"
+    return symbol_anchor + link_to_source + symbol_definition
 
-    if isfunction(symbol):
-        ret_val = f"### `{symbol.__name__}`" + f" {{#{symbol.__name__.strip('_')}}}\n\n"
-        ret_val = ret_val + f"`def {symbol.__name__}({arg_list})"
-        if _signature.return_annotation and "inspect._empty" not in str(
-            _signature.return_annotation
-        ):
-            if isinstance(_signature.return_annotation, type):
-                ret_val = ret_val + f" -> {_signature.return_annotation.__name__}`\n"
-            else:
-                ret_val = ret_val + f" -> {_signature.return_annotation}`\n"
+# %% ../nbs/096_Docusaurus_Helper.ipynb 44
+def _is_method(symbol: Union[types.FunctionType, Type[Any]]) -> bool:
+    """Check if the given symbol is a method.
 
-        else:
-            ret_val = ret_val + " -> None`\n"
+    Args:
+        symbol: A function or method object to check.
 
-    return ret_val
+    Returns:
+        A boolean indicating whether the symbol is a method.
+    """
+    return ismethod(symbol) or isfunction(symbol) or isinstance(symbol, property)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 28
+# %% ../nbs/096_Docusaurus_Helper.ipynb 46
 def _get_formatted_docstring_for_symbol(
-    symbol: Union[types.FunctionType, Type[Any]]
+    symbol: Union[types.FunctionType, Type[Any]],
+    lib_version: str,
+    header_level: int = 2,
 ) -> str:
     """Recursively parses and get formatted docstring of a symbol.
 
     Args:
         symbol: A Python class or function object to parse the docstring for.
+        lib_version: The current version of the library.
+        header_level: The level of the markdown header to append.
 
     Returns:
         A formatted docstring of the symbol and its members.
 
     """
 
-    def traverse(symbol: Union[types.FunctionType, Type[Any]], contents: str) -> str:
+    def traverse(
+        symbol: Union[types.FunctionType, Type[Any]],
+        contents: str,
+        header_level: int,
+        lib_version: str,
+    ) -> str:
         """Recursively traverse the members of a symbol and append their docstrings to the provided contents string.
 
         Args:
             symbol: A Python class or function object to parse the docstring for.
             contents: The current formatted docstrings.
+            header_level: The level of the markdown header to append.
+            lib_version: The current version of the library.
 
         Returns:
             The updated formatted docstrings.
 
         """
         for x, y in getmembers(symbol):
-            if not x.startswith("_") or x.endswith("__"):
-                if isfunction(y) and y.__doc__ is not None:
-                    contents += f"{_get_symbol_definition(y)}\n{_docstring_to_markdown(y.__doc__)}"
-                elif isclass(y) and not x.startswith("__") and y.__doc__ is not None:
-                    contents += f"{_get_symbol_definition(y)}\n{_docstring_to_markdown(y.__doc__)}"
-                    contents = traverse(y, contents)
+            if not x.startswith("_") or x == "__init__":
+                if _is_method(y) and y.__doc__ is not None:
+                    contents += f"{_get_symbol_definition(y, header_level, lib_version)}\n{_docstring_to_markdown(y.__doc__)}"
+                elif isclass(y) and y.__doc__ is not None and not x.startswith("_"):
+                    contents += f"{_get_symbol_definition(y, header_level+1, lib_version)}\n{_docstring_to_markdown(y.__doc__)}"
+                    contents = traverse(y, contents, header_level + 1, lib_version)
         return contents
 
     contents = (
-        f"{_get_symbol_definition(symbol)}\n{_docstring_to_markdown(symbol.__doc__)}"
+        f"{_get_symbol_definition(symbol, header_level+1, lib_version)}\n{_docstring_to_markdown(symbol.__doc__)}"
         if symbol.__doc__ is not None
         else ""
     )
     if isclass(symbol):
-        contents = traverse(symbol, contents)
+        contents = traverse(symbol, contents, header_level + 1, lib_version)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 32
+# %% ../nbs/096_Docusaurus_Helper.ipynb 49
 def _convert_html_style_attribute_to_jsx(contents: str) -> str:
     """Converts the inline style attributes in an HTML string to JSX compatible format.
 
     Args:
         contents: A string containing an HTML document or fragment.
 
     Returns:
@@ -258,46 +405,46 @@
         for key, value in style_dict.items():
             replacement += f"{key}: '{value}', "
         replacement = replacement[:-2] + "}}"
         contents = contents.replace(f'style="{style_match}"', replacement)
 
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 34
+# %% ../nbs/096_Docusaurus_Helper.ipynb 51
 def _get_all_markdown_files_path(docs_path: Path) -> List[Path]:
     """Get all Markdown files in a directory and its subdirectories.
 
     Args:
         directory: The path to the directory to search in.
 
     Returns:
         A list of paths to all Markdown files found in the directory and its subdirectories.
     """
     markdown_files = [file_path for file_path in docs_path.glob("**/*.md")]
     return markdown_files
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 36
+# %% ../nbs/096_Docusaurus_Helper.ipynb 53
 def _fix_special_symbols_in_html(contents: str) -> str:
     contents = contents.replace("”", '"')
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 38
+# %% ../nbs/096_Docusaurus_Helper.ipynb 55
 def _add_file_extension_to_link(url: str) -> str:
     """Add file extension to the last segment of a URL
 
     Args:
         url: A URL string.
 
     Returns:
         A string of the updated URL with a file extension added to the last segment of the URL.
     """
     segments = url.split("/#")[0].split("/")[-2:]
-    return url.replace(f"/{segments[1]}", f"/{segments[1]}.md")
+    return url.replace(f"/{segments[1]}", f"/{segments[1]}.md").replace(".md/#", ".md#")
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 42
+# %% ../nbs/096_Docusaurus_Helper.ipynb 59
 def _fix_symbol_links(
     contents: str, dir_prefix: str, doc_host: str, doc_baseurl: str
 ) -> str:
     """Fix symbol links in Markdown content.
 
     Args:
         contents: The Markdown content to search for symbol links.
@@ -315,15 +462,15 @@
         old_url = match[1]
         new_url = _add_file_extension_to_link(old_url).replace("/api/", "/docs/api/")
         dir_prefix = "./" if dir_prefix == "" else dir_prefix
         relative_url = dir_prefix + new_url.split("/docs/")[1]
         contents = contents.replace(old_url, relative_url)
     return contents
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 49
+# %% ../nbs/096_Docusaurus_Helper.ipynb 66
 def _get_relative_url_prefix(docs_path: Path, sub_path: Path) -> str:
     """Returns a relative url prefix from a sub path to a docs path.
 
     Args:
         docs_path (Path): The docs directory path.
         sub_path (Path): The sub directory path.
 
@@ -338,15 +485,15 @@
     except ValueError:
         raise ValueError(f"{sub_path} is not a descendant of {docs_path}")
 
     return (
         "../" * (len(relative_path.parts) - 1) if len(relative_path.parts) > 1 else ""
     )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 51
+# %% ../nbs/096_Docusaurus_Helper.ipynb 68
 def fix_invalid_syntax_in_markdown(docs_path: str) -> None:
     """Fix invalid HTML syntax in markdown files and converts inline style attributes to JSX-compatible format.
 
     Args:
         docs_path: The path to the root directory to search for markdown files.
     """
     cfg = get_config()
@@ -359,39 +506,37 @@
         contents = Path(file).read_text()
 
         contents = _convert_html_style_attribute_to_jsx(contents)
         contents = _fix_special_symbols_in_html(contents)
         contents = _fix_symbol_links(
             contents, relative_url_prefix, doc_host, doc_baseurl
         )
-
         file.write_text(contents)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 53
+# %% ../nbs/096_Docusaurus_Helper.ipynb 70
 def generate_markdown_docs(module_name: str, docs_path: str) -> None:
     """Generates Markdown documentation files for the symbols in the given module and save them to the given directory.
 
     Args:
         module_name: The name of the module to generate documentation for.
         docs_path: The path to the directory where the documentation files will be saved.
     """
     members_with_submodules = _get_submodules(module_name)
     symbols = _load_submodules(module_name, members_with_submodules)
+    lib_version = get_config()["version"]
 
     for symbol in symbols:
-        content = f"## `{symbol.__module__}.{symbol.__name__}` {{#{symbol.__module__}.{symbol.__name__}}}\n\n"
-        content += _get_formatted_docstring_for_symbol(symbol)
+        content = _get_formatted_docstring_for_symbol(symbol, lib_version)
         target_file_path = (
             "/".join(f"{symbol.__module__}.{symbol.__name__}".split(".")) + ".md"
         )
-
         with open((Path(docs_path) / "api" / target_file_path), "w") as f:
             f.write(content)
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 55
+# %% ../nbs/096_Docusaurus_Helper.ipynb 73
 def _parse_lines(lines: List[str]) -> Tuple[List[str], int]:
     """Parse a list of lines and return a tuple containing a list of filenames and an index indicating how many lines to skip.
 
     Args:
         lines: A list of strings representing lines of input text.
 
     Returns:
@@ -400,15 +545,15 @@
     """
     index = next(
         (i for i, line in enumerate(lines) if not line.strip().startswith("- [")),
         len(lines),
     )
     return [line.split("(")[1][:-4] for line in lines[:index]], index
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 58
+# %% ../nbs/096_Docusaurus_Helper.ipynb 76
 def _parse_section(text: str, ignore_first_line: bool = False) -> List[Any]:
     """Parse the given section contents and return a list of file names in the expected format.
 
     Args:
         text: A string representing the contents of a file.
         ignore_first_line: Flag indicating whether to ignore the first line extracting the section contents.
 
@@ -429,15 +574,15 @@
             value, skip_lines = _parse_lines(lines[index + 1 :])
             ret_val.append({line.replace("-", "").strip(): value})
             index += skip_lines + 1
         else:
             index += 1
     return ret_val
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 61
+# %% ../nbs/096_Docusaurus_Helper.ipynb 79
 def _get_section_from_markdown(
     markdown_text: str, section_header: str
 ) -> Optional[str]:
     """Get the contents of the section header from the given markdown text
 
     Args:
         markdown_text: A string containing the markdown text to extract the section from.
@@ -447,15 +592,15 @@
         A string representing the contents of the section header if the section header
         is present in the markdown text, else None
     """
     pattern = re.compile(rf"^- {section_header}\n((?:\s+- .*\n)+)", re.M)
     match = pattern.search(markdown_text)
     return match.group(1) if match else None
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 66
+# %% ../nbs/096_Docusaurus_Helper.ipynb 84
 def generate_sidebar(
     summary_file: str = "./docusaurus/docs/SUMMARY.md",
     summary: str = "",
     target: str = "./docusaurus/sidebars.js",
 ) -> None:
     """
     Generate a sidebar js file for a Docusaurus documentation site based on a SUMMARY.md file.
@@ -503,15 +648,15 @@
     "LICENSE",
     "CONTRIBUTING",
     "CHANGELOG",
 ],
 };"""
         )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 68
+# %% ../nbs/096_Docusaurus_Helper.ipynb 86
 def _get_markdown_filenames_from_sidebar(sidebar_file_path: str) -> List[str]:
     """Get a list of Markdown filenames included in the sidebar.
 
     Args:
         sidebar_file_path: The path to the sidebar file.
 
     Returns:
@@ -524,15 +669,15 @@
         match = re.search(pattern, file_content, re.DOTALL)
         all_sidebar_files = ast.literal_eval(match.group(1)) if match else []
         markdown_filenames = [
             f"{v}.md" for v in all_sidebar_files if isinstance(v, str)
         ]
         return markdown_filenames
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 70
+# %% ../nbs/096_Docusaurus_Helper.ipynb 88
 def _delete_files(files: List[Path]) -> None:
     """Deletes a list of files.
 
     Args:
         files: A list of Path objects representing the files to be deleted.
 
     Raises:
@@ -543,15 +688,15 @@
         try:
             file.unlink()
         except OSError as e:
             typer.echo(
                 f"Error deleting files from docusaurus/docs directory. Could not delete file: {file} - {e}"
             )
 
-# %% ../nbs/096_Docusaurus_Helper.ipynb 73
+# %% ../nbs/096_Docusaurus_Helper.ipynb 91
 def delete_unused_markdown_files_from_sidebar(
     docs_path: str, sidebar_file_path: str
 ) -> None:
     """Delete the markdown files from the docs directory that are not present in the sidebar.
 
     Args:
         docs_path: Path to the directory containing the markdown files.
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_helpers.py` & `fastkafka-0.8.0rc0/fastkafka/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import json
 import textwrap
 from datetime import datetime, timedelta
 from typing import *
 
 import aiohttp
 import anyio
-from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
+from ._aiokafka_imports import AIOKafkaProducer, AIOKafkaConsumer
 from aiokafka.helpers import create_ssl_context
 from aiokafka.structs import RecordMetadata
 from IPython.display import Markdown
 
 from ._components.helpers import in_notebook
 from ._components.logger import get_logger
 from ._components.meta import delegates
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_modidx.py` & `fastkafka-0.8.0rc0/fastkafka/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,18 +97,14 @@
                                                                                                      'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._create_mirrors': ( 'tester.html#tester._create_mirrors',
                                                                                                          'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._start_tester': ( 'tester.html#tester._start_tester',
                                                                                                        'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.Tester._stop_tester': ( 'tester.html#tester._stop_tester',
                                                                                                       'fastkafka/_application/tester.py'),
-                                               'fastkafka._application.tester.Tester.using_local_kafka': ( 'tester.html#tester.using_local_kafka',
-                                                                                                           'fastkafka/_application/tester.py'),
-                                               'fastkafka._application.tester.Tester.using_local_redpanda': ( 'tester.html#tester.using_local_redpanda',
-                                                                                                              'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester._get_broker_spec': ( 'tester.html#_get_broker_spec',
                                                                                                    'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_consumer': ( 'tester.html#mirror_consumer',
                                                                                                   'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.mirror_producer': ( 'tester.html#mirror_producer',
                                                                                                   'fastkafka/_application/tester.py'),
                                                'fastkafka._application.tester.set_sugar': ( 'tester.html#set_sugar',
@@ -341,28 +337,36 @@
                                                                                                                    'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming._process_items_coro': ( 'taskstreaming.html#_process_items_coro',
                                                                                                                     'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming._process_items_task': ( 'taskstreaming.html#_process_items_task',
                                                                                                                     'fastkafka/_components/task_streaming.py'),
                                                       'fastkafka._components.task_streaming.get_executor': ( 'taskstreaming.html#get_executor',
                                                                                                              'fastkafka/_components/task_streaming.py')},
-            'fastkafka._components.test_dependencies': { 'fastkafka._components.test_dependencies._install_java': ( 'test_dependencies.html#_install_java',
+            'fastkafka._components.test_dependencies': { 'fastkafka._components.test_dependencies.VersionParser': ( 'test_dependencies.html#versionparser',
+                                                                                                                    'fastkafka/_components/test_dependencies.py'),
+                                                         'fastkafka._components.test_dependencies.VersionParser.__init__': ( 'test_dependencies.html#versionparser.__init__',
+                                                                                                                             'fastkafka/_components/test_dependencies.py'),
+                                                         'fastkafka._components.test_dependencies.VersionParser.handle_data': ( 'test_dependencies.html#versionparser.handle_data',
+                                                                                                                                'fastkafka/_components/test_dependencies.py'),
+                                                         'fastkafka._components.test_dependencies._install_java': ( 'test_dependencies.html#_install_java',
                                                                                                                     'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_kafka': ( 'test_dependencies.html#_install_kafka',
                                                                                                                      'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies._install_testing_deps': ( 'test_dependencies.html#_install_testing_deps',
                                                                                                                             'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies.check_java': ( 'test_dependencies.html#check_java',
                                                                                                                  'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies.check_kafka': ( 'test_dependencies.html#check_kafka',
                                                                                                                   'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies.generate_app_in_tmp': ( 'test_dependencies.html#generate_app_in_tmp',
                                                                                                                           'fastkafka/_components/test_dependencies.py'),
                                                          'fastkafka._components.test_dependencies.generate_app_src': ( 'test_dependencies.html#generate_app_src',
-                                                                                                                       'fastkafka/_components/test_dependencies.py')},
+                                                                                                                       'fastkafka/_components/test_dependencies.py'),
+                                                         'fastkafka._components.test_dependencies.get_kafka_version': ( 'test_dependencies.html#get_kafka_version',
+                                                                                                                        'fastkafka/_components/test_dependencies.py')},
             'fastkafka._testing.apache_kafka_broker': { 'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker': ( 'apachekafkabroker.html#apachekafkabroker',
                                                                                                                       'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.__aenter__': ( 'apachekafkabroker.html#apachekafkabroker.__aenter__',
                                                                                                                                  'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.__aexit__': ( 'apachekafkabroker.html#apachekafkabroker.__aexit__',
                                                                                                                                 'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.__enter__': ( 'apachekafkabroker.html#apachekafkabroker.__enter__',
@@ -389,22 +393,34 @@
                                                                                                                                                 'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.is_started': ( 'apachekafkabroker.html#apachekafkabroker.is_started',
                                                                                                                                  'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.start': ( 'apachekafkabroker.html#apachekafkabroker.start',
                                                                                                                             'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.ApacheKafkaBroker.stop': ( 'apachekafkabroker.html#apachekafkabroker.stop',
                                                                                                                            'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker._get_unique_local_brokers_to_start': ( 'apachekafkabroker.html#_get_unique_local_brokers_to_start',
+                                                                                                                                       'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker._start_and_stop_brokers': ( 'apachekafkabroker.html#_start_and_stop_brokers',
+                                                                                                                            'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker._start_broker': ( 'apachekafkabroker.html#_start_broker',
+                                                                                                                  'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker._stop_broker': ( 'apachekafkabroker.html#_stop_broker',
+                                                                                                                 'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.get_free_port': ( 'apachekafkabroker.html#get_free_port',
                                                                                                                   'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.get_kafka_config_string': ( 'apachekafkabroker.html#get_kafka_config_string',
                                                                                                                             'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.get_zookeeper_config_string': ( 'apachekafkabroker.html#get_zookeeper_config_string',
                                                                                                                                 'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker.is_port_in_use': ( 'apachekafkabroker.html#is_port_in_use',
+                                                                                                                   'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.run_and_match': ( 'apachekafkabroker.html#run_and_match',
                                                                                                                   'fastkafka/_testing/apache_kafka_broker.py'),
+                                                        'fastkafka._testing.apache_kafka_broker.start_apache_kafka_brokers': ( 'apachekafkabroker.html#start_apache_kafka_brokers',
+                                                                                                                               'fastkafka/_testing/apache_kafka_broker.py'),
                                                         'fastkafka._testing.apache_kafka_broker.write_config_and_run': ( 'apachekafkabroker.html#write_config_and_run',
                                                                                                                          'fastkafka/_testing/apache_kafka_broker.py')},
             'fastkafka._testing.in_memory_broker': { 'fastkafka._testing.in_memory_broker.GroupMetadata': ( 'inmemorybroker.html#groupmetadata',
                                                                                                             'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.GroupMetadata.__init__': ( 'inmemorybroker.html#groupmetadata.__init__',
                                                                                                                      'fastkafka/_testing/in_memory_broker.py'),
                                                      'fastkafka._testing.in_memory_broker.GroupMetadata.assign_partitions': ( 'inmemorybroker.html#groupmetadata.assign_partitions',
@@ -538,15 +554,17 @@
                                                           'fastkafka._testing.local_redpanda_broker.LocalRedpandaBroker.start': ( 'localredpandabroker.html#localredpandabroker.start',
                                                                                                                                   'fastkafka/_testing/local_redpanda_broker.py'),
                                                           'fastkafka._testing.local_redpanda_broker.LocalRedpandaBroker.stop': ( 'localredpandabroker.html#localredpandabroker.stop',
                                                                                                                                  'fastkafka/_testing/local_redpanda_broker.py'),
                                                           'fastkafka._testing.local_redpanda_broker.check_docker': ( 'localredpandabroker.html#check_docker',
                                                                                                                      'fastkafka/_testing/local_redpanda_broker.py'),
                                                           'fastkafka._testing.local_redpanda_broker.get_redpanda_docker_cmd': ( 'localredpandabroker.html#get_redpanda_docker_cmd',
-                                                                                                                                'fastkafka/_testing/local_redpanda_broker.py')},
+                                                                                                                                'fastkafka/_testing/local_redpanda_broker.py'),
+                                                          'fastkafka._testing.local_redpanda_broker.start_redpanda_brokers': ( 'localredpandabroker.html#start_redpanda_brokers',
+                                                                                                                               'fastkafka/_testing/local_redpanda_broker.py')},
             'fastkafka._testing.test_utils': { 'fastkafka._testing.test_utils.display_docs': ( 'test_utils.html#display_docs',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.mock_AIOKafkaProducer_send': ( 'test_utils.html#mock_aiokafkaproducer_send',
                                                                                                              'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.nb_safe_seed': ( 'test_utils.html#nb_safe_seed',
                                                                                                'fastkafka/_testing/test_utils.py'),
                                                'fastkafka._testing.test_utils.run_script_and_cancel': ( 'test_utils.html#run_script_and_cancel',
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_server.py` & `fastkafka-0.8.0rc0/fastkafka/_server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/021_FastKafkaServer.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'ServerProcess', 'run_fastkafka_server_process', 'terminate_asyncio_process', 'run_fastkafka_server',
-           'run_in_process']
+__all__ = ['logger', 'ServerProcess', 'run_fastkafka_server_process', 'run_fastkafka_server', 'run_in_process']
 
 # %% ../nbs/021_FastKafkaServer.ipynb 1
 import asyncio
 import multiprocessing
 import platform
 import signal
 import threading
@@ -15,14 +14,15 @@
 from types import FrameType
 
 import asyncer
 import typer
 
 from ._components.helpers import _import_from_string
 from ._components.logger import get_logger
+from ._components._subprocess import terminate_asyncio_process
 
 # %% ../nbs/021_FastKafkaServer.ipynb 5
 logger = get_logger(__name__, level=20)
 
 # %% ../nbs/021_FastKafkaServer.ipynb 7
 class ServerProcess:
     def __init__(self, app: str, kafka_broker_name: str):
@@ -64,14 +64,16 @@
 
         loop = asyncio.get_event_loop()
 
         HANDLED_SIGNALS = (
             signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
             signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
         )
+        if platform.system() == "Windows":
+            HANDLED_SIGNALS = (*HANDLED_SIGNALS, signal.SIGBREAK)  # type: ignore
 
         def handle_windows_exit(signum: int, frame: Optional[FrameType]) -> None:
             self.should_exit = True
 
         def handle_exit(sig: int) -> None:
             self.should_exit = True
 
@@ -101,50 +103,15 @@
     kafka_broker: str = typer.Option(
         ...,
         help="Kafka broker, one of the keys of the kafka_brokers dictionary passed in the constructor of FastKafka class.",
     ),
 ) -> None:
     ServerProcess(app, kafka_broker).run()
 
-# %% ../nbs/021_FastKafkaServer.ipynb 10
-async def terminate_asyncio_process(p: asyncio.subprocess.Process) -> None:
-    """
-    Terminates an asyncio process.
-
-    Args:
-        p (asyncio.subprocess.Process): The process to terminate.
-    """
-    logger.info(f"terminate_asyncio_process(): Terminating the process {p.pid}...")
-    # Check if SIGINT already propagated to process
-    try:
-        await asyncio.wait_for(p.wait(), 1)
-        logger.info(
-            f"terminate_asyncio_process(): Process {p.pid} was already terminated."
-        )
-        return
-    except asyncio.TimeoutError:
-        pass
-
-    for i in range(3):
-        p.terminate()
-        try:
-            await asyncio.wait_for(p.wait(), 10)
-            logger.info(f"terminate_asyncio_process(): Process {p.pid} terminated.")
-            return
-        except asyncio.TimeoutError:
-            logger.warning(
-                f"terminate_asyncio_process(): Process {p.pid} not terminated, retrying..."
-            )
-
-    logger.warning(f"Killing the process {p.pid}...")
-    p.kill()
-    await p.wait()
-    logger.warning(f"terminate_asyncio_process(): Process {p.pid} killed!")
-
-# %% ../nbs/021_FastKafkaServer.ipynb 12
+# %% ../nbs/021_FastKafkaServer.ipynb 11
 async def run_fastkafka_server(num_workers: int, app: str, kafka_broker: str) -> None:
     """
     Runs the FastKafka server with multiple worker processes.
 
     Args:
         num_workers (int): Number of FastKafka instances to run.
         app (str): Input in the form of 'path:app', where **path** is the path to a python file and **app** is an object of type **FastKafka**.
@@ -152,14 +119,16 @@
     """
     loop = asyncio.get_event_loop()
 
     HANDLED_SIGNALS = (
         signal.SIGINT,  # Unix signal 2. Sent by Ctrl+C.
         signal.SIGTERM,  # Unix signal 15. Sent by `kill <pid>`.
     )
+    if platform.system() == "Windows":
+        HANDLED_SIGNALS = (*HANDLED_SIGNALS, signal.SIGBREAK)  # type: ignore
 
     d = {"should_exit": False}
 
     def handle_windows_exit(
         signum: int, frame: Optional[FrameType], d: Dict[str, bool] = d
     ) -> None:
         d["should_exit"] = True
@@ -222,15 +191,15 @@
         typer.secho(
             f"Return codes are not all zero: {returncodes}",
             err=True,
             fg=typer.colors.RED,
         )
         raise typer.Exit(1)
 
-# %% ../nbs/021_FastKafkaServer.ipynb 13
+# %% ../nbs/021_FastKafkaServer.ipynb 12
 @contextmanager
 def run_in_process(
     target: Callable[..., Any]
 ) -> Generator[multiprocessing.Process, None, None]:
     """
     Runs the target function in a separate process.
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_testing/apache_kafka_broker.py` & `fastkafka-0.8.0rc0/fastkafka/_testing/apache_kafka_broker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/002_ApacheKafkaBroker.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'get_zookeeper_config_string', 'get_kafka_config_string', 'ApacheKafkaBroker', 'run_and_match',
-           'get_free_port', 'write_config_and_run']
+__all__ = ['logger', 'T', 'get_zookeeper_config_string', 'get_kafka_config_string', 'ApacheKafkaBroker', 'run_and_match',
+           'is_port_in_use', 'get_free_port', 'write_config_and_run', 'start_apache_kafka_brokers']
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 1
 import asyncio
 import re
 import platform
 import socket
+import subprocess  # nosec
+from contextlib import asynccontextmanager
 from datetime import datetime, timedelta
 from os import environ
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import *
 
 import asyncer
@@ -206,14 +208,23 @@
         self.kafka_task: Optional[asyncio.subprocess.Process] = None
         self.zookeeper_task: Optional[asyncio.subprocess.Process] = None
         self._is_started = False
         self.topics: Iterable[str] = topics
 
     @property
     def is_started(self) -> bool:
+        """Property indicating whether the ApacheKafkaBroker object is started.
+
+        The is_started property indicates if the ApacheKafkaBroker object is currently
+        in a started state. This implies that Zookeeper and Kafka broker processes have
+        sucesfully started and are ready for handling events.
+
+        Returns:
+            bool: True if the object is started, False otherwise.
+        """
         return self._is_started
 
     @classmethod
     def _check_deps(cls) -> None:
         """Prepares the environment for running Kafka brokers.
         Returns:
            None
@@ -339,19 +350,28 @@
         ValueError: If the capture parameter has an unsupported value.
         TimeoutError: If the process times out.
         RuntimeError: If the process returns a non-zero return code.
     """
     # Create the subprocess; redirect the standard output
     # into a pipe.
     matched = 0
-    proc = await asyncio.create_subprocess_exec(
-        *args,
-        stdout=asyncio.subprocess.PIPE,
-        stderr=asyncio.subprocess.PIPE,
-    )
+
+    if platform.system() == "Windows":
+        proc = await asyncio.create_subprocess_shell(
+            " ".join(args),
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+            creationflags=subprocess.CREATE_NEW_PROCESS_GROUP,  # type: ignore
+        )
+    else:
+        proc = await asyncio.create_subprocess_exec(
+            *args,
+            stdout=asyncio.subprocess.PIPE,
+            stderr=asyncio.subprocess.PIPE,
+        )
 
     # Read one line of output.
     t = datetime.now()
     while datetime.now() - t < timedelta(seconds=timeout):
         try:
             if capture == "stdout":
                 data = await asyncio.wait_for(proc.stdout.readline(), timeout=1.0)  # type: ignore
@@ -372,25 +392,41 @@
             pass
 
         if proc.returncode is not None:
             stdout, stderr = await proc.communicate()
             dstdout = stdout.decode("utf-8")
             dstderr = stderr.decode("utf-8")
             if proc.returncode == 0:
-                raise TimeoutError()
+                raise TimeoutError(
+                    f"stdout={dstdout}, stderr={dstderr}, returncode={proc.returncode}"
+                )
             else:
                 raise RuntimeError(
                     f"stdout={dstdout}, stderr={dstderr}, returncode={proc.returncode}"
                 )
 
     await terminate_asyncio_process(proc)
 
     raise TimeoutError()
 
 # %% ../../nbs/002_ApacheKafkaBroker.ipynb 20
+def is_port_in_use(port: Union[int, str]) -> bool:
+    """
+    Checks if a port is already in use.
+
+    Args:
+        port (Union[int, str]): The port number to check. It can be provided as an integer or a string.
+
+    Returns:
+        bool: True if the port is in use, False otherwise.
+    """
+    with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+        return s.connect_ex(("localhost", int(port))) == 0
+
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 22
 def get_free_port() -> str:
     """Gets a port number which is available and free in the system.
 
     Returns:
         The free port number as a string.
     """
     s = socket.socket()
@@ -469,20 +505,28 @@
             f.write(
                 self.get_service_config_string(
                     service, data_dir=self.temporary_directory_path
                 )
             )
 
         try:
+            port = (
+                self.zookeeper_kwargs["zookeeper_port"]
+                if service == "zookeeper"
+                else self.kafka_kwargs["listener_port"]
+            )
+            if is_port_in_use(port):
+                raise ValueError(f"Port {port} is already in use")
+
             script_extension = "bat" if platform.system() == "Windows" else "sh"
             service_start_script = f"{service}-server-start.{script_extension}"
             service_task = await run_and_match(
                 service_start_script,
                 str(service_config_path),
-                pattern="INFO \[KafkaServer id=0\] started"
+                pattern="Recorded new controller, from now on will use node"
                 if service == "kafka"
                 else "INFO Snapshot taken",
                 timeout=30,
             )
         except Exception as e:
             print(e)
             logger.info(
@@ -576,15 +620,15 @@
 async def _stop(self: ApacheKafkaBroker) -> None:
     """Stops a local Kafka broker and ZooKeeper instance asynchronously."""
     await terminate_asyncio_process(self.kafka_task)  # type: ignore
     await terminate_asyncio_process(self.zookeeper_task)  # type: ignore
     self.temporary_directory.__exit__(None, None, None)  # type: ignore
     self._is_started = False
 
-# %% ../../nbs/002_ApacheKafkaBroker.ipynb 23
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 25
 @patch
 def start(self: ApacheKafkaBroker) -> str:
     """Starts a local Kafka broker and ZooKeeper instance synchronously.
 
     Returns:
         The Kafka broker bootstrap server address in string format: host:port.
     """
@@ -638,7 +682,115 @@
                 "ApacheKafkaBroker not started yet, please call ApacheKafkaBroker.start() before!"
             )
 
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._stop())
     finally:
         logger.info(f"{self.__class__.__name__}.stop(): exited.")
+
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 30
+async def _start_broker(broker: Any) -> Union[Any, Exception]:
+    try:
+        await broker._start()
+        return broker
+    except Exception as e:
+        return e
+
+
+async def _stop_broker(broker: Any) -> Union[Any, Exception]:
+    try:
+        await broker._stop()
+        return broker
+    except Exception as e:
+        return e
+
+
+async def _get_unique_local_brokers_to_start(
+    kafka_brokers_name: str,
+    kafka_brokers: List[Dict[str, Dict[str, Any]]],
+    duplicate_ok: bool = False,
+    zookeeper_ports: List[int] = [2181],
+    ignore_nonlocal_brokers: bool = False,
+) -> List[Tuple[str, int]]:
+    brokers_to_start = [
+        x[kafka_brokers_name] for x in kafka_brokers if kafka_brokers_name in x
+    ]
+    unique_brokers_to_start = set([(x["url"], x["port"]) for x in brokers_to_start])
+
+    if len(unique_brokers_to_start) < len(brokers_to_start) and not duplicate_ok:
+        raise ValueError(
+            f"Duplicate kafka_brokers are found - {brokers_to_start}. Please change values or use 'duplicate_ok=True'"
+        )
+
+    unique_urls = set([x[0] for x in unique_brokers_to_start])
+    localhost_urls = set(
+        [
+            "localhost",
+            "127.0.0.1",
+            "0.0.0.0",  # nosec: B104 - Possible binding to all interfaces
+        ]
+    )
+    if not unique_urls.issubset(localhost_urls) and not ignore_nonlocal_brokers:
+        raise ValueError(
+            f"URL values other than {', '.join(sorted(localhost_urls))} are found - {unique_urls - localhost_urls}. Please change values or use 'ignore_nonlocal_brokers=True'"
+        )
+
+    unique_local_brokers_to_start = [
+        x for x in unique_brokers_to_start if x[0] in localhost_urls
+    ]
+    return unique_local_brokers_to_start
+
+# %% ../../nbs/002_ApacheKafkaBroker.ipynb 31
+T = TypeVar("T")
+
+
+@asynccontextmanager
+async def _start_and_stop_brokers(brokers: List[T]) -> AsyncIterator[None]:
+    try:
+        retvals = [await _start_broker(broker) for broker in brokers]
+        exceptions = [x for x in retvals if isinstance(x, Exception)]
+
+        if exceptions:
+            raise RuntimeError(exceptions)
+
+        yield
+    finally:
+        retvals = [
+            await _stop_broker(broker)
+            for broker in retvals
+            if not isinstance(broker, Exception)
+        ]
+        exceptions = [x for x in retvals if isinstance(x, Exception)]
+
+        if exceptions:
+            raise RuntimeError(exceptions)
+
+
+@asynccontextmanager
+async def start_apache_kafka_brokers(
+    kafka_brokers_name: str,
+    kafka_brokers: List[Dict[str, Dict[str, Any]]],
+    duplicate_ok: bool = False,
+    zookeeper_ports: List[int] = [2181],
+    ignore_nonlocal_brokers: bool = False,
+) -> AsyncIterator[None]:
+    unique_local_brokers_to_start = await _get_unique_local_brokers_to_start(
+        kafka_brokers_name=kafka_brokers_name,
+        kafka_brokers=kafka_brokers,
+        duplicate_ok=duplicate_ok,
+        ignore_nonlocal_brokers=ignore_nonlocal_brokers,
+    )
+
+    if len(zookeeper_ports) < len(unique_local_brokers_to_start):
+        raise ValueError(
+            f"Atleast {len(unique_local_brokers_to_start)} zookeeper ports are needed to start kafka. Current zookeeper_ports length is {len(zookeeper_ports)}"
+        )
+
+    brokers = [
+        ApacheKafkaBroker(listener_port=broker[1], zookeeper_port=zookeeper_port)  # type: ignore
+        for broker, zookeeper_port in zip(
+            unique_local_brokers_to_start, zookeeper_ports
+        )
+    ]
+
+    async with _start_and_stop_brokers(brokers=brokers):
+        yield
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_testing/in_memory_broker.py` & `fastkafka-0.8.0rc0/fastkafka/_testing/in_memory_broker.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 import hashlib
 import random
 import string
 import uuid
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from typing import *
+from types import ModuleType
 
-from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from aiokafka.structs import ConsumerRecord, RecordMetadata, TopicPartition
 
-import fastkafka._application.app
 import fastkafka._components.aiokafka_consumer_loop
+import fastkafka._aiokafka_imports
+from .._aiokafka_imports import AIOKafkaConsumer, AIOKafkaProducer
 from .._components.logger import get_logger
 from fastkafka._components.meta import (
     _get_default_kwargs_from_sig,
     classcontextmanager,
     delegates,
     patch,
 )
@@ -317,19 +318,22 @@
 
 # %% ../../nbs/001_InMemoryBroker.ipynb 22
 @classcontextmanager()
 class InMemoryBroker:
     def __init__(
         self,
         num_partitions: int = 1,
+        *,
+        patch_module: Optional[ModuleType] = None,
     ):
         self.num_partitions = num_partitions
         self.topics: Dict[Tuple[str, str], KafkaTopic] = {}
         self.topic_groups: Dict[Tuple[str, str, str], GroupMetadata] = {}
         self.is_started: bool = False
+        self.patch_module = patch_module
 
     def connect(self) -> uuid.UUID:
         return uuid.uuid4()
 
     def dissconnect(self, consumer_id: uuid.UUID) -> None:
         """
         Disconnect a consumer from the broker.
@@ -918,31 +922,22 @@
     """
     logger.info(
         "InMemoryBroker._patch_consumers_and_producers(): Patching consumers and producers!"
     )
     try:
         logger.info("InMemoryBroker starting")
 
-        old_consumer_app = fastkafka._application.app.AIOKafkaConsumer
-        old_producer_app = fastkafka._application.app.AIOKafkaProducer
-        old_consumer_loop = (
-            fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer
-        )
+        old_consumer = fastkafka._aiokafka_imports.AIOKafkaConsumer
+        old_producer = fastkafka._aiokafka_imports.AIOKafkaProducer
 
-        fastkafka._application.app.AIOKafkaConsumer = InMemoryConsumer(self)
-        fastkafka._application.app.AIOKafkaProducer = InMemoryProducer(self)
-        fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer = (
-            InMemoryConsumer(self)
-        )
+        fastkafka._aiokafka_imports.AIOKafkaConsumer = InMemoryConsumer(self)
+        fastkafka._aiokafka_imports.AIOKafkaProducer = InMemoryProducer(self)
 
         self.is_started = True
         yield self
     finally:
         logger.info("InMemoryBroker stopping")
 
-        fastkafka._application.app.AIOKafkaConsumer = old_consumer_app
-        fastkafka._application.app.AIOKafkaProducer = old_producer_app
-        fastkafka._components.aiokafka_consumer_loop.AIOKafkaConsumer = (
-            old_consumer_loop
-        )
+        fastkafka._aiokafka_imports.AIOKafkaConsumer = old_consumer
+        fastkafka._aiokafka_imports.AIOKafkaProducer = old_producer
 
         self.is_started = False
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_testing/local_redpanda_broker.py` & `fastkafka-0.8.0rc0/fastkafka/_testing/local_redpanda_broker.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/003_LocalRedpandaBroker.ipynb.
 
 # %% auto 0
-__all__ = ['logger', 'get_redpanda_docker_cmd', 'LocalRedpandaBroker', 'check_docker']
+__all__ = ['logger', 'get_redpanda_docker_cmd', 'LocalRedpandaBroker', 'check_docker', 'start_redpanda_brokers']
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 1
 import asyncio
 from pathlib import Path
+from contextlib import asynccontextmanager
 from tempfile import TemporaryDirectory
 from typing import *
 
 import asyncer
 import nest_asyncio
 
 from .._components._subprocess import terminate_asyncio_process
 from .._components.helpers import in_notebook
 from .._components.logger import get_logger
 from .._components.meta import delegates, export, patch
-from .apache_kafka_broker import get_free_port, run_and_match
+from fastkafka._testing.apache_kafka_broker import (
+    get_free_port,
+    run_and_match,
+    _get_unique_local_brokers_to_start,
+    _start_and_stop_brokers,
+)
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 3
 if in_notebook():
     from tqdm.notebook import tqdm
 else:
     from tqdm import tqdm
 
@@ -112,14 +118,23 @@
         self.temporary_directory_path: Optional[Path] = None
         self.redpanda_task: Optional[asyncio.subprocess.Process] = None
         self._is_started = False
         self.topics: Iterable[str] = topics
 
     @property
     def is_started(self) -> bool:
+        """Property indicating whether the LocalRedpandaBroker object is started.
+
+        The is_started property indicates if the LocalRedpandaBroker object is currently
+        in a started state. This implies that Redpanda docker container has sucesfully
+        started and is ready for handling events.
+
+        Returns:
+            bool: True if the object is started, False otherwise.
+        """
         return self._is_started
 
     @classmethod
     async def _check_deps(cls) -> None:
         """Prepares the environment for running redpanda brokers.
         Returns:
            None
@@ -185,17 +200,31 @@
     async def __aenter__(self) -> str:
         return await self._start()
 
     async def __aexit__(self, *args: Any, **kwargs: Any) -> None:
         await self._stop()
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 10
-async def check_docker() -> bool:
+async def check_docker(tag: str = "v23.1.2") -> bool:
+    """
+    Checks if a Docker image with the specified tag is available.
+
+    Args:
+        tag: The tag of the Docker image to check. Defaults to "v23.1.2".
+
+    Returns:
+        bool: True if the Docker image is available; False otherwise.
+    """
     try:
-        docker_task = await run_and_match("docker", "-v", pattern="Docker version")
+        docker_task = await run_and_match(
+            "docker",
+            "pull",
+            f"docker.redpanda.com/redpandadata/redpanda:{tag}",
+            pattern=f"docker.redpanda.com/redpandadata/redpanda:{tag}",
+        )
         return True
     except Exception as e:
         logger.debug(f"Error in check_docker() : {e}")
         return False
 
 # %% ../../nbs/003_LocalRedpandaBroker.ipynb 12
 @patch(cls_method=True)  # type: ignore
@@ -360,7 +389,30 @@
                 "LocalRedpandaBroker not started yet, please call LocalRedpandaBroker.start() before!"
             )
 
         loop = asyncio.get_event_loop()
         loop.run_until_complete(self._stop())
     finally:
         logger.info(f"{self.__class__.__name__}.stop(): exited.")
+
+# %% ../../nbs/003_LocalRedpandaBroker.ipynb 21
+@asynccontextmanager
+async def start_redpanda_brokers(
+    kafka_brokers_name: str,
+    kafka_brokers: List[Dict[str, Dict[str, Any]]],
+    duplicate_ok: bool = False,
+    ignore_nonlocal_brokers: bool = False,
+) -> AsyncIterator[None]:
+    unique_local_brokers_to_start = await _get_unique_local_brokers_to_start(
+        kafka_brokers_name=kafka_brokers_name,
+        kafka_brokers=kafka_brokers,
+        duplicate_ok=duplicate_ok,
+        ignore_nonlocal_brokers=ignore_nonlocal_brokers,
+    )
+
+    brokers = [
+        LocalRedpandaBroker(listener_port=broker[1])  # type: ignore
+        for broker in unique_local_brokers_to_start
+    ]
+
+    async with _start_and_stop_brokers(brokers=brokers):
+        yield
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/_testing/test_utils.py` & `fastkafka-0.8.0rc0/fastkafka/_testing/test_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 # %% auto 0
 __all__ = ['logger', 'nb_safe_seed', 'mock_AIOKafkaProducer_send', 'run_script_and_cancel', 'display_docs']
 
 # %% ../../nbs/004_Test_Utils.ipynb 1
 import asyncio
 import hashlib
+import platform
 import shlex
+import signal
 import subprocess  # nosec
 import unittest
 import unittest.mock
 from contextlib import contextmanager
 from pathlib import Path
 from tempfile import TemporaryDirectory
 from typing import *
@@ -104,19 +106,30 @@
                 )
                 await asyncer.asyncify(kafka_app.create_docs)()
             except Exception as e:
                 logger.warning(
                     f"Generating docs failed for: {Path(script_file).stem}:{kafka_app_name}, ignoring it for now."
                 )
 
-        proc = subprocess.Popen(  # nosec: [B603:subprocess_without_shell_equals_true] subprocess call - check for execution of untrusted input.
-            shlex.split(cmd), stdout=subprocess.PIPE, stderr=subprocess.STDOUT, cwd=d
+        creationflags = 0 if platform.system() != "Windows" else subprocess.CREATE_NEW_PROCESS_GROUP  # type: ignore
+        proc = subprocess.Popen(
+            shlex.split(cmd),
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            cwd=d,
+            shell=True  # nosec: [B602:subprocess_without_shell_equals_true] subprocess call - check for execution of untrusted input.
+            if platform.system() == "Windows"
+            else False,
+            creationflags=creationflags,
         )
         await asyncio.sleep(cancel_after)
-        proc.terminate()
+        if platform.system() == "Windows":
+            proc.send_signal(signal.CTRL_BREAK_EVENT)  # type: ignore
+        else:
+            proc.terminate()
         output, _ = proc.communicate()
 
         return (proc.returncode, output)
 
 # %% ../../nbs/004_Test_Utils.ipynb 14
 async def display_docs(docs_path: str, port: int = 4000) -> None:
     """
```

### Comparing `fastkafka-0.7.0rc2/fastkafka/encoder.py` & `fastkafka-0.8.0rc0/fastkafka/encoder.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka/testing.py` & `fastkafka-0.8.0rc0/fastkafka/testing.py`

 * *Files identical despite different names*

### Comparing `fastkafka-0.7.0rc2/fastkafka.egg-info/PKG-INFO` & `fastkafka-0.8.0rc0/fastkafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastkafka
-Version: 0.7.0rc2
+Version: 0.8.0rc0
 Summary: FastKafka is a powerful and easy-to-use Python library for building asynchronous web services that interact with Kafka topics. Built on top of FastAPI, Starlette, Pydantic, AIOKafka and AsyncAPI, FastKafka simplifies the process of writing producers and consumers for Kafka topics.
 Home-page: https://github.com/airtai/fastkafka
 Author: airt
 Author-email: info@airt.ai
 License: Apache Software License 2.0
 Project-URL: Bug Tracker, https://github.com/airtai/fastkafka/issues
 Project-URL: CI, https://github.com/airtai/fastkafka/actions
@@ -81,15 +81,15 @@
 
 #### 🐝🐝🐝 We were busy lately 🐝🐝🐝
 
 ![Activity](https://repobeats.axiom.co/api/embed/21f36049093d5eb8e5fdad18c3c5d8df5428ca30.svg "Repobeats analytics image")
 
 ## Install
 
-FastKafka works on macOS, Linux, and most Unix-style operating systems.
+FastKafka works on Windows, macOS, Linux, and most Unix-style operating systems.
 You can install base version of `fastkafka` with `pip` as usual:
 
 ``` sh
 pip install fastkafka
 ```
 
 To install fastkafka with testing features please use:
@@ -250,15 +250,15 @@
     processed_data = Data(data=data+1.0)
     return processed_data
 ```
 
 ## Testing the service
 
 The service can be tested using the
-[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester#fastkafka.testing.Tester)
+[`Tester`](https://fastkafka.airt.ai/docs/api/fastkafka/testing/Tester)
 instances which internally starts InMemory implementation of Kafka
 broker.
 
 The Tester will redirect your consumes and produces decorated functions
 to the InMemory Kafka broker so that you can quickly test your app
 without the need for a running Kafka broker and all its dependencies.
 
@@ -384,15 +384,17 @@
     return processed_data
 ```
 
 To run the service, use the FastKafka CLI command and pass the module
 (in this case, the file where the app implementation is located) and the
 app simbol to the command.
 
-`shell fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app`
+``` sh
+fastkafka run --num-workers=1 --kafka-broker localhost application:kafka_app
+```
 
 After running the command, you should see the following output in your
 command line:
 
     [1504]: 23-05-31 11:36:45.874 [INFO] fastkafka._application.app: set_kafka_broker() : Setting bootstrap_servers value to 'localhost:9092'
     [1504]: 23-05-31 11:36:45.875 [INFO] fastkafka._application.app: _create_producer() : created producer using the config: '{'bootstrap_servers': 'localhost:9092'}'
     [1504]: 23-05-31 11:36:45.937 [INFO] fastkafka._components.aiokafka_consumer_loop: aiokafka_consumer_loop() starting...
```

### Comparing `fastkafka-0.7.0rc2/fastkafka.egg-info/SOURCES.txt` & `fastkafka-0.8.0rc0/fastkafka.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
 fastkafka/__init__.py
+fastkafka/_aiokafka_imports.py
 fastkafka/_cli.py
 fastkafka/_cli_docs.py
 fastkafka/_cli_testing.py
 fastkafka/_docusaurus_helper.py
 fastkafka/_helpers.py
 fastkafka/_modidx.py
 fastkafka/_server.py
```

### Comparing `fastkafka-0.7.0rc2/fastkafka.egg-info/requires.txt` & `fastkafka-0.8.0rc0/fastkafka.egg-info/requires.txt`

 * *Files 21% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 fastavro>=1.7.3
 install-jdk==0.3.0
 ipython<8.13
 ipywidgets<=8.0.4,>=8.0
 isort==5.12.0
 mypy==1.3.0
 nbconvert>=7.2.9
-nbdev-mkdocs==0.5.0
+nbdev-mkdocs==0.6.0
 nbformat>=5.7.3
 nbqa==1.6.3
 numpy>=1.21.0
 pandas>=1.2.0
 pre-commit==3.3.1
 pytest==7.3.1
 requests>=2.20
```

### Comparing `fastkafka-0.7.0rc2/settings.ini` & `fastkafka-0.8.0rc0/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = fastkafka
 lib_name = %(repo)s
-version = 0.7.0rc2
+version = 0.8.0rc0
 min_python = 3.8
 license = apache2
 
 
 ### nbdev ###
 doc_path = _docs
 lib_path = fastkafka
```

### Comparing `fastkafka-0.7.0rc2/setup.py` & `fastkafka-0.8.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 
 dev_requirements = [
     "nbconvert>=7.2.9",
     "nbformat>=5.7.3",
-    "nbdev-mkdocs==0.5.0",
+    "nbdev-mkdocs==0.6.0",
     "mypy==1.3.0",
     "pre-commit==3.3.1",
     "nbqa==1.6.3",
     "black==23.3.0",
     "isort==5.12.0",
     "bandit==1.7.5",
     "semgrep==1.21.0",
```

