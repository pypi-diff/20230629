# Comparing `tmp/prog_algs-1.4.3rc0.tar.gz` & `tmp/prog_algs-1.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_algs-1.4.3rc0.tar", last modified: Sat Dec  3 00:27:09 2022, max compression
+gzip compressed data, was "prog_algs-1.5.0rc0.tar", last modified: Thu Jun 29 14:59:55 2023, max compression
```

## Comparing `prog_algs-1.4.3rc0.tar` & `prog_algs-1.5.0rc0.tar`

### file list

```diff
@@ -1,47 +1,56 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.013863 prog_algs-1.4.3rc0/
--rw-r--r--   0 cteubert   (507) staff       (20)     6771 2022-12-03 00:27:09.013962 prog_algs-1.4.3rc0/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     4870 2022-12-03 00:26:43.000000 prog_algs-1.4.3rc0/README.md
--rw-r--r--   0 cteubert   (507) staff       (20)      107 2022-12-03 00:27:09.014561 prog_algs-1.4.3rc0/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2682 2022-12-03 00:26:59.000000 prog_algs-1.4.3rc0/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.006259 prog_algs-1.4.3rc0/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.007537 prog_algs-1.4.3rc0/src/prog_algs/
--rw-r--r--   0 cteubert   (507) staff       (20)     1670 2022-12-03 00:26:43.000000 prog_algs-1.4.3rc0/src/prog_algs/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)      543 2021-10-13 23:52:45.000000 prog_algs-1.4.3rc0/src/prog_algs/exceptions.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.008949 prog_algs-1.4.3rc0/src/prog_algs/metrics/
--rw-r--r--   0 cteubert   (507) staff       (20)      507 2022-10-27 16:46:06.000000 prog_algs-1.4.3rc0/src/prog_algs/metrics/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1790 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/metrics/samples.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3236 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/metrics/toe_metrics.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8614 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/metrics/toe_profile_metrics.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5403 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/metrics/uncertain_data_metrics.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.009860 prog_algs-1.4.3rc0/src/prog_algs/predictors/
--rw-r--r--   0 cteubert   (507) staff       (20)     1111 2022-03-08 19:58:41.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7294 2022-10-27 17:24:09.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/monte_carlo.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6992 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/prediction.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3959 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/predictor.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10332 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/toe_prediction_profile.py
--rw-r--r--   0 cteubert   (507) staff       (20)    13680 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/predictors/unscented_transform.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.011332 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/
--rw-r--r--   0 cteubert   (507) staff       (20)      498 2022-01-18 17:21:49.000000 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6517 2022-12-03 00:26:43.000000 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/kalman_filter.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6733 2022-12-01 23:19:49.000000 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/particle_filter.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3071 2022-12-01 23:19:49.000000 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/state_estimator.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5268 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/state_estimators/unscented_kalman_filter.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.012313 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/
--rw-r--r--   0 cteubert   (507) staff       (20)      436 2021-11-05 20:06:46.000000 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3409 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/multivariate_normal_dist.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2933 2022-10-27 17:10:21.000000 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/scalar_data.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10020 2022-10-27 17:15:20.000000 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/uncertain_data.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7217 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/unweighted_samples.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.012749 prog_algs-1.4.3rc0/src/prog_algs/utils/
--rw-r--r--   0 cteubert   (507) staff       (20)      202 2022-04-15 22:04:25.000000 prog_algs-1.4.3rc0/src/prog_algs/utils/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3926 2022-04-15 22:04:25.000000 prog_algs-1.4.3rc0/src/prog_algs/utils/table.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.013681 prog_algs-1.4.3rc0/src/prog_algs/visualize/
--rw-r--r--   0 cteubert   (507) staff       (20)      270 2021-11-08 20:08:02.000000 prog_algs-1.4.3rc0/src/prog_algs/visualize/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1948 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/visualize/plot_hist.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3674 2022-10-27 16:51:01.000000 prog_algs-1.4.3rc0/src/prog_algs/visualize/plot_scatter.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2022-12-03 00:27:09.008173 prog_algs-1.4.3rc0/src/prog_algs.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     6771 2022-12-03 00:27:09.000000 prog_algs-1.4.3rc0/src/prog_algs.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)     1379 2022-12-03 00:27:09.000000 prog_algs-1.4.3rc0/src/prog_algs.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2022-12-03 00:27:09.000000 prog_algs-1.4.3rc0/src/prog_algs.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)       51 2022-12-03 00:27:09.000000 prog_algs-1.4.3rc0/src/prog_algs.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       10 2022-12-03 00:27:09.000000 prog_algs-1.4.3rc0/src/prog_algs.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.407032 prog_algs-1.5.0rc0/
+-rw-r--r--   0 cteubert   (507) staff       (20)     6666 2023-06-29 14:59:55.406857 prog_algs-1.5.0rc0/PKG-INFO
+-rw-r--r--   0 cteubert   (507) staff       (20)     4765 2023-06-23 20:51:30.000000 prog_algs-1.5.0rc0/README.md
+-rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-29 14:59:55.407081 prog_algs-1.5.0rc0/setup.cfg
+-rw-r--r--   0 cteubert   (507) staff       (20)     2682 2023-06-29 14:57:35.000000 prog_algs-1.5.0rc0/setup.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.395671 prog_algs-1.5.0rc0/src/
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.396611 prog_algs-1.5.0rc0/src/prog_algs/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1674 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/__init__.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.398883 prog_algs-1.5.0rc0/src/prog_algs/metrics/
+-rw-r--r--   0 cteubert   (507) staff       (20)      507 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/metrics/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1786 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/metrics/samples.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3234 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_metrics.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     8605 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_profile_metrics.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     5401 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/metrics/uncertain_data_metrics.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.400109 prog_algs-1.5.0rc0/src/prog_algs/predictors/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1111 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7292 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/monte_carlo.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6985 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/prediction.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3409 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/predictor.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    10325 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/toe_prediction_profile.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    13679 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/predictors/unscented_transform.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.401633 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/
+-rw-r--r--   0 cteubert   (507) staff       (20)      498 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7491 2023-06-27 22:08:35.000000 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/kalman_filter.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     9336 2023-06-27 22:08:35.000000 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/particle_filter.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     4861 2023-06-27 22:08:35.000000 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/state_estimator.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     6172 2023-06-27 22:08:35.000000 prog_algs-1.5.0rc0/src/prog_algs/state_estimators/unscented_kalman_filter.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.402604 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/
+-rw-r--r--   0 cteubert   (507) staff       (20)      436 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3401 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/multivariate_normal_dist.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     2923 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/scalar_data.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    10019 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/uncertain_data.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     7214 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/unweighted_samples.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.403015 prog_algs-1.5.0rc0/src/prog_algs/utils/
+-rw-r--r--   0 cteubert   (507) staff       (20)      202 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/utils/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3926 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/utils/table.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.403557 prog_algs-1.5.0rc0/src/prog_algs/visualize/
+-rw-r--r--   0 cteubert   (507) staff       (20)      270 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/visualize/__init__.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1948 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_hist.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     3674 2023-06-27 22:08:27.000000 prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_scatter.py
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.397864 prog_algs-1.5.0rc0/src/prog_algs.egg-info/
+-rw-------   0 cteubert   (507) staff       (20)     6666 2023-06-29 14:59:55.000000 prog_algs-1.5.0rc0/src/prog_algs.egg-info/PKG-INFO
+-rw-------   0 cteubert   (507) staff       (20)     1564 2023-06-29 14:59:55.000000 prog_algs-1.5.0rc0/src/prog_algs.egg-info/SOURCES.txt
+-rw-------   0 cteubert   (507) staff       (20)        1 2023-06-29 14:59:55.000000 prog_algs-1.5.0rc0/src/prog_algs.egg-info/dependency_links.txt
+-rw-------   0 cteubert   (507) staff       (20)       51 2023-06-29 14:59:55.000000 prog_algs-1.5.0rc0/src/prog_algs.egg-info/requires.txt
+-rw-------   0 cteubert   (507) staff       (20)       10 2023-06-29 14:59:55.000000 prog_algs-1.5.0rc0/src/prog_algs.egg-info/top_level.txt
+drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 14:59:55.406571 prog_algs-1.5.0rc0/tests/
+-rw-r--r--   0 cteubert   (507) staff       (20)     1750 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_examples.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1230 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_manual.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    25519 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_metrics.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    17001 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_predictors.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    20665 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_state_estimators.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      582 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_templates.py
+-rw-r--r--   0 cteubert   (507) staff       (20)      743 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_tutorials.py
+-rw-r--r--   0 cteubert   (507) staff       (20)    21671 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_uncertain_data.py
+-rw-r--r--   0 cteubert   (507) staff       (20)     1693 2023-06-20 20:23:09.000000 prog_algs-1.5.0rc0/tests/test_visualize.py
```

### Comparing `prog_algs-1.4.3rc0/PKG-INFO` & `prog_algs-1.5.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_algs
-Version: 1.4.3rc0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations
 Home-page: https://nasa.github.io/progpy/prog_algs_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_algs/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_algs_guide.html
