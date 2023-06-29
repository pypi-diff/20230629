# Comparing `tmp/pypesto-0.3.0.tar.gz` & `tmp/pypesto-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypesto-0.3.0.tar", last modified: Tue May  2 14:39:34 2023, max compression
+gzip compressed data, was "pypesto-0.3.1.tar", last modified: Thu Jun 29 09:24:32 2023, max compression
```

## Comparing `pypesto-0.3.0.tar` & `pypesto-0.3.1.tar`

### file list

```diff
@@ -1,186 +1,185 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.698900 pypesto-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-02 14:39:24.000000 pypesto-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 14:39:34.698900 pypesto-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-02 14:39:24.000000 pypesto-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/
--rw-r--r--   0 runner    (1001) docker     (123)     9148 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/C.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/mpi_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/multi_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/multi_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/single_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/engine/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/covariance_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    43151 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/ensemble/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/hierarchical/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/inner_calculator_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27156 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    42311 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/petab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11265 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    27144 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/spline_approximation/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/hierarchical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto/history/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/history/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/objective/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/objective/aesara/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/aesara/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/aesara/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/aggregated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/objective/amici/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/amici/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21961 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/amici/amici.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/amici/amici_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/amici/amici_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/finite_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/objective/jax/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/jax/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/objective/julia/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/julia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/pre_post_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/objective/priors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/optimize/ess/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/cess.py
--rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/function_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/refset.py
--rw-r--r--   0 runner    (1001) docker     (123)    23958 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/ess/sacess.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    41744 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/optimize/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/petab/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31467 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/petab/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/petab/pysb_importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/predict/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/predict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/predict/amici_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/predict/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.690899 pypesto-0.3.0/pypesto/problem/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17970 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/problem/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/approximate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/profile_next_guess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/validation_intervals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/profile/walk_along_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/result/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/result/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/sample/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/adaptive_metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/adaptive_parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/auto_correlation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/dynesty.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/emcee.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/geweke_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/parallel_tempering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/pymc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/sample/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/select/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18700 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/model_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/select/problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/startpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/startpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/startpoint/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/startpoint/latin_hypercube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/startpoint/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/startpoint/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/store/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/store/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/store/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/store/read_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/store/save_to_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.694900 pypesto-0.3.0/pypesto/testing/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/testing/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.698900 pypesto-0.3.0/pypesto/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/clust_color.py
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/dimension_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/model_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/optimization_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/optimizer_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/optimizer_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    32131 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/ordinal_categories.py
--rw-r--r--   0 runner    (1001) docker     (123)    17508 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/profile_cis.py
--rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/reference_points.py
--rw-r--r--   0 runner    (1001) docker     (123)    46051 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/spline_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-02 14:39:24.000000 pypesto-0.3.0/pypesto/visualize/waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:39:34.686900 pypesto-0.3.0/pypesto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-05-02 14:39:34.000000 pypesto-0.3.0/pypesto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 14:39:34.000000 pypesto-0.3.0/pypesto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:39:34.000000 pypesto-0.3.0/pypesto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-02 14:39:34.000000 pypesto-0.3.0/pypesto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 14:39:34.000000 pypesto-0.3.0/pypesto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-02 14:39:24.000000 pypesto-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-02 14:39:34.698900 pypesto-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-02 14:39:24.000000 pypesto-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.283898 pypesto-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-06-29 09:24:15.000000 pypesto-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-29 09:24:32.283898 pypesto-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-29 09:24:15.000000 pypesto-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.267897 pypesto-0.3.1/pypesto/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.267897 pypesto-0.3.1/pypesto/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/mpi_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/multi_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/multi_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/single_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/engine/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.267897 pypesto-0.3.1/pypesto/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/covariance_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42868 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11582 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/ensemble/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/hierarchical/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/inner_calculator_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42771 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17602 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/petab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13025 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15350 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31495 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/spline_approximation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/hierarchical/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/history/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9537 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13740 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/history/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/objective/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.271897 pypesto-0.3.1/pypesto/objective/aesara/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/aesara/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/aesara/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/aggregated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/objective/amici/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/amici/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22221 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/amici/amici.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/amici/amici_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/amici/amici_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24325 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/finite_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/objective/jax/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/jax/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/objective/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/julia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/pre_post_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/objective/priors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/optimize/ess/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/cess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21040 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/function_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/refset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23958 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/ess/sacess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41918 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/optimize/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/petab/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31474 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/petab/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/predict/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/predict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/predict/amici_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/predict/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.275897 pypesto-0.3.1/pypesto/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/problem/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.279898 pypesto-0.3.1/pypesto/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/approximate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/profile_next_guess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5189 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/validation_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/profile/walk_along_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.279898 pypesto-0.3.1/pypesto/result/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12223 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7798 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/result/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.279898 pypesto-0.3.1/pypesto/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/adaptive_metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/adaptive_parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/auto_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/dynesty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/emcee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/geweke_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/parallel_tempering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/pymc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/sample/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.279898 pypesto-0.3.1/pypesto/select/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7117 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/model_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/select/problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.279898 pypesto-0.3.1/pypesto/startpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/startpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/startpoint/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/startpoint/latin_hypercube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/startpoint/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/startpoint/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.283898 pypesto-0.3.1/pypesto/store/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/store/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/store/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/store/read_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/store/save_to_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.283898 pypesto-0.3.1/pypesto/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/testing/examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.283898 pypesto-0.3.1/pypesto/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6832 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/clust_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/dimension_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10333 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/model_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/optimization_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/optimizer_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/optimizer_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32226 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/ordinal_categories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18784 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/profile_cis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/reference_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46051 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11350 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/spline_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-29 09:24:15.000000 pypesto-0.3.1/pypesto/visualize/waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 09:24:32.267897 pypesto-0.3.1/pypesto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4599 2023-06-29 09:24:31.000000 pypesto-0.3.1/pypesto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-29 09:24:32.000000 pypesto-0.3.1/pypesto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 09:24:31.000000 pypesto-0.3.1/pypesto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 09:24:31.000000 pypesto-0.3.1/pypesto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 09:24:31.000000 pypesto-0.3.1/pypesto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-29 09:24:15.000000 pypesto-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-29 09:24:32.283898 pypesto-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-29 09:24:15.000000 pypesto-0.3.1/setup.py
```

### Comparing `pypesto-0.3.0/LICENSE` & `pypesto-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/PKG-INFO` & `pypesto-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.3.0
+Version: 0.3.1
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 Maintainer: Yannik Schaelte, Jakob Vanhoefer, Paul Jost
 Maintainer-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de,paul.jost@uni-bonn.de
 License: BSD-3-Clause
@@ -42,15 +42,14 @@
 Provides-Extra: dynesty
 Provides-Extra: mltools
 Provides-Extra: julia
 Provides-Extra: doc
 Provides-Extra: example
 Provides-Extra: select
 Provides-Extra: test
-Provides-Extra: test_petab
 License-File: LICENSE
 
 # pyPESTO - Parameter EStimation TOolbox for python
 
 <img src="https://raw.githubusercontent.com/ICB-DCM/pyPESTO/master/doc/logo/logo_wordmark.png" width="50%" alt="pyPESTO logo"/>
 
 **pyPESTO** is a widely applicable and highly customizable toolbox for
```

### Comparing `pypesto-0.3.0/README.md` & `pypesto-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/C.py` & `pypesto-0.3.1/pypesto/C.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,14 +191,25 @@
 
 SPLINE_RATIO = 'spline_ratio'
 MIN_DIFF_FACTOR = 'min_diff_factor'
 SPLINE_APPROXIMATION_OPTIONS = [SPLINE_RATIO, MIN_DIFF_FACTOR]
 
 MIN_SIM_RANGE = 1e-16
 
+SPLINE_PAR_TYPE = 'spline'
+N_SPLINE_PARS = 'n_spline_pars'
+DATAPOINTS = 'datapoints'
+MIN_DATAPOINT = 'min_datapoint'
+MAX_DATAPOINT = 'max_datapoint'
+EXPDATA_MASK = 'expdata_mask'
+CURRENT_SIMULATION = 'current_simulation'
+INNER_NOISE_PARS = 'inner_noise_pars'
+OPTIMIZE_NOISE = 'optimize_noise'
+
+
 ###############################################################################
 # HISTORY
 
 HISTORY = "history"
 TRACE = "trace"
 N_ITERATIONS = "n_iterations"
 MESSAGES = "messages"
@@ -206,23 +217,14 @@
 EXITFLAG = "exitflag"
 TRACE_SAVE_ITER = "trace_save_iter"
 
 SUFFIXES_CSV = ["csv"]
 SUFFIXES_HDF5 = ["hdf5", "h5"]
 SUFFIXES = SUFFIXES_CSV + SUFFIXES_HDF5
 
-SPLINE_PAR_TYPE = 'spline'
-N_SPLINE_PARS = 'n_spline_pars'
-DATAPOINTS = 'datapoints'
-MIN_DATAPOINT = 'min_datapoint'
-MAX_DATAPOINT = 'max_datapoint'
-EXPDATA_MASK = 'expdata_mask'
-CURRENT_SIMULATION = 'current_simulation'
-NOISE_PARAMETERS = 'noise_parameters'
-
 
 ###############################################################################
 # PRIOR
 
 LIN = 'lin'  # linear
 LOG = 'log'  # logarithmic to basis e
 LOG10 = 'log10'  # logarithmic to basis 10
```

### Comparing `pypesto-0.3.0/pypesto/__init__.py` & `pypesto-0.3.1/pypesto/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/engine/base.py` & `pypesto-0.3.1/pypesto/engine/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/engine/mpi_pool.py` & `pypesto-0.3.1/pypesto/engine/mpi_pool.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/engine/multi_process.py` & `pypesto-0.3.1/pypesto/engine/multi_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/engine/multi_thread.py` & `pypesto-0.3.1/pypesto/engine/multi_thread.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/engine/single_core.py` & `pypesto-0.3.1/pypesto/engine/single_core.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/ensemble/__init__.py` & `pypesto-0.3.1/pypesto/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/ensemble/covariance_analysis.py` & `pypesto-0.3.1/pypesto/ensemble/covariance_analysis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/ensemble/dimension_reduction.py` & `pypesto-0.3.1/pypesto/ensemble/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/ensemble/ensemble.py` & `pypesto-0.3.1/pypesto/ensemble/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1107,37 +1107,33 @@
         A list of number of candidates per start that are to
         be included in the ensemble.
     """
     # choose possible candidates
     ens_ind = [np.flatnonzero(fval <= cutoff) for fval in fval_traces]
 
     # count the number of candidates per start
-    n_per_start = np.array([len(start) for start in ens_ind])
-
-    # if all possible indices can be included, return
-    if (n_per_start < max_per_start).all() and sum(n_per_start) < max_size:
-        return n_per_start
+    n_theo = np.array([len(start) for start in ens_ind])
 
     # trimm down starts that exceed the limit:
-    n_per_start = [min(n, max_per_start) for n in n_per_start]
+    n_per_start = [min(n, max_per_start) for n in n_theo]
 
-    # trimm down more until it fits the max size
-    decr = 0
-    while sum(n_per_start) > max_size:
-        n_per_start = [min(n, max_per_start - decr) for n in n_per_start]
-        decr += 1
-    # TODO: Possibility. With this implementation we could
-    #  in a scenario, where we have more candidates than
-    #  max size end up with an ensemble of size
-    #  `max_size - len(n_starts)` in the worst case. We could introduce
-    #  a flag which would be `force_max`, that indicates
-    #  whether those remaining free slots should be filled by
-    #  entries from certain starts. This would brng up the
-    #  discussion which starts to choose. One obvious choice
-    #  would be the best starts based on their endpoint.
+    # if all possible indices can be included, return
+    if sum(n_per_start) < max_size:
+        return n_per_start
+    n_equally = max_size // len(n_per_start)
+    n_left = max_size % len(n_per_start)
+    # divide numbers equally
+    n_per_start = [min(n, n_equally) for n in n_per_start]
+    # add one more to the first n_left possible (where n_theo > n_equally):
+    to_add = np.where(n_theo > n_equally)[0]
+    if len(to_add) > n_left:
+        to_add = to_add[0:n_left]
+    n_per_start = [
+        n + 1 if i in to_add else n for i, n in enumerate(n_per_start)
+    ]
 
     return n_per_start
 
 
 def get_vector_indices(
     trace_start: np.ndarray,
     cutoff: float,
@@ -1167,15 +1163,15 @@
     """
     candidates = np.flatnonzero(trace_start <= cutoff)
 
     if distribute:
         indices = np.round(np.linspace(0, len(candidates) - 1, n_vectors))
         return candidates[indices.astype(int)]
     else:
