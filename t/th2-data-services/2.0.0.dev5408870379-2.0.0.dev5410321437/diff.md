# Comparing `tmp/th2_data_services-2.0.0.dev5408870379.tar.gz` & `tmp/th2_data_services-2.0.0.dev5410321437.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5408870379.tar", last modified: Thu Jun 29 05:39:44 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5410321437.tar", last modified: Thu Jun 29 08:55:23 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5408870379.tar` & `th2_data_services-2.0.0.dev5410321437.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-29 05:39:30.000000 th2_data_services-2.0.0.dev5408870379/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     4188 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-06-29 05:38:26.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 05:39:44.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 05:39:43.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-29 05:39:43.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 05:39:43.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-29 05:39:43.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-29 05:39:43.000000 th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23948 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-06-29 08:55:05.000000 th2_data_services-2.0.0.dev5410321437/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36165 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1054 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2682 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4528 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     4366 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4638 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6860 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14697 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10769 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-06-29 08:54:20.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    29227 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-29 08:55:23.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      530 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-29 08:55:22.000000 th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5408870379/PKG-INFO` & `th2_data_services-2.0.0.dev5410321437/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 325f  : 2.1.Name: th2_
 00000020: 6461 7461 5f73 6572 7669 6365 730a 5665  data_services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3534 3038 3837 3033 3739 0a53 756d 6d61  5408870379.Summa
+00000040: 3534 3130 3332 3134 3337 0a53 756d 6d61  5410321437.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5408870379/README.md` & `th2_data_services-2.0.0.dev5410321437/README.md`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/setup.py` & `th2_data_services-2.0.0.dev5410321437/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/config/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from th2_data_services.interfaces.utils.resolver import EventFieldsResolver, MessageFieldsResolver
+from th2_data_services.interfaces.utils.resolver import EventFieldResolver, MessageFieldResolver
 
 
 class TH2Config:
     def __init__(self) -> None:
+        """Global configuration for the DS library."""
         self.INTERACTIVE_MODE = False
-        self.EVENT_FIELDS_RESOLVER: EventFieldsResolver = None
-        self.MESSAGE_FIELDS_RESOLVER: MessageFieldsResolver = None
+        self.EVENT_FIELDS_RESOLVER: EventFieldResolver = None
+        self.MESSAGE_FIELDS_RESOLVER: MessageFieldResolver = None
 
     def __str__(self):
         s = (
             f"INTERACTIVE_MODE={self.INTERACTIVE_MODE}\n"
             f"EVENT_FIELDS_RESOLVER={self.EVENT_FIELDS_RESOLVER}\n"
             f"MESSAGE_FIELDS_RESOLVER={self.MESSAGE_FIELDS_RESOLVER}"
         )
```

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/struct.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 #  limitations under the License.
 from abc import ABC
 
 
 class IEventStruct(ABC):
     """Just to mark Event Struct class.
 
+    Actually, this class doesn't describe the structure, it describes filed names.
+
     It should look like a class with constants.
     """
 
 
 class IMessageStruct(ABC):
     """Just to mark Message Struct class.
 
+    Actually, this class doesn't describe the structure, it describes filed names.
+
     It should look like a class with constants.
     """
```

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/interfaces/utils/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     DIRECT LwdpEventFieldsResolver get_and_return_10_fields_by_direct_resolvers
     Total time taken in :  test_iterate 16.423101902008057  ~ 1546912
     Via http_event_struct get_and_return_10_fields_via_http_event_struct
     Total time taken in :  test_iterate 14.83995270729065   ~ 1700247
 """
 
 
-class EventFieldsResolver(ABC):
+class EventFieldResolver(ABC):
     @staticmethod
     @abstractmethod
     def get_id(event):
         pass
 
     @staticmethod
     @abstractmethod
@@ -103,15 +103,19 @@
 
     @staticmethod
     @abstractmethod
     def get_body(event):
         pass
 
 
-class MessageFieldsResolver(ABC):
+# TODO - should be remove during release.
+EventFieldsResolver = EventFieldResolver  # For backward compatibility.
+
+
+class MessageFieldResolver(ABC):
     @staticmethod
     @abstractmethod
     def get_direction(message):
         pass
 
     @staticmethod
     @abstractmethod
@@ -121,54 +125,65 @@
     @staticmethod
     @abstractmethod
     def get_type(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_connection_id(message):
+    def get_sequence(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_session_alias(message):
+    def get_timestamp(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_subsequence(message):
+    def get_body(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_sequence(message):
+    def get_body_base64(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_timestamp(message):
+    def get_id(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_body(message):
+    def get_attached_event_ids(message):
+        pass
+
+
+# TODO - should be remove during release.
+MessageFieldsResolver = MessageFieldResolver  # For backward compatibility.
+
+
+class SubMessageFieldResolver(ABC):
+    @staticmethod
+    @abstractmethod
+    def get_subsequence(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_body_base64(message):
+    def get_type(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_id(message):
+    def get_fields(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_attached_event_ids(message):
+    def get_metadata(message):
         pass
 
     @staticmethod
     @abstractmethod
-    def get_fields(message):
+    def get_protocol(message):
         pass
```

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/message_utils/message_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 
 # # NOT STREAMABLE
 # Extract compounded message into list of individual messages
 # m: compounded message (retrieved from Data object)
 # result: list of individual message objects
 def expand_message(message: Th2Message) -> Iterable[Th2Message]:
