# Comparing `tmp/timely-beliefs-1.9.1.tar.gz` & `tmp/timely-beliefs-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timely-beliefs-1.9.1.tar", last modified: Thu Jan  6 15:38:26 2022, max compression
+gzip compressed data, was "timely-beliefs-1.9.2.tar", last modified: Thu Jan  6 16:00:08 2022, max compression
```

## Comparing `timely-beliefs-1.9.1.tar` & `timely-beliefs-1.9.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.655538 timely-beliefs-1.9.1/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.631538 timely-beliefs-1.9.1/.github/
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.635538 timely-beliefs-1.9.1/.github/workflows/
--rw-r--r--   0 felix     (1000) felix     (1000)     1229 2021-12-01 09:30:30.000000 timely-beliefs-1.9.1/.github/workflows/lint-and-test.yml
--rw-r--r--   0 felix     (1000) felix     (1000)     1203 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/.gitignore
--rw-r--r--   0 felix     (1000) felix     (1000)      595 2021-12-03 21:43:36.000000 timely-beliefs-1.9.1/.pre-commit-config.yaml
--rw-r--r--   0 felix     (1000) felix     (1000)     1065 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/LICENSE
--rw-r--r--   0 felix     (1000) felix     (1000)       38 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/MANIFEST.in
--rw-r--r--   0 felix     (1000) felix     (1000)      533 2021-12-03 21:43:36.000000 timely-beliefs-1.9.1/Makefile
--rw-r--r--   0 felix     (1000) felix     (1000)     1114 2022-01-06 15:38:26.655538 timely-beliefs-1.9.1/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     9404 2021-12-26 15:01:41.000000 timely-beliefs-1.9.1/README.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.639538 timely-beliefs-1.9.1/dev/
--rw-r--r--   0 felix     (1000) felix     (1000)      670 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/dev/dev.md
--rw-r--r--   0 felix     (1000) felix     (1000)     1333 2021-09-30 07:23:14.000000 timely-beliefs-1.9.1/dev/requirements.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      347 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/pyproject.toml
--rw-r--r--   0 felix     (1000) felix     (1000)      207 2022-01-06 15:38:26.655538 timely-beliefs-1.9.1/setup.cfg
--rw-r--r--   0 felix     (1000) felix     (1000)     2563 2021-12-26 15:01:41.000000 timely-beliefs-1.9.1/setup.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.639538 timely-beliefs-1.9.1/timely_beliefs/
--rw-r--r--   0 felix     (1000) felix     (1000)     1232 2021-12-03 21:43:36.000000 timely-beliefs-1.9.1/timely_beliefs/__init__.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.639538 timely-beliefs-1.9.1/timely_beliefs/beliefs/
--rw-r--r--   0 felix     (1000) felix     (1000)     6287 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/beliefs/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    84487 2022-01-06 15:35:51.000000 timely-beliefs-1.9.1/timely_beliefs/beliefs/classes.py
--rw-r--r--   0 felix     (1000) felix     (1000)    24624 2021-12-27 13:01:28.000000 timely-beliefs-1.9.1/timely_beliefs/beliefs/probabilistic_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)    22280 2021-12-27 13:01:28.000000 timely-beliefs-1.9.1/timely_beliefs/beliefs/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)       83 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/db_base.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.643539 timely-beliefs-1.9.1/timely_beliefs/docs/
--rw-r--r--   0 felix     (1000) felix     (1000)     2646 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/accuracy.md
--rw-r--r--   0 felix     (1000) felix     (1000)   189137 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/belief_history_ridgeline.png
--rw-r--r--   0 felix     (1000) felix     (1000)   172491 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png
--rw-r--r--   0 felix     (1000) felix     (1000)     1948 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/confidence.md
--rw-r--r--   0 felix     (1000) felix     (1000)     6880 2021-12-26 15:01:41.000000 timely-beliefs-1.9.1/timely_beliefs/docs/db.md
--rw-r--r--   0 felix     (1000) felix     (1000)   187292 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/fixed_viewpoint_ridgeline.png
--rw-r--r--   0 felix     (1000) felix     (1000)     5382 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/init.md
--rw-r--r--   0 felix     (1000) felix     (1000)      287 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/lineage.md
--rw-r--r--   0 felix     (1000) felix     (1000)     4668 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/docs/resampling.md
--rw-r--r--   0 felix     (1000) felix     (1000)     4456 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/docs/slicing.md
--rw-r--r--   0 felix     (1000) felix     (1000)     5004 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/docs/timing.md
--rw-r--r--   0 felix     (1000) felix     (1000)     3575 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/docs/viz.md
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.647539 timely-beliefs-1.9.1/timely_beliefs/examples/
--rw-r--r--   0 felix     (1000) felix     (1000)      512 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/examples/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1904 2021-12-21 09:13:09.000000 timely-beliefs-1.9.1/timely_beliefs/examples/beliefs_data_frames.py
--rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/examples/chart.html
--rw-r--r--   0 felix     (1000) felix     (1000)  1362729 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/examples/temperature.csv
--rw-r--r--   0 felix     (1000) felix     (1000)      451 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/examples/visualize_example.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.647539 timely-beliefs-1.9.1/timely_beliefs/sensors/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5300 2021-12-21 09:13:09.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/classes.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.647539 timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)      433 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/event_values.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5704 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/knowledge_horizons.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4049 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/test_knowledge_horizons.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4177 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sensors/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.651538 timely-beliefs-1.9.1/timely_beliefs/sources/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sources/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1593 2021-10-28 18:09:21.000000 timely-beliefs-1.9.1/timely_beliefs/sources/classes.py
--rw-r--r--   0 felix     (1000) felix     (1000)      648 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/sources/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.655538 timely-beliefs-1.9.1/timely_beliefs/tests/
--rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/README.md
--rw-r--r--   0 felix     (1000) felix     (1000)      204 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4269 2021-10-07 08:28:54.000000 timely-beliefs-1.9.1/timely_beliefs/tests/conftest.py
--rw-r--r--   0 felix     (1000) felix     (1000)     5850 2021-12-27 13:01:28.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_accuracy.py
--rw-r--r--   0 felix     (1000) felix     (1000)     3534 2021-10-26 13:48:17.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_init.py
--rw-r--r--   0 felix     (1000) felix     (1000)    20333 2021-12-21 09:13:09.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_io.py
--rw-r--r--   0 felix     (1000) felix     (1000)     2193 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_persistence.py
--rw-r--r--   0 felix     (1000) felix     (1000)    14325 2021-12-06 11:59:18.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_query.py
--rw-r--r--   0 felix     (1000) felix     (1000)     4400 2021-12-01 09:30:30.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_db_subclassing.py
--rw-r--r--   0 felix     (1000) felix     (1000)    11713 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_df_resampling.py
--rw-r--r--   0 felix     (1000) felix     (1000)      389 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_ignore_36.py
--rw-r--r--   0 felix     (1000) felix     (1000)      606 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_plotting.py
--rw-r--r--   0 felix     (1000) felix     (1000)     9996 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_probabilistic_downsampling.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1352 2021-09-30 07:22:48.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_ridgeline.py
--rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_sensor_init.py
--rw-r--r--   0 felix     (1000) felix     (1000)      151 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_sensor_query.py
--rw-r--r--   0 felix     (1000) felix     (1000)      323 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/test_utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     1517 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/tests/utils.py
--rw-r--r--   0 felix     (1000) felix     (1000)     7735 2021-09-21 10:34:51.000000 timely-beliefs-1.9.1/timely_beliefs/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.655538 timely-beliefs-1.9.1/timely_beliefs/visualization/
--rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/visualization/__init__.py
--rw-r--r--   0 felix     (1000) felix     (1000)    12546 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/visualization/graphs.py
--rw-r--r--   0 felix     (1000) felix     (1000)     8743 2021-09-09 13:27:19.000000 timely-beliefs-1.9.1/timely_beliefs/visualization/selectors.py
--rw-r--r--   0 felix     (1000) felix     (1000)    17479 2021-12-27 13:01:28.000000 timely-beliefs-1.9.1/timely_beliefs/visualization/utils.py
-drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 15:38:26.639538 timely-beliefs-1.9.1/timely_beliefs.egg-info/
--rw-r--r--   0 felix     (1000) felix     (1000)     1114 2022-01-06 15:38:26.000000 timely-beliefs-1.9.1/timely_beliefs.egg-info/PKG-INFO
--rw-r--r--   0 felix     (1000) felix     (1000)     2525 2022-01-06 15:38:26.000000 timely-beliefs-1.9.1/timely_beliefs.egg-info/SOURCES.txt
--rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-01-06 15:38:26.000000 timely-beliefs-1.9.1/timely_beliefs.egg-info/dependency_links.txt
--rw-r--r--   0 felix     (1000) felix     (1000)      137 2022-01-06 15:38:26.000000 timely-beliefs-1.9.1/timely_beliefs.egg-info/requires.txt
--rw-r--r--   0 felix     (1000) felix     (1000)       15 2022-01-06 15:38:26.000000 timely-beliefs-1.9.1/timely_beliefs.egg-info/top_level.txt
--rwxr-xr-x   0 felix     (1000) felix     (1000)     1352 2021-12-03 21:43:36.000000 timely-beliefs-1.9.1/to_pypi.sh
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.012669 timely-beliefs-1.9.2/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:07.996669 timely-beliefs-1.9.2/.github/
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.000669 timely-beliefs-1.9.2/.github/workflows/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1229 2021-12-01 09:30:30.000000 timely-beliefs-1.9.2/.github/workflows/lint-and-test.yml
+-rw-r--r--   0 felix     (1000) felix     (1000)     1203 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/.gitignore
+-rw-r--r--   0 felix     (1000) felix     (1000)      595 2021-12-03 21:43:36.000000 timely-beliefs-1.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 felix     (1000) felix     (1000)     1065 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/LICENSE
+-rw-r--r--   0 felix     (1000) felix     (1000)       38 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/MANIFEST.in
+-rw-r--r--   0 felix     (1000) felix     (1000)      533 2021-12-03 21:43:36.000000 timely-beliefs-1.9.2/Makefile
+-rw-r--r--   0 felix     (1000) felix     (1000)     1114 2022-01-06 16:00:08.012669 timely-beliefs-1.9.2/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     9404 2021-12-26 15:01:41.000000 timely-beliefs-1.9.2/README.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.000669 timely-beliefs-1.9.2/dev/
+-rw-r--r--   0 felix     (1000) felix     (1000)      670 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/dev/dev.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     1333 2021-09-30 07:23:14.000000 timely-beliefs-1.9.2/dev/requirements.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      347 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/pyproject.toml
+-rw-r--r--   0 felix     (1000) felix     (1000)      207 2022-01-06 16:00:08.016669 timely-beliefs-1.9.2/setup.cfg
+-rw-r--r--   0 felix     (1000) felix     (1000)     2563 2021-12-26 15:01:41.000000 timely-beliefs-1.9.2/setup.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.000669 timely-beliefs-1.9.2/timely_beliefs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1232 2021-12-03 21:43:36.000000 timely-beliefs-1.9.2/timely_beliefs/__init__.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.004669 timely-beliefs-1.9.2/timely_beliefs/beliefs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     6287 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/beliefs/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    83610 2022-01-06 15:55:55.000000 timely-beliefs-1.9.2/timely_beliefs/beliefs/classes.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    24624 2021-12-27 13:01:28.000000 timely-beliefs-1.9.2/timely_beliefs/beliefs/probabilistic_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    22280 2021-12-27 13:01:28.000000 timely-beliefs-1.9.2/timely_beliefs/beliefs/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)       83 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/db_base.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.004669 timely-beliefs-1.9.2/timely_beliefs/docs/
+-rw-r--r--   0 felix     (1000) felix     (1000)     2646 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/accuracy.md
+-rw-r--r--   0 felix     (1000) felix     (1000)   189137 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/belief_history_ridgeline.png
+-rw-r--r--   0 felix     (1000) felix     (1000)   172491 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png
+-rw-r--r--   0 felix     (1000) felix     (1000)     1948 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/confidence.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     6880 2021-12-26 15:01:41.000000 timely-beliefs-1.9.2/timely_beliefs/docs/db.md
+-rw-r--r--   0 felix     (1000) felix     (1000)   187292 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/fixed_viewpoint_ridgeline.png
+-rw-r--r--   0 felix     (1000) felix     (1000)     5382 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/init.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      287 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/lineage.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     4668 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/docs/resampling.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     4456 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/docs/slicing.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     5004 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/docs/timing.md
+-rw-r--r--   0 felix     (1000) felix     (1000)     3575 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/docs/viz.md
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.008669 timely-beliefs-1.9.2/timely_beliefs/examples/
+-rw-r--r--   0 felix     (1000) felix     (1000)      512 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/examples/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1904 2021-12-21 09:13:09.000000 timely-beliefs-1.9.2/timely_beliefs/examples/beliefs_data_frames.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/examples/chart.html
+-rw-r--r--   0 felix     (1000) felix     (1000)  1362729 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/examples/temperature.csv
+-rw-r--r--   0 felix     (1000) felix     (1000)      451 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/examples/visualize_example.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.008669 timely-beliefs-1.9.2/timely_beliefs/sensors/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5300 2021-12-21 09:13:09.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/classes.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.008669 timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      433 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/event_values.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5704 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/knowledge_horizons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4049 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/test_knowledge_horizons.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4177 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sensors/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.008669 timely-beliefs-1.9.2/timely_beliefs/sources/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sources/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1593 2021-10-28 18:09:21.000000 timely-beliefs-1.9.2/timely_beliefs/sources/classes.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      648 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/sources/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.012669 timely-beliefs-1.9.2/timely_beliefs/tests/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1818 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/README.md
+-rw-r--r--   0 felix     (1000) felix     (1000)      204 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4269 2021-10-07 08:28:54.000000 timely-beliefs-1.9.2/timely_beliefs/tests/conftest.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     5850 2021-12-27 13:01:28.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_accuracy.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     3534 2021-10-26 13:48:17.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_init.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    20333 2021-12-21 09:13:09.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_io.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     2193 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_persistence.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    14325 2021-12-06 11:59:18.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_query.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     4400 2021-12-01 09:30:30.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_db_subclassing.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    11713 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_df_resampling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      389 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_ignore_36.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      606 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_plotting.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     9996 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_probabilistic_downsampling.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1352 2021-09-30 07:22:48.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_ridgeline.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      750 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_sensor_init.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      151 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_sensor_query.py
+-rw-r--r--   0 felix     (1000) felix     (1000)      323 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/test_utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     1517 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/tests/utils.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     7735 2021-09-21 10:34:51.000000 timely-beliefs-1.9.2/timely_beliefs/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.012669 timely-beliefs-1.9.2/timely_beliefs/visualization/
+-rw-r--r--   0 felix     (1000) felix     (1000)        0 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/visualization/__init__.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    12546 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/visualization/graphs.py
+-rw-r--r--   0 felix     (1000) felix     (1000)     8743 2021-09-09 13:27:19.000000 timely-beliefs-1.9.2/timely_beliefs/visualization/selectors.py
+-rw-r--r--   0 felix     (1000) felix     (1000)    17479 2021-12-27 13:01:28.000000 timely-beliefs-1.9.2/timely_beliefs/visualization/utils.py
+drwxr-xr-x   0 felix     (1000) felix     (1000)        0 2022-01-06 16:00:08.004669 timely-beliefs-1.9.2/timely_beliefs.egg-info/
+-rw-r--r--   0 felix     (1000) felix     (1000)     1114 2022-01-06 16:00:07.000000 timely-beliefs-1.9.2/timely_beliefs.egg-info/PKG-INFO
+-rw-r--r--   0 felix     (1000) felix     (1000)     2525 2022-01-06 16:00:07.000000 timely-beliefs-1.9.2/timely_beliefs.egg-info/SOURCES.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)        1 2022-01-06 16:00:07.000000 timely-beliefs-1.9.2/timely_beliefs.egg-info/dependency_links.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)      137 2022-01-06 16:00:07.000000 timely-beliefs-1.9.2/timely_beliefs.egg-info/requires.txt
+-rw-r--r--   0 felix     (1000) felix     (1000)       15 2022-01-06 16:00:07.000000 timely-beliefs-1.9.2/timely_beliefs.egg-info/top_level.txt
+-rwxr-xr-x   0 felix     (1000) felix     (1000)     1352 2021-12-03 21:43:36.000000 timely-beliefs-1.9.2/to_pypi.sh
```

### Comparing `timely-beliefs-1.9.1/.github/workflows/lint-and-test.yml` & `timely-beliefs-1.9.2/.github/workflows/lint-and-test.yml`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/.gitignore` & `timely-beliefs-1.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/.pre-commit-config.yaml` & `timely-beliefs-1.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/LICENSE` & `timely-beliefs-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/Makefile` & `timely-beliefs-1.9.2/Makefile`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/PKG-INFO` & `timely-beliefs-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timely-beliefs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Data modelled as beliefs (at a certain time) about events (at a certain time).
 Home-page: https://github.com/seitabv/timely-beliefs
 Author: Seita BV
 Author-email: felix@seita.nl
 License: UNKNOWN
 Keywords: time series,forecasting,analytics,visualization,uncertainty,lineage
 Platform: UNKNOWN
