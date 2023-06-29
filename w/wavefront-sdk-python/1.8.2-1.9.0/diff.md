# Comparing `tmp/wavefront-sdk-python-1.8.2.tar.gz` & `tmp/wavefront-sdk-python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wavefront-sdk-python-1.8.2.tar", last modified: Mon Nov 29 21:14:47 2021, max compression
+gzip compressed data, was "wavefront-sdk-python-1.9.0.tar", last modified: Thu Jun 29 17:20:44 2023, max compression
```

## Comparing `wavefront-sdk-python-1.8.2.tar` & `wavefront-sdk-python-1.9.0.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.029503 wavefront-sdk-python-1.8.2/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11342 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)    24387 2021-11-29 21:14:47.029503 wavefront-sdk-python-1.8.2/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)    23765 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-11-29 21:14:47.029503 wavefront-sdk-python-1.8.2/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1335 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.021498 wavefront-sdk-python-1.8.2/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)       74 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2214 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/test_applicaiton_tags.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7960 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/test_histogram_impl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2885 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/test_wavefront_client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3201 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/test_wavefront_metrics_registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13137 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/test/test_wavefront_python_sdk.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.021498 wavefront-sdk-python-1.8.2/wavefront_sdk/
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22517 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2847 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/client_factory.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)      603 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3194 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/application_tags.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      704 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/connection_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1434 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/constants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3687 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/heartbeater_service.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      854 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/counter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      239 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/deltacounter.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      512 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/gauge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      189 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3975 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2523 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/proxy_connection_handler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16080 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/common/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25923 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/direct.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/
--rw-rw-r--   0 travis    (2000) travis    (2000)      604 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/event/
--rw-rw-r--   0 travis    (2000) travis    (2000)       73 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/event/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1479 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/event/sender.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      121 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/histogram_granularity.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13016 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/histogram_impl.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1765 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/sender.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/metrics/
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/metrics/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2245 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/metrics/sender.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/tracing/
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/tracing/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2441 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/tracing/sender.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      469 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/entities/tracing/span_log.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7858 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/multi_clients.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19368 2021-11-29 21:13:55.000000 wavefront-sdk-python-1.8.2/wavefront_sdk/proxy.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-11-29 21:14:47.025500 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24387 2021-11-29 21:14:46.000000 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1626 2021-11-29 21:14:46.000000 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-11-29 21:14:46.000000 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       51 2021-11-29 21:14:46.000000 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2021-11-29 21:14:46.000000 wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23728 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.239710 wavefront-sdk-python-1.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_applicaiton_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7960 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_histogram_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_metrics_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13137 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/test/test_wavefront_python_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/application_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/heartbeater_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/deltacounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/proxy_connection_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26131 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/direct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.243710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_granularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/span_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7858 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/multi_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19412 2023-06-29 17:20:06.000000 wavefront-sdk-python-1.9.0/wavefront_sdk/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 17:20:44.247710 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25008 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 17:20:44.000000 wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/top_level.txt
```

### Comparing `wavefront-sdk-python-1.8.2/LICENSE` & `wavefront-sdk-python-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/PKG-INFO` & `wavefront-sdk-python-1.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,88 +1,77 @@
 Metadata-Version: 2.1
 Name: wavefront-sdk-python
-Version: 1.8.2
-Summary: Wavefront Python SDK
+Version: 1.9.0
+Summary: VMware Aria Operations for Applications Python SDK
 Home-page: https://github.com/wavefrontHQ/wavefront-sdk-python
-Author: Wavefront by VMware
-Author-email: chitimba@wavefront.com
+Author: VMware Aria Operations for Applications Team
 License: Apache-2.0
-Keywords: Wavefront,Wavefront SDK
-Platform: UNKNOWN
+Keywords: Aria,Aria Operations,Aria Operations for Applications,3D Observability,Distributed Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware Aria,VMware Aria Operations,VMware Aria Operations for Applications,Wavefront,Wavefront SDK
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking :: Monitoring
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wavefront-sdk-python
 
