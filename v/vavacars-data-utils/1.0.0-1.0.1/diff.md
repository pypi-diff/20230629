# Comparing `tmp/vavacars_data_utils-1.0.0.tar.gz` & `tmp/vavacars_data_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vavacars_data_utils-1.0.0.tar", last modified: Thu Jun 29 09:18:45 2023, max compression
+gzip compressed data, was "vavacars_data_utils-1.0.1.tar", last modified: Thu Jun 29 09:22:54 2023, max compression
```

## Comparing `vavacars_data_utils-1.0.0.tar` & `vavacars_data_utils-1.0.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.922788 vavacars_data_utils-1.0.0/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:18:45.922788 vavacars_data_utils-1.0.0/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/README.md
--rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/pyproject.toml
--rwxrwxrwx   0 pga       (1000) pga       (1000)      799 2023-06-29 09:18:45.941556 vavacars_data_utils-1.0.0/setup.cfg
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.434080 vavacars_data_utils-1.0.0/test/
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.639239 vavacars_data_utils-1.0.0/test/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/test/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/test/utils/test_strings.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.670570 vavacars_data_utils-1.0.0/vava_utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/__init__.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.733876 vavacars_data_utils-1.0.0/vava_utils/azure/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.0.0/vava_utils/azure/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    10180 2023-03-06 06:57:28.000000 vavacars_data_utils-1.0.0/vava_utils/azure/az_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.814763 vavacars_data_utils-1.0.0/vava_utils/bigquery/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/bigquery/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/bigquery/bigquery_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.891846 vavacars_data_utils-1.0.0/vava_utils/camunda/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/camunda/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.0.0/vava_utils/camunda/camunda_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:44.972228 vavacars_data_utils-1.0.0/vava_utils/email/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.0.0/vava_utils/email/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.0.0/vava_utils/email/email_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.052187 vavacars_data_utils-1.0.0/vava_utils/salesforce/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.0.0/vava_utils/salesforce/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2136 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/salesforce/salesforce_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.193542 vavacars_data_utils-1.0.0/vava_utils/smartiq/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper_v2.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.286701 vavacars_data_utils-1.0.0/vava_utils/sql/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.0.0/vava_utils/sql/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)    12971 2023-06-19 15:21:04.000000 vavacars_data_utils-1.0.0/vava_utils/sql/sql_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.381572 vavacars_data_utils-1.0.0/vava_utils/turkey/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/turkey/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/turkey/dates.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.635387 vavacars_data_utils-1.0.0/vava_utils/utils/
--rwxrwxrwx   0 pga       (1000) pga       (1000)      288 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/utils/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/utils/callables.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.0.0/vava_utils/utils/comparisons.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.0/vava_utils/utils/naming.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.0/vava_utils/utils/singleton.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.0/vava_utils/utils/strings.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.730404 vavacars_data_utils-1.0.0/vava_utils/vavaprice/
--rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.0.0/vava_utils/vavaprice/__init__.py
--rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.0.0/vava_utils/vavaprice/vavaprice_helper.py
-drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:18:45.891842 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/
--rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/PKG-INFO
--rwxrwxrwx   0 pga       (1000) pga       (1000)     1185 2023-06-29 09:18:44.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/SOURCES.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/dependency_links.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)       97 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/requires.txt
--rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2023-06-29 09:18:43.000000 vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/top_level.txt
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:54.110368 vavacars_data_utils-1.0.1/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:22:54.110368 vavacars_data_utils-1.0.1/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2321 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/README.md
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      124 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/pyproject.toml
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      799 2023-06-29 09:22:54.121782 vavacars_data_utils-1.0.1/setup.cfg
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:52.583089 vavacars_data_utils-1.0.1/test/
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:52.805148 vavacars_data_utils-1.0.1/test/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/test/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1159 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/test/utils/test_strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:52.834080 vavacars_data_utils-1.0.1/vava_utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        0 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/__init__.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:52.915411 vavacars_data_utils-1.0.1/vava_utils/azure/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       70 2022-05-04 13:49:57.000000 vavacars_data_utils-1.0.1/vava_utils/azure/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    10180 2023-03-06 06:57:28.000000 vavacars_data_utils-1.0.1/vava_utils/azure/az_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.001450 vavacars_data_utils-1.0.1/vava_utils/bigquery/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       43 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/vava_utils/bigquery/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1187 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/vava_utils/bigquery/bigquery_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.090654 vavacars_data_utils-1.0.1/vava_utils/camunda/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       85 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/camunda/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     4008 2023-05-16 14:47:25.000000 vavacars_data_utils-1.0.1/vava_utils/camunda/camunda_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.175598 vavacars_data_utils-1.0.1/vava_utils/email/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       37 2023-06-15 13:04:41.000000 vavacars_data_utils-1.0.1/vava_utils/email/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3862 2023-06-29 09:16:49.000000 vavacars_data_utils-1.0.1/vava_utils/email/email_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.254507 vavacars_data_utils-1.0.1/vava_utils/salesforce/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       47 2023-06-09 14:13:08.000000 vavacars_data_utils-1.0.1/vava_utils/salesforce/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2136 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/vava_utils/salesforce/salesforce_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.379317 vavacars_data_utils-1.0.1/vava_utils/smartiq/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      205 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.1/vava_utils/smartiq/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     7909 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.1/vava_utils/smartiq/smartiq_helper.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     9856 2022-06-16 14:27:47.000000 vavacars_data_utils-1.0.1/vava_utils/smartiq/smartiq_helper_v2.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.482159 vavacars_data_utils-1.0.1/vava_utils/sql/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      160 2022-06-21 13:02:18.000000 vavacars_data_utils-1.0.1/vava_utils/sql/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)    12976 2023-06-29 09:21:57.000000 vavacars_data_utils-1.0.1/vava_utils/sql/sql_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.568466 vavacars_data_utils-1.0.1/vava_utils/turkey/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      148 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/turkey/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      889 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/turkey/dates.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.820912 vavacars_data_utils-1.0.1/vava_utils/utils/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      288 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/vava_utils/utils/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      369 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/utils/callables.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1950 2022-07-04 11:26:35.000000 vavacars_data_utils-1.0.1/vava_utils/utils/comparisons.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1168 2023-06-15 14:28:48.000000 vavacars_data_utils-1.0.1/vava_utils/utils/naming.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      273 2022-04-25 14:18:59.000000 vavacars_data_utils-1.0.1/vava_utils/utils/singleton.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)      734 2022-03-09 12:03:29.000000 vavacars_data_utils-1.0.1/vava_utils/utils/strings.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:53.912568 vavacars_data_utils-1.0.1/vava_utils/vavaprice/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       91 2022-03-11 15:04:33.000000 vavacars_data_utils-1.0.1/vava_utils/vavaprice/__init__.py
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     3225 2022-10-18 14:03:18.000000 vavacars_data_utils-1.0.1/vava_utils/vavaprice/vavaprice_helper.py
+drwxrwxrwx   0 pga       (1000) pga       (1000)        0 2023-06-29 09:22:54.075728 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     2801 2023-06-29 09:22:52.000000 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/PKG-INFO
+-rwxrwxrwx   0 pga       (1000) pga       (1000)     1185 2023-06-29 09:22:52.000000 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)        1 2023-06-29 09:22:52.000000 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       97 2023-06-29 09:22:52.000000 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/requires.txt
+-rwxrwxrwx   0 pga       (1000) pga       (1000)       16 2023-06-29 09:22:52.000000 vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/top_level.txt
```

### Comparing `vavacars_data_utils-1.0.0/PKG-INFO` & `vavacars_data_utils-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vavacars_data_utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `vavacars_data_utils-1.0.0/README.md` & `vavacars_data_utils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/setup.cfg` & `vavacars_data_utils-1.0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vavacars_data_utils
-version = 1.0.0
+version = 1.0.1
 author = Vavacars Data Science Team
 author_email = acg@vava.cars
 description = Package with utils
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 project_urls =
```