```

### Comparing `timely-beliefs-1.9.1/README.md` & `timely-beliefs-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/dev/dev.md` & `timely-beliefs-1.9.2/dev/dev.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/dev/requirements.txt` & `timely-beliefs-1.9.2/dev/requirements.txt`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/setup.py` & `timely-beliefs-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/__init__.py` & `timely-beliefs-1.9.2/timely_beliefs/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/beliefs/__init__.py` & `timely-beliefs-1.9.2/timely_beliefs/beliefs/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/beliefs/classes.py` & `timely-beliefs-1.9.2/timely_beliefs/beliefs/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             belief_time=belief_time,
         )
 
     @classmethod
     def add_to_session(
         cls,
         session: Session,
-        beliefs_data_frame: "BeliefsDataFrame",  # todo: allow passing List[TimedBelief], too
+        beliefs_data_frame: "BeliefsDataFrame",
         expunge_session: bool = False,
         allow_overwrite: bool = False,
         bulk_save_objects: bool = False,
         commit_transaction: bool = False,
     ):
         """Add a BeliefsDataFrame as timed beliefs to a database session.
 
@@ -288,30 +288,14 @@
         else:
             for belief in beliefs:
                 session.merge(belief)
         if commit_transaction:
             session.commit()
 
     @classmethod
-    def expunge_from_session(
-        cls,
-        session: Session,
-        beliefs_data_frame: "BeliefsDataFrame",  # todo: allow passing List[TimedBelief], too
-    ):
-        # Belief timing is stored as the belief horizon rather than as the belief time
-        belief_records = (
-            beliefs_data_frame.convert_index_from_belief_time_to_horizon()
-                .reset_index()
-                .to_dict("records")
-        )
-        beliefs = [cls(sensor=beliefs_data_frame.sensor, **d) for d in belief_records]
-        for belief in beliefs:
-            session.expunge(belief)
-
-    @classmethod
     @tb_utils.append_doc_of("TimedBeliefDBMixin.search_session")
     def query(cls, *args, **kwargs):
         """Function will be deprecated. Please switch to using search_session."""
         # todo: deprecate this function (announced v1.3.0), which can clash with SQLAlchemy's Model.query()
         import warnings
 
         warnings.warn(
@@ -1342,24 +1326,19 @@
         df = self
 
         belief_timing_col = (
             "belief_time" if "belief_time" in df.index.names else "belief_horizon"
         )
 
         # fast track a common case where each event has only one deterministic belief and only the most recent belief is needed
-        print("bbbbbbbbb")
-        print(df.lineage.number_of_beliefs == df.lineage.number_of_events)
-        print(keep_only_most_recent_belief)
-        print( df.lineage.number_of_sources)
         if (
             df.lineage.number_of_beliefs == df.lineage.number_of_events
             and keep_only_most_recent_belief
             and df.lineage.number_of_sources == 1
         ):
-            print("rrrrrrrrrr")
             if event_resolution > self.event_resolution:
                 # downsample
                 column_functions = {
                     "event_value": "mean",
                     "source": "first",  # keep the only source
                     belief_timing_col: "max"
                     if belief_timing_col == "belief_time"
```