@@ -21,15 +21,15 @@
 Classifier: License :: Other/Proprietary License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 
 # Prognostics Algorithm Python Package
 [![CodeFactor](https://www.codefactor.io/repository/github/nasa/prog_algs/badge)](https://www.codefactor.io/repository/github/nasa/prog_algs)
 [![GitHub License](https://img.shields.io/badge/License-NOSA-green)](https://github.com/nasa/prog_algs/blob/master/license.pdf)
 [![GitHub Releases](https://img.shields.io/github/release/nasa/prog_algs.svg)](https://github.com/nasa/prog_algs/releases)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nasa/prog_algs/master?tutorial.ipynb)
@@ -43,40 +43,39 @@
 
 ## Documentation
 See documentation [here](https://nasa.github.io/progpy/prog_algs_guide.html)
 
 ## Repository Directory Structure 
 
 `src/prog_algs/` - The prognostics algorithm python package<br />
-`docs/` - Project documentation (see also [github.io](https://nasa.github.io/prog_algs/))<br />
 `examples/` - Example Python scripts using prog_algs<br />
 `tests/` - Tests for prog_models<br />
 `README.md` - The readme (this file)<br />
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2022_nasa_prog_algs,
+@misc{2023_nasa_prog_algs,
     author    = {Christopher Teubert and Matteo Corbetta and Chetan Kulkarni},
     title     = {Prognostics Algorithm Python Package},
-    month     = Dec,
-    year      = 2022,
-    version   = {1.4.3},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog\_algs}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.4.3, Dec 2022. URL https://github.com/nasa/prog_algs.
+C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.5, May 2023. URL https://github.com/nasa/prog_algs.
 
 Alternatively, if using both prog_models and prog_algs, you can cite the combined package as
 
-C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.4, December 2022. URL https://nasa.github.io/progpy.
+C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.5, May 2023. URL https://nasa.github.io/progpy.
 
 ## Acknowledgements
 The structure and algorithms of this package are strongly inspired by the [MATLAB Prognostics Algorithm Library](https://github.com/nasa/PrognosticsAlgorithmLibrary) and the [MATLAB Prognostics Metrics Library](https://github.com/nasa/PrognosticsMetricsLibrary). We would like to recognize Matthew Daigle, Shankar Sankararaman and the rest of the team that contributed to the Prognostics Model Library for the contributions their work on the MATLAB library made to the design of prog_algs
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
```

### Comparing `prog_algs-1.4.3rc0/README.md` & `prog_algs-1.5.0rc0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,40 +13,39 @@
 
 ## Documentation
 See documentation [here](https://nasa.github.io/progpy/prog_algs_guide.html)
 
 ## Repository Directory Structure 
 
 `src/prog_algs/` - The prognostics algorithm python package<br />
-`docs/` - Project documentation (see also [github.io](https://nasa.github.io/prog_algs/))<br />
 `examples/` - Example Python scripts using prog_algs<br />
 `tests/` - Tests for prog_models<br />
 `README.md` - The readme (this file)<br />
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2022_nasa_prog_algs,
+@misc{2023_nasa_prog_algs,
     author    = {Christopher Teubert and Matteo Corbetta and Chetan Kulkarni},
     title     = {Prognostics Algorithm Python Package},
-    month     = Dec,
-    year      = 2022,
-    version   = {1.4.3},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog\_algs}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.4.3, Dec 2022. URL https://github.com/nasa/prog_algs.
+C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.5, May 2023. URL https://github.com/nasa/prog_algs.
 
 Alternatively, if using both prog_models and prog_algs, you can cite the combined package as
 
-C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.4, December 2022. URL https://nasa.github.io/progpy.
+C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.5, May 2023. URL https://nasa.github.io/progpy.
 
 ## Acknowledgements
 The structure and algorithms of this package are strongly inspired by the [MATLAB Prognostics Algorithm Library](https://github.com/nasa/PrognosticsAlgorithmLibrary) and the [MATLAB Prognostics Metrics Library](https://github.com/nasa/PrognosticsMetricsLibrary). We would like to recognize Matthew Daigle, Shankar Sankararaman and the rest of the team that contributed to the Prognostics Model Library for the contributions their work on the MATLAB library made to the design of prog_algs
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
```

### Comparing `prog_algs-1.4.3rc0/setup.py` & `prog_algs-1.5.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name = 'prog_algs',
-    version = '1.4.3-rc0',
+    version = '1.5.0.pre',
     description = "The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url = 'https://nasa.github.io/progpy/prog_algs_guide.html',
     author = 'Christopher Teubert',
     author_email = 'christopher.a.teubert@nasa.gov',
     classifiers = [
@@ -32,21 +32,21 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3 :: Only'
     ],
     keywords = ['prognostics', 'diagnostics', 'fault detection', 'fdir', 'prognostics and health management', 'PHM', 'health management', 'ivhm'],
     package_dir = {"":"src"},
     packages = find_packages(where = 'src'),
-    python_requires='>=3.7, <3.11',
+    python_requires='>=3.7, <3.12',
     install_requires = [
         'numpy',
         'scipy',
         'filterpy',
         'matplotlib',
-        'prog_models>=1.4.0'
+        'prog_models>=1.5.0'
     ],
     license = 'NOSA',
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/nasa/prog_algs/issues',
         'Docs': 'https://nasa.github.io/progpy/prog_algs_guide.html',
         'Organization': 'https://www.nasa.gov/content/diagnostics-prognostics',
         'Source': 'https://github.com/nasa/prog_algs',
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/__init__.py` & `prog_algs-1.5.0rc0/src/prog_algs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 __all__ = ['predictors', 'uncertain_data', 'state_estimators', 'run_prog_playback', 'metrics']
 from . import predictors, state_estimators, uncertain_data
 
 import warnings
 
-__version__ = '1.4.3'
+__version__ = '1.5.0.pre'
 
 def run_prog_playback(obs, pred, future_loading, output_measurements, **kwargs):
     warnings.warn("Depreciated in 1.2.0, will be removed in a future release.", DeprecationWarning)
     config = {# Defaults
         'predict_rate': 0, # Default- predict every step
         'num_samples': 10,
         'predict_config': {}
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/metrics/samples.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/samples.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from numpy import mean, sqrt
 from warnings import warn
 
 from .uncertain_data_metrics import calc_metrics as eol_metrics
 from .toe_metrics import prob_success
 from .toe_profile_metrics import alpha_lambda
 
-def mean_square_error(values : list, ground_truth : float) -> float:
+def mean_square_error(values: list, ground_truth: float) -> float:
     """Mean Square Error
     Args:
         values (List[float]): Times of Event (ToE) for a single event, output from predictor
         ground_truth (float): Ground truth ToE
     Returns:
         float: mean square error of ToE predictions
     """
@@ -24,15 +24,15 @@
         values (List[float]): Times of Event (ToE) for a single event, output from predictor
         ground_truth (float): Ground truth ToE
     Returns:
         float: root mean square error of ToE predictions
     """
     return sqrt(sum([(mean(x) - ground_truth)**2 for x in values])/len(values))
 
-def percentage_in_bounds(toe : list, bounds : tuple) -> float:
+def percentage_in_bounds(toe: list, bounds: tuple) -> float:
     """Calculate percentage of ToE dist is within specified bounds
 
     Args:
         toe (List[float]): Times of Event (ToE) for a single event, output from predictor
         bounds ((float, float)): Lower and upper bounds
 
     Returns:
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/metrics/toe_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file includes functions for calculating metrics specific to Time of Event (ToE) from a single event or multiple events given the same time of prediction
 """
 from typing import Iterable
 from numpy import isscalar
 
 from ..uncertain_data import UncertainData, UnweightedSamples
 
-def prob_success(toe : UncertainData, time : float, **kwargs) -> float:
+def prob_success(toe: UncertainData, time: float, **kwargs) -> float:
     """Calculate probability of success - i.e., probability that event will not occur within a given time (i.e., success)
 
     Args:
         toe (UncertainData or list[float]): Times of event for a single event (array[float]) or multiple events, output from predictor
         time (float): time for calculation
         **kwargs (optional): Configuration parameters. Supported parameters include:
           * n_samples (int): Number of samples to use for calculating metrics (if ToE is not UnweightedSamples). Defaults to 10,000.
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/metrics/toe_profile_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_profile_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 from numpy import sign
 from collections import defaultdict
 from typing import Callable, Dict
 
 from ..predictors import ToEPredictionProfile
 
-def alpha_lambda(toe_profile : ToEPredictionProfile, ground_truth : dict, lambda_value : float, alpha : float, beta : float, **kwargs) -> dict: 
+def alpha_lambda(toe_profile: ToEPredictionProfile, ground_truth: dict, lambda_value: float, alpha: float, beta: float, **kwargs) -> dict: 
     """
     Compute alpha lambda metric, a common metric in prognostics. Alpha-Lambda is met if alpha % of the Time to Event (TtE) distribution is within beta % of the ground truth at prediction time lambda.
 
     Args:
         toe_profile (ToEPredictionProfile): A profile of predictions, the combination of multiple predictions
         ground_truth (dict): Ground Truth time of event for each event (e.g., {'event1': 748, 'event2', 2233, ...})
         lambda_value (float): Prediction time at or after which metric is evaluated. Evaluation occurs at this time (if a prediction exists) or the next prediction following.
@@ -41,15 +41,15 @@
             if params['print']:
                 for key in keys:
                     print('\n', key)
                     print('\ttoe:', toe.key(key))
                     print('\tBounds: [{} - {}]({}%)'.format(bounds[key][0], bounds[key][1], pib[key]))
             return result
 
-def prognostic_horizon(toe_profile : ToEPredictionProfile, criteria_eqn : Callable, ground_truth : dict, **kwargs) -> dict:
+def prognostic_horizon(toe_profile: ToEPredictionProfile, criteria_eqn: Callable, ground_truth: dict, **kwargs) -> dict:
     """
     Compute prognostic horizon metric, defined as the difference between a time ti, when the predictions meet specified performance criteria, and the time corresponding to the true Time of Event (ToE), for each event.
     PH = ToE - ti
     Args:
         toe_profile (ToEPredictionProfile): A profile of predictions, the combination of multiple predictions
         criteria_eqn (Callable function): A function (tte: UncertainData, ground_truth_tte: dict[str, float]) -> dict[str, bool] calculating whether a prediction in ToEPredictionProfile meets some criteria. \n
             | Args: 
@@ -65,34 +65,34 @@
         dict: Dictionary containing prognostic horizon calculations (value) for each event (key). e.g., {'event1': 12.3, 'event2': 15.1}
     """
     params = {
         'print': False
     }
     params.update(kwargs)
 
-    ph_result = {k:None for k in ground_truth.keys()} # False means not yet met; will be either a numerical value or None if met
+    ph_result = {k:None for k in ground_truth.keys()}  # False means not yet met; will be either a numerical value or None if met
     for (t_prediction, toe) in toe_profile.items():
         # Convert to TtE for toe and ground_truth
         tte = toe - t_prediction
         ground_truth_tte = {}
         ground_truth_tte = {k:v-t_prediction for k,v in ground_truth.items()}
         # Pass to criteria_eqn
         criteria_eqn_dict = criteria_eqn(tte, ground_truth_tte) # -> dict[event_names as str, bool]
         for k,v in criteria_eqn_dict.items():
             if v and (ph_result[k] == None):
                 ph_calc = ground_truth[k] - t_prediction
                 if ph_calc > 0:
-                    ph_result[k] = ph_calc # PH = EOL - ti # ground truth is a dictionary {'EOD': 3005.2} should be ph_result[k] = g_truth[key] - t_prediction
+                    ph_result[k] = ph_calc  # PH = EOL - ti # ground truth is a dictionary {'EOD': 3005.2} should be ph_result[k] = g_truth[key] - t_prediction
                 if (all(v != None for v in ph_result.values())):
                     # Return PH once all criteria are met
                     return ph_result
     # Return PH when criteria not met for at least one event key
     return ph_result
 
-def cumulative_relative_accuracy(toe_profile : ToEPredictionProfile, ground_truth : dict, **kwargs) -> Dict[str, float]:
+def cumulative_relative_accuracy(toe_profile: ToEPredictionProfile, ground_truth: dict, **kwargs) -> Dict[str, float]:
     """
     Compute cumulative relative accuracy for a given profile, defined as the normalized sum of relative prediction accuracies at specific time instances.
     
     CRA = Σ(RA)/N for each event
     Where Σ is summation of all relative accuracies for a given profile and N is the total count of profiles (Journal Prognostics Health Management, Saxena et al.)
     Args:
         toe_profile (ToEPredictionProfile): A profile of predictions, the combination of multiple predictions
@@ -104,15 +104,15 @@
     """
     ra_sums = defaultdict(int)
     for uncertaindata in toe_profile.values():
         for event,value in uncertaindata.relative_accuracy(ground_truth).items():
             ra_sums[event] += value
     return {event:ra_sum/len(toe_profile) for event, ra_sum in ra_sums.items()}
 
-def monotonicity(toe_profile : ToEPredictionProfile, **kwargs) -> Dict[str, float]:
+def monotonicity(toe_profile: ToEPredictionProfile, **kwargs) -> Dict[str, float]:
         """Calculate monotonicty for a prediction profile. 
         Given a prediction profile, for each prediction: go through all predicted events and compare those to the next one.
         Calculates monotonicity for each prediction key using its associated mean value in UncertainData.
         
         monotonoicity = |Σsign(i+1 - i) / N-1|
         Where N is number of measurements and sign indicates sign of calculation.
         Coble, J., et. al. (2021). Identifying Optimal Prognostic Parameters from Data: A Genetic Algorithms Approach. Annual Conference of the PHM Society.
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/metrics/uncertain_data_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/uncertain_data_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Iterable, Union
 from numpy import isscalar, mean, std, array
 from scipy import stats
 from warnings import warn
 
 from ..uncertain_data import UncertainData, UnweightedSamples
 
-def calc_metrics(data : UncertainData, ground_truth : Union[float, dict] = None, **kwargs) -> dict:
+def calc_metrics(data: UncertainData, ground_truth: Union[float, dict] = None, **kwargs) -> dict:
     """Calculate all time of event metrics
 
     Args:
         data (array[float] or UncertainData): data from a single event
         ground_truth (float, optional): Ground truth value. Defaults to None. dict when data is  of type UncertainData.
         **kwargs (optional): Configuration parameters. Supported parameters include:
           * n_samples (int): Number of samples to use for calculating metrics (if data is not UnweightedSamples). Defaults to 10,000.
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/__init__.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/monte_carlo.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/monte_carlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         Any additional savepoints (s) e.g., [10.1, 22.5]
     """
 
     default_parameters = { 
         'n_samples': 100  # Default number of samples to use, if none specified
     }
 
-    def predict(self, state : UncertainData, future_loading_eqn : Callable, **kwargs) -> PredictionResults:
+    def predict(self, state: UncertainData, future_loading_eqn: Callable, **kwargs) -> PredictionResults:
         if isinstance(state, dict) or isinstance(state, self.model.StateContainer):
             from prog_algs.uncertain_data import ScalarData
             state = ScalarData(state, _type = self.model.StateContainer)
         elif isinstance(state, UncertainData):
             state._type = self.model.StateContainer
         else:
             raise TypeError("state must be UncertainData, dict, or StateContainer")
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/prediction.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,26 +21,26 @@
             Data points for each time in times 
     """
 
     def __init__(self, times : list, data : list):
         self.times = times
         self.data = data
 
-    def __eq__(self, other : "Prediction") -> bool:
+    def __eq__(self, other: "Prediction") -> bool:
         """Compare 2 Predictions
 
         Args:
             other (Prediction):
 
         Returns:
             bool: If the two Predictions are equal
         """
         return self.times == other.times and self.data == other.data
 
-    def snapshot(self, time_index : int) -> UncertainData:
+    def snapshot(self, time_index: int) -> UncertainData:
         """Get all samples from a specific timestep
 
         Args:
             index (int):
                 Timestep (index number from times)
 
         Returns:
@@ -59,15 +59,15 @@
                 e.g., [{'state1': 1.2, 'state2': 1.3, ...}, ...]
 
         Example:
             mean_value = data.mean
         """
         return [dist.mean for dist in self.data]
 
-    def time(self, index : int):
+    def time(self, index: int):
         warn("Deprecated. Please use prediction.times[index] instead.")
         return self.times[index]
 
     def monotonicity(self) -> Dict[str, float]:
         """Calculate monotonicty for a single prediction. 
         Given a single prediction, for each event: go through all predicted states and compare those to the next one.
         Calculates monotonicity for each event key using its associated mean value in UncertainData.
@@ -106,15 +106,15 @@
     Args:
         times (list[float]):
             Times for each data point where times[n] corresponds to data[:][n]
         data (list[SimResult]):
             Data points where data[n] is a SimResult for sample n
     """
 
-    def __init__(self, times : list, data : list):
+    def __init__(self, times: list, data: list):
         super(UnweightedSamplesPrediction, self).__init__(times, data)
         self.__transformed = False  # If transform has been calculated
 
     def __calculate_tranform(self):
         """
         Calculate tranform of the data from data[sample_id][time_id] to data[time_id][sample_id]. Result is cached as self.__transform and is used in methods which look at a snapshot for a specific time
         """
@@ -129,19 +129,19 @@
 
     @property
     def mean(self) -> list:
         if not self.__transformed:
             self.__calculate_tranform()
         return [dist.mean for dist in self.__transform]
 
-    def sample(self, sample_id : int):
+    def sample(self, sample_id: int):
         warn("Deprecated. Please use prediction[sample_id] instead.")
         return self[sample_id]
 
-    def snapshot(self, time_index : int) -> UnweightedSamples:
+    def snapshot(self, time_index: int) -> UnweightedSamples:
         """Get all samples from a specific timestep
 
         Args:
             index (int): Timestep (index number from times)
 
         Returns:
             UnweightedSamples: Samples for time corresponding to times[timestep]
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/predictor.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/predictor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 from abc import ABC, abstractmethod
 from copy import deepcopy
 from typing import Callable
 
 from prog_algs.predictors.prediction import PredictionResults
-from ..exceptions import ProgAlgTypeError
 from ..uncertain_data import UncertainData
 
 
 class Predictor(ABC):
     """
     Interface class for predictors
 
@@ -22,60 +21,47 @@
         A prognostics model to be used in prediction
     kwargs : optional, keyword arguments
     """
     default_parameters = {}
 
     def __init__(self, model, **kwargs):
         if not hasattr(model, 'output'):
-            raise ProgAlgTypeError("model must have `output` method")
+            raise NotImplementedError("model must have `output` method")
         if not hasattr(model, 'next_state'):
-            raise ProgAlgTypeError("model must have `next_state` method")
+            raise NotImplementedError("model must have `next_state` method")
         if not hasattr(model, 'inputs'):
-            raise ProgAlgTypeError("model must have `inputs` property")
+            raise NotImplementedError("model must have `inputs` property")
         if not hasattr(model, 'outputs'):
-            raise ProgAlgTypeError("model must have `outputs` property")
+            raise NotImplementedError("model must have `outputs` property")
         if not hasattr(model, 'states'):
-            raise ProgAlgTypeError("model must have `states` property")
+            raise NotImplementedError("model must have `states` property")
         if not hasattr(model, 'simulate_to_threshold'):
-            raise ProgAlgTypeError("model must have `simulate_to_threshold` property")
+            raise NotImplementedError("model must have `simulate_to_threshold` property")
         self.model = model
 
         self.parameters = deepcopy(self.default_parameters)
         self.parameters['events'] = self.model.events.copy()  # Events to predict to
         self.parameters.update(kwargs)
 
     @abstractmethod
-    def predict(self, state : UncertainData, future_loading_eqn : Callable, **kwargs) -> PredictionResults:
+    def predict(self, state: UncertainData, future_loading_eqn: Callable, **kwargs) -> PredictionResults:
         """
         Perform a single prediction
 
         Parameters
         ----------
         state : UncertainData 
             Distribution representing current state of the system
         future_loading_eqn : function (t, x) -> z
             Function to generate an estimate of loading at future time t, and state x
 
-        Keyword Arguments
-        -------------------
-        dt : float
-            Simulation step size (s), e.g., 0.1
-        events : list[str]
-            Events to predict (subset of model.events) e.g., ['event1', 'event2']
-        horizon : float
-            Prediction horizon (s)
-        save_freq : float
-            Frequency at which results are saved (s)
-        save_pts : list[float]
-            Any additional savepoints (s) e.g., [10.1, 22.5]
-
         Return
         ----------
-        NamedTuple
-            * times (list[float]): Times for each savepoint such that inputs.snapshot(i), states.snapshot(i), outputs.snapshot(i), and event_states.snapshot(i) are all at times[i]            
-            * inputs (:py:class:`Prediction`): Inputs at each savepoint such that inputs.snapshot(i) is the input distribution (type UncertainData) at times[i]
-            * states (:py:class:`Prediction`): States at each savepoint such that states.snapshot(i) is the state distribution (type UncertainData) at times[i]
-            * outputs (:py:class:`Prediction`): Outputs at each savepoint such that outputs.snapshot(i) is the output distribution (type UncertainData) at times[i]
-            * event_states (:py:class:`Prediction`): Event states at each savepoint such that event_states.snapshot(i) is the event state distribution (type UncertainData) at times[i]
-            * time_of_event (:py:class:`prog_algs.uncertain_data.UncertainData`): Distribution of predicted Time of Event (ToE) for each predicted event, represented by some subclass of UncertaintData (e.g., :py:class:`MultivariateNormalDist`)
+        result from prediction, including: NameTuple
+            * times (List[float]): Times for each savepoint such that inputs.snapshot(i), states.snapshot(i), outputs.snapshot(i), and event_states.snapshot(i) are all at times[i]            
+            * inputs (Prediction): Inputs at each savepoint such that inputs.snapshot(i) is the input distribution (type UncertainData) at times[i]
+            * states (Prediction): States at each savepoint such that states.snapshot(i) is the state distribution (type UncertainData) at times[i]
+            * outputs (Prediction): Outputs at each savepoint such that outputs.snapshot(i) is the output distribution (type UncertainData) at times[i]
+            * event_states (Prediction): Event states at each savepoint such that event_states.snapshot(i) is the event state distribution (type UncertainData) at times[i]
+            * time_of_event (UncertainData): Distribution of predicted Time of Event (ToE) for each predicted event, represented by some subclass of UncertaintData (e.g., MultivariateNormalDist)
         """
         pass
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/toe_prediction_profile.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/toe_prediction_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     def values(self):
         """
         Get iterator for the values (i.e., toe_prediction) of the prediction profile
         """
         return [self[k] for k in self.keys()]
 
-    def alpha_lambda(self, ground_truth : Dict[str, float], lambda_value : float, alpha : float, beta : float, **kwargs) -> Dict[str, bool]:
+    def alpha_lambda(self, ground_truth: Dict[str, float], lambda_value: float, alpha: float, beta: float, **kwargs) -> Dict[str, bool]:
         """Calculate Alpha lambda metric for the prediction profile
 
         Args:
             ground_truth (dict[str, float]):
                 Ground Truth time of event for each event (e.g., {'event1': 748, 'event2', 2233, ...})
             lambda_value (float):
                 Prediction time at or after which metric is evaluated. Evaluation occurs at this time (if a prediction exists) or the next prediction following.
@@ -130,15 +130,15 @@
         References:
             .. [1] Coble, J., et. al. (2021). Identifying Optimal Prognostic Parameters from Data: A Genetic Algorithms Approach. Annual Conference of the PHM Society. http://www.papers.phmsociety.org/index.php/phmconf/article/view/1404
             .. [2] Baptistia, M., et. al. (2022). Relation between prognostics predictor evaluation metrics and local interpretability SHAP values. Aritifical Intelligence, Volume 306. https://www.sciencedirect.com/science/article/pii/S0004370222000078
         """
         from ..metrics import monotonicity
         return monotonicity(self, **kwargs)
     
-    def plot(self, ground_truth : dict = None , alpha : float = None, show : bool = True) -> dict: # use ground truth, alpha if given,
+    def plot(self, ground_truth: dict = None , alpha: float = None, show: bool = True) -> dict: # use ground truth, alpha if given,
         """Produce an alpha-beta plot depicting the TtE distribution by time of prediction for each event.
 
         Args:
             ground_truth (dict):
                 Optional dictionary argument containing event and its respective ground truth value; none by default and plotted if specified
             alpha (float):
                 Optional alpha value; none by default and plotted if specified
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/predictors/unscented_transform.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/unscented_transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
             x = model.apply_limits(x)
             return array(list(x.values()))
 
         self.sigma_points = kalman.MerweScaledSigmaPoints(num_states, alpha=self.parameters['alpha'], beta=self.parameters['beta'], kappa=self.parameters['kappa'])
         self.filter = kalman.UnscentedKalmanFilter(num_states, num_measurements, self.parameters['dt'], measure, state_transition, self.sigma_points)
         self.filter.Q = self.parameters['Q']
 
-    def predict(self, state, future_loading_eqn : Callable, **kwargs) -> PredictionResults:
+    def predict(self, state, future_loading_eqn: Callable, **kwargs) -> PredictionResults:
         """
         Perform a single prediction
 
         Parameters
         ----------
         state (UncertaintData): Distribution of states
         future_loading_eqn : function (t, x={}) -> z
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/state_estimators/kalman_filter.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/kalman_filter.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     Keyword Args:
         alpha (float, optional):
             KF Scaling parameter. An alpha > 1 turns this into a fading memory filter.
         t0 (float, optional):
             Starting time (s)
         dt (float, optional):
-            time step (s)
+            Maximum timestep for prediction in seconds. By default, the timestep dt is the difference between the last and current call of .estimate(). Some models are unstable at larger dt. Setting a smaller dt will force the model to take smaller steps; resulting in multiple prediction steps for each estimate step. Default is the parameters['dt']
+            e.g., dt = 1e-2
         Q (list[list[float]], optional):
             Kalman Process Noise Matrix 
         R (list[list[float]], optional):
             Kalman Measurement Noise Matrix
     """
     default_parameters = {
         'alpha': 1, 
@@ -92,54 +93,60 @@
             raise TypeError("TypeError: x0 initial state must be of type {{dict, UncertainData}}")
 
         self.filter.Q = self.parameters['Q']
         self.filter.R = self.parameters['R']
         self.filter.F = F
         self.filter.B = B
 
-    def estimate(self, t : float, u, z):
+    def estimate(self, t: float, u, z, **kwargs):
         """
         Perform one state estimation step (i.e., update the state estimate)
 
         Parameters
         ----------
         t : double
             Current timestamp in seconds (≥ 0.0)
             e.g., t = 3.4
         u : dict
             Measured inputs, with keys defined by model.inputs.
             e.g., u = {'i':3.2} given inputs = ['i']
         z : dict
             Measured outputs, with keys defined by model.outputs.
             e.g., z = {'t':12.4, 'v':3.3} given inputs = ['t', 'v']
+
+        Keyword Arguments
+        -----------------
+        dt : float, optional
+            Maximum timestep for prediction in seconds. By default, the timestep dt is the difference between the last and current call of .estimate(). Some models are unstable at larger dt. Setting a smaller dt will force the model to take smaller steps; resulting in multiple prediction steps for each estimate step. Default is the parameters['dt']
+            e.g., dt = 1e-2
         """
         assert t > self.t, "New time must be greater than previous"
-
-        dt = t - self.t
+        dt = kwargs.get('dt', self.parameters['dt'])
+        dt = min(t - self.t, dt)  # Ensure dt is not larger than the maximum time step
         # Create u array, ensuring order of model.inputs. And reshaping to (n,1), n can be 0.
         inputs = np.array([u[key] for key in self.model.inputs]).reshape((-1,1))
 
         # Add row of ones (to account for constant E term)
         if np.size(inputs) == 0:
             inputs = np.array([[1]])
         else:
             inputs = np.append(inputs, [[1]], 0)
 
-        self.t = t
-
         # Update equations
         # prog_models is dx = Ax + Bu + E
         # kalman_models is x' = Fx + Bu, where x' is the next state
         # Therefore we need to add the diagnol matrix 1 to A to convert
         # And A and B should be multiplied by the time step
         B = np.multiply(self.filter.B, dt) 
         F = np.multiply(self.filter.F, dt) + np.diag([1]* self.model.n_states)
 
         # Predict
-        self.filter.predict(u = inputs, B = B, F = F)
+        while self.t < t :
+            self.filter.predict(u = inputs, B = B, F = F)
+            self.t += dt
 
         # Create z array, ensuring order of model.outputs
         outputs = np.array([z[key] for key in self.model.outputs])
 
         # Subtract D from outputs
         # This is done because prog_models expects the form: 
         #   z = Cx + D
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/state_estimators/unscented_kalman_filter.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/unscented_kalman_filter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 from filterpy import kalman
 from numpy import diag, array
 from warnings import warn
 
-from . import state_estimator
-from ..uncertain_data import MultivariateNormalDist, UncertainData
+from prog_algs.state_estimators import state_estimator
+from prog_algs.uncertain_data import MultivariateNormalDist, UncertainData
 
 class UnscentedKalmanFilter(state_estimator.StateEstimator):
     """
     An Unscented Kalman Filter (UKF) for state estimation
 
     This class defines logic for performing an unscented kalman filter with a Prognostics Model (see Prognostics Model Package). This filter uses measurement data with noise to generate a state estimate and covariance matrix. 
 
@@ -29,26 +29,25 @@
         beta (float, optional):
             UKF Scaling parameter
         kappa (float, optional):
             UKF Scaling parameter
         t0 (float, optional):
             Starting time (s)
         dt (float, optional):
-            time step (s)
+            Maximum timestep for prediction in seconds. By default, the timestep dt is the difference between the last and current call of .estimate(). Some models are unstable at larger dt. Setting a smaller dt will force the model to take smaller steps; resulting in multiple prediction steps for each estimate step. Default is the parameters['dt']
+            e.g., dt = 1e-2
         Q (list[list[float]], optional):
             Process Noise Matrix 
         R (list[list[float]], optional):
             Measurement Noise Matrix 
     """
     default_parameters = {
         'alpha': 1, 
         'beta': 0, 
         'kappa': -1,
-        't0': -1e-10,
-        'dt': 1
     } 
 
     def __init__(self, model, x0, **kwargs):
         super().__init__(model, x0, **kwargs)
 
         self.__input = None
         self.x0 = x0
@@ -59,15 +58,15 @@
             R_err = model.parameters['measurement_noise'].copy()
             model.parameters['measurement_noise'] = dict.fromkeys(R_err, 0)
             z = model.output(x)
             model.parameters['measurement_noise'] = R_err
             return array(list(z.values())).ravel()
 
         if 'Q' not in self.parameters:
-            self.parameters['Q'] = diag([1.0e-3 for i in x0.keys()])
+            self.parameters['Q'] = diag([1.0e-3 for _ in x0.keys()])
 
         def state_transition(x, dt):
             x = model.StateContainer({key: value for (key, value) in zip(x0.keys(), x)})
             Q_err = model.parameters['process_noise'].copy()
             model.parameters['process_noise'] = dict.fromkeys(Q_err, 0)
             x = model.next_state(x, self.__input, dt)
             return array(list(x.values())).ravel()
@@ -91,40 +90,48 @@
         if 'R' not in self.parameters:
             # Size of what's being measured (not output) 
             # This is determined by running the measure function on the first state
             self.parameters['R'] = diag([1.0e-3 for i in range(len(measure(self.filter.x)))])
         self.filter.Q = self.parameters['Q']
         self.filter.R = self.parameters['R']
 
-    def estimate(self, t : float, u, z):
+    def estimate(self, t: float, u, z, **kwargs):
         """
         Perform one state estimation step (i.e., update the state estimate)
 
         Parameters
         ----------
         t : double
             Current timestamp in seconds (≥ 0.0)
             e.g., t = 3.4
         u : dict
             Measured inputs, with keys defined by model.inputs.
             e.g., u = {'i':3.2} given inputs = ['i']
         z : dict
             Measured outputs, with keys defined by model.outputs.
             e.g., z = {'t':12.4, 'v':3.3} given inputs = ['t', 'v']
+
+        Keyword Args
+        ------------
+        dt : float, optional
+            Maximum timestep for prediction in seconds. By default, the timestep dt is the difference between the last and current call of .estimate(). Some models are unstable at larger dt. Setting a smaller dt will force the model to take smaller steps; resulting in multiple prediction steps for each estimate step. Default is the parameters['dt']
+            e.g., dt = 1e-2
         """
         assert t > self.t, "New time must be greater than previous"
-        dt = t - self.t
+        dt = kwargs.get('dt', self.parameters['dt'])
+        dt = min(t - self.t, dt)
         self.__input = u
-        self.t = t
-        self.filter.predict(dt=dt)
+        while self.t < t:
+            self.filter.predict(dt=dt)
+            self.t += dt
         self.filter.update(array(list(z.values())))
     
     @property
     def x(self) -> MultivariateNormalDist:
         """
         Getter for property 'x', the current estimated state. 
 
         Example
         -------
         state = observer.x
         """
-        return MultivariateNormalDist(self.x0.keys(), self.filter.x, self.filter.P, _type = self.model.StateContainer)
+        return MultivariateNormalDist(self.x0.keys(), self.filter.x, self.filter.P, _type=self.model.StateContainer)
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/multivariate_normal_dist.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/multivariate_normal_dist.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,48 +20,48 @@
         self.__mean = array(list(mean))
         self.__covar = array(list(covar))
         super().__init__(_type)
 
     def __reduce__(self):
         return (MultivariateNormalDist, (self.__labels, self.__mean, self.__covar))
 
-    def __eq__(self, other : "MultivariateNormalDist") -> bool:
+    def __eq__(self, other: "MultivariateNormalDist") -> bool:
         return isinstance(other, MultivariateNormalDist) and self.keys() == other.keys() and self.mean == other.mean and (self.cov == other.cov).all()
 
-    def __add__(self, other : int) -> "UncertainData":
+    def __add__(self, other: int) -> "UncertainData":
         if other == 0:
             return self
         return MultivariateNormalDist(self.__labels, array([i+other for i in self.__mean]), self.__covar)
 
-    def __radd__(self, other : int) -> "UncertainData":
+    def __radd__(self, other: int) -> "UncertainData":
         return self.__add__(other)
 
-    def __iadd__(self, other : int) -> "UncertainData":
+    def __iadd__(self, other: int) -> "UncertainData":
         if not isinstance(other, (int, float)):
             raise TypeError(f" unsupported operand type(s) for +: '{type(other)}' and '{type(self.__mean[0])}'")
         if other != 0:
             self.__mean = array([i+other for i in self.__mean])
         return self
 
-    def __sub__(self, other : int) -> "UncertainData":
+    def __sub__(self, other: int) -> "UncertainData":
         if other == 0:
             return self
         return MultivariateNormalDist(self.__labels, array([i-other for i in self.__mean]), self.__covar)
 
-    def __rsub__(self, other : int) -> "UncertainData":
+    def __rsub__(self, other: int) -> "UncertainData":
         return self.__sub__(other)
 
-    def __isub__(self, other : int) -> "UncertainData":
+    def __isub__(self, other: int) -> "UncertainData":
         if not isinstance(other, (int, float)):
             raise TypeError(f" unsupported operand type(s) for -: '{type(other)}' and '{type(self.__mean[0])}'")
         if other != 0:
             self.__mean = array([i-other for i in self.__mean])
         return self
 
-    def sample(self, num_samples : int = 1) -> UnweightedSamples:
+    def sample(self, num_samples: int = 1) -> UnweightedSamples:
         if len(self.__mean) != len(self.__labels):
             raise Exception("labels must be provided for each value")
     
         samples = multivariate_normal(self.__mean, self.__covar, num_samples)
         samples = [{key: value for (key, value) in zip(self.__labels, x)} for x in samples]
         return UnweightedSamples(samples, _type = self._type)
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/scalar_data.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/scalar_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,51 +9,51 @@
 class ScalarData(UncertainData):
     """
     Data without uncertainty- single value
 
     Args:
         state (dict or Container): Single state in the form of dict or model.*Container (InputContainer, OutputContainer, Statecontainer) representing states and respective values.
     """
-    def __init__(self, state, _type = dict): 
+    def __init__(self, state, _type=dict): 
         self.__state = state
         super().__init__(_type)
     
     def __reduce__(self):
         return (ScalarData, (self.__state, ))
 
-    def __eq__(self, other : "ScalarData") -> bool:
+    def __eq__(self, other: "ScalarData") -> bool:
         return isinstance(other, ScalarData) and other.mean == self.__state
 
-    def __add__(self, other : int) -> "UncertainData":
+    def __add__(self, other: int) -> "UncertainData":
         if other == 0:
             return self
         new_state = dict()
         for k,v in self.__state.items():
             new_state[k] = v + other
         return ScalarData(new_state)
 
-    def __radd__(self, other : int) -> "UncertainData":
+    def __radd__(self, other: int) -> "UncertainData":
         return self.__add__(other)
 
-    def __iadd__(self, other : int) -> "UncertainData":
+    def __iadd__(self, other: int) -> "UncertainData":
         if other != 0:
             for k in self.__state.keys():
                 self.__state[k] += other
         return self
 
-    def __sub__(self, other : int) -> "UncertainData":
+    def __sub__(self, other: int) -> "UncertainData":
         new_state = dict()
         for k,v in self.__state.items():
             new_state[k] = v - other
         return ScalarData(new_state)
 
-    def __rsub__(self, other : int) -> "UncertainData":
+    def __rsub__(self, other: int) -> "UncertainData":
         return self.__sub__(other)
 
-    def __isub__(self, other : int) -> "UncertainData":
+    def __isub__(self, other: int) -> "UncertainData":
         if other != 0:
             for k in self.__state.keys():
                 self.__state[k] -= other
         return self
 
     @property
     def median(self) -> dict:
@@ -72,13 +72,13 @@
         
     def sample(self, num_samples : int = 1) -> UnweightedSamples:
         return UnweightedSamples([self.__state] * num_samples, _type = self._type)
 
     def __str__(self) -> str:
         return 'ScalarData({})'.format(self.__state)
 
-    def percentage_in_bounds(self, bounds : Union[list, dict]) -> dict:
+    def percentage_in_bounds(self, bounds: Union[list, dict]) -> dict:
         if isinstance(bounds, list):
             bounds = {key: bounds for key in self.keys()}
         if not isinstance(bounds, dict) and all([isinstance(b, list) for b in bounds]):
             raise TypeError("Bounds must be list [lower, upper] or dict (key: [lower, upper]), was {}".format(type(bounds)))
         return {key: (1 if bounds[key][0] < x and bounds[key][1] > x else 0) for (key, x) in self.__state.items()}
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/uncertain_data.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/uncertain_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
 
 class UncertainData(ABC):
     """
     Abstract base class for data with uncertainty. Any new uncertainty type must implement this class
     """
 
-    def __init__(self, _type = dict):
+    def __init__(self, _type=dict):
         self._type = _type
     
     @abstractmethod
-    def sample(self, nSamples : int = 1):
+    def sample(self, nSamples: int = 1):
         """Generate samples from data
 
         Args:
             nSamples (int, optional): Number of samples to generate. Defaults to 1.
 
         Returns:
             samples (UnweightedSamples): Array of nSamples samples
@@ -72,15 +72,15 @@
 
         Example:
             ::
 
                 covariance_matrix = data.cov
         """
 
-    def relative_accuracy(self, ground_truth : dict) -> dict:
+    def relative_accuracy(self, ground_truth: dict) -> dict:
         """The relative accuracy is how close the mean of the distribution is to the ground truth, on relative terms
         
         :math:`RA = 1 - \dfrac{\| r-p \|}{r}`
 
         Where r is ground truth and p is mean of predicted distribution [0]_
 
         Returns:
@@ -113,15 +113,15 @@
                 
                 keys = data.keys()
         """
 
     def __contains__(self, key):
         return key in self.keys()
 
-    def percentage_in_bounds(self, bounds : tuple, keys : list = None, n_samples = 1000) -> dict:
+    def percentage_in_bounds(self, bounds: tuple, keys: list = None, n_samples: int = 1000) -> dict:
         """Calculate percentage of dist is within specified bounds
 
         Args:
             bounds (tuple[float, float] or dict): Lower and upper bounds. \n
                 if tuple: (lower, upper)\n
                 if dict: {key: (lower, upper), ...}
             keys (list[str], optional): UncertainData keys to consider when calculating. Defaults to all keys.
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/uncertain_data/unweighted_samples.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/unweighted_samples.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Args:
         samples (array, dict, or model.*Container, optional): array of samples. Defaults to empty array.\n
             If dict, must be of the form of {key: [value, ...], ...}\n
             If list, must be of the form of [{key: value, ...}, ...]\n
             If InputContainer, OutputContainer, or StateContainer, must be of the form of *Container({'key': value, ...})
     """
-    def __init__(self, samples : list = [], _type = dict):
+    def __init__(self, samples: list = [], _type=dict):
         super().__init__(_type)
         if isinstance(samples, dict) or isinstance(samples, DictLikeMatrixWrapper):
             # Is in form of {key: [value, ...], ...}
             # Convert to array of samples
             if len(samples.keys()) == 0:
                 self.data = []  # is empty
                 return
@@ -35,67 +35,67 @@
             self.data = samples
         else:
             raise ValueError('Invalid input. Must be list or dict, was {}'.format(type(samples)))
 
     def __eq__(self, other):
         return isinstance(other, UnweightedSamples) and self.data == other.data
 
-    def __getitem__(self,n):
+    def __getitem__(self, n):
         datem = self.data[n]
         return self._type(datem) if datem is not None else None
 
-    def __add__(self, other : int) -> "UncertainData":
+    def __add__(self, other: int) -> "UncertainData":
         if other == 0:
             return self
         result = []
         for i in range(len(self.data)):
             new_dict = {}
             for k,v in self.data[i].items():
                 new_dict[k] = v + other
             result.append(new_dict)
         return UnweightedSamples(result)
 
-    def __radd__(self, other : int) -> "UncertainData":
+    def __radd__(self, other: int) -> "UncertainData":
         return self.__add__(other)
 
-    def __iadd__(self, other : int) -> "UncertainData":
+    def __iadd__(self, other: int) -> "UncertainData":
         if other != 0:
             for i in range(len(self.data)):
                 for k,v in self.data[i].items():
                     self.data[i][k] += other
         return self
 
-    def __sub__(self, other : int) -> "UncertainData":
+    def __sub__(self, other: int) -> "UncertainData":
         if other == 0:
             return self
         result = []
         for i in range(len(self.data)):
             new_dict = {}
             for k,v in self.data[i].items():
                 new_dict[k] = v - other
             result.append(new_dict)
         return UnweightedSamples(result)
 
-    def __rsub__(self, other : int) -> "UncertainData":
+    def __rsub__(self, other: int) -> "UncertainData":
         return self.__sub__(other)
 
-    def __isub__(self, other : int) -> "UncertainData":
+    def __isub__(self, other: int) -> "UncertainData":
         if other != 0:
             for i in range(len(self.data)):
                 for k,v in self.data[i].items():
                     self.data[i][k] -= other
         return self
 
     def __reduce__(self):
         return (UnweightedSamples, (self.data, ))
 
-    def sample(self, num_samples : int = 1, replace = True) -> "UnweightedSamples":
+    def sample(self, num_samples: int = 1, replace: bool = True) -> "UnweightedSamples":
         # Completely random resample
-        indices = random.choice(len(self.data), num_samples, replace = replace)
-        return UnweightedSamples([self.data[i] for i in indices], _type = self._type)
+        indices = random.choice(len(self.data), int(num_samples), replace=replace)
+        return UnweightedSamples([self.data[i] for i in indices], _type=self._type)
 
     def keys(self) -> list:
         if len(self.data) == 0:
             return []  # is empty
         for sample in self:
             if sample is not None:
                 return sample.keys()
@@ -159,15 +159,15 @@
         """Get the number of samples. Note: kept for backwards compatibility, prefer using len() instead.
 
         Returns:
             int: Number of samples
         """
         return len(self)
 
-    def percentage_in_bounds(self, bounds, keys : list = None) -> dict:
+    def percentage_in_bounds(self, bounds, keys: list = None) -> dict:
         if not keys:
             keys = self.keys()
         if isinstance(keys, str):
             keys = [keys]
         if isinstance(bounds, list):
             bounds = {key: bounds for key in self.keys()}
         if not isinstance(bounds, dict) or all([isinstance(b, list) and len(b) == 2 for b in bounds]):
```

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/utils/table.py` & `prog_algs-1.5.0rc0/src/prog_algs/utils/table.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/visualize/plot_hist.py` & `prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_hist.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.4.3rc0/src/prog_algs/visualize/plot_scatter.py` & `prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.4.3rc0/src/prog_algs.egg-info/PKG-INFO` & `prog_algs-1.5.0rc0/src/prog_algs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-algs
-Version: 1.4.3rc0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations
 Home-page: https://nasa.github.io/progpy/prog_algs_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_algs/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_algs_guide.html
@@ -21,15 +21,15 @@
 Classifier: License :: Other/Proprietary License 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7, <3.11
+Requires-Python: >=3.7, <3.12
 Description-Content-Type: text/markdown
 
 # Prognostics Algorithm Python Package
 [![CodeFactor](https://www.codefactor.io/repository/github/nasa/prog_algs/badge)](https://www.codefactor.io/repository/github/nasa/prog_algs)
 [![GitHub License](https://img.shields.io/badge/License-NOSA-green)](https://github.com/nasa/prog_algs/blob/master/license.pdf)
 [![GitHub Releases](https://img.shields.io/github/release/nasa/prog_algs.svg)](https://github.com/nasa/prog_algs/releases)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nasa/prog_algs/master?tutorial.ipynb)
@@ -43,40 +43,39 @@
 
 ## Documentation
 See documentation [here](https://nasa.github.io/progpy/prog_algs_guide.html)
 
 ## Repository Directory Structure 
 
 `src/prog_algs/` - The prognostics algorithm python package<br />
-`docs/` - Project documentation (see also [github.io](https://nasa.github.io/prog_algs/))<br />
 `examples/` - Example Python scripts using prog_algs<br />
 `tests/` - Tests for prog_models<br />
 `README.md` - The readme (this file)<br />
 
 ## Citing this repository
 Use the following to cite this repository:
 
 ```
-@misc{2022_nasa_prog_algs,
+@misc{2023_nasa_prog_algs,
     author    = {Christopher Teubert and Matteo Corbetta and Chetan Kulkarni},
     title     = {Prognostics Algorithm Python Package},
-    month     = Dec,
-    year      = 2022,
-    version   = {1.4.3},
+    month     = May,
+    year      = 2023,
+    version   = {1.5},
     url       = {https://github.com/nasa/prog\_algs}
     }
 ```
 
 The corresponding reference should look like this:
 
-C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.4.3, Dec 2022. URL https://github.com/nasa/prog_algs.
+C. Teubert, M. Corbetta, C. Kulkarni, Prognostics Algorithm Python Package, v1.5, May 2023. URL https://github.com/nasa/prog_algs.
 
 Alternatively, if using both prog_models and prog_algs, you can cite the combined package as
 
-C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.4, December 2022. URL https://nasa.github.io/progpy.
+C. Teubert, C. Kulkarni, M. Corbetta, K. Jarvis, M. Daigle, ProgPy Prognostics Python Packages, v1.5, May 2023. URL https://nasa.github.io/progpy.
 
 ## Acknowledgements
 The structure and algorithms of this package are strongly inspired by the [MATLAB Prognostics Algorithm Library](https://github.com/nasa/PrognosticsAlgorithmLibrary) and the [MATLAB Prognostics Metrics Library](https://github.com/nasa/PrognosticsMetricsLibrary). We would like to recognize Matthew Daigle, Shankar Sankararaman and the rest of the team that contributed to the Prognostics Model Library for the contributions their work on the MATLAB library made to the design of prog_algs
 
 ## Notices
 Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
```