-[![travis build status](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python)
+[![Build Status](https://github.com/wavefrontHQ/wavefront-sdk-python/actions/workflows/main.yml/badge.svg)](https://github.com/wavefrontHQ/wavefront-sdk-python/actions)
 [![image](https://img.shields.io/pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/pyversions/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/wavefront-sdk-python)
 
 
 ## Table of Content
 * [Prerequisites](#Prerequisites)
-* [Set Up a Wavefront Sender](#set-up-a-wavefront-sender)
-* [Send a Single Data Point to Wavefront](#send-a-single-data-point-to-wavefront)
-* [Send Batch Data to Wavefront](#send-batch-data-to-wavefront)
+* [Set Up a Sender](#set-up-a-sender)
+* [Send a Single Data Point](#send-a-single-data-point)
+* [Send Batch Data](#send-batch-data)
 * [Get the Failure Count](#get-the-failure-count)
 * [Close the Connection](#close-the-connection)
 * [License](#License)
 * [How to Get Support and Contribute](#how-to-get-support-and-contribute)
+* [How to Release](#how-to-release)
 
-# Welcome to the Wavefront Python SDK
+# VMware Aria Operations™ for Applications Python SDK
 
-Wavefront by VMware Python SDK lets you send raw data from your Python application to Wavefront using a `wavefront_sender` interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python. 
+VMware Aria Operations for Applications (formerly known as Wavefront) Python SDK lets you send raw data from your Python application to Operations for Applications using a wavefront_sender interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python.
 
-Although this library is mostly used by the other Wavefront Python SDKs to send data to Wavefront, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Wavefront.
+Although this library is mostly used by the other Operations for Applications Python SDKs to send data to Operations for Applications, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Operations for Applications.
+
+Note: We're in the process of updating the product name to Operations for Applications, but in many places we still refer to it as Wavefront.
 
 **Before you start implementing, let us make sure you are using the correct SDK!**
 
 ![Python Sender SDK Decision Tree](docs/python_sender_sdk.png)
 
 > ***Note***:
 > </br>
->   * **This is the Wavefront by VMware SDK for Python (Wavefront Sender SDK for Python)!**
+>   * **This is the VMware Aria Operations for Applications SDK for Python (Sender SDK for Python)!**
 >   If this SDK is not what you were looking for, see the [table](#wavefront-sdks) below.
 
-#### Wavefront SDKs
+#### VMware Aria Operations for Applications SDKs
 <table id="SDKlevels" style="width: 100%">
 <tr>
   <th width="10%">SDK Type</th>
   <th width="45%">SDK Description</th>
   <th width="45%">Supported Languages</th>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-trace-data">OpenTracing SDK</a></td>
-  <td align="justify">Implements the OpenTracing specification. Lets you define, collect, and report custom trace data from any part of your application code. <br>Automatically derives Rate Errors Duration (RED) metrics from the reported spans. </td>
-  <td>
-    <ul>
-    <li>
-      <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-java">OpenTracing SDK</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-bundle-java">Tracing Agent</a>
-    </li>
-    <li>
-      <b>Python</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-python">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>Go</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-go">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-csharp">OpenTracing SDK</a>
-    </li>
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-metrics-and-histograms">Metrics SDK</a></td>
   <td align="justify">Implements a standard metrics library. Lets you define, collect, and report custom business metrics and histograms from any part of your application code.   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-dropwizard-metrics-sdk-java">Dropwizard</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-runtime-sdk-jvm">JVM</a>
     </li>
@@ -96,30 +85,16 @@
     <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-appmetrics-sdk-csharp">App Metrics SDK</a>
     </li>
     </ul>
   </td>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-that-instrument-frameworks">Framework SDK</a></td>
-  <td align="justify">Reports predefined traces, metrics, and histograms from the APIs of a supported app framework. Lets you get started quickly with minimal code changes.</td>
-  <td>
-    <ul>
-    <li><b>Java</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-dropwizard-sdk-java">Dropwizard</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-gRPC-sdk-java">gRPC</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jaxrs-sdk-java">JAX-RS</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jersey-sdk-java">Jersey</a></li>
-    <li><b>.Net/C#</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-aspnetcore-sdk-csharp">ASP.Net core</a> </li>
-    <!--- [Python](wavefront_sdks_python.html#python-sdks-that-instrument-frameworks) --->
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-sending-raw-data-to-wavefront">Sender SDK</a></td>
-  <td align="justify">Lets you send raw data to Wavefront for storage as metrics, histograms, or traces, e.g., to import CSV data into Wavefront.
+  <td align="justify">Lets you send raw data for storage as metrics, histograms, or traces, e.g., to import CSV data into the service.
   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-sdk-java">Sender SDK</a>
     </li>
     <li>
@@ -139,59 +114,59 @@
 </tr>
 
 </tbody>
 </table>
 
 ## Prerequisites
 
-* Python ~~2.7+~~ and Python 3.x are supported.
+* Python versions 3.7 - 3.11 are supported.
 * Install `wavefront-sdk-python`
     ```
     pip install wavefront-sdk-python
     ```
 
-## Set Up a Wavefront Sender
+## Set Up a Sender
 
-You can send metrics, histograms, or trace data from your application to the Wavefront service using a Wavefront proxy or direct ingestions.
+You can send metrics, histograms, or trace data from your application to the service using a Wavefront Proxy or direct ingestions.
 
-* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the Wavefront service. This is the simplest way to get up and running quickly.
-* Use a [**Wavefront proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the Wavefront service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
+* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the service. This is the simplest way to get up and running quickly.
+* Use a [**Wavefront Proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
 
 You instantiate an object that corresponds to your choice:
 * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront service.
-* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy.
-* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to a Wavefront service directly or via proxy.
+* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront Proxy.
+* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the service directly or via proxy.
 > **Deprecated implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy version 7.0 onwards. We recommend all new applications to use the `WavefrontClient`.*
 
 ### Option 1: Create a WavefrontDirectClient
-When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the Wavefront URL and API token to send data directly to Wavefront.
+When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the cluster URL and API token to send data directly to the service.
 
 >**Prerequisites**
 > * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-> * The URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `https://<domain>.wavefront.com`.
+> * The URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `https://<domain>.wavefront.com`.
 > * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 #### Initialize the WavefrontDirectClient
 You initialize a `WavefrontDirectClient` by providing the access information you obtained in the Prerequisites section..
 
 Optionally, you can specify parameters to tune the following ingestion properties:
 
-* Max queue size - Internal buffer capacity of the Wavefront sender. Any data in excess of this size is dropped.
-* Flush interval - Interval for flushing data from the Wavefront sender directly to Wavefront.
-* Batch size - Amount of data to send to Wavefront in each flush interval.
+* Max queue size - Internal buffer capacity of the sender. Any data in excess of this size is dropped.
+* Flush interval - Interval for flushing data from the sender directly to the service.
+* Batch size - Amount of data to send to the service in each flush interval.
 
-Together, the batch size and flush interval control the maximum theoretical throughput of the Wavefront sender. You should override the defaults _only_ to set higher values.
+Together, the batch size and flush interval control the maximum theoretical throughput of the sender. You should override the defaults _only_ to set higher values.
 
 
 ```python
 from wavefront_sdk import WavefrontDirectClient
 
 # Create a sender with:
-   # your Wavefront URL
-   # a Wavefront API token that was created with direct ingestion permission
+   # your cluster URL
+   # an API token that was created with direct ingestion permission
    # max queue size (in data points). Default: 50,000
    # batch size (in data points). Default: 10,000
    # flush interval  (in seconds). Default: 1 second
 wavefront_sender = WavefrontDirectClient(
     server="<SERVER_ADDR>",
     token="<TOKEN>",
     max_queue_size=50000,
@@ -201,17 +176,17 @@
 ```
 
 ### Option 2: Create a WavefrontProxyClient
 
 >**Prerequisite** <br/>
 >Before your application can use a `WavefrontProxyClient`, you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
 
-When sending data via the Wavefront proxy, you need to create a `WavefrontProxyClient`. Include the following information.
+When sending data via the Wavefront Proxy, you need to create a `WavefrontProxyClient`. Include the following information.
 
-* The name of the host that will run the Wavefront proxy.
+* The name of the host that will run the Wavefront Proxy.
 * One or more proxy listening ports to send data to. The ports you specify depend on the kinds of data you want to send (metrics, histograms, and/or trace data). You must specify at least one listener port.
 * Optional settings for tuning communication with the proxy.
 
 > **Note**: See [Advanced Proxy Configuration and Installation](https://docs.wavefront.com/proxies_configuring.html) for details.
 
 ```python
 from wavefront_sdk import WavefrontProxyClient
@@ -227,32 +202,32 @@
    metrics_port=2878,
    distribution_port=2878,
    tracing_port=30000,
    event_port=2878
 )
 ```
 
-> **Note:** When you set up a Wavefront proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
+> **Note:** When you set up a Wavefront Proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront Proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
 
 | `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf` |
 | ----- | -------- |
 | `metrics_port` | `pushListenerPorts=` |
 | `distribution_port` | `histogramDistListenerPorts=` |
 | `tracing_port` | `traceListenerPorts=` |
 
 ### Option 3: Create a WavefrontClient
-Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to a Wavefront service or send data using a Wavefront Proxy.
+Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to the service or send data using a Wavefront Proxy.
 
-The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple Wavefront services.
+The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple services.
 ### Prerequisites
-* Sending data via Wavefront proxy?
-  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
+* Sending data via Wavefront Proxy?
+  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html).
 * Sending data via direct ingestion?
   * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-  * The HTTP URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
+  * The HTTP URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
   * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 ### Initialize the WavefrontClient
 ```python
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 # Create a sender with:
@@ -268,48 +243,53 @@
 client_factory.add_client(
     url="<URL for proxy or direct ingestions>",
     max_queue_size=50000,
     batch_size=10000,
     flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client()
 ```
-#### Add multiple clients to client factory to send data to multiple Wavefront services.
+#### Add multiple clients to client factory to send data to multiple services.
 ```
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 client_factory = WavefrontClientFactory()
 client_factory.add_client("proxy://our.proxy.lb.com:2878")
 client_factory.add_client("https://someToken@DOMAIN.wavefront.com")
 
 # Send traces and spans to the tracing port. If you are directly using the sender SDK to send spans without using any other SDK, use the same port as the customTracingListenerPorts configured in the wavefront proxy. Assume you have installed and started the proxy on <proxy_hostname>.
 client_factory.add_client("http://<proxy_hostname>:30000")
 
 wavefront_sender = client_factory.get_client()
 ```
 
-## Send a Single Data Point to Wavefront
+## Send a Single Data Point
 
-The following examples show how to send a single data point to Wavefront. You use the Wavefront sender you created above.
+The following examples show how to send a single data point to the service. You use the Wavefront Sender you created above.
 
 ### Single Metric or  Delta Counter
 
 ```python
 from uuid import UUID
 
 # Wavefront metrics data format:
 # <metricName> <metricValue> [<timestamp>] source=<source> [pointTags]
 wavefront_sender.send_metric(
-    name="new york.power.usage", value=42422.0, timestamp=1533529977,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="new_york.power.usage",
+    value=42422.0,
+    timestamp=1533529977,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 
 # Wavefront delta counter data format:
 # <metricName> <metricValue> source=<source> [pointTags]
 wavefront_sender.send_delta_counter(
-    name="delta.counter", value=1.0,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="delta.counter",
+    value=1.0,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 ```
 ***Note***: If your metric name has a bad character, that character is replaced with a `-`.
 
 ### Single Histogram Distribution
 
 ```python
 from uuid import UUID
@@ -318,71 +298,87 @@
 # Wavefront histogram data format:
 # {!M | !H | !D} [<timestamp>] #<count> <mean> [centroids] <histogramName> source=<source> [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day
 # "!M 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 wavefront_sender.send_distribution(
-    name="request.latency", centroids=[(30, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.DAY,
                              histogram_granularity.HOUR,
                              histogram_granularity.MINUTE},
-    timestamp=1533529977, source="appServer1", tags={"region": "us-west"})
+    timestamp=1533529977,
+    source="appServer1",
+    tags={"region": "us-west"})
 ```
 
 ### Single Span
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with the Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 
 # Wavefront trace and span data format:
 # <tracingSpanName> source=<source> [pointTags] <start_millis> <duration_milliseconds>
 # Example: "getAllUsers source=localhost
 #           traceId=7b3bf470-9456-11e8-9eb6-529269fb1459
 #           spanId=0313bafe-9457-11e8-9eb6-529269fb1459
 #           parent=2f64e538-9457-11e8-9eb6-529269fb1459
 #           application=Wavefront http.method=GET
 #           1533529977 343500"
 wavefront_sender.send_span(
-    name="getAllUsers", start_millis=1533529977, duration_millis=343500,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1533529977,
+    duration_millis=343500,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
-    follows_from=None, tags=[("application", "Wavefront"),
-                             ("service", "istio"),
-                             ("http.method", "GET")],
+    follows_from=None,
+    tags=[("application", "Wavefront"),
+          ("service", "istio"),
+          ("http.method", "GET")],
     span_logs=None)
 ```
 
 ### Single Event
 
 ```python
 # Wavefront event format:
 # @Event <StartTime> <EndTime> "<EventName>"  severity="<Severity>"
 # type="<Type>" details="<EventDetail>" host="<Source>" tag="<Tags>"
-wavefront_sender.send_event('event name', 1592200048, 1592201048, "localhost",
-    ["env:", "dev"], {"severity": "info", "type": "backup", "details": "broker backup"})
+wavefront_sender.send_event('event name',
+                            1592200048,
+                            1592201048,
+                            "localhost",
+                            ["env:", "dev"],
+                            {"severity": "info",
+                             "type": "backup",
+                             "details": "broker backup"})
 ```
 
-## Send Batch Data to Wavefront
+## Send Batch Data
 
 The following examples show how to generate data points manually and send them as a batch to Wavefront.
 
 ### Batch Metrics
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import metric_to_line_data
 
 # Generate string data in Wavefront metric format
 one_metric_data = metric_to_line_data(
-    name="new-york.power.usage", value=42422, timestamp=1493773500,
-    source="localhost", tags={"datacenter": "dc1"},
+    name="new-york.power.usage",
+    value=42422,
+    timestamp=1493773500,
+    source="localhost",
+    tags={"datacenter": "dc1"},
     default_source="defaultSource")
 
 # Result of one_metric_data:
   # '"new-york.power.usage" 42422.0 1493773500 source="localhost" "datacenter"="dc1"\n'
 
 # List of data
 batch_metric_data = [one_metric_data, one_metric_data]
@@ -397,19 +393,22 @@
 ```python
 from uuid import UUID
 from wavefront_sdk.entities.histogram import histogram_granularity
 from wavefront_sdk.common import histogram_to_line_data
 
 # Generate string data in Wavefront histogram format
 one_histogram_data = histogram_to_line_data(
-    name="request.latency", centroids=[(30.0, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30.0, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.MINUTE,
                              histogram_granularity.HOUR,
                              histogram_granularity.DAY},
-    timestamp=1493773500, source="appServer1", tags={"region": "us-west"},
+    timestamp=1493773500,
+    source="appServer1",
+    tags={"region": "us-west"},
     default_source ="defaultSource")
 
 # Result of one_histogram_data:
   # '!D 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !H 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n'
 
@@ -417,29 +416,33 @@
 batch_histogram_data = [one_histogram_data, one_histogram_data]
 
 # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data)
 ```
 ### Batch Trace Data
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import tracing_span_to_line_data
 
 # Generate string data in Wavefront tracing span format
 one_tracing_span_data = tracing_span_to_line_data(
-    name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1552949776000,
+    duration_millis=343,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
     follows_from=[UUID("5f64e538-9457-11e8-9eb6-529269fb1459")],
     tags=[("application", "Wavefront"), ("http.method", "GET")],
-    span_logs=None, default_source="defaultSource")
+    span_logs=None,
+    default_source="defaultSource")
 
 # Result of one_tracing_span_data:
   # '"getAllUsers" source="localhost" traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe-
   # 9457-11e8-9eb6-529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
   # 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000 343\n'
 
 # List of data
@@ -451,16 +454,23 @@
 
 ### Batch Events
 
 ```python
 from wavefront_sdk.common import event_to_line_data
 
 # Generate string data in Wavefront event format
-one_event_data = event_to_line_data(name="event name", start_time=1592200048, end_time=1592201048,
- source="localhost", tags=["env", "dev"], annotations={"severity": "info", "type": "backup", "details": "broker backup"})
+one_event_data = event_to_line_data(
+    name="event name",
+    start_time=1592200048,
+    end_time=1592201048,
+    source="localhost",
+    tags=["env", "dev"],
+    annotations={"severity": "info",
+                 "type": "backup",
+                 "details": "broker backup"})
 
 # Result of one_event_data:
 # '@Event 1592200048 1592201048 "event name" severity="info" type="backup" details="broker backup"
 # host="localhost" tag="env" tag="dev"\n'
 
 # List of events
 batch_event_data = [one_event_data, one_event_data]
@@ -475,34 +485,34 @@
 
 ```python
 # Get the total failure count
 total_failures = wavefront_sender.get_failure_count()
 ```
 ## Close the Connection
 
-* If the Wavefront sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
+* If the sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
 
     ```python
     # To shut down a sender from a WavefrontClientFactory
     wavefront_sender = client_factory.get_client()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
+* If the sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontDirectClient
     # Flush all buffers.
     wavefront_sender.flush_now()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
+* If the sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontProxyClient
 
     # Close the sender connection
     wavefront_sender.close()
     ```
@@ -518,8 +528,24 @@
   (last number). For backward compatible changes to the API, update the
   minor version (second number), and zero out the patch version. For breaking
   changes to the API, increment the major version (first number) and zero out
   the minor and patch versions.
 * Reach out to us on our public [Slack channel](https://www.wavefront.com/join-public-slack).
 * If you run into any issues, let us know by creating a GitHub issue.
 
+## How to Release
 
+1. Merge all the changes that need to go into the release to the master branch.
+2. Open the `setup.py` file from the top level directory of the project.
+3. Search for version= in the file to find the version number, for example 1.8.15.
+4. Create a pull request, get it reviewed and approved, and merge it after approval.
+5. Check [test.pypi.org](https://test.pypi.org/project/wavefront-sdk-python) for a published package, make sure it's production ready.
+6. Log in to GitHub, click Releases on the right, and click Draft a new release.
+7. For **Choose a tag**, choose the version you found in step 3, and prefix it with `v` for example `v1.8.15`. You need to enter the version where it says **Find or create new tag**.
+
+<img src="images/choose-version.png" alt="A diagram that shows how to choose version"/>
+
+8. Provide a short but descriptive title for the release.
+9. Fill in the details of the release. Please copy the markdown from the previous release and follow the same format.
+10. Click **Publish release.** to start publishing the release to pypi.org.
+11. From the GitHub top navigation bar of this project, click the **Actions** tab. On the first line of the list of workflows, you should see a workflow running that will publish your release to pypi.org.
+12. When the workflow from step 9 has a green checkmark next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/) and verify that the latest version is published.
```

#### html2text {}

```diff
@@ -1,218 +1,216 @@
-Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.8.2 Summary:
-Wavefront Python SDK Home-page: https://github.com/wavefrontHQ/wavefront-sdk-
-python Author: Wavefront by VMware Author-email: chitimba@wavefront.com
-License: Apache-2.0 Keywords: Wavefront,Wavefront SDK Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 2.7 Classifier: Programming Language ::
-Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # wavefront-sdk-python [![travis build status](https://
-travis-ci.com/wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://
-travis-ci.com/wavefrontHQ/wavefront-sdk-python) [![image](https://
-img.shields.io/pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/
-wavefront-sdk-python/) [![image](https://img.shields.io/pypi/l/wavefront-sdk-
+Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.9.0 Summary: VMware
+Aria Operations for Applications Python SDK Home-page: https://github.com/
+wavefrontHQ/wavefront-sdk-python Author: VMware Aria Operations for
+Applications Team License: Apache-2.0 Keywords: Aria,Aria Operations,Aria
+Operations for Applications,3D Observability,Distributed
+Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware
+Aria,VMware Aria Operations,VMware Aria Operations for
+Applications,Wavefront,Wavefront SDK Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Information Technology Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: System ::
+Monitoring Classifier: Topic :: System :: Networking :: Monitoring Description-
+Content-Type: text/markdown License-File: LICENSE # wavefront-sdk-python [!
+[Build Status](https://github.com/wavefrontHQ/wavefront-sdk-python/actions/
+workflows/main.yml/badge.svg)](https://github.com/wavefrontHQ/wavefront-sdk-
+python/actions) [![image](https://img.shields.io/pypi/v/wavefront-sdk-
 python.svg)](https://pypi.org/project/wavefront-sdk-python/) [![image](https://
-img.shields.io/pypi/pyversions/wavefront-sdk-python.svg)](https://pypi.org/
-project/wavefront-sdk-python/) ## Table of Content * [Prerequisites]
-(#Prerequisites) * [Set Up a Wavefront Sender](#set-up-a-wavefront-sender) *
-[Send a Single Data Point to Wavefront](#send-a-single-data-point-to-wavefront)
-* [Send Batch Data to Wavefront](#send-batch-data-to-wavefront) * [Get the
-Failure Count](#get-the-failure-count) * [Close the Connection](#close-the-
-connection) * [License](#License) * [How to Get Support and Contribute](#how-
-to-get-support-and-contribute) # Welcome to the Wavefront Python SDK Wavefront
-by VMware Python SDK lets you send raw data from your Python application to
-Wavefront using a `wavefront_sender` interface. The data is then stored as
+img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://pypi.org/project/
+wavefront-sdk-python/) [![image](https://img.shields.io/pypi/pyversions/
+wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/) !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/wavefront-sdk-python) ##
+Table of Content * [Prerequisites](#Prerequisites) * [Set Up a Sender](#set-up-
+a-sender) * [Send a Single Data Point](#send-a-single-data-point) * [Send Batch
+Data](#send-batch-data) * [Get the Failure Count](#get-the-failure-count) *
+[Close the Connection](#close-the-connection) * [License](#License) * [How to
+Get Support and Contribute](#how-to-get-support-and-contribute) * [How to
+Release](#how-to-release) # VMware Aria Operationsâ¢ for Applications Python
+SDK VMware Aria Operations for Applications (formerly known as Wavefront)
+Python SDK lets you send raw data from your Python application to Operations
+for Applications using a wavefront_sender interface. The data is then stored as
 metrics, histograms, and trace data. This SDK is also referred to as the
 Wavefront Sender SDK for Python. Although this library is mostly used by the
-other Wavefront Python SDKs to send data to Wavefront, you can also use this
-SDK directly. For example, you can send data directly from a data store or CSV
-file to Wavefront. **Before you start implementing, let us make sure you are
-using the correct SDK!** ![Python Sender SDK Decision Tree](docs/
-python_sender_sdk.png) > ***Note***: >  > * **This is the Wavefront by VMware
-SDK for Python (Wavefront Sender SDK for Python)!** > If this SDK is not what
-you were looking for, see the [table](#wavefront-sdks) below. #### Wavefront
-SDKs
-SDK Type        SDK Description                 Supported Languages
-                Implements the OpenTracing
-                specification. Lets you define,     * Java: OpenTracing_SDK |
-                collect, and report custom            Tracing_Agent
-OpenTracing_SDK trace data from any part of         * Python: OpenTracing_SDK
-                your application code.              * Go: OpenTracing_SDK
-                Automatically derives Rate          * .Net/C#: OpenTracing_SDK
-                Errors Duration (RED) metrics
-                from the reported spans.
-                Implements a standard metrics
-                library. Lets you define,           * Java: Dropwizard | JVM
-Metrics_SDK     collect, and report custom          * Python: Pyformance_SDK
-                business metrics and histograms     * Go: Go_Metrics_SDK
-                from any part of your               * .Net/C#: App_Metrics_SDK
-                application code.
-                Reports predefined traces,
-                metrics, and histograms from        * Java: Dropwizard | gRPC |
-Framework_SDK   the APIs of a supported app           JAX-RS | Jersey
-                framework. Lets you get started     * .Net/C#: ASP.Net_core
-                quickly with minimal code
-                changes.
-                Lets you send raw data to           * Java: Sender_SDK
-                Wavefront for storage as            * Python: Sender_SDK
-Sender_SDK      metrics, histograms, or traces,     * Go: Sender_SDK
-                e.g., to import CSV data into       * .Net/C#: Sender_SDK
-                Wavefront.                          * C++: Sender_SDK
-## Prerequisites * Python ~~2.7+~~ and Python 3.x are supported. * Install
+other Operations for Applications Python SDKs to send data to Operations for
+Applications, you can also use this SDK directly. For example, you can send
+data directly from a data store or CSV file to Operations for Applications.
+Note: We're in the process of updating the product name to Operations for
+Applications, but in many places we still refer to it as Wavefront. **Before
+you start implementing, let us make sure you are using the correct SDK!** !
+[Python Sender SDK Decision Tree](docs/python_sender_sdk.png) > ***Note***: >
+> * **This is the VMware Aria Operations for Applications SDK for Python
+(Sender SDK for Python)!** > If this SDK is not what you were looking for, see
+the [table](#wavefront-sdks) below. #### VMware Aria Operations for
+Applications SDKs
+SDK Type    SDK Description                      Supported Languages
+            Implements a standard metrics            * Java: Dropwizard | JVM
+            library. Lets you define, collect,       * Python: Pyformance_SDK
+Metrics_SDK and report custom business metrics       * Go: Go_Metrics_SDK
+            and histograms from any part of your     * .Net/C#: App_Metrics_SDK
+            application code.
+            Lets you send raw data for storage       * Java: Sender_SDK
+            as metrics, histograms, or traces,       * Python: Sender_SDK
+Sender_SDK  e.g., to import CSV data into the        * Go: Sender_SDK
+            service.                                 * .Net/C#: Sender_SDK
+                                                     * C++: Sender_SDK
+## Prerequisites * Python versions 3.7 - 3.11 are supported. * Install
 `wavefront-sdk-python` ``` pip install wavefront-sdk-python ``` ## Set Up a
-Wavefront Sender You can send metrics, histograms, or trace data from your
-application to the Wavefront service using a Wavefront proxy or direct
-ingestions. * Use [**direct ingestion**](https://docs.wavefront.com/
-direct_ingestion.html) to send the data directly to the Wavefront service. This
-is the simplest way to get up and running quickly. * Use a [**Wavefront
-proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data
-to the Wavefront service. This is the recommended choice for a large-scale
-deployment that needs resilience to internet outages, control over data queuing
-and filtering, and more. You instantiate an object that corresponds to your
-choice: * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`]
-(#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront
-service. * Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`]
-(#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy. *
-Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to
-send data to a Wavefront service directly or via proxy. > **Deprecated
-implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are
-deprecated from proxy version 7.0 onwards. We recommend all new applications to
-use the `WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When
-sending data via direct ingestion, you need to create a
-`WavefrontDirectClient`, and build it with the Wavefront URL and API token to
-send data directly to Wavefront. >**Prerequisites** > * Verify that you have
-the Direct Data Ingestion permission. For details, see [Examine Groups, Roles,
-and Permissions](https://docs.wavefront.com/
-users_account_managing.html#examine-groups-roles-and-permissions). > * The URL
-of your Wavefront instance. This is the URL you connect to when you log in to
-Wavefront, typically something like `https://.wavefront.com`. > * [Obtain the
-API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-
-token). #### Initialize the WavefrontDirectClient You initialize a
-`WavefrontDirectClient` by providing the access information you obtained in the
-Prerequisites section.. Optionally, you can specify parameters to tune the
-following ingestion properties: * Max queue size - Internal buffer capacity of
-the Wavefront sender. Any data in excess of this size is dropped. * Flush
-interval - Interval for flushing data from the Wavefront sender directly to
-Wavefront. * Batch size - Amount of data to send to Wavefront in each flush
-interval. Together, the batch size and flush interval control the maximum
-theoretical throughput of the Wavefront sender. You should override the
-defaults _only_ to set higher values. ```python from wavefront_sdk import
-WavefrontDirectClient # Create a sender with: # your Wavefront URL # a
-Wavefront API token that was created with direct ingestion permission # max
-queue size (in data points). Default: 50,000 # batch size (in data points).
-Default: 10,000 # flush interval (in seconds). Default: 1 second
-wavefront_sender = WavefrontDirectClient( server="", token="",
-max_queue_size=50000, batch_size=10000, flush_interval_seconds=5 ) ``` ###
-Option 2: Create a WavefrontProxyClient >**Prerequisite**
+Sender You can send metrics, histograms, or trace data from your application to
+the service using a Wavefront Proxy or direct ingestions. * Use [**direct
+ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data
+directly to the service. This is the simplest way to get up and running
+quickly. * Use a [**Wavefront Proxy**](https://docs.wavefront.com/
+proxies.html), which then forwards the data to the service. This is the
+recommended choice for a large-scale deployment that needs resilience to
+internet outages, control over data queuing and filtering, and more. You
+instantiate an object that corresponds to your choice: * Option 1 **
+(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-
+wavefrontdirectclient) to send data directly to a Wavefront service. * Option 2
+**(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-
+wavefrontproxyclient) to send data to a Wavefront Proxy. * Option 3: [Create a
+`WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the
+service directly or via proxy. > **Deprecated implementations**:
+*`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy
+version 7.0 onwards. We recommend all new applications to use the
+`WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When sending
+data via direct ingestion, you need to create a `WavefrontDirectClient`, and
+build it with the cluster URL and API token to send data directly to the
+service. >**Prerequisites** > * Verify that you have the Direct Data Ingestion
+permission. For details, see [Examine Groups, Roles, and Permissions](https://
+docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-
+permissions). > * The URL of your cluster. This is the URL you connect to when
+you log in to the service, typically something like `https://.wavefront.com`. >
+* [Obtain the API token](http://docs.wavefront.com/
+wavefront_api.html#generating-an-api-token). #### Initialize the
+WavefrontDirectClient You initialize a `WavefrontDirectClient` by providing the
+access information you obtained in the Prerequisites section.. Optionally, you
+can specify parameters to tune the following ingestion properties: * Max queue
+size - Internal buffer capacity of the sender. Any data in excess of this size
+is dropped. * Flush interval - Interval for flushing data from the sender
+directly to the service. * Batch size - Amount of data to send to the service
+in each flush interval. Together, the batch size and flush interval control the
+maximum theoretical throughput of the sender. You should override the defaults
+_only_ to set higher values. ```python from wavefront_sdk import
+WavefrontDirectClient # Create a sender with: # your cluster URL # an API token
+that was created with direct ingestion permission # max queue size (in data
+points). Default: 50,000 # batch size (in data points). Default: 10,000 # flush
+interval (in seconds). Default: 1 second wavefront_sender =
+WavefrontDirectClient( server="", token="", max_queue_size=50000,
+batch_size=10000, flush_interval_seconds=5 ) ``` ### Option 2: Create a
+WavefrontProxyClient >**Prerequisite**
 >Before your application can use a `WavefrontProxyClient`, you must [set up and
 start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
-When sending data via the Wavefront proxy, you need to create a
+When sending data via the Wavefront Proxy, you need to create a
 `WavefrontProxyClient`. Include the following information. * The name of the
-host that will run the Wavefront proxy. * One or more proxy listening ports to
+host that will run the Wavefront Proxy. * One or more proxy listening ports to
 send data to. The ports you specify depend on the kinds of data you want to
 send (metrics, histograms, and/or trace data). You must specify at least one
 listener port. * Optional settings for tuning communication with the proxy. >
 **Note**: See [Advanced Proxy Configuration and Installation](https://
 docs.wavefront.com/proxies_configuring.html) for details. ```python from
 wavefront_sdk import WavefrontProxyClient # Create a sender with: # the proxy
 hostname or address # the default listener port (2878) for sending metrics to #
 the recommended listener port (2878) for sending histograms to # the
 recommended listener port (30000) for sending trace data. # if you are directly
 using the sender sdk to send spans without using any other sdk, use the same
 port as the customTracingListenerPorts configured in the wavefront proxy for
 the tracing_port wavefront_sender = WavefrontProxyClient( host="",
 metrics_port=2878, distribution_port=2878, tracing_port=30000, event_port=2878
-) ``` > **Note:** When you set up a Wavefront proxy on the specified proxy
+) ``` > **Note:** When you set up a Wavefront Proxy on the specified proxy
 host, you specify the port it will listen to for each type of data to be sent.
 The `WavefrontProxyClient` must send data to the same ports that the Wavefront
-proxy listens to. Consequently, the port-related parameters must specify the
+Proxy listens to. Consequently, the port-related parameters must specify the
 same port numbers as the corresponding proxy configuration properties: |
 `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf`
 | | ----- | -------- | | `metrics_port` | `pushListenerPorts=` | |
 `distribution_port` | `histogramDistListenerPorts=` | | `tracing_port` |
 `traceListenerPorts=` | ### Option 3: Create a WavefrontClient Use
 `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send
-data directly to a Wavefront service or send data using a Wavefront Proxy. The
+data directly to the service or send data using a Wavefront Proxy. The
 `WavefrontClientFactory` supports multiple client bindings. If more than one
 client configuration is specified, you can create a `WavefrontMultiClient`
-instance, which can send data to multiple Wavefront services. ### Prerequisites
-* Sending data via Wavefront proxy?
+instance, which can send data to multiple services. ### Prerequisites * Sending
+data via Wavefront Proxy?
 Before your application can use a `WavefrontClient` you must [set up and start
-a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html). *
+a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html). *
 Sending data via direct ingestion? * Verify that you have the Direct Data
 Ingestion permission. For details, see [Examine Groups, Roles, and Permissions]
 (https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-
-and-permissions). * The HTTP URL of your Wavefront instance. This is the URL
-you connect to when you log in to Wavefront, typically something like `http:/
+and-permissions). * The HTTP URL of your cluster. This is the URL you connect
+to when you log in to the service, typically something like `http:/
 /.wavefront.com`.
 You can also use HTTP client with Wavefront Proxy version 7.0 or newer.
 Example: `http://proxy.acme.corp:2878`. * [Obtain the API token](http://
 docs.wavefront.com/wavefront_api.html#generating-an-api-token). ### Initialize
 the WavefrontClient ```python from wavefront_sdk.client_factory import
 WavefrontClientFactory # Create a sender with: # Required Parameter # URL
 format to send data via proxy: "proxy://
 proxy.load.balancer.com>:" # URL format to send data via direct ingestion:
 "https://TOKEN@DOMAIN.wavefront.com" # Optional Parameter # max queue size (in
 data points). Default: 50000 # batch size (in data points). Default: 10000 #
 flush interval (in seconds). Default: 1 second client_factory =
 WavefrontClientFactory() client_factory.add_client( url="",
 max_queue_size=50000, batch_size=10000, flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client() ``` #### Add multiple clients to
-client factory to send data to multiple Wavefront services. ``` from
+client factory to send data to multiple services. ``` from
 wavefront_sdk.client_factory import WavefrontClientFactory client_factory =
 WavefrontClientFactory() client_factory.add_client("proxy://our.proxy.lb.com:
 2878") client_factory.add_client("https://someToken@DOMAIN.wavefront.com") #
 Send traces and spans to the tracing port. If you are directly using the sender
 SDK to send spans without using any other SDK, use the same port as the
 customTracingListenerPorts configured in the wavefront proxy. Assume you have
 installed and started the proxy on . client_factory.add_client("http://:30000")
 wavefront_sender = client_factory.get_client() ``` ## Send a Single Data Point
-to Wavefront The following examples show how to send a single data point to
-Wavefront. You use the Wavefront sender you created above. ### Single Metric or
-Delta Counter ```python from uuid import UUID # Wavefront metrics data format:
-#   [] source= [pointTags] wavefront_sender.send_metric( name="new
-york.power.usage", value=42422.0, timestamp=1533529977, source="localhost",
-tags={"datacenter": "dc1"}) # Wavefront delta counter data format: #   source=
-[pointTags] wavefront_sender.send_delta_counter( name="delta.counter",
-value=1.0, source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If
-your metric name has a bad character, that character is replaced with a `-`.
-### Single Histogram Distribution ```python from uuid import UUID from
+The following examples show how to send a single data point to the service. You
+use the Wavefront Sender you created above. ### Single Metric or Delta Counter
+```python from uuid import UUID # Wavefront metrics data format: #   [] source=
+[pointTags] wavefront_sender.send_metric( name="new_york.power.usage",
+value=42422.0, timestamp=1533529977, source="localhost", tags={"datacenter":
+"dc1"}) # Wavefront delta counter data format: #   source= [pointTags]
+wavefront_sender.send_delta_counter( name="delta.counter", value=1.0,
+source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If your metric
+name has a bad character, that character is replaced with a `-`. ### Single
+Histogram Distribution ```python from uuid import UUID from
 wavefront_sdk.entities.histogram import histogram_granularity # Wavefront
 histogram data format: # {!M | !H | !D} [] #  [centroids]  source= [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day # "!M
 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west" #
 "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-
 west" # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1
 region=us-west" wavefront_sender.send_distribution( name="request.latency",
 centroids=[(30, 20), (5.1, 10)], histogram_granularities=
 {histogram_granularity.DAY, histogram_granularity.HOUR,
 histogram_granularity.MINUTE}, timestamp=1533529977, source="appServer1", tags=
 {"region": "us-west"}) ``` ### Single Span If you are directly using the Sender
-SDK to send data to Wavefront, you wonât see span-level RED metrics by
-default unless you use the Wavefront proxy and define a custom tracing port
-(`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs]
-(https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-
-your-application-with-wavefront-sender-sdks) for details. ```python from uuid
-import UUID # Wavefront trace and span data format: #  source= [pointTags]   #
+SDK to send data to the service, you wonât see span-level RED metrics by
+default unless you use the Wavefront Proxy and define a custom tracing port
+(`tracing_port`). See [Instrument Your Application with the Sender SDKs](https:
+//docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID # Wavefront trace and span data format: #  source= [pointTags]   #
 Example: "getAllUsers source=localhost # traceId=7b3bf470-9456-11e8-9eb6-
 529269fb1459 # spanId=0313bafe-9457-11e8-9eb6-529269fb1459 # parent=2f64e538-
 9457-11e8-9eb6-529269fb1459 # application=Wavefront http.method=GET #
 1533529977 343500" wavefront_sender.send_span( name="getAllUsers",
 start_millis=1533529977, duration_millis=343500, source="localhost",
 trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"), span_id=UUID("0313bafe-
 9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-9457-11e8-9eb6-
 529269fb1459")], follows_from=None, tags=[("application", "Wavefront"),
 ("service", "istio"), ("http.method", "GET")], span_logs=None) ``` ### Single
 Event ```python # Wavefront event format: # @Event   "" severity="" # type=""
 details="" host="" tag="" wavefront_sender.send_event('event name', 1592200048,
 1592201048, "localhost", ["env:", "dev"], {"severity": "info", "type":
-"backup", "details": "broker backup"}) ``` ## Send Batch Data to Wavefront The
-following examples show how to generate data points manually and send them as a
-batch to Wavefront. ### Batch Metrics ```python from uuid import UUID from
+"backup", "details": "broker backup"}) ``` ## Send Batch Data The following
+examples show how to generate data points manually and send them as a batch to
+Wavefront. ### Batch Metrics ```python from uuid import UUID from
 wavefront_sdk.common import metric_to_line_data # Generate string data in
 Wavefront metric format one_metric_data = metric_to_line_data( name="new-
 york.power.usage", value=42422, timestamp=1493773500, source="localhost", tags=
 {"datacenter": "dc1"}, default_source="defaultSource") # Result of
 one_metric_data: # '"new-york.power.usage" 42422.0 1493773500
 source="localhost" "datacenter"="dc1"\n' # List of data batch_metric_data =
 [one_metric_data, one_metric_data] # Send list of data immediately
@@ -229,61 +227,79 @@
 ="defaultSource") # Result of one_histogram_data: # '!D 1493773500 #20 30.0 #10
 5.1 "request.latency" source="appServer1" "region"="us-west"\n # !H 1493773500
 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n #
 !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1"
 "region"="us-west"\n' # List of data batch_histogram_data =
 [one_histogram_data, one_histogram_data] # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data) ``` ### Batch
-Trace Data If you are directly using the Sender SDK to send data to Wavefront,
-you wonât see span-level RED metrics by default unless you use the Wavefront
-proxy and define a custom tracing port (`tracing_port`). See [Instrument Your
-Application with Wavefront Sender SDKs](https://docs.wavefront.com/
-tracing_instrumenting_frameworks.html#instrument-your-application-with-
-wavefront-sender-sdks) for details. ```python from uuid import UUID from
-wavefront_sdk.common import tracing_span_to_line_data # Generate string data in
-Wavefront tracing span format one_tracing_span_data = tracing_span_to_line_data
-( name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
-span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-
-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID("5f64e538-9457-11e8-9eb6-
-529269fb1459")], tags=[("application", "Wavefront"), ("http.method", "GET")],
-span_logs=None, default_source="defaultSource") # Result of
-one_tracing_span_data: # '"getAllUsers" source="localhost" traceId=7b3bf470-
-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-529269fb1459
-parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538- # 9457-11e8-
-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000
-343\n' # List of data batch_span_data = [one_tracing_span_data,
+Trace Data If you are directly using the Sender SDK to send data to the
+service, you wonât see span-level RED metrics by default unless you use the
+Wavefront Proxy and define a custom tracing port (`tracing_port`). See
+[Instrument Your Application with Wavefront Sender SDKs](https://
+docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID from wavefront_sdk.common import tracing_span_to_line_data # Generate
+string data in Wavefront tracing span format one_tracing_span_data =
+tracing_span_to_line_data( name="getAllUsers", start_millis=1552949776000,
+duration_millis=343, source="localhost", trace_id=UUID("7b3bf470-9456-11e8-
+9eb6-529269fb1459"), span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
+parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID
+("5f64e538-9457-11e8-9eb6-529269fb1459")], tags=[("application", "Wavefront"),
+("http.method", "GET")], span_logs=None, default_source="defaultSource") #
+Result of one_tracing_span_data: # '"getAllUsers" source="localhost"
+traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-
+529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
+# 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET"
+1552949776000 343\n' # List of data batch_span_data = [one_tracing_span_data,
 one_tracing_span_data] # Send list of data immediately
 wavefront_sender.send_span_now(batch_span_data) ``` ### Batch Events ```python
 from wavefront_sdk.common import event_to_line_data # Generate string data in
-Wavefront event format one_event_data = event_to_line_data(name="event name",
+Wavefront event format one_event_data = event_to_line_data( name="event name",
 start_time=1592200048, end_time=1592201048, source="localhost", tags=["env",
 "dev"], annotations={"severity": "info", "type": "backup", "details": "broker
 backup"}) # Result of one_event_data: # '@Event 1592200048 1592201048 "event
 name" severity="info" type="backup" details="broker backup" # host="localhost"
 tag="env" tag="dev"\n' # List of events batch_event_data = [one_event_data,
 one_event_data] # Send list of events immediately
 wavefront_sender.send_event_now(batch_event_data) ``` ## Get the Failure Count
 If the application failed to send metrics, histograms, or trace data via the
 `wavefront_sender`, you can get the total failure count. ```python # Get the
 total failure count total_failures = wavefront_sender.get_failure_count() ```
-## Close the Connection * If the Wavefront sender is from a
-`WavefrontClientFactory`, close the connection before shutting down the
-application. ```python # To shut down a sender from a WavefrontClientFactory
-wavefront_sender = client_factory.get_client() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontDirectClient`, flush all buffers and then close the connection before
-shutting down the application. ```python # To shut down a WavefrontDirectClient
-# Flush all buffers. wavefront_sender.flush_now() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontProxyClient`, close the connection before shutting down the
-application. ```python # To shut down a WavefrontProxyClient # Close the sender
-connection wavefront_sender.close() ``` ## License [Apache 2.0 License]
-(LICENSE). ## How to Get Support and Contribute * When submitting changes, be
-sure to increment the version number in setup.py. The version number is
-documented as such in setup.py. We follow semantic versioning. For bug fixes,
-increment the patch version (last number). For backward compatible changes to
-the API, update the minor version (second number), and zero out the patch
-version. For breaking changes to the API, increment the major version (first
-number) and zero out the minor and patch versions. * Reach out to us on our
-public [Slack channel](https://www.wavefront.com/join-public-slack). * If you
-run into any issues, let us know by creating a GitHub issue.
+## Close the Connection * If the sender is from a `WavefrontClientFactory`,
+close the connection before shutting down the application. ```python # To shut
+down a sender from a WavefrontClientFactory wavefront_sender =
+client_factory.get_client() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontDirectClient`,
+flush all buffers and then close the connection before shutting down the
+application. ```python # To shut down a WavefrontDirectClient # Flush all
+buffers. wavefront_sender.flush_now() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontProxyClient`, close
+the connection before shutting down the application. ```python # To shut down a
+WavefrontProxyClient # Close the sender connection wavefront_sender.close() ```
+## License [Apache 2.0 License](LICENSE). ## How to Get Support and Contribute
+* When submitting changes, be sure to increment the version number in setup.py.
+The version number is documented as such in setup.py. We follow semantic
+versioning. For bug fixes, increment the patch version (last number). For
+backward compatible changes to the API, update the minor version (second
+number), and zero out the patch version. For breaking changes to the API,
+increment the major version (first number) and zero out the minor and patch
+versions. * Reach out to us on our public [Slack channel](https://
+www.wavefront.com/join-public-slack). * If you run into any issues, let us know
+by creating a GitHub issue. ## How to Release 1. Merge all the changes that
+need to go into the release to the master branch. 2. Open the `setup.py` file
+from the top level directory of the project. 3. Search for version= in the file
+to find the version number, for example 1.8.15. 4. Create a pull request, get
+it reviewed and approved, and merge it after approval. 5. Check [test.pypi.org]
+(https://test.pypi.org/project/wavefront-sdk-python) for a published package,
+make sure it's production ready. 6. Log in to GitHub, click Releases on the
+right, and click Draft a new release. 7. For **Choose a tag**, choose the
+version you found in step 3, and prefix it with `v` for example `v1.8.15`. You
+need to enter the version where it says **Find or create new tag**. [A diagram
+that shows how to choose version] 8. Provide a short but descriptive title for
+the release. 9. Fill in the details of the release. Please copy the markdown
+from the previous release and follow the same format. 10. Click **Publish
+release.** to start publishing the release to pypi.org. 11. From the GitHub top
+navigation bar of this project, click the **Actions** tab. On the first line of
+the list of workflows, you should see a workflow running that will publish your
+release to pypi.org. 12. When the workflow from step 9 has a green checkmark
+next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/
+) and verify that the latest version is published.
```

### Comparing `wavefront-sdk-python-1.8.2/README.md` & `wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,77 @@
+Metadata-Version: 2.1
+Name: wavefront-sdk-python
+Version: 1.9.0
+Summary: VMware Aria Operations for Applications Python SDK
+Home-page: https://github.com/wavefrontHQ/wavefront-sdk-python
+Author: VMware Aria Operations for Applications Team
+License: Apache-2.0
+Keywords: Aria,Aria Operations,Aria Operations for Applications,3D Observability,Distributed Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware Aria,VMware Aria Operations,VMware Aria Operations for Applications,Wavefront,Wavefront SDK
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Monitoring
+Classifier: Topic :: System :: Networking :: Monitoring
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # wavefront-sdk-python
 
-[![travis build status](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python)
+[![Build Status](https://github.com/wavefrontHQ/wavefront-sdk-python/actions/workflows/main.yml/badge.svg)](https://github.com/wavefrontHQ/wavefront-sdk-python/actions)
 [![image](https://img.shields.io/pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/pyversions/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/wavefront-sdk-python)
 
 
 ## Table of Content
 * [Prerequisites](#Prerequisites)
-* [Set Up a Wavefront Sender](#set-up-a-wavefront-sender)
-* [Send a Single Data Point to Wavefront](#send-a-single-data-point-to-wavefront)
-* [Send Batch Data to Wavefront](#send-batch-data-to-wavefront)
+* [Set Up a Sender](#set-up-a-sender)
+* [Send a Single Data Point](#send-a-single-data-point)
+* [Send Batch Data](#send-batch-data)
 * [Get the Failure Count](#get-the-failure-count)
 * [Close the Connection](#close-the-connection)
 * [License](#License)
 * [How to Get Support and Contribute](#how-to-get-support-and-contribute)
+* [How to Release](#how-to-release)
+
+# VMware Aria Operations™ for Applications Python SDK
 
-# Welcome to the Wavefront Python SDK
+VMware Aria Operations for Applications (formerly known as Wavefront) Python SDK lets you send raw data from your Python application to Operations for Applications using a wavefront_sender interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python.
 
-Wavefront by VMware Python SDK lets you send raw data from your Python application to Wavefront using a `wavefront_sender` interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python. 
+Although this library is mostly used by the other Operations for Applications Python SDKs to send data to Operations for Applications, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Operations for Applications.
 
-Although this library is mostly used by the other Wavefront Python SDKs to send data to Wavefront, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Wavefront.
+Note: We're in the process of updating the product name to Operations for Applications, but in many places we still refer to it as Wavefront.
 
 **Before you start implementing, let us make sure you are using the correct SDK!**
 
 ![Python Sender SDK Decision Tree](docs/python_sender_sdk.png)
 
 > ***Note***:
 > </br>
->   * **This is the Wavefront by VMware SDK for Python (Wavefront Sender SDK for Python)!**
+>   * **This is the VMware Aria Operations for Applications SDK for Python (Sender SDK for Python)!**
 >   If this SDK is not what you were looking for, see the [table](#wavefront-sdks) below.
 
-#### Wavefront SDKs
+#### VMware Aria Operations for Applications SDKs
 <table id="SDKlevels" style="width: 100%">
 <tr>
   <th width="10%">SDK Type</th>
   <th width="45%">SDK Description</th>
   <th width="45%">Supported Languages</th>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-trace-data">OpenTracing SDK</a></td>
-  <td align="justify">Implements the OpenTracing specification. Lets you define, collect, and report custom trace data from any part of your application code. <br>Automatically derives Rate Errors Duration (RED) metrics from the reported spans. </td>
-  <td>
-    <ul>
-    <li>
-      <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-java">OpenTracing SDK</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-bundle-java">Tracing Agent</a>
-    </li>
-    <li>
-      <b>Python</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-python">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>Go</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-go">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-csharp">OpenTracing SDK</a>
-    </li>
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-metrics-and-histograms">Metrics SDK</a></td>
   <td align="justify">Implements a standard metrics library. Lets you define, collect, and report custom business metrics and histograms from any part of your application code.   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-dropwizard-metrics-sdk-java">Dropwizard</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-runtime-sdk-jvm">JVM</a>
     </li>
@@ -78,30 +85,16 @@
     <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-appmetrics-sdk-csharp">App Metrics SDK</a>
     </li>
     </ul>
   </td>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-that-instrument-frameworks">Framework SDK</a></td>
-  <td align="justify">Reports predefined traces, metrics, and histograms from the APIs of a supported app framework. Lets you get started quickly with minimal code changes.</td>
-  <td>
-    <ul>
-    <li><b>Java</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-dropwizard-sdk-java">Dropwizard</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-gRPC-sdk-java">gRPC</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jaxrs-sdk-java">JAX-RS</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jersey-sdk-java">Jersey</a></li>
-    <li><b>.Net/C#</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-aspnetcore-sdk-csharp">ASP.Net core</a> </li>
-    <!--- [Python](wavefront_sdks_python.html#python-sdks-that-instrument-frameworks) --->
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-sending-raw-data-to-wavefront">Sender SDK</a></td>
-  <td align="justify">Lets you send raw data to Wavefront for storage as metrics, histograms, or traces, e.g., to import CSV data into Wavefront.
+  <td align="justify">Lets you send raw data for storage as metrics, histograms, or traces, e.g., to import CSV data into the service.
   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-sdk-java">Sender SDK</a>
     </li>
     <li>
@@ -121,59 +114,59 @@
 </tr>
 
 </tbody>
 </table>
 
 ## Prerequisites
 
-* Python ~~2.7+~~ and Python 3.x are supported.
+* Python versions 3.7 - 3.11 are supported.
 * Install `wavefront-sdk-python`
     ```
     pip install wavefront-sdk-python
     ```
 
-## Set Up a Wavefront Sender
+## Set Up a Sender
 
-You can send metrics, histograms, or trace data from your application to the Wavefront service using a Wavefront proxy or direct ingestions.
+You can send metrics, histograms, or trace data from your application to the service using a Wavefront Proxy or direct ingestions.
 
-* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the Wavefront service. This is the simplest way to get up and running quickly.
-* Use a [**Wavefront proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the Wavefront service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
+* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the service. This is the simplest way to get up and running quickly.
+* Use a [**Wavefront Proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
 
 You instantiate an object that corresponds to your choice:
 * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront service.
-* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy.
-* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to a Wavefront service directly or via proxy.
+* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront Proxy.
+* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the service directly or via proxy.
 > **Deprecated implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy version 7.0 onwards. We recommend all new applications to use the `WavefrontClient`.*
 
 ### Option 1: Create a WavefrontDirectClient
-When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the Wavefront URL and API token to send data directly to Wavefront.
+When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the cluster URL and API token to send data directly to the service.
 
 >**Prerequisites**
 > * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-> * The URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `https://<domain>.wavefront.com`.
+> * The URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `https://<domain>.wavefront.com`.
 > * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 #### Initialize the WavefrontDirectClient
 You initialize a `WavefrontDirectClient` by providing the access information you obtained in the Prerequisites section..
 
 Optionally, you can specify parameters to tune the following ingestion properties:
 
-* Max queue size - Internal buffer capacity of the Wavefront sender. Any data in excess of this size is dropped.
-* Flush interval - Interval for flushing data from the Wavefront sender directly to Wavefront.
-* Batch size - Amount of data to send to Wavefront in each flush interval.
+* Max queue size - Internal buffer capacity of the sender. Any data in excess of this size is dropped.
+* Flush interval - Interval for flushing data from the sender directly to the service.
+* Batch size - Amount of data to send to the service in each flush interval.
 
-Together, the batch size and flush interval control the maximum theoretical throughput of the Wavefront sender. You should override the defaults _only_ to set higher values.
+Together, the batch size and flush interval control the maximum theoretical throughput of the sender. You should override the defaults _only_ to set higher values.
 
 
 ```python
 from wavefront_sdk import WavefrontDirectClient
 
 # Create a sender with:
-   # your Wavefront URL
-   # a Wavefront API token that was created with direct ingestion permission
+   # your cluster URL
+   # an API token that was created with direct ingestion permission
    # max queue size (in data points). Default: 50,000
    # batch size (in data points). Default: 10,000
    # flush interval  (in seconds). Default: 1 second
 wavefront_sender = WavefrontDirectClient(
     server="<SERVER_ADDR>",
     token="<TOKEN>",
     max_queue_size=50000,
@@ -183,17 +176,17 @@
 ```
 
 ### Option 2: Create a WavefrontProxyClient
 
 >**Prerequisite** <br/>
 >Before your application can use a `WavefrontProxyClient`, you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
 
-When sending data via the Wavefront proxy, you need to create a `WavefrontProxyClient`. Include the following information.
+When sending data via the Wavefront Proxy, you need to create a `WavefrontProxyClient`. Include the following information.
 
-* The name of the host that will run the Wavefront proxy.
+* The name of the host that will run the Wavefront Proxy.
 * One or more proxy listening ports to send data to. The ports you specify depend on the kinds of data you want to send (metrics, histograms, and/or trace data). You must specify at least one listener port.
 * Optional settings for tuning communication with the proxy.
 
 > **Note**: See [Advanced Proxy Configuration and Installation](https://docs.wavefront.com/proxies_configuring.html) for details.
 
 ```python
 from wavefront_sdk import WavefrontProxyClient
@@ -209,32 +202,32 @@
    metrics_port=2878,
    distribution_port=2878,
    tracing_port=30000,
    event_port=2878
 )
 ```
 
-> **Note:** When you set up a Wavefront proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
+> **Note:** When you set up a Wavefront Proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront Proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
 
 | `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf` |
 | ----- | -------- |
 | `metrics_port` | `pushListenerPorts=` |
 | `distribution_port` | `histogramDistListenerPorts=` |
 | `tracing_port` | `traceListenerPorts=` |
 
 ### Option 3: Create a WavefrontClient
-Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to a Wavefront service or send data using a Wavefront Proxy.
+Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to the service or send data using a Wavefront Proxy.
 
-The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple Wavefront services.
+The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple services.
 ### Prerequisites
-* Sending data via Wavefront proxy?
-  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
+* Sending data via Wavefront Proxy?
+  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html).
 * Sending data via direct ingestion?
   * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-  * The HTTP URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
+  * The HTTP URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
   * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 ### Initialize the WavefrontClient
 ```python
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 # Create a sender with:
@@ -250,48 +243,53 @@
 client_factory.add_client(
     url="<URL for proxy or direct ingestions>",
     max_queue_size=50000,
     batch_size=10000,
     flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client()
 ```
-#### Add multiple clients to client factory to send data to multiple Wavefront services.
+#### Add multiple clients to client factory to send data to multiple services.
 ```
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 client_factory = WavefrontClientFactory()
 client_factory.add_client("proxy://our.proxy.lb.com:2878")
 client_factory.add_client("https://someToken@DOMAIN.wavefront.com")
 
 # Send traces and spans to the tracing port. If you are directly using the sender SDK to send spans without using any other SDK, use the same port as the customTracingListenerPorts configured in the wavefront proxy. Assume you have installed and started the proxy on <proxy_hostname>.
 client_factory.add_client("http://<proxy_hostname>:30000")
 
 wavefront_sender = client_factory.get_client()
 ```
 
-## Send a Single Data Point to Wavefront
+## Send a Single Data Point
 
-The following examples show how to send a single data point to Wavefront. You use the Wavefront sender you created above.
+The following examples show how to send a single data point to the service. You use the Wavefront Sender you created above.
 
 ### Single Metric or  Delta Counter
 
 ```python
 from uuid import UUID
 
 # Wavefront metrics data format:
 # <metricName> <metricValue> [<timestamp>] source=<source> [pointTags]
 wavefront_sender.send_metric(
-    name="new york.power.usage", value=42422.0, timestamp=1533529977,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="new_york.power.usage",
+    value=42422.0,
+    timestamp=1533529977,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 
 # Wavefront delta counter data format:
 # <metricName> <metricValue> source=<source> [pointTags]
 wavefront_sender.send_delta_counter(
-    name="delta.counter", value=1.0,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="delta.counter",
+    value=1.0,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 ```
 ***Note***: If your metric name has a bad character, that character is replaced with a `-`.
 
 ### Single Histogram Distribution
 
 ```python
 from uuid import UUID
@@ -300,71 +298,87 @@
 # Wavefront histogram data format:
 # {!M | !H | !D} [<timestamp>] #<count> <mean> [centroids] <histogramName> source=<source> [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day
 # "!M 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 wavefront_sender.send_distribution(
-    name="request.latency", centroids=[(30, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.DAY,
                              histogram_granularity.HOUR,
                              histogram_granularity.MINUTE},
-    timestamp=1533529977, source="appServer1", tags={"region": "us-west"})
+    timestamp=1533529977,
+    source="appServer1",
+    tags={"region": "us-west"})
 ```
 
 ### Single Span
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with the Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 
 # Wavefront trace and span data format:
 # <tracingSpanName> source=<source> [pointTags] <start_millis> <duration_milliseconds>
 # Example: "getAllUsers source=localhost
 #           traceId=7b3bf470-9456-11e8-9eb6-529269fb1459
 #           spanId=0313bafe-9457-11e8-9eb6-529269fb1459
 #           parent=2f64e538-9457-11e8-9eb6-529269fb1459
 #           application=Wavefront http.method=GET
 #           1533529977 343500"
 wavefront_sender.send_span(
-    name="getAllUsers", start_millis=1533529977, duration_millis=343500,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1533529977,
+    duration_millis=343500,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
-    follows_from=None, tags=[("application", "Wavefront"),
-                             ("service", "istio"),
-                             ("http.method", "GET")],
+    follows_from=None,
+    tags=[("application", "Wavefront"),
+          ("service", "istio"),
+          ("http.method", "GET")],
     span_logs=None)
 ```
 
 ### Single Event
 
 ```python
 # Wavefront event format:
 # @Event <StartTime> <EndTime> "<EventName>"  severity="<Severity>"
 # type="<Type>" details="<EventDetail>" host="<Source>" tag="<Tags>"
-wavefront_sender.send_event('event name', 1592200048, 1592201048, "localhost",
-    ["env:", "dev"], {"severity": "info", "type": "backup", "details": "broker backup"})
+wavefront_sender.send_event('event name',
+                            1592200048,
+                            1592201048,
+                            "localhost",
+                            ["env:", "dev"],
+                            {"severity": "info",
+                             "type": "backup",
+                             "details": "broker backup"})
 ```
 
-## Send Batch Data to Wavefront
+## Send Batch Data
 
 The following examples show how to generate data points manually and send them as a batch to Wavefront.
 
 ### Batch Metrics
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import metric_to_line_data
 
 # Generate string data in Wavefront metric format
 one_metric_data = metric_to_line_data(
-    name="new-york.power.usage", value=42422, timestamp=1493773500,
-    source="localhost", tags={"datacenter": "dc1"},
+    name="new-york.power.usage",
+    value=42422,
+    timestamp=1493773500,
+    source="localhost",
+    tags={"datacenter": "dc1"},
     default_source="defaultSource")
 
 # Result of one_metric_data:
   # '"new-york.power.usage" 42422.0 1493773500 source="localhost" "datacenter"="dc1"\n'
 
 # List of data
 batch_metric_data = [one_metric_data, one_metric_data]
@@ -379,19 +393,22 @@
 ```python
 from uuid import UUID
 from wavefront_sdk.entities.histogram import histogram_granularity
 from wavefront_sdk.common import histogram_to_line_data
 
 # Generate string data in Wavefront histogram format
 one_histogram_data = histogram_to_line_data(
-    name="request.latency", centroids=[(30.0, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30.0, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.MINUTE,
                              histogram_granularity.HOUR,
                              histogram_granularity.DAY},
-    timestamp=1493773500, source="appServer1", tags={"region": "us-west"},
+    timestamp=1493773500,
+    source="appServer1",
+    tags={"region": "us-west"},
     default_source ="defaultSource")
 
 # Result of one_histogram_data:
   # '!D 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !H 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n'
 
@@ -399,29 +416,33 @@
 batch_histogram_data = [one_histogram_data, one_histogram_data]
 
 # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data)
 ```
 ### Batch Trace Data
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import tracing_span_to_line_data
 
 # Generate string data in Wavefront tracing span format
 one_tracing_span_data = tracing_span_to_line_data(
-    name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1552949776000,
+    duration_millis=343,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
     follows_from=[UUID("5f64e538-9457-11e8-9eb6-529269fb1459")],
     tags=[("application", "Wavefront"), ("http.method", "GET")],
-    span_logs=None, default_source="defaultSource")
+    span_logs=None,
+    default_source="defaultSource")
 
 # Result of one_tracing_span_data:
   # '"getAllUsers" source="localhost" traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe-
   # 9457-11e8-9eb6-529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
   # 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000 343\n'
 
 # List of data
@@ -433,16 +454,23 @@
 
 ### Batch Events
 
 ```python
 from wavefront_sdk.common import event_to_line_data
 
 # Generate string data in Wavefront event format
-one_event_data = event_to_line_data(name="event name", start_time=1592200048, end_time=1592201048,
- source="localhost", tags=["env", "dev"], annotations={"severity": "info", "type": "backup", "details": "broker backup"})
+one_event_data = event_to_line_data(
+    name="event name",
+    start_time=1592200048,
+    end_time=1592201048,
+    source="localhost",
+    tags=["env", "dev"],
+    annotations={"severity": "info",
+                 "type": "backup",
+                 "details": "broker backup"})
 
 # Result of one_event_data:
 # '@Event 1592200048 1592201048 "event name" severity="info" type="backup" details="broker backup"
 # host="localhost" tag="env" tag="dev"\n'
 
 # List of events
 batch_event_data = [one_event_data, one_event_data]
@@ -457,34 +485,34 @@
 
 ```python
 # Get the total failure count
 total_failures = wavefront_sender.get_failure_count()
 ```
 ## Close the Connection
 
-* If the Wavefront sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
+* If the sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
 
     ```python
     # To shut down a sender from a WavefrontClientFactory
     wavefront_sender = client_factory.get_client()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
+* If the sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontDirectClient
     # Flush all buffers.
     wavefront_sender.flush_now()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
+* If the sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontProxyClient
 
     # Close the sender connection
     wavefront_sender.close()
     ```
@@ -499,7 +527,25 @@
   We follow semantic versioning. For bug fixes, increment the patch version
   (last number). For backward compatible changes to the API, update the
   minor version (second number), and zero out the patch version. For breaking
   changes to the API, increment the major version (first number) and zero out
   the minor and patch versions.
 * Reach out to us on our public [Slack channel](https://www.wavefront.com/join-public-slack).
 * If you run into any issues, let us know by creating a GitHub issue.
+
+## How to Release
+
+1. Merge all the changes that need to go into the release to the master branch.
+2. Open the `setup.py` file from the top level directory of the project.
+3. Search for version= in the file to find the version number, for example 1.8.15.
+4. Create a pull request, get it reviewed and approved, and merge it after approval.
+5. Check [test.pypi.org](https://test.pypi.org/project/wavefront-sdk-python) for a published package, make sure it's production ready.
+6. Log in to GitHub, click Releases on the right, and click Draft a new release.
+7. For **Choose a tag**, choose the version you found in step 3, and prefix it with `v` for example `v1.8.15`. You need to enter the version where it says **Find or create new tag**.
+
+<img src="images/choose-version.png" alt="A diagram that shows how to choose version"/>
+
+8. Provide a short but descriptive title for the release.
+9. Fill in the details of the release. Please copy the markdown from the previous release and follow the same format.
+10. Click **Publish release.** to start publishing the release to pypi.org.
+11. From the GitHub top navigation bar of this project, click the **Actions** tab. On the first line of the list of workflows, you should see a workflow running that will publish your release to pypi.org.
+12. When the workflow from step 9 has a green checkmark next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/) and verify that the latest version is published.
```

#### html2text {}

```diff
@@ -1,209 +1,216 @@
-# wavefront-sdk-python [![travis build status](https://travis-ci.com/
-wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://travis-ci.com/
-wavefrontHQ/wavefront-sdk-python) [![image](https://img.shields.io/pypi/v/
-wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/) [!
-[image](https://img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://
-pypi.org/project/wavefront-sdk-python/) [![image](https://img.shields.io/pypi/
-pyversions/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-
-python/) ## Table of Content * [Prerequisites](#Prerequisites) * [Set Up a
-Wavefront Sender](#set-up-a-wavefront-sender) * [Send a Single Data Point to
-Wavefront](#send-a-single-data-point-to-wavefront) * [Send Batch Data to
-Wavefront](#send-batch-data-to-wavefront) * [Get the Failure Count](#get-the-
-failure-count) * [Close the Connection](#close-the-connection) * [License]
-(#License) * [How to Get Support and Contribute](#how-to-get-support-and-
-contribute) # Welcome to the Wavefront Python SDK Wavefront by VMware Python
-SDK lets you send raw data from your Python application to Wavefront using a
-`wavefront_sender` interface. The data is then stored as metrics, histograms,
-and trace data. This SDK is also referred to as the Wavefront Sender SDK for
-Python. Although this library is mostly used by the other Wavefront Python SDKs
-to send data to Wavefront, you can also use this SDK directly. For example, you
-can send data directly from a data store or CSV file to Wavefront. **Before you
-start implementing, let us make sure you are using the correct SDK!** ![Python
-Sender SDK Decision Tree](docs/python_sender_sdk.png) > ***Note***: >  > *
-**This is the Wavefront by VMware SDK for Python (Wavefront Sender SDK for
-Python)!** > If this SDK is not what you were looking for, see the [table]
-(#wavefront-sdks) below. #### Wavefront SDKs
-SDK Type        SDK Description                 Supported Languages
-                Implements the OpenTracing
-                specification. Lets you define,     * Java: OpenTracing_SDK |
-                collect, and report custom            Tracing_Agent
-OpenTracing_SDK trace data from any part of         * Python: OpenTracing_SDK
-                your application code.              * Go: OpenTracing_SDK
-                Automatically derives Rate          * .Net/C#: OpenTracing_SDK
-                Errors Duration (RED) metrics
-                from the reported spans.
-                Implements a standard metrics
-                library. Lets you define,           * Java: Dropwizard | JVM
-Metrics_SDK     collect, and report custom          * Python: Pyformance_SDK
-                business metrics and histograms     * Go: Go_Metrics_SDK
-                from any part of your               * .Net/C#: App_Metrics_SDK
-                application code.
-                Reports predefined traces,
-                metrics, and histograms from        * Java: Dropwizard | gRPC |
-Framework_SDK   the APIs of a supported app           JAX-RS | Jersey
-                framework. Lets you get started     * .Net/C#: ASP.Net_core
-                quickly with minimal code
-                changes.
-                Lets you send raw data to           * Java: Sender_SDK
-                Wavefront for storage as            * Python: Sender_SDK
-Sender_SDK      metrics, histograms, or traces,     * Go: Sender_SDK
-                e.g., to import CSV data into       * .Net/C#: Sender_SDK
-                Wavefront.                          * C++: Sender_SDK
-## Prerequisites * Python ~~2.7+~~ and Python 3.x are supported. * Install
+Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.9.0 Summary: VMware
+Aria Operations for Applications Python SDK Home-page: https://github.com/
+wavefrontHQ/wavefront-sdk-python Author: VMware Aria Operations for
+Applications Team License: Apache-2.0 Keywords: Aria,Aria Operations,Aria
+Operations for Applications,3D Observability,Distributed
+Tracing,Histograms,Logging,Metrics,Monitoring,Observability,Tracing,VMware
+Aria,VMware Aria Operations,VMware Aria Operations for
+Applications,Wavefront,Wavefront SDK Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: Information Technology Classifier: Intended Audience ::
+System Administrators Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Topic :: System ::
+Monitoring Classifier: Topic :: System :: Networking :: Monitoring Description-
+Content-Type: text/markdown License-File: LICENSE # wavefront-sdk-python [!
+[Build Status](https://github.com/wavefrontHQ/wavefront-sdk-python/actions/
+workflows/main.yml/badge.svg)](https://github.com/wavefrontHQ/wavefront-sdk-
+python/actions) [![image](https://img.shields.io/pypi/v/wavefront-sdk-
+python.svg)](https://pypi.org/project/wavefront-sdk-python/) [![image](https://
+img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://pypi.org/project/
+wavefront-sdk-python/) [![image](https://img.shields.io/pypi/pyversions/
+wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/) !
+[PyPI - Downloads](https://img.shields.io/pypi/dm/wavefront-sdk-python) ##
+Table of Content * [Prerequisites](#Prerequisites) * [Set Up a Sender](#set-up-
+a-sender) * [Send a Single Data Point](#send-a-single-data-point) * [Send Batch
+Data](#send-batch-data) * [Get the Failure Count](#get-the-failure-count) *
+[Close the Connection](#close-the-connection) * [License](#License) * [How to
+Get Support and Contribute](#how-to-get-support-and-contribute) * [How to
+Release](#how-to-release) # VMware Aria Operationsâ¢ for Applications Python
+SDK VMware Aria Operations for Applications (formerly known as Wavefront)
+Python SDK lets you send raw data from your Python application to Operations
+for Applications using a wavefront_sender interface. The data is then stored as
+metrics, histograms, and trace data. This SDK is also referred to as the
+Wavefront Sender SDK for Python. Although this library is mostly used by the
+other Operations for Applications Python SDKs to send data to Operations for
+Applications, you can also use this SDK directly. For example, you can send
+data directly from a data store or CSV file to Operations for Applications.
+Note: We're in the process of updating the product name to Operations for
+Applications, but in many places we still refer to it as Wavefront. **Before
+you start implementing, let us make sure you are using the correct SDK!** !
+[Python Sender SDK Decision Tree](docs/python_sender_sdk.png) > ***Note***: >
+> * **This is the VMware Aria Operations for Applications SDK for Python
+(Sender SDK for Python)!** > If this SDK is not what you were looking for, see
+the [table](#wavefront-sdks) below. #### VMware Aria Operations for
+Applications SDKs
+SDK Type    SDK Description                      Supported Languages
+            Implements a standard metrics            * Java: Dropwizard | JVM
+            library. Lets you define, collect,       * Python: Pyformance_SDK
+Metrics_SDK and report custom business metrics       * Go: Go_Metrics_SDK
+            and histograms from any part of your     * .Net/C#: App_Metrics_SDK
+            application code.
+            Lets you send raw data for storage       * Java: Sender_SDK
+            as metrics, histograms, or traces,       * Python: Sender_SDK
+Sender_SDK  e.g., to import CSV data into the        * Go: Sender_SDK
+            service.                                 * .Net/C#: Sender_SDK
+                                                     * C++: Sender_SDK
+## Prerequisites * Python versions 3.7 - 3.11 are supported. * Install
 `wavefront-sdk-python` ``` pip install wavefront-sdk-python ``` ## Set Up a
-Wavefront Sender You can send metrics, histograms, or trace data from your
-application to the Wavefront service using a Wavefront proxy or direct
-ingestions. * Use [**direct ingestion**](https://docs.wavefront.com/
-direct_ingestion.html) to send the data directly to the Wavefront service. This
-is the simplest way to get up and running quickly. * Use a [**Wavefront
-proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data
-to the Wavefront service. This is the recommended choice for a large-scale
-deployment that needs resilience to internet outages, control over data queuing
-and filtering, and more. You instantiate an object that corresponds to your
-choice: * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`]
-(#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront
-service. * Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`]
-(#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy. *
-Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to
-send data to a Wavefront service directly or via proxy. > **Deprecated
-implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are
-deprecated from proxy version 7.0 onwards. We recommend all new applications to
-use the `WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When
-sending data via direct ingestion, you need to create a
-`WavefrontDirectClient`, and build it with the Wavefront URL and API token to
-send data directly to Wavefront. >**Prerequisites** > * Verify that you have
-the Direct Data Ingestion permission. For details, see [Examine Groups, Roles,
-and Permissions](https://docs.wavefront.com/
-users_account_managing.html#examine-groups-roles-and-permissions). > * The URL
-of your Wavefront instance. This is the URL you connect to when you log in to
-Wavefront, typically something like `https://.wavefront.com`. > * [Obtain the
-API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-
-token). #### Initialize the WavefrontDirectClient You initialize a
-`WavefrontDirectClient` by providing the access information you obtained in the
-Prerequisites section.. Optionally, you can specify parameters to tune the
-following ingestion properties: * Max queue size - Internal buffer capacity of
-the Wavefront sender. Any data in excess of this size is dropped. * Flush
-interval - Interval for flushing data from the Wavefront sender directly to
-Wavefront. * Batch size - Amount of data to send to Wavefront in each flush
-interval. Together, the batch size and flush interval control the maximum
-theoretical throughput of the Wavefront sender. You should override the
-defaults _only_ to set higher values. ```python from wavefront_sdk import
-WavefrontDirectClient # Create a sender with: # your Wavefront URL # a
-Wavefront API token that was created with direct ingestion permission # max
-queue size (in data points). Default: 50,000 # batch size (in data points).
-Default: 10,000 # flush interval (in seconds). Default: 1 second
-wavefront_sender = WavefrontDirectClient( server="", token="",
-max_queue_size=50000, batch_size=10000, flush_interval_seconds=5 ) ``` ###
-Option 2: Create a WavefrontProxyClient >**Prerequisite**
+Sender You can send metrics, histograms, or trace data from your application to
+the service using a Wavefront Proxy or direct ingestions. * Use [**direct
+ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data
+directly to the service. This is the simplest way to get up and running
+quickly. * Use a [**Wavefront Proxy**](https://docs.wavefront.com/
+proxies.html), which then forwards the data to the service. This is the
+recommended choice for a large-scale deployment that needs resilience to
+internet outages, control over data queuing and filtering, and more. You
+instantiate an object that corresponds to your choice: * Option 1 **
+(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-
+wavefrontdirectclient) to send data directly to a Wavefront service. * Option 2
+**(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-
+wavefrontproxyclient) to send data to a Wavefront Proxy. * Option 3: [Create a
+`WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the
+service directly or via proxy. > **Deprecated implementations**:
+*`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy
+version 7.0 onwards. We recommend all new applications to use the
+`WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When sending
+data via direct ingestion, you need to create a `WavefrontDirectClient`, and
+build it with the cluster URL and API token to send data directly to the
+service. >**Prerequisites** > * Verify that you have the Direct Data Ingestion
+permission. For details, see [Examine Groups, Roles, and Permissions](https://
+docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-
+permissions). > * The URL of your cluster. This is the URL you connect to when
+you log in to the service, typically something like `https://.wavefront.com`. >
+* [Obtain the API token](http://docs.wavefront.com/
+wavefront_api.html#generating-an-api-token). #### Initialize the
+WavefrontDirectClient You initialize a `WavefrontDirectClient` by providing the
+access information you obtained in the Prerequisites section.. Optionally, you
+can specify parameters to tune the following ingestion properties: * Max queue
+size - Internal buffer capacity of the sender. Any data in excess of this size
+is dropped. * Flush interval - Interval for flushing data from the sender
+directly to the service. * Batch size - Amount of data to send to the service
+in each flush interval. Together, the batch size and flush interval control the
+maximum theoretical throughput of the sender. You should override the defaults
+_only_ to set higher values. ```python from wavefront_sdk import
+WavefrontDirectClient # Create a sender with: # your cluster URL # an API token
+that was created with direct ingestion permission # max queue size (in data
+points). Default: 50,000 # batch size (in data points). Default: 10,000 # flush
+interval (in seconds). Default: 1 second wavefront_sender =
+WavefrontDirectClient( server="", token="", max_queue_size=50000,
+batch_size=10000, flush_interval_seconds=5 ) ``` ### Option 2: Create a
+WavefrontProxyClient >**Prerequisite**
 >Before your application can use a `WavefrontProxyClient`, you must [set up and
 start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
-When sending data via the Wavefront proxy, you need to create a
+When sending data via the Wavefront Proxy, you need to create a
 `WavefrontProxyClient`. Include the following information. * The name of the
-host that will run the Wavefront proxy. * One or more proxy listening ports to
+host that will run the Wavefront Proxy. * One or more proxy listening ports to
 send data to. The ports you specify depend on the kinds of data you want to
 send (metrics, histograms, and/or trace data). You must specify at least one
 listener port. * Optional settings for tuning communication with the proxy. >
 **Note**: See [Advanced Proxy Configuration and Installation](https://
 docs.wavefront.com/proxies_configuring.html) for details. ```python from
 wavefront_sdk import WavefrontProxyClient # Create a sender with: # the proxy
 hostname or address # the default listener port (2878) for sending metrics to #
 the recommended listener port (2878) for sending histograms to # the
 recommended listener port (30000) for sending trace data. # if you are directly
 using the sender sdk to send spans without using any other sdk, use the same
 port as the customTracingListenerPorts configured in the wavefront proxy for
 the tracing_port wavefront_sender = WavefrontProxyClient( host="",
 metrics_port=2878, distribution_port=2878, tracing_port=30000, event_port=2878
-) ``` > **Note:** When you set up a Wavefront proxy on the specified proxy
+) ``` > **Note:** When you set up a Wavefront Proxy on the specified proxy
 host, you specify the port it will listen to for each type of data to be sent.
 The `WavefrontProxyClient` must send data to the same ports that the Wavefront
-proxy listens to. Consequently, the port-related parameters must specify the
+Proxy listens to. Consequently, the port-related parameters must specify the
 same port numbers as the corresponding proxy configuration properties: |
 `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf`
 | | ----- | -------- | | `metrics_port` | `pushListenerPorts=` | |
 `distribution_port` | `histogramDistListenerPorts=` | | `tracing_port` |
 `traceListenerPorts=` | ### Option 3: Create a WavefrontClient Use
 `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send
-data directly to a Wavefront service or send data using a Wavefront Proxy. The
+data directly to the service or send data using a Wavefront Proxy. The
 `WavefrontClientFactory` supports multiple client bindings. If more than one
 client configuration is specified, you can create a `WavefrontMultiClient`
-instance, which can send data to multiple Wavefront services. ### Prerequisites
-* Sending data via Wavefront proxy?
+instance, which can send data to multiple services. ### Prerequisites * Sending
+data via Wavefront Proxy?
 Before your application can use a `WavefrontClient` you must [set up and start
-a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html). *
+a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html). *
 Sending data via direct ingestion? * Verify that you have the Direct Data
 Ingestion permission. For details, see [Examine Groups, Roles, and Permissions]
 (https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-
-and-permissions). * The HTTP URL of your Wavefront instance. This is the URL
-you connect to when you log in to Wavefront, typically something like `http:/
+and-permissions). * The HTTP URL of your cluster. This is the URL you connect
+to when you log in to the service, typically something like `http:/
 /.wavefront.com`.
 You can also use HTTP client with Wavefront Proxy version 7.0 or newer.
 Example: `http://proxy.acme.corp:2878`. * [Obtain the API token](http://
 docs.wavefront.com/wavefront_api.html#generating-an-api-token). ### Initialize
 the WavefrontClient ```python from wavefront_sdk.client_factory import
 WavefrontClientFactory # Create a sender with: # Required Parameter # URL
 format to send data via proxy: "proxy://
 proxy.load.balancer.com>:" # URL format to send data via direct ingestion:
 "https://TOKEN@DOMAIN.wavefront.com" # Optional Parameter # max queue size (in
 data points). Default: 50000 # batch size (in data points). Default: 10000 #
 flush interval (in seconds). Default: 1 second client_factory =
 WavefrontClientFactory() client_factory.add_client( url="",
 max_queue_size=50000, batch_size=10000, flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client() ``` #### Add multiple clients to
-client factory to send data to multiple Wavefront services. ``` from
+client factory to send data to multiple services. ``` from
 wavefront_sdk.client_factory import WavefrontClientFactory client_factory =
 WavefrontClientFactory() client_factory.add_client("proxy://our.proxy.lb.com:
 2878") client_factory.add_client("https://someToken@DOMAIN.wavefront.com") #
 Send traces and spans to the tracing port. If you are directly using the sender
 SDK to send spans without using any other SDK, use the same port as the
 customTracingListenerPorts configured in the wavefront proxy. Assume you have
 installed and started the proxy on . client_factory.add_client("http://:30000")
 wavefront_sender = client_factory.get_client() ``` ## Send a Single Data Point
-to Wavefront The following examples show how to send a single data point to
-Wavefront. You use the Wavefront sender you created above. ### Single Metric or
-Delta Counter ```python from uuid import UUID # Wavefront metrics data format:
-#   [] source= [pointTags] wavefront_sender.send_metric( name="new
-york.power.usage", value=42422.0, timestamp=1533529977, source="localhost",
-tags={"datacenter": "dc1"}) # Wavefront delta counter data format: #   source=
-[pointTags] wavefront_sender.send_delta_counter( name="delta.counter",
-value=1.0, source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If
-your metric name has a bad character, that character is replaced with a `-`.
-### Single Histogram Distribution ```python from uuid import UUID from
+The following examples show how to send a single data point to the service. You
+use the Wavefront Sender you created above. ### Single Metric or Delta Counter
+```python from uuid import UUID # Wavefront metrics data format: #   [] source=
+[pointTags] wavefront_sender.send_metric( name="new_york.power.usage",
+value=42422.0, timestamp=1533529977, source="localhost", tags={"datacenter":
+"dc1"}) # Wavefront delta counter data format: #   source= [pointTags]
+wavefront_sender.send_delta_counter( name="delta.counter", value=1.0,
+source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If your metric
+name has a bad character, that character is replaced with a `-`. ### Single
+Histogram Distribution ```python from uuid import UUID from
 wavefront_sdk.entities.histogram import histogram_granularity # Wavefront
 histogram data format: # {!M | !H | !D} [] #  [centroids]  source= [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day # "!M
 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west" #
 "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-
 west" # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1
 region=us-west" wavefront_sender.send_distribution( name="request.latency",
 centroids=[(30, 20), (5.1, 10)], histogram_granularities=
 {histogram_granularity.DAY, histogram_granularity.HOUR,
 histogram_granularity.MINUTE}, timestamp=1533529977, source="appServer1", tags=
 {"region": "us-west"}) ``` ### Single Span If you are directly using the Sender
-SDK to send data to Wavefront, you wonât see span-level RED metrics by
-default unless you use the Wavefront proxy and define a custom tracing port
-(`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs]
-(https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-
-your-application-with-wavefront-sender-sdks) for details. ```python from uuid
-import UUID # Wavefront trace and span data format: #  source= [pointTags]   #
+SDK to send data to the service, you wonât see span-level RED metrics by
+default unless you use the Wavefront Proxy and define a custom tracing port
+(`tracing_port`). See [Instrument Your Application with the Sender SDKs](https:
+//docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID # Wavefront trace and span data format: #  source= [pointTags]   #
 Example: "getAllUsers source=localhost # traceId=7b3bf470-9456-11e8-9eb6-
 529269fb1459 # spanId=0313bafe-9457-11e8-9eb6-529269fb1459 # parent=2f64e538-
 9457-11e8-9eb6-529269fb1459 # application=Wavefront http.method=GET #
 1533529977 343500" wavefront_sender.send_span( name="getAllUsers",
 start_millis=1533529977, duration_millis=343500, source="localhost",
 trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"), span_id=UUID("0313bafe-
 9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-9457-11e8-9eb6-
 529269fb1459")], follows_from=None, tags=[("application", "Wavefront"),
 ("service", "istio"), ("http.method", "GET")], span_logs=None) ``` ### Single
 Event ```python # Wavefront event format: # @Event   "" severity="" # type=""
 details="" host="" tag="" wavefront_sender.send_event('event name', 1592200048,
 1592201048, "localhost", ["env:", "dev"], {"severity": "info", "type":
-"backup", "details": "broker backup"}) ``` ## Send Batch Data to Wavefront The
-following examples show how to generate data points manually and send them as a
-batch to Wavefront. ### Batch Metrics ```python from uuid import UUID from
+"backup", "details": "broker backup"}) ``` ## Send Batch Data The following
+examples show how to generate data points manually and send them as a batch to
+Wavefront. ### Batch Metrics ```python from uuid import UUID from
 wavefront_sdk.common import metric_to_line_data # Generate string data in
 Wavefront metric format one_metric_data = metric_to_line_data( name="new-
 york.power.usage", value=42422, timestamp=1493773500, source="localhost", tags=
 {"datacenter": "dc1"}, default_source="defaultSource") # Result of
 one_metric_data: # '"new-york.power.usage" 42422.0 1493773500
 source="localhost" "datacenter"="dc1"\n' # List of data batch_metric_data =
 [one_metric_data, one_metric_data] # Send list of data immediately
@@ -220,61 +227,79 @@
 ="defaultSource") # Result of one_histogram_data: # '!D 1493773500 #20 30.0 #10
 5.1 "request.latency" source="appServer1" "region"="us-west"\n # !H 1493773500
 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n #
 !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1"
 "region"="us-west"\n' # List of data batch_histogram_data =
 [one_histogram_data, one_histogram_data] # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data) ``` ### Batch
-Trace Data If you are directly using the Sender SDK to send data to Wavefront,
-you wonât see span-level RED metrics by default unless you use the Wavefront
-proxy and define a custom tracing port (`tracing_port`). See [Instrument Your
-Application with Wavefront Sender SDKs](https://docs.wavefront.com/
-tracing_instrumenting_frameworks.html#instrument-your-application-with-
-wavefront-sender-sdks) for details. ```python from uuid import UUID from
-wavefront_sdk.common import tracing_span_to_line_data # Generate string data in
-Wavefront tracing span format one_tracing_span_data = tracing_span_to_line_data
-( name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
-span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-
-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID("5f64e538-9457-11e8-9eb6-
-529269fb1459")], tags=[("application", "Wavefront"), ("http.method", "GET")],
-span_logs=None, default_source="defaultSource") # Result of
-one_tracing_span_data: # '"getAllUsers" source="localhost" traceId=7b3bf470-
-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-529269fb1459
-parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538- # 9457-11e8-
-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000
-343\n' # List of data batch_span_data = [one_tracing_span_data,
+Trace Data If you are directly using the Sender SDK to send data to the
+service, you wonât see span-level RED metrics by default unless you use the
+Wavefront Proxy and define a custom tracing port (`tracing_port`). See
+[Instrument Your Application with Wavefront Sender SDKs](https://
+docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID from wavefront_sdk.common import tracing_span_to_line_data # Generate
+string data in Wavefront tracing span format one_tracing_span_data =
+tracing_span_to_line_data( name="getAllUsers", start_millis=1552949776000,
+duration_millis=343, source="localhost", trace_id=UUID("7b3bf470-9456-11e8-
+9eb6-529269fb1459"), span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
+parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID
+("5f64e538-9457-11e8-9eb6-529269fb1459")], tags=[("application", "Wavefront"),
+("http.method", "GET")], span_logs=None, default_source="defaultSource") #
+Result of one_tracing_span_data: # '"getAllUsers" source="localhost"
+traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-
+529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
+# 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET"
+1552949776000 343\n' # List of data batch_span_data = [one_tracing_span_data,
 one_tracing_span_data] # Send list of data immediately
 wavefront_sender.send_span_now(batch_span_data) ``` ### Batch Events ```python
 from wavefront_sdk.common import event_to_line_data # Generate string data in
-Wavefront event format one_event_data = event_to_line_data(name="event name",
+Wavefront event format one_event_data = event_to_line_data( name="event name",
 start_time=1592200048, end_time=1592201048, source="localhost", tags=["env",
 "dev"], annotations={"severity": "info", "type": "backup", "details": "broker
 backup"}) # Result of one_event_data: # '@Event 1592200048 1592201048 "event
 name" severity="info" type="backup" details="broker backup" # host="localhost"
 tag="env" tag="dev"\n' # List of events batch_event_data = [one_event_data,
 one_event_data] # Send list of events immediately
 wavefront_sender.send_event_now(batch_event_data) ``` ## Get the Failure Count
 If the application failed to send metrics, histograms, or trace data via the
 `wavefront_sender`, you can get the total failure count. ```python # Get the
 total failure count total_failures = wavefront_sender.get_failure_count() ```
-## Close the Connection * If the Wavefront sender is from a
-`WavefrontClientFactory`, close the connection before shutting down the
-application. ```python # To shut down a sender from a WavefrontClientFactory
-wavefront_sender = client_factory.get_client() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontDirectClient`, flush all buffers and then close the connection before
-shutting down the application. ```python # To shut down a WavefrontDirectClient
-# Flush all buffers. wavefront_sender.flush_now() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontProxyClient`, close the connection before shutting down the
-application. ```python # To shut down a WavefrontProxyClient # Close the sender
-connection wavefront_sender.close() ``` ## License [Apache 2.0 License]
-(LICENSE). ## How to Get Support and Contribute * When submitting changes, be
-sure to increment the version number in setup.py. The version number is
-documented as such in setup.py. We follow semantic versioning. For bug fixes,
-increment the patch version (last number). For backward compatible changes to
-the API, update the minor version (second number), and zero out the patch
-version. For breaking changes to the API, increment the major version (first
-number) and zero out the minor and patch versions. * Reach out to us on our
-public [Slack channel](https://www.wavefront.com/join-public-slack). * If you
-run into any issues, let us know by creating a GitHub issue.
+## Close the Connection * If the sender is from a `WavefrontClientFactory`,
+close the connection before shutting down the application. ```python # To shut
+down a sender from a WavefrontClientFactory wavefront_sender =
+client_factory.get_client() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontDirectClient`,
+flush all buffers and then close the connection before shutting down the
+application. ```python # To shut down a WavefrontDirectClient # Flush all
+buffers. wavefront_sender.flush_now() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontProxyClient`, close
+the connection before shutting down the application. ```python # To shut down a
+WavefrontProxyClient # Close the sender connection wavefront_sender.close() ```
+## License [Apache 2.0 License](LICENSE). ## How to Get Support and Contribute
+* When submitting changes, be sure to increment the version number in setup.py.
+The version number is documented as such in setup.py. We follow semantic
+versioning. For bug fixes, increment the patch version (last number). For
+backward compatible changes to the API, update the minor version (second
+number), and zero out the patch version. For breaking changes to the API,
+increment the major version (first number) and zero out the minor and patch
+versions. * Reach out to us on our public [Slack channel](https://
+www.wavefront.com/join-public-slack). * If you run into any issues, let us know
+by creating a GitHub issue. ## How to Release 1. Merge all the changes that
+need to go into the release to the master branch. 2. Open the `setup.py` file
+from the top level directory of the project. 3. Search for version= in the file
+to find the version number, for example 1.8.15. 4. Create a pull request, get
+it reviewed and approved, and merge it after approval. 5. Check [test.pypi.org]
+(https://test.pypi.org/project/wavefront-sdk-python) for a published package,
+make sure it's production ready. 6. Log in to GitHub, click Releases on the
+right, and click Draft a new release. 7. For **Choose a tag**, choose the
+version you found in step 3, and prefix it with `v` for example `v1.8.15`. You
+need to enter the version where it says **Find or create new tag**. [A diagram
+that shows how to choose version] 8. Provide a short but descriptive title for
+the release. 9. Fill in the details of the release. Please copy the markdown
+from the previous release and follow the same format. 10. Click **Publish
+release.** to start publishing the release to pypi.org. 11. From the GitHub top
+navigation bar of this project, click the **Actions** tab. On the first line of
+the list of workflows, you should see a workflow running that will publish your
+release to pypi.org. 12. When the workflow from step 9 has a green checkmark
+next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/
+) and verify that the latest version is published.
```

### Comparing `wavefront-sdk-python-1.8.2/test/test_applicaiton_tags.py` & `wavefront-sdk-python-1.9.0/test/test_applicaiton_tags.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/test/test_histogram_impl.py` & `wavefront-sdk-python-1.9.0/test/test_histogram_impl.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/test/test_wavefront_client.py` & `wavefront-sdk-python-1.9.0/test/test_wavefront_client.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/test/test_wavefront_metrics_registry.py` & `wavefront-sdk-python-1.9.0/test/test_wavefront_metrics_registry.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/test/test_wavefront_python_sdk.py` & `wavefront-sdk-python-1.9.0/test/test_wavefront_python_sdk.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/__init__.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,24 +5,19 @@
 
 @author Hao Song (songhao@vmware.com)
 """
 
 import pkg_resources
 
 from .client_factory import WavefrontClientFactory
-from .direct import WavefrontDirectClient
-from .proxy import WavefrontProxyClient
 
 
-__all__ = ['WavefrontDirectClient',
-           'WavefrontProxyClient',
-           'WavefrontClientFactory']
+__all__ = ['WavefrontClientFactory']
 
 __version__ = None
 
 try:
     __version__ = pkg_resources.get_distribution(
-        'wavefront-sdk-python'
-    ).version
+            'wavefront-sdk-python').version
 except pkg_resources.DistributionNotFound:
     # __version__ is only available when distribution is installed.
     pass
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/client.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,19 @@
     WAVEFRONT_HISTOGRAM_FORMAT = 'histogram'
     WAVEFRONT_TRACING_SPAN_FORMAT = 'trace'
     WAVEFRONT_SPAN_LOG_FORMAT = 'spanLogs'
     WAVEFRONT_EVENT_FORMAT = 'event'
 
     REPORT_END_POINT = '/report'
     EVENT_END_POINT = '/api/v2/event'
+    HTTP_TIMEOUT = 60.0
 
     def __init__(self, server, token, max_queue_size=50000, batch_size=10000,
-                 flush_interval_seconds=5, enable_internal_metrics=True):
+                 flush_interval_seconds=5, enable_internal_metrics=True,
+                 queue_impl=queue.Queue):
         # pylint: disable=too-many-arguments,too-many-statements
         """Construct Direct Client.
 
         @param server: Server address,
         @type server: str
         @param token: Server token,
         @type token: str
@@ -64,38 +66,40 @@
         super().__init__()
         self.server = server
         self._token = token
         self._max_queue_size = max_queue_size
         self._batch_size = batch_size
         self._flush_interval_seconds = flush_interval_seconds
         self._default_source = socket.gethostname() or 'unknown'
-        self._metrics_buffer = queue.Queue(max_queue_size)
-        self._histograms_buffer = queue.Queue(max_queue_size)
-        self._tracing_spans_buffer = queue.Queue(max_queue_size)
-        self._spans_log_buffer = queue.Queue(max_queue_size)
-        self._events_buffer = queue.Queue(max_queue_size)
-        self._headers = {'Content-Type': 'application/octet-stream',
-                         'Content-Encoding': 'gzip'}
-        self._event_headers = {'Content-Type': 'application/json',
-                               'Content-Encoding': 'gzip'}
+        self._metrics_buffer = queue_impl(max_queue_size)
+        self._histograms_buffer = queue_impl(max_queue_size)
+        self._tracing_spans_buffer = queue_impl(max_queue_size)
+        self._spans_log_buffer = queue_impl(max_queue_size)
+        self._events_buffer = queue_impl(max_queue_size)
+        self._headers = {'Content-Type': 'application/octet-stream'}
+        self._event_headers = {'Content-Type': 'application/json'}
         self._closed = False
-        self._schedule_lock = threading.Lock()
+        self._schedule_lock = threading.RLock()
         self._timer = None
         self._schedule_timer()
+        self._session = requests.Session()
+        self._session.headers.update({'Content-Encoding': 'gzip'})
+        self._session.timeout = self.HTTP_TIMEOUT
 
         if token:
-            self._headers['Authorization'] = 'Bearer ' + token
-            self._event_headers['Authorization'] = 'Bearer ' + token
+            self._session.headers.update({'Authorization': 'Bearer ' + token})
             ingestion_type = 'direct'
         else:
             ingestion_type = 'proxy'
 
         if enable_internal_metrics:
+            version = utils.get_version(constants.WAVEFRONT_SDK_PYTHON)
             self._sdk_metrics_registry = registry.WavefrontSdkMetricsRegistry(
                 wf_metric_sender=self,
+                tags={'version': version},
                 prefix=f'{constants.SDK_METRIC_PREFIX}'
                        f'.core.sender.{ingestion_type}'
             )
         else:
             self._sdk_metrics_registry = registry.WavefrontSdkMetricsRegistry(
                 wf_metric_sender=None)
         self._sdk_metrics_registry.new_gauge(
@@ -184,24 +188,26 @@
         @param entity_prefix: Type of metric
         @type: str
         @param report_errors: metrics registry to report errors
         @type: metrics registry
         """
         try:
             if data_format == self.WAVEFRONT_EVENT_FORMAT and self._token:
-                response = requests.post(self.server + self.EVENT_END_POINT,
-                                         params=None,
-                                         headers=self._event_headers,
-                                         data=points)
+                response = self._session.post(
+                    self.server + self.EVENT_END_POINT,
+                    headers=self._event_headers,
+                    data=points)
             else:
                 params = {'f': data_format}
                 compressed_data = utils.gzip_compress(points.encode('utf-8'))
-                response = requests.post(self.server + self.REPORT_END_POINT,
-                                         params=params, headers=self._headers,
-                                         data=compressed_data)
+                response = self._session.post(
+                    self.server + self.REPORT_END_POINT,
+                    headers=self._headers,
+                    data=compressed_data,
+                    params=params)
 
             self._sdk_metrics_registry.new_delta_counter(
                 f'{entity_prefix}.report.{response.status_code}').inc()
             response.raise_for_status()
         except Exception as error:
             report_errors.inc()
             raise error
@@ -321,15 +327,15 @@
                                                   source, tags,
                                                   self._default_source)
             self._points_valid.inc()
         except ValueError as error:
             self._points_invalid.inc()
             raise error
         try:
-            self._metrics_buffer.put(line_data)
+            self._metrics_buffer.put_nowait(line_data)
         except queue.Full as error:
             self._points_dropped.inc()
             raise error
 
     def send_metric_now(self, metrics):
         """Send a list of metrics immediately.
 
@@ -372,15 +378,15 @@
                                                      timestamp, source, tags,
                                                      self._default_source)
             self._histograms_valid.inc()
         except ValueError as error:
             self._histograms_invalid.inc()
             raise error
         try:
-            self._histograms_buffer.put(line_data)
+            self._histograms_buffer.put_nowait(line_data)
         except queue.Full as error:
             self._histograms_dropped.inc()
             raise error
 
     def send_distribution_now(self, distributions):
         """Send a list of distribution immediately.
 
@@ -433,28 +439,28 @@
                 name, start_millis, duration_millis, source, trace_id, span_id,
                 parents, follows_from, tags, span_logs, self._default_source)
             self._spans_valid.inc()
         except ValueError as error:
             self._spans_invalid.inc()
             raise error
         try:
-            self._tracing_spans_buffer.put(line_data)
+            self._tracing_spans_buffer.put_nowait(line_data)
         except queue.Full as error:
             self._spans_dropped.inc()
             raise error
         if span_logs:
             try:
                 line_data = utils.span_log_to_line_data(trace_id, span_id,
-                                                        span_logs)
+                                                        span_logs, line_data)
                 self._span_logs_valid.inc()
             except ValueError as error:
                 self._span_logs_invalid.inc()
                 raise error
             try:
-                self._spans_log_buffer.put(line_data)
+                self._spans_log_buffer.put_nowait(line_data)
             except queue.Full as error:
                 self._span_logs_dropped.inc()
                 raise error
 
     def send_span_now(self, spans):
         """
         Send a list of spans immediately.
@@ -519,15 +525,15 @@
                                                      annotations,
                                                      self._default_source)
             self._events_valid.inc()
         except ValueError as error:
             self._events_invalid.inc()
             raise error
         try:
-            self._events_buffer.put(line_data)
+            self._events_buffer.put_nowait(line_data)
         except queue.Full as error:
             self._events_dropped.inc()
             raise error
 
     def send_event_now(self, events):
         """Send a list of events immediately.
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/client_factory.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/client_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Wavefront MultiClient to support Data Ingestion for Multiple Clients.
 
 @author Yogesh Prasad Kurmi (ykurmi@vmware.com)
 """
 
+import queue
 from urllib.parse import urlparse
 
 from wavefront_sdk.client import WavefrontClient
 from wavefront_sdk.multi_clients import WavefrontMultiClient
 
 
-# pylint: disable=W0232  # Class has no __init__ method
 class WavefrontClientFactory:
     """Wavefront client factory.
 
     Create wavefront direct/proxy data ingestion client.
     """
 
     PROXY_SCHEME = "proxy"
@@ -21,23 +21,32 @@
     DIRECT_DATA_INGESTION_SCHEME = "https"
     clients = []
 
     # pylint: disable=too-many-arguments
     def add_client(self, url, max_queue_size=50000,
                    batch_size=10000,
                    flush_interval_seconds=5,
-                   enable_internal_metrics=True):
+                   enable_internal_metrics=True,
+                   queue_impl=queue.Queue):
         """Create a unique client."""
         server, token = self.get_server_info_from_endpoint(url)
 
         if self.existing_client(server):
             raise RuntimeError("client with id " + url + " already exists.")
-        self.clients.append(WavefrontClient(server, token, max_queue_size,
-                                            batch_size, flush_interval_seconds,
-                                            enable_internal_metrics))
+
+        client = WavefrontClient(
+            server=server,
+            token=token,
+            max_queue_size=max_queue_size,
+            batch_size=batch_size,
+            flush_interval_seconds=flush_interval_seconds,
+            enable_internal_metrics=enable_internal_metrics,
+            queue_impl=queue_impl,
+        )
+        self.clients.append(client)
 
     def get_server_info_from_endpoint(self, url):
         """Get Server and API token from the end point.
 
         Return None for token if URL belongs to proxy.
         """
         base_url = urlparse(url)
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/__init__.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/__init__.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/application_tags.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/application_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,13 +90,14 @@
 
     def add_custom_tag_from_env(self, tag_key, var_key):
         """Set a custom tag from the given environment variable.
 
         @param tag_key: Key of the custom tag
         @param var_name: Key of the environment variable
         """
+        # pylint: disable=broad-exception-raised
         if var_key in os.environ:
             value = os.environ[var_key]
             if value:
                 self._custom_tags.append((tag_key, value))
         else:
             raise Exception("var_key is an invalid environment variable.")
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/connection_handler.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/connection_handler.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/constants.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/constants.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/heartbeater_service.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/heartbeater_service.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/counter.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/counter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class WavefrontSdkCounter(metrics.WavefrontSdkMetric):
     """Wavefront SDK Counter."""
 
     def __init__(self):
         """Construct Wavefront SDK Counter."""
-        self._lock = threading.Lock()
+        self._lock = threading.RLock()
         self._count = 0
 
     def inc(self, val=1):
         """Increase the value of the counter."""
         with self._lock:
             self._count += val
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/gauge.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/gauge.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/metrics/registry.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/metrics/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.wf_metric_sender = wf_metric_sender
         self.source = source
         self.tags = tags
         self.prefix = '' if not prefix else prefix + '.'
         self.reporting_interval_secs = reporting_interval_secs
         self.metrics = {}
         self._closed = False
-        self._schedule_lock = threading.Lock()
+        self._schedule_lock = threading.RLock()
         self._timer = None
         if wf_metric_sender:
             self._schedule_timer()
 
     def _schedule_timer(self):
         if not self._closed:
             self._timer = threading.Timer(self.reporting_interval_secs,
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/proxy_connection_handler.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/proxy_connection_handler.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/common/utils.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/common/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
     def __init__(self, initial=0):
         """Construct Atomic Counter.
 
         @param initial: Initial value of the counter
         """
         self.value = initial
-        self._lock = threading.Lock()
+        self._lock = threading.RLock()
 
     def increment(self, num=1):
         """Increment atomic counter value.
 
         @param num: Num to be increased, 1 by default
         @return: Current value after increment
         """
@@ -363,26 +363,28 @@
                 str_builder.append(cur_tag)
                 tag_set.add(cur_tag)
     str_builder.append(str(start_millis))
     str_builder.append(str(duration_millis))
     return ' '.join(str_builder) + '\n'
 
 
-def span_log_to_line_data(trace_id, span_id, span_logs, scrambler=None):
+def span_log_to_line_data(trace_id, span_id, span_logs, span, scrambler=None):
     """Wavefront Tracing Span Log JSON format.
 
     @param trace_id: Trace ID
     @param span_id: Span ID
     @param span_logs: Span Log
+    @param span: Span line
     @param scrambler: Additional UUID, optional
     @return: Span Log in JSON Format
     """
     span_log_json = {'traceId': str(trace_id),
                      'spanId': str(span_id),
-                     'logs': span_logs}
+                     'logs': span_logs,
+                     'span': str(span)}
     if scrambler:
         span_log_json['_scrambler'] = str(scrambler)
     return json.dumps(span_log_json, default=lambda o: o.__dict__) + '\n'
 
 
 # pylint: disable=too-many-branches
 def event_to_json(name, start_time, end_time, source, tags,
@@ -429,29 +431,43 @@
     if tags:
         validate_tags(tags)
         event['tags'] = tags
 
     return str(json.dumps(event))
 
 
-def get_sem_ver(name):
-    """Return semantic version of sdk used in Wavefront reportable format.
-
-    Ex: <major>.<2-digit-minor><2-digit-patch> (1.0603 => v1.6.3)
+def get_version(name):
+    """Return semantic version of sdk used ex: 'v1.6.3'.
 
     @param name: SDK Name
     @type name: str
-    @return: Semantic version in wavefront format as String
+    @return: The version of this library. ex: 'v1.6.3' If version can't be
+      found, returns 'unknown'
     """
     try:
         version = pkg_resources.require(name)[0].version
-        return get_sem_ver_value(version)
+        return "v" + version
     except pkg_resources.DistributionNotFound:
         LOGGER.warning('Unable to get version info,'
                        ' No distribution found for : %s', name)
+    return "unknown"
+
+
+def get_sem_ver(name):
+    """Return semantic version of sdk used in Wavefront reportable format.
+
+    Ex: <major>.<2-digit-minor><2-digit-patch> (1.0603 => v1.6.3)
+
+    @param name: SDK Name
+    @type name: str
+    @return: Semantic version in wavefront format as String. Ex: '1.0603'
+    """
+    version = get_version(name)
+    if version.startswith('v'):
+        return get_sem_ver_value(version[1:])
     return "0.0"
 
 
 def get_sem_ver_value(version):
     """Return semantic version of sdk in Wavefront reportable format.
 
     Ex: <major>.<2-digit-minor><2-digit-patch> (1.0603 => v1.6.3)
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/direct.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/direct.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,25 +40,27 @@
     WAVEFRONT_HISTOGRAM_FORMAT = 'histogram'
     WAVEFRONT_TRACING_SPAN_FORMAT = 'trace'
     WAVEFRONT_SPAN_LOG_FORMAT = 'spanLogs'
     WAVEFRONT_EVENT_FORMAT = 'event'
 
     REPORT_END_POINT = '/report'
     EVENT_END_POINT = '/api/v2/event'
+    HTTP_TIMEOUT = 60.0
 
     # pylint: disable=too-many-arguments
     # pylint: disable=too-many-statements
 
     def __init__(self,
                  server,
                  token,
                  max_queue_size=50000,
                  batch_size=10000,
                  flush_interval_seconds=5,
-                 enable_internal_metrics=True):
+                 enable_internal_metrics=True,
+                 queue_impl=queue.Queue):
         """Construct Direct Client.
 
         @param server: Server address, Example: https://INSTANCE.wavefront.com
         @type server: str
         @param token: Token with Direct Data Ingestion permission granted
         @type token: str
         @param max_queue_size:
@@ -74,27 +76,27 @@
         super().__init__()
         self.server = server
         self._token = token
         self._max_queue_size = max_queue_size
         self._batch_size = batch_size
         self._flush_interval_seconds = flush_interval_seconds
         self._default_source = socket.gethostname() or 'unknown'
-        self._metrics_buffer = queue.Queue(max_queue_size)
-        self._histograms_buffer = queue.Queue(max_queue_size)
-        self._tracing_spans_buffer = queue.Queue(max_queue_size)
-        self._spans_log_buffer = queue.Queue(max_queue_size)
-        self._events_buffer = queue.Queue(max_queue_size)
+        self._metrics_buffer = queue_impl(max_queue_size)
+        self._histograms_buffer = queue_impl(max_queue_size)
+        self._tracing_spans_buffer = queue_impl(max_queue_size)
+        self._spans_log_buffer = queue_impl(max_queue_size)
+        self._events_buffer = queue_impl(max_queue_size)
         self._headers = {'Content-Type': 'application/octet-stream',
                          'Content-Encoding': 'gzip',
                          'Authorization': 'Bearer ' + token}
         self._event_headers = {'Content-Type': 'application/json',
                                'Content-Encoding': 'gzip',
                                'Authorization': 'Bearer ' + token}
         self._closed = False
-        self._schedule_lock = threading.Lock()
+        self._schedule_lock = threading.RLock()
         self._timer = None
 
         if enable_internal_metrics:
             self._sdk_metrics_registry = registry.WavefrontSdkMetricsRegistry(
                 wf_metric_sender=self,
                 prefix=f'{constants.SDK_METRIC_PREFIX}.core.sender.direct')
         else:
@@ -191,22 +193,24 @@
         """
         status_code = constants.NO_HTTP_RESPONSE
         try:
             if data_format == self.WAVEFRONT_EVENT_FORMAT:
                 response = requests.post(self.server + self.EVENT_END_POINT,
                                          params=None,
                                          headers=self._event_headers,
-                                         data=points)
+                                         data=points,
+                                         timeout=self.HTTP_TIMEOUT)
             else:
                 params = {'f': data_format}
                 compressed_data = utils.gzip_compress(points.encode('utf-8'))
                 response = requests.post(self.server + self.REPORT_END_POINT,
                                          params=params,
                                          headers=self._headers,
-                                         data=compressed_data)
+                                         data=compressed_data,
+                                         timeout=self.HTTP_TIMEOUT)
             status_code = response.status_code
             self._sdk_metrics_registry.new_delta_counter(
                 f'{entity_prefix}.report.{status_code}').inc()
         except requests.exceptions.RequestException:
             report_errors.inc()
         return status_code
 
@@ -509,15 +513,15 @@
             self._tracing_spans_buffer.put_nowait(line_data)
         except queue.Full as error:
             self._spans_dropped.inc()
             raise error
         if span_logs:
             try:
                 line_data = utils.span_log_to_line_data(
-                    trace_id, span_id, span_logs)
+                    trace_id, span_id, span_logs, line_data)
                 self._span_logs_valid.inc()
             except ValueError as error:
                 self._span_logs_invalid.inc()
                 raise error
             try:
                 self._spans_log_buffer.put_nowait(line_data)
             except queue.Full as error:
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/__init__.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/event/sender.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/event/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/histogram_impl.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/histogram_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """Construct Wavefront Histogram.
 
         @param clock_millis: A function which returns timestamp.
         @type clock_millis: function
         """
         self._clock_millis = clock_millis or self.current_clock_millis
         self._prior_minute_bins_list = []
-        self._lock = threading.Lock()
+        self._lock = threading.RLock()
         self._current_minute_bin = ThreadMinuteBin(
             self._ACCURACY, self.current_minute_millis())
 
     @staticmethod
     def current_clock_millis():
         """Get current time in millisecond."""
         return time.time() * 1000
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/histogram/sender.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/histogram/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/metrics/sender.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/metrics/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/entities/tracing/sender.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/entities/tracing/sender.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/multi_clients.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/multi_clients.py`

 * *Files identical despite different names*

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk/proxy.py` & `wavefront-sdk-python-1.9.0/wavefront_sdk/proxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,24 +336,25 @@
         try:
             line_data = utils.tracing_span_to_line_data(
                 name, start_millis, duration_millis, source, trace_id,
                 span_id, parents, follows_from, tags, span_logs,
                 self._default_source)
             self._spans_valid.inc()
             self._tracing_proxy_connection_handler.send_data(line_data)
-        except ValueError:
+        except ValueError as error:
             self._spans_invalid.inc()
+            raise error
         except Exception as error:
             self._spans_dropped.inc()
             self._tracing_proxy_connection_handler.increment_failure_count()
             raise error
         if span_logs:
             try:
                 span_log_line_data = utils.span_log_to_line_data(
-                    trace_id, span_id, span_logs)
+                    trace_id, span_id, span_logs, line_data)
                 self._span_logs_valid.inc()
                 self._tracing_proxy_connection_handler.send_data(
                     span_log_line_data)
             except ValueError:
                 self._span_logs_invalid.inc()
             except Exception as error:
                 self._span_logs_dropped.inc()
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/PKG-INFO` & `wavefront-sdk-python-1.9.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,88 +1,53 @@
-Metadata-Version: 2.1
-Name: wavefront-sdk-python
-Version: 1.8.2
-Summary: Wavefront Python SDK
-Home-page: https://github.com/wavefrontHQ/wavefront-sdk-python
-Author: Wavefront by VMware
-Author-email: chitimba@wavefront.com
-License: Apache-2.0
-Keywords: Wavefront,Wavefront SDK
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # wavefront-sdk-python
 
-[![travis build status](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://travis-ci.com/wavefrontHQ/wavefront-sdk-python)
+[![Build Status](https://github.com/wavefrontHQ/wavefront-sdk-python/actions/workflows/main.yml/badge.svg)](https://github.com/wavefrontHQ/wavefront-sdk-python/actions)
 [![image](https://img.shields.io/pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/l/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
 [![image](https://img.shields.io/pypi/pyversions/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-python/)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/wavefront-sdk-python)
 
 
 ## Table of Content
 * [Prerequisites](#Prerequisites)
-* [Set Up a Wavefront Sender](#set-up-a-wavefront-sender)
-* [Send a Single Data Point to Wavefront](#send-a-single-data-point-to-wavefront)
-* [Send Batch Data to Wavefront](#send-batch-data-to-wavefront)
+* [Set Up a Sender](#set-up-a-sender)
+* [Send a Single Data Point](#send-a-single-data-point)
+* [Send Batch Data](#send-batch-data)
 * [Get the Failure Count](#get-the-failure-count)
 * [Close the Connection](#close-the-connection)
 * [License](#License)
 * [How to Get Support and Contribute](#how-to-get-support-and-contribute)
+* [How to Release](#how-to-release)
+
+# VMware Aria Operations™ for Applications Python SDK
 
-# Welcome to the Wavefront Python SDK
+VMware Aria Operations for Applications (formerly known as Wavefront) Python SDK lets you send raw data from your Python application to Operations for Applications using a wavefront_sender interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python.
 
-Wavefront by VMware Python SDK lets you send raw data from your Python application to Wavefront using a `wavefront_sender` interface. The data is then stored as metrics, histograms, and trace data. This SDK is also referred to as the Wavefront Sender SDK for Python. 
+Although this library is mostly used by the other Operations for Applications Python SDKs to send data to Operations for Applications, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Operations for Applications.
 
-Although this library is mostly used by the other Wavefront Python SDKs to send data to Wavefront, you can also use this SDK directly. For example, you can send data directly from a data store or CSV file to Wavefront.
+Note: We're in the process of updating the product name to Operations for Applications, but in many places we still refer to it as Wavefront.
 
 **Before you start implementing, let us make sure you are using the correct SDK!**
 
 ![Python Sender SDK Decision Tree](docs/python_sender_sdk.png)
 
 > ***Note***:
 > </br>
->   * **This is the Wavefront by VMware SDK for Python (Wavefront Sender SDK for Python)!**
+>   * **This is the VMware Aria Operations for Applications SDK for Python (Sender SDK for Python)!**
 >   If this SDK is not what you were looking for, see the [table](#wavefront-sdks) below.
 
-#### Wavefront SDKs
+#### VMware Aria Operations for Applications SDKs
 <table id="SDKlevels" style="width: 100%">
 <tr>
   <th width="10%">SDK Type</th>
   <th width="45%">SDK Description</th>
   <th width="45%">Supported Languages</th>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-trace-data">OpenTracing SDK</a></td>
-  <td align="justify">Implements the OpenTracing specification. Lets you define, collect, and report custom trace data from any part of your application code. <br>Automatically derives Rate Errors Duration (RED) metrics from the reported spans. </td>
-  <td>
-    <ul>
-    <li>
-      <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-java">OpenTracing SDK</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-bundle-java">Tracing Agent</a>
-    </li>
-    <li>
-      <b>Python</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-python">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>Go</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-go">OpenTracing SDK</a>
-    </li>
-    <li>
-      <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-opentracing-sdk-csharp">OpenTracing SDK</a>
-    </li>
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-collecting-metrics-and-histograms">Metrics SDK</a></td>
   <td align="justify">Implements a standard metrics library. Lets you define, collect, and report custom business metrics and histograms from any part of your application code.   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-dropwizard-metrics-sdk-java">Dropwizard</a> <b>|</b> <a href ="https://github.com/wavefrontHQ/wavefront-runtime-sdk-jvm">JVM</a>
     </li>
@@ -96,30 +61,16 @@
     <b>.Net/C#</b>: <a href ="https://github.com/wavefrontHQ/wavefront-appmetrics-sdk-csharp">App Metrics SDK</a>
     </li>
     </ul>
   </td>
 </tr>
 
 <tr>
-  <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-that-instrument-frameworks">Framework SDK</a></td>
-  <td align="justify">Reports predefined traces, metrics, and histograms from the APIs of a supported app framework. Lets you get started quickly with minimal code changes.</td>
-  <td>
-    <ul>
-    <li><b>Java</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-dropwizard-sdk-java">Dropwizard</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-gRPC-sdk-java">gRPC</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jaxrs-sdk-java">JAX-RS</a> <b>|</b> <a href="https://github.com/wavefrontHQ/wavefront-jersey-sdk-java">Jersey</a></li>
-    <li><b>.Net/C#</b>:
-    <a href="https://github.com/wavefrontHQ/wavefront-aspnetcore-sdk-csharp">ASP.Net core</a> </li>
-    <!--- [Python](wavefront_sdks_python.html#python-sdks-that-instrument-frameworks) --->
-    </ul>
-  </td>
-</tr>
-
-<tr>
   <td><a href="https://docs.wavefront.com/wavefront_sdks.html#sdks-for-sending-raw-data-to-wavefront">Sender SDK</a></td>
-  <td align="justify">Lets you send raw data to Wavefront for storage as metrics, histograms, or traces, e.g., to import CSV data into Wavefront.
+  <td align="justify">Lets you send raw data for storage as metrics, histograms, or traces, e.g., to import CSV data into the service.
   </td>
   <td>
     <ul>
     <li>
     <b>Java</b>: <a href ="https://github.com/wavefrontHQ/wavefront-sdk-java">Sender SDK</a>
     </li>
     <li>
@@ -139,59 +90,59 @@
 </tr>
 
 </tbody>
 </table>
 
 ## Prerequisites
 
-* Python ~~2.7+~~ and Python 3.x are supported.
+* Python versions 3.7 - 3.11 are supported.
 * Install `wavefront-sdk-python`
     ```
     pip install wavefront-sdk-python
     ```
 
-## Set Up a Wavefront Sender
+## Set Up a Sender
 
-You can send metrics, histograms, or trace data from your application to the Wavefront service using a Wavefront proxy or direct ingestions.
+You can send metrics, histograms, or trace data from your application to the service using a Wavefront Proxy or direct ingestions.
 
-* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the Wavefront service. This is the simplest way to get up and running quickly.
-* Use a [**Wavefront proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the Wavefront service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
+* Use [**direct ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data directly to the service. This is the simplest way to get up and running quickly.
+* Use a [**Wavefront Proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data to the service. This is the recommended choice for a large-scale deployment that needs resilience to internet outages, control over data queuing and filtering, and more.
 
 You instantiate an object that corresponds to your choice:
 * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront service.
-* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy.
-* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to a Wavefront service directly or via proxy.
+* Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront Proxy.
+* Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the service directly or via proxy.
 > **Deprecated implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy version 7.0 onwards. We recommend all new applications to use the `WavefrontClient`.*
 
 ### Option 1: Create a WavefrontDirectClient
-When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the Wavefront URL and API token to send data directly to Wavefront.
+When sending data via direct ingestion, you need to create a `WavefrontDirectClient`, and build it with the cluster URL and API token to send data directly to the service.
 
 >**Prerequisites**
 > * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-> * The URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `https://<domain>.wavefront.com`.
+> * The URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `https://<domain>.wavefront.com`.
 > * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 #### Initialize the WavefrontDirectClient
 You initialize a `WavefrontDirectClient` by providing the access information you obtained in the Prerequisites section..
 
 Optionally, you can specify parameters to tune the following ingestion properties:
 
-* Max queue size - Internal buffer capacity of the Wavefront sender. Any data in excess of this size is dropped.
-* Flush interval - Interval for flushing data from the Wavefront sender directly to Wavefront.
-* Batch size - Amount of data to send to Wavefront in each flush interval.
+* Max queue size - Internal buffer capacity of the sender. Any data in excess of this size is dropped.
+* Flush interval - Interval for flushing data from the sender directly to the service.
+* Batch size - Amount of data to send to the service in each flush interval.
 
-Together, the batch size and flush interval control the maximum theoretical throughput of the Wavefront sender. You should override the defaults _only_ to set higher values.
+Together, the batch size and flush interval control the maximum theoretical throughput of the sender. You should override the defaults _only_ to set higher values.
 
 
 ```python
 from wavefront_sdk import WavefrontDirectClient
 
 # Create a sender with:
-   # your Wavefront URL
-   # a Wavefront API token that was created with direct ingestion permission
+   # your cluster URL
+   # an API token that was created with direct ingestion permission
    # max queue size (in data points). Default: 50,000
    # batch size (in data points). Default: 10,000
    # flush interval  (in seconds). Default: 1 second
 wavefront_sender = WavefrontDirectClient(
     server="<SERVER_ADDR>",
     token="<TOKEN>",
     max_queue_size=50000,
@@ -201,17 +152,17 @@
 ```
 
 ### Option 2: Create a WavefrontProxyClient
 
 >**Prerequisite** <br/>
 >Before your application can use a `WavefrontProxyClient`, you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
 
-When sending data via the Wavefront proxy, you need to create a `WavefrontProxyClient`. Include the following information.
+When sending data via the Wavefront Proxy, you need to create a `WavefrontProxyClient`. Include the following information.
 
-* The name of the host that will run the Wavefront proxy.
+* The name of the host that will run the Wavefront Proxy.
 * One or more proxy listening ports to send data to. The ports you specify depend on the kinds of data you want to send (metrics, histograms, and/or trace data). You must specify at least one listener port.
 * Optional settings for tuning communication with the proxy.
 
 > **Note**: See [Advanced Proxy Configuration and Installation](https://docs.wavefront.com/proxies_configuring.html) for details.
 
 ```python
 from wavefront_sdk import WavefrontProxyClient
@@ -227,32 +178,32 @@
    metrics_port=2878,
    distribution_port=2878,
    tracing_port=30000,
    event_port=2878
 )
 ```
 
-> **Note:** When you set up a Wavefront proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
+> **Note:** When you set up a Wavefront Proxy on the specified proxy host, you specify the port it will listen to for each type of data to be sent. The `WavefrontProxyClient` must send data to the same ports that the Wavefront Proxy listens to. Consequently, the port-related parameters must specify the same port numbers as the corresponding proxy configuration properties:
 
 | `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf` |
 | ----- | -------- |
 | `metrics_port` | `pushListenerPorts=` |
 | `distribution_port` | `histogramDistListenerPorts=` |
 | `tracing_port` | `traceListenerPorts=` |
 
 ### Option 3: Create a WavefrontClient
-Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to a Wavefront service or send data using a Wavefront Proxy.
+Use `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send data directly to the service or send data using a Wavefront Proxy.
 
-The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple Wavefront services.
+The `WavefrontClientFactory` supports multiple client bindings. If more than one client configuration is specified, you can create a `WavefrontMultiClient` instance, which can send data to multiple services.
 ### Prerequisites
-* Sending data via Wavefront proxy?
-  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
+* Sending data via Wavefront Proxy?
+  <br/>Before your application can use a `WavefrontClient` you must [set up and start a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html).
 * Sending data via direct ingestion?
   * Verify that you have the Direct Data Ingestion permission. For details, see [Examine Groups, Roles, and Permissions](https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-permissions).
-  * The HTTP URL of your Wavefront instance. This is the URL you connect to when you log in to Wavefront, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
+  * The HTTP URL of your cluster. This is the URL you connect to when you log in to the service, typically something like `http://<domain>.wavefront.com`.<br/> You can also use HTTP client with Wavefront Proxy version 7.0 or newer. Example: `http://proxy.acme.corp:2878`.
   * [Obtain the API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-token).
 
 ### Initialize the WavefrontClient
 ```python
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 # Create a sender with:
@@ -268,48 +219,53 @@
 client_factory.add_client(
     url="<URL for proxy or direct ingestions>",
     max_queue_size=50000,
     batch_size=10000,
     flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client()
 ```
-#### Add multiple clients to client factory to send data to multiple Wavefront services.
+#### Add multiple clients to client factory to send data to multiple services.
 ```
 from wavefront_sdk.client_factory import WavefrontClientFactory
 
 client_factory = WavefrontClientFactory()
 client_factory.add_client("proxy://our.proxy.lb.com:2878")
 client_factory.add_client("https://someToken@DOMAIN.wavefront.com")
 
 # Send traces and spans to the tracing port. If you are directly using the sender SDK to send spans without using any other SDK, use the same port as the customTracingListenerPorts configured in the wavefront proxy. Assume you have installed and started the proxy on <proxy_hostname>.
 client_factory.add_client("http://<proxy_hostname>:30000")
 
 wavefront_sender = client_factory.get_client()
 ```
 
-## Send a Single Data Point to Wavefront
+## Send a Single Data Point
 
-The following examples show how to send a single data point to Wavefront. You use the Wavefront sender you created above.
+The following examples show how to send a single data point to the service. You use the Wavefront Sender you created above.
 
 ### Single Metric or  Delta Counter
 
 ```python
 from uuid import UUID
 
 # Wavefront metrics data format:
 # <metricName> <metricValue> [<timestamp>] source=<source> [pointTags]
 wavefront_sender.send_metric(
-    name="new york.power.usage", value=42422.0, timestamp=1533529977,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="new_york.power.usage",
+    value=42422.0,
+    timestamp=1533529977,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 
 # Wavefront delta counter data format:
 # <metricName> <metricValue> source=<source> [pointTags]
 wavefront_sender.send_delta_counter(
-    name="delta.counter", value=1.0,
-    source="localhost", tags={"datacenter": "dc1"})
+    name="delta.counter",
+    value=1.0,
+    source="localhost",
+    tags={"datacenter": "dc1"})
 ```
 ***Note***: If your metric name has a bad character, that character is replaced with a `-`.
 
 ### Single Histogram Distribution
 
 ```python
 from uuid import UUID
@@ -318,71 +274,87 @@
 # Wavefront histogram data format:
 # {!M | !H | !D} [<timestamp>] #<count> <mean> [centroids] <histogramName> source=<source> [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day
 # "!M 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west"
 wavefront_sender.send_distribution(
-    name="request.latency", centroids=[(30, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.DAY,
                              histogram_granularity.HOUR,
                              histogram_granularity.MINUTE},
-    timestamp=1533529977, source="appServer1", tags={"region": "us-west"})
+    timestamp=1533529977,
+    source="appServer1",
+    tags={"region": "us-west"})
 ```
 
 ### Single Span
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with the Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 
 # Wavefront trace and span data format:
 # <tracingSpanName> source=<source> [pointTags] <start_millis> <duration_milliseconds>
 # Example: "getAllUsers source=localhost
 #           traceId=7b3bf470-9456-11e8-9eb6-529269fb1459
 #           spanId=0313bafe-9457-11e8-9eb6-529269fb1459
 #           parent=2f64e538-9457-11e8-9eb6-529269fb1459
 #           application=Wavefront http.method=GET
 #           1533529977 343500"
 wavefront_sender.send_span(
-    name="getAllUsers", start_millis=1533529977, duration_millis=343500,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1533529977,
+    duration_millis=343500,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
-    follows_from=None, tags=[("application", "Wavefront"),
-                             ("service", "istio"),
-                             ("http.method", "GET")],
+    follows_from=None,
+    tags=[("application", "Wavefront"),
+          ("service", "istio"),
+          ("http.method", "GET")],
     span_logs=None)
 ```
 
 ### Single Event
 
 ```python
 # Wavefront event format:
 # @Event <StartTime> <EndTime> "<EventName>"  severity="<Severity>"
 # type="<Type>" details="<EventDetail>" host="<Source>" tag="<Tags>"
-wavefront_sender.send_event('event name', 1592200048, 1592201048, "localhost",
-    ["env:", "dev"], {"severity": "info", "type": "backup", "details": "broker backup"})
+wavefront_sender.send_event('event name',
+                            1592200048,
+                            1592201048,
+                            "localhost",
+                            ["env:", "dev"],
+                            {"severity": "info",
+                             "type": "backup",
+                             "details": "broker backup"})
 ```
 
-## Send Batch Data to Wavefront
+## Send Batch Data
 
 The following examples show how to generate data points manually and send them as a batch to Wavefront.
 
 ### Batch Metrics
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import metric_to_line_data
 
 # Generate string data in Wavefront metric format
 one_metric_data = metric_to_line_data(
-    name="new-york.power.usage", value=42422, timestamp=1493773500,
-    source="localhost", tags={"datacenter": "dc1"},
+    name="new-york.power.usage",
+    value=42422,
+    timestamp=1493773500,
+    source="localhost",
+    tags={"datacenter": "dc1"},
     default_source="defaultSource")
 
 # Result of one_metric_data:
   # '"new-york.power.usage" 42422.0 1493773500 source="localhost" "datacenter"="dc1"\n'
 
 # List of data
 batch_metric_data = [one_metric_data, one_metric_data]
@@ -397,19 +369,22 @@
 ```python
 from uuid import UUID
 from wavefront_sdk.entities.histogram import histogram_granularity
 from wavefront_sdk.common import histogram_to_line_data
 
 # Generate string data in Wavefront histogram format
 one_histogram_data = histogram_to_line_data(
-    name="request.latency", centroids=[(30.0, 20), (5.1, 10)],
+    name="request.latency",
+    centroids=[(30.0, 20), (5.1, 10)],
     histogram_granularities={histogram_granularity.MINUTE,
                              histogram_granularity.HOUR,
                              histogram_granularity.DAY},
-    timestamp=1493773500, source="appServer1", tags={"region": "us-west"},
+    timestamp=1493773500,
+    source="appServer1",
+    tags={"region": "us-west"},
     default_source ="defaultSource")
 
 # Result of one_histogram_data:
   # '!D 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !H 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n
   # !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n'
 
@@ -417,29 +392,33 @@
 batch_histogram_data = [one_histogram_data, one_histogram_data]
 
 # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data)
 ```
 ### Batch Trace Data
 
-If you are directly using the Sender SDK to send data to Wavefront, you won’t see span-level RED metrics by default unless you use the Wavefront proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
+If you are directly using the Sender SDK to send data to the service, you won’t see span-level RED metrics by default unless you use the Wavefront Proxy and define a custom tracing port (`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs](https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-application-with-wavefront-sender-sdks) for details.
 
 ```python
 from uuid import UUID
 from wavefront_sdk.common import tracing_span_to_line_data
 
 # Generate string data in Wavefront tracing span format
 one_tracing_span_data = tracing_span_to_line_data(
-    name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-    source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
+    name="getAllUsers",
+    start_millis=1552949776000,
+    duration_millis=343,
+    source="localhost",
+    trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
     span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
     parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")],
     follows_from=[UUID("5f64e538-9457-11e8-9eb6-529269fb1459")],
     tags=[("application", "Wavefront"), ("http.method", "GET")],
-    span_logs=None, default_source="defaultSource")
+    span_logs=None,
+    default_source="defaultSource")
 
 # Result of one_tracing_span_data:
   # '"getAllUsers" source="localhost" traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe-
   # 9457-11e8-9eb6-529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
   # 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000 343\n'
 
 # List of data
@@ -451,16 +430,23 @@
 
 ### Batch Events
 
 ```python
 from wavefront_sdk.common import event_to_line_data
 
 # Generate string data in Wavefront event format
-one_event_data = event_to_line_data(name="event name", start_time=1592200048, end_time=1592201048,
- source="localhost", tags=["env", "dev"], annotations={"severity": "info", "type": "backup", "details": "broker backup"})
+one_event_data = event_to_line_data(
+    name="event name",
+    start_time=1592200048,
+    end_time=1592201048,
+    source="localhost",
+    tags=["env", "dev"],
+    annotations={"severity": "info",
+                 "type": "backup",
+                 "details": "broker backup"})
 
 # Result of one_event_data:
 # '@Event 1592200048 1592201048 "event name" severity="info" type="backup" details="broker backup"
 # host="localhost" tag="env" tag="dev"\n'
 
 # List of events
 batch_event_data = [one_event_data, one_event_data]
@@ -475,34 +461,34 @@
 
 ```python
 # Get the total failure count
 total_failures = wavefront_sender.get_failure_count()
 ```
 ## Close the Connection
 
-* If the Wavefront sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
+* If the sender is from a `WavefrontClientFactory`, close the connection before shutting down the application.
 
     ```python
     # To shut down a sender from a WavefrontClientFactory
     wavefront_sender = client_factory.get_client()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
+* If the sender is a `WavefrontDirectClient`, flush all buffers and then close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontDirectClient
     # Flush all buffers.
     wavefront_sender.flush_now()
 
     # Close the sender connection
     wavefront_sender.close()
     ```
-* If the Wavefront sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
+* If the sender is a `WavefrontProxyClient`, close the connection before shutting down the application.
 
     ```python
     # To shut down a WavefrontProxyClient
 
     # Close the sender connection
     wavefront_sender.close()
     ```
@@ -518,8 +504,24 @@
   (last number). For backward compatible changes to the API, update the
   minor version (second number), and zero out the patch version. For breaking
   changes to the API, increment the major version (first number) and zero out
   the minor and patch versions.
 * Reach out to us on our public [Slack channel](https://www.wavefront.com/join-public-slack).
 * If you run into any issues, let us know by creating a GitHub issue.
 
+## How to Release
 
+1. Merge all the changes that need to go into the release to the master branch.
+2. Open the `setup.py` file from the top level directory of the project.
+3. Search for version= in the file to find the version number, for example 1.8.15.
+4. Create a pull request, get it reviewed and approved, and merge it after approval.
+5. Check [test.pypi.org](https://test.pypi.org/project/wavefront-sdk-python) for a published package, make sure it's production ready.
+6. Log in to GitHub, click Releases on the right, and click Draft a new release.
+7. For **Choose a tag**, choose the version you found in step 3, and prefix it with `v` for example `v1.8.15`. You need to enter the version where it says **Find or create new tag**.
+
+<img src="images/choose-version.png" alt="A diagram that shows how to choose version"/>
+
+8. Provide a short but descriptive title for the release.
+9. Fill in the details of the release. Please copy the markdown from the previous release and follow the same format.
+10. Click **Publish release.** to start publishing the release to pypi.org.
+11. From the GitHub top navigation bar of this project, click the **Actions** tab. On the first line of the list of workflows, you should see a workflow running that will publish your release to pypi.org.
+12. When the workflow from step 9 has a green checkmark next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/) and verify that the latest version is published.
```

#### html2text {}

```diff
@@ -1,218 +1,198 @@
-Metadata-Version: 2.1 Name: wavefront-sdk-python Version: 1.8.2 Summary:
-Wavefront Python SDK Home-page: https://github.com/wavefrontHQ/wavefront-sdk-
-python Author: Wavefront by VMware Author-email: chitimba@wavefront.com
-License: Apache-2.0 Keywords: Wavefront,Wavefront SDK Platform: UNKNOWN
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 2.7 Classifier: Programming Language ::
-Python :: 3.5 Classifier: Programming Language :: Python :: 3.6 Classifier:
-Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
-License-File: LICENSE # wavefront-sdk-python [![travis build status](https://
-travis-ci.com/wavefrontHQ/wavefront-sdk-python.svg?branch=master)](https://
-travis-ci.com/wavefrontHQ/wavefront-sdk-python) [![image](https://
-img.shields.io/pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/
-wavefront-sdk-python/) [![image](https://img.shields.io/pypi/l/wavefront-sdk-
-python.svg)](https://pypi.org/project/wavefront-sdk-python/) [![image](https://
+# wavefront-sdk-python [![Build Status](https://github.com/wavefrontHQ/
+wavefront-sdk-python/actions/workflows/main.yml/badge.svg)](https://github.com/
+wavefrontHQ/wavefront-sdk-python/actions) [![image](https://img.shields.io/
+pypi/v/wavefront-sdk-python.svg)](https://pypi.org/project/wavefront-sdk-
+python/) [![image](https://img.shields.io/pypi/l/wavefront-sdk-python.svg)]
+(https://pypi.org/project/wavefront-sdk-python/) [![image](https://
 img.shields.io/pypi/pyversions/wavefront-sdk-python.svg)](https://pypi.org/
-project/wavefront-sdk-python/) ## Table of Content * [Prerequisites]
-(#Prerequisites) * [Set Up a Wavefront Sender](#set-up-a-wavefront-sender) *
-[Send a Single Data Point to Wavefront](#send-a-single-data-point-to-wavefront)
-* [Send Batch Data to Wavefront](#send-batch-data-to-wavefront) * [Get the
-Failure Count](#get-the-failure-count) * [Close the Connection](#close-the-
-connection) * [License](#License) * [How to Get Support and Contribute](#how-
-to-get-support-and-contribute) # Welcome to the Wavefront Python SDK Wavefront
-by VMware Python SDK lets you send raw data from your Python application to
-Wavefront using a `wavefront_sender` interface. The data is then stored as
-metrics, histograms, and trace data. This SDK is also referred to as the
-Wavefront Sender SDK for Python. Although this library is mostly used by the
-other Wavefront Python SDKs to send data to Wavefront, you can also use this
-SDK directly. For example, you can send data directly from a data store or CSV
-file to Wavefront. **Before you start implementing, let us make sure you are
-using the correct SDK!** ![Python Sender SDK Decision Tree](docs/
-python_sender_sdk.png) > ***Note***: >  > * **This is the Wavefront by VMware
-SDK for Python (Wavefront Sender SDK for Python)!** > If this SDK is not what
-you were looking for, see the [table](#wavefront-sdks) below. #### Wavefront
-SDKs
-SDK Type        SDK Description                 Supported Languages
-                Implements the OpenTracing
-                specification. Lets you define,     * Java: OpenTracing_SDK |
-                collect, and report custom            Tracing_Agent
-OpenTracing_SDK trace data from any part of         * Python: OpenTracing_SDK
-                your application code.              * Go: OpenTracing_SDK
-                Automatically derives Rate          * .Net/C#: OpenTracing_SDK
-                Errors Duration (RED) metrics
-                from the reported spans.
-                Implements a standard metrics
-                library. Lets you define,           * Java: Dropwizard | JVM
-Metrics_SDK     collect, and report custom          * Python: Pyformance_SDK
-                business metrics and histograms     * Go: Go_Metrics_SDK
-                from any part of your               * .Net/C#: App_Metrics_SDK
-                application code.
-                Reports predefined traces,
-                metrics, and histograms from        * Java: Dropwizard | gRPC |
-Framework_SDK   the APIs of a supported app           JAX-RS | Jersey
-                framework. Lets you get started     * .Net/C#: ASP.Net_core
-                quickly with minimal code
-                changes.
-                Lets you send raw data to           * Java: Sender_SDK
-                Wavefront for storage as            * Python: Sender_SDK
-Sender_SDK      metrics, histograms, or traces,     * Go: Sender_SDK
-                e.g., to import CSV data into       * .Net/C#: Sender_SDK
-                Wavefront.                          * C++: Sender_SDK
-## Prerequisites * Python ~~2.7+~~ and Python 3.x are supported. * Install
+project/wavefront-sdk-python/) ![PyPI - Downloads](https://img.shields.io/pypi/
+dm/wavefront-sdk-python) ## Table of Content * [Prerequisites](#Prerequisites)
+* [Set Up a Sender](#set-up-a-sender) * [Send a Single Data Point](#send-a-
+single-data-point) * [Send Batch Data](#send-batch-data) * [Get the Failure
+Count](#get-the-failure-count) * [Close the Connection](#close-the-connection)
+* [License](#License) * [How to Get Support and Contribute](#how-to-get-
+support-and-contribute) * [How to Release](#how-to-release) # VMware Aria
+Operationsâ¢ for Applications Python SDK VMware Aria Operations for
+Applications (formerly known as Wavefront) Python SDK lets you send raw data
+from your Python application to Operations for Applications using a
+wavefront_sender interface. The data is then stored as metrics, histograms, and
+trace data. This SDK is also referred to as the Wavefront Sender SDK for
+Python. Although this library is mostly used by the other Operations for
+Applications Python SDKs to send data to Operations for Applications, you can
+also use this SDK directly. For example, you can send data directly from a data
+store or CSV file to Operations for Applications. Note: We're in the process of
+updating the product name to Operations for Applications, but in many places we
+still refer to it as Wavefront. **Before you start implementing, let us make
+sure you are using the correct SDK!** ![Python Sender SDK Decision Tree](docs/
+python_sender_sdk.png) > ***Note***: >  > * **This is the VMware Aria
+Operations for Applications SDK for Python (Sender SDK for Python)!** > If this
+SDK is not what you were looking for, see the [table](#wavefront-sdks) below.
+#### VMware Aria Operations for Applications SDKs
+SDK Type    SDK Description                      Supported Languages
+            Implements a standard metrics            * Java: Dropwizard | JVM
+            library. Lets you define, collect,       * Python: Pyformance_SDK
+Metrics_SDK and report custom business metrics       * Go: Go_Metrics_SDK
+            and histograms from any part of your     * .Net/C#: App_Metrics_SDK
+            application code.
+            Lets you send raw data for storage       * Java: Sender_SDK
+            as metrics, histograms, or traces,       * Python: Sender_SDK
+Sender_SDK  e.g., to import CSV data into the        * Go: Sender_SDK
+            service.                                 * .Net/C#: Sender_SDK
+                                                     * C++: Sender_SDK
+## Prerequisites * Python versions 3.7 - 3.11 are supported. * Install
 `wavefront-sdk-python` ``` pip install wavefront-sdk-python ``` ## Set Up a
-Wavefront Sender You can send metrics, histograms, or trace data from your
-application to the Wavefront service using a Wavefront proxy or direct
-ingestions. * Use [**direct ingestion**](https://docs.wavefront.com/
-direct_ingestion.html) to send the data directly to the Wavefront service. This
-is the simplest way to get up and running quickly. * Use a [**Wavefront
-proxy**](https://docs.wavefront.com/proxies.html), which then forwards the data
-to the Wavefront service. This is the recommended choice for a large-scale
-deployment that needs resilience to internet outages, control over data queuing
-and filtering, and more. You instantiate an object that corresponds to your
-choice: * Option 1 **(Deprecated)**: [Create a `WavefrontDirectClient`]
-(#option-1-create-a-wavefrontdirectclient) to send data directly to a Wavefront
-service. * Option 2 **(Deprecated)**: [Create a `WavefrontProxyClient`]
-(#option-2-create-a-wavefrontproxyclient) to send data to a Wavefront proxy. *
-Option 3: [Create a `WavefrontClient`](#option-3-create-a-wavefrontclient) to
-send data to a Wavefront service directly or via proxy. > **Deprecated
-implementations**: *`WavefrontDirectClient` and `WavefrontProxyClient` are
-deprecated from proxy version 7.0 onwards. We recommend all new applications to
-use the `WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When
-sending data via direct ingestion, you need to create a
-`WavefrontDirectClient`, and build it with the Wavefront URL and API token to
-send data directly to Wavefront. >**Prerequisites** > * Verify that you have
-the Direct Data Ingestion permission. For details, see [Examine Groups, Roles,
-and Permissions](https://docs.wavefront.com/
-users_account_managing.html#examine-groups-roles-and-permissions). > * The URL
-of your Wavefront instance. This is the URL you connect to when you log in to
-Wavefront, typically something like `https://.wavefront.com`. > * [Obtain the
-API token](http://docs.wavefront.com/wavefront_api.html#generating-an-api-
-token). #### Initialize the WavefrontDirectClient You initialize a
-`WavefrontDirectClient` by providing the access information you obtained in the
-Prerequisites section.. Optionally, you can specify parameters to tune the
-following ingestion properties: * Max queue size - Internal buffer capacity of
-the Wavefront sender. Any data in excess of this size is dropped. * Flush
-interval - Interval for flushing data from the Wavefront sender directly to
-Wavefront. * Batch size - Amount of data to send to Wavefront in each flush
-interval. Together, the batch size and flush interval control the maximum
-theoretical throughput of the Wavefront sender. You should override the
-defaults _only_ to set higher values. ```python from wavefront_sdk import
-WavefrontDirectClient # Create a sender with: # your Wavefront URL # a
-Wavefront API token that was created with direct ingestion permission # max
-queue size (in data points). Default: 50,000 # batch size (in data points).
-Default: 10,000 # flush interval (in seconds). Default: 1 second
-wavefront_sender = WavefrontDirectClient( server="", token="",
-max_queue_size=50000, batch_size=10000, flush_interval_seconds=5 ) ``` ###
-Option 2: Create a WavefrontProxyClient >**Prerequisite**
+Sender You can send metrics, histograms, or trace data from your application to
+the service using a Wavefront Proxy or direct ingestions. * Use [**direct
+ingestion**](https://docs.wavefront.com/direct_ingestion.html) to send the data
+directly to the service. This is the simplest way to get up and running
+quickly. * Use a [**Wavefront Proxy**](https://docs.wavefront.com/
+proxies.html), which then forwards the data to the service. This is the
+recommended choice for a large-scale deployment that needs resilience to
+internet outages, control over data queuing and filtering, and more. You
+instantiate an object that corresponds to your choice: * Option 1 **
+(Deprecated)**: [Create a `WavefrontDirectClient`](#option-1-create-a-
+wavefrontdirectclient) to send data directly to a Wavefront service. * Option 2
+**(Deprecated)**: [Create a `WavefrontProxyClient`](#option-2-create-a-
+wavefrontproxyclient) to send data to a Wavefront Proxy. * Option 3: [Create a
+`WavefrontClient`](#option-3-create-a-wavefrontclient) to send data to the
+service directly or via proxy. > **Deprecated implementations**:
+*`WavefrontDirectClient` and `WavefrontProxyClient` are deprecated from proxy
+version 7.0 onwards. We recommend all new applications to use the
+`WavefrontClient`.* ### Option 1: Create a WavefrontDirectClient When sending
+data via direct ingestion, you need to create a `WavefrontDirectClient`, and
+build it with the cluster URL and API token to send data directly to the
+service. >**Prerequisites** > * Verify that you have the Direct Data Ingestion
+permission. For details, see [Examine Groups, Roles, and Permissions](https://
+docs.wavefront.com/users_account_managing.html#examine-groups-roles-and-
+permissions). > * The URL of your cluster. This is the URL you connect to when
+you log in to the service, typically something like `https://.wavefront.com`. >
+* [Obtain the API token](http://docs.wavefront.com/
+wavefront_api.html#generating-an-api-token). #### Initialize the
+WavefrontDirectClient You initialize a `WavefrontDirectClient` by providing the
+access information you obtained in the Prerequisites section.. Optionally, you
+can specify parameters to tune the following ingestion properties: * Max queue
+size - Internal buffer capacity of the sender. Any data in excess of this size
+is dropped. * Flush interval - Interval for flushing data from the sender
+directly to the service. * Batch size - Amount of data to send to the service
+in each flush interval. Together, the batch size and flush interval control the
+maximum theoretical throughput of the sender. You should override the defaults
+_only_ to set higher values. ```python from wavefront_sdk import
+WavefrontDirectClient # Create a sender with: # your cluster URL # an API token
+that was created with direct ingestion permission # max queue size (in data
+points). Default: 50,000 # batch size (in data points). Default: 10,000 # flush
+interval (in seconds). Default: 1 second wavefront_sender =
+WavefrontDirectClient( server="", token="", max_queue_size=50000,
+batch_size=10000, flush_interval_seconds=5 ) ``` ### Option 2: Create a
+WavefrontProxyClient >**Prerequisite**
 >Before your application can use a `WavefrontProxyClient`, you must [set up and
 start a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html).
-When sending data via the Wavefront proxy, you need to create a
+When sending data via the Wavefront Proxy, you need to create a
 `WavefrontProxyClient`. Include the following information. * The name of the
-host that will run the Wavefront proxy. * One or more proxy listening ports to
+host that will run the Wavefront Proxy. * One or more proxy listening ports to
 send data to. The ports you specify depend on the kinds of data you want to
 send (metrics, histograms, and/or trace data). You must specify at least one
 listener port. * Optional settings for tuning communication with the proxy. >
 **Note**: See [Advanced Proxy Configuration and Installation](https://
 docs.wavefront.com/proxies_configuring.html) for details. ```python from
 wavefront_sdk import WavefrontProxyClient # Create a sender with: # the proxy
 hostname or address # the default listener port (2878) for sending metrics to #
 the recommended listener port (2878) for sending histograms to # the
 recommended listener port (30000) for sending trace data. # if you are directly
 using the sender sdk to send spans without using any other sdk, use the same
 port as the customTracingListenerPorts configured in the wavefront proxy for
 the tracing_port wavefront_sender = WavefrontProxyClient( host="",
 metrics_port=2878, distribution_port=2878, tracing_port=30000, event_port=2878
-) ``` > **Note:** When you set up a Wavefront proxy on the specified proxy
+) ``` > **Note:** When you set up a Wavefront Proxy on the specified proxy
 host, you specify the port it will listen to for each type of data to be sent.
 The `WavefrontProxyClient` must send data to the same ports that the Wavefront
-proxy listens to. Consequently, the port-related parameters must specify the
+Proxy listens to. Consequently, the port-related parameters must specify the
 same port numbers as the corresponding proxy configuration properties: |
 `WavefrontProxyClient()` parameter | Corresponding property in `wavefront.conf`
 | | ----- | -------- | | `metrics_port` | `pushListenerPorts=` | |
 `distribution_port` | `histogramDistListenerPorts=` | | `tracing_port` |
 `traceListenerPorts=` | ### Option 3: Create a WavefrontClient Use
 `WavefrontClientFactory` to create a `WavefrontClient` instance, which can send
-data directly to a Wavefront service or send data using a Wavefront Proxy. The
+data directly to the service or send data using a Wavefront Proxy. The
 `WavefrontClientFactory` supports multiple client bindings. If more than one
 client configuration is specified, you can create a `WavefrontMultiClient`
-instance, which can send data to multiple Wavefront services. ### Prerequisites
-* Sending data via Wavefront proxy?
+instance, which can send data to multiple services. ### Prerequisites * Sending
+data via Wavefront Proxy?
 Before your application can use a `WavefrontClient` you must [set up and start
-a Wavefront proxy](https://docs.wavefront.com/proxies_installing.html). *
+a Wavefront Proxy](https://docs.wavefront.com/proxies_installing.html). *
 Sending data via direct ingestion? * Verify that you have the Direct Data
 Ingestion permission. For details, see [Examine Groups, Roles, and Permissions]
 (https://docs.wavefront.com/users_account_managing.html#examine-groups-roles-
-and-permissions). * The HTTP URL of your Wavefront instance. This is the URL
-you connect to when you log in to Wavefront, typically something like `http:/
+and-permissions). * The HTTP URL of your cluster. This is the URL you connect
+to when you log in to the service, typically something like `http:/
 /.wavefront.com`.
 You can also use HTTP client with Wavefront Proxy version 7.0 or newer.
 Example: `http://proxy.acme.corp:2878`. * [Obtain the API token](http://
 docs.wavefront.com/wavefront_api.html#generating-an-api-token). ### Initialize
 the WavefrontClient ```python from wavefront_sdk.client_factory import
 WavefrontClientFactory # Create a sender with: # Required Parameter # URL
 format to send data via proxy: "proxy://
 proxy.load.balancer.com>:" # URL format to send data via direct ingestion:
 "https://TOKEN@DOMAIN.wavefront.com" # Optional Parameter # max queue size (in
 data points). Default: 50000 # batch size (in data points). Default: 10000 #
 flush interval (in seconds). Default: 1 second client_factory =
 WavefrontClientFactory() client_factory.add_client( url="",
 max_queue_size=50000, batch_size=10000, flush_interval_seconds=5)
 wavefront_sender = client_factory.get_client() ``` #### Add multiple clients to
-client factory to send data to multiple Wavefront services. ``` from
+client factory to send data to multiple services. ``` from
 wavefront_sdk.client_factory import WavefrontClientFactory client_factory =
 WavefrontClientFactory() client_factory.add_client("proxy://our.proxy.lb.com:
 2878") client_factory.add_client("https://someToken@DOMAIN.wavefront.com") #
 Send traces and spans to the tracing port. If you are directly using the sender
 SDK to send spans without using any other SDK, use the same port as the
 customTracingListenerPorts configured in the wavefront proxy. Assume you have
 installed and started the proxy on . client_factory.add_client("http://:30000")
 wavefront_sender = client_factory.get_client() ``` ## Send a Single Data Point
-to Wavefront The following examples show how to send a single data point to
-Wavefront. You use the Wavefront sender you created above. ### Single Metric or
-Delta Counter ```python from uuid import UUID # Wavefront metrics data format:
-#   [] source= [pointTags] wavefront_sender.send_metric( name="new
-york.power.usage", value=42422.0, timestamp=1533529977, source="localhost",
-tags={"datacenter": "dc1"}) # Wavefront delta counter data format: #   source=
-[pointTags] wavefront_sender.send_delta_counter( name="delta.counter",
-value=1.0, source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If
-your metric name has a bad character, that character is replaced with a `-`.
-### Single Histogram Distribution ```python from uuid import UUID from
+The following examples show how to send a single data point to the service. You
+use the Wavefront Sender you created above. ### Single Metric or Delta Counter
+```python from uuid import UUID # Wavefront metrics data format: #   [] source=
+[pointTags] wavefront_sender.send_metric( name="new_york.power.usage",
+value=42422.0, timestamp=1533529977, source="localhost", tags={"datacenter":
+"dc1"}) # Wavefront delta counter data format: #   source= [pointTags]
+wavefront_sender.send_delta_counter( name="delta.counter", value=1.0,
+source="localhost", tags={"datacenter": "dc1"}) ``` ***Note***: If your metric
+name has a bad character, that character is replaced with a `-`. ### Single
+Histogram Distribution ```python from uuid import UUID from
 wavefront_sdk.entities.histogram import histogram_granularity # Wavefront
 histogram data format: # {!M | !H | !D} [] #  [centroids]  source= [pointTags]
 # Example: You can choose to send to at most 3 bins: Minute, Hour, Day # "!M
 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-west" #
 "!H 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1 region=us-
 west" # "!D 1533529977 #20 30.0 #10 5.1 request.latency source=appServer1
 region=us-west" wavefront_sender.send_distribution( name="request.latency",
 centroids=[(30, 20), (5.1, 10)], histogram_granularities=
 {histogram_granularity.DAY, histogram_granularity.HOUR,
 histogram_granularity.MINUTE}, timestamp=1533529977, source="appServer1", tags=
 {"region": "us-west"}) ``` ### Single Span If you are directly using the Sender
-SDK to send data to Wavefront, you wonât see span-level RED metrics by
-default unless you use the Wavefront proxy and define a custom tracing port
-(`tracing_port`). See [Instrument Your Application with Wavefront Sender SDKs]
-(https://docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-
-your-application-with-wavefront-sender-sdks) for details. ```python from uuid
-import UUID # Wavefront trace and span data format: #  source= [pointTags]   #
+SDK to send data to the service, you wonât see span-level RED metrics by
+default unless you use the Wavefront Proxy and define a custom tracing port
+(`tracing_port`). See [Instrument Your Application with the Sender SDKs](https:
+//docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID # Wavefront trace and span data format: #  source= [pointTags]   #
 Example: "getAllUsers source=localhost # traceId=7b3bf470-9456-11e8-9eb6-
 529269fb1459 # spanId=0313bafe-9457-11e8-9eb6-529269fb1459 # parent=2f64e538-
 9457-11e8-9eb6-529269fb1459 # application=Wavefront http.method=GET #
 1533529977 343500" wavefront_sender.send_span( name="getAllUsers",
 start_millis=1533529977, duration_millis=343500, source="localhost",
 trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"), span_id=UUID("0313bafe-
 9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-9457-11e8-9eb6-
 529269fb1459")], follows_from=None, tags=[("application", "Wavefront"),
 ("service", "istio"), ("http.method", "GET")], span_logs=None) ``` ### Single
 Event ```python # Wavefront event format: # @Event   "" severity="" # type=""
 details="" host="" tag="" wavefront_sender.send_event('event name', 1592200048,
 1592201048, "localhost", ["env:", "dev"], {"severity": "info", "type":
-"backup", "details": "broker backup"}) ``` ## Send Batch Data to Wavefront The
-following examples show how to generate data points manually and send them as a
-batch to Wavefront. ### Batch Metrics ```python from uuid import UUID from
+"backup", "details": "broker backup"}) ``` ## Send Batch Data The following
+examples show how to generate data points manually and send them as a batch to
+Wavefront. ### Batch Metrics ```python from uuid import UUID from
 wavefront_sdk.common import metric_to_line_data # Generate string data in
 Wavefront metric format one_metric_data = metric_to_line_data( name="new-
 york.power.usage", value=42422, timestamp=1493773500, source="localhost", tags=
 {"datacenter": "dc1"}, default_source="defaultSource") # Result of
 one_metric_data: # '"new-york.power.usage" 42422.0 1493773500
 source="localhost" "datacenter"="dc1"\n' # List of data batch_metric_data =
 [one_metric_data, one_metric_data] # Send list of data immediately
@@ -229,61 +209,79 @@
 ="defaultSource") # Result of one_histogram_data: # '!D 1493773500 #20 30.0 #10
 5.1 "request.latency" source="appServer1" "region"="us-west"\n # !H 1493773500
 #20 30.0 #10 5.1 "request.latency" source="appServer1" "region"="us-west"\n #
 !M 1493773500 #20 30.0 #10 5.1 "request.latency" source="appServer1"
 "region"="us-west"\n' # List of data batch_histogram_data =
 [one_histogram_data, one_histogram_data] # Send list of data immediately
 wavefront_sender.send_distribution_now(batch_histogram_data) ``` ### Batch
-Trace Data If you are directly using the Sender SDK to send data to Wavefront,
-you wonât see span-level RED metrics by default unless you use the Wavefront
-proxy and define a custom tracing port (`tracing_port`). See [Instrument Your
-Application with Wavefront Sender SDKs](https://docs.wavefront.com/
-tracing_instrumenting_frameworks.html#instrument-your-application-with-
-wavefront-sender-sdks) for details. ```python from uuid import UUID from
-wavefront_sdk.common import tracing_span_to_line_data # Generate string data in
-Wavefront tracing span format one_tracing_span_data = tracing_span_to_line_data
-( name="getAllUsers", start_millis=1552949776000, duration_millis=343,
-source="localhost", trace_id=UUID("7b3bf470-9456-11e8-9eb6-529269fb1459"),
-span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"), parents=[UUID("2f64e538-
-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID("5f64e538-9457-11e8-9eb6-
-529269fb1459")], tags=[("application", "Wavefront"), ("http.method", "GET")],
-span_logs=None, default_source="defaultSource") # Result of
-one_tracing_span_data: # '"getAllUsers" source="localhost" traceId=7b3bf470-
-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-529269fb1459
-parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538- # 9457-11e8-
-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET" 1552949776000
-343\n' # List of data batch_span_data = [one_tracing_span_data,
+Trace Data If you are directly using the Sender SDK to send data to the
+service, you wonât see span-level RED metrics by default unless you use the
+Wavefront Proxy and define a custom tracing port (`tracing_port`). See
+[Instrument Your Application with Wavefront Sender SDKs](https://
+docs.wavefront.com/tracing_instrumenting_frameworks.html#instrument-your-
+application-with-wavefront-sender-sdks) for details. ```python from uuid import
+UUID from wavefront_sdk.common import tracing_span_to_line_data # Generate
+string data in Wavefront tracing span format one_tracing_span_data =
+tracing_span_to_line_data( name="getAllUsers", start_millis=1552949776000,
+duration_millis=343, source="localhost", trace_id=UUID("7b3bf470-9456-11e8-
+9eb6-529269fb1459"), span_id=UUID("0313bafe-9457-11e8-9eb6-529269fb1459"),
+parents=[UUID("2f64e538-9457-11e8-9eb6-529269fb1459")], follows_from=[UUID
+("5f64e538-9457-11e8-9eb6-529269fb1459")], tags=[("application", "Wavefront"),
+("http.method", "GET")], span_logs=None, default_source="defaultSource") #
+Result of one_tracing_span_data: # '"getAllUsers" source="localhost"
+traceId=7b3bf470-9456-11e8-9eb6-529269fb1459 spanId=0313bafe- # 9457-11e8-9eb6-
+529269fb1459 parent=2f64e538-9457-11e8-9eb6-529269fb1459 followsFrom=5f64e538-
+# 9457-11e8-9eb6-529269fb1459 "application"="Wavefront" "http.method"="GET"
+1552949776000 343\n' # List of data batch_span_data = [one_tracing_span_data,
 one_tracing_span_data] # Send list of data immediately
 wavefront_sender.send_span_now(batch_span_data) ``` ### Batch Events ```python
 from wavefront_sdk.common import event_to_line_data # Generate string data in
-Wavefront event format one_event_data = event_to_line_data(name="event name",
+Wavefront event format one_event_data = event_to_line_data( name="event name",
 start_time=1592200048, end_time=1592201048, source="localhost", tags=["env",
 "dev"], annotations={"severity": "info", "type": "backup", "details": "broker
 backup"}) # Result of one_event_data: # '@Event 1592200048 1592201048 "event
 name" severity="info" type="backup" details="broker backup" # host="localhost"
 tag="env" tag="dev"\n' # List of events batch_event_data = [one_event_data,
 one_event_data] # Send list of events immediately
 wavefront_sender.send_event_now(batch_event_data) ``` ## Get the Failure Count
 If the application failed to send metrics, histograms, or trace data via the
 `wavefront_sender`, you can get the total failure count. ```python # Get the
 total failure count total_failures = wavefront_sender.get_failure_count() ```
-## Close the Connection * If the Wavefront sender is from a
-`WavefrontClientFactory`, close the connection before shutting down the
-application. ```python # To shut down a sender from a WavefrontClientFactory
-wavefront_sender = client_factory.get_client() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontDirectClient`, flush all buffers and then close the connection before
-shutting down the application. ```python # To shut down a WavefrontDirectClient
-# Flush all buffers. wavefront_sender.flush_now() # Close the sender connection
-wavefront_sender.close() ``` * If the Wavefront sender is a
-`WavefrontProxyClient`, close the connection before shutting down the
-application. ```python # To shut down a WavefrontProxyClient # Close the sender
-connection wavefront_sender.close() ``` ## License [Apache 2.0 License]
-(LICENSE). ## How to Get Support and Contribute * When submitting changes, be
-sure to increment the version number in setup.py. The version number is
-documented as such in setup.py. We follow semantic versioning. For bug fixes,
-increment the patch version (last number). For backward compatible changes to
-the API, update the minor version (second number), and zero out the patch
-version. For breaking changes to the API, increment the major version (first
-number) and zero out the minor and patch versions. * Reach out to us on our
-public [Slack channel](https://www.wavefront.com/join-public-slack). * If you
-run into any issues, let us know by creating a GitHub issue.
+## Close the Connection * If the sender is from a `WavefrontClientFactory`,
+close the connection before shutting down the application. ```python # To shut
+down a sender from a WavefrontClientFactory wavefront_sender =
+client_factory.get_client() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontDirectClient`,
+flush all buffers and then close the connection before shutting down the
+application. ```python # To shut down a WavefrontDirectClient # Flush all
+buffers. wavefront_sender.flush_now() # Close the sender connection
+wavefront_sender.close() ``` * If the sender is a `WavefrontProxyClient`, close
+the connection before shutting down the application. ```python # To shut down a
+WavefrontProxyClient # Close the sender connection wavefront_sender.close() ```
+## License [Apache 2.0 License](LICENSE). ## How to Get Support and Contribute
+* When submitting changes, be sure to increment the version number in setup.py.
+The version number is documented as such in setup.py. We follow semantic
+versioning. For bug fixes, increment the patch version (last number). For
+backward compatible changes to the API, update the minor version (second
+number), and zero out the patch version. For breaking changes to the API,
+increment the major version (first number) and zero out the minor and patch
+versions. * Reach out to us on our public [Slack channel](https://
+www.wavefront.com/join-public-slack). * If you run into any issues, let us know
+by creating a GitHub issue. ## How to Release 1. Merge all the changes that
+need to go into the release to the master branch. 2. Open the `setup.py` file
+from the top level directory of the project. 3. Search for version= in the file
+to find the version number, for example 1.8.15. 4. Create a pull request, get
+it reviewed and approved, and merge it after approval. 5. Check [test.pypi.org]
+(https://test.pypi.org/project/wavefront-sdk-python) for a published package,
+make sure it's production ready. 6. Log in to GitHub, click Releases on the
+right, and click Draft a new release. 7. For **Choose a tag**, choose the
+version you found in step 3, and prefix it with `v` for example `v1.8.15`. You
+need to enter the version where it says **Find or create new tag**. [A diagram
+that shows how to choose version] 8. Provide a short but descriptive title for
+the release. 9. Fill in the details of the release. Please copy the markdown
+from the previous release and follow the same format. 10. Click **Publish
+release.** to start publishing the release to pypi.org. 11. From the GitHub top
+navigation bar of this project, click the **Actions** tab. On the first line of
+the list of workflows, you should see a workflow running that will publish your
+release to pypi.org. 12. When the workflow from step 9 has a green checkmark
+next to it, go to [pypi.org](https://pypi.org/project/wavefront-sdk-python/
+) and verify that the latest version is published.
```

### Comparing `wavefront-sdk-python-1.8.2/wavefront_sdk_python.egg-info/SOURCES.txt` & `wavefront-sdk-python-1.9.0/wavefront_sdk_python.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 LICENSE
 README.md
 setup.py
 test/__init__.py
 test/test_applicaiton_tags.py
+test/test_client.py
+test/test_direct.py
 test/test_histogram_impl.py
+test/test_proxy.py
 test/test_wavefront_client.py
 test/test_wavefront_metrics_registry.py
 test/test_wavefront_python_sdk.py
 wavefront_sdk/__init__.py
 wavefront_sdk/client.py
 wavefront_sdk/client_factory.py
 wavefront_sdk/direct.py
```