+    # TODO - should be updated for version with Th2Transport
     """Extract compounded message into list of individual messages.
 
     Args:
         message: TH2-Message
 
     Returns:
         Iterable[Th2Message]
@@ -49,35 +50,43 @@
             # m_index = int(k[k.index("-") + 1:])
 
         new_msg = {}
         new_msg.update(message)
         new_msg["messageType"] = msg_type
         new_msg["body"] = {}
         new_msg["body"]["metadata"] = {}
-        new_msg["body"]["metadata"].update(options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"])
+        new_msg["body"]["metadata"].update(
+            options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"]
+        )
         new_msg["body"]["metadata"]["id"] = {}
-        new_msg["body"]["metadata"]["id"].update(options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"]["id"])
+        new_msg["body"]["metadata"]["id"].update(
+            options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"]["id"]
+        )
         new_msg["body"]["metadata"]["messageType"] = msg_type
         new_msg["body"]["metadata"]["id"]["subsequence"] = [
-            options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"]["id"]["subsequence"][msg_index]
+            options.MESSAGE_FIELDS_RESOLVER.get_body(message)["metadata"]["id"]["subsequence"][
+                msg_index
+            ]
         ]
         new_msg["body"]["fields"] = fields[k]["messageValue"]["fields"]
         result.append(new_msg)
 
     return result
 
 
 # # STREAMABLE
 # Gets Dictionary quantities of events for different message categories
 # parameters are: iterable messages object
 # category_list: list categorizer functions
 # result contains calculation for keys: "category1 category2 ... categoryN"
 # result: dictionary {string: int}
 def get_totals(
-    messages: Iterable[Th2Message], categorizers: List[Callable[[Dict], str]], filter_: Callable = None
+    messages: Iterable[Th2Message],
+    categorizers: List[Callable[[Dict], str]],
+    filter_: Callable = None,
 ) -> Dict[str, int]:
     """Returns dictionary quantities of events for different message categories.
 
     Args:
         messages: TH2-Messages
         categorizers: List of categorizer functions
         filter_: Filter functon, defaults to None
@@ -102,15 +111,17 @@
 
 # STREAMABLE
 # Prints Dictionary quantities of events for different message categories
 # parameters are: iterable messages object
 # category_list: list categorizer functions
 # result contains calculation for keys: "category1 category2 ... categoryN"
 # result: table -> stdout
-def print_totals(messages: Iterable[Th2Message], categorizers: List[Callable], filter_: Callable = None) -> None:
+def print_totals(
+    messages: Iterable[Th2Message], categorizers: List[Callable], filter_: Callable = None
+) -> None:
     """Prints dictionary quantities of events for different message categories.
 
     Args:
         messages: TH2-Messages
         categorizers: List of categorizer functions
         filter_: Filter functon, defaults to None
 
@@ -159,15 +170,17 @@
 # NOT STREAMABLE
 # Prints limited list of messages from the stream in dictionary format
 # parameters are: iterable messages object
 # max: maximum messages to retrieve
 # start(optional): extract events starting form this number (to investigate middle of the stream)
 # maxPrint(optional): maximum messages to print
 # result: List of message objects in dictionary format -> stdout
-def print_some_raw(messages: Iterable[Th2Message], max_count: int, start: int = 0, filter_: Callable = None) -> None:
+def print_some_raw(
+    messages: Iterable[Th2Message], max_count: int, start: int = 0, filter_: Callable = None
+) -> None:
     """Prints limited list of messages from the stream in dictionary format.
 
     Args:
         messages: TH2-Messages
         max_count: Maximum messages to retrieve
         start: Extract events starting form this number, defaults to 0
         filter_: Filter function, defaults to None
