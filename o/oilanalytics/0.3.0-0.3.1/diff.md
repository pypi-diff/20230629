# Comparing `tmp/oilanalytics-0.3.0.tar.gz` & `tmp/oilanalytics-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oilanalytics-0.3.0.tar", last modified: Tue Jun 27 15:44:55 2023, max compression
+gzip compressed data, was "oilanalytics-0.3.1.tar", last modified: Thu Jun 29 12:53:09 2023, max compression
```

## Comparing `oilanalytics-0.3.0.tar` & `oilanalytics-0.3.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/notebooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/balances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/balance_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/balance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/global_oil_balances.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/balances/key_agency_comparisons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics/eia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/eia.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/monthly_drilling_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/steo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/eia/weeklypetreport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/energyaspects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/china_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/europe_diesel_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/fsu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/energyaspects/tars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/euroilstock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/euroilstock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/euroilstock/euroilstock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/geo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/geo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/highfreq/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/ara.py
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/highfreq/singapore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/iea/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/iea/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/iea/omr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/jodi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/jodi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/jodi/jodiapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/opec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/opec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/opec/momr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/prices/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/prices/futures_prices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/oilanalytics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/chartutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/eikonutils.py
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/oilanalytics/utils/fileutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.833706 oilanalytics-0.3.0/oilanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-27 15:44:55.000000 oilanalytics-0.3.0/oilanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:55.837706 oilanalytics-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_ea_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_eia.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_eia_weekly_rep.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_futures_prices.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_highfreq.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_iea.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_key_agency_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-27 15:44:45.000000 oilanalytics-0.3.0/test/test_opec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.732569 oilanalytics-0.3.1/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/notebooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.732569 oilanalytics-0.3.1/oilanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.732569 oilanalytics-0.3.1/oilanalytics/balances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/balances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/balances/balance_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/balances/balance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7601 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/balances/global_oil_balances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/balances/key_agency_comparisons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.732569 oilanalytics-0.3.1/oilanalytics/eia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/eia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/eia/eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/eia/monthly_drilling_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/eia/steo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/eia/weeklypetreport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/energyaspects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/energyaspects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/energyaspects/china_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/energyaspects/europe_diesel_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/energyaspects/fsu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/energyaspects/tars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/euroilstock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/euroilstock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/euroilstock/euroilstock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/geo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/highfreq/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/highfreq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/highfreq/ara.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/highfreq/singapore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/iea/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/iea/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/iea/omr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/jodi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/jodi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/jodi/jodiapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/opec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/opec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/opec/momr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/prices/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/prices/futures_prices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/oilanalytics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/utils/chartutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/utils/eikonutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/oilanalytics/utils/fileutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.732569 oilanalytics-0.3.1/oilanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 12:53:09.000000 oilanalytics-0.3.1/oilanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-29 12:53:09.000000 oilanalytics-0.3.1/oilanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 12:53:09.000000 oilanalytics-0.3.1/oilanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 12:53:09.000000 oilanalytics-0.3.1/oilanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 12:53:09.000000 oilanalytics-0.3.1/oilanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 12:53:09.736569 oilanalytics-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_ea_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_eia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_eia_weekly_rep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_futures_prices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_highfreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_iea.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_key_agency_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-29 12:52:55.000000 oilanalytics-0.3.1/test/test_opec.py
```

### Comparing `oilanalytics-0.3.0/oilanalytics/balances/balance_utils.py` & `oilanalytics-0.3.1/oilanalytics/balances/balance_utils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/balances/global_oil_balances.py` & `oilanalytics-0.3.1/oilanalytics/balances/global_oil_balances.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/balances/key_agency_comparisons.py` & `oilanalytics-0.3.1/oilanalytics/balances/key_agency_comparisons.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/eia/eia.py` & `oilanalytics-0.3.1/oilanalytics/eia/eia.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/eia/monthly_drilling_report.py` & `oilanalytics-0.3.1/oilanalytics/eia/monthly_drilling_report.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/eia/steo.py` & `oilanalytics-0.3.1/oilanalytics/eia/steo.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/eia/weeklypetreport.py` & `oilanalytics-0.3.1/oilanalytics/eia/weeklypetreport.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/energyaspects/china_stats.py` & `oilanalytics-0.3.1/oilanalytics/energyaspects/china_stats.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/energyaspects/europe_diesel_balance.py` & `oilanalytics-0.3.1/oilanalytics/energyaspects/europe_diesel_balance.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/energyaspects/fsu_stats.py` & `oilanalytics-0.3.1/oilanalytics/energyaspects/fsu_stats.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/energyaspects/tars.py` & `oilanalytics-0.3.1/oilanalytics/energyaspects/tars.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/euroilstock/euroilstock.py` & `oilanalytics-0.3.1/oilanalytics/euroilstock/euroilstock.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/highfreq/ara.py` & `oilanalytics-0.3.1/oilanalytics/highfreq/ara.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/highfreq/singapore.py` & `oilanalytics-0.3.1/oilanalytics/highfreq/singapore.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/iea/omr.py` & `oilanalytics-0.3.1/oilanalytics/iea/omr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/opec/momr.py` & `oilanalytics-0.3.1/oilanalytics/opec/momr.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/prices/futures_prices.py` & `oilanalytics-0.3.1/oilanalytics/prices/futures_prices.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics/utils/chartutils.py` & `oilanalytics-0.3.1/oilanalytics/utils/chartutils.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/oilanalytics.egg-info/SOURCES.txt` & `oilanalytics-0.3.1/oilanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/setup.py` & `oilanalytics-0.3.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="oilanalytics",
-    version="0.3.0",
+    version="0.3.1",
     author="aeorxc",
     description="Utilities for oil analytics",
     url="https://github.com/aeorxc/oilanalytics",
     project_urls={
         "Source": "https://github.com/aeorxc/oilanalytics",
     },
     packages=setuptools.find_packages(),
```

### Comparing `oilanalytics-0.3.0/test/test_eia.py` & `oilanalytics-0.3.1/test/test_eia.py`

 * *Files identical despite different names*

### Comparing `oilanalytics-0.3.0/test/test_highfreq.py` & `oilanalytics-0.3.1/test/test_highfreq.py`

 * *Files identical despite different names*

