# Comparing `tmp/rlax-0.1.5.tar.gz` & `tmp/rlax-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlax-0.1.5.tar", last modified: Mon Jan  9 13:23:52 2023, max compression
+gzip compressed data, was "rlax-0.1.6.tar", last modified: Thu Jun 29 15:03:33 2023, max compression
```

## Comparing `rlax-0.1.5.tar` & `rlax-0.1.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.555113 rlax-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-01-09 13:23:40.000000 rlax-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-09 13:23:40.000000 rlax-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-01-09 13:23:52.555113 rlax-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-01-09 13:23:40.000000 rlax-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-01-09 13:23:40.000000 rlax-0.1.5/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/docs/ext/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-01-09 13:23:40.000000 rlax-0.1.5/docs/ext/coverage_check.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/online_q_lambda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/online_q_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/pop_art.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-01-09 13:23:40.000000 rlax-0.1.5/examples/simple_dqn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-09 13:23:40.000000 rlax-0.1.5/requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-01-09 13:23:40.000000 rlax-0.1.5/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-09 13:23:40.000000 rlax-0.1.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-09 13:23:40.000000 rlax-0.1.5/requirements/requirements_examples.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/rlax/
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.555113 rlax-0.1.5/rlax/_src/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/clipping_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/distributions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/episodic_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/episodic_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/exploration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/exploration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/general_value_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/general_value_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/interruptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/interruptions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/losses_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/model_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/model_learning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/moving_averages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/moving_averages_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/mpo_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    24818 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/mpo_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/multistep_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/nested_updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/nested_updates_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/nonlinear_bellman.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/nonlinear_bellman_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/policy_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/policy_gradients_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/policy_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/policy_targets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/pop_art.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/pop_art_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/tree_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/tree_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    31372 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/value_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)    32382 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/value_learning_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/vtrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/_src/vtrace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-09 13:23:40.000000 rlax-0.1.5/rlax/rlax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 13:23:52.547113 rlax-0.1.5/rlax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-09 13:23:52.000000 rlax-0.1.5/rlax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 13:23:52.555113 rlax-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-09 13:23:40.000000 rlax-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.881862 rlax-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-29 15:03:22.000000 rlax-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 15:03:22.000000 rlax-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-29 15:03:33.881862 rlax-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-29 15:03:22.000000 rlax-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.873862 rlax-0.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-29 15:03:22.000000 rlax-0.1.6/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.877862 rlax-0.1.6/docs/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-29 15:03:22.000000 rlax-0.1.6/docs/ext/coverage_check.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.877862 rlax-0.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/online_q_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/online_q_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/pop_art.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-06-29 15:03:22.000000 rlax-0.1.6/examples/simple_dqn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.877862 rlax-0.1.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 15:03:22.000000 rlax-0.1.6/requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-29 15:03:22.000000 rlax-0.1.6/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 15:03:22.000000 rlax-0.1.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 15:03:22.000000 rlax-0.1.6/requirements/requirements_examples.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.877862 rlax-0.1.6/rlax/
+-rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.881862 rlax-0.1.6/rlax/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/clipping_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23382 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/distributions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/episodic_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/episodic_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/exploration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/exploration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/general_value_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/general_value_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/interruptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/interruptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/losses_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/model_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/model_learning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/moving_averages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/moving_averages_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25523 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/mpo_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24862 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/mpo_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17856 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/multistep_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/nested_updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/nested_updates_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/nonlinear_bellman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/nonlinear_bellman_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10229 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/policy_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/policy_gradients_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/policy_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/policy_targets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/pop_art.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/pop_art_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/tree_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/tree_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31372 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/value_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32382 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/value_learning_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/vtrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/_src/vtrace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-29 15:03:22.000000 rlax-0.1.6/rlax/rlax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 15:03:33.877862 rlax-0.1.6/rlax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 15:03:33.000000 rlax-0.1.6/rlax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 15:03:33.881862 rlax-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-06-29 15:03:22.000000 rlax-0.1.6/setup.py
```

### Comparing `rlax-0.1.5/LICENSE` & `rlax-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/PKG-INFO` & `rlax-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlax
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of reinforcement learning building blocks in JAX.
 Home-page: https://github.com/deepmind/rlax
 Author: DeepMind
 Author-email: rlax-dev@google.com
 License: Apache 2.0
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RLax
 
 ![CI status](https://github.com/deepmind/rlax/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/rlax/badge/?version=latest)
```

### Comparing `rlax-0.1.5/README.md` & `rlax-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/docs/conf.py` & `rlax-0.1.6/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     'sphinx.ext.inheritance_diagram',
     'sphinx.ext.intersphinx',
     'sphinx.ext.linkcode',
     'sphinx.ext.napoleon',
     'sphinxcontrib.bibtex',
     'sphinxcontrib.katex',
     'sphinx_autodoc_typehints',
-    'sphinx_rtd_theme',
+    'sphinx_book_theme',
     'coverage_check',
     'myst_nb',  # This is used for the .ipynb notebooks
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
@@ -114,20 +114,24 @@
 
 autodoc_default_options = {
     'member-order': 'bysource',
     'special-members': True,
     'exclude-members': '__repr__, __str__, __weakref__',
 }
 
+# -- Options for bibtex ------------------------------------------------------
+
+bibtex_bibfiles = []
+
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'sphinx_rtd_theme'
+html_theme = 'sphinx_book_theme'
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = []
 # html_favicon = '_static/favicon.ico'
```

### Comparing `rlax-0.1.5/docs/ext/coverage_check.py` & `rlax-0.1.6/docs/ext/coverage_check.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/__init__.py` & `rlax-0.1.6/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/experiment.py` & `rlax-0.1.6/examples/experiment.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/online_q_lambda.py` & `rlax-0.1.6/examples/online_q_lambda.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/online_q_learning.py` & `rlax-0.1.6/examples/online_q_learning.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/pop_art.py` & `rlax-0.1.6/examples/pop_art.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/examples/simple_dqn.py` & `rlax-0.1.6/examples/simple_dqn.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/__init__.py` & `rlax-0.1.6/rlax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 from rlax._src.value_learning import td_lambda
 from rlax._src.value_learning import td_learning
 from rlax._src.vtrace import leaky_vtrace
 from rlax._src.vtrace import leaky_vtrace_td_error_and_advantage
 from rlax._src.vtrace import vtrace
 from rlax._src.vtrace import vtrace_td_error_and_advantage
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __all__ = (
     "add_gaussian_noise",
     "add_ornstein_uhlenbeck_noise",
     "add_dirichlet_noise",
     "AllSum",
     "batched_index",
```

### Comparing `rlax-0.1.5/rlax/_src/__init__.py` & `rlax-0.1.6/rlax/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/base.py` & `rlax-0.1.6/rlax/_src/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,24 @@
     broadcast_shape = source.shape + (1,) * (target.ndim - source.ndim)
     return jnp.reshape(source, broadcast_shape)
   raise ValueError(
       f"source shape {source.shape} is not compatible with "
       f"target shape {target.shape}")
 
 
-def replace_masked(data: chex.Array, replacement: chex.Array, mask: chex.Array):
+def replace_masked(
+    data: chex.Array, replacement: Optional[chex.Array], mask: chex.Array
+):
   """Replace slices of an array as indicated by a mask.
 
   Args:
     data: an array whose some elements we want to replace.
-    replacement: an array with the same shape as `data`, containing
-      the data to insert according to `mask`. If `None` is passed,
-      then the masked elements in `data` will be replaced with zeros.
+    replacement: an array with the same shape as `data`, containing the data to
+      insert according to `mask`. If `None` is passed, then the masked elements
+      in `data` will be replaced with zeros.
     mask: a mask of 0/1s, whose shape is a prefix of `data` and `replacements`.
       When the mask is 1, values of data are replaced.
 
   Returns:
     the updated tensor.
   """
   if replacement is None:
@@ -97,12 +99,12 @@
 
   def __init__(self, axis_name: Optional[str] = None):
     """Sums locally and then over devices with the axis name provided."""
     self._axis_name = axis_name
 
   def __call__(
       self, x: Array, axis: Optional[Union[int, Sequence[int]]] = None
-  ) -> Numeric:
+  ) -> Array:
     s = jnp.sum(x, axis=axis)
     if self._axis_name:
       s = jax.lax.psum(s, axis_name=self._axis_name)
     return s
```

### Comparing `rlax-0.1.5/rlax/_src/base_test.py` & `rlax-0.1.6/rlax/_src/base_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/clipping.py` & `rlax-0.1.6/rlax/_src/clipping.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/clipping_test.py` & `rlax-0.1.6/rlax/_src/clipping_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/distributions.py` & `rlax-0.1.6/rlax/_src/distributions.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/distributions_test.py` & `rlax-0.1.6/rlax/_src/distributions_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/embedding.py` & `rlax-0.1.6/rlax/_src/embedding.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/embedding_test.py` & `rlax-0.1.6/rlax/_src/embedding_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/episodic_memory.py` & `rlax-0.1.6/rlax/_src/episodic_memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,42 +23,38 @@
 from typing import Callable
 
 import chex
 import jax
 import jax.numpy as jnp
 
 Array = chex.Array
-Scalar = chex.Scalar
+MetricFn = Callable[[Array, Array], Array]
 
 
 @chex.dataclass
 class KNNQueryResult():
   neighbors: jnp.ndarray
   neighbor_indices: jnp.ndarray
   neighbor_neg_distances: jnp.ndarray
 
 
-def _sqeuclidian(x: Array, y: Array) -> Scalar:
+def _sqeuclidian(x: Array, y: Array) -> Array:
   return jnp.sum(jnp.square(x - y))
 
 
-def _cdist(
-    a: Array,
-    b: Array,
-    metric: Callable[[Array, Array], Scalar]
-) -> Array:
+def _cdist(a: Array, b: Array, metric: MetricFn) -> Array:
   """Returns the distance between each pair of the two collections of inputs."""
   return jax.vmap(jax.vmap(metric, (None, 0)), (0, None))(a, b)
 
 
 def knn_query(
     data: Array,
     query_points: Array,
     num_neighbors: int,
-    metric: Callable[[Array, Array], Scalar] = _sqeuclidian
+    metric: MetricFn = _sqeuclidian,
 ) -> KNNQueryResult:
   """Finds closest neighbors in data to the query points & their neg distances.
 
   NOTE: For this function to be jittable, static_argnums=[2,] must be passed, as
   the internal jax.lax.top_k(neg_distances, num_neighbors) computation cannot be
   jitted with a dynamic num_neighbors that is passed as an argument.
```

### Comparing `rlax-0.1.5/rlax/_src/episodic_memory_test.py` & `rlax-0.1.6/rlax/_src/episodic_memory_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/exploration.py` & `rlax-0.1.6/rlax/_src/exploration.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,15 +254,15 @@
                               jnp.zeros_like(distance_rate))
 
   # Compute the Kernel value K(xₖ, x) = ε/(rate + ε).
   kernel_output = epsilon / (distance_rate + epsilon)
 
   # Compute the similarity for the embedding x:
   # s = √(Σ_{xₖ ∈ Nₖ} K(xₖ, x)) + c
-  similarity = (jnp.sqrt(jnp.sum(kernel_output, axis=-1)) + constant)
+  similarity = jnp.sqrt(jnp.sum(kernel_output, axis=-1)) + constant
 
   # Compute the intrinsic reward:
   # r = 1 / s.
   reward_new = jnp.ones_like(embeddings[..., 0]) / similarity
 
   # Zero the reward if similarity is greater than max_similarity
   # r <- 0 if s > sₘₐₓ otherwise r.
```

### Comparing `rlax-0.1.5/rlax/_src/exploration_test.py` & `rlax-0.1.6/rlax/_src/exploration_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/general_value_functions.py` & `rlax-0.1.6/rlax/_src/general_value_functions.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/general_value_functions_test.py` & `rlax-0.1.6/rlax/_src/general_value_functions_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/interruptions.py` & `rlax-0.1.6/rlax/_src/interruptions.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/interruptions_test.py` & `rlax-0.1.6/rlax/_src/interruptions_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/losses.py` & `rlax-0.1.6/rlax/_src/losses.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,11 +204,11 @@
     expectile: A float value that represents the weights assigned to predictions
       that over-estimate targets.
 
   Returns:
     a vector of same shape as predictions.
   """
   chex.assert_equal_shape([predictions, targets])
-  diff = (targets - predictions)
+  diff = targets - predictions
   is_underestimation = jnp.less(diff, 0)
   weight = jnp.abs(expectile - is_underestimation)
   return weight * (diff**2)
```

### Comparing `rlax-0.1.5/rlax/_src/losses_test.py` & `rlax-0.1.6/rlax/_src/losses_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/model_learning.py` & `rlax-0.1.6/rlax/_src/model_learning.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/model_learning_test.py` & `rlax-0.1.6/rlax/_src/model_learning_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/moving_averages.py` & `rlax-0.1.6/rlax/_src/moving_averages.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/moving_averages_test.py` & `rlax-0.1.6/rlax/_src/moving_averages_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/mpo_ops.py` & `rlax-0.1.6/rlax/_src/mpo_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,22 +36,18 @@
 
 from absl import logging
 import chex
 import jax
 import jax.numpy as jnp
 from rlax._src import base
 
-# This op is not in the list of officially supported ops because the jax team
-# have not fully tested it, but it works nonetheless so we add and use it.
-# TODO(b/160450576): Remove when this op is officially supported.
-jax.interpreters.pxla.multi_host_supported_collectives.add(jax.lax.pmax_p)
-
 Array = chex.Array
 Numeric = chex.Numeric
 Scalar = chex.Scalar
+ProjectionOperatorFn = Callable[[Array], Array]
 
 
 class LagrangePenalty(NamedTuple):
   # Dual variable responsible for modulating the penalty for this constraint.
   alpha: Array
   # Bound for this constraint.
   epsilon: Scalar
@@ -77,15 +73,15 @@
 
 
 def mpo_loss(
     sample_log_probs: Array,
     sample_q_values: Array,
     temperature_constraint: LagrangePenalty,
     kl_constraints: Sequence[Tuple[Array, LagrangePenalty]],
-    projection_operator: Callable[[Numeric], Numeric] = functools.partial(
+    projection_operator: ProjectionOperatorFn = functools.partial(
         jnp.clip, a_min=_EPSILON),
     policy_loss_weight: float = 1.0,
     temperature_loss_weight: float = 1.0,
     kl_loss_weight: float = 1.0,
     alpha_loss_weight: float = 1.0,
     sample_axis: int = 0,
     use_stop_gradient: bool = True,
@@ -178,15 +174,15 @@
       kl_loss=kl_loss, alpha_loss=alpha_loss, normalized_weights=norm_weights,
       num_samples=num_samples)
 
 
 def mpo_compute_weights_and_temperature_loss(
     sample_q_values: Array,
     temperature_constraint: LagrangePenalty,
-    projection_operator: Callable[[Numeric], Numeric],
+    projection_operator: ProjectionOperatorFn,
     sample_axis: int = 0,
 ) -> Tuple[Array, Array, Scalar]:
   """Computes the weights and temperature loss for MPO.
 
   The E-Step computes a non-parameteric sample-based approximation of the
   current policy by reweighting the state-action value function.
 
@@ -245,15 +241,15 @@
   norm_weights = weights / jnp.sum(weights, axis=sample_axis, keepdims=True)
 
   return temperature_loss, norm_weights, n_action_samples
 
 
 def compute_parametric_kl_penalty_and_dual_loss(
     kl_constraints: Sequence[Tuple[Array, LagrangePenalty]],
-    projection_operator: Callable[[Numeric], Numeric],
+    projection_operator: ProjectionOperatorFn,
     use_stop_gradient: bool = True,
 ) -> Tuple[Array, Array]:
   """Optimize hard KL constraints between the current and previous policies."""
   for kl, penalty in kl_constraints:
     chex.assert_rank(penalty.epsilon, 0)
     chex.assert_type([kl, penalty.alpha, penalty.epsilon], float)
 
@@ -268,15 +264,15 @@
 
 
 def vmpo_loss(
     sample_log_probs: Array,
     advantages: Array,
     temperature_constraint: LagrangePenalty,
     kl_constraints: Sequence[Tuple[Array, LagrangePenalty]],
-    projection_operator: Callable[[Numeric], Numeric] = functools.partial(
+    projection_operator: ProjectionOperatorFn = functools.partial(
         jnp.clip, a_min=_EPSILON),
     restarting_weights: Optional[Array] = None,
     importance_weights: Optional[Array] = None,
     top_k_fraction: float = 0.5,
     policy_loss_weight: float = 1.0,
     temperature_loss_weight: float = 1.0,
     kl_loss_weight: float = 1.0,
@@ -380,15 +376,15 @@
 
 def get_top_k_weights(
     top_k_fraction: float,
     restarting_weights: Array,
     scaled_advantages: Array,
     axis_name: Optional[str] = None,
     use_stop_gradient: bool = True,
-):
+) -> Array:
   """Get the weights for the top top_k_fraction of advantages.
 
   Args:
     top_k_fraction: The fraction of weights to use.
     restarting_weights: Restarting weights, shape E*, 0 means that this step is
       the start of a new episode and we ignore losses at this step because the
       agent cannot influence these.
@@ -439,19 +435,19 @@
 
 
 def vmpo_compute_weights_and_temperature_loss(
     advantages: Array,
     restarting_weights: Array,
     importance_weights: Array,
     temperature_constraint: LagrangePenalty,
-    projection_operator: Callable[[Numeric], Numeric],
+    projection_operator: ProjectionOperatorFn,
     top_k_fraction: float,
     axis_name: Optional[str] = None,
     use_stop_gradient: bool = True,
-) -> Tuple[Scalar, Array, Scalar]:
+) -> Tuple[Array, Array, Array]:
   """Computes the weights and temperature loss for V-MPO.
 
   Args:
     advantages: Advantages for the E-step. Shape E*.
     restarting_weights: Restarting weights, 0 means that this
       step is the start of a new episode and we ignore losses at this step
       because the agent cannot influence these. Shape E*.
@@ -521,15 +517,15 @@
 
   return temperature_loss, normalized_weights, num_samples
 
 
 def kl_constraint_loss(
     kl: Array,
     penalty: LagrangePenalty,
-    projection_operator: Callable[[Numeric], Numeric],
+    projection_operator: ProjectionOperatorFn,
     use_stop_gradient: bool = True,
 ) -> Tuple[Array, Array, Array]:
   """Implements a hard KL constraint.
 
   The optimization proceeds in two phases. First, we optimize the weighting
   term `alpha` keeping the KL constant and then we optimize the KL keeping
   `alpha` constant. Each phase is implemented by appropriately using a
@@ -555,15 +551,15 @@
     of computation. `clipped_alpha` is the clipped lagrangian multiplier `alpha`
     that is learnt.
   """
   chex.assert_type([kl, penalty.alpha, penalty.epsilon], float)
 
   alpha = projection_operator(penalty.alpha)
   alpha_constant = jax.lax.select(
-      use_stop_gradient, jax.lax.stop_gradient(penalty.alpha), penalty.alpha)
+      use_stop_gradient, jax.lax.stop_gradient(alpha), alpha)
 
   # First step: Optimize w.r.t. alphas
   alpha_loss = alpha * (
       penalty.epsilon -
       jax.lax.select(use_stop_gradient, jax.lax.stop_gradient(kl), kl))
 
   # Second step: KL loss.
@@ -615,8 +611,7 @@
     kl_loss = all_sum(kl_loss * restarting_weights) / num_samples
     alpha_loss = all_sum(alpha_loss * restarting_weights) / num_samples
   else:
     # No M-step constraint.
     kl_loss = jnp.asarray(0.0)
     alpha_loss = jnp.asarray(0.0)
   return kl_loss, alpha_loss
-
```

### Comparing `rlax-0.1.5/rlax/_src/mpo_ops_test.py` & `rlax-0.1.6/rlax/_src/mpo_ops_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
   s_tm1 = jax.random.normal(
       next(key_seq), (TIME_DIM, BATCH_DIM, ACTION_DIM), jnp.float32)
   online_params = init_fn(next(key_seq), s_tm1)
   return dict(
       online=online_params,
       target=online_params,
       mpo=dict(
-          temperature=_INIT_TEMPERATURE,
+          temperature=jnp.array(_INIT_TEMPERATURE),
           alpha_mean=_INIT_ALPHA_MEAN,
           alpha_covariance=_INIT_ALPHA_COVARIANCE),
   )
 
 
 def _mock_outputs(online_params, target_params, key, target_name):
   """Returns mock network outputs."""
@@ -365,15 +365,15 @@
   def test_e_step_stop_gradient(
       self, e_step_fn, additional_inputs, sample_dimension):
     """Tests no gradients flow through `weights` in the E-Step."""
     # Target has shape [NUM_SAMPLES, T, B] => [1, 1, 1]
     target = jnp.array([[3]], jnp.float32)
     if sample_dimension:
       target = jnp.expand_dims(target, axis=0)
-    temperature = 0.1
+    temperature = jnp.array(0.1)
     # pylint: disable=g-long-lambda
     def mean_weights_fn(target_, temperature_):
       temperature_constraint = mpo_ops.LagrangePenalty(
           temperature_, _EPSILON_BOUND)
       _, weights, _ = e_step_fn(
           target_, temperature_constraint=temperature_constraint,
           projection_operator=_PROJECTION_OPERATOR,
@@ -464,15 +464,15 @@
        'expected_temperature_loss': 1.0 + _EPSILON_BOUND},
   )
   def test_restarting_weights(
       self, advantages, restarting_weights, expected_temperature_loss):
     """Test that calculation is correct if restarting weight is set to 0."""
     temperature_loss, _, _ = mpo_ops.vmpo_compute_weights_and_temperature_loss(
         advantages, restarting_weights, np.ones_like(restarting_weights),
-        mpo_ops.LagrangePenalty(1.0, _EPSILON_BOUND),
+        mpo_ops.LagrangePenalty(jnp.array(1.0), _EPSILON_BOUND),
         functools.partial(np.clip, a_min=1e-8, a_max=None), 1.0)
     self.assertAlmostEqual(
         temperature_loss, expected_temperature_loss, places=4)
 
   @parameterized.parameters(
       # When the top k fraction is 1.0 all of the weights should be 1
       {'top_k_fraction': 1.0,
@@ -512,15 +512,15 @@
                                      math.log(2.0) + _EPSILON_BOUND)},
   )
   def test_importance_weights(
       self, advantages, importance_weights, expected_temperature_loss):
     """Test that importance weights have the correct effect."""
     temperature_loss, _, _ = mpo_ops.vmpo_compute_weights_and_temperature_loss(
         advantages, np.ones_like(importance_weights), importance_weights,
-        mpo_ops.LagrangePenalty(1.0, _EPSILON_BOUND),
+        mpo_ops.LagrangePenalty(jnp.array(1.0), _EPSILON_BOUND),
         functools.partial(np.clip, a_min=1e-8, a_max=None), 1.0)
     self.assertAlmostEqual(
         temperature_loss, expected_temperature_loss, places=4)
 
   @parameterized.parameters({'per_dimension': True}, {'per_dimension': False})
   def test_mpo_input_axis_order_equivalence(self, per_dimension):
     """Test loss functions are equivalent regardless of axis order."""
```

### Comparing `rlax-0.1.5/rlax/_src/multistep.py` & `rlax-0.1.6/rlax/_src/multistep.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/multistep_test.py` & `rlax-0.1.6/rlax/_src/multistep_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/nested_updates.py` & `rlax-0.1.6/rlax/_src/nested_updates.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/nested_updates_test.py` & `rlax-0.1.6/rlax/_src/nested_updates_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/nonlinear_bellman.py` & `rlax-0.1.6/rlax/_src/nonlinear_bellman.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/nonlinear_bellman_test.py` & `rlax-0.1.6/rlax/_src/nonlinear_bellman_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/policy_gradients.py` & `rlax-0.1.6/rlax/_src/policy_gradients.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Policy gradient algorithms directly update the policy of an agent based on
 a stochatic estimate of the direction of steepest ascent in a score function
 representing the expected return of that policy. This subpackage provides a
 number of utility functions for implementing policy gradient algorithms for
 discrete and continuous policies.
 """
 
-from typing import Optional
+from typing import Optional, Tuple
 import chex
 import jax
 import jax.numpy as jnp
 from rlax._src import distributions
 from rlax._src import losses
 
 Array = chex.Array
@@ -139,15 +139,15 @@
 
   entropy_per_timestep = distributions.softmax().entropy(logits_t)
   return -jnp.mean(entropy_per_timestep * w_t)
 
 
 def _compute_advantages(logits_t: Array,
                         q_t: Array,
-                        use_stop_gradient=True) -> Array:
+                        use_stop_gradient=True) -> Tuple[Array, Array]:
   """Computes summed advantage using logits and action values."""
   policy_t = jax.nn.softmax(logits_t, axis=1)
 
   # Avoid computing gradients for action_values.
   q_t = jax.lax.select(use_stop_gradient, jax.lax.stop_gradient(q_t), q_t)
   baseline_t = jnp.sum(policy_t * q_t, axis=1)