### Comparing `vavacars_data_utils-1.0.0/test/utils/test_strings.py` & `vavacars_data_utils-1.0.1/test/utils/test_strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/azure/az_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/azure/az_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/bigquery/bigquery_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/bigquery/bigquery_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/camunda/camunda_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/camunda/camunda_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/email/email_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/email/email_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/salesforce/salesforce_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/salesforce/salesforce_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/smartiq/smartiq_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/smartiq/smartiq_helper_v2.py` & `vavacars_data_utils-1.0.1/vava_utils/smartiq/smartiq_helper_v2.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/sql/sql_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/sql/sql_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from typing import List
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-def get_mysql_helper(host, user, port, database, password=None, **kwargs):
+def get_mysql_helper(host, user, port, database=None, password=None, **kwargs):
     engine_url = URL.create(
         drivername="mysql+pymysql", host=host, username=user, database=database, password=password, port=port
     )
     engine = create_engine(
         engine_url, connect_args={"ssl": {"ssl_check_hostname": False}}, pool_pre_ping=True, **kwargs
     )
     if not password:
```

### Comparing `vavacars_data_utils-1.0.0/vava_utils/turkey/dates.py` & `vavacars_data_utils-1.0.1/vava_utils/turkey/dates.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/utils/comparisons.py` & `vavacars_data_utils-1.0.1/vava_utils/utils/comparisons.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/utils/naming.py` & `vavacars_data_utils-1.0.1/vava_utils/utils/naming.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/utils/strings.py` & `vavacars_data_utils-1.0.1/vava_utils/utils/strings.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vava_utils/vavaprice/vavaprice_helper.py` & `vavacars_data_utils-1.0.1/vava_utils/vavaprice/vavaprice_helper.py`

 * *Files identical despite different names*

### Comparing `vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/PKG-INFO` & `vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vavacars-data-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package with utils
 Home-page: https://dev.azure.com/vavacars/DataScience/_git/Data.Utils
 Author: Vavacars Data Science Team
 Author-email: acg@vava.cars
 Project-URL: Bug Tracker, https://dev.azure.com/vavacars/DataScience/_workitems/recentlyupdated/
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `vavacars_data_utils-1.0.0/vavacars_data_utils.egg-info/SOURCES.txt` & `vavacars_data_utils-1.0.1/vavacars_data_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

