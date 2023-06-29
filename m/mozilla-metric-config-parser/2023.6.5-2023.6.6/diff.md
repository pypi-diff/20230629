# Comparing `tmp/mozilla-metric-config-parser-2023.6.5.tar.gz` & `tmp/mozilla-metric-config-parser-2023.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2023.6.5.tar", last modified: Fri Jun 23 21:21:06 2023, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2023.6.6.tar", last modified: Thu Jun 29 15:10:11 2023, max compression
```

## Comparing `mozilla-metric-config-parser-2023.6.5.tar` & `mozilla-metric-config-parser-2023.6.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.509301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    27669 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9608 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    14411 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.509301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     4708 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    25190 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    14533 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-23 21:21:06.000000 mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-23 21:21:06.513301 mozilla-metric-config-parser-2023.6.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-23 21:20:57.000000 mozilla-metric-config-parser-2023.6.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.220658 mozilla-metric-config-parser-2023.6.6/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    27669 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    14299 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.220658 mozilla-metric-config-parser-2023.6.6/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    25217 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    14533 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 15:10:11.000000 mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-29 15:10:11.224658 mozilla-metric-config-parser-2023.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-29 15:10:03.000000 mozilla-metric-config-parser-2023.6.6/setup.py
```

### Comparing `mozilla-metric-config-parser-2023.6.5/LICENSE` & `mozilla-metric-config-parser-2023.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/PKG-INFO` & `mozilla-metric-config-parser-2023.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.5
+Version: 2023.6.6
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/config.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/function.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import defaultdict
 from enum import Enum
 from textwrap import dedent
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import attr
 import jinja2
+from mozilla_nimbus_schemas.jetstream import AnalysisBasis
 
 from metric_config_parser.errors import DefinitionNotFound
 
 if TYPE_CHECKING:
     from .analysis import AnalysisSpec
     from .config import ConfigCollection
     from .experiment import ExperimentConfiguration
@@ -19,21 +20,14 @@
 from .data_source import DataSource, DataSourceReference
 from .parameter import ParameterDefinition
 from .pre_treatment import PreTreatmentReference
 from .statistic import Statistic
 from .util import converter
 
 
-class AnalysisBasis(Enum):
-    """Determines what the population used for the analysis will be based on."""
-
-    ENROLLMENTS = "enrollments"
-    EXPOSURES = "exposures"
-
-
 class AnalysisPeriod(Enum):
     DAY = "day"
     WEEK = "week"
     DAYS_28 = "days28"
     OVERALL = "overall"
 
     @property
```

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/population.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/project.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 import toml
 from cattrs.errors import ClassValidationError
+from mozilla_nimbus_schemas.jetstream import AnalysisBasis
 
 from metric_config_parser.analysis import AnalysisConfiguration, AnalysisSpec
 from metric_config_parser.data_source import DataSource
 from metric_config_parser.errors import InvalidConfigurationException
 from metric_config_parser.exposure_signal import AnalysisWindow, ExposureSignal
-from metric_config_parser.metric import (
-    AnalysisBasis,
-    AnalysisPeriod,
-    DefinitionNotFound,
-)
+from metric_config_parser.metric import AnalysisPeriod, DefinitionNotFound
 from metric_config_parser.parameter import ParameterDefinition, ParameterSpec
 
 TEST_DIR = Path(__file__).parent
 DEFAULT_METRICS_CONFIG = TEST_DIR / "data" / "jetstream" / "defaults" / "firefox_desktop.toml"
 
 
 class TestAnalysisSpec:
```

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/metric_config_parser/util.py` & `mozilla-metric-config-parser-2023.6.6/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.5
+Version: 2023.6.6
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.5/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2023.6.6/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.5/setup.py` & `mozilla-metric-config-parser-2023.6.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2023.6.5",
+    version="2023.6.6",
 )
```

