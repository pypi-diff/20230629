# Comparing `tmp/prog_algs-1.5.0.tar.gz` & `tmp/prog_algs-1.5.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prog_algs-1.5.0.tar", last modified: Thu Jun 29 15:12:58 2023, max compression
+gzip compressed data, was "prog_algs-1.5.0rc0.tar", last modified: Thu Jun 29 14:59:55 2023, max compression
```

## Comparing `prog_algs-1.5.0.tar` & `prog_algs-1.5.0rc0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.817492 prog_algs-1.5.0/
--rw-r--r--   0 cteubert   (507) staff       (20)     6663 2023-06-29 15:12:58.817318 prog_algs-1.5.0/PKG-INFO
--rw-r--r--   0 cteubert   (507) staff       (20)     4765 2023-06-23 20:51:30.000000 prog_algs-1.5.0/README.md
--rw-r--r--   0 cteubert   (507) staff       (20)       38 2023-06-29 15:12:58.817527 prog_algs-1.5.0/setup.cfg
--rw-r--r--   0 cteubert   (507) staff       (20)     2678 2023-06-29 15:11:20.000000 prog_algs-1.5.0/setup.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.810011 prog_algs-1.5.0/src/
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.811275 prog_algs-1.5.0/src/prog_algs/
--rw-r--r--   0 cteubert   (507) staff       (20)     1670 2023-06-29 15:11:27.000000 prog_algs-1.5.0/src/prog_algs/__init__.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.812588 prog_algs-1.5.0/src/prog_algs/metrics/
--rw-r--r--   0 cteubert   (507) staff       (20)      507 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/metrics/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1786 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/metrics/samples.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3234 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/metrics/toe_metrics.py
--rw-r--r--   0 cteubert   (507) staff       (20)     8605 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/metrics/toe_profile_metrics.py
--rw-r--r--   0 cteubert   (507) staff       (20)     5401 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/metrics/uncertain_data_metrics.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.813345 prog_algs-1.5.0/src/prog_algs/predictors/
--rw-r--r--   0 cteubert   (507) staff       (20)     1111 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7292 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/monte_carlo.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6985 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/prediction.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3409 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/predictor.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10325 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/toe_prediction_profile.py
--rw-r--r--   0 cteubert   (507) staff       (20)    13679 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/predictors/unscented_transform.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.813973 prog_algs-1.5.0/src/prog_algs/state_estimators/
--rw-r--r--   0 cteubert   (507) staff       (20)      498 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/state_estimators/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7491 2023-06-27 22:08:35.000000 prog_algs-1.5.0/src/prog_algs/state_estimators/kalman_filter.py
--rw-r--r--   0 cteubert   (507) staff       (20)     9336 2023-06-27 22:08:35.000000 prog_algs-1.5.0/src/prog_algs/state_estimators/particle_filter.py
--rw-r--r--   0 cteubert   (507) staff       (20)     4861 2023-06-27 22:08:35.000000 prog_algs-1.5.0/src/prog_algs/state_estimators/state_estimator.py
--rw-r--r--   0 cteubert   (507) staff       (20)     6172 2023-06-27 22:08:35.000000 prog_algs-1.5.0/src/prog_algs/state_estimators/unscented_kalman_filter.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.814583 prog_algs-1.5.0/src/prog_algs/uncertain_data/
--rw-r--r--   0 cteubert   (507) staff       (20)      436 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/uncertain_data/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3401 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/uncertain_data/multivariate_normal_dist.py
--rw-r--r--   0 cteubert   (507) staff       (20)     2923 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/uncertain_data/scalar_data.py
--rw-r--r--   0 cteubert   (507) staff       (20)    10019 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/uncertain_data/uncertain_data.py
--rw-r--r--   0 cteubert   (507) staff       (20)     7214 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/uncertain_data/unweighted_samples.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.814859 prog_algs-1.5.0/src/prog_algs/utils/
--rw-r--r--   0 cteubert   (507) staff       (20)      202 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/utils/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3926 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/utils/table.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.815264 prog_algs-1.5.0/src/prog_algs/visualize/
--rw-r--r--   0 cteubert   (507) staff       (20)      270 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/visualize/__init__.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1948 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/visualize/plot_hist.py
--rw-r--r--   0 cteubert   (507) staff       (20)     3674 2023-06-27 22:08:27.000000 prog_algs-1.5.0/src/prog_algs/visualize/plot_scatter.py
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.811959 prog_algs-1.5.0/src/prog_algs.egg-info/
--rw-------   0 cteubert   (507) staff       (20)     6663 2023-06-29 15:12:58.000000 prog_algs-1.5.0/src/prog_algs.egg-info/PKG-INFO
--rw-------   0 cteubert   (507) staff       (20)     1564 2023-06-29 15:12:58.000000 prog_algs-1.5.0/src/prog_algs.egg-info/SOURCES.txt
--rw-------   0 cteubert   (507) staff       (20)        1 2023-06-29 15:12:58.000000 prog_algs-1.5.0/src/prog_algs.egg-info/dependency_links.txt
--rw-------   0 cteubert   (507) staff       (20)       51 2023-06-29 15:12:58.000000 prog_algs-1.5.0/src/prog_algs.egg-info/requires.txt
--rw-------   0 cteubert   (507) staff       (20)       10 2023-06-29 15:12:58.000000 prog_algs-1.5.0/src/prog_algs.egg-info/top_level.txt
-drwxr-xr-x   0 cteubert   (507) staff       (20)        0 2023-06-29 15:12:58.817084 prog_algs-1.5.0/tests/
--rw-r--r--   0 cteubert   (507) staff       (20)     1750 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_examples.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1230 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_manual.py
--rw-r--r--   0 cteubert   (507) staff       (20)    25519 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_metrics.py
--rw-r--r--   0 cteubert   (507) staff       (20)    17001 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_predictors.py
--rw-r--r--   0 cteubert   (507) staff       (20)    20665 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_state_estimators.py
--rw-r--r--   0 cteubert   (507) staff       (20)      582 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_templates.py
--rw-r--r--   0 cteubert   (507) staff       (20)      743 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_tutorials.py
--rw-r--r--   0 cteubert   (507) staff       (20)    21671 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_uncertain_data.py
--rw-r--r--   0 cteubert   (507) staff       (20)     1693 2023-06-20 20:23:09.000000 prog_algs-1.5.0/tests/test_visualize.py
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