-        return candidates[:n_vectors]
+        return sorted(candidates, key=lambda i: trace_start[i])[:n_vectors]
 
 
 def get_percentile_label(percentile: Union[float, int, str]) -> str:
     """Convert a percentile to a label.
 
     Labels for percentiles are used at different locations (e.g. ensemble
     prediction code, and visualization code). This method ensures that the same
```

### Comparing `pypesto-0.3.0/pypesto/ensemble/task.py` & `pypesto-0.3.1/pypesto/ensemble/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/ensemble/util.py` & `pypesto-0.3.1/pypesto/ensemble/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/calculator.py` & `pypesto-0.3.1/pypesto/hierarchical/calculator.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         self.inner_solver = inner_solver
 
     def initialize(self):
         """Initialize."""
         super().initialize()
         self.inner_solver.initialize()
 
+    def get_inner_parameter_ids(self) -> List[str]:
+        """Get the ids of the inner parameters."""
+        return self.inner_problem.get_x_ids()
+
     def __call__(
         self,
         x_dct: Dict,
         sensi_orders: Tuple[int],
         mode: ModeType,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/inner_calculator_collector.py` & `pypesto-0.3.1/pypesto/hierarchical/inner_calculator_collector.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     AMICI_SSIGMAZ,
     AMICI_SY,
     AMICI_Y,
     CENSORED,
     FVAL,
     GRAD,
     HESS,
+    INNER_PARAMETERS,
     MEASUREMENT_TYPE,
     METHOD,
     MODE_RES,
     NONLINEAR_MONOTONE,
     OPTIMAL_SCALING_OPTIONS,
     ORDINAL,
     RDATAS,
@@ -104,25 +105,28 @@
             petab_problem, model.getObservableIds(), edatas
         )
 
         self._known_least_squares_safe = False
 
     def initialize(self):
         """Initialize."""
+        self.best_fval = np.inf
         for calculator in self.inner_calculators:
             calculator.initialize()
 
     def construct_inner_calculators(
         self,
         petab_problem: 'petab.Problem',
         model: AmiciModel,
         edatas: List['amici.ExpData'],
         inner_options: Dict,
     ):
         """Construct inner calculators for each data type."""
+        self.noise_dummy_values = {}
+        self.best_fval = np.inf
         if ORDINAL in self.data_types or CENSORED in self.data_types:
             optimal_scaling_inner_options = {
                 key: value
                 for key, value in inner_options.items()
                 if key in OPTIMAL_SCALING_OPTIONS
             }
             inner_problem_method = optimal_scaling_inner_options.get(
@@ -151,14 +155,17 @@
             )
             spline_inner_solver = SplineInnerSolver(
                 options=spline_inner_options
             )
             spline_calculator = SplineAmiciCalculator(
                 spline_inner_problem, spline_inner_solver
             )
+            self.noise_dummy_values = (
+                spline_inner_problem.get_noise_dummy_values(scaled=True)
+            )
             self.inner_calculators.append(spline_calculator)
         # TODO relative data
 
         if set(self.data_types) - {ORDINAL, CENSORED, NONLINEAR_MONOTONE}:
             unsupported_data_types = set(self.data_types) - {
                 ORDINAL,
                 CENSORED,
@@ -212,14 +219,22 @@
 
         # If there is no quantitative data, return None
         if not all(mask.any() for mask in quantitative_data_mask):
             return None
 
         return quantitative_data_mask
 
+    def get_inner_parameter_ids(self) -> List[str]:
+        """Return the ids of the inner parameters."""
+        return [
+            parameter_id
+            for inner_calculator in self.inner_calculators
+            for parameter_id in inner_calculator.get_inner_parameter_ids()
+        ]
+
     def __call__(
         self,
         x_dct: Dict,
         sensi_orders: Tuple[int],
         mode: ModeType,
         amici_model: AmiciModel,
         amici_solver: AmiciSolver,
@@ -273,25 +288,26 @@
         # get dimension of outer problem
         dim = len(x_ids)
 
         # initialize return values
         nllh, snllh, s2nllh, chi2, res, sres = init_return_values(
             sensi_orders, mode, dim
         )
-        inner_parameters_dictionary = {}
+        all_inner_pars = {}
+        interpretable_inner_pars = {}
 
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
         amici_solver.setSensitivityOrder(sensi_order)
 
         x_dct = copy.deepcopy(x_dct)
-
+        x_dct.update(self.noise_dummy_values)
         # fill in parameters
         amici.parameter_mapping.fill_in_parameters(
             edatas=edatas,
             problem_parameters=x_dct,
             scaled_parameters=True,
             parameter_mapping=parameter_mapping,
             amici_model=amici_model,
@@ -311,15 +327,16 @@
             ret = {
                 FVAL: nllh,
                 GRAD: snllh,
                 HESS: s2nllh,
                 RES: res,
                 SRES: sres,
                 RDATAS: rdatas,
-                X_INNER_OPT: inner_parameters_dictionary,
+                X_INNER_OPT: all_inner_pars,
+                INNER_PARAMETERS: interpretable_inner_pars,
             }
             ret[FVAL] = np.inf
             # if the gradient was requested,
             # we need to provide some value for it
             if 1 in sensi_orders:
                 ret[GRAD] = np.full(shape=len(x_ids), fill_value=np.nan)
             return filter_return_dict(ret)
@@ -361,15 +378,18 @@
                 parameter_mapping=parameter_mapping,
                 fim_for_hess=fim_for_hess,
                 rdatas=rdatas,
             )
             nllh += inner_result[FVAL]
             if sensi_order > 0:
                 snllh += inner_result[GRAD]
-            inner_parameters_dictionary.update(inner_result[X_INNER_OPT])
+
+            all_inner_pars.update(inner_result[X_INNER_OPT])
+            if INNER_PARAMETERS in inner_result:
+                interpretable_inner_pars.update(inner_result[INNER_PARAMETERS])
 
         # add result for quantitative data
         if self.quantitative_data_mask is not None:
             quantitative_result = calculate_quantitative_result(
                 rdatas=rdatas,
                 sensi_orders=sensi_orders,
                 edatas=edatas,
@@ -388,17 +408,23 @@
         ret = {
             FVAL: nllh,
             GRAD: snllh,
             HESS: s2nllh,
             RES: res,
             SRES: sres,
             RDATAS: rdatas,
-            X_INNER_OPT: inner_parameters_dictionary,
         }
 
+        # Add inner parameters to return dict
+        # only if the objective value improved.
+        if ret[FVAL] < self.best_fval:
+            ret[X_INNER_OPT] = all_inner_pars
+            ret[INNER_PARAMETERS] = interpretable_inner_pars
+            self.best_fval = ret[FVAL]
+
         return filter_return_dict(ret)
 
 
 def calculate_quantitative_result(
     rdatas: List[amici.ReturnDataView],
     edatas: List[amici.ExpData],
     sensi_orders: Tuple[int],
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/__init__.py` & `pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/calculator.py` & `pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,19 @@
             raise ValueError(
                 f"The inner problem method {self.inner_problem.method} and the inner solver method {self.inner_solver.options['method']} have to coincide."
             )
 
     def initialize(self):
         """Initialize."""
         self.inner_solver.initialize()
+        self.inner_problem.initialize()
+
+    def get_inner_parameter_ids(self) -> List[str]:
+        """Get the ids of the inner parameters."""
+        return self.inner_problem.get_x_ids()
 
     def __call__(
         self,
         x_dct: Dict,
         sensi_orders: Tuple[int, ...],
         mode: str,
         amici_model: AmiciModel,
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/parameter.py` & `pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,7 +81,11 @@
 
         self.observable_id = observable_id
         self.category = category
         self.group = group
         self.estimate = estimate
         self.value = self.dummy_value
         self.censoring_type = censoring_type
+
+    def initialize(self):
+        """Initialize."""
+        self.value = self.dummy_value
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/problem.py` & `pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,26 @@
                 self.groups[group][W_DOT_MATRIX] = self.initialize_w(group)
             else:
                 raise ValueError(
                     'Censoring types of optimal scaling parameters of a group '
                     'have to either be all None, or all not None.'
                 )
 
+    def initialize(self) -> None:
+        """Initialize the subproblem."""
+        # Initialize all parameter values.
+        for x in self.xs.values():
+            x.initialize()
+
+        # Initialize the groups.
+        for group in self.get_groups_for_xs(InnerParameterType.SPLINE):
+            self.groups[group][SURROGATE_DATA] = np.zeros(
+                self.groups[group][NUM_DATAPOINTS]
+            )
+
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
         amici_model: 'amici.Model',
         edatas: List['amici.ExpData'],
         method: str = None,
     ) -> 'OptimalScalingProblem':
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/optimal_scaling/solver.py` & `pypesto-0.3.1/pypesto/hierarchical/optimal_scaling/solver.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,24 @@
             # Iterate over outer optimization parameters.
             for par_sim, par_opt in condition_map_sim_var.items():
                 if (
                     not isinstance(par_opt, str)
                     or par_opt in already_calculated
                 ):
                     continue
+                # Current fix for scaling/offset parameters in models.
+                elif par_sim.startswith('observableParameter'):
+                    continue
+                # For noise parameters optimized hierarchically, we
+                # do not calculate the gradient.
+                elif (
+                    par_sim.startswith('noiseParameter')
+                    and par_opt not in par_opt_ids
+                ):
+                    continue
                 else:
                     already_calculated.add(par_opt)
 
                 par_opt_idx = par_opt_ids.index(par_opt)
                 par_sim_idx = par_sim_ids.index(par_sim)
                 par_edata_idx = [
                     par_edata_indices.index(par_sim_idx)
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/parameter.py` & `pypesto-0.3.1/pypesto/hierarchical/parameter.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/petab.py` & `pypesto-0.3.1/pypesto/hierarchical/petab.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/problem.py` & `pypesto-0.3.1/pypesto/hierarchical/problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/solver.py` & `pypesto-0.3.1/pypesto/hierarchical/solver.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/spline_approximation/__init__.py` & `pypesto-0.3.1/pypesto/hierarchical/spline_approximation/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/hierarchical/spline_approximation/calculator.py` & `pypesto-0.3.1/pypesto/hierarchical/spline_approximation/calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import copy
 from typing import Dict, List, Sequence, Tuple
 
 import numpy as np
 
 from ...C import (
     AMICI_SIGMAY,
+    AMICI_SSIGMAY,
     AMICI_SY,
     AMICI_Y,
     FVAL,
     GRAD,
     HESS,
+    INNER_PARAMETERS,
     MODE_RES,
     RDATAS,
     RES,
     SRES,
     X_INNER_OPT,
 )
 from ...objective.amici.amici_calculator import (
@@ -63,14 +65,19 @@
         if inner_solver is None:
             inner_solver = SplineInnerSolver()
         self.inner_solver = inner_solver
 
     def initialize(self):
         """Initialize."""
         self.inner_solver.initialize()
+        self.inner_problem.initialize()
+
+    def get_inner_parameter_ids(self) -> List[str]:
+        """Get the ids of the inner parameters."""
+        return self.inner_problem.get_x_ids()
 
     def __call__(
         self,
         x_dct: Dict,
         sensi_orders: Tuple[int, ...],
         mode: str,
         amici_model: AmiciModel,
@@ -103,15 +110,15 @@
         x_ids:
             Ids of optimization parameters.
         parameter_mapping:
             Mapping of optimization to simulation parameters.
         fim_for_hess:
             Whether to use the FIM (if available) instead of the Hessian (if
             requested).
-        inner_rdatas:
+        rdatas:
             AMICI simulation return data. In case the calculator is part of
             the :class:`pypesto.objective.amici.InnerCalculatorCollector`,
             it will already simulate the model and pass the results here.
 
 
         Returns
         -------
@@ -136,18 +143,22 @@
         )
         # set order in solver
         sensi_order = 0
         if sensi_orders:
             sensi_order = max(sensi_orders)
 
         # If AMICI ReturnData is not provided, we need to simulate the model
+
         if rdatas is None:
             amici_solver.setSensitivityOrder(sensi_order)
 
             x_dct = copy.deepcopy(x_dct)
+            x_dct.update(
+                self.inner_problem.get_noise_dummy_values(scaled=True)
+            )
 
             # fill in parameters
             amici.parameter_mapping.fill_in_parameters(
                 edatas=edatas,
                 problem_parameters=x_dct,
                 scaled_parameters=True,
                 parameter_mapping=parameter_mapping,
@@ -195,23 +206,29 @@
         inner_result[FVAL] = self.inner_solver.calculate_obj_function(
             x_inner_opt
         )
         inner_result[
             X_INNER_OPT
         ] = self.inner_problem.get_inner_parameter_dictionary()
 
+        inner_result[
+            INNER_PARAMETERS
+        ] = self.inner_problem.get_inner_noise_parameter_dictionary()
+
         # Calculate analytical gradients if requested
         if sensi_order > 0:
             sy = [rdata[AMICI_SY] for rdata in rdatas]
+            ssigma = [rdata[AMICI_SSIGMAY] for rdata in rdatas]
             inner_result[GRAD] = self.inner_solver.calculate_gradients(
                 problem=self.inner_problem,
                 x_inner_opt=x_inner_opt,
                 sim=sim,
-                sigma=sigma,
+                amici_sigma=sigma,
                 sy=sy,
+                amici_ssigma=ssigma,
                 parameter_mapping=parameter_mapping,
                 par_opt_ids=x_ids,
                 par_sim_ids=amici_model.getParameterIds(),
                 snllh=snllh,
             )
 
         return filter_return_dict(inner_result)
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/spline_approximation/parameter.py` & `pypesto-0.3.1/pypesto/hierarchical/spline_approximation/parameter.py`

 * *Files 19% similar despite different names*

```diff
@@ -36,24 +36,36 @@
         """Construct.
 
         Parameters
         ----------
         See class attributes.
         """
         super().__init__(*args, **kwargs)
-        if self.inner_parameter_type != InnerParameterType.SPLINE:
+        if self.inner_parameter_type not in [
+            InnerParameterType.SPLINE,
+            InnerParameterType.SIGMA,
+        ]:
             raise ValueError(
-                "For the SplineParameter class, the parameter type has to be spline."
+                "For the SplineParameter class, the parameter type has to be spline or sigma."
             )
 
         if observable_id is None:
             raise ValueError("No observable id provided.")
         if group is None:
             raise ValueError("No Parameter group provided.")
-        if index is None:
-            raise ValueError("No Parameter index provided.")
+        if (
+            index is None
+            and self.inner_parameter_type == InnerParameterType.SPLINE
+        ):
+            raise ValueError(
+                "No Parameter index provided for spline parameter."
+            )
 
         self.observable_id = observable_id
         self.group = group
         self.index = index
         self.estimate = estimate
         self.value = self.dummy_value
+
+    def initialize(self):
+        """Initialize."""
+        self.value = self.dummy_value
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/spline_approximation/problem.py` & `pypesto-0.3.1/pypesto/hierarchical/spline_approximation/problem.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,38 +3,48 @@
 import numpy as np
 import pandas as pd
 
 from ...C import (
     CURRENT_SIMULATION,
     DATAPOINTS,
     EXPDATA_MASK,
+    INNER_NOISE_PARS,
     INNER_PARAMETER_BOUNDS,
     LIN,
     MAX_DATAPOINT,
     MEASUREMENT_TYPE,
     MIN_DATAPOINT,
     N_SPLINE_PARS,
-    NOISE_PARAMETERS,
     NONLINEAR_MONOTONE,
     NUM_DATAPOINTS,
+    OPTIMIZE_NOISE,
+    PARAMETER_TYPE,
     SPLINE_PAR_TYPE,
     TIME,
     InnerParameterType,
 )
 from ..problem import (
     InnerProblem,
     _get_timepoints_with_replicates,
     ix_matrices_from_arrays,
+    scale_value,
 )
 from .parameter import SplineInnerParameter
 
 try:
     import amici
     import petab
-    from petab.C import OBSERVABLE_ID
+    from petab.C import (
+        ESTIMATE,
+        LOWER_BOUND,
+        NOISE_PARAMETERS,
+        OBSERVABLE_ID,
+        PARAMETER_ID,
+        UPPER_BOUND,
+    )
 except ImportError:
     pass
 
 
 class SplineInnerProblem(InnerProblem):
     """Inner optimization problem for spline approximation.
 