### Comparing `timely-beliefs-1.9.1/timely_beliefs/beliefs/probabilistic_utils.py` & `timely-beliefs-1.9.2/timely_beliefs/beliefs/probabilistic_utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/beliefs/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/beliefs/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/accuracy.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/accuracy.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/belief_history_ridgeline.png` & `timely-beliefs-1.9.2/timely_beliefs/docs/belief_history_ridgeline.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png` & `timely-beliefs-1.9.2/timely_beliefs/docs/comparing_wind_speed_forecasting_models.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/confidence.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/confidence.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/db.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/db.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/fixed_viewpoint_ridgeline.png` & `timely-beliefs-1.9.2/timely_beliefs/docs/fixed_viewpoint_ridgeline.png`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/init.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/init.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/resampling.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/resampling.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/slicing.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/slicing.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/timing.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/timing.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/docs/viz.md` & `timely-beliefs-1.9.2/timely_beliefs/docs/viz.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/examples/__init__.py` & `timely-beliefs-1.9.2/timely_beliefs/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/examples/beliefs_data_frames.py` & `timely-beliefs-1.9.2/timely_beliefs/examples/beliefs_data_frames.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/examples/chart.html` & `timely-beliefs-1.9.2/timely_beliefs/examples/chart.html`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/examples/temperature.csv` & `timely-beliefs-1.9.2/timely_beliefs/examples/temperature.csv`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sensors/classes.py` & `timely-beliefs-1.9.2/timely_beliefs/sensors/classes.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/knowledge_horizons.py` & `timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/knowledge_horizons.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sensors/func_store/test_knowledge_horizons.py` & `timely-beliefs-1.9.2/timely_beliefs/sensors/func_store/test_knowledge_horizons.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sensors/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/sensors/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sources/classes.py` & `timely-beliefs-1.9.2/timely_beliefs/sources/classes.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/sources/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/sources/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/README.md` & `timely-beliefs-1.9.2/timely_beliefs/tests/README.md`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/conftest.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_accuracy.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_init.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_init.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_io.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_io.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_persistence.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_persistence.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_belief_query.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_belief_query.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_db_subclassing.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_db_subclassing.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_df_resampling.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_df_resampling.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_plotting.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_probabilistic_downsampling.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_probabilistic_downsampling.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_ridgeline.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_ridgeline.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/test_sensor_init.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/test_sensor_init.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/tests/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/tests/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/visualization/graphs.py` & `timely-beliefs-1.9.2/timely_beliefs/visualization/graphs.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/visualization/selectors.py` & `timely-beliefs-1.9.2/timely_beliefs/visualization/selectors.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs/visualization/utils.py` & `timely-beliefs-1.9.2/timely_beliefs/visualization/utils.py`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/timely_beliefs.egg-info/PKG-INFO` & `timely-beliefs-1.9.2/timely_beliefs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timely-beliefs
-Version: 1.9.1
+Version: 1.9.2
 Summary: Data modelled as beliefs (at a certain time) about events (at a certain time).
 Home-page: https://github.com/seitabv/timely-beliefs
 Author: Seita BV
 Author-email: felix@seita.nl
 License: UNKNOWN
 Keywords: time series,forecasting,analytics,visualization,uncertainty,lineage
 Platform: UNKNOWN
```

### Comparing `timely-beliefs-1.9.1/timely_beliefs.egg-info/SOURCES.txt` & `timely-beliefs-1.9.2/timely_beliefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timely-beliefs-1.9.1/to_pypi.sh` & `timely-beliefs-1.9.2/to_pypi.sh`

 * *Files identical despite different names*