### Comparing `prog_algs-1.5.0/PKG-INFO` & `prog_algs-1.5.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog_algs
-Version: 1.5.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations
 Home-page: https://nasa.github.io/progpy/prog_algs_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_algs/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_algs_guide.html
```

### Comparing `prog_algs-1.5.0/README.md` & `prog_algs-1.5.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/setup.py` & `prog_algs-1.5.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name = 'prog_algs',
-    version = '1.5.0',
+    version = '1.5.0.pre',
     description = "The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url = 'https://nasa.github.io/progpy/prog_algs_guide.html',
     author = 'Christopher Teubert',
     author_email = 'christopher.a.teubert@nasa.gov',
     classifiers = [
```

### Comparing `prog_algs-1.5.0/src/prog_algs/__init__.py` & `prog_algs-1.5.0rc0/src/prog_algs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright © 2021 United States Government as represented by the Administrator of the National Aeronautics and Space Administration.  All Rights Reserved.
 
 __all__ = ['predictors', 'uncertain_data', 'state_estimators', 'run_prog_playback', 'metrics']
 from . import predictors, state_estimators, uncertain_data
 
 import warnings
 
-__version__ = '1.5.0'
+__version__ = '1.5.0.pre'
 
 def run_prog_playback(obs, pred, future_loading, output_measurements, **kwargs):
     warnings.warn("Depreciated in 1.2.0, will be removed in a future release.", DeprecationWarning)
     config = {# Defaults
         'predict_rate': 0, # Default- predict every step
         'num_samples': 10,
         'predict_config': {}
```

### Comparing `prog_algs-1.5.0/src/prog_algs/metrics/samples.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/samples.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/metrics/toe_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_metrics.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/metrics/toe_profile_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/toe_profile_metrics.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/metrics/uncertain_data_metrics.py` & `prog_algs-1.5.0rc0/src/prog_algs/metrics/uncertain_data_metrics.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/__init__.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/monte_carlo.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/monte_carlo.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/prediction.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/prediction.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/predictor.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/predictor.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/toe_prediction_profile.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/toe_prediction_profile.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/predictors/unscented_transform.py` & `prog_algs-1.5.0rc0/src/prog_algs/predictors/unscented_transform.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/state_estimators/kalman_filter.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/state_estimators/particle_filter.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/particle_filter.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/state_estimators/state_estimator.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/state_estimator.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/state_estimators/unscented_kalman_filter.py` & `prog_algs-1.5.0rc0/src/prog_algs/state_estimators/unscented_kalman_filter.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/uncertain_data/multivariate_normal_dist.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/multivariate_normal_dist.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/uncertain_data/scalar_data.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/scalar_data.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/uncertain_data/uncertain_data.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/uncertain_data.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/uncertain_data/unweighted_samples.py` & `prog_algs-1.5.0rc0/src/prog_algs/uncertain_data/unweighted_samples.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/utils/table.py` & `prog_algs-1.5.0rc0/src/prog_algs/utils/table.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/visualize/plot_hist.py` & `prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_hist.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs/visualize/plot_scatter.py` & `prog_algs-1.5.0rc0/src/prog_algs/visualize/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/src/prog_algs.egg-info/PKG-INFO` & `prog_algs-1.5.0rc0/src/prog_algs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prog-algs
-Version: 1.5.0
+Version: 1.5.0rc0
 Summary: The NASA Prognostics Algorithm Package is a framework for model-based prognostics (computation of remaining useful life) of engineering systems. It includes algorithms for state estimation and prediction, including uncertainty propagation. The algorithms use prognostic models (see prog_models) to perform estimation and prediction. The package enables rapid development of prognostics solutions for given models of components and systems. Algorithms can be swapped for comparative studies and evaluations
 Home-page: https://nasa.github.io/progpy/prog_algs_guide.html
 Author: Christopher Teubert
 Author-email: christopher.a.teubert@nasa.gov
 License: NOSA
 Project-URL: Bug Reports, https://github.com/nasa/prog_algs/issues
 Project-URL: Docs, https://nasa.github.io/progpy/prog_algs_guide.html
```

### Comparing `prog_algs-1.5.0/src/prog_algs.egg-info/SOURCES.txt` & `prog_algs-1.5.0rc0/src/prog_algs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_examples.py` & `prog_algs-1.5.0rc0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_manual.py` & `prog_algs-1.5.0rc0/tests/test_manual.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_metrics.py` & `prog_algs-1.5.0rc0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_predictors.py` & `prog_algs-1.5.0rc0/tests/test_predictors.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_state_estimators.py` & `prog_algs-1.5.0rc0/tests/test_state_estimators.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_templates.py` & `prog_algs-1.5.0rc0/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_tutorials.py` & `prog_algs-1.5.0rc0/tests/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_uncertain_data.py` & `prog_algs-1.5.0rc0/tests/test_uncertain_data.py`

 * *Files identical despite different names*

### Comparing `prog_algs-1.5.0/tests/test_visualize.py` & `prog_algs-1.5.0rc0/tests/test_visualize.py`

 * *Files identical despite different names*