@@ -86,17 +96,31 @@
                 self.groups[group][DATAPOINTS]
             )
 
             self.groups[group][EXPDATA_MASK] = xs[0].ixs
             self.groups[group][CURRENT_SIMULATION] = np.zeros(
                 self.groups[group][NUM_DATAPOINTS]
             )
-            self.groups[group][NOISE_PARAMETERS] = np.zeros(
+            self.groups[group][INNER_NOISE_PARS] = 1
+            self.groups[group][OPTIMIZE_NOISE] = (
+                len(self.get_noise_parameters_for_group(group)) > 0
+            )
+
+    def initialize(self) -> None:
+        """Initialize the subproblem."""
+        # Initialize all parameter values.
+        for x in self.xs.values():
+            x.initialize()
+
+        # Initialize the groups.
+        for group in self.get_groups_for_xs(InnerParameterType.SPLINE):
+            self.groups[group][CURRENT_SIMULATION] = np.zeros(
                 self.groups[group][NUM_DATAPOINTS]
             )
+            self.groups[group][INNER_NOISE_PARS] = 1
 
     @staticmethod
     def from_petab_amici(
         petab_problem: petab.Problem,
         amici_model: 'amici.Model',
         edatas: List['amici.ExpData'],
         spline_ratio: float = None,
@@ -111,52 +135,87 @@
     def get_groups_for_xs(self, inner_parameter_type: str) -> List[int]:
         """Get unique list of ``SplineParameter.group`` values."""
         groups = [x.group for x in self.get_xs_for_type(inner_parameter_type)]
         return list(set(groups))
 
     def get_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that belong to the given group."""
-        return [x for x in self.xs.values() if x.group == group]
+        return [
+            x
+            for x in self.xs.values()
+            if x.group == group
+            and x.inner_parameter_type == InnerParameterType.SPLINE
+        ]
 
     def get_free_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that are free and belong to the given group."""
         return [
             x
             for x in self.xs.values()
-            if x.group == group and x.estimate is True
+            if x.group == group
+            and x.estimate is True
+            and x.inner_parameter_type == InnerParameterType.SPLINE
         ]
 
     def get_fixed_xs_for_group(self, group: int) -> List[SplineInnerParameter]:
         r"""Get ``SplineParameter``\s that are fixed and belong to the given group."""
         return [
             x
             for x in self.xs.values()
-            if x.group == group and x.estimate is False
+            if x.group == group
+            and x.estimate is False
+            and x.inner_parameter_type == InnerParameterType.SPLINE
+        ]
+
+    def get_noise_parameters_for_group(
+        self, group: int
+    ) -> SplineInnerParameter:
+        r"""Get the ``SplineParameter``\ that is a noise parameters and belongs to the given group."""
+        return [
+            x
+            for x in self.xs.values()
+            if x.group == group
+            and x.inner_parameter_type == InnerParameterType.SIGMA
         ]
 
     def get_inner_parameter_dictionary(self) -> Dict:
         """Get a dictionary with all inner parameter ids and their values."""
         inner_par_dict = {}
         for x_id, x in self.xs.items():
             inner_par_dict[x_id] = x.value
         return inner_par_dict
 
+    def get_inner_noise_parameter_dictionary(self) -> Dict:
+        """Get a dictionary with all noise inner parameter ids and their values."""
+        inner_par_dict = {}
+        for x in self.get_xs_for_type(InnerParameterType.SIGMA):
+            inner_par_dict[x.inner_parameter_id] = x.value
+        return inner_par_dict
+
     def get_measurements_for_group(self, gr) -> np.ndarray:
         """Get measurements for a group."""
         # Taking the ixs of first inner parameter since
         # all of them are the same for the same group.
         ixs = self.get_xs_for_group(gr)[0].ixs
 
         return np.concatenate(
             [
                 self.data[condition_index][ixs[condition_index]]
                 for condition_index in range(len(ixs))
             ]
         )
 
+    def get_noise_dummy_values(self, scaled: bool) -> Dict[str, float]:
+        """Get dummy values for noise parameters of the nonlinear-monotone observable."""
+        return {
+            x_id: scale_value(x.value, x.scale) if scaled else x.value
+            for x_id, x in self.xs.items()
+            if x.inner_parameter_type == InnerParameterType.SIGMA
+        }
+
 
 def get_default_options() -> Dict:
     """Return the default spline problem options dictionary."""
     spline_ratio = 1 / 2
     return spline_ratio
 
 
@@ -173,14 +232,20 @@
         raise ValueError("Spline ratio must be a positive float.")
 
     # inner parameters
     inner_parameters = spline_inner_parameters_from_measurement_df(
         petab_problem.measurement_df, spline_ratio, amici_model
     )
 
+    # noise parameters for nonlinear-monotone observables
+    noise_parameters = noise_inner_parameters_from_parameter_df(
+        petab_problem, amici_model
+    )
+    inner_parameters.extend(noise_parameters)
+
     # used indices for all measurement specific parameters
     ixs = spline_ixs_for_measurement_specific_parameters(
         petab_problem, amici_model, inner_parameters
     )
 
     # transform experimental data
     edatas = [
@@ -202,15 +267,15 @@
 
 
 def spline_inner_parameters_from_measurement_df(
     df: pd.DataFrame,
     spline_ratio: float,
     amici_model: 'amici.Model',
 ) -> List[SplineInnerParameter]:
-    """Create list of inner free parameters from PEtab measurement table."""
+    """Create list of inner free spline parameters from PEtab measurement table."""
     df = df.reset_index()
 
     observable_ids = amici_model.getObservableIds()
 
     par_type = SPLINE_PAR_TYPE
     estimate = True
     lb, ub = INNER_PARAMETER_BOUNDS[InnerParameterType.SPLINE].values()
@@ -245,14 +310,64 @@
             )
 
     inner_parameters.sort(key=lambda x: (x.group, x.index))
 
     return inner_parameters
 
 
+def noise_inner_parameters_from_parameter_df(
+    petab_problem: 'petab.Problem',
+    amici_model: 'amici.Model',
+) -> List[SplineInnerParameter]:
+    """Create list of inner free noise parameters from PEtab parameter table."""
+    # Select the nonlinear monotone measurements.
+    measurement_df = petab_problem.measurement_df
+    measurement_df = measurement_df[
+        measurement_df[MEASUREMENT_TYPE] == NONLINEAR_MONOTONE
+    ]
+
+    observable_ids = amici_model.getObservableIds()
+
+    # Create a dictionary with unique pairs of observable id
+    # and noise parameter from the measurement table.
+    noise_parameter_to_observable = {}
+    for _, row in measurement_df.iterrows():
+        observable_id = row[OBSERVABLE_ID]
+        noise_parameter_id = row[NOISE_PARAMETERS]
+        noise_parameter_to_observable[noise_parameter_id] = observable_id
+
+    noise_parameters = []
+
+    parameter_df = petab_problem.parameter_df.reset_index()
+    # Create noise inner parameters.
+    for _, row in parameter_df.iterrows():
+        if row[PARAMETER_ID] not in noise_parameter_to_observable:
+            continue
+        if petab.is_empty(row.get(PARAMETER_TYPE)) or not row[ESTIMATE]:
+            continue
+        observable_id = noise_parameter_to_observable[row[PARAMETER_ID]]
+        group = observable_ids.index(observable_id) + 1
+
+        noise_parameters.append(
+            SplineInnerParameter(
+                inner_parameter_id=row[PARAMETER_ID],
+                inner_parameter_type=InnerParameterType.SIGMA,
+                scale=LIN,
+                lb=row[LOWER_BOUND],
+                ub=row[UPPER_BOUND],
+                observable_id=observable_id,
+                group=group,
+                index=None,
+                estimate=True,
+            )
+        )
+
+    return noise_parameters
+
+
 def spline_ixs_for_measurement_specific_parameters(
     petab_problem: 'petab.Problem',
     amici_model: 'amici.Model',
     inner_parameters: List[SplineInnerParameter],
 ) -> Dict[str, List[Tuple[int, int, int]]]:
     """Create mapping of parameters to measurements.
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/spline_approximation/solver.py` & `pypesto-0.3.1/pypesto/hierarchical/spline_approximation/solver.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import numpy as np
 from scipy.optimize import minimize
 
 from ...C import (
     CURRENT_SIMULATION,
     DATAPOINTS,
     EXPDATA_MASK,
+    INNER_NOISE_PARS,
     MAX_DATAPOINT,
     MIN_DATAPOINT,
     MIN_DIFF_FACTOR,
     MIN_SIM_RANGE,
     N_SPLINE_PARS,
-    NOISE_PARAMETERS,
     NUM_DATAPOINTS,
+    OPTIMIZE_NOISE,
     SCIPY_FUN,
     SCIPY_SUCCESS,
     SCIPY_X,
     InnerParameterType,
 )
 from ..solver import InnerSolver
 from .parameter import SplineInnerParameter
@@ -58,53 +59,70 @@
             if key not in self.get_default_options():
                 raise ValueError(f"Unknown SplineInnerSolver option {key}.")
 
     def solve(
         self,
         problem: SplineInnerProblem,
         sim: List[np.ndarray],
-        sigma: List[np.ndarray],
+        amici_sigma: List[np.ndarray],
     ) -> list:
         """Get results for every group (inner optimization problem).
 
         Parameters
         ----------
         problem:
             InnerProblem from pyPESTO hierarchical.
         sim:
             Simulations from AMICI.
-        sigma:
+        amici_sigma:
             List of sigmas from AMICI.
 
         Returns
         -------
         List of optimization results of the inner subproblem.
         """
-        inner_optimization_results = []
+        inner_results = []
         for group in problem.get_groups_for_xs(InnerParameterType.SPLINE):
             group_dict = problem.groups[group]
-            group_dict[NOISE_PARAMETERS] = extract_expdata_using_mask(
-                expdata=sigma, mask=group_dict[EXPDATA_MASK]
-            )
             group_dict[CURRENT_SIMULATION] = extract_expdata_using_mask(
                 expdata=sim, mask=group_dict[EXPDATA_MASK]
             )
-
-            inner_optimization_results_per_group = self._optimize_spline(
+            # Optimize the spline for this group.
+            inner_result_for_group = self._optimize_spline(
                 inner_parameters=problem.get_free_xs_for_group(group),
                 group_dict=group_dict,
             )
-            inner_optimization_results.append(
-                inner_optimization_results_per_group
+
+            # If the parameters are optimized in the inner problem, we
+            # calculate the sigma analytically from the inner result.
+            if group_dict[OPTIMIZE_NOISE]:
+                group_dict[INNER_NOISE_PARS] = _calculate_sigma_for_group(
+                    inner_result=inner_result_for_group,
+                    n_datapoints=group_dict[NUM_DATAPOINTS],
+                )
+            # Otherwise, we extract the sigma from the AMICI noise parameters.
+            else:
+                group_dict[INNER_NOISE_PARS] = extract_expdata_using_mask(
+                    expdata=amici_sigma, mask=group_dict[EXPDATA_MASK]
+                )[0]
+
+            # Apply sigma to inner result.
+            inner_result_for_group = _calculate_nllh_for_group(
+                inner_result=inner_result_for_group,
+                sigma=group_dict[INNER_NOISE_PARS],
+                n_datapoints=group_dict[NUM_DATAPOINTS],
             )
+
+            inner_results.append(inner_result_for_group)
             save_inner_parameters_to_inner_problem(
-                inner_parameters=problem.get_xs_for_group(group),
-                s=inner_optimization_results_per_group[SCIPY_X],
+                inner_problem=problem,
+                s=inner_result_for_group[SCIPY_X],
+                group=group,
             )
-        return inner_optimization_results
+        return inner_results
 
     @staticmethod
     def calculate_obj_function(x_inner_opt: list):
         """Calculate the inner objective function value.
 
         Calculates the inner objective function value from a list of inner
         optimization results returned from `_optimize_spline`.
@@ -133,16 +151,17 @@
         return obj
 
     def calculate_gradients(
         self,
         problem: SplineInnerProblem,
         x_inner_opt: List[Dict],
         sim: List[np.ndarray],
-        sigma: List[np.ndarray],
+        amici_sigma: List[np.ndarray],
         sy: List[np.ndarray],
+        amici_ssigma: List[np.ndarray],
         parameter_mapping: ParameterMapping,
         par_opt_ids: List,
         par_sim_ids: List,
         snllh: Dict,
     ):
         """Calculate gradients of the inner objective function.
 
@@ -184,106 +203,164 @@
                     not isinstance(par_opt, str)
                     or par_opt in already_calculated
                 ):
                     continue
                 # Current fix for scaling/offset parameters in models.
                 elif par_sim.startswith('observableParameter'):
                     continue
+                # For noise parameters optimized hierarchically, we
+                # do not calculate the gradient.
+                elif (
+                    par_sim.startswith('noiseParameter')
+                    and par_opt not in par_opt_ids
+                ):
+                    continue
                 else:
                     already_calculated.add(par_opt)
                 par_sim_idx = par_sim_ids.index(par_sim)
                 par_opt_idx = par_opt_ids.index(par_opt)
                 grad = 0.0
+
                 sy_for_outer_parameter = [
                     sy_cond[:, par_sim_idx, :] for sy_cond in sy
                 ]
+                ssigma_for_outer_parameter = [
+                    ssigma_cond[:, par_sim_idx, :]
+                    for ssigma_cond in amici_ssigma
+                ]
 
                 for group_idx, group in enumerate(
                     problem.get_groups_for_xs(InnerParameterType.SPLINE)
                 ):
                     # Get the reformulated spline parameters
                     s = np.asarray(x_inner_opt[group_idx][SCIPY_X])
                     group_dict = problem.groups[group]
 
                     measurements = group_dict[DATAPOINTS]
-                    sigma = group_dict[NOISE_PARAMETERS]
+                    sigma = group_dict[INNER_NOISE_PARS]
                     sim_all = group_dict[CURRENT_SIMULATION]
                     N = group_dict[N_SPLINE_PARS]
                     K = group_dict[NUM_DATAPOINTS]
 
                     sy_all = extract_expdata_using_mask(
                         expdata=sy_for_outer_parameter,
                         mask=group_dict[EXPDATA_MASK],
                     )
+                    ssigma_all = extract_expdata_using_mask(
+                        expdata=ssigma_for_outer_parameter,
+                        mask=group_dict[EXPDATA_MASK],
+                    )
 
                     delta_c, c, n = self._rescale_spline_bases(
                         sim_all=sim_all, N=N, K=K
                     )
                     delta_c_dot, c_dot = calculate_spline_bases_gradient(
                         sim_all=sim_all, sy_all=sy_all, N=N
                     )
                     C = np.diag(-np.ones(N))
 
                     # For the reformulated problem, mu can be calculated
                     # as the inner gradient at the optimal point s.
-                    mu = calculate_inner_gradient(
+                    mu = calculate_inner_gradient_for_obs(
                         s=s,
                         sim_all=sim_all,
                         measurements=measurements,
-                        sigma=sigma,
                         N=N,
                         delta_c=delta_c,
                         c=c,
                         n=n,
                     )
                     min_meas = group_dict[MIN_DATAPOINT]
                     max_meas = group_dict[MAX_DATAPOINT]
                     min_diff = self._get_minimal_difference(
                         measurement_range=max_meas - min_meas,
                         N=N,
                         min_diff_factor=self.options[MIN_DIFF_FACTOR],
                     )
 
-                    # Calculate df_ds term only if mu is not all 0
+                    # If the spline parameter is at its boundary, the
+                    # corresponding Lagrangian multiplier mu is set to 0.
+                    min_diff_all = np.full(N, min_diff)
+                    min_diff_all[0] = 0.0
+                    mu = np.asarray(
+                        [
+                            mu[i]
+                            if np.isclose(s[i] - min_diff_all[i], 0)
+                            else 0
+                            for i in range(len(s))
+                        ]
+                    )
+
+                    # Calculate (dJ_ds * ds_dtheta) term only if mu is not all 0
+                    ds_grad_term = 0.0
                     if np.any(mu):
                         s_dot = calculate_ds_dtheta(
                             sim_all=sim_all,
                             sy_all=sy_all,
                             measurements=measurements,
-                            sigma=sigma,
                             s=s,
                             C=C,
                             mu=mu,
                             N=N,
                             delta_c=delta_c,
                             delta_c_dot=delta_c_dot,
                             c=c,
                             c_dot=c_dot,
                             n=n,
                             min_diff=min_diff,
                         )
-                        df_ds = mu
-                        grad += df_ds.dot(s_dot)
+                        dres_ds = mu
+                        ds_grad_term = dres_ds.dot(s_dot)
 
-                    # Let's calculate the df_dyk term now:
-                    df_dyk = calculate_df_dyk(
+                    # Let's calculate the (dJ_dy * dy_dtheta) term now:
+                    dy_grad_term = calculate_dy_term(
                         sim_all=sim_all,
                         sy_all=sy_all,
                         measurements=measurements,
-                        sigma=sigma,
                         s=s,
                         N=N,
                         delta_c=delta_c,
                         delta_c_dot=delta_c_dot,
                         c=c,
                         c_dot=c_dot,
                         n=n,
                     )
 
-                    grad += df_dyk
+                    # Let's calculate the (dJ_dsigma^2 * dsigma^2_dtheta) term now:
+                    if not group_dict[OPTIMIZE_NOISE]:
+                        residual_squared = (
+                            calculate_objective_function_for_obs(
+                                s=s,
+                                sim_all=sim_all,
+                                measurements=measurements,
+                                N=N,
+                                delta_c=delta_c,
+                                c=c,
+                                n=n,
+                            )
+                        )
+                        dJ_dsigma2 = (
+                            K / (2 * sigma**2)
+                            - residual_squared / sigma**4
+                        )
+                        dsigma2_dtheta = ssigma_all[0]
+                        dsigma_grad_term = dJ_dsigma2 * dsigma2_dtheta
+                    # If we optimize the noise hierarchically,
+                    # the last term (dJ_dsigma^2 * dsigma^2_dtheta) is always 0
+                    # since the sigma is optimized such that dJ_dsigma2=0.
+                    else:
+                        dsigma_grad_term = 0.0
+
+                    # Combine all terms to get the complete gradient contribution
+                    grad += (
+                        dy_grad_term / sigma**2
+                        + ds_grad_term / sigma**2
+                        + dsigma_grad_term
+                    )
+
                 snllh[par_opt_idx] = grad
 
         return snllh
 
     @staticmethod
     def get_default_options() -> Dict:
         """Return default options for solving the inner problem."""
@@ -303,15 +380,14 @@
         ----------
         inner_parameters:
             The spline inner parameters.
         group_dict:
             The group dictionary.
         """
         group_measurements = group_dict[DATAPOINTS]
-        group_noise_parameters = group_dict[NOISE_PARAMETERS]
         current_group_simulation = group_dict[CURRENT_SIMULATION]
         n_datapoints = group_dict[NUM_DATAPOINTS]
         n_spline_pars = group_dict[N_SPLINE_PARS]
 
         (
             distance_between_bases,
             spline_bases,
@@ -333,31 +409,29 @@
             N=n_spline_pars,
             min_meas=min_meas,
             max_meas=max_meas,
             min_diff=min_diff,
         )
 
         def objective_function_wrapper(x):
-            return calculate_objective_function(
+            return calculate_objective_function_for_obs(
                 s=x,
                 sim_all=current_group_simulation,
                 measurements=group_measurements,
-                sigma=group_noise_parameters,
                 N=n_spline_pars,
                 delta_c=distance_between_bases,
                 c=spline_bases,
                 n=intervals_per_sim,
             )
 
         def inner_gradient_wrapper(x):
-            return calculate_inner_gradient(
+            return calculate_inner_gradient_for_obs(
                 s=x,
                 sim_all=current_group_simulation,
                 measurements=group_measurements,
-                sigma=group_noise_parameters,
                 N=n_spline_pars,
                 delta_c=distance_between_bases,
                 c=spline_bases,
                 n=intervals_per_sim,
             )
 
         results = minimize(
@@ -501,46 +575,61 @@
             x0[0] = np.max([min_meas - 0.3 * range_all, 0])
 
         from scipy.optimize import Bounds
 
         inner_options = {
             "x0": x0,
             "method": "L-BFGS-B",
-            "options": {"ftol": 1e-10, "disp": None},
+            "options": {"ftol": 1e-16, "disp": None},
             "bounds": Bounds(lb=constraint_min_diff),
         }
 
         return inner_options
 
 
-def calculate_objective_function(
+def _calculate_sigma_for_group(
+    inner_result: Dict,
+    n_datapoints: int,
+):
+    """Calculate the noise parameter sigma.
+
+    Parameters
+    ----------
+    noise_parameters:
+        The noise parameters of a group of the inner problem.
+    inner_result:
+        The inner optimization result.
+    """
+    sigma = np.sqrt(2 * inner_result[SCIPY_FUN] / (n_datapoints))
+
+    return sigma
+
+
+def calculate_objective_function_for_obs(
     s: np.ndarray,
     sim_all: np.ndarray,
     measurements: np.ndarray,
-    sigma: np.ndarray,
     N: int,
     delta_c: float,
     c: np.ndarray,
     n: np.ndarray,
 ):
     """Objective function for reformulated inner spline problem."""
     obj = 0
 
-    for y_k, z_k, sigma_k, n_k in zip(sim_all, measurements, sigma, n):
+    for y_k, z_k, n_k in zip(sim_all, measurements, n):
         i = n_k - 1
         sum_s = 0
         sum_s = np.sum(s[:i])
         if i == 0:
-            obj += (1 / sigma_k**2) * (z_k - s[i]) ** 2
+            obj += (z_k - s[i]) ** 2
         elif i == N:
-            obj += (1 / sigma_k**2) * (z_k - sum_s) ** 2
+            obj += (z_k - sum_s) ** 2
         else:
-            obj += (1 / sigma_k**2) * (
-                z_k - (y_k - c[i - 1]) * s[i] / delta_c - sum_s
-            ) ** 2
+            obj += (z_k - (y_k - c[i - 1]) * s[i] / delta_c - sum_s) ** 2
     obj = obj / 2
     return obj
 
 
 def get_spline_mapped_simulations(
     s: np.ndarray,
     sim_all: np.ndarray,
@@ -563,48 +652,44 @@
             mapped_simulations[index] = (y_k - c[interval_index - 1]) * (
                 xi[interval_index] - xi[interval_index - 1]
             ) / delta_c + xi[interval_index - 1]
 
     return mapped_simulations
 
 
-def calculate_inner_gradient(
+def calculate_inner_gradient_for_obs(
     s: np.ndarray,
     sim_all: np.ndarray,
     measurements: np.ndarray,
-    sigma: np.ndarray,
     N: int,
     delta_c: float,
     c: np.ndarray,
     n: np.ndarray,
 ):
     """Gradient of the objective function for the reformulated inner spline problem."""
 
     gradient = np.zeros(N)
 
-    for y_k, z_k, sigma_k, n_k in zip(sim_all, measurements, sigma, n):
-        weight_k = 1 / sigma_k**2
+    for y_k, z_k, n_k in zip(sim_all, measurements, n):
         sum_s = 0
         i = n_k - 1  # just the iterator to go over the Jacobian array
         sum_s = np.sum(s[:i])
         if i == 0:
-            gradient[i] += weight_k * (s[i] - z_k)
+            gradient[i] += s[i] - z_k
         elif i == N:
-            for j in range(i):
-                gradient[j] += weight_k * (sum_s - z_k)
+            gradient[:i] += np.full(i, sum_s - z_k)
         else:
             gradient[i] += (
-                weight_k
-                * ((y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k)
+                ((y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k)
                 * (y_k - c[i - 1])
                 / delta_c
             )
             gradient[:i] += np.full(
                 i,
-                weight_k * ((y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k),
+                (y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k,
             )
     return gradient
 
 
 def calculate_inner_hessian(
     s: np.ndarray,
     sim_all: np.ndarray,
@@ -634,15 +719,14 @@
     return hessian
 
 
 def calculate_ds_dtheta(
     sim_all: np.ndarray,
     sy_all: np.ndarray,
     measurements: np.ndarray,
-    sigma: np.ndarray,
     s: np.ndarray,
     C: np.ndarray,
     mu: np.ndarray,
     N: int,
     delta_c: float,
     delta_c_dot: float,
     c: np.ndarray,
@@ -655,126 +739,121 @@
     Calculates the derivative of reformulated spline parameters s with respect to the
     dynamical parameter theta. Firstly, we calculate the derivative of the
     first two equations of the necessary optimality conditions of the
     optimization problem with inequality constraints. Then we solve the linear
     system to obtain the derivatives.
     """
 
-    Jacobian_derivative = np.zeros((N, N))
-    rhs = np.zeros(2 * N)
+    dgrad_dtheta_lhs = np.zeros((N, N))
+    dgrad_dtheta_rhs = np.zeros(2 * N)
 
-    for y_k, z_k, y_dot_k, sigma_k, n_k in zip(
-        sim_all, measurements, sy_all, sigma, n
-    ):
-        i = n_k - 1  # just the iterator to go over the Jacobian matrix
-        weight_k = 1 / sigma_k**2
+    for y_k, z_k, y_dot_k, n_k in zip(sim_all, measurements, sy_all, n):
+        i = n_k - 1  # just the iterator to go over the matrix
         sum_s = 0
         sum_s = np.sum(s[:i])
 
-        # calculate the Jacobian derivative:
+        # Calculate dgrad_dtheta in the form of a linear system:
         if i == 0:
-            Jacobian_derivative[i][i] += weight_k
+            dgrad_dtheta_lhs[i][i] += 1
         elif i == N:
-            Jacobian_derivative = Jacobian_derivative + np.full(
-                (N, N), weight_k
-            )
+            dgrad_dtheta_lhs = dgrad_dtheta_lhs + np.full((N, N), 1)
 
         else:
-            Jacobian_derivative[i][i] += (
-                weight_k * (y_k - c[i - 1]) ** 2 / delta_c**2
-            )
-            rhs[i] += (
-                weight_k
-                * (2 * (y_k - c[i - 1]) / delta_c * s[i] + sum_s - z_k)
+            dgrad_dtheta_lhs[i][i] += (y_k - c[i - 1]) ** 2 / delta_c**2
+            dgrad_dtheta_rhs[i] += (
+                (2 * (y_k - c[i - 1]) / delta_c * s[i] + sum_s - z_k)
                 * (
                     (y_dot_k - c_dot[i - 1]) * delta_c
                     - (y_k - c[i - 1]) * delta_c_dot
                 )
                 / delta_c**2
             )
-            if i > 0:
-                Jacobian_derivative[i, :i] += np.full(
-                    i, weight_k * (y_k - c[i - 1]) / delta_c
-                )
-                Jacobian_derivative[:i, i] += np.full(
-                    i, weight_k * (y_k - c[i - 1]) / delta_c
-                )
-                rhs[:i] += np.full(
-                    i,
-                    weight_k
-                    * (
-                        (y_dot_k - c_dot[i - 1]) * delta_c
-                        - (y_k - c[i - 1]) * delta_c_dot
-                    )
-                    * s[i]
-                    / delta_c**2,
+
+            dgrad_dtheta_lhs[i, :i] += np.full(i, (y_k - c[i - 1]) / delta_c)
+            dgrad_dtheta_lhs[:i, i] += np.full(i, (y_k - c[i - 1]) / delta_c)
+            dgrad_dtheta_rhs[:i] += np.full(
+                i,
+                (
+                    (y_dot_k - c_dot[i - 1]) * delta_c
+                    - (y_k - c[i - 1]) * delta_c_dot
                 )
-                Jacobian_derivative[:i, :i] += np.full((i, i), weight_k)
+                * s[i]
+                / delta_c**2,
+            )
+            dgrad_dtheta_lhs[:i, :i] += np.full((i, i), 1)
 
     from scipy import linalg
 
     constraint_min_diff = np.diag(np.full(N, min_diff))
-    constraint_min_diff[0][0] = 0
+    constraint_min_diff[0, 0] = 0
+
     lhs = np.block(
         [
-            [Jacobian_derivative, C],
+            [dgrad_dtheta_lhs, C],
             [-np.diag(mu), constraint_min_diff - np.diag(s)],
         ]
     )
-    ds_dtheta = linalg.lstsq(lhs, rhs, lapack_driver="gelsy")
+
+    ds_dtheta = linalg.lstsq(lhs, dgrad_dtheta_rhs, lapack_driver="gelsy")
 
     return ds_dtheta[0][:N]
 
 
-def calculate_df_dyk(
+def calculate_dy_term(
     sim_all: np.ndarray,
     sy_all: np.ndarray,
     measurements: np.ndarray,
-    sigma: np.ndarray,
     s: np.ndarray,
     N: int,
     delta_c: float,
     delta_c_dot: float,
     c: np.ndarray,
     c_dot: np.ndarray,
     n: np.ndarray,
 ):
     """Calculate the derivative of the objective function for one group with respect to the simulations."""
-    df_dyk = 0
+    df_dy = 0
 
-    for y_k, z_k, y_dot_k, sigma_k, n_k in zip(
-        sim_all, measurements, sy_all, sigma, n
-    ):
+    for y_k, z_k, y_dot_k, n_k in zip(sim_all, measurements, sy_all, n):
         i = n_k - 1
         sum_s = np.sum(s[:i])
         if i > 0 and i < N:
-            df_dyk += (
-                (1 / sigma_k**2)
-                * ((y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k)
+            df_dy += (
+                ((y_k - c[i - 1]) * s[i] / delta_c + sum_s - z_k)
                 * s[i]
                 * (
                     (y_dot_k - c_dot[i - 1]) * delta_c
                     - (y_k - c[i - 1]) * delta_c_dot
                 )
                 / delta_c**2
             )
-    return df_dyk
+        # There is no i==0 case, because in this case
+        # c[0] == y_k and so the derivative is zero.
+    return df_dy
 
 
 def calculate_spline_bases_gradient(
     sim_all: np.ndarray, sy_all: np.ndarray, N: int
 ):
     """Calculate gradient of the rescaled spline bases."""
 
     min_idx = np.argmin(sim_all)
     max_idx = np.argmax(sim_all)
 
+    min_all = sim_all[min_idx]
+    max_all = sim_all[max_idx]
+    # Coming directly from differentiating _rescale_spline_bases
     if sim_all[max_idx] - sim_all[min_idx] < MIN_SIM_RANGE:
         delta_c_dot = 0
         c_dot = np.full(N, (sy_all[max_idx] - sy_all[min_idx]) / 2)
+        average_value = (max_all + min_all) / 2
+        if average_value < (MIN_SIM_RANGE / 2):
+            c_dot = np.full(N, 0)
+        else:
+            c_dot = np.full(N, (sy_all[max_idx] - sy_all[min_idx]) / 2)
     else:
         delta_c_dot = (sy_all[max_idx] - sy_all[min_idx]) / (N - 1)
         c_dot = np.linspace(sy_all[min_idx], sy_all[max_idx], N)
 
     return delta_c_dot, c_dot
 
 
@@ -787,36 +866,70 @@
             expdata[condition_index][mask[condition_index]]
             for condition_index in range(len(mask))
         ]
     )
 
 
 def save_inner_parameters_to_inner_problem(
-    inner_parameters,
-    s,
+    inner_problem: SplineInnerProblem,
+    s: np.ndarray,
+    group: int,
 ) -> None:
     """Save inner parameter values to the inner subproblem.
 
     Calculates the non-reformulated inner spline parameters from
     the reformulated inner spline parameters and saves them to
     the inner subproblem.
 
     Parameters
     ----------
     inner_parameters : list
         List of inner parameters.
     s : np.ndarray
         Reformulated inner spline parameters.
     """
+    group_dict = inner_problem.groups[group]
+    inner_spline_parameters = inner_problem.get_xs_for_group(group)
+    inner_noise_parameters = inner_problem.get_noise_parameters_for_group(
+        group
+    )
+
     xi = np.zeros(len(s))
     for i in range(len(s)):
         xi[i] = np.sum(s[: i + 1])
 
-    for idx in range(len(inner_parameters)):
-        inner_parameters[idx].value = xi[idx]
+    for idx in range(len(inner_spline_parameters)):
+        inner_spline_parameters[idx].value = xi[idx]
+
+    sigma = group_dict[INNER_NOISE_PARS]
+
+    if group_dict[OPTIMIZE_NOISE]:
+        inner_noise_parameters[0].value = sigma
+
+
+def _calculate_nllh_for_group(
+    inner_result: Dict,
+    sigma: float,
+    n_datapoints: int,
+):
+    """Calculate the negative log-likelihood for the group.
+
+    Parameters
+    ----------
+    inner_result : dict
+        Result of the inner problem.
+    sigma : float
+        Standard deviation of the measurement noise.
+    n_datapoints : int
+        Number of datapoints.
+    """
+    inner_result[SCIPY_FUN] = 0.5 * np.log(
+        2 * np.pi * sigma**2
+    ) * n_datapoints + inner_result[SCIPY_FUN] / (sigma**2)
+    return inner_result
 
 
 def get_monotonicity_measure(measurement, simulation):
     """Get monotonicity measure by calculating inversions.
 
     Calculate the number of inversions in the simulation data
     with respect to the measurement data.
```

### Comparing `pypesto-0.3.0/pypesto/hierarchical/util.py` & `pypesto-0.3.1/pypesto/hierarchical/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/__init__.py` & `pypesto-0.3.1/pypesto/history/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/base.py` & `pypesto-0.3.1/pypesto/history/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/csv.py` & `pypesto-0.3.1/pypesto/history/csv.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/generate.py` & `pypesto-0.3.1/pypesto/history/generate.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/hdf5.py` & `pypesto-0.3.1/pypesto/history/hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/memory.py` & `pypesto-0.3.1/pypesto/history/memory.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/optimizer.py` & `pypesto-0.3.1/pypesto/history/optimizer.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/options.py` & `pypesto-0.3.1/pypesto/history/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/history/util.py` & `pypesto-0.3.1/pypesto/history/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/logging.py` & `pypesto-0.3.1/pypesto/logging.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/aesara/base.py` & `pypesto-0.3.1/pypesto/objective/aesara/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/aggregated.py` & `pypesto-0.3.1/pypesto/objective/aggregated.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from copy import deepcopy
-from typing import Sequence, Tuple
+from typing import Any, Dict, Sequence, Tuple
 
 import numpy as np
 
 from ..C import FVAL, GRAD, HESS, HESSP, RDATAS, RES, SRES, ModeType
 from .base import ObjectiveBase, ResultDict
 
 
@@ -77,26 +77,46 @@
         )
 
     def call_unprocessed(
         self,
         x: np.ndarray,
         sensi_orders: Tuple[int, ...],
         mode: ModeType,
+        kwargs_list: Sequence[Dict[str, Any]] = None,
         **kwargs,
     ) -> ResultDict:
         """
         See `ObjectiveBase` for more documentation.
 
         Main method to overwrite from the base class. It handles and
         delegates the actual objective evaluation.
+
+        Parameters
+        ----------
+        kwargs_list:
+            Objective-specific keyword arguments, where the dictionaries are
+            ordered by the objectives.
         """
+        if kwargs_list is None:
+            kwargs_list = [{}] * len(self._objectives)
+        elif len(kwargs_list) != len(self._objectives):
+            raise ValueError(
+                "The length of `kwargs_list` must match the number of "
+                "objectives you are aggregating."
+            )
         return aggregate_results(
             [
-                objective.call_unprocessed(x, sensi_orders, mode, **kwargs)
-                for objective in self._objectives
+                objective.call_unprocessed(
+                    x,
+                    sensi_orders,
+                    mode,
+                    **kwargs,
+                    **cur_kwargs,
+                )
+                for objective, cur_kwargs in zip(self._objectives, kwargs_list)
             ]
         )
 
     def initialize(self):
         """See `ObjectiveBase` documentation."""
         for objective in self._objectives:
             objective.initialize()
```

### Comparing `pypesto-0.3.0/pypesto/objective/amici/amici.py` & `pypesto-0.3.1/pypesto/objective/amici/amici.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import tempfile
 from collections import OrderedDict
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
-from ...C import FVAL, MODE_FUN, MODE_RES, RDATAS, ModeType
+from ...C import FVAL, INNER_PARAMETERS, MODE_FUN, MODE_RES, RDATAS, ModeType
 from ..base import ObjectiveBase, ResultDict
 from .amici_calculator import AmiciCalculator
 from .amici_util import (
     create_identity_parameter_mapping,
     map_par_opt_to_par_sim,
 )
 
@@ -210,14 +210,17 @@
         self.calculator = calculator
         super().__init__(x_names=x_names)
 
         # Custom (condition-specific) timepoints. See the
         # `set_custom_timepoints` method for more information.
         self.custom_timepoints = None
 
+        # Initialize the dictionary for saving of inner parameters.
+        self.inner_parameters: Dict[str, float] = {}
+
     def get_config(self) -> dict:
         """Return basic information of the objective configuration."""
         info = super().get_config()
         info['x_names'] = self.x_names
         info['model_name'] = self.amici_model.getName()
         info['solver'] = str(type(self.amici_solver))
         info['sensi_order'] = self.max_sensi_order
@@ -449,14 +452,16 @@
             x_ids=self.x_ids,
             parameter_mapping=parameter_mapping,
             fim_for_hess=self.fim_for_hess,
         )
 
         nllh = ret[FVAL]
         rdatas = ret[RDATAS]
+        if INNER_PARAMETERS in ret and ret[INNER_PARAMETERS]:
+            self.inner_parameters = ret[INNER_PARAMETERS]
 
         # check whether we should update data for preequilibration guesses
         if (
             self.guess_steadystate
             and nllh <= self.steadystate_guesses['fval']
             and nllh < np.inf
         ):
```

### Comparing `pypesto-0.3.0/pypesto/objective/amici/amici_calculator.py` & `pypesto-0.3.1/pypesto/objective/amici/amici_calculator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/amici/amici_util.py` & `pypesto-0.3.1/pypesto/objective/amici/amici_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,21 @@
         condition_map_sim_var[par_id]
         for par_id in amici_model.getParameterIds()
     ]
 
     # iterate over simulation parameter indices
     for ix, val in enumerate(par_sim_vals):
         if not isinstance(val, numbers.Number):
-            # value is optimization parameter id
-            par_sim_vals[ix] = x_dct[val]
+            try:
+                # value is optimization parameter id
+                par_sim_vals[ix] = x_dct[val]
+            except KeyError:
+                # this may happen in case of states with NaN in the conditions
+                #  table
+                par_sim_vals[ix] = np.nan
 
     # return the created simulation parameter vector
     return np.array(par_sim_vals)
 
 
 def create_plist_from_par_opt_to_par_sim(mapping_par_opt_to_par_sim):
     """
```

### Comparing `pypesto-0.3.0/pypesto/objective/base.py` & `pypesto-0.3.1/pypesto/objective/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/finite_difference.py` & `pypesto-0.3.1/pypesto/objective/finite_difference.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/function.py` & `pypesto-0.3.1/pypesto/objective/function.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/jax/base.py` & `pypesto-0.3.1/pypesto/objective/jax/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/julia/base.py` & `pypesto-0.3.1/pypesto/objective/julia/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/pre_post_process.py` & `pypesto-0.3.1/pypesto/objective/pre_post_process.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/objective/priors.py` & `pypesto-0.3.1/pypesto/objective/priors.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/__init__.py` & `pypesto-0.3.1/pypesto/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/ess/cess.py` & `pypesto-0.3.1/pypesto/optimize/ess/cess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/ess/ess.py` & `pypesto-0.3.1/pypesto/optimize/ess/ess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/ess/function_evaluator.py` & `pypesto-0.3.1/pypesto/optimize/ess/function_evaluator.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/ess/refset.py` & `pypesto-0.3.1/pypesto/optimize/ess/refset.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/ess/sacess.py` & `pypesto-0.3.1/pypesto/optimize/ess/sacess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/load.py` & `pypesto-0.3.1/pypesto/optimize/load.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/optimize.py` & `pypesto-0.3.1/pypesto/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/optimizer.py` & `pypesto-0.3.1/pypesto/optimize/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import time
 import warnings
 from typing import TYPE_CHECKING, Dict, Optional
 
 import numpy as np
 import scipy.optimize
 
-from ..C import FVAL, GRAD, MODE_FUN, MODE_RES
+from ..C import FVAL, GRAD, INNER_PARAMETERS, MODE_FUN, MODE_RES
 from ..history import (
     HistoryOptions,
     NoHistory,
     OptimizerHistory,
     create_history,
 )
 from ..objective import Objective
@@ -447,14 +447,16 @@
             x=np.array(res.x),
             fval=fval,
             grad=grad,
             hess=getattr(res, 'hess', None),
             exitflag=res.status,
             message=res.message,
         )
+        if hasattr(objective, INNER_PARAMETERS) and objective.inner_parameters:
+            optimizer_result[INNER_PARAMETERS] = objective.inner_parameters
 
         return optimizer_result
 
     def is_least_squares(self):
         """Check whether optimizer is a least squares optimizer."""
         return re.match(r'(?i)^(ls_)', self.method)
```

### Comparing `pypesto-0.3.0/pypesto/optimize/options.py` & `pypesto-0.3.1/pypesto/optimize/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/task.py` & `pypesto-0.3.1/pypesto/optimize/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/optimize/util.py` & `pypesto-0.3.1/pypesto/optimize/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,25 +149,24 @@
         A result object to append the optimization results to. For example,
         one might append more runs to a previous optimization. Assign only
         unique ids.
     n_starts:
         Number of starts of the optimizer.
     """
     used_ids = set()
+    n_used = 0
     if result is not None:
         used_ids = set(result.optimize_result.id)
-        N_used = len(used_ids)
+        n_used = len(used_ids)
     if ids is None:
         i = 0
-        ids = [str(j) for j in range(i * n_starts, (i + 1) * n_starts)]
+        ids = [str(j) for j in range(0, n_starts)]
         while not used_ids.isdisjoint(ids):
             i += 1
-            ids = [
-                str(j) for j in range(N_used * i, N_used * (i + 1) + n_starts)
-            ]
+            ids = [str(j) for j in range(n_used * i, n_used * i + n_starts)]
     if len(ids) != n_starts:
         raise AssertionError("Number of starts and ids must coincide.")
     if not used_ids.isdisjoint(ids):
         raise AssertionError(
             "Manually assigned ids must differ from existing ones."
         )
     return ids
```

### Comparing `pypesto-0.3.0/pypesto/petab/__init__.py` & `pypesto-0.3.1/pypesto/petab/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 =====
 
 pyPESTO support for the PEtab data format.
 """
 import warnings
 
 from .importer import PetabImporter
-from .pysb_importer import PetabImporterPysb
 
 # PEtab and amici are optional dependencies
 
 
 try:
     import petab
 except ImportError:
```

### Comparing `pypesto-0.3.0/pypesto/petab/importer.py` & `pypesto-0.3.1/pypesto/petab/importer.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,22 +331,23 @@
         """
         Compile the model.
 
         If the output folder exists already, it is first deleted.
 
         Parameters
         ----------
-        kwargs: Extra arguments passed to `amici.SbmlImporter.sbml2amici`.
-
+        kwargs:
+            Extra arguments passed to :meth:`amici.SbmlImporter.sbml2amici`
+            or :meth:`amici.pysb_import.pysb2amici`.
         """
         # delete output directory
         if os.path.exists(self.output_folder):
             shutil.rmtree(self.output_folder)
 
-        amici.petab_import.import_model(
+        amici.petab_import.import_petab_problem(
             petab_problem=self.petab_problem,
             model_name=self.model_name,
             model_output_dir=self.output_folder,
             **kwargs,
         )
 
     def create_solver(self, model: amici.Model = None) -> amici.Solver:
@@ -464,24 +465,24 @@
 
         elif self._hierarchical:
             inner_problem = InnerProblem.from_petab_amici(
                 self.petab_problem, model, edatas
             )
             calculator = HierarchicalAmiciCalculator(inner_problem)
             amici_reporting = amici.RDataReporting.full
-            inner_parameter_ids = calculator.inner_problem.get_x_ids()
-            par_ids = [x for x in par_ids if x not in inner_parameter_ids]
 
         if self._hierarchical:
             # FIXME: currently not supported with hierarchical
             if 'guess_steadystate' in kwargs and kwargs['guess_steadystate']:
                 warnings.warn(
                     "`guess_steadystate` not supported with hierarchical optimization. Disabling `guess_steadystate`."
                 )
             kwargs['guess_steadystate'] = False
+            inner_parameter_ids = calculator.get_inner_parameter_ids()
+            par_ids = [x for x in par_ids if x not in inner_parameter_ids]
 
         # create objective
         obj = AmiciObjective(
             amici_model=model,
             amici_solver=solver,
             edatas=edatas,
             x_ids=par_ids,
@@ -696,17 +697,17 @@
                 objective.calculator, HierarchicalAmiciCalculator
             ):
                 raise AssertionError(
                     f"If hierarchical optimization of relative data is enabled, the `calculator` attribute of the `objective` has to be {HierarchicalAmiciCalculator} and not {objective.calculator}."
                 )
         # In case of hierarchical optimization, parameters estimated in the
         # inner subproblem are removed from the outer problem
-        if not self._non_quantitative_data_types and self._hierarchical:
+        if self._hierarchical:
             inner_parameter_ids = (
-                objective.calculator.inner_problem.get_x_ids()
+                objective.calculator.get_inner_parameter_ids()
             )
             lb = [b for x, b in zip(x_ids, lb) if x not in inner_parameter_ids]
             ub = [b for x, b in zip(x_ids, ub) if x not in inner_parameter_ids]
             x_ids = [x for x in x_ids if x not in inner_parameter_ids]
             x_fixed_indices = list(
                 map(x_ids.index, self.petab_problem.x_fixed_ids)
             )
@@ -853,40 +854,40 @@
 def _find_output_folder_name(
     petab_problem: petab.Problem,
     model_name: str,
 ) -> str:
     """
     Find a name for storing the compiled amici model in.
 
-    If available, use the sbml model name from the `petab_problem` or the
-    provided `model_name` (latter is given priority), otherwise create a
+    If available, use the model name from the ``petab_problem`` or the
+    provided ``model_name`` (latter is given priority), otherwise create a
     unique name. The folder will be located in the
-    `PetabImporter.MODEL_BASE_DIR` subdirectory of the current directory.
+    ``PetabImporter.MODEL_BASE_DIR`` subdirectory of the current directory.
     """
     # check whether location for amici model is a file
     if os.path.exists(PetabImporter.MODEL_BASE_DIR) and not os.path.isdir(
         PetabImporter.MODEL_BASE_DIR
     ):
         raise AssertionError(
             f"{PetabImporter.MODEL_BASE_DIR} exists and is not a directory, "
             f"thus cannot create a directory for the compiled amici model."
         )
 
     # create base directory if non-existent
     if not os.path.exists(PetabImporter.MODEL_BASE_DIR):
         os.makedirs(PetabImporter.MODEL_BASE_DIR)
 
-    # try sbml model id
-    sbml_model_id = petab_problem.sbml_model.getId()
+    # try model id
+    model_id = petab_problem.model.model_id
     if model_name is not None:
-        sbml_model_id = model_name
+        model_id = model_name
 
-    if sbml_model_id:
+    if model_id:
         output_folder = os.path.abspath(
-            os.path.join(PetabImporter.MODEL_BASE_DIR, sbml_model_id)
+            os.path.join(PetabImporter.MODEL_BASE_DIR, model_id)
         )
     else:
         # create random folder name
         output_folder = os.path.abspath(
             tempfile.mkdtemp(dir=PetabImporter.MODEL_BASE_DIR)
         )
     return output_folder
```

### Comparing `pypesto-0.3.0/pypesto/predict/amici_predictor.py` & `pypesto-0.3.1/pypesto/predict/amici_predictor.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/predict/task.py` & `pypesto-0.3.1/pypesto/predict/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/problem/base.py` & `pypesto-0.3.1/pypesto/problem/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,18 +233,18 @@
         if np.isnan(self.ub).any():
             raise ValueError('ub must not contain nan values')
         if np.any(self.lb >= self.ub):
             raise ValueError('lb<ub not fulfilled.')
 
     def _check_x_guesses(self):
         """Check whether the supplied x_guesses adhere to the bounds."""
-        if self.x_guesses == np.zeros((0, self.dim_full)):
+        if self.x_guesses.size == 0:
             return
-        adheres_ub = self.x_guesses < self.ub
-        adheres_lb = self.x_guesses < self.lb
+        adheres_ub = self.x_guesses <= self.ub
+        adheres_lb = self.x_guesses >= self.lb
         adheres_bounds = adheres_ub & adheres_lb
         # if any bounds are violated, log a warning
         if not adheres_bounds.all():
             logger.warning(
                 "Some initial guesses supplied violate the bounds "
                 "set for this problem."
             )
```

### Comparing `pypesto-0.3.0/pypesto/profile/approximate.py` & `pypesto-0.3.1/pypesto/profile/approximate.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/options.py` & `pypesto-0.3.1/pypesto/profile/options.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/profile.py` & `pypesto-0.3.1/pypesto/profile/profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/profile_next_guess.py` & `pypesto-0.3.1/pypesto/profile/profile_next_guess.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/task.py` & `pypesto-0.3.1/pypesto/profile/task.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/util.py` & `pypesto-0.3.1/pypesto/profile/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/validation_intervals.py` & `pypesto-0.3.1/pypesto/profile/validation_intervals.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/profile/walk_along_profile.py` & `pypesto-0.3.1/pypesto/profile/walk_along_profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/result/optimize.py` & `pypesto-0.3.1/pypesto/result/optimize.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/result/predict.py` & `pypesto-0.3.1/pypesto/result/predict.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/result/profile.py` & `pypesto-0.3.1/pypesto/result/profile.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/result/result.py` & `pypesto-0.3.1/pypesto/result/result.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/result/sample.py` & `pypesto-0.3.1/pypesto/result/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/__init__.py` & `pypesto-0.3.1/pypesto/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/adaptive_metropolis.py` & `pypesto-0.3.1/pypesto/sample/adaptive_metropolis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/adaptive_parallel_tempering.py` & `pypesto-0.3.1/pypesto/sample/adaptive_parallel_tempering.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/auto_correlation.py` & `pypesto-0.3.1/pypesto/sample/auto_correlation.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/diagnostics.py` & `pypesto-0.3.1/pypesto/sample/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/dynesty.py` & `pypesto-0.3.1/pypesto/sample/dynesty.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/emcee.py` & `pypesto-0.3.1/pypesto/sample/emcee.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/geweke_test.py` & `pypesto-0.3.1/pypesto/sample/geweke_test.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/metropolis.py` & `pypesto-0.3.1/pypesto/sample/metropolis.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,14 +108,17 @@
         if not self.temper_lpost:
             # extract current log likelihood value
             llh = lpost - lprior
             # extract proposed log likelihood value
             llh_new = lpost_new - lprior_new
             # log acceptance probability (temper log likelihood)
             log_p_acc = min(beta * (llh_new - llh) + (lprior_new - lprior), 0)
+            # catch the nan case which occurs if both lpost_new and lprior_new are -inf
+            if np.isnan(log_p_acc):
+                log_p_acc = -np.inf
         else:
             # log acceptance probability (temper log posterior)
             log_p_acc = min(beta * (lpost_new - lpost), 0)
 
         # flip a coin
         u = np.random.uniform(0, 1)
```

### Comparing `pypesto-0.3.0/pypesto/sample/parallel_tempering.py` & `pypesto-0.3.1/pypesto/sample/parallel_tempering.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/pymc.py` & `pypesto-0.3.1/pypesto/sample/pymc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/sample.py` & `pypesto-0.3.1/pypesto/sample/sample.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/sampler.py` & `pypesto-0.3.1/pypesto/sample/sampler.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/sample/util.py` & `pypesto-0.3.1/pypesto/sample/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/select/__init__.py` & `pypesto-0.3.1/pypesto/select/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/select/method.py` & `pypesto-0.3.1/pypesto/select/method.py`

 * *Files 1% similar despite different names*

```diff
@@ -296,20 +296,27 @@
         # Use candidate space if provided.
         if candidate_space is not None:
             self.candidate_space = candidate_space
             if predecessor_model is not None:
                 candidate_space.set_predecessor_model(predecessor_model)
         # Else generate one based on the PEtab Select problem.
         else:
-            self.candidate_space = (
-                self.petab_select_problem.new_candidate_space(
-                    method=self.method,
-                    predecessor_model=self.predecessor_model,
+            if predecessor_model is not None:
+                self.candidate_space = (
+                    self.petab_select_problem.new_candidate_space(
+                        method=self.method,
+                        predecessor_model=self.predecessor_model,
+                    )
+                )
+            else:
+                self.candidate_space = (
+                    self.petab_select_problem.new_candidate_space(
+                        method=self.method,
+                    )
                 )
-            )
         # May have changed from `None` to `petab_select.VIRTUAL_INITIAL_MODEL`
         self.predecessor_model = self.candidate_space.get_predecessor_model()
 
     def __call__(
         self,
         predecessor_model: Optional[Union[Model, None]] = None,
         newly_calibrated_models: Optional[Dict[str, Model]] = None,
@@ -353,18 +360,14 @@
         candidate_space = petab_select.ui.candidates(
             problem=self.petab_select_problem,
             candidate_space=self.candidate_space,
             limit=self.limit,
             calibrated_models=self.calibrated_models,
             newly_calibrated_models=newly_calibrated_models,
             excluded_model_hashes=self.calibrated_models.keys(),
-            # FIXME meaning changes here, i.e. predecessor model is used as previous
-            #       predecessor model, since PEtab Select now gets the next predecessor
-            #       model if the candidate space has models.
-            previous_predecessor_model=predecessor_model,
             criterion=self.criterion,
         )
         predecessor_model = self.candidate_space.predecessor_model
 
         if not candidate_space.models:
             raise StopIteration("No valid models found.")
```

### Comparing `pypesto-0.3.0/pypesto/select/misc.py` & `pypesto-0.3.1/pypesto/select/misc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/select/model_problem.py` & `pypesto-0.3.1/pypesto/select/model_problem.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/select/postprocessors.py` & `pypesto-0.3.1/pypesto/select/postprocessors.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/select/problem.py` & `pypesto-0.3.1/pypesto/select/problem.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,17 @@
         model_lists = []
         newly_calibrated_models_list = [
             self.newly_calibrated_models for _ in predecessor_models
         ]
 
         method_caller = self.create_method_caller(**kwargs)
         for start_index, predecessor_model in enumerate(predecessor_models):
+            method_caller.candidate_space.previous_predecessor_model = (
+                predecessor_model
+            )
             (
                 best_model,
                 newly_calibrated_models_list[start_index],
             ) = method_caller(
                 predecessor_model=predecessor_model,
                 newly_calibrated_models=newly_calibrated_models_list[
                     start_index
```

### Comparing `pypesto-0.3.0/pypesto/startpoint/base.py` & `pypesto-0.3.1/pypesto/startpoint/base.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/startpoint/latin_hypercube.py` & `pypesto-0.3.1/pypesto/startpoint/latin_hypercube.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/startpoint/uniform.py` & `pypesto-0.3.1/pypesto/startpoint/uniform.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/store/auto.py` & `pypesto-0.3.1/pypesto/store/auto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 """Auto-saving."""
 
 import binascii
 import datetime
+import logging
 import os
 from typing import Callable, Union
 
+import h5py
+
 from ..result import Result
 from .save_to_hdf5 import write_result
 
+logger = logging.getLogger(__name__)
+
 
 def autosave(
     filename: Union[str, Callable, None],
     result: Result,
     store_type: str,
     overwrite: bool = False,
 ):
@@ -36,14 +41,25 @@
         Whether to overwrite the currently existing results.
     """
     if filename is None:
         return
 
     if filename == "Auto":
         filename = default_filename
+    elif isinstance(filename, str):
+        if os.path.exists(filename) and not overwrite:
+            with h5py.File(filename, 'r') as f:
+                storage_used = store_type in f.keys()
+            if storage_used:
+                logger.warning(
+                    f"There is already a {store_type}-result saved in "
+                    f"{filename}. Please choose a different filename or set "
+                    f"overwrite=True. File will be saved as in AUTO mode."
+                )
+                filename = default_filename
     if not isinstance(filename, str):
         filename = filename(
             result=result,
             store_type=store_type,
             overwrite=overwrite,
         )
     # set the type to True and pass it on to write_result
```

### Comparing `pypesto-0.3.0/pypesto/store/hdf5.py` & `pypesto-0.3.1/pypesto/store/hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/store/read_from_hdf5.py` & `pypesto-0.3.1/pypesto/store/read_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/store/save_to_hdf5.py` & `pypesto-0.3.1/pypesto/store/save_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/testing/examples.py` & `pypesto-0.3.1/pypesto/testing/examples.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/util.py` & `pypesto-0.3.1/pypesto/util.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/__init__.py` & `pypesto-0.3.1/pypesto/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/clust_color.py` & `pypesto-0.3.1/pypesto/visualize/clust_color.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/dimension_reduction.py` & `pypesto-0.3.1/pypesto/visualize/dimension_reduction.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/ensemble.py` & `pypesto-0.3.1/pypesto/visualize/ensemble.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/misc.py` & `pypesto-0.3.1/pypesto/visualize/misc.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/model_fit.py` & `pypesto-0.3.1/pypesto/visualize/model_fit.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/optimization_stats.py` & `pypesto-0.3.1/pypesto/visualize/optimization_stats.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/optimizer_convergence.py` & `pypesto-0.3.1/pypesto/visualize/optimizer_convergence.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/optimizer_history.py` & `pypesto-0.3.1/pypesto/visualize/optimizer_history.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/ordinal_categories.py` & `pypesto-0.3.1/pypesto/visualize/ordinal_categories.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,17 @@
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
             pypesto_result.optimize_result.list[start_index]['x'],
         )
     )
+    x_dct.update(
+        pypesto_result.problem.objective.calculator.noise_dummy_values
+    )
 
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_result.problem.objective.edatas
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
     petab_problem = (
```

### Comparing `pypesto-0.3.0/pypesto/visualize/parameters.py` & `pypesto-0.3.1/pypesto/visualize/parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     size: Optional[Tuple[float, float]] = None,
     reference: Optional[List[ReferencePoint]] = None,
     colors: Optional[Union[RGBA, List[RGBA]]] = None,
     legends: Optional[Union[str, List[str]]] = None,
     balance_alpha: bool = True,
     start_indices: Optional[Union[int, Iterable[int]]] = None,
     scale_to_interval: Optional[Tuple[float, float]] = None,
+    plot_inner_parameters: bool = True,
 ) -> matplotlib.axes.Axes:
     """
     Plot parameter values.
 
     Parameters
     ----------
     results:
@@ -69,14 +70,16 @@
         avoid overplotting (default: True)
     start_indices:
         list of integers specifying the multistarts to be plotted or
         int specifying up to which start index should be plotted
     scale_to_interval:
         Tuple of bounds to which to scale all parameter values and bounds, or
         ``None`` to use bounds as determined by ``lb, ub``.
+    plot_inner_parameters:
+        Flag indicating whether to plot inner parameters (default: True).
 
     Returns
     -------
     ax:
         The plot axes.
     """
     # parse input
@@ -106,14 +109,15 @@
         # handle results and bounds
         (lb, ub, x_labels, fvals, xs) = handle_inputs(
             result=result,
             lb=lb,
             ub=ub,
             parameter_indices=parameter_indices,
             start_indices=start_indices,
+            plot_inner_parameters=plot_inner_parameters,
         )
         lb, ub, xs = map(scale_parameters, (lb, ub, xs))
 
         # call lowlevel routine
         ax = parameters_lowlevel(
             xs=xs,
             fvals=fvals,
@@ -332,14 +336,15 @@
 
 def handle_inputs(
     result: Result,
     parameter_indices: List[int],
     lb: Optional[Union[np.ndarray, List[float]]] = None,
     ub: Optional[Union[np.ndarray, List[float]]] = None,
     start_indices: Optional[Union[int, Iterable[int]]] = None,
+    plot_inner_parameters: bool = False,
 ) -> Tuple[np.ndarray, np.ndarray, List[str], np.ndarray, List[np.ndarray]]:
     """
     Compute the correct bounds for the parameter indices to be plotted.
 
     Outputs the corresponding parameters and their labels.
 
     Parameters
@@ -350,14 +355,16 @@
         Specifies which parameters should be plotted.
     lb, ub:
         If not None, override result.problem.lb, problem.problem.ub.
         Dimension either result.problem.dim or result.problem.dim_full.
     start_indices:
         list of integers specifying the multistarts to be plotted or
         int specifying up to which start index should be plotted
+    plot_inner_parameters:
+        Flag indicating whether inner parameters should be plotted.
 
     Returns
     -------
     lb, ub:
         Dimension either result.problem.dim or result.problem.dim_full.
     x_labels:
         ytick labels to be applied later on
@@ -365,26 +372,39 @@
         objective function values which are needed for plotting later
     xs:
         parameter values which will be plotted later
     """
     # retrieve results
     fvals = result.optimize_result.fval
     xs = result.optimize_result.x
+    # retrieve inner parameters if available
+    try:
+        inner_xs = result.optimize_result.inner_parameters
+        inner_xs_names = list(inner_xs[0].keys())
+        inner_xs = [list(inner_xs_idx.values()) for inner_xs_idx in inner_xs]
+        inner_lb = np.full(len(inner_xs_names), -np.inf)
+        inner_ub = np.full(len(inner_xs_names), np.inf)
+    except AttributeError:
+        inner_xs = None
 
     # parse indices which should be plotted
     if start_indices is not None:
         start_indices = process_start_indices(result, start_indices)
 
         # reduce number of displayed results
         xs_out = [xs[ind] for ind in start_indices]
         fvals_out = [fvals[ind] for ind in start_indices]
+        if inner_xs is not None and plot_inner_parameters:
+            inner_xs_out = [inner_xs[ind] for ind in start_indices]
     else:
         # use non-reduced versions
         xs_out = xs
         fvals_out = fvals
+        if inner_xs is not None and plot_inner_parameters:
+            inner_xs_out = inner_xs
 
     # get bounds
     if lb is None:
         lb = result.problem.lb_full
     if ub is None:
         ub = result.problem.ub_full
 
@@ -400,14 +420,23 @@
         lb = result.problem.get_reduced_vector(lb, parameter_indices)
         ub = result.problem.get_reduced_vector(ub, parameter_indices)
         x_labels = [x_labels[int(i)] for i in parameter_indices]
     else:
         lb = result.problem.get_full_vector(lb)
         ub = result.problem.get_full_vector(ub)
 
+    if inner_xs is not None and plot_inner_parameters:
+        lb = np.concatenate([lb, inner_lb])
+        ub = np.concatenate([ub, inner_ub])
+        x_labels = x_labels + inner_xs_names
+        xs_out = [
+            np.concatenate([x, inner_x])
+            for x, inner_x in zip(xs_out, inner_xs_out)
+        ]
+
     return lb, ub, x_labels, fvals_out, xs_out
 
 
 def parameters_correlation_matrix(
     result: Result,
     parameter_indices: Union[str, Sequence[int]] = 'free_only',
     start_indices: Optional[Union[int, Iterable[int]]] = None,
```

### Comparing `pypesto-0.3.0/pypesto/visualize/profile_cis.py` & `pypesto-0.3.1/pypesto/visualize/profile_cis.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/profiles.py` & `pypesto-0.3.1/pypesto/visualize/profiles.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/reference_points.py` & `pypesto-0.3.1/pypesto/visualize/reference_points.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/sampling.py` & `pypesto-0.3.1/pypesto/visualize/sampling.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/select.py` & `pypesto-0.3.1/pypesto/visualize/select.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto/visualize/spline_approximation.py` & `pypesto-0.3.1/pypesto/visualize/spline_approximation.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     x_dct = dict(
         zip(
             pypesto_result.problem.objective.x_ids,
             pypesto_result.optimize_result.list[start_index]['x'],
         )
     )
 
+    x_dct.update(
+        pypesto_result.problem.objective.calculator.noise_dummy_values
+    )
+
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_result.problem.objective.edatas
     parameter_mapping = pypesto_result.problem.objective.parameter_mapping
     amici_model = pypesto_result.problem.objective.amici_model
     amici_solver = pypesto_result.problem.objective.amici_solver
     n_threads = pypesto_result.problem.objective.n_threads
     observable_ids = amici_model.getObservableIds()
@@ -235,15 +239,15 @@
     # Get the parameters from the pypesto result for the start_index.
     x_dct = dict(
         zip(
             pypesto_problem.objective.x_ids,
             result.optimize_result.list[start_index]['x'],
         )
     )
-
+    x_dct.update(pypesto_problem.objective.calculator.noise_dummy_values)
     # Get the needed objects from the pypesto problem.
     edatas = pypesto_problem.objective.edatas
     parameter_mapping = pypesto_problem.objective.parameter_mapping
     amici_model = pypesto_problem.objective.amici_model
     amici_solver = pypesto_problem.objective.amici_solver
     n_threads = pypesto_problem.objective.n_threads
```

### Comparing `pypesto-0.3.0/pypesto/visualize/waterfall.py` & `pypesto-0.3.1/pypesto/visualize/waterfall.py`

 * *Files identical despite different names*

### Comparing `pypesto-0.3.0/pypesto.egg-info/PKG-INFO` & `pypesto-0.3.1/pypesto.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypesto
-Version: 0.3.0
+Version: 0.3.1
 Summary: python-based Parameter EStimation TOolbox
 Home-page: https://github.com/icb-dcm/pypesto
 Author: The pyPESTO developers
 Author-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de
 Maintainer: Yannik Schaelte, Jakob Vanhoefer, Paul Jost
 Maintainer-email: yannik.schaelte@gmail.com,jakob.vanhoefer@uni-bonn.de,paul.jost@uni-bonn.de
 License: BSD-3-Clause
@@ -42,15 +42,14 @@
 Provides-Extra: dynesty
 Provides-Extra: mltools
 Provides-Extra: julia
 Provides-Extra: doc
 Provides-Extra: example
 Provides-Extra: select
 Provides-Extra: test
-Provides-Extra: test_petab
 License-File: LICENSE
 
 # pyPESTO - Parameter EStimation TOolbox for python
 
 <img src="https://raw.githubusercontent.com/ICB-DCM/pyPESTO/master/doc/logo/logo_wordmark.png" width="50%" alt="pyPESTO logo"/>
 
 **pyPESTO** is a widely applicable and highly customizable toolbox for
```

### Comparing `pypesto-0.3.0/pypesto.egg-info/SOURCES.txt` & `pypesto-0.3.1/pypesto.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 pypesto/optimize/ess/cess.py
 pypesto/optimize/ess/ess.py
 pypesto/optimize/ess/function_evaluator.py
 pypesto/optimize/ess/refset.py
 pypesto/optimize/ess/sacess.py
 pypesto/petab/__init__.py
 pypesto/petab/importer.py
-pypesto/petab/pysb_importer.py
 pypesto/predict/__init__.py
 pypesto/predict/amici_predictor.py
 pypesto/predict/task.py
 pypesto/problem/__init__.py
 pypesto/problem/base.py
 pypesto/profile/__init__.py
 pypesto/profile/approximate.py
```

### Comparing `pypesto-0.3.0/pypesto.egg-info/requires.txt` & `pypesto-0.3.1/pypesto.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 tqdm>=4.46.0
 tabulate>=0.8.10
 
 [aesara]
 aesara>=2.0.5
 
 [all]
-amici>=0.14.0
-petab>=0.1.14
+amici>=0.18.0
+petab>=0.2.0
 ipopt
 dlib>=19.19.0
 nlopt>=2.6.2
 pyswarm>=0.6
 cma>=3.0.3
 pyswarms>=1.3.0
 fides>=0.6.1
@@ -40,37 +40,36 @@
 sphinx-rtd-theme>=1.2.0
 sphinx-autodoc-typehints>=1.18.3
 sphinxcontrib-bibtex>=2.5.0
 ipython>=8.4.0
 myst-parser>=0.18.0
 ipykernel>=6.15.1
 networkx>=2.5.1
-petab-select>=0.1.1
+petab-select>=0.1.8
 fides>=0.6.1
 notebook>=6.1.4
 networkx>=2.5.1
-petab-select>=0.1.1
+petab-select>=0.1.8
 pytest>=5.4.3
 pytest-cov>=2.10.0
 gitpython>=3.1.7
 pytest-rerunfailures>=9.1.1
 autograd>=1.3
-petabtests>=0.0.0a6
 
 [all_optimizers]
 ipopt
 dlib>=19.19.0
 nlopt>=2.6.2
 pyswarm>=0.6
 cma>=3.0.3
 pyswarms>=1.3.0
 fides>=0.6.1
 
 [amici]
-amici>=0.14.0
+amici>=0.18.0
 
 [cmaes]
 cma>=3.0.3
 
 [dlib]
 dlib>=19.19.0
 
@@ -81,15 +80,15 @@
 sphinx-rtd-theme>=1.2.0
 sphinx-autodoc-typehints>=1.18.3
 sphinxcontrib-bibtex>=2.5.0
 ipython>=8.4.0
 myst-parser>=0.18.0
 ipykernel>=6.15.1
 networkx>=2.5.1
-petab-select>=0.1.1
+petab-select>=0.1.8
 fides>=0.6.1
 
 [dynesty]
 dill>=0.3.6
 dynesty>=2.0.3
 
 [emcee]
@@ -120,33 +119,30 @@
 [mpi]
 mpi4py>=3.0.3
 
 [nlopt]
 nlopt>=2.6.2
 
 [petab]
-petab>=0.1.14
+petab>=0.2.0
 
 [pymc]
 arviz>=0.12.1
 aesara>=2.8.6
 pymc>=4.2.1
 
 [pyswarm]
 pyswarm>=0.6
 
 [pyswarms]
 pyswarms>=1.3.0
 
 [select]
 networkx>=2.5.1
-petab-select>=0.1.1
+petab-select>=0.1.8
 
 [test]
 pytest>=5.4.3
 pytest-cov>=2.10.0
 gitpython>=3.1.7
 pytest-rerunfailures>=9.1.1
 autograd>=1.3
-
-[test_petab]
-petabtests>=0.0.0a6
```

### Comparing `pypesto-0.3.0/setup.cfg` & `pypesto-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -64,27 +64,26 @@
 	%(emcee)s
 	%(dynesty)s
 	%(mltools)s
 	%(doc)s
 	%(example)s
 	%(select)s
 	%(test)s
-	%(test_petab)s
 all_optimizers = 
 	%(ipopt)s
 	%(dlib)s
 	%(nlopt)s
 	%(pyswarm)s
 	%(cmaes)s
 	%(pyswarms)s
 	%(fides)s
 amici = 
-	amici >= 0.14.0
+	amici >= 0.18.0
 petab = 
-	petab >= 0.1.14
+	petab >= 0.2.0
 ipopt = 
 	ipopt
 dlib = 
 	dlib >= 19.19.0
 nlopt = 
 	nlopt >= 2.6.2
 pyswarm = 
@@ -130,23 +129,21 @@
 	ipykernel >= 6.15.1
 	%(select)s
 	%(fides)s
 example = 
 	notebook >= 6.1.4
 select = 
 	networkx >= 2.5.1
-	petab-select >= 0.1.1
+	petab-select >= 0.1.8
 test = 
 	pytest >= 5.4.3
 	pytest-cov >= 2.10.0
 	gitpython >= 3.1.7
 	pytest-rerunfailures >= 9.1.1
 	autograd >= 1.3
-test_petab = 
-	petabtests >= 0.0.0a6
 
 [bdist_wheel]
 universal = False
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