```

### Comparing `rlax-0.1.5/rlax/_src/policy_gradients_test.py` & `rlax-0.1.6/rlax/_src/policy_gradients_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/policy_targets.py` & `rlax-0.1.6/rlax/_src/policy_targets.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/policy_targets_test.py` & `rlax-0.1.6/rlax/_src/policy_targets_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/pop_art.py` & `rlax-0.1.6/rlax/_src/pop_art.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/pop_art_test.py` & `rlax-0.1.6/rlax/_src/pop_art_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/test_utils.py` & `rlax-0.1.6/rlax/_src/test_utils.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/transforms.py` & `rlax-0.1.6/rlax/_src/transforms.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/transforms_test.py` & `rlax-0.1.6/rlax/_src/transforms_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/tree_util.py` & `rlax-0.1.6/rlax/_src/tree_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     on_false: a nested structure identical to `on_true`.
 
   Returns:
     the selected nested structure.
   """
   if tree_structure(on_true) != tree_structure(on_false):
     raise ValueError('The two branches must have the same structure.')
-  return jax.tree_util.tree_map(lambda x, y: jax.lax.select(pred, x, y),
-                                     on_true, on_false)
+  return jax.tree_util.tree_map(
+      lambda x, y: jax.lax.select(pred, x, y), on_true, on_false
+  )
 
 
 def tree_map_zipped(fn: Callable[..., Any], nests: Sequence[Any]):
   """Map a function over a list of identical nested structures.
 
   Args:
     fn: the function to map; must have arity equal to `len(list_of_nests)`.