@@ -207,15 +220,17 @@
 # NOT STREAMABLE
 # Prints limited list of messages from the stream in dictionary format
 # parameters are: iterable messages object
 # max: maximum messages to retrieve
 # start(optional): extract events starting form this number (to investigate middle of the stream)
 # maxPrint(optional): maximum messages to print
 # result: List of message objects in dictionary format -> stdout
-def print_some(messages: Iterable[Th2Message], max_count: int, start: int = 0, filter_: Callable = None) -> None:
+def print_some(
+    messages: Iterable[Th2Message], max_count: int, start: int = 0, filter_: Callable = None
+) -> None:
     """Prints limited list of messages from the stream in dictionary format.
 
     Args:
         messages: TH2-Messages
         max_count: Maximum messages to retrieve
         start: Extract events starting form this number, defaults to 0
         filter_: Filter function, defaults to None
@@ -240,15 +255,17 @@
             new_prefix = f"{prefix}{field}."
             message_fields_to_flat_dict(content["messageValue"], result, new_prefix)
 
         if "listValue" in content:
             list_values = content["listValue"]["values"]
             for i in range(len(list_values)):
                 new_prefix = f"{prefix}{field}."
-                message_fields_to_flat_dict({"fields": {str(i): list_values[i]}}, result, new_prefix)
+                message_fields_to_flat_dict(
+                    {"fields": {str(i): list_values[i]}}, result, new_prefix
+                )
 
 
 # STREAMABLE
 # Converts message body tree structure
 # parameters are: message object
 # max: maximum messages to retrieve # TODO: Add Argument?
 # result: dictionary representing body in flat format
@@ -276,15 +293,17 @@
 
     Args:
         message: TH2-Message
 
     Returns:
         str
     """
-    return th2_data_services.utils.time.extract_timestamp(options.MESSAGE_FIELDS_RESOLVER.get_timestamp(message))
+    return th2_data_services.utils.time.extract_timestamp(
+        options.MESSAGE_FIELDS_RESOLVER.get_timestamp(message)
+    )
 
 
 # STREAMABLE
 def print_message(message: Th2Message) -> None:
     """Print message (verbose).
 
     Args:
@@ -298,15 +317,17 @@
         f"{message_to_dict(message)}"
     )
 
 
 # STREAMABLE
 # Todo: Is This Useful
 def get_raw_body_str(message: Dict):  # noqa
-    my_bytes = base64.b64decode(options.MESSAGE_FIELDS_RESOLVER.get_body_base64(message).encode("ascii"))
+    my_bytes = base64.b64decode(
+        options.MESSAGE_FIELDS_RESOLVER.get_body_base64(message).encode("ascii")
+    )
     my_bytes = my_bytes.replace(b"\x01", b".")
     raw_body = my_bytes.decode("ascii")
     return raw_body
 
 
 # STREAMABLE
 # TODO: Is This Useful?
@@ -386,15 +407,18 @@
 #         print(tabulate(result, headers="firstrow", tablefmt="grid"))
 #         return None
 
 
 # NOT STREAMABLE
 # TODO: Is This Useful?
 def get_messages_examples(
-    messages: Iterable[Th2Message], categories: List[str], categorizer: Callable, filter_: Callable = None
+    messages: Iterable[Th2Message],
+    categories: List[str],
+    categorizer: Callable,
+    filter_: Callable = None,
 ) -> Dict:  # noqa
     # TODO: Add Docstrings
     # It returns {category_name: message}
     result = {}
     categories = set(categories)
     for message in messages:
         expanded_messages = expand_message(message)
```

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5410321437/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/PKG-INFO` & `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7468 322d  : 2.1.Name: th2-
 00000020: 6461 7461 2d73 6572 7669 6365 730a 5665  data-services.Ve
 00000030: 7273 696f 6e3a 2032 2e30 2e30 2e64 6576  rsion: 2.0.0.dev
-00000040: 3534 3038 3837 3033 3739 0a53 756d 6d61  5408870379.Summa
+00000040: 3534 3130 3332 3134 3337 0a53 756d 6d61  5410321437.Summa
 00000050: 7279 3a20 7468 325f 6461 7461 5f73 6572  ry: th2_data_ser
 00000060: 7669 6365 730a 486f 6d65 2d70 6167 653a  vices.Home-page:
 00000070: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 00000080: 636f 6d2f 7468 322d 6e65 742f 7468 322d  com/th2-net/th2-
 00000090: 6461 7461 2d73 6572 7669 6365 730a 4175  data-services.Au
 000000a0: 7468 6f72 3a20 5448 322d 6465 7673 0a41  thor: TH2-devs.A
 000000b0: 7574 686f 722d 656d 6169 6c3a 2074 6832  uthor-email: th2
```

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5408870379/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5410321437/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