@@ -142,15 +143,15 @@
   """
   pfn = functools.partial(fn, **unmapped_kwargs)
   def _wrapped(*args):
     return jax.tree_map(pfn, *args)
   return _wrapped
 
 
-def transpose_last_axis_to_first(tree: Array):
+def transpose_last_axis_to_first(tree: chex.ArrayTree) -> chex.ArrayTree:
   """Function to transpose the last axis to be first for all leaves in a pytree.
 
   This function will transpose the last axis to the front for all leaves in a
   pytree; each leaf with shape [D_1, ..., D_{n-1}, D_n] will have shape
   [D_n, D_1, ..., D_{n-1}].
 
   Args:
@@ -160,15 +161,15 @@
     tree: the transposed output tree.
   """
   def _transpose(tree):
     return jnp.transpose(tree, [tree.ndim - 1] + list(range(tree.ndim - 1)))
   return tree_fn(_transpose)(tree)
 
 
-def transpose_first_axis_to_last(tree: Array):
+def transpose_first_axis_to_last(tree: chex.ArrayTree) -> chex.ArrayTree:
   """Function to transpose the first axis to be last for all leaves in a pytree.
 
   This function will transpose the first axis to the last dim of all leaves in a
   pytree; each leaf with shape [D_1, D_2, ..., D_n] will have shape
   [D_2, ..., D_n, D_1].
 
   Args:
```

### Comparing `rlax-0.1.5/rlax/_src/tree_util_test.py` & `rlax-0.1.6/rlax/_src/tree_util_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,21 +51,21 @@
   def test_tree_map_zipped_empty(self):
     outputs = tree_util.tree_map_zipped(lambda *args: jnp.concatenate(args), [])
     self.assertEmpty(outputs)
 
   def test_select_true(self):
     on_true = ((jnp.zeros(3,),), jnp.zeros(4,))
     on_false = ((jnp.ones(3,),), jnp.ones(4,))
-    output = tree_util.tree_select(True, on_true, on_false)
+    output = tree_util.tree_select(jnp.array(True), on_true, on_false)
     chex.assert_tree_all_close(output, on_true)
 
   def test_select_false(self):
     on_true = ((jnp.zeros(3,),), jnp.zeros(4,))
     on_false = ((jnp.ones(3,),), jnp.ones(4,))
-    output = tree_util.tree_select(False, on_true, on_false)
+    output = tree_util.tree_select(jnp.array(False), on_true, on_false)
     chex.assert_tree_all_close(output, on_false)
 
   def test_tree_split_leaves(self):
     t = {
         'a0': np.zeros(3),
         'd': {
             'a1': np.arange(3),
```

### Comparing `rlax-0.1.5/rlax/_src/value_learning.py` & `rlax-0.1.6/rlax/_src/value_learning.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/value_learning_test.py` & `rlax-0.1.6/rlax/_src/value_learning_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/vtrace.py` & `rlax-0.1.6/rlax/_src/vtrace.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/_src/vtrace_test.py` & `rlax-0.1.6/rlax/_src/vtrace_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax/rlax_test.py` & `rlax-0.1.6/rlax/rlax_test.py`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/rlax.egg-info/PKG-INFO` & `rlax-0.1.6/rlax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rlax
-Version: 0.1.5
+Version: 0.1.6
 Summary: A library of reinforcement learning building blocks in JAX.
 Home-page: https://github.com/deepmind/rlax
 Author: DeepMind
 Author-email: rlax-dev@google.com
 License: Apache 2.0
 Keywords: reinforcement-learning python machine learning
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RLax
 
 ![CI status](https://github.com/deepmind/rlax/workflows/ci/badge.svg)
 ![docs](https://readthedocs.org/projects/rlax/badge/?version=latest)
```

### Comparing `rlax-0.1.5/rlax.egg-info/SOURCES.txt` & `rlax-0.1.6/rlax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rlax-0.1.5/setup.py` & `rlax-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     keywords='reinforcement-learning python machine learning',
     packages=find_namespace_packages(exclude=['*_test.py']),
     install_requires=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements.txt')),
     tests_require=_parse_requirements(
         os.path.join(_CURRENT_DIR, 'requirements', 'requirements-test.txt')),
     zip_safe=False,  # Required for full installation.
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: POSIX :: Linux',
         'Operating System :: Microsoft :: Windows',
```

