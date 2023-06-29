# Comparing `tmp/squlearn-0.1.0.tar.gz` & `tmp/squlearn-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squlearn-0.1.0.tar", last modified: Tue Jun  6 12:39:43 2023, max compression
+gzip compressed data, was "squlearn-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `squlearn-0.1.0.tar` & `squlearn-0.2.0.tar`

### file list

```diff
@@ -1,90 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.278775 squlearn-0.1.0/
--rw-rw-rw-   0        0        0    11622 2023-06-01 08:52:55.000000 squlearn-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0    17318 2023-06-06 12:39:43.277776 squlearn-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3313 2023-06-06 12:37:20.000000 squlearn-0.1.0/README.md
--rw-rw-rw-   0        0        0     1399 2023-06-06 12:34:22.000000 squlearn-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 12:39:43.278775 squlearn-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.123774 squlearn-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.137781 squlearn-0.1.0/src/squlearn/
--rw-rw-rw-   0        0        0       21 2023-06-06 12:17:41.000000 squlearn-0.1.0/src/squlearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.151774 squlearn-0.1.0/src/squlearn/expectation_operator/
--rw-rw-rw-   0        0        0      884 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/__init__.py
--rw-rw-rw-   0        0        0     7277 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_base.py
--rw-rw-rw-   0        0        0    13758 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_derivatives.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.165776 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/__init__.py
--rw-rw-rw-   0        0        0     2016 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/custom_expectation_operator.py
--rw-rw-rw-   0        0        0     3663 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/ising_hamiltonian.py
--rw-rw-rw-   0        0        0     1556 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_amplitude.py
--rw-rw-rw-   0        0        0     2043 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_pauli.py
--rw-rw-rw-   0        0        0     1944 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_amplitudes.py
--rw-rw-rw-   0        0        0     1544 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_paulis.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.178775 squlearn-0.1.0/src/squlearn/feature_map/
--rw-rw-rw-   0        0        0     1390 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/__init__.py
--rw-rw-rw-   0        0        0     5918 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_base.py
--rw-rw-rw-   0        0        0    18353 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_derivatives.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.198775 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/__init__.py
--rw-rw-rw-   0        0        0     4972 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/cheb_pqc.py
--rw-rw-rw-   0        0        0     2751 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/cheb_rx.py
--rw-rw-rw-   0        0        0     3424 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/chebyshev_tower.py
--rw-rw-rw-   0        0        0     7194 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/highdim_feature_map.py
--rw-rw-rw-   0        0        0     3630 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/hz_crxcrycrz.py
--rw-rw-rw-   0        0        0     3800 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/qek_feature_map.py
--rw-rw-rw-   0        0        0     2330 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/qiskit_z_feature_map.py
--rw-rw-rw-   0        0        0     3199 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/yz_cx_feature_map.py
--rw-rw-rw-   0        0        0     1774 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/zfeaturemap_cx.py
--rw-rw-rw-   0        0        0   103025 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/layered_feature_map.py
--rw-rw-rw-   0        0        0     9545 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/pruned_feature_map.py
--rw-rw-rw-   0        0        0     4432 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/feature_map/transpiled_feature_map.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.200776 squlearn-0.1.0/src/squlearn/kernel/
--rw-rw-rw-   0        0        0        0 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.208782 squlearn-0.1.0/src/squlearn/kernel/matrix/
--rw-rw-rw-   0        0        0      253 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/matrix/__init__.py
--rw-rw-rw-   0        0        0     5831 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/matrix/fidelity_kernel.py
--rw-rw-rw-   0        0        0     4150 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/matrix/kernel_matrix_base.py
--rw-rw-rw-   0        0        0    14215 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.224777 squlearn-0.1.0/src/squlearn/kernel/ml/
--rw-rw-rw-   0        0        0      236 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/__init__.py
--rw-rw-rw-   0        0        0      273 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/helper_functions.py
--rw-rw-rw-   0        0        0      367 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/kernel_ml_base.py
--rw-rw-rw-   0        0        0     2060 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/kernel_util.py
--rw-rw-rw-   0        0        0     1055 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/qgpc.py
--rw-rw-rw-   0        0        0     4785 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/qgpr.py
--rw-rw-rw-   0        0        0     4428 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/qkrr.py
--rw-rw-rw-   0        0        0     1024 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/qsvc.py
--rw-rw-rw-   0        0        0     1018 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/ml/qsvr.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.239776 squlearn-0.1.0/src/squlearn/kernel/optimization/
--rw-rw-rw-   0        0        0      370 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/__init__.py
--rw-rw-rw-   0        0        0      241 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/kernel_loss_base.py
--rw-rw-rw-   0        0        0      597 2023-06-01 08:52:55.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/kernel_optimization_base.py
--rw-rw-rw-   0        0        0     1637 2023-06-01 08:52:55.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/kernel_optimizer.py
--rw-rw-rw-   0        0        0     1425 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/negative_log_likelihood.py
--rw-rw-rw-   0        0        0     1389 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/kernel/optimization/target_alignment.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.248775 squlearn-0.1.0/src/squlearn/optimizers/
--rw-rw-rw-   0        0        0      470 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/optimizers/__init__.py
--rw-rw-rw-   0        0        0     4861 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/optimizers/adam.py
--rw-rw-rw-   0        0        0     4638 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/optimizers/approximated_gradients.py
--rw-rw-rw-   0        0        0     1890 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/optimizers/optimizer_base.py
--rw-rw-rw-   0        0        0     3880 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/optimizers/optimizers_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.264775 squlearn-0.1.0/src/squlearn/qnn/
--rw-rw-rw-   0        0        0       43 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/__init__.py
--rw-rw-rw-   0        0        0     8692 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/barren_plateau_analysis.py
--rw-rw-rw-   0        0        0     4317 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/base_qnn.py
--rw-rw-rw-   0        0        0     7687 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/loss.py
--rw-rw-rw-   0        0        0    42194 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/qnn.py
--rw-rw-rw-   0        0        0     6252 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/qnnc.py
--rw-rw-rw-   0        0        0     5505 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/qnnr.py
--rw-rw-rw-   0        0        0    22377 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/qnn/training.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.275777 squlearn-0.1.0/src/squlearn/util/
--rw-rw-rw-   0        0        0       56 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/util/__init__.py
--rw-rw-rw-   0        0        0     2840 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/util/data_preprocessing.py
--rw-rw-rw-   0        0        0     9870 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/util/evaluate_opflow.py
--rw-rw-rw-   0        0        0    42010 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/util/executor.py
--rw-rw-rw-   0        0        0     5762 2023-05-17 07:30:25.000000 squlearn-0.1.0/src/squlearn/util/quantum_fisher.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:39:43.145774 squlearn-0.1.0/src/squlearn.egg-info/
--rw-rw-rw-   0        0        0    17318 2023-06-06 12:39:43.000000 squlearn-0.1.0/src/squlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3438 2023-06-06 12:39:43.000000 squlearn-0.1.0/src/squlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 12:39:43.000000 squlearn-0.1.0/src/squlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      158 2023-06-06 12:39:43.000000 squlearn-0.1.0/src/squlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 12:39:43.000000 squlearn-0.1.0/src/squlearn.egg-info/top_level.txt
+-rw-r--r--   0        0        0     2076 2023-06-29 13:08:18.471675 squlearn-0.2.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      528 2023-06-29 13:08:18.471675 squlearn-0.2.0/.github/workflows/format.yml
+-rw-r--r--   0        0        0      678 2023-06-29 13:08:18.471675 squlearn-0.2.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3159 2023-06-29 13:08:18.471675 squlearn-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11421 2023-06-29 13:08:18.471675 squlearn-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1293 2023-06-29 13:08:18.471675 squlearn-0.2.0/README.md
+-rw-r--r--   0        0        0      632 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/Makefile
+-rw-r--r--   0        0        0      226 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/README.md
+-rw-r--r--   0        0        0     2301 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      644 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/index.rst
+-rw-r--r--   0        0        0      765 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/make.bat
+-rw-r--r--   0        0        0     3004 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/modules/classes.rst
+-rw-r--r--   0        0        0      169 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/templates/class.rst
+-rw-r--r--   0        0        0      495 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/templates/class_with_call.rst
+-rw-r--r--   0        0        0      179 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/templates/function.rst
+-rw-r--r--   0        0        0     1006 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/tutorials/install.rst
+-rw-r--r--   0        0        0     1812 2023-06-29 13:08:18.471675 squlearn-0.2.0/docs/tutorials/operators.rst
+-rw-r--r--   0        0        0      329 2023-06-29 13:08:18.475675 squlearn-0.2.0/docs/tutorials/pqk.rst
+-rw-r--r--   0        0        0      235 2023-06-29 13:08:18.475675 squlearn-0.2.0/docs/tutorials/use_executor.rst
+-rw-r--r--   0        0        0       24 2023-06-29 13:08:18.475675 squlearn-0.2.0/examples/executor/.gitignore
+-rw-r--r--   0        0        0    14688 2023-06-29 13:08:18.475675 squlearn-0.2.0/examples/executor/example_executor.ipynb
+-rw-r--r--   0        0        0    98077 2023-06-29 13:08:18.475675 squlearn-0.2.0/examples/feature_maps/layered_feature_map.ipynb
+-rw-r--r--   0        0        0    24924 2023-06-29 13:08:18.475675 squlearn-0.2.0/examples/feature_maps/pruning_example.ipynb
+-rw-r--r--   0        0        0   383088 2023-06-29 13:08:18.475675 squlearn-0.2.0/examples/feature_maps/various_feature_maps.ipynb
+-rw-r--r--   0        0        0    23355 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/example_fidelity_kernel.ipynb
+-rw-r--r--   0        0        0   216577 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/example_projected_kernel.ipynb
+-rw-r--r--   0        0        0    43993 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/example_regularization_mitigation.ipynb
+-rw-r--r--   0        0        0    77370 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/qgpc_workflow.ipynb
+-rw-r--r--   0        0        0    59611 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/qgpr_optimization_workflow.ipynb
+-rw-r--r--   0        0        0    73223 2023-06-29 13:08:18.479675 squlearn-0.2.0/examples/kernel/qgpr_workflow.ipynb
+-rw-r--r--   0        0        0   209407 2023-06-29 13:08:18.483675 squlearn-0.2.0/examples/qnn/classification_example.ipynb
+-rw-r--r--   0        0        0   207500 2023-06-29 13:08:18.483675 squlearn-0.2.0/examples/qnn/example_adam.ipynb
+-rw-r--r--   0        0        0    48388 2023-06-29 13:08:18.483675 squlearn-0.2.0/examples/qnn/example_minibatch.ipynb
+-rw-r--r--   0        0        0   104582 2023-06-29 13:08:18.483675 squlearn-0.2.0/examples/qnn/example_shot_adjusting.ipynb
+-rw-r--r--   0        0        0    19425 2023-06-29 13:08:18.483675 squlearn-0.2.0/examples/qnn/expectation_operator.ipynb
+-rw-r--r--   0        0        0   331594 2023-06-29 13:08:18.487675 squlearn-0.2.0/examples/qnn/regression_example.ipynb
+-rw-r--r--   0        0        0   420820 2023-06-29 13:08:18.491675 squlearn-0.2.0/examples/qnn/regression_example_layered_fm.ipynb
+-rw-r--r--   0        0        0   220954 2023-06-29 13:08:18.491675 squlearn-0.2.0/examples/qnn/regression_with_variance.ipynb
+-rw-r--r--   0        0        0    57473 2023-06-29 13:08:18.491675 squlearn-0.2.0/examples/tutorials/kernel_regression.ipynb
+-rw-r--r--   0        0        0     3299 2023-06-29 13:08:18.491675 squlearn-0.2.0/examples/tutorials/pipeline_example.ipynb
+-rw-r--r--   0        0        0     5910 2023-06-29 13:08:18.491675 squlearn-0.2.0/examples/tutorials/qml_sklearn_interaction.ipynb
+-rw-r--r--   0        0        0     1573 2023-06-29 13:08:18.491675 squlearn-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      339 2023-06-29 13:08:18.491675 squlearn-0.2.0/src/squlearn/__init__.py
+-rw-r--r--   0        0        0      667 2023-06-29 13:08:18.491675 squlearn-0.2.0/src/squlearn/expectation_operator/__init__.py
+-rw-r--r--   0        0        0     8643 2023-06-29 13:08:18.491675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_base.py
+-rw-r--r--   0        0        0    13414 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_derivatives.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/__init__.py
+-rw-r--r--   0        0        0     2848 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/custom_expectation_operator.py
+-rw-r--r--   0        0        0     5044 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/ising_hamiltonian.py
+-rw-r--r--   0        0        0     2031 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_pauli.py
+-rw-r--r--   0        0        0     2206 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_probability.py
+-rw-r--r--   0        0        0     2735 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_paulis.py
+-rw-r--r--   0        0        0     2635 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_probabilities.py
+-rw-r--r--   0        0        0     1030 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/__init__.py
+-rw-r--r--   0        0        0     5644 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_base.py
+-rw-r--r--   0        0        0    17896 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_derivatives.py
+-rw-r--r--   0        0        0        0 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/cheb_pqc.py
+-rw-r--r--   0        0        0     2669 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/cheb_rx.py
+-rw-r--r--   0        0        0     3307 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/chebyshev_tower.py
+-rw-r--r--   0        0        0     7005 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/highdim_feature_map.py
+-rw-r--r--   0        0        0     3533 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/hz_crxcrycrz.py
+-rw-r--r--   0        0        0     3701 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/qek_feature_map.py
+-rw-r--r--   0        0        0     2263 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/qiskit_z_feature_map.py
+-rw-r--r--   0        0        0     3109 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/yz_cx_feature_map.py
+-rw-r--r--   0        0        0     1719 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/zfeaturemap_cx.py
+-rw-r--r--   0        0        0   100889 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/layered_feature_map.py
+-rw-r--r--   0        0        0     9301 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/pruned_feature_map.py
+-rw-r--r--   0        0        0     4301 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/feature_map/transpiled_feature_map.py
+-rw-r--r--   0        0        0       83 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/__init__.py
+-rw-r--r--   0        0        0      161 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/matrix/__init__.py
+-rw-r--r--   0        0        0     5810 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/matrix/fidelity_kernel.py
+-rw-r--r--   0        0        0     4022 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/matrix/kernel_matrix_base.py
+-rw-r--r--   0        0        0    13982 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py
+-rw-r--r--   0        0        0      168 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/__init__.py
+-rw-r--r--   0        0        0     2021 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/kernel_util.py
+-rw-r--r--   0        0        0     1001 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/qgpc.py
+-rw-r--r--   0        0        0     4182 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/qgpr.py
+-rw-r--r--   0        0        0     3856 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/qkrr.py
+-rw-r--r--   0        0        0     1010 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/qsvc.py
+-rw-r--r--   0        0        0     1005 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/ml/qsvr.py
+-rw-r--r--   0        0        0      190 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/optimization/__init__.py
+-rw-r--r--   0        0        0      251 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/optimization/kernel_loss_base.py
+-rw-r--r--   0        0        0      593 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/optimization/kernel_optimization_base.py
+-rw-r--r--   0        0        0     1430 2023-06-29 13:08:18.495675 squlearn-0.2.0/src/squlearn/kernel/optimization/kernel_optimizer.py
+-rw-r--r--   0        0        0     1406 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/kernel/optimization/negative_log_likelihood.py
+-rw-r--r--   0        0        0     1172 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/kernel/optimization/target_alignment.py
+-rw-r--r--   0        0        0      279 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/optimizers/__init__.py
+-rw-r--r--   0        0        0     5265 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/optimizers/adam.py
+-rw-r--r--   0        0        0     4520 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/optimizers/approximated_gradients.py
+-rw-r--r--   0        0        0     1815 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/optimizers/optimizer_base.py
+-rw-r--r--   0        0        0     3772 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/optimizers/optimizers_wrapper.py
+-rw-r--r--   0        0        0      351 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/__init__.py
+-rw-r--r--   0        0        0     8450 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/barren_plateau_analysis.py
+-rw-r--r--   0        0        0     3881 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/base_qnn.py
+-rw-r--r--   0        0        0    17294 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/loss.py
+-rw-r--r--   0        0        0    41324 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/qnn.py
+-rw-r--r--   0        0        0     6030 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/qnnc.py
+-rw-r--r--   0        0        0     5201 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/qnnr.py
+-rw-r--r--   0        0        0    17973 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/qnn/training.py
+-rw-r--r--   0        0        0       55 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/util/__init__.py
+-rw-r--r--   0        0        0     2747 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/util/data_preprocessing.py
+-rw-r--r--   0        0        0    11749 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/util/evaluate_opflow.py
+-rw-r--r--   0        0        0    42067 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/util/executor.py
+-rw-r--r--   0        0        0     5628 2023-06-29 13:08:18.499675 squlearn-0.2.0/src/squlearn/util/quantum_fisher.py
+-rw-r--r--   0        0        0     1331 2023-06-29 13:08:18.499675 squlearn-0.2.0/tests/qnn/test_training.py
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 squlearn-0.2.0/PKG-INFO
```

### Comparing `squlearn-0.1.0/LICENSE.txt` & `squlearn-0.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 Fraunhofer Institute for Manufacturing Engineering and Automation IPA and its contributors.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 Fraunhofer Institute for Manufacturing Engineering and Automation IPA and its contributors.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_base.py` & `squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,209 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-
-from qiskit.quantum_info import Pauli, SparsePauliOp
-from qiskit.circuit import ParameterExpression, ParameterVector
-from qiskit.opflow import ListOp, PauliOp, PauliSumOp
-from qiskit.opflow.gradients.derivative_base import _coeff_derivative
-from qiskit.opflow import SummedOp, Zero, One
-from qiskit.opflow import OperatorBase
-from qiskit.opflow import TensoredOp, OperatorStateFn, StateFn
-from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
-
-
-class ExpectationOperatorBase:
-    """Empty parent class for a Expectation operator."""
-
-    def __init__(self, num_qubits: int) -> None:
-        """Initialization
-        Args:
-            number_of_qubits: Number of qubits.
-        """
-        self._num_qubits = num_qubits
-        self._num_all_qubits = num_qubits
-        self._qubit_map = np.linspace(0, num_qubits - 1, num_qubits, dtype=int)
-
-    def set_map(self, qubit_map, num_all_qubits):
-        self._qubit_map = qubit_map
-        self._num_all_qubits = num_all_qubits
-
-    @property
-    def num_parameters(self):
-        """
-        Returns:
-            the number of free parameters in the expectation operator.
-        """
-        return 0
-
-    @property
-    def num_qubits(self):
-        """
-        Returns:
-            the number of free parameters in the expectation operator.
-        """
-        return self._num_qubits
-
-    def get_operator(self, parameters: Union[ParameterVector, np.ndarray]):
-        """Returns the PauliOp expression of the expectation operator.
-        Args
-            param: ParameterVector.
-        Returns:
-            Return PauliOp expression of the expectation operator.
-        """
-
-        # Return as measurement operator!
-        return StateFn(self.get_pauli_mapped(parameters), is_measurement=True)
-
-    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
-        return PauliOp(Pauli("I" * self._num_all_qubits))
-
-    def get_pauli_mapped(self, parameters: Union[ParameterVector, np.ndarray]):
-        def map_expectation_op(operator: OperatorBase) -> OperatorBase:
-            """ """
-
-            # We reached the Composed object or the wavefunction
-            if isinstance(operator, PauliOp):
-                blank = Pauli("I" * self._num_all_qubits)
-                for i, p in enumerate(operator.primitive):
-                    blank[self._qubit_map[i]] = p
-                return PauliOp(blank, operator.coeff)
-            elif isinstance(operator, PauliSumOp):
-                PauliList = []
-                for i, p in enumerate(operator.primitive.paulis):
-                    blank = Pauli("I" * self._num_all_qubits)
-                    for j, op in enumerate(p):
-                        blank[self._qubit_map[j]] = op
-                    PauliList.append(PauliOp(blank, coeff=operator.coeffs[i]))
-                return_op = sum(PauliList)
-                return_op._coeff = operator.coeff
-                return return_op
-            elif isinstance(operator, ListOp):
-                # List object reached, recursive call of the function
-                op_list = [map_expectation_op(op) for op in operator.oplist]
-
-                # Sort out the Zero @ One terms
-                if operator.combo_fn == ListOp.default_combo_fn:  # If using default
-                    return ListOp(
-                        oplist=[op for op in op_list if op != ~Zero @ One],
-                        coeff=operator.coeff,
-                    )
-                elif isinstance(operator, SummedOp):
-                    return SummedOp(
-                        oplist=[op for op in op_list if op != ~Zero @ One],
-                        coeff=operator.coeff,
-                    )
-                elif isinstance(operator, TensoredOp):
-                    return TensoredOp(
-                        oplist=[op for op in op_list if op != ~Zero @ One],
-                        coeff=operator.coeff,
-                    )
-                else:
-                    raise ValueError("Unknown Type in ListOp")
-            else:
-                raise ValueError("Wrong Type in operator: ", type(operator))
-
-        return map_expectation_op(self.get_pauli(parameters))
-
-    def __str__(self):
-        p = ParameterVector("p", self.num_parameters)
-        return str(self.get_pauli(p))
-
-    def __repr__(self):
-        p = ParameterVector("p", self.num_parameters)
-        return repr(self.get_pauli(p))
-
-    def __add__(self, x):
-        if not isinstance(x, ExpectationOperatorBase):
-            raise ValueError("Only the addition with other expectation operator is allowed!")
-
-        class ComposedExpectationOperator(ExpectationOperatorBase):
-            def __init__(self, op1: ExpectationOperatorBase, op2: ExpectationOperatorBase):
-                if op1.num_qubits != op2.num_qubits:
-                    raise ValueError("Number of qubits is not equal in both expectation operator.")
-
-                super().__init__(op1.num_qubits)
-
-                self._op1 = op1
-                self._op2 = op2
-
-            @property
-            def num_parameters(self) -> int:
-                """Returns the number of trainable parameters of composed expectation operator.
-                Is equal to the sum of both trainable parameters
-                """
-                return self._op1.num_parameters + self._op2.num_parameters
-
-            def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
-                paulis_op1 = self._op1.get_pauli(parameters[: self._op1.num_parameters])
-                paulis_op2 = self._op2.get_pauli(parameters[self._op1.num_parameters :])
-                return paulis_op1 + paulis_op2
-
-        return ComposedExpectationOperator(self, x)
-
-    def __mul__(self, x):
-        if not isinstance(x, ExpectationOperatorBase):
-            raise ValueError("Only the multiplication with other expectation operator is allowed!")
-
-        class MultipliedExpectationOperator(ExpectationOperatorBase):
-            def __init__(self, op1: ExpectationOperatorBase, op2: ExpectationOperatorBase):
-                if op1.num_qubits != op2.num_qubits:
-                    raise ValueError("Number of qubits is not equal in both expectation operator.")
-
-                super().__init__(op1.num_qubits)
-
-                self._op1 = op1
-                self._op2 = op2
-
-            @property
-            def num_parameters(self) -> int:
-                """Returns the number of trainable parameters of composed expectation operator.
-                Is equal to the sum of both trainable parameters
-                """
-                return self._op1.num_parameters + self._op2.num_parameters
-
-            def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
-                paulis_op1 = self._op1.get_pauli(parameters[: self._op1.num_parameters])
-                paulis_op2 = self._op2.get_pauli(parameters[self._op1.num_parameters :])
-                return (paulis_op1 @ paulis_op2).reduce().reduce()
-
-        return MultipliedExpectationOperator(self, x)
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+
+from qiskit.quantum_info import Pauli, SparsePauliOp
+from qiskit.circuit import ParameterExpression, ParameterVector
+from qiskit.opflow import ListOp, PauliOp, PauliSumOp
+from qiskit.opflow.gradients.derivative_base import _coeff_derivative
+from qiskit.opflow import SummedOp, Zero, One
+from qiskit.opflow import OperatorBase
+from qiskit.opflow import TensoredOp, OperatorStateFn, StateFn
+from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
+
+
+class ExpectationOperatorBase:
+    """Empty parent class for a Expectation operator."""
+
+    def __init__(self, num_qubits: int) -> None:
+        """Initialization
+        Args:
+            number_of_qubits: Number of qubits.
+        """
+        self._num_qubits = num_qubits
+        self._num_all_qubits = num_qubits
+        self._qubit_map = np.linspace(0, num_qubits - 1, num_qubits, dtype=int)
+
+    def set_map(self, qubit_map: Union[list, dict], num_all_qubits: int):
+        """
+        Function for setting a qubit mapping (either a dictionary or a list).
+
+        This function is necessary for evaluating expectation values on a real backend, where the
+        number of qubits in the system is larger than the number of qubits in the expectation operator.
+
+        Args:
+            qubit_map: A list or dictionary specifying which of the input qubits are mapped to the output qubits.
+            num_all_qubits: The total number of qubits in the system.
+        """
+        self._qubit_map = qubit_map
+        self._num_all_qubits = num_all_qubits
+
+    @property
+    def num_parameters(self):
+        """
+        Returns:
+            the number of free parameters in the expectation operator.
+        """
+        return 0
+
+    @property
+    def num_qubits(self):
+        """
+        Returns:
+            the number of free parameters in the expectation operator.
+        """
+        return self._num_qubits
+
+    def get_operator(self, parameters: Union[ParameterVector, np.ndarray]):
+        """Returns the PauliOp expression of the expectation operator.
+        Args
+            param: ParameterVector.
+        Returns:
+            Return PauliOp expression of the expectation operator.
+        """
+
+        # Return as measurement operator!
+        # TODO: depricate this function!
+        return StateFn(self.get_pauli_mapped(parameters), is_measurement=True)
+
+    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
+        """
+        Returns the PauliOp expression of the expectation operator.
+
+        Args:
+            parameters (Union[ParameterVector, np.ndarray]): Vector of parameters used in the operator
+
+        Returns:
+            PauliOp: Expectation operator in qiskit's PauliOp class
+        """
+        return PauliOp(Pauli("I" * self._num_all_qubits))
+
+    def get_pauli_mapped(self, parameters: Union[ParameterVector, np.ndarray]):
+        """
+        Returns the mapped PauliOp expression of the expectation operator:
+
+        Here, the previously set qubit map (set_map) is used to map the PauliOp to the correct qubits.
+
+        Args:
+            parameters (Union[ParameterVector, np.ndarray]): Vector of parameters used in the operator
+
+        Returns:
+            PauliOp: Expectation operator in qiskit's PauliOp class
+        """
+
+        def map_expectation_op(operator: OperatorBase) -> OperatorBase:
+            """ """
+
+            # We reached the Composed object or the wavefunction
+            if isinstance(operator, PauliOp):
+                blank = Pauli("I" * self._num_all_qubits)
+                for i, p in enumerate(operator.primitive):
+                    blank[self._qubit_map[i]] = p
+                return PauliOp(blank, operator.coeff)
+            elif isinstance(operator, PauliSumOp):
+                PauliList = []
+                for i, p in enumerate(operator.primitive.paulis):
+                    blank = Pauli("I" * self._num_all_qubits)
+                    for j, op in enumerate(p):
+                        blank[self._qubit_map[j]] = op
+                    PauliList.append(PauliOp(blank, coeff=operator.coeffs[i]))
+                return_op = sum(PauliList)
+                return_op._coeff = operator.coeff
+                return return_op
+            elif isinstance(operator, ListOp):
+                # List object reached, recursive call of the function
+                op_list = [map_expectation_op(op) for op in operator.oplist]
+
+                # Sort out the Zero @ One terms
+                if operator.combo_fn == ListOp.default_combo_fn:  # If using default
+                    return ListOp(
+                        oplist=[op for op in op_list if op != ~Zero @ One],
+                        coeff=operator.coeff,
+                    )
+                elif isinstance(operator, SummedOp):
+                    return SummedOp(
+                        oplist=[op for op in op_list if op != ~Zero @ One],
+                        coeff=operator.coeff,
+                    )
+                elif isinstance(operator, TensoredOp):
+                    return TensoredOp(
+                        oplist=[op for op in op_list if op != ~Zero @ One],
+                        coeff=operator.coeff,
+                    )
+                else:
+                    raise ValueError("Unknown Type in ListOp")
+            else:
+                raise ValueError("Wrong Type in operator: ", type(operator))
+
+        return map_expectation_op(self.get_pauli(parameters))
+
+    def __str__(self):
+        """Return a string representation of the ExpectationOperatorBase."""
+        p = ParameterVector("p", self.num_parameters)
+        return str(self.get_pauli(p))
+
+    def __repr__(self):
+        """Return a string representation of the ExpectationOperatorBase."""
+        p = ParameterVector("p", self.num_parameters)
+        return repr(self.get_pauli(p))
+
+    def __add__(self, x):
+        """Addition of two expectation operators."""
+        if not isinstance(x, ExpectationOperatorBase):
+            raise ValueError("Only the addition with other expectation operator is allowed!")
+
+        class ComposedExpectationOperator(ExpectationOperatorBase):
+            def __init__(self, op1: ExpectationOperatorBase, op2: ExpectationOperatorBase):
+                if op1.num_qubits != op2.num_qubits:
+                    raise ValueError("Number of qubits is not equal in both expectation operator.")
+
+                super().__init__(op1.num_qubits)
+
+                self._op1 = op1
+                self._op2 = op2
+
+            @property
+            def num_parameters(self) -> int:
+                """Returns the number of trainable parameters of composed expectation operator.
+                Is equal to the sum of both trainable parameters
+                """
+                return self._op1.num_parameters + self._op2.num_parameters
+
+            def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
+                paulis_op1 = self._op1.get_pauli(parameters[: self._op1.num_parameters])
+                paulis_op2 = self._op2.get_pauli(parameters[self._op1.num_parameters :])
+                return paulis_op1 + paulis_op2
+
+        return ComposedExpectationOperator(self, x)
+
+    def __mul__(self, x):
+        """Multiplication of two expectation operators."""
+        if not isinstance(x, ExpectationOperatorBase):
+            raise ValueError("Only the multiplication with other expectation operator is allowed!")
+
+        class MultipliedExpectationOperator(ExpectationOperatorBase):
+            def __init__(self, op1: ExpectationOperatorBase, op2: ExpectationOperatorBase):
+                if op1.num_qubits != op2.num_qubits:
+                    raise ValueError("Number of qubits is not equal in both expectation operator.")
+
+                super().__init__(op1.num_qubits)
+
+                self._op1 = op1
+                self._op2 = op2
+
+            @property
+            def num_parameters(self) -> int:
+                """Returns the number of trainable parameters of composed expectation operator.
+                Is equal to the sum of both trainable parameters
+                """
+                return self._op1.num_parameters + self._op2.num_parameters
+
+            def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
+                paulis_op1 = self._op1.get_pauli(parameters[: self._op1.num_parameters])
+                paulis_op2 = self._op2.get_pauli(parameters[self._op1.num_parameters :])
+                return (paulis_op1 @ paulis_op2).reduce().reduce()
+
+        return MultipliedExpectationOperator(self, x)
```

### Comparing `squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_derivatives.py` & `squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_derivatives.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,344 +1,344 @@
-from qiskit.circuit import ParameterVector, ParameterExpression
-from qiskit.circuit.parametervector import ParameterVectorElement
-from qiskit.opflow import StateFn, OperatorStateFn
-from qiskit.opflow import SummedOp, ListOp, PauliOp, TensoredOp, PauliSumOp
-from qiskit.opflow import Zero, One
-from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
-from qiskit.opflow.gradients.derivative_base import _coeff_derivative
-from qiskit.quantum_info import Pauli, SparsePauliOp
-from typing import Union
-import numpy as np
-
-from .expectation_operator_base import ExpectationOperatorBase
-from ..util.data_preprocessing import adjust_input
-
-
-class ExpectationOperatorDerivatives:
-    def __init__(
-        self,
-        expectation_operator: Union[ExpectationOperatorBase, list],
-        opflow_caching=True,
-    ):
-        # handling multiple Expectation_operators also done here
-
-        self.expectation_operator = expectation_operator
-
-        # Contains the OperatorMeasurement() of the expectation-operator for later replacement
-        if isinstance(self.expectation_operator, ExpectationOperatorBase):
-            # 1d output by a single expectation-operator
-            self.multiple_output = False
-            self._num_operators = 1
-            self.parameters = ParameterVector("p_op", expectation_operator.num_parameters)
-
-            opflow = self.expectation_operator.get_operator(self.parameters)
-            opflow.replace = False
-        else:
-            # multi dimensional output by multiple Expectation-operators
-            expectation_op_list = []
-            self.multiple_output = True
-            self._num_operators = len(expectation_operator)
-            try:
-                n_oper = 0
-                for op in self.expectation_operator:
-                    n_oper = n_oper + op.num_parameters
-
-                self.parameters = ParameterVector("p_op", n_oper)
-                ioff = 0
-                for op in self.expectation_operator:
-                    expectation_op_list.append(op.get_operator(self.parameters[ioff:]))
-                    ioff = ioff + op.num_parameters
-                opflow = ListOp(expectation_op_list)
-                opflow.replace = False
-            except:
-                raise ValueError("Unknown structure of the Expectation operator!")
-
-        self.opflow = opflow
-        self.opflow_cache = {}
-        self.opflow_caching = opflow_caching
-
-        if self.opflow_caching:
-            self.opflow_cache["O"] = opflow
-
-    def get_derivate(self, input: Union[str, tuple]):
-        """return the opflow structure of the wavefunction"""
-        if isinstance(input, str):
-            # todo change with replaced operator
-            if input == "I":
-                measure_op = StateFn(
-                    PauliOp(Pauli("I" * self.opflow.num_qubits)), is_measurement=True
-                )
-            elif input == "O":
-                measure_op = self.opflow
-            elif input == "OO":
-                measure_op = self.get_operator_squared()
-            elif input == "dop" or input == "Odop":
-                measure_op = self._differentiation_from_tuple(
-                    self.opflow.copy(), (self.parameters,), "O"
-                )
-            elif input == "dopdop" or input == "Odopdop":
-                measure_op = self._differentiation_from_tuple(
-                    self.opflow.copy(), (self.parameters, self.parameters), "O"
-                )
-            elif input == "OOdop":
-                measure_op = self._differentiation_from_tuple(
-                    self.get_operator_squared(), (self.parameters,), "OO"
-                )
-            elif input == "OOdopdop":
-                measure_op = self._differentiation_from_tuple(
-                    self.get_operator_squared(),
-                    (self.parameters, self.parameters),
-                    "OO",
-                )
-            else:
-                raise ValueError("Unknown string command:", input)
-
-        elif isinstance(input, tuple):
-            measure_op = self._differentiation_from_tuple(self.opflow, input, "O")
-        else:
-            raise TypeError("Input is neither string nor tuple, but:", type(input))
-
-        measure_op.replace = False
-        return measure_op
-
-    def get_differentiation_from_tuple(self, diff_tuple: tuple):
-        return self.get_derivate(diff_tuple)
-
-    def get_derivation_from_string(self, input_string: str):
-        return self.get_derivate(input_string)
-
-    def _differentiation_from_tuple(self, expectation_op, diff_tuple: tuple, expectation_op_label):
-        """Recursive routine for automatic differentiating the expectation_operator
-        Args:
-            diff_tuple : tuple containing ParameterVectors or ParameterExpressions
-        Returns:
-            The differentiated opflow expression
-        """
-        # TODO: outer function for input checking
-
-        if diff_tuple == ():
-            # Cancel the recursion by returning the opflow of the simply measured feature map
-            return expectation_op
-        else:
-            # Check if differentiating tuple is already stored in opflow_cache
-            if (
-                self.opflow_caching == True
-                and (diff_tuple, expectation_op_label) in self.opflow_cache
-            ):
-                # If stored -> return
-                return self.opflow_cache[(diff_tuple, expectation_op_label)].copy()
-            else:
-                # Recursive differentiation with the most left object
-                measure = _opflow_differentiation(
-                    self._differentiation_from_tuple(
-                        expectation_op, diff_tuple[1:], expectation_op_label
-                    ),
-                    diff_tuple[0],
-                )
-                # Store result in the opflow_cache
-                if self.opflow_caching == True:
-                    self.opflow_cache[(diff_tuple, expectation_op_label)] = measure
-                return measure
-
-    def get_operator_squared(self):
-        "Builds and caches the squared form of the expectation operator OO=O^2"
-        if self.opflow_caching == True and "OO" in self.opflow_cache:
-            return self.opflow_cache["OO"].copy()
-        else:
-            # Get the operator and store it in ListOp structure
-            if not isinstance(self.opflow, ListOp):
-                op_list = ListOp([self.opflow])
-            else:
-                op_list = self.opflow
-
-            # Loop through the ListOp and generate the squared mesaurment operator
-            o2_list = []
-            for op in op_list:
-                o2_list.append(
-                    StateFn(
-                        (op.primitive @ op.primitive).reduce().reduce(),
-                        is_measurement=True,
-                    )
-                )
-
-            # Suitable export format
-            if not isinstance(self.opflow, ListOp):
-                O2 = o2_list[0]
-            else:
-                O2 = ListOp(o2_list)
-
-            # If caching is enabled, store in the dictionary
-            if self.opflow_caching == True:
-                self.opflow_cache["OO"] = O2
-            return O2
-
-    def get_parameter_vector(self):
-        return self.parameters
-
-    @property
-    def num_parameters(self):
-        return len(self.parameters)
-
-    @property
-    def num_operators(self):
-        return self._num_operators
-
-    def assign_parameters(self, operator, parameters: np.ndarray):
-        param_op_inp, multi_param_op = adjust_input(parameters, len(self.parameters))
-
-        return_list = []
-        for p in param_op_inp:
-            dic = dict(zip(self.parameters, p))
-            return_list.append(_convert_to_sparse(operator.assign_parameters(dic)))
-
-        if multi_param_op:
-            return ListOp(return_list)
-        else:
-            return return_list[0]
-
-
-def _opflow_differentiation(opflow, parameters):
-    """Special routines for differentiating a given expectation operator
-    w.r.t. the Expectation operator parameters
-
-    Args:
-        expectation_op : opflow structure of the expectation operator
-        param : parameters of the differentiation
-    Returns:
-        opflow structure of the differentiated input opflow
-        return ListOp for multiple parameters
-    """
-    # Make a list if input is not a list
-    if parameters == None or parameters == []:
-        return None
-
-    if isinstance(parameters, ParameterVectorElement):
-        parameters = [parameters]
-
-    if not isinstance(opflow, ListOp):
-        expectation_op_ = ListOp([opflow])
-    else:
-        expectation_op_ = opflow
-
-    list_op = []
-    for op in expectation_op_:
-        if len(parameters) == 1:
-            # In case of a single parameter no array has to be returned
-            expectation_op_grad = _operator_differentiation(op, parameters[0])
-            list_op.append(expectation_op_grad)
-        else:
-            # Build list and derive the differentiated circuit for each parameter separately
-            expectation_op_grad_list = []
-            for p in parameters:
-                expectation_op_grad = _operator_differentiation(op, p)
-                expectation_op_grad_list.append(expectation_op_grad)
-            list_op.append(ListOp(expectation_op_grad_list))
-
-    if not isinstance(opflow, ListOp):
-        return list_op[0]
-    else:
-        return ListOp(list_op)
-
-
-def _operator_differentiation(operator, parameters):
-    """
-    Computes the differentiation of a single operator
-    """
-
-    # Helper function for getting the coefficient
-    def is_coeff_c(coeff, c):
-        if isinstance(coeff, ParameterExpression):
-            expr = coeff._symbol_expr
-            return expr == c
-        return coeff == c
-
-    # Check for parameter lists, this is not supported here!
-
-    # TODO also iterationable
-    if isinstance(parameters, (ParameterVector, list)):
-        grad_list = [_operator_differentiation(operator, p) for p in parameters]
-        return ListOp(grad_list)
-
-    # In case input operator is 0 return 0
-    if operator == 0:
-        return 0.0 * PauliOp(Pauli("I" * operator.num_qubits))
-
-    if isinstance(operator, OperatorStateFn):
-        op = _operator_differentiation(operator.primitive, parameters)
-        if op == 0:
-            return StateFn(
-                PauliOp(Pauli("I" * operator.num_qubits)),
-                is_measurement=True,
-                coeff=0.0,
-            )
-        return StateFn(op, is_measurement=True)
-
-    # Handle SummedOp but also ListOps!!
-    if isinstance(operator, ListOp):
-        # Iterate the gradient derivation through the list
-        grad_ops = [_operator_differentiation(op, parameters) for op in operator.oplist]
-
-        # pylint: disable=comparison-with-callable
-        if isinstance(operator, SummedOp):
-            without_zeros = [grad for grad in grad_ops if grad != 0]
-            if len(without_zeros) == 0:
-                return 0
-            return SummedOp(oplist=without_zeros, coeff=operator.coeff).reduce()
-        elif isinstance(operator, real_ListOp):
-            return ListOp(grad_ops, coeff=operator.coeff, combo_fn=operator.combo_fn)
-        else:
-            raise TypeError("Only SummedOp or ListOp are allowed! Type found:", type(operator))
-
-    # No we can finally do the differentiation
-    if not is_coeff_c(operator._coeff, 1.0) and not is_coeff_c(operator._coeff, 1.0j):
-        coeff = operator._coeff
-        if is_coeff_c(coeff, 0.0):
-            return ~Zero @ One
-        op = operator / coeff
-
-        d_coeff = _coeff_derivative(coeff, parameters)
-        grad_op = 0
-        if op != ~Zero @ One and not is_coeff_c(d_coeff, 0.0):
-            grad_op += d_coeff * op
-
-        return grad_op
-
-    # Only operator without coefficients is left, return 0 since a constant value is differentiated
-    return 0.0 * PauliOp(Pauli("I" * operator.num_qubits))
-
-
-def _convert_to_sparse(operator):
-    # convert operator into sparse form
-    if isinstance(operator, OperatorStateFn):
-        if not isinstance(operator.primitive, PauliOp) and not isinstance(
-            operator.primitive, PauliSumOp
-        ):
-            # Recreate OperatorStateFn with PauliSumOp instead of SummedOp -> large speed up!
-            return OperatorStateFn(
-                sum(operator.primitive.oplist),
-                coeff=operator.coeff,
-                is_measurement=operator.is_measurement,
-            )
-        elif isinstance(operator.primitive, PauliOp):
-            return OperatorStateFn(
-                PauliSumOp(
-                    SparsePauliOp(operator.primitive.primitive, coeffs=[operator.primitive.coeff])
-                ),
-                coeff=operator.coeff,
-                is_measurement=operator.is_measurement,
-            )
-        else:
-            return operator
-
-    elif isinstance(operator, ListOp):
-        op_list = [_convert_to_sparse(op) for op in operator.oplist]
-
-        if isinstance(operator, SummedOp):
-            return SummedOp(oplist=op_list, coeff=operator.coeff)
-        elif isinstance(operator, TensoredOp):
-            return TensoredOp(oplist=op_list, coeff=operator.coeff)
-        elif isinstance(operator, real_ListOp):
-            return ListOp(oplist=op_list, coeff=operator.coeff)
-        else:
-            raise ValueError("Unknown ListOp type in _convert_to_sparse:", type(operator))
-    else:
-        raise ValueError("Unsupported type in _convert_to_sparse:", type(operator))
+from qiskit.circuit import ParameterVector, ParameterExpression
+from qiskit.circuit.parametervector import ParameterVectorElement
+from qiskit.opflow import StateFn, OperatorStateFn
+from qiskit.opflow import SummedOp, ListOp, PauliOp, TensoredOp, PauliSumOp
+from qiskit.opflow import Zero, One
+from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
+from qiskit.opflow.gradients.derivative_base import _coeff_derivative
+from qiskit.quantum_info import Pauli, SparsePauliOp
+from typing import Union
+import numpy as np
+
+from .expectation_operator_base import ExpectationOperatorBase
+from ..util.data_preprocessing import adjust_input
+
+
+class ExpectationOperatorDerivatives:
+    def __init__(
+        self,
+        expectation_operator: Union[ExpectationOperatorBase, list],
+        opflow_caching=True,
+    ):
+        # handling multiple Expectation_operators also done here
+
+        self.expectation_operator = expectation_operator
+
+        # Contains the OperatorMeasurement() of the expectation-operator for later replacement
+        if isinstance(self.expectation_operator, ExpectationOperatorBase):
+            # 1d output by a single expectation-operator
+            self.multiple_output = False
+            self._num_operators = 1
+            self.parameters = ParameterVector("p_op", expectation_operator.num_parameters)
+
+            opflow = self.expectation_operator.get_operator(self.parameters)
+            opflow.replace = False
+        else:
+            # multi dimensional output by multiple Expectation-operators
+            expectation_op_list = []
+            self.multiple_output = True
+            self._num_operators = len(expectation_operator)
+            try:
+                n_oper = 0
+                for op in self.expectation_operator:
+                    n_oper = n_oper + op.num_parameters
+
+                self.parameters = ParameterVector("p_op", n_oper)
+                ioff = 0
+                for op in self.expectation_operator:
+                    expectation_op_list.append(op.get_operator(self.parameters[ioff:]))
+                    ioff = ioff + op.num_parameters
+                opflow = ListOp(expectation_op_list)
+                opflow.replace = False
+            except:
+                raise ValueError("Unknown structure of the Expectation operator!")
+
+        self.opflow = opflow
+        self.opflow_cache = {}
+        self.opflow_caching = opflow_caching
+
+        if self.opflow_caching:
+            self.opflow_cache["O"] = opflow
+
+    def get_derivate(self, input: Union[str, tuple]):
+        """return the opflow structure of the wavefunction"""
+        if isinstance(input, str):
+            # todo change with replaced operator
+            if input == "I":
+                measure_op = StateFn(
+                    PauliOp(Pauli("I" * self.opflow.num_qubits)), is_measurement=True
+                )
+            elif input == "O":
+                measure_op = self.opflow
+            elif input == "OO":
+                measure_op = self.get_operator_squared()
+            elif input == "dop" or input == "Odop":
+                measure_op = self._differentiation_from_tuple(
+                    self.opflow.copy(), (self.parameters,), "O"
+                )
+            elif input == "dopdop" or input == "Odopdop":
+                measure_op = self._differentiation_from_tuple(
+                    self.opflow.copy(), (self.parameters, self.parameters), "O"
+                )
+            elif input == "OOdop":
+                measure_op = self._differentiation_from_tuple(
+                    self.get_operator_squared(), (self.parameters,), "OO"
+                )
+            elif input == "OOdopdop":
+                measure_op = self._differentiation_from_tuple(
+                    self.get_operator_squared(),
+                    (self.parameters, self.parameters),
+                    "OO",
+                )
+            else:
+                raise ValueError("Unknown string command:", input)
+
+        elif isinstance(input, tuple):
+            measure_op = self._differentiation_from_tuple(self.opflow, input, "O")
+        else:
+            raise TypeError("Input is neither string nor tuple, but:", type(input))
+
+        measure_op.replace = False
+        return measure_op
+
+    def get_differentiation_from_tuple(self, diff_tuple: tuple):
+        return self.get_derivate(diff_tuple)
+
+    def get_derivation_from_string(self, input_string: str):
+        return self.get_derivate(input_string)
+
+    def _differentiation_from_tuple(self, expectation_op, diff_tuple: tuple, expectation_op_label):
+        """Recursive routine for automatic differentiating the expectation_operator
+        Args:
+            diff_tuple : tuple containing ParameterVectors or ParameterExpressions
+        Returns:
+            The differentiated opflow expression
+        """
+        # TODO: outer function for input checking
+
+        if diff_tuple == ():
+            # Cancel the recursion by returning the opflow of the simply measured feature map
+            return expectation_op
+        else:
+            # Check if differentiating tuple is already stored in opflow_cache
+            if (
+                self.opflow_caching == True
+                and (diff_tuple, expectation_op_label) in self.opflow_cache
+            ):
+                # If stored -> return
+                return self.opflow_cache[(diff_tuple, expectation_op_label)].copy()
+            else:
+                # Recursive differentiation with the most left object
+                measure = _opflow_differentiation(
+                    self._differentiation_from_tuple(
+                        expectation_op, diff_tuple[1:], expectation_op_label
+                    ),
+                    diff_tuple[0],
+                )
+                # Store result in the opflow_cache
+                if self.opflow_caching == True:
+                    self.opflow_cache[(diff_tuple, expectation_op_label)] = measure
+                return measure
+
+    def get_operator_squared(self):
+        "Builds and caches the squared form of the expectation operator OO=O^2"
+        if self.opflow_caching == True and "OO" in self.opflow_cache:
+            return self.opflow_cache["OO"].copy()
+        else:
+            # Get the operator and store it in ListOp structure
+            if not isinstance(self.opflow, ListOp):
+                op_list = ListOp([self.opflow])
+            else:
+                op_list = self.opflow
+
+            # Loop through the ListOp and generate the squared mesaurment operator
+            o2_list = []
+            for op in op_list:
+                o2_list.append(
+                    StateFn(
+                        (op.primitive @ op.primitive).reduce().reduce(),
+                        is_measurement=True,
+                    )
+                )
+
+            # Suitable export format
+            if not isinstance(self.opflow, ListOp):
+                O2 = o2_list[0]
+            else:
+                O2 = ListOp(o2_list)
+
+            # If caching is enabled, store in the dictionary
+            if self.opflow_caching == True:
+                self.opflow_cache["OO"] = O2
+            return O2
+
+    def get_parameter_vector(self):
+        return self.parameters
+
+    @property
+    def num_parameters(self):
+        return len(self.parameters)
+
+    @property
+    def num_operators(self):
+        return self._num_operators
+
+    def assign_parameters(self, operator, parameters: np.ndarray):
+        param_op_inp, multi_param_op = adjust_input(parameters, len(self.parameters))
+
+        return_list = []
+        for p in param_op_inp:
+            dic = dict(zip(self.parameters, p))
+            return_list.append(_convert_to_sparse(operator.assign_parameters(dic)))
+
+        if multi_param_op:
+            return ListOp(return_list)
+        else:
+            return return_list[0]
+
+
+def _opflow_differentiation(opflow, parameters):
+    """Special routines for differentiating a given expectation operator
+    w.r.t. the Expectation operator parameters
+
+    Args:
+        expectation_op : opflow structure of the expectation operator
+        param : parameters of the differentiation
+    Returns:
+        opflow structure of the differentiated input opflow
+        return ListOp for multiple parameters
+    """
+    # Make a list if input is not a list
+    if parameters == None or parameters == []:
+        return None
+
+    if isinstance(parameters, ParameterVectorElement):
+        parameters = [parameters]
+
+    if not isinstance(opflow, ListOp):
+        expectation_op_ = ListOp([opflow])
+    else:
+        expectation_op_ = opflow
+
+    list_op = []
+    for op in expectation_op_:
+        if len(parameters) == 1:
+            # In case of a single parameter no array has to be returned
+            expectation_op_grad = _operator_differentiation(op, parameters[0])
+            list_op.append(expectation_op_grad)
+        else:
+            # Build list and derive the differentiated circuit for each parameter separately
+            expectation_op_grad_list = []
+            for p in parameters:
+                expectation_op_grad = _operator_differentiation(op, p)
+                expectation_op_grad_list.append(expectation_op_grad)
+            list_op.append(ListOp(expectation_op_grad_list))
+
+    if not isinstance(opflow, ListOp):
+        return list_op[0]
+    else:
+        return ListOp(list_op)
+
+
+def _operator_differentiation(operator, parameters):
+    """
+    Computes the differentiation of a single operator
+    """
+
+    # Helper function for getting the coefficient
+    def is_coeff_c(coeff, c):
+        if isinstance(coeff, ParameterExpression):
+            expr = coeff._symbol_expr
+            return expr == c
+        return coeff == c
+
+    # Check for parameter lists, this is not supported here!
+
+    # TODO also iterationable
+    if isinstance(parameters, (ParameterVector, list)):
+        grad_list = [_operator_differentiation(operator, p) for p in parameters]
+        return ListOp(grad_list)
+
+    # In case input operator is 0 return 0
+    if operator == 0:
+        return 0.0 * PauliOp(Pauli("I" * operator.num_qubits))
+
+    if isinstance(operator, OperatorStateFn):
+        op = _operator_differentiation(operator.primitive, parameters)
+        if op == 0:
+            return StateFn(
+                PauliOp(Pauli("I" * operator.num_qubits)),
+                is_measurement=True,
+                coeff=0.0,
+            )
+        return StateFn(op, is_measurement=True)
+
+    # Handle SummedOp but also ListOps!!
+    if isinstance(operator, ListOp):
+        # Iterate the gradient derivation through the list
+        grad_ops = [_operator_differentiation(op, parameters) for op in operator.oplist]
+
+        # pylint: disable=comparison-with-callable
+        if isinstance(operator, SummedOp):
+            without_zeros = [grad for grad in grad_ops if grad != 0]
+            if len(without_zeros) == 0:
+                return 0
+            return SummedOp(oplist=without_zeros, coeff=operator.coeff).reduce()
+        elif isinstance(operator, real_ListOp):
+            return ListOp(grad_ops, coeff=operator.coeff, combo_fn=operator.combo_fn)
+        else:
+            raise TypeError("Only SummedOp or ListOp are allowed! Type found:", type(operator))
+
+    # No we can finally do the differentiation
+    if not is_coeff_c(operator._coeff, 1.0) and not is_coeff_c(operator._coeff, 1.0j):
+        coeff = operator._coeff
+        if is_coeff_c(coeff, 0.0):
+            return ~Zero @ One
+        op = operator / coeff
+
+        d_coeff = _coeff_derivative(coeff, parameters)
+        grad_op = 0
+        if op != ~Zero @ One and not is_coeff_c(d_coeff, 0.0):
+            grad_op += d_coeff * op
+
+        return grad_op
+
+    # Only operator without coefficients is left, return 0 since a constant value is differentiated
+    return 0.0 * PauliOp(Pauli("I" * operator.num_qubits))
+
+
+def _convert_to_sparse(operator):
+    # convert operator into sparse form
+    if isinstance(operator, OperatorStateFn):
+        if not isinstance(operator.primitive, PauliOp) and not isinstance(
+            operator.primitive, PauliSumOp
+        ):
+            # Recreate OperatorStateFn with PauliSumOp instead of SummedOp -> large speed up!
+            return OperatorStateFn(
+                sum(operator.primitive.oplist),
+                coeff=operator.coeff,
+                is_measurement=operator.is_measurement,
+            )
+        elif isinstance(operator.primitive, PauliOp):
+            return OperatorStateFn(
+                PauliSumOp(
+                    SparsePauliOp(operator.primitive.primitive, coeffs=[operator.primitive.coeff])
+                ),
+                coeff=operator.coeff,
+                is_measurement=operator.is_measurement,
+            )
+        else:
+            return operator
+
+    elif isinstance(operator, ListOp):
+        op_list = [_convert_to_sparse(op) for op in operator.oplist]
+
+        if isinstance(operator, SummedOp):
+            return SummedOp(oplist=op_list, coeff=operator.coeff)
+        elif isinstance(operator, TensoredOp):
+            return TensoredOp(oplist=op_list, coeff=operator.coeff)
+        elif isinstance(operator, real_ListOp):
+            return ListOp(oplist=op_list, coeff=operator.coeff)
+        else:
+            raise ValueError("Unknown ListOp type in _convert_to_sparse:", type(operator))
+    else:
+        raise ValueError("Unsupported type in _convert_to_sparse:", type(operator))
```

### Comparing `squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_amplitude.py` & `squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/single_pauli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,69 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit.opflow import PauliOp
-from qiskit.quantum_info import Pauli
-
-from ..expectation_operator_base import ExpectationOperatorBase
-
-
-class SingleAmplitude(ExpectationOperatorBase):
-    """Initialization
-
-    Operator for measuring the probability of being in state 0 or 1 of a qubit.
-    Implemented by |0><0| = 0.5*(I+Z) and |1><1| = 0.5*(I-Z)
-
-    Args:
-        number_of_qubits: Number of qubits.
-        qubits: index of the qubit for which the probability is measured
-        one_state: if false the |0><0| state is measured, if true the |1><1| state is measured
-    """
-
-    def __init__(self, num_qubits: int, qubit=0, one_state=False) -> None:
-        super().__init__(num_qubits)
-        self.qubit = qubit
-        self.one_state = one_state
-
-    @property
-    def num_parameters(self):
-        return 0
-
-    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray] = None):
-        """
-        Returns:
-            Return PauliOp expression of the specified Expectation operator.
-        """
-
-        i = self.qubit
-        if 0 > i or self.num_qubits <= i:
-            raise ValueError("Specified qubit out of range")
-        I = "I" * self.num_qubits
-        Z = I[(i + 1) :] + "Z" + I[:i]
-
-        if self.one_state:
-            H = 0.5 * PauliOp(Pauli(I)) - 0.5 * PauliOp(Pauli(Z))
-        else:
-            H = 0.5 * PauliOp(Pauli(I)) + 0.5 * PauliOp(Pauli(Z))
-
-        return H.reduce()
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit.opflow import PauliOp
+from qiskit.quantum_info import Pauli
+
+from ..expectation_operator_base import ExpectationOperatorBase
+
+
+class SinglePauli(ExpectationOperatorBase):
+    r"""
+    Expectation operator for evaluating the expectation value of a single Pauli operator.
+
+
+    Example :math:`\hat{Z_i}`.
+
+    Args:
+        num_qubits (int): Number of qubits.
+        qubit (int): Qubit for which the Pauli expectation value is obtained.
+        op_str (str): Pauli operator to measure. Must be one of ``'I'``, ``'X'``, ``'Y'``, ``'Z'``.
+        parameterized (bool): If True, the operator is parameterized.
+
+    """
+
+    def __init__(
+        self, num_qubits: int, qubit: int, op_str: str = "Z", parameterized: bool = False
+    ) -> None:
+        super().__init__(num_qubits)
+
+        self.qubit = qubit
+        self.op_str = op_str
+        self.parameterized = parameterized
+
+        if self.op_str not in ["I", "X", "Y", "Z"]:
+            raise ValueError("Specified operator not supported")
+
+    @property
+    def num_parameters(self):
+        """Returns the number of free parameters in the single pauli operator"""
+
+        if self.parameterized:
+            return 1
+        else:
+            return 0
+
+    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray]):
+        """
+        Function for generating the PauliOp expression of the single pauli operator.
+
+        Args:
+            parameters (Union[ParameterVector, np.ndarray]): Parameters of the single
+                pauli operator.
+
+        Returns:
+            PauliOp expression of the specified single pauli operator.
+        """
+
+        i = self.qubit
+        if 0 > i or self.num_qubits <= i:
+            raise ValueError("Specified qubit out of range")
+
+        H = "I" * self.num_qubits
+        H = PauliOp(Pauli(H[(i + 1) :] + self.op_str + H[:i]))
+
+        if self.parameterized:
+            H = H * parameters[0]
+
+        return H.reduce()
```

### Comparing `squlearn-0.1.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_amplitudes.py` & `squlearn-0.2.0/src/squlearn/expectation_operator/expectation_operator_implemented/summed_probabilities.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,81 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit.opflow import PauliOp
-from qiskit.quantum_info import Pauli
-
-from ..expectation_operator_base import ExpectationOperatorBase
-
-
-class SummedAmplitudes(ExpectationOperatorBase):
-    """
-    Operator for a + sum_i b_i |0_i><0_i|
-    Implemented by |0><0| = 0.5*(I+Z) and |1><1| = 0.5*(I-Z)
-
-    Args:
-        num_qubits: Number of qubits.
-        one_state: if false the |0><0| state is measured, if true the |1><1| state is measured
-
-    """
-
-    def __init__(self, num_qubits: int, one_state=False, full_sum: bool = True) -> None:
-        super().__init__(num_qubits)
-        self.one_state = one_state
-        self.full_sum = full_sum
-
-    @property
-    def num_parameters(self):
-        if self.full_sum:
-            return 1 + self.num_qubits
-        else:
-            return 2
-
-    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray] = None):
-        """
-        Returns:
-            Return PauliOp expression of the specified Expectation operator.
-        """
-
-        nparam = len(parameters)
-        H = PauliOp(Pauli("I" * self.num_qubits)) * parameters[0 % nparam]
-
-        ioff = 1
-        for i in range(self.num_qubits):
-            I = "I" * self.num_qubits
-            Z = I[(i + 1) :] + "Z" + I[:i]
-
-            if self.one_state:
-                H = (
-                    H
-                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(I))
-                    - parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(Z))
-                )
-            else:
-                H = (
-                    H
-                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(I))
-                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(Z))
-                )
-            if self.full_sum:
-                ioff += 1
-
-        return H.reduce()
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit.opflow import PauliOp
+from qiskit.quantum_info import Pauli
+
+from ..expectation_operator_base import ExpectationOperatorBase
+
+
+class SummedProbabilities(ExpectationOperatorBase):
+    r"""
+    Operator for summed probabilities of being in state 0 or 1.
+
+    Operator reads:
+
+    .. math::
+
+        \hat{H} = a\hat{I} + \sum_i b_i (\ket{0}\bra{0})_i
+
+    Implemented by :math:`\ket{0}\bra{0} = 0.5(\hat{I}+\hat{Z})` and :math:`\ket{1}\bra{1} = 0.5(\hat{I}-\hat{Z})`
+
+    Args:
+        num_qubits (int): Number of qubits.
+        one_state: If false the :math:`\ket{0}\bra{0}` state is measured,
+            if true the :math:`\ket{1}\bra{1}` state is measured
+        full_sum (bool): If False, the parameters are excluded from the sum,
+            i.e. the sum is :math:`b\sum_i (\ket{0}\bra{0})_i`
+            instead of :math:`\sum_i b_i (\ket{0}\bra{0})_i`
+
+    """
+
+    def __init__(self, num_qubits: int, one_state=False, full_sum: bool = True) -> None:
+        super().__init__(num_qubits)
+        self.one_state = one_state
+        self.full_sum = full_sum
+
+    @property
+    def num_parameters(self):
+        """Returns the number of free parameters in the summed probabilities operator"""
+        if self.full_sum:
+            return 1 + self.num_qubits
+        else:
+            return 2
+
+    def get_pauli(self, parameters: Union[ParameterVector, np.ndarray] = None):
+        """
+        Function for generating the PauliOp expression of the summed probabilities operator.
+
+        Args:
+            parameters (Union[ParameterVector, np.ndarray]): Parameters of the summed
+                probabilities operator.
+
+        Returns:
+            PauliOp expression of the specified summed probabilities operator.
+        """
+
+        nparam = len(parameters)
+        H = PauliOp(Pauli("I" * self.num_qubits)) * parameters[0 % nparam]
+
+        ioff = 1
+        for i in range(self.num_qubits):
+            I = "I" * self.num_qubits
+            Z = I[(i + 1) :] + "Z" + I[:i]
+
+            if self.one_state:
+                H = (
+                    H
+                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(I))
+                    - parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(Z))
+                )
+            else:
+                H = (
+                    H
+                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(I))
+                    + parameters[ioff % nparam] * 0.5 * PauliOp(Pauli(Z))
+                )
+            if self.full_sum:
+                ioff += 1
+
+        return H.reduce()
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_base.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-
-class FeatureMapBase:
-    """
-    Feature map base class
-
-    Args:
-        num_qubits (int): Number of Qubits of the feature map
-        num_features (int): Dimension of the feature vector
-    """
-
-    def __init__(self, num_qubits: int, num_features: int) -> None:
-        self._num_qubits = num_qubits
-        self._num_features = num_features
-
-    @property
-    def num_qubits(self) -> int:
-        """Returns the number of qubits of the feature map."""
-        return self._num_qubits
-
-    @property
-    def num_features(self) -> int:
-        """Returns the dimension of features of the feature map."""
-        return self._num_features
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the feature map."""
-        return 0
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in qiskit QuantumCircuit format
-        """
-
-        raise NotImplementedError()
-
-    def draw(
-        self,
-        feature_label: str = "x",
-        parameter_label: str = "θ",
-        output: str = "mpl",
-        filename: str = None,
-    ) -> None:
-        """
-        Draws the feature map circuit using the QuantumCircuit.draw() function.
-
-        Args:
-            feature_label (str): Label for the feature vector (default:"x").
-            parameter_label (str): Label for the parameter vector (default:"θ").
-            output (str): One of the qiskit output options ('text', 'mpl', 'latex', 'latex_source').
-                The default is 'mpl'
-            filename (str): Location for storing the output (default: None)
-
-        No other arguments are passed to the draw function!
-        """
-
-        feature_vec = ParameterVector(feature_label, self.num_features)
-        parameters_vec = ParameterVector(parameter_label, self.num_parameters)
-        if filename is None:
-            return self.get_circuit(feature_vec, parameters_vec).draw(output=output)
-        else:
-            return self.get_circuit(feature_vec, parameters_vec).draw(
-                output=output, filename=filename
-            )
-
-    def __mul__(self, x):
-        return self.__add__(x)
-
-    def __add__(self, x):
-        """
-        Overwrites the a + b function, such that the addition of
-        feature maps returns the composition of both feature maps.
-
-        Number of qubits and features have to be equal in both feature maps!
-        The special function and properties of the both feature maps are lost
-        by this composition.
-
-        Args:
-            self (FeatureMapBase): right / first feature map
-            x (FeatureMapBase): left / second feature map
-
-        Returns:
-            Returns the composed feature map as special class ComposedFeatureMap
-        """
-
-        if not isinstance(x, FeatureMapBase):
-            raise ValueError("Only the addition with other feature maps is allowed!")
-
-        class ComposedFeatureMap(FeatureMapBase):
-            """
-            Special class for composed feature maps.
-
-            Args:
-                fm1 (FeatureMapBase): right / first feature map
-                fm2 (FeatureMapBase): left / second feature map
-            """
-
-            def __init__(self, fm1: FeatureMapBase, fm2: FeatureMapBase):
-                if fm1.num_qubits != fm2.num_qubits:
-                    raise ValueError("Number of qubits is not equal in both feature maps.")
-
-                if fm1.num_features != fm2.num_features:
-                    raise ValueError("Feature dimension is not equal in both feature maps.")
-
-                super().__init__(fm1.num_qubits, fm2.num_features)
-
-                self._fm1 = fm1
-                self._fm2 = fm2
-
-            @property
-            def num_parameters(self) -> int:
-                """Returns the number of trainable parameters of composed feature map.
-                Is equal to the sum of both trainable parameters
-                """
-                return self._fm1.num_parameters + self._fm2.num_parameters
-
-            def get_circuit(
-                self,
-                features: Union[ParameterVector, np.ndarray],
-                parameters: Union[ParameterVector, np.ndarray],
-            ) -> QuantumCircuit:
-                """
-                Returns the circuit of the composed feature maps
-
-                Args:
-                    features Union[ParameterVector,np.ndarray]: Input vector of the features
-                        from which the gate inputs are obtained
-                    param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                        from which the gate inputs are obtained
-
-                Return:
-                    Returns the circuit of the composed feature maps in qiskit QuantumCircuit format
-                """
-
-                circ1 = self._fm1.get_circuit(features, parameters[: self._fm1.num_parameters])
-                circ2 = self._fm2.get_circuit(features, parameters[self._fm1.num_parameters :])
-
-                return circ1.compose(circ2, range(self._fm1.num_qubits))
-
-        return ComposedFeatureMap(self, x)
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+
+class FeatureMapBase:
+    """
+    Feature map base class
+
+    Args:
+        num_qubits (int): Number of Qubits of the feature map
+        num_features (int): Dimension of the feature vector
+    """
+
+    def __init__(self, num_qubits: int, num_features: int) -> None:
+        self._num_qubits = num_qubits
+        self._num_features = num_features
+
+    @property
+    def num_qubits(self) -> int:
+        """Returns the number of qubits of the feature map."""
+        return self._num_qubits
+
+    @property
+    def num_features(self) -> int:
+        """Returns the dimension of features of the feature map."""
+        return self._num_features
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the feature map."""
+        return 0
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in qiskit QuantumCircuit format
+        """
+
+        raise NotImplementedError()
+
+    def draw(
+        self,
+        feature_label: str = "x",
+        parameter_label: str = "p",
+        decompose: bool = False,
+        **kwargs,
+    ) -> None:
+        """
+        Draws the feature map circuit using the QuantumCircuit.draw() function.
+
+        Args:
+            feature_label (str): Label for the feature vector (default:"x").
+            parameter_label (str): Label for the parameter vector (default:"θ").
+            decompose (bool): If True, the circuit is decomposed before printing (default: False).
+            kwargs: Additional arguments from Qiskit's QuantumCircuit.draw() function.
+
+        Returns:
+            Returns the circuit in qiskit QuantumCircuit.draw() format
+        """
+
+        feature_vec = ParameterVector(feature_label, self.num_features)
+        parameters_vec = ParameterVector(parameter_label, self.num_parameters)
+
+        circ = self.get_circuit(feature_vec, parameters_vec)
+        if decompose:
+            circ = circ.decompose()
+
+        return circ.draw(**kwargs)
+
+    def __mul__(self, x):
+        return self.__add__(x)
+
+    def __add__(self, x):
+        """
+        Overwrites the a + b function, such that the addition of
+        feature maps returns the composition of both feature maps.
+
+        Number of qubits and features have to be equal in both feature maps!
+        The special function and properties of the both feature maps are lost
+        by this composition.
+
+        Args:
+            self (FeatureMapBase): right / first feature map
+            x (FeatureMapBase): left / second feature map
+
+        Returns:
+            Returns the composed feature map as special class ComposedFeatureMap
+        """
+
+        if not isinstance(x, FeatureMapBase):
+            raise ValueError("Only the addition with other feature maps is allowed!")
+
+        class ComposedFeatureMap(FeatureMapBase):
+            """
+            Special class for composed feature maps.
+
+            Args:
+                fm1 (FeatureMapBase): right / first feature map
+                fm2 (FeatureMapBase): left / second feature map
+            """
+
+            def __init__(self, fm1: FeatureMapBase, fm2: FeatureMapBase):
+                if fm1.num_qubits != fm2.num_qubits:
+                    raise ValueError("Number of qubits is not equal in both feature maps.")
+
+                if fm1.num_features != fm2.num_features:
+                    raise ValueError("Feature dimension is not equal in both feature maps.")
+
+                super().__init__(fm1.num_qubits, fm2.num_features)
+
+                self._fm1 = fm1
+                self._fm2 = fm2
+
+            @property
+            def num_parameters(self) -> int:
+                """Returns the number of trainable parameters of composed feature map.
+                Is equal to the sum of both trainable parameters
+                """
+                return self._fm1.num_parameters + self._fm2.num_parameters
+
+            def get_circuit(
+                self,
+                features: Union[ParameterVector, np.ndarray],
+                parameters: Union[ParameterVector, np.ndarray],
+            ) -> QuantumCircuit:
+                """
+                Returns the circuit of the composed feature maps
+
+                Args:
+                    features Union[ParameterVector,np.ndarray]: Input vector of the features
+                        from which the gate inputs are obtained
+                    param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                        from which the gate inputs are obtained
+
+                Return:
+                    Returns the circuit of the composed feature maps in qiskit QuantumCircuit format
+                """
+
+                circ1 = self._fm1.get_circuit(features, parameters[: self._fm1.num_parameters])
+                circ2 = self._fm2.get_circuit(features, parameters[self._fm1.num_parameters :])
+
+                return circ1.compose(circ2, range(self._fm1.num_qubits))
+
+        return ComposedFeatureMap(self, x)
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_derivatives.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_derivatives.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,457 +1,457 @@
-from qiskit.circuit import ParameterVector, ParameterExpression
-from qiskit.circuit.parametervector import ParameterVectorElement
-from qiskit.opflow import CircuitSampler
-from qiskit.opflow import OperatorBase
-from qiskit.opflow import StateFn, CircuitStateFn, OperatorStateFn, DictStateFn
-from qiskit.opflow import SummedOp, ComposedOp, TensoredOp
-from qiskit.opflow import ListOp, PauliOp
-from qiskit.opflow import Zero, One
-from qiskit.compiler import transpile
-from qiskit.quantum_info import Pauli
-from qiskit.opflow import PauliOp
-from qiskit.opflow.gradients import Gradient
-from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
-import numpy as np
-from typing import Union
-
-from .feature_map_base import FeatureMapBase
-
-
-class FeatureMapDerivatives:
-    def __init__(
-        self,
-        feature_map: FeatureMapBase,
-        opflow_caching=True,
-    ):
-        self.feature_map = feature_map
-
-        self.x = ParameterVector("x", self.feature_map.num_features)
-        self.p = ParameterVector("p", self.feature_map.num_parameters)
-
-        circuit = feature_map.get_circuit(self.x, self.p)
-
-        # TODO transpiling
-
-        self.circuit_opflow = CircuitStateFn(primitive=circuit, coeff=1.0)
-
-        self.num_qubits = self.circuit_opflow.num_qubits
-
-        identity_measurement = StateFn(PauliOp(Pauli("I" * self.num_qubits)), is_measurement=True)
-        identity_measurement.replace = True
-
-        self.opflow = identity_measurement @ self.circuit_opflow
-
-        self.opflow_cache = {}
-        self.opflow_caching = opflow_caching
-
-        if self.opflow_caching:
-            self.opflow_cache["f"] = self.opflow
-
-        # get the instruction gates from the original circuit for transpiling the circuits back to this basis
-        self.instruction_set = set()
-        for instruction in circuit.data:
-            self.instruction_set.add(instruction.operation.name)
-        self.instruction_set = list(self.instruction_set)
-
-    def get_derivate(self, input: Union[str, tuple]):
-        """return the opflow structure of the circuit from the input"""
-        if isinstance(input, str):
-            if input == "I":
-                opflow = self.opflow
-            elif input == "dx":
-                opflow = self._differentiation_from_tuple((self.x,)).copy()
-            elif input == "dxdx":
-                opflow = self._differentiation_from_tuple((self.x, self.x)).copy()
-            elif input == "dpdxdx":
-                opflow = self._differentiation_from_tuple((self.p, self.x, self.x)).copy()
-            elif input == "laplace":
-                list_sum = []
-                for xi in self.x:
-                    list_sum.append(self._differentiation_from_tuple((xi, xi)).copy())
-                opflow = SummedOp(list_sum)
-            elif input == "laplace_dp":
-                list_sum = []
-                for xi in self.x:
-                    list_sum.append(self._differentiation_from_tuple((self.p, xi, xi)).copy())
-                opflow = SummedOp(list_sum)
-            elif input == "dp":
-                opflow = self._differentiation_from_tuple((self.p,)).copy()
-            elif input == "dpdp":
-                opflow = self._differentiation_from_tuple((self.p, self.p)).copy()
-            elif input == "dpdx":
-                opflow = self._differentiation_from_tuple((self.p, self.x)).copy()
-            else:
-                raise ValueError("Unknown string command:", input)
-        elif isinstance(input, tuple):
-            opflow = self._differentiation_from_tuple(input)
-        else:
-            raise TypeError("Input is neither string nor tuple, but:", type(input))
-
-        # remove mesurement operator
-
-        return _remove_measure(opflow)
-
-    def get_differentiation_from_tuple(self, diff_tuple: tuple):
-        return self.get_derivate(diff_tuple)
-
-    def get_derivation_from_string(self, input_string: str):
-        return self.get_derivate(input_string)
-
-    def _differentiation_from_tuple(self, diff_tuple: tuple):
-        """Recursive routine for automatic differentiating the feature map
-
-        Variables for the differentiation are supplied by a tuple
-        (x,param,param_op) from left to right -> ∂x ∂param ∂param_op PQC(x,param,param_op)
-
-
-        Args:
-            diff_tuple : tuple containing ParameterVectors or ParameterExpressions or Strings
-            determining the derivation
-            cost_op : String for specifying the used cost operator operator (default: None)
-                      (None or 'C' -> Standard, 'CC' -> Squared cost operator)
-        Returns:
-            The differentiated opflow expression
-        """
-        # TODO: outer function for input checking
-
-        if diff_tuple == ():
-            # Cancel the recursion by returning the opflow of the simply measured feature map
-            return self.opflow.copy()
-        else:
-            # Check if differentiating tuple is already stored in opflow_cache
-            if self.opflow_caching == True and (diff_tuple,) in self.opflow_cache:
-                # If stored -> return
-                return self.opflow_cache[(diff_tuple,)].copy()
-            else:
-                # Recursive differentiation with the most left object
-                circ = _opflow_differentiation(
-                    self._differentiation_from_tuple(diff_tuple[1:]), diff_tuple[0]
-                )
-                # Store result in the opflow_cache
-                if self.opflow_caching == True:
-                    self.opflow_cache[(diff_tuple,)] = circ
-                return circ
-
-    def get_parameter_vector(self):
-        return self.p
-
-    def get_feature_vector(self):
-        return self.x
-
-    @property
-    def num_parameters(self):
-        return len(self.p)
-
-    @property
-    def num_features(self):
-        return len(self.x)
-
-    def assign_parameters(self, opflow, features: np.ndarray, parameters: np.ndarray):
-        """
-        Assigns circuit parameters
-        """
-
-        if opflow == None:
-            return None
-
-        todo_list = []  # list for the variables
-        multi_list = []  # list of return ListOp or no list
-        param_list = []  # list of parameters that are substituted
-
-        # check shape of the x and adjust to [[]] form if necessary
-        if features is not None:
-            xx, multi_x = _adjust_input(features, len(self.x))
-            todo_list.append(xx)
-            param_list.append(self.x)
-            multi_list.append(multi_x)
-        if parameters is not None:
-            pp, multi_p = _adjust_input(parameters, len(self.p))
-            todo_list.append(pp)
-            param_list.append(self.p)
-            multi_list.append(multi_p)
-
-        # Recursive construction of the assignment dictionary and list structure
-        def rec_assign(dic, todo_list, param_list, multi_list):
-            if len(todo_list) <= 0:
-                return None
-            return_list = []
-            for x_ in todo_list[0]:
-                for A, B in zip(param_list[0], x_):
-                    dic[A] = B
-                if len(multi_list[1:]) > 0:
-                    return_list.append(
-                        rec_assign(dic.copy(), todo_list[1:], param_list[1:], multi_list[1:])
-                    )
-                else:
-                    return_list.append(opflow.assign_parameters(dic))
-
-            if multi_list[0]:
-                return ListOp(return_list)
-            else:
-                return return_list[0]
-
-        return rec_assign({}, todo_list, param_list, multi_list)
-
-
-def _adjust_input(x, x_length):
-    # check shape of the x and adjust to [[]] form if necessary
-    multiple_inputs = False
-    error = False
-    shape = np.shape(x)
-    if shape == () and x_length == 1:
-        # Single floating point number
-        xx = np.array([[x]])
-    elif len(shape) == 1:
-        if x_length == 1:
-            xx = np.array([np.array([xx]) for xx in x])
-            multiple_inputs = True
-        else:
-            # We have a single multi dimensional x (e.g. parameter vector)
-            if len(x) == x_length:
-                xx = np.array([x])
-            else:
-                error = True
-    elif len(shape) == 2:
-        if shape[1] == x_length:
-            xx = x
-            multiple_inputs = True
-        else:
-            error = True
-    else:
-        error = True
-
-    if error:
-        raise ValueError("Wrong format of an input variable.")
-
-    return xx, multiple_inputs
-
-
-def _remove_measure(operator: OperatorBase) -> OperatorBase:
-    """
-    Replace all flagged measurements in the input opflow expression
-    Recursive function
-
-    Args:
-        operator : Opflow expression
-        measurement : new measurement operator
-    Returns:
-        New opflow expression with replaced measurement operator
-    """
-    # We reached a ComposedOp term -> replace the measurement
-    if isinstance(operator, ComposedOp):
-        for i in range(len(operator.oplist)):
-            if isinstance(operator.oplist[i], CircuitStateFn):
-                return_op = operator.oplist[i]
-                return_op._coeff = operator.coeff
-                return return_op
-
-        return ~Zero @ One
-
-    # We reached a CircuitStateFn term -> apply the measurement to the wavefunction
-    elif isinstance(operator, CircuitStateFn):
-        return operator
-
-    # We reached a list of opflow terms, recursive call of
-    # the function to all children in the list
-    elif isinstance(operator, ListOp):
-        op_list = [_remove_measure(op) for op in operator.oplist]
-
-        if isinstance(operator, SummedOp):
-            return SummedOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, TensoredOp):
-            return TensoredOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, real_ListOp):
-            return ListOp(
-                oplist=[op for op in op_list if op != ~Zero @ One],
-                coeff=operator.coeff,
-                combo_fn=operator.combo_fn,
-            )
-        else:
-            raise ValueError("Unknown ListOp type in _remove_measure:", type(operator))
-    else:
-        raise ValueError("Unknown type in _remove_measure:", type(operator))
-
-
-def measure_feature_map_derivative(operator: OperatorBase, measurement) -> OperatorBase:
-    """
-    Replace all flagged measurements in the input opflow expression
-    Recursive function
-
-    Args:
-        operator : Opflow expression
-        measurement : new measurement operator
-    Returns:
-        New opflow expression with replaced measurement operator
-    """
-    # We reached a ComposedOp term -> replace the measurement
-    if isinstance(operator, ComposedOp):
-        for i in range(len(operator.oplist)):
-            if isinstance(operator.oplist[i], OperatorStateFn):
-                if hasattr(operator.oplist[i], "replace"):
-                    if operator.oplist[i].replace:
-                        operator.oplist[i] = measurement
-                else:
-                    operator.oplist[i] = measurement
-        return operator
-
-    # We reached a CircuitStateFn term -> apply the measurement to the wavefunction
-    elif isinstance(operator, CircuitStateFn):
-        coeff = operator._coeff
-        operator._coeff = 1.0
-        measured_op = measurement @ operator
-        measured_op._coeff = coeff
-        return measured_op
-
-    # We reached a list of opflow terms, recursive call of
-    # the function to all children in the list
-    elif isinstance(operator, ListOp):
-        op_list = [measure_feature_map_derivative(op, measurement) for op in operator.oplist]
-
-        if isinstance(operator, SummedOp):
-            return SummedOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, TensoredOp):
-            return TensoredOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, real_ListOp):
-            return ListOp(
-                oplist=[op for op in op_list if op != ~Zero @ One],
-                coeff=operator.coeff,
-                combo_fn=operator.combo_fn,
-            )
-        else:
-            raise ValueError("Unknown ListOp type in measure_derivative:", type(operator))
-    else:
-        raise ValueError("Unknown type in measure_derivative:", type(operator))
-
-
-def _opflow_differentiation(opflow, parameters):
-    """
-    Routine for the automatic differentiation based on qiskit routines
-
-    Args:
-        opflow : Input opflow expression
-        params (list | ParameterVector): variables which are used in the
-                                            differentiation (have to be the same type )
-    Returns:
-        opflow structure of the differentiated input opflow
-    """
-
-    # Make list if input is not a list
-    if isinstance(parameters, ParameterVectorElement):
-        parameters = [parameters]
-    if isinstance(parameters, tuple):
-        parameters = list(parameters)
-
-    # Call the automatic differentiation routine
-    # Separate routine for for one dim. or multi dim. variables
-    if len(parameters) == 1:
-        # Automatic qiskit differentiation
-        # ParameterExpression(0) is removed by clean_opflow_circ
-        # Gates are transpiled in Gradient(), this can yield different set of gates
-        # than supported by the QC hardware, this is also fixed by clean_opflow_circ
-        return _clean_opflow_circ(Gradient().convert(operator=opflow, params=parameters)[0])
-    else:
-        # If multiple variables are differentiated -> results are returned in array
-
-        # Check if the same variables are the same type
-        params_name = parameters[0].name.split("[", 1)[0]
-        for p in parameters:
-            if p.name.split("[", 1)[0] != params_name:
-                raise TypeError("Differentiable variables are not the same type.")
-
-        # Automatic qiskit differentiation
-        # ParameterExpression(0) is removed by clean_opflow_circ
-        # Gates are transpiled in Gradient(), this can yield different set of gates
-        # than supported by the QC hardware, this is also fixed by clean_opflow_circ
-        return _clean_opflow_circ(Gradient().get_gradient(operator=opflow, params=parameters))
-
-
-def _clean_opflow_circ(operator: OperatorBase, instruction_set=None) -> OperatorBase:
-    """
-    Function for removing ParameterExpression(0) terms from an opflow expression.
-    Transpiles all circuits in the opflow expression.
-    This fixes gate changes in the gradient() routine
-
-    Args:
-        operator : input opflow expression
-
-    Returns:
-        The opflow expression without the zero contributions and transpiled circuts
-    """
-
-    # We reached the Composed object or the wavefunction
-    if isinstance(operator, CircuitStateFn):
-        # If coefficient is zero replace by Zero @ One which is sorted out later
-        ZeroParameterExpr = False
-        if isinstance(operator.coeff, ParameterExpression):
-            # Check for ParameterExpression(0)
-            ZeroParameterExpr = operator.coeff.sympify() == 0
-        if operator.coeff != 0.0 and operator.coeff != 0 and ZeroParameterExpr == False:
-            if instruction_set is None:
-                return operator
-            else:
-                # Transpile back to the original basis set
-                transpiled_circ = transpile(
-                    operator.primitive,
-                    basis_gates=instruction_set,
-                    optimization_level=1,  # 1 for reducing number of gates
-                    layout_method="trivial",
-                )
-
-                transpiled_circ = operator.primitive
-                return CircuitStateFn(
-                    primitive=transpiled_circ,
-                    coeff=operator.coeff,
-                    is_measurement=operator.is_measurement,
-                )
-        else:
-            return ~Zero @ One
-    elif isinstance(operator, OperatorStateFn):
-        # Measurement operator -> do nothing
-        return operator
-    elif isinstance(operator, ComposedOp):
-        # If coefficient is zero replace by Zero @ One which is sorted out later
-        ZeroParameterExpr = False
-        if isinstance(operator.coeff, ParameterExpression):
-            # Check for ParameterExpression(0)
-            ZeroParameterExpr = operator.coeff.sympify() == 0
-        if operator.coeff != 0.0 and operator.coeff != 0 and ZeroParameterExpr == False:
-            # None-zero coefficient found, iterate through composed operators
-            op_list = [_clean_opflow_circ(op, instruction_set) for op in operator.oplist]
-            if ~Zero @ One in op_list:
-                return ~Zero @ One
-            else:
-                return ComposedOp(op_list, coeff=operator.coeff)
-        else:
-            return ~Zero @ One
-
-    elif isinstance(operator, ListOp):
-        # List object reached, recursive call of the function
-        op_list = [_clean_opflow_circ(op, instruction_set) for op in operator.oplist]
-
-        # Sort out the Zero @ One terms
-        if isinstance(operator, SummedOp):
-            return SummedOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, TensoredOp):
-            return TensoredOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, real_ListOp):
-            return ListOp(
-                oplist=[op for op in op_list if op != ~Zero @ One],
-                coeff=operator.coeff,
-                combo_fn=operator.combo_fn,
-            )
-        else:
-            raise ValueError("Unknown Type in ListOp")
-    else:
-        raise ValueError("Unknown Type in OperatorBase:", type(operator))
+from qiskit.circuit import ParameterVector, ParameterExpression
+from qiskit.circuit.parametervector import ParameterVectorElement
+from qiskit.opflow import CircuitSampler
+from qiskit.opflow import OperatorBase
+from qiskit.opflow import StateFn, CircuitStateFn, OperatorStateFn, DictStateFn
+from qiskit.opflow import SummedOp, ComposedOp, TensoredOp
+from qiskit.opflow import ListOp, PauliOp
+from qiskit.opflow import Zero, One
+from qiskit.compiler import transpile
+from qiskit.quantum_info import Pauli
+from qiskit.opflow import PauliOp
+from qiskit.opflow.gradients import Gradient
+from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
+import numpy as np
+from typing import Union
+
+from .feature_map_base import FeatureMapBase
+
+
+class FeatureMapDerivatives:
+    def __init__(
+        self,
+        feature_map: FeatureMapBase,
+        opflow_caching=True,
+    ):
+        self.feature_map = feature_map
+
+        self.x = ParameterVector("x", self.feature_map.num_features)
+        self.p = ParameterVector("p", self.feature_map.num_parameters)
+
+        circuit = feature_map.get_circuit(self.x, self.p)
+
+        # TODO transpiling
+
+        self.circuit_opflow = CircuitStateFn(primitive=circuit, coeff=1.0)
+
+        self.num_qubits = self.circuit_opflow.num_qubits
+
+        identity_measurement = StateFn(PauliOp(Pauli("I" * self.num_qubits)), is_measurement=True)
+        identity_measurement.replace = True
+
+        self.opflow = identity_measurement @ self.circuit_opflow
+
+        self.opflow_cache = {}
+        self.opflow_caching = opflow_caching
+
+        if self.opflow_caching:
+            self.opflow_cache["f"] = self.opflow
+
+        # get the instruction gates from the original circuit for transpiling the circuits back to this basis
+        self.instruction_set = set()
+        for instruction in circuit.data:
+            self.instruction_set.add(instruction.operation.name)
+        self.instruction_set = list(self.instruction_set)
+
+    def get_derivate(self, input: Union[str, tuple]):
+        """return the opflow structure of the circuit from the input"""
+        if isinstance(input, str):
+            if input == "I":
+                opflow = self.opflow
+            elif input == "dx":
+                opflow = self._differentiation_from_tuple((self.x,)).copy()
+            elif input == "dxdx":
+                opflow = self._differentiation_from_tuple((self.x, self.x)).copy()
+            elif input == "dpdxdx":
+                opflow = self._differentiation_from_tuple((self.p, self.x, self.x)).copy()
+            elif input == "laplace":
+                list_sum = []
+                for xi in self.x:
+                    list_sum.append(self._differentiation_from_tuple((xi, xi)).copy())
+                opflow = SummedOp(list_sum)
+            elif input == "laplace_dp":
+                list_sum = []
+                for xi in self.x:
+                    list_sum.append(self._differentiation_from_tuple((self.p, xi, xi)).copy())
+                opflow = SummedOp(list_sum)
+            elif input == "dp":
+                opflow = self._differentiation_from_tuple((self.p,)).copy()
+            elif input == "dpdp":
+                opflow = self._differentiation_from_tuple((self.p, self.p)).copy()
+            elif input == "dpdx":
+                opflow = self._differentiation_from_tuple((self.p, self.x)).copy()
+            else:
+                raise ValueError("Unknown string command:", input)
+        elif isinstance(input, tuple):
+            opflow = self._differentiation_from_tuple(input)
+        else:
+            raise TypeError("Input is neither string nor tuple, but:", type(input))
+
+        # remove mesurement operator
+
+        return _remove_measure(opflow)
+
+    def get_differentiation_from_tuple(self, diff_tuple: tuple):
+        return self.get_derivate(diff_tuple)
+
+    def get_derivation_from_string(self, input_string: str):
+        return self.get_derivate(input_string)
+
+    def _differentiation_from_tuple(self, diff_tuple: tuple):
+        """Recursive routine for automatic differentiating the feature map
+
+        Variables for the differentiation are supplied by a tuple
+        (x,param,param_op) from left to right -> ∂x ∂param ∂param_op PQC(x,param,param_op)
+
+
+        Args:
+            diff_tuple : tuple containing ParameterVectors or ParameterExpressions or Strings
+            determining the derivation
+            cost_op : String for specifying the used cost operator operator (default: None)
+                      (None or 'C' -> Standard, 'CC' -> Squared cost operator)
+        Returns:
+            The differentiated opflow expression
+        """
+        # TODO: outer function for input checking
+
+        if diff_tuple == ():
+            # Cancel the recursion by returning the opflow of the simply measured feature map
+            return self.opflow.copy()
+        else:
+            # Check if differentiating tuple is already stored in opflow_cache
+            if self.opflow_caching == True and (diff_tuple,) in self.opflow_cache:
+                # If stored -> return
+                return self.opflow_cache[(diff_tuple,)].copy()
+            else:
+                # Recursive differentiation with the most left object
+                circ = _opflow_differentiation(
+                    self._differentiation_from_tuple(diff_tuple[1:]), diff_tuple[0]
+                )
+                # Store result in the opflow_cache
+                if self.opflow_caching == True:
+                    self.opflow_cache[(diff_tuple,)] = circ
+                return circ
+
+    def get_parameter_vector(self):
+        return self.p
+
+    def get_feature_vector(self):
+        return self.x
+
+    @property
+    def num_parameters(self):
+        return len(self.p)
+
+    @property
+    def num_features(self):
+        return len(self.x)
+
+    def assign_parameters(self, opflow, features: np.ndarray, parameters: np.ndarray):
+        """
+        Assigns circuit parameters
+        """
+
+        if opflow == None:
+            return None
+
+        todo_list = []  # list for the variables
+        multi_list = []  # list of return ListOp or no list
+        param_list = []  # list of parameters that are substituted
+
+        # check shape of the x and adjust to [[]] form if necessary
+        if features is not None:
+            xx, multi_x = _adjust_input(features, len(self.x))
+            todo_list.append(xx)
+            param_list.append(self.x)
+            multi_list.append(multi_x)
+        if parameters is not None:
+            pp, multi_p = _adjust_input(parameters, len(self.p))
+            todo_list.append(pp)
+            param_list.append(self.p)
+            multi_list.append(multi_p)
+
+        # Recursive construction of the assignment dictionary and list structure
+        def rec_assign(dic, todo_list, param_list, multi_list):
+            if len(todo_list) <= 0:
+                return None
+            return_list = []
+            for x_ in todo_list[0]:
+                for A, B in zip(param_list[0], x_):
+                    dic[A] = B
+                if len(multi_list[1:]) > 0:
+                    return_list.append(
+                        rec_assign(dic.copy(), todo_list[1:], param_list[1:], multi_list[1:])
+                    )
+                else:
+                    return_list.append(opflow.assign_parameters(dic))
+
+            if multi_list[0]:
+                return ListOp(return_list)
+            else:
+                return return_list[0]
+
+        return rec_assign({}, todo_list, param_list, multi_list)
+
+
+def _adjust_input(x, x_length):
+    # check shape of the x and adjust to [[]] form if necessary
+    multiple_inputs = False
+    error = False
+    shape = np.shape(x)
+    if shape == () and x_length == 1:
+        # Single floating point number
+        xx = np.array([[x]])
+    elif len(shape) == 1:
+        if x_length == 1:
+            xx = np.array([np.array([xx]) for xx in x])
+            multiple_inputs = True
+        else:
+            # We have a single multi dimensional x (e.g. parameter vector)
+            if len(x) == x_length:
+                xx = np.array([x])
+            else:
+                error = True
+    elif len(shape) == 2:
+        if shape[1] == x_length:
+            xx = x
+            multiple_inputs = True
+        else:
+            error = True
+    else:
+        error = True
+
+    if error:
+        raise ValueError("Wrong format of an input variable.")
+
+    return xx, multiple_inputs
+
+
+def _remove_measure(operator: OperatorBase) -> OperatorBase:
+    """
+    Replace all flagged measurements in the input opflow expression
+    Recursive function
+
+    Args:
+        operator : Opflow expression
+        measurement : new measurement operator
+    Returns:
+        New opflow expression with replaced measurement operator
+    """
+    # We reached a ComposedOp term -> replace the measurement
+    if isinstance(operator, ComposedOp):
+        for i in range(len(operator.oplist)):
+            if isinstance(operator.oplist[i], CircuitStateFn):
+                return_op = operator.oplist[i]
+                return_op._coeff = operator.coeff
+                return return_op
+
+        return ~Zero @ One
+
+    # We reached a CircuitStateFn term -> apply the measurement to the wavefunction
+    elif isinstance(operator, CircuitStateFn):
+        return operator
+
+    # We reached a list of opflow terms, recursive call of
+    # the function to all children in the list
+    elif isinstance(operator, ListOp):
+        op_list = [_remove_measure(op) for op in operator.oplist]
+
+        if isinstance(operator, SummedOp):
+            return SummedOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, TensoredOp):
+            return TensoredOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, real_ListOp):
+            return ListOp(
+                oplist=[op for op in op_list if op != ~Zero @ One],
+                coeff=operator.coeff,
+                combo_fn=operator.combo_fn,
+            )
+        else:
+            raise ValueError("Unknown ListOp type in _remove_measure:", type(operator))
+    else:
+        raise ValueError("Unknown type in _remove_measure:", type(operator))
+
+
+def measure_feature_map_derivative(operator: OperatorBase, measurement) -> OperatorBase:
+    """
+    Replace all flagged measurements in the input opflow expression
+    Recursive function
+
+    Args:
+        operator : Opflow expression
+        measurement : new measurement operator
+    Returns:
+        New opflow expression with replaced measurement operator
+    """
+    # We reached a ComposedOp term -> replace the measurement
+    if isinstance(operator, ComposedOp):
+        for i in range(len(operator.oplist)):
+            if isinstance(operator.oplist[i], OperatorStateFn):
+                if hasattr(operator.oplist[i], "replace"):
+                    if operator.oplist[i].replace:
+                        operator.oplist[i] = measurement
+                else:
+                    operator.oplist[i] = measurement
+        return operator
+
+    # We reached a CircuitStateFn term -> apply the measurement to the wavefunction
+    elif isinstance(operator, CircuitStateFn):
+        coeff = operator._coeff
+        operator._coeff = 1.0
+        measured_op = measurement @ operator
+        measured_op._coeff = coeff
+        return measured_op
+
+    # We reached a list of opflow terms, recursive call of
+    # the function to all children in the list
+    elif isinstance(operator, ListOp):
+        op_list = [measure_feature_map_derivative(op, measurement) for op in operator.oplist]
+
+        if isinstance(operator, SummedOp):
+            return SummedOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, TensoredOp):
+            return TensoredOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, real_ListOp):
+            return ListOp(
+                oplist=[op for op in op_list if op != ~Zero @ One],
+                coeff=operator.coeff,
+                combo_fn=operator.combo_fn,
+            )
+        else:
+            raise ValueError("Unknown ListOp type in measure_derivative:", type(operator))
+    else:
+        raise ValueError("Unknown type in measure_derivative:", type(operator))
+
+
+def _opflow_differentiation(opflow, parameters):
+    """
+    Routine for the automatic differentiation based on qiskit routines
+
+    Args:
+        opflow : Input opflow expression
+        params (list | ParameterVector): variables which are used in the
+                                            differentiation (have to be the same type )
+    Returns:
+        opflow structure of the differentiated input opflow
+    """
+
+    # Make list if input is not a list
+    if isinstance(parameters, ParameterVectorElement):
+        parameters = [parameters]
+    if isinstance(parameters, tuple):
+        parameters = list(parameters)
+
+    # Call the automatic differentiation routine
+    # Separate routine for for one dim. or multi dim. variables
+    if len(parameters) == 1:
+        # Automatic qiskit differentiation
+        # ParameterExpression(0) is removed by clean_opflow_circ
+        # Gates are transpiled in Gradient(), this can yield different set of gates
+        # than supported by the QC hardware, this is also fixed by clean_opflow_circ
+        return _clean_opflow_circ(Gradient().convert(operator=opflow, params=parameters)[0])
+    else:
+        # If multiple variables are differentiated -> results are returned in array
+
+        # Check if the same variables are the same type
+        params_name = parameters[0].name.split("[", 1)[0]
+        for p in parameters:
+            if p.name.split("[", 1)[0] != params_name:
+                raise TypeError("Differentiable variables are not the same type.")
+
+        # Automatic qiskit differentiation
+        # ParameterExpression(0) is removed by clean_opflow_circ
+        # Gates are transpiled in Gradient(), this can yield different set of gates
+        # than supported by the QC hardware, this is also fixed by clean_opflow_circ
+        return _clean_opflow_circ(Gradient().get_gradient(operator=opflow, params=parameters))
+
+
+def _clean_opflow_circ(operator: OperatorBase, instruction_set=None) -> OperatorBase:
+    """
+    Function for removing ParameterExpression(0) terms from an opflow expression.
+    Transpiles all circuits in the opflow expression.
+    This fixes gate changes in the gradient() routine
+
+    Args:
+        operator : input opflow expression
+
+    Returns:
+        The opflow expression without the zero contributions and transpiled circuts
+    """
+
+    # We reached the Composed object or the wavefunction
+    if isinstance(operator, CircuitStateFn):
+        # If coefficient is zero replace by Zero @ One which is sorted out later
+        ZeroParameterExpr = False
+        if isinstance(operator.coeff, ParameterExpression):
+            # Check for ParameterExpression(0)
+            ZeroParameterExpr = operator.coeff.sympify() == 0
+        if operator.coeff != 0.0 and operator.coeff != 0 and ZeroParameterExpr == False:
+            if instruction_set is None:
+                return operator
+            else:
+                # Transpile back to the original basis set
+                transpiled_circ = transpile(
+                    operator.primitive,
+                    basis_gates=instruction_set,
+                    optimization_level=1,  # 1 for reducing number of gates
+                    layout_method="trivial",
+                )
+
+                transpiled_circ = operator.primitive
+                return CircuitStateFn(
+                    primitive=transpiled_circ,
+                    coeff=operator.coeff,
+                    is_measurement=operator.is_measurement,
+                )
+        else:
+            return ~Zero @ One
+    elif isinstance(operator, OperatorStateFn):
+        # Measurement operator -> do nothing
+        return operator
+    elif isinstance(operator, ComposedOp):
+        # If coefficient is zero replace by Zero @ One which is sorted out later
+        ZeroParameterExpr = False
+        if isinstance(operator.coeff, ParameterExpression):
+            # Check for ParameterExpression(0)
+            ZeroParameterExpr = operator.coeff.sympify() == 0
+        if operator.coeff != 0.0 and operator.coeff != 0 and ZeroParameterExpr == False:
+            # None-zero coefficient found, iterate through composed operators
+            op_list = [_clean_opflow_circ(op, instruction_set) for op in operator.oplist]
+            if ~Zero @ One in op_list:
+                return ~Zero @ One
+            else:
+                return ComposedOp(op_list, coeff=operator.coeff)
+        else:
+            return ~Zero @ One
+
+    elif isinstance(operator, ListOp):
+        # List object reached, recursive call of the function
+        op_list = [_clean_opflow_circ(op, instruction_set) for op in operator.oplist]
+
+        # Sort out the Zero @ One terms
+        if isinstance(operator, SummedOp):
+            return SummedOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, TensoredOp):
+            return TensoredOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, real_ListOp):
+            return ListOp(
+                oplist=[op for op in op_list if op != ~Zero @ One],
+                coeff=operator.coeff,
+                combo_fn=operator.combo_fn,
+            )
+        else:
+            raise ValueError("Unknown Type in ListOp")
+    else:
+        raise ValueError("Unknown Type in OperatorBase:", type(operator))
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/cheb_pqc.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/cheb_pqc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-from ..feature_map_base import FeatureMapBase
-
-
-class ChebPQC(FeatureMapBase):
-    """
-    Cheb PQC feature map
-
-    -Ry(p)-[-Rx(p*arcos(x))-c-----------Rz(p)-]-Ry(p)-
-    -Ry(p)-[-Rx(p*arcos(x))-Rz(p)-c-----|-----]-Ry(p)-
-    -Ry(p)-[-Rx(p*arcos(x))-c-----Rz(p)-|-----]-Ry(p)-
-    -Ry(p)-[-Rx(p*arcos(x))-Rz(p)-------c ----]-Ry(p)-
-                  repeated by num_layers
-
-    Args:
-        num_qubits (int): Number of qubits of the ChebPQC feature map
-        num_features (int): Dimension of the feature vector
-        num_layers (int): Number of layers of the arcos encoding and the two qubit manipulation (default: 1)
-        closed (bool): If true, the last and the first qubit are entangled;
-                       not necessarily hardware efficient! (default: true)
-    """
-
-    def __init__(
-        self,
-        num_qubits: int,
-        num_features: int,
-        num_layers: int = 1,
-        closed: bool = True,
-        entangling_gate: str = 'crz'
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-        self.num_layers = num_layers
-        self.closed = closed
-        self.entangling_gate = entangling_gate
-        if self.entangling_gate not in ('crz','rzz'):
-            raise ValueError("Unknown value for entangling_gate: ", entangling_gate)
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns th e numbeself)r of trainable parameters of the Cheb PQC feature map."""
-        num_param = 2 * self.num_qubits + self.num_qubits * self.num_layers
-        if self.closed:
-            num_param += self.num_qubits * self.num_layers
-        else:
-            num_param += (self.num_qubits - 1) * self.num_layers
-        return num_param
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Returns the circuit of the Cheb PQC feature map
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in Qiskit's QuantumCircuit format
-        """
-        nfeature = len(features)
-        nparam = len(parameters)
-        QC = QuantumCircuit(self.num_qubits)
-        ioff = 0
-
-        if self.entangling_gate == "crz":
-            egate = QC.crz
-        elif self.entangling_gate == "rzz":
-            egate = QC.rzz
-        else:
-            raise ValueError("Unknown entangling gate")
-
-        for i in range(self.num_qubits):
-            QC.ry(parameters[ioff % nparam], i)
-            ioff = ioff + 1
-
-        for ilayer in range(self.num_layers):
-            # Chebyshev feature map
-            for i in range(self.num_qubits):
-                QC.rx(self.__phi_map(parameters[ioff % nparam], features[i % nfeature]), i)
-                ioff = ioff + 1
-
-            for i in range(0, self.num_qubits, 2):
-                egate(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                ioff = ioff + 1
-
-            if self.num_qubits > 2:
-                if self.closed:
-                    istop = self.num_qubits
-                else:
-                    istop = self.num_qubits - 1
-                for i in range(1, istop, 2):
-                    egate(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                    ioff = ioff + 1
-
-        for i in range(self.num_qubits):
-            QC.ry(parameters[ioff % nparam], i)
-            ioff = ioff + 1
-
-        return QC
-
-    def __phi_map(self, a, x):
-        """Helper function for returning a*arccos(x)"""
-        return a * np.arccos(x)
-
-    def get_cheb_indices(self):
-        """
-        Returns a nested list of the indices of the parameters involved
-        in the arccos encoding.
-        The outer list is connected to the layers of the feature map.
-        """
-        cheb_index = []
-        ioff = self.num_qubits
-        for ilayer in range(self.num_layers):
-            cheb_index_layer = []
-            for i in range(self.num_qubits):
-                cheb_index_layer.append(ioff)
-                ioff = ioff + 1
-
-            for i in range(0, self.num_qubits, 2):
-                ioff = ioff + 1
-
-            if self.num_qubits > 2:
-                if self.closed:
-                    istop = self.num_qubits
-                else:
-                    istop = self.num_qubits - 1
-                for i in range(1, istop, 2):
-                    ioff = ioff + 1
-            cheb_index.append(cheb_index_layer)
-        return cheb_index
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+from ..feature_map_base import FeatureMapBase
+
+
+class ChebPQC(FeatureMapBase):
+    """
+    Cheb PQC feature map
+
+    -Ry(p)-[-Rx(p*arcos(x))-c-----------Rz(p)-]-Ry(p)-
+    -Ry(p)-[-Rx(p*arcos(x))-Rz(p)-c-----|-----]-Ry(p)-
+    -Ry(p)-[-Rx(p*arcos(x))-c-----Rz(p)-|-----]-Ry(p)-
+    -Ry(p)-[-Rx(p*arcos(x))-Rz(p)-------c ----]-Ry(p)-
+                  repeated by num_layers
+
+    Args:
+        num_qubits (int): Number of qubits of the ChebPQC feature map
+        num_features (int): Dimension of the feature vector
+        num_layers (int): Number of layers of the arcos encoding and the two qubit manipulation (default: 1)
+        closed (bool): If true, the last and the first qubit are entangled;
+                       not necessarily hardware efficient! (default: true)
+    """
+
+    def __init__(
+        self,
+        num_qubits: int,
+        num_features: int,
+        num_layers: int = 1,
+        closed: bool = True,
+        entangling_gate: str = "crz",
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+        self.num_layers = num_layers
+        self.closed = closed
+        self.entangling_gate = entangling_gate
+        if self.entangling_gate not in ("crz", "rzz"):
+            raise ValueError("Unknown value for entangling_gate: ", entangling_gate)
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns th e numbeself)r of trainable parameters of the Cheb PQC feature map."""
+        num_param = 2 * self.num_qubits + self.num_qubits * self.num_layers
+        if self.closed:
+            num_param += self.num_qubits * self.num_layers
+        else:
+            num_param += (self.num_qubits - 1) * self.num_layers
+        return num_param
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Returns the circuit of the Cheb PQC feature map
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in Qiskit's QuantumCircuit format
+        """
+        nfeature = len(features)
+        nparam = len(parameters)
+        QC = QuantumCircuit(self.num_qubits)
+        ioff = 0
+
+        if self.entangling_gate == "crz":
+            egate = QC.crz
+        elif self.entangling_gate == "rzz":
+            egate = QC.rzz
+        else:
+            raise ValueError("Unknown entangling gate")
+
+        for i in range(self.num_qubits):
+            QC.ry(parameters[ioff % nparam], i)
+            ioff = ioff + 1
+
+        for ilayer in range(self.num_layers):
+            # Chebyshev feature map
+            for i in range(self.num_qubits):
+                QC.rx(self.__phi_map(parameters[ioff % nparam], features[i % nfeature]), i)
+                ioff = ioff + 1
+
+            for i in range(0, self.num_qubits, 2):
+                egate(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                ioff = ioff + 1
+
+            if self.num_qubits > 2:
+                if self.closed:
+                    istop = self.num_qubits
+                else:
+                    istop = self.num_qubits - 1
+                for i in range(1, istop, 2):
+                    egate(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                    ioff = ioff + 1
+
+        for i in range(self.num_qubits):
+            QC.ry(parameters[ioff % nparam], i)
+            ioff = ioff + 1
+
+        return QC
+
+    def __phi_map(self, a, x):
+        """Helper function for returning a*arccos(x)"""
+        return a * np.arccos(x)
+
+    def get_cheb_indices(self):
+        """
+        Returns a nested list of the indices of the parameters involved
+        in the arccos encoding.
+        The outer list is connected to the layers of the feature map.
+        """
+        cheb_index = []
+        ioff = self.num_qubits
+        for ilayer in range(self.num_layers):
+            cheb_index_layer = []
+            for i in range(self.num_qubits):
+                cheb_index_layer.append(ioff)
+                ioff = ioff + 1
+
+            for i in range(0, self.num_qubits, 2):
+                ioff = ioff + 1
+
+            if self.num_qubits > 2:
+                if self.closed:
+                    istop = self.num_qubits
+                else:
+                    istop = self.num_qubits - 1
+                for i in range(1, istop, 2):
+                    ioff = ioff + 1
+            cheb_index.append(cheb_index_layer)
+        return cheb_index
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/cheb_rx.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/cheb_rx.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-from ..feature_map_base import FeatureMapBase
-
-
-class ChebRx(FeatureMapBase):
-    """
-    ChebRx feature map
-
-    -[-Rx(p*arcos(x))-Rx(p)-c-----]-
-    -[-Rx(p*arcos(x))-Rx(p)-X-c---]-
-    -[-Rx(p*arcos(x))-Rx(p)---X-c-]-
-    -[-Rx(p*arcos(x))-Rx(p)-----X-]-
-
-    [] = is repeated by num_layers
-
-    Args:
-        num_qubits (int): Number of qubits of the ChebRx feature map
-        num_features (int): Dimension of the feature vector
-        num_layers (int): Number of repetitions (default: 1)
-    """
-
-    def __init__(self, num_qubits: int, num_features: int, num_layers: int = 1) -> None:
-        super().__init__(num_qubits, num_features)
-        self.num_layers = num_layers
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the ChebRx feature map."""
-        return 2 * self.num_qubits * self.num_layers
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Returns the circuit of the ChebRx feature map
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in Qiskit's QuantumCircuit format
-        """
-        nfeature = len(features)
-        nparam = len(parameters)
-        QC = QuantumCircuit(self.num_qubits)
-        ioff = 0
-        for ilayer in range(self.num_layers):
-            # Chebyshev feature map
-            for i in range(self.num_qubits):
-                QC.rx(self.__phi_map(parameters[ioff % nparam], features[i % nfeature]), i)
-                ioff = ioff + 1
-            # Trafo
-            for i in range(self.num_qubits):
-                QC.rx(parameters[ioff % nparam], i)
-                ioff = ioff + 1
-            QC = self.__entangle_layer(QC)
-
-        return QC
-
-    def __entangle_layer(self, QC: QuantumCircuit) -> QuantumCircuit:
-        """
-        Creation of a simple nearest neighbor entangling layer
-        """
-        for i in range(0, self.num_qubits - 1, 2):
-            QC.cx(i, i + 1)
-        for i in range(1, self.num_qubits - 1, 2):
-            QC.cx(i, i + 1)
-        return QC
-
-    def __phi_map(self, a, x):
-        """Helper function for returning a*arccos(x)"""
-        return a * np.arccos(x)
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+from ..feature_map_base import FeatureMapBase
+
+
+class ChebRx(FeatureMapBase):
+    """
+    ChebRx feature map
+
+    -[-Rx(p*arcos(x))-Rx(p)-c-----]-
+    -[-Rx(p*arcos(x))-Rx(p)-X-c---]-
+    -[-Rx(p*arcos(x))-Rx(p)---X-c-]-
+    -[-Rx(p*arcos(x))-Rx(p)-----X-]-
+
+    [] = is repeated by num_layers
+
+    Args:
+        num_qubits (int): Number of qubits of the ChebRx feature map
+        num_features (int): Dimension of the feature vector
+        num_layers (int): Number of repetitions (default: 1)
+    """
+
+    def __init__(self, num_qubits: int, num_features: int, num_layers: int = 1) -> None:
+        super().__init__(num_qubits, num_features)
+        self.num_layers = num_layers
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the ChebRx feature map."""
+        return 2 * self.num_qubits * self.num_layers
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Returns the circuit of the ChebRx feature map
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in Qiskit's QuantumCircuit format
+        """
+        nfeature = len(features)
+        nparam = len(parameters)
+        QC = QuantumCircuit(self.num_qubits)
+        ioff = 0
+        for ilayer in range(self.num_layers):
+            # Chebyshev feature map
+            for i in range(self.num_qubits):
+                QC.rx(self.__phi_map(parameters[ioff % nparam], features[i % nfeature]), i)
+                ioff = ioff + 1
+            # Trafo
+            for i in range(self.num_qubits):
+                QC.rx(parameters[ioff % nparam], i)
+                ioff = ioff + 1
+            QC = self.__entangle_layer(QC)
+
+        return QC
+
+    def __entangle_layer(self, QC: QuantumCircuit) -> QuantumCircuit:
+        """
+        Creation of a simple nearest neighbor entangling layer
+        """
+        for i in range(0, self.num_qubits - 1, 2):
+            QC.cx(i, i + 1)
+        for i in range(1, self.num_qubits - 1, 2):
+            QC.cx(i, i + 1)
+        return QC
+
+    def __phi_map(self, a, x):
+        """Helper function for returning a*arccos(x)"""
+        return a * np.arccos(x)
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/chebyshev_tower.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/chebyshev_tower.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-from ..feature_map_base import FeatureMapBase
-
-
-class ChebyshevTower(FeatureMapBase):
-    """
-    Creates a featurmap based on Chebyshev polynomials created by Ry(arcos(x))
-
-    One layer has the following structure (for n_chebyshev = 2):
-
-    -H-Ry(alpha*1*arcos(x0))-.---
-    -H-Ry(alpha*2*arcos(x0))-x-.-
-    -H-Ry(alpha*1*arcos(x1))-.-x-
-    -H-Ry(alpha*2*arcos(x1))-x---
-
-    The structure of the Chebyshev feature map reads:
-    0-Layer1-Layer2- ...
-
-    Args:
-        num_qubits (int): Number of Qubits
-        num_features (int): Dimension of feature vector
-        n_chebyshev (int): Number of Chebyshev terms per feature
-        alpha (float): scaling factor of Chebyshev tower
-        num_layers (int): Number of layers
-    """
-
-    def __init__(
-        self,
-        num_qubits: int,
-        num_features: int,
-        n_chebyshev: int,
-        alpha: float = 1.0,
-        num_layers: int = 1,
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-
-        self.n_chebyshev = n_chebyshev
-        self.alpha = alpha
-        self.num_layers = num_layers
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the feature map."""
-        return 0
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray] = None,
-    ) -> QuantumCircuit:
-        """
-        Generates and returns the circuit of the Chebyshev feature map
-        """
-
-        if self.num_features != len(features):
-            raise ValueError("Wrong number of features")
-
-        if parameters is not None:
-            if len(parameters) != 0:
-                raise ValueError("No parameters are needed!")
-
-        # Create the circuit
-        QC = QuantumCircuit(self.num_qubits)
-        for ilayer in range(self.num_layers):
-            QC.h(range(self.num_qubits))
-            # Loops through the data encoding gates
-            ifeature = 0
-            for i in range(self.num_features):
-                for icheb in range(self.n_chebyshev):
-                    QC.ry(
-                        self._phi_map(features[i], icheb + 1),
-                        ifeature % self.num_qubits,
-                    )
-                    ifeature += 1
-            # Entangling layer
-            if ilayer + 1 < self.num_layers:
-                QC = self._entangle_layer(QC)
-
-        return QC
-
-    def _entangle_layer(self, QC: QuantumCircuit):
-        """
-        Creation of a simple NN entangling layer
-
-        Args:
-            QC (QuantumCircuit): Quantum circuit
-
-        Returns:
-            Returns the Quantum circuit with a NN entangling layer added
-        """
-        for i in range(0, self.num_qubits - 1, 2):
-            QC.cx(i, i + 1)
-        for i in range(
-            1,
-            self.num_qubits - 1,
-            2,
-        ):
-            QC.cx(i, i + 1)
-        return QC
-
-    def _phi_map(self, x, i):
-        """
-        Non-linear mapping for x: alpha*i*arccos(x)
-
-        Args:
-            x: x for arcos
-            i: factor i
-
-        Returns:
-            alpha*i*arccos(x)
-        """
-        return self.alpha * i * np.arccos(x)
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+from ..feature_map_base import FeatureMapBase
+
+
+class ChebyshevTower(FeatureMapBase):
+    """
+    Creates a featurmap based on Chebyshev polynomials created by Ry(arcos(x))
+
+    One layer has the following structure (for n_chebyshev = 2):
+
+    -H-Ry(alpha*1*arcos(x0))-.---
+    -H-Ry(alpha*2*arcos(x0))-x-.-
+    -H-Ry(alpha*1*arcos(x1))-.-x-
+    -H-Ry(alpha*2*arcos(x1))-x---
+
+    The structure of the Chebyshev feature map reads:
+    0-Layer1-Layer2- ...
+
+    Args:
+        num_qubits (int): Number of Qubits
+        num_features (int): Dimension of feature vector
+        n_chebyshev (int): Number of Chebyshev terms per feature
+        alpha (float): scaling factor of Chebyshev tower
+        num_layers (int): Number of layers
+    """
+
+    def __init__(
+        self,
+        num_qubits: int,
+        num_features: int,
+        n_chebyshev: int,
+        alpha: float = 1.0,
+        num_layers: int = 1,
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+
+        self.n_chebyshev = n_chebyshev
+        self.alpha = alpha
+        self.num_layers = num_layers
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the feature map."""
+        return 0
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray] = None,
+    ) -> QuantumCircuit:
+        """
+        Generates and returns the circuit of the Chebyshev feature map
+        """
+
+        if self.num_features != len(features):
+            raise ValueError("Wrong number of features")
+
+        if parameters is not None:
+            if len(parameters) != 0:
+                raise ValueError("No parameters are needed!")
+
+        # Create the circuit
+        QC = QuantumCircuit(self.num_qubits)
+        for ilayer in range(self.num_layers):
+            QC.h(range(self.num_qubits))
+            # Loops through the data encoding gates
+            ifeature = 0
+            for i in range(self.num_features):
+                for icheb in range(self.n_chebyshev):
+                    QC.ry(
+                        self._phi_map(features[i], icheb + 1),
+                        ifeature % self.num_qubits,
+                    )
+                    ifeature += 1
+            # Entangling layer
+            if ilayer + 1 < self.num_layers:
+                QC = self._entangle_layer(QC)
+
+        return QC
+
+    def _entangle_layer(self, QC: QuantumCircuit):
+        """
+        Creation of a simple NN entangling layer
+
+        Args:
+            QC (QuantumCircuit): Quantum circuit
+
+        Returns:
+            Returns the Quantum circuit with a NN entangling layer added
+        """
+        for i in range(0, self.num_qubits - 1, 2):
+            QC.cx(i, i + 1)
+        for i in range(
+            1,
+            self.num_qubits - 1,
+            2,
+        ):
+            QC.cx(i, i + 1)
+        return QC
+
+    def _phi_map(self, x, i):
+        """
+        Non-linear mapping for x: alpha*i*arccos(x)
+
+        Args:
+            x: x for arcos
+            i: factor i
+
+        Returns:
+            alpha*i*arccos(x)
+        """
+        return self.alpha * i * np.arccos(x)
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/highdim_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/highdim_feature_map.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,189 +1,189 @@
-import numpy as np
-from typing import Union
-from qiskit import QuantumCircuit
-from qiskit.circuit import ParameterVector
-from qiskit.quantum_info.operators import Operator
-
-from ..feature_map_base import FeatureMapBase
-
-
-class HighDimFeatureMap(FeatureMapBase):
-    """
-    High-dimensional feature map from https://doi.org/10.1103/PhysRevA.106.042431
-
-    Inputs:
-        num_qubits (int): Number of Qubits of the feature map
-        num_features (int): Dimension of the feature vector
-
-        cycling (bool): If true, the assignment of gates cycles, i.e. if reaching the last feature x_n,
-                    the layer is filled by starting again from the first feature
-                    (e.g. Rz(x_n)-Ry(x0)-Rz(x1)).
-                    If false, the gates are left out after reaching feature x_n
-
-        cycling_type (str): Defines, how the indices are cycled
-                        'saw' : restarts by 0, e.g. 0,1,2,3,0,1,2,3 (recommended)
-                        'hat' : goes up and then down, e.g. 0,1,2,3,2,1,0,1,2,3
-
-        number_of_layers (int): Sets the number of layer repetitions. If not given, the number of layers
-                            is determined automatically by the number of features and qubits.
-                            If the given number of layers
-
-        layer_type (str): Defines in which directions the features are assigned to the gates:
-                    'columns': assignment as shown above
-                    'rows': assignment in rows, e.g. -Rz(x0)-Ry(x2)-Rz(x4)-|iSWAP|-
-                                                     -Rz(x1)-Ry(x3)-Rz(x5)-|     |-
-    """
-
-    def __init__(
-        self,
-        num_qubits: int,
-        num_features: int,
-        cycling: bool = True,
-        cycling_type: str = "saw",
-        num_layers: int = -1,
-        layer_type: str = "rows",
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-
-        self.cycling = cycling
-        self.cycling_type = cycling_type
-        self.num_layers = num_layers
-        self.layer_type = layer_type
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the feature map."""
-        return 0
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray] = None,
-    ) -> QuantumCircuit:
-        """
-        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit pf the high-dimensional feature map
-        """
-
-        if self.num_features != len(features):
-            raise ValueError("Wrong number of features")
-
-        if parameters is not None:
-            if len(parameters) != 0:
-                raise ValueError("No parameters are needed!")
-
-        # Initialize circuit and start with the Hadamard gate
-        QC = QuantumCircuit(self.num_qubits)
-        qubit_list = range(self.num_qubits)
-        QC.h(qubit_list)
-
-        # Determine the number of layers
-        num_layers = int(self.num_features / (self.num_qubits * 3)) + 1
-
-        # Overwrite number of layers if given by the user
-        if self.num_layers > 0:
-            if self.num_layers < num_layers:
-                raise RuntimeError("Not all features are represented in the feature map!")
-            num_layers = self.num_layers
-
-        # Loop through the layers
-        ioff = 0
-        for i in range(num_layers):
-            if i != 0:
-                QC = self._entangle_layer_iswap(QC)
-            QC = self._build_layer(QC, features, ioff)
-            ioff = ioff + self.num_qubits * 3
-            if self.cycling == False and ioff >= self.num_features:
-                ioff = 0
-
-        return QC
-
-    def _build_layer(self, QC: QuantumCircuit, feature_vec: ParameterVector, ioff: int):
-        """
-        Private function which creates a single layer
-        """
-        if self.layer_type == "rows":
-            rows = True
-        elif self.layer_type == "columns":
-            rows = False
-        else:
-            raise ValueError("Unknown layer type:", self.layer_type)
-
-        # Loop through all 3*n_qubit gates in this layer
-        for i in range(3 * self.num_qubits):
-            # Determine qubit of the gate, depending on row or column counting
-            if rows:
-                iqubit = int(i / 3)
-            else:
-                iqubit = i % self.num_qubits
-
-            # Determine the index of the feature (x_i)
-            ii = ioff + i
-            if self.cycling:
-                if self.cycling_type == "saw":
-                    ii = ii % self.num_features
-                elif self.cycling_type == "hat":  # todo better name
-                    itest = ii % max(self.num_features + self.num_features - 2, 1)
-                    if itest >= self.num_features:
-                        ii = self.num_features + self.num_features - 2 - itest
-                    else:
-                        ii = itest
-                else:
-                    raise ValueError("Unknown cycling type!")
-
-            # Terminate if all features in this layer have been addressed
-            if iqubit >= self.num_qubits or ii >= self.num_features:
-                break
-
-            # Create Rz and Ry gates
-            if rows:
-                if i % 3 == 0:
-                    QC.rz(feature_vec[ii], iqubit)
-                elif i % 3 == 1:
-                    QC.ry(feature_vec[ii], iqubit)
-                else:  # i % 3 == 2
-                    QC.rz(feature_vec[ii], iqubit)
-            else:
-                if int(i / self.num_qubits) == 0:
-                    QC.rz(feature_vec[ii], iqubit)
-                elif int(i / self.num_qubits) == 1:
-                    QC.ry(feature_vec[ii], iqubit)
-                else:  # int(i/self.num_qubits) == 2
-                    QC.rz(feature_vec[ii], iqubit)
-
-        return QC
-
-    def _entangle_layer_iswap(self, QC: QuantumCircuit):
-        """
-        Private function which creates the entangeling layer by iSWAP neighboring qubits
-        """
-
-        # Manually build the iSWAP operator, since it is not available in Qiskit
-        iswap_op = Operator(
-            [
-                [1, 0, 0, 0],
-                [0, 1 / np.sqrt(2), 1j / np.sqrt(2), 0],
-                [0, 1j / np.sqrt(2), 1 / np.sqrt(2), 0],
-                [0, 0, 0, 1],
-            ]
-        )
-
-        # Build the layer
-        for i in range(0, self.num_qubits - 1, 2):
-            QC.unitary(iswap_op, [i, i + 1], label="iswap")
-        for i in range(
-            1,
-            self.num_qubits - 1,
-            2,
-        ):
-            QC.unitary(iswap_op, [i, i + 1], label="iswap")
-
-        return QC
+import numpy as np
+from typing import Union
+from qiskit import QuantumCircuit
+from qiskit.circuit import ParameterVector
+from qiskit.quantum_info.operators import Operator
+
+from ..feature_map_base import FeatureMapBase
+
+
+class HighDimFeatureMap(FeatureMapBase):
+    """
+    High-dimensional feature map from https://doi.org/10.1103/PhysRevA.106.042431
+
+    Inputs:
+        num_qubits (int): Number of Qubits of the feature map
+        num_features (int): Dimension of the feature vector
+
+        cycling (bool): If true, the assignment of gates cycles, i.e. if reaching the last feature x_n,
+                    the layer is filled by starting again from the first feature
+                    (e.g. Rz(x_n)-Ry(x0)-Rz(x1)).
+                    If false, the gates are left out after reaching feature x_n
+
+        cycling_type (str): Defines, how the indices are cycled
+                        'saw' : restarts by 0, e.g. 0,1,2,3,0,1,2,3 (recommended)
+                        'hat' : goes up and then down, e.g. 0,1,2,3,2,1,0,1,2,3
+
+        number_of_layers (int): Sets the number of layer repetitions. If not given, the number of layers
+                            is determined automatically by the number of features and qubits.
+                            If the given number of layers
+
+        layer_type (str): Defines in which directions the features are assigned to the gates:
+                    'columns': assignment as shown above
+                    'rows': assignment in rows, e.g. -Rz(x0)-Ry(x2)-Rz(x4)-|iSWAP|-
+                                                     -Rz(x1)-Ry(x3)-Rz(x5)-|     |-
+    """
+
+    def __init__(
+        self,
+        num_qubits: int,
+        num_features: int,
+        cycling: bool = True,
+        cycling_type: str = "saw",
+        num_layers: int = -1,
+        layer_type: str = "rows",
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+
+        self.cycling = cycling
+        self.cycling_type = cycling_type
+        self.num_layers = num_layers
+        self.layer_type = layer_type
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the feature map."""
+        return 0
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray] = None,
+    ) -> QuantumCircuit:
+        """
+        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit pf the high-dimensional feature map
+        """
+
+        if self.num_features != len(features):
+            raise ValueError("Wrong number of features")
+
+        if parameters is not None:
+            if len(parameters) != 0:
+                raise ValueError("No parameters are needed!")
+
+        # Initialize circuit and start with the Hadamard gate
+        QC = QuantumCircuit(self.num_qubits)
+        qubit_list = range(self.num_qubits)
+        QC.h(qubit_list)
+
+        # Determine the number of layers
+        num_layers = int(self.num_features / (self.num_qubits * 3)) + 1
+
+        # Overwrite number of layers if given by the user
+        if self.num_layers > 0:
+            if self.num_layers < num_layers:
+                raise RuntimeError("Not all features are represented in the feature map!")
+            num_layers = self.num_layers
+
+        # Loop through the layers
+        ioff = 0
+        for i in range(num_layers):
+            if i != 0:
+                QC = self._entangle_layer_iswap(QC)
+            QC = self._build_layer(QC, features, ioff)
+            ioff = ioff + self.num_qubits * 3
+            if self.cycling == False and ioff >= self.num_features:
+                ioff = 0
+
+        return QC
+
+    def _build_layer(self, QC: QuantumCircuit, feature_vec: ParameterVector, ioff: int):
+        """
+        Private function which creates a single layer
+        """
+        if self.layer_type == "rows":
+            rows = True
+        elif self.layer_type == "columns":
+            rows = False
+        else:
+            raise ValueError("Unknown layer type:", self.layer_type)
+
+        # Loop through all 3*n_qubit gates in this layer
+        for i in range(3 * self.num_qubits):
+            # Determine qubit of the gate, depending on row or column counting
+            if rows:
+                iqubit = int(i / 3)
+            else:
+                iqubit = i % self.num_qubits
+
+            # Determine the index of the feature (x_i)
+            ii = ioff + i
+            if self.cycling:
+                if self.cycling_type == "saw":
+                    ii = ii % self.num_features
+                elif self.cycling_type == "hat":  # todo better name
+                    itest = ii % max(self.num_features + self.num_features - 2, 1)
+                    if itest >= self.num_features:
+                        ii = self.num_features + self.num_features - 2 - itest
+                    else:
+                        ii = itest
+                else:
+                    raise ValueError("Unknown cycling type!")
+
+            # Terminate if all features in this layer have been addressed
+            if iqubit >= self.num_qubits or ii >= self.num_features:
+                break
+
+            # Create Rz and Ry gates
+            if rows:
+                if i % 3 == 0:
+                    QC.rz(feature_vec[ii], iqubit)
+                elif i % 3 == 1:
+                    QC.ry(feature_vec[ii], iqubit)
+                else:  # i % 3 == 2
+                    QC.rz(feature_vec[ii], iqubit)
+            else:
+                if int(i / self.num_qubits) == 0:
+                    QC.rz(feature_vec[ii], iqubit)
+                elif int(i / self.num_qubits) == 1:
+                    QC.ry(feature_vec[ii], iqubit)
+                else:  # int(i/self.num_qubits) == 2
+                    QC.rz(feature_vec[ii], iqubit)
+
+        return QC
+
+    def _entangle_layer_iswap(self, QC: QuantumCircuit):
+        """
+        Private function which creates the entangeling layer by iSWAP neighboring qubits
+        """
+
+        # Manually build the iSWAP operator, since it is not available in Qiskit
+        iswap_op = Operator(
+            [
+                [1, 0, 0, 0],
+                [0, 1 / np.sqrt(2), 1j / np.sqrt(2), 0],
+                [0, 1j / np.sqrt(2), 1 / np.sqrt(2), 0],
+                [0, 0, 0, 1],
+            ]
+        )
+
+        # Build the layer
+        for i in range(0, self.num_qubits - 1, 2):
+            QC.unitary(iswap_op, [i, i + 1], label="iswap")
+        for i in range(
+            1,
+            self.num_qubits - 1,
+            2,
+        ):
+            QC.unitary(iswap_op, [i, i + 1], label="iswap")
+
+        return QC
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/hz_crxcrycrz.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/hz_crxcrycrz.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-
-from ..feature_map_base import FeatureMapBase
-
-
-class HZCRxCRyCRz(FeatureMapBase):
-    """
-    HZ encoding followed by controlled Rx, Ry Rz rotations:
-
-    -[-H-Rz(x)-c-----c-----c-----------------------Rx(p)-Ry(p)-Rz(p)-]-
-    -[-H-Rz(x)-Rx(p)-Ry(p)-Rz(p)-c-----c-----c-----|-----|-----|-----]-
-    -[-H-Rz(x)-c-----c-----c-----Rx(p)-Ry(p)-Rz(p)-|-----|-----|-----]-
-    -[-H-Rz(x)-Rx(p)-Ry(p)-Rz(p)-------------------c-----c-----c-----]-
-        [] = repeated by num_layers
-
-    Args:
-        num_qubits (int): Number of qubits of the HZCRxCRyCRz feature map
-        num_features (int): Dimension of the feature vector
-        num_layers (int): Number of layers (default: 1)
-        closed (bool): If true, the last and the first qubit are entangled;
-                       not necessarily hardware efficient! (default: true)
-    """
-
-    def __init__(
-        self,
-        num_qubits: int,
-        num_features: int,
-        num_layers: int = 1,
-        closed: bool = True,
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-        self.num_layers = num_layers
-        self.closed = closed
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the HZCRxCRyCRz feature map."""
-        num_param = 3 * (self.num_qubits - 1) * self.num_layers
-        if self.closed:
-            num_param += 3 * self.num_qubits * self.num_layers
-        return num_param
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Returns the circuit of the HZCRxCRyCRz feature map
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in Qiskit's QuantumCircuit format
-        """
-        nfeature = len(features)
-        nparam = len(parameters)
-        QC = QuantumCircuit(self.num_qubits)
-        ioff = 0
-
-        for ilayer in range(self.num_layers):
-            # First ZZ-feature map
-            QC.h(range(self.num_qubits))
-            for i in range(self.num_qubits):
-                QC.rz(features[i % nfeature], i)
-
-            for i in range(0, self.num_qubits - 1, 2):
-                QC.crx(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                ioff = ioff + 1
-                QC.cry(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                ioff = ioff + 1
-                QC.crz(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                ioff = ioff + 1
-
-            if self.num_qubits > 2:
-                if self.closed:
-                    istop = self.num_qubits
-                else:
-                    istop = self.num_qubits - 1
-
-                for i in range(1, istop, 2):
-                    QC.crx(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                    ioff = ioff + 1
-                    QC.cry(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                    ioff = ioff + 1
-                    QC.crz(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
-                    ioff = ioff + 1
-
-        return QC
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+
+from ..feature_map_base import FeatureMapBase
+
+
+class HZCRxCRyCRz(FeatureMapBase):
+    """
+    HZ encoding followed by controlled Rx, Ry Rz rotations:
+
+    -[-H-Rz(x)-c-----c-----c-----------------------Rx(p)-Ry(p)-Rz(p)-]-
+    -[-H-Rz(x)-Rx(p)-Ry(p)-Rz(p)-c-----c-----c-----|-----|-----|-----]-
+    -[-H-Rz(x)-c-----c-----c-----Rx(p)-Ry(p)-Rz(p)-|-----|-----|-----]-
+    -[-H-Rz(x)-Rx(p)-Ry(p)-Rz(p)-------------------c-----c-----c-----]-
+        [] = repeated by num_layers
+
+    Args:
+        num_qubits (int): Number of qubits of the HZCRxCRyCRz feature map
+        num_features (int): Dimension of the feature vector
+        num_layers (int): Number of layers (default: 1)
+        closed (bool): If true, the last and the first qubit are entangled;
+                       not necessarily hardware efficient! (default: true)
+    """
+
+    def __init__(
+        self,
+        num_qubits: int,
+        num_features: int,
+        num_layers: int = 1,
+        closed: bool = True,
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+        self.num_layers = num_layers
+        self.closed = closed
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the HZCRxCRyCRz feature map."""
+        num_param = 3 * (self.num_qubits - 1) * self.num_layers
+        if self.closed:
+            num_param += 3 * self.num_qubits * self.num_layers
+        return num_param
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Returns the circuit of the HZCRxCRyCRz feature map
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in Qiskit's QuantumCircuit format
+        """
+        nfeature = len(features)
+        nparam = len(parameters)
+        QC = QuantumCircuit(self.num_qubits)
+        ioff = 0
+
+        for ilayer in range(self.num_layers):
+            # First ZZ-feature map
+            QC.h(range(self.num_qubits))
+            for i in range(self.num_qubits):
+                QC.rz(features[i % nfeature], i)
+
+            for i in range(0, self.num_qubits - 1, 2):
+                QC.crx(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                ioff = ioff + 1
+                QC.cry(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                ioff = ioff + 1
+                QC.crz(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                ioff = ioff + 1
+
+            if self.num_qubits > 2:
+                if self.closed:
+                    istop = self.num_qubits
+                else:
+                    istop = self.num_qubits - 1
+
+                for i in range(1, istop, 2):
+                    QC.crx(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                    ioff = ioff + 1
+                    QC.cry(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                    ioff = ioff + 1
+                    QC.crz(parameters[ioff % nparam], i, (i + 1) % self.num_qubits)
+                    ioff = ioff + 1
+
+        return QC
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/qek_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/qek_feature_map.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import numpy as np
-from typing import Union
-from qiskit import QuantumCircuit
-from qiskit.circuit import ParameterVector
-
-from ..feature_map_base import FeatureMapBase
-
-
-class QEKFeatureMap(FeatureMapBase):
-
-    """
-    Creates the QEK feature map as presented in Reference http://arxiv.org/pdf/2105.02276v1
-
-    The structure of the whole QEK feature map reads:
-    0-H-Layer1-Layer2-Rz(x) ...
-
-    A single layer is constructed as:
-
-    -Rz(x0)-Ry(theta[i+0])-------x-------------------------------------CRz(theta[i+5])-
-    -Rz(x1)-Ry(theta[i+1])-CRz(theta[i+3])--------------x--------------------|---------
-    -Rz(x0)-Ry(theta[i+2])------------------------CRz(theta[i+4])------------x---------
-
-    The layers are finalized by a last layer of encoding the data, since otherwise the last parameterized gates are redundant
-
-    Args:
-        num_qubits (int): Number of Qubits of the feature map
-        num_features (int): Dimension of the feature vector
-        num_layers (int): Number of layers (default:1)
-
-    """
-
-    def __init__(self, num_qubits: int, num_features: int, num_layers: int = 1) -> None:
-        super().__init__(num_qubits, num_features)
-
-        self.num_layers = num_layers
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the feature map."""
-        return 2 * self.num_qubits * self.num_layers
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Generates and returns the circuit of the QEK feature map
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the QEK circuit in qiskit QuantumCircuit format
-        """
-
-        if self._num_features != len(features):
-            raise ValueError("Wrong number of features in supplied vector")
-
-        if self.num_parameters != len(parameters):
-            raise ValueError("Wrong number of parameters in supplied vector")
-
-        QC = QuantumCircuit(self.num_qubits)
-        ioff = 0
-
-        QC.h(range(self.num_qubits))
-
-        # Loops through the layers
-        for ilayer in range(self.num_layers):
-            # Loops through the data encoding gates
-            n_feature_loop = int(np.ceil(self.num_features / self.num_qubits))
-            for i in range(n_feature_loop * self.num_qubits):
-                if (i // self.num_qubits) % 2 == 0:
-                    QC.rz(features[i % self.num_features], i % self.num_qubits)
-                else:
-                    QC.rx(features[i % self.num_features], i % self.num_qubits)
-
-            # Single theta Ry gates
-            for i in range(self.num_qubits):
-                QC.ry(parameters[ioff], i)
-                ioff = ioff + 1
-
-            # Entangled theta CRZ gates
-            for i in range(self.num_qubits):
-                QC.crz(parameters[ioff], i, (i + 1) % self.num_qubits)
-                ioff = ioff + 1
-
-        # Repeat encoding finally to make the previous rotations not redundant
-        n_feature_loop = int(np.ceil(self.num_features / self.num_qubits))
-        for i in range(n_feature_loop * self.num_qubits):
-            if int(np.ceil(i / self.num_qubits)) % 2 == 0:
-                QC.rz(features[i % self.num_features], i % self.num_qubits)
-            else:
-                QC.rx(features[i % self.num_features], i % self.num_qubits)
-
-        return QC
+import numpy as np
+from typing import Union
+from qiskit import QuantumCircuit
+from qiskit.circuit import ParameterVector
+
+from ..feature_map_base import FeatureMapBase
+
+
+class QEKFeatureMap(FeatureMapBase):
+
+    """
+    Creates the QEK feature map as presented in Reference http://arxiv.org/pdf/2105.02276v1
+
+    The structure of the whole QEK feature map reads:
+    0-H-Layer1-Layer2-Rz(x) ...
+
+    A single layer is constructed as:
+
+    -Rz(x0)-Ry(theta[i+0])-------x-------------------------------------CRz(theta[i+5])-
+    -Rz(x1)-Ry(theta[i+1])-CRz(theta[i+3])--------------x--------------------|---------
+    -Rz(x0)-Ry(theta[i+2])------------------------CRz(theta[i+4])------------x---------
+
+    The layers are finalized by a last layer of encoding the data, since otherwise the last parameterized gates are redundant
+
+    Args:
+        num_qubits (int): Number of Qubits of the feature map
+        num_features (int): Dimension of the feature vector
+        num_layers (int): Number of layers (default:1)
+
+    """
+
+    def __init__(self, num_qubits: int, num_features: int, num_layers: int = 1) -> None:
+        super().__init__(num_qubits, num_features)
+
+        self.num_layers = num_layers
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the feature map."""
+        return 2 * self.num_qubits * self.num_layers
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Generates and returns the circuit of the QEK feature map
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the QEK circuit in qiskit QuantumCircuit format
+        """
+
+        if self._num_features != len(features):
+            raise ValueError("Wrong number of features in supplied vector")
+
+        if self.num_parameters != len(parameters):
+            raise ValueError("Wrong number of parameters in supplied vector")
+
+        QC = QuantumCircuit(self.num_qubits)
+        ioff = 0
+
+        QC.h(range(self.num_qubits))
+
+        # Loops through the layers
+        for ilayer in range(self.num_layers):
+            # Loops through the data encoding gates
+            n_feature_loop = int(np.ceil(self.num_features / self.num_qubits))
+            for i in range(n_feature_loop * self.num_qubits):
+                if (i // self.num_qubits) % 2 == 0:
+                    QC.rz(features[i % self.num_features], i % self.num_qubits)
+                else:
+                    QC.rx(features[i % self.num_features], i % self.num_qubits)
+
+            # Single theta Ry gates
+            for i in range(self.num_qubits):
+                QC.ry(parameters[ioff], i)
+                ioff = ioff + 1
+
+            # Entangled theta CRZ gates
+            for i in range(self.num_qubits):
+                QC.crz(parameters[ioff], i, (i + 1) % self.num_qubits)
+                ioff = ioff + 1
+
+        # Repeat encoding finally to make the previous rotations not redundant
+        n_feature_loop = int(np.ceil(self.num_features / self.num_qubits))
+        for i in range(n_feature_loop * self.num_qubits):
+            if int(np.ceil(i / self.num_qubits)) % 2 == 0:
+                QC.rz(features[i % self.num_features], i % self.num_qubits)
+            else:
+                QC.rx(features[i % self.num_features], i % self.num_qubits)
+
+        return QC
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/qiskit_z_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/qiskit_z_feature_map.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import numpy as np
-from typing import Union, Optional, Callable
-from qiskit import QuantumCircuit
-from qiskit.circuit import ParameterVector
-from qiskit.circuit.library import ZFeatureMap
-
-from ..feature_map_base import FeatureMapBase
-
-
-class QiskitZFeatureMap(FeatureMapBase):
-    """
-    Wrapper to use Qiskit's feature maps within IPA's
-    quantum kernel module.
-
-    Args:
-        num_qubits: The number of qubits
-        num_features: The number of features
-        reps: The number of repeated circuits. Defaults to 2, has a minimum value of 1
-        data_map_func: A mapping function for data x which can be supplied to override the default mapping from self_product()
-        parameter_prefix: The prefix used if default parameters are generated
-        insert_barriers: If True, barriers are inserted in between the evolution instructions and hadamard layers
-    """
-
-    def __init__(
-        self,
-        num_qubits: int,
-        num_features: int,
-        reps: int = 2,
-        data_map_func: Optional[Callable[[np.ndarray], float]] = None,
-        parameter_prefix: str = "x",
-        insert_barriers: bool = False,
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-
-        self._reps = reps
-        self._data_map_func = data_map_func
-        self._parameter_prefix = parameter_prefix
-        self._insert_barriers = insert_barriers
-
-    @property
-    def num_parameters(self) -> int:
-        return 0
-
-    @property
-    def num_layers(self) -> int:
-        return self._reps
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        if self._num_features != len(features):
-            raise ValueError("Wrong number of features in supplied vector")
-
-        # if self.num_parameters != len(parameters):
-        #    raise ValueError("Wrong number of parameters in supplied vector")
-
-        circuit_z_feature_map = ZFeatureMap(
-            feature_dimension=self._num_features,
-            reps=self._reps,
-            data_map_func=self._data_map_func,
-            parameter_prefix=self._parameter_prefix,
-            insert_barriers=self._insert_barriers,
-        )
-
-        return circuit_z_feature_map
+import numpy as np
+from typing import Union, Optional, Callable
+from qiskit import QuantumCircuit
+from qiskit.circuit import ParameterVector
+from qiskit.circuit.library import ZFeatureMap
+
+from ..feature_map_base import FeatureMapBase
+
+
+class QiskitZFeatureMap(FeatureMapBase):
+    """
+    Wrapper to use Qiskit's feature maps within IPA's
+    quantum kernel module.
+
+    Args:
+        num_qubits: The number of qubits
+        num_features: The number of features
+        reps: The number of repeated circuits. Defaults to 2, has a minimum value of 1
+        data_map_func: A mapping function for data x which can be supplied to override the default mapping from self_product()
+        parameter_prefix: The prefix used if default parameters are generated
+        insert_barriers: If True, barriers are inserted in between the evolution instructions and hadamard layers
+    """
+
+    def __init__(
+        self,
+        num_qubits: int,
+        num_features: int,
+        reps: int = 2,
+        data_map_func: Optional[Callable[[np.ndarray], float]] = None,
+        parameter_prefix: str = "x",
+        insert_barriers: bool = False,
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+
+        self._reps = reps
+        self._data_map_func = data_map_func
+        self._parameter_prefix = parameter_prefix
+        self._insert_barriers = insert_barriers
+
+    @property
+    def num_parameters(self) -> int:
+        return 0
+
+    @property
+    def num_layers(self) -> int:
+        return self._reps
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        if self._num_features != len(features):
+            raise ValueError("Wrong number of features in supplied vector")
+
+        # if self.num_parameters != len(parameters):
+        #    raise ValueError("Wrong number of parameters in supplied vector")
+
+        circuit_z_feature_map = ZFeatureMap(
+            feature_dimension=self._num_features,
+            reps=self._reps,
+            data_map_func=self._data_map_func,
+            parameter_prefix=self._parameter_prefix,
+            insert_barriers=self._insert_barriers,
+        )
+
+        return circuit_z_feature_map
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/yz_cx_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/yz_cx_feature_map.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import numpy as np
-from typing import Union
-from qiskit import QuantumCircuit
-from qiskit.circuit import ParameterVector
-
-from ..feature_map_base import FeatureMapBase
-
-
-class YZ_CX_FeatureMap(FeatureMapBase):
-    """
-    Creates the YZ-CX PQC feature map from Reference https://arxiv.org/pdf/2108.01039v1.pdf
-
-    The structure of the feature map is
-
-    -Ry(c*x0+theta_y0,0)-Rz(c*x0+theta_z0,0)-.-Ry(c*x0+theta_y0,1)-Rz(c*x0+theta_z0,1)--
-    -Ry(c*x1+theta_y1,0)-Rz(c*x1+theta_z1,0)-x-Ry(c*x1+theta_y1,1)-Rz(c*x1+theta_z1,1)-.
-    -Ry(c*x2+theta_y2,0)-Rz(c*x2+theta_z2,0)-.-Ry(c*x2+theta_y2,1)-Rz(c*x2+theta_z2,1)-x
-    -Ry(c*x3+theta_y3,0)-Rz(c*x3+theta_z3,0)-X-Ry(c*x3+theta_y3,1)-Rz(c*x3+theta_z3,1)--
-
-    The number of qubits and the number of features have to be the same!
-
-    One combination of Ry and Rz is considered as a single layer
-    """
-
-    def __init__(
-        self, num_qubits: int, num_features: int, num_layers: int = 1, c: float = 1.0
-    ) -> None:
-        super().__init__(num_qubits, num_features)
-
-        self._num_layers = num_layers
-        self._c = c
-
-        if self._num_features != self._num_qubits:
-            raise ValueError(
-                "The number of qubits and the number of features have to be the same!"
-            )
-
-    @property
-    def num_parameters(self) -> int:
-        return 2 * self._num_qubits * self._num_layers
-
-    @property
-    def num_layers(self) -> int:
-        return self._num_layers
-
-    @property
-    def c(self) -> int:
-        return self._c
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Return the circuit of the YZ-CX feature map
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in qiskit format
-        """
-
-        if self._num_features != len(features):
-            raise ValueError("Wrong number of features in supplied vector")
-
-        if self.num_parameters != len(parameters):
-            raise ValueError("Wrong number of parameters in supplied vector")
-
-        # Creates the layers of the feature map
-        QC = QuantumCircuit(self._num_qubits)
-        ioff = 0
-        for ilayer in range(self._num_layers):
-            for i in range(self._num_qubits):
-                QC.ry(parameters[ioff] + self._c * features[i], i)
-                ioff = ioff + 1
-                QC.rz(parameters[ioff] + self._c * features[i], i)
-                ioff = ioff + 1
-            # Entangling layer depends on odd or even layer
-            if ilayer % 2 == 0:
-                for i in range(0, self._num_qubits - 1, 2):
-                    QC.cx(i, i + 1)
-            else:
-                for i in range(1, self._num_qubits - 1, 2):
-                    QC.cx(i, i + 1)
-        return QC
+import numpy as np
+from typing import Union
+from qiskit import QuantumCircuit
+from qiskit.circuit import ParameterVector
+
+from ..feature_map_base import FeatureMapBase
+
+
+class YZ_CX_FeatureMap(FeatureMapBase):
+    """
+    Creates the YZ-CX PQC feature map from Reference https://arxiv.org/pdf/2108.01039v1.pdf
+
+    The structure of the feature map is
+
+    -Ry(c*x0+theta_y0,0)-Rz(c*x0+theta_z0,0)-.-Ry(c*x0+theta_y0,1)-Rz(c*x0+theta_z0,1)--
+    -Ry(c*x1+theta_y1,0)-Rz(c*x1+theta_z1,0)-x-Ry(c*x1+theta_y1,1)-Rz(c*x1+theta_z1,1)-.
+    -Ry(c*x2+theta_y2,0)-Rz(c*x2+theta_z2,0)-.-Ry(c*x2+theta_y2,1)-Rz(c*x2+theta_z2,1)-x
+    -Ry(c*x3+theta_y3,0)-Rz(c*x3+theta_z3,0)-X-Ry(c*x3+theta_y3,1)-Rz(c*x3+theta_z3,1)--
+
+    The number of qubits and the number of features have to be the same!
+
+    One combination of Ry and Rz is considered as a single layer
+    """
+
+    def __init__(
+        self, num_qubits: int, num_features: int, num_layers: int = 1, c: float = 1.0
+    ) -> None:
+        super().__init__(num_qubits, num_features)
+
+        self._num_layers = num_layers
+        self._c = c
+
+        if self._num_features != self._num_qubits:
+            raise ValueError(
+                "The number of qubits and the number of features have to be the same!"
+            )
+
+    @property
+    def num_parameters(self) -> int:
+        return 2 * self._num_qubits * self._num_layers
+
+    @property
+    def num_layers(self) -> int:
+        return self._num_layers
+
+    @property
+    def c(self) -> int:
+        return self._c
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Return the circuit of the YZ-CX feature map
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in qiskit format
+        """
+
+        if self._num_features != len(features):
+            raise ValueError("Wrong number of features in supplied vector")
+
+        if self.num_parameters != len(parameters):
+            raise ValueError("Wrong number of parameters in supplied vector")
+
+        # Creates the layers of the feature map
+        QC = QuantumCircuit(self._num_qubits)
+        ioff = 0
+        for ilayer in range(self._num_layers):
+            for i in range(self._num_qubits):
+                QC.ry(parameters[ioff] + self._c * features[i], i)
+                ioff = ioff + 1
+                QC.rz(parameters[ioff] + self._c * features[i], i)
+                ioff = ioff + 1
+            # Entangling layer depends on odd or even layer
+            if ilayer % 2 == 0:
+                for i in range(0, self._num_qubits - 1, 2):
+                    QC.cx(i, i + 1)
+            else:
+                for i in range(1, self._num_qubits - 1, 2):
+                    QC.cx(i, i + 1)
+        return QC
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/feature_map_implemented/zfeaturemap_cx.py` & `squlearn-0.2.0/src/squlearn/feature_map/feature_map_implemented/zfeaturemap_cx.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-import numpy as np
-from typing import Union
-
-from qiskit import QuantumCircuit
-from qiskit.circuit import ParameterVector
-from ..feature_map_base import FeatureMapBase
-
-
-class ZFeatureMap_CX(FeatureMapBase):
-    """
-    Creates Qiskit's ZFeatureMap with additional CNOT gates between the default layers.
-
-    The number of qubits and the number of features have to be the same!
-    """
-
-    def __init__(self, num_qubits: int, num_features: int, reps: int = 2) -> None:
-        super().__init__(num_qubits, num_features)
-        self._reps = reps
-
-        if self._num_features != self._num_qubits:
-            raise ValueError(
-                "The number of qubits and the number of features have to be the same!"
-            )
-
-    @property
-    def num_parameters(self) -> int:
-        return self._num_qubits * self._reps
-
-    @property
-    def num_layers(self) -> int:
-        return self._reps
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        if self._num_features != len(features):
-            raise ValueError("Wrong number of features!")
-
-        circuit = QuantumCircuit(self._num_qubits)
-        ioff = 0
-        for _ in range(self._reps):
-            for i in range(self._num_qubits):
-                circuit.h(i)
-                circuit.p(parameters[ioff] * features[i], i)
-                ioff += 1
-            if self._reps % 2 == 0:
-                for j in range(self._num_qubits - 1):
-                    circuit.cx(j, j + 1)
-            else:
-                for j in range(1, self._num_qubits - 1, 2):
-                    circuit.cx(j, j + 1)
-
-        return circuit
+import numpy as np
+from typing import Union
+
+from qiskit import QuantumCircuit
+from qiskit.circuit import ParameterVector
+from ..feature_map_base import FeatureMapBase
+
+
+class ZFeatureMap_CX(FeatureMapBase):
+    """
+    Creates Qiskit's ZFeatureMap with additional CNOT gates between the default layers.
+
+    The number of qubits and the number of features have to be the same!
+    """
+
+    def __init__(self, num_qubits: int, num_features: int, reps: int = 2) -> None:
+        super().__init__(num_qubits, num_features)
+        self._reps = reps
+
+        if self._num_features != self._num_qubits:
+            raise ValueError(
+                "The number of qubits and the number of features have to be the same!"
+            )
+
+    @property
+    def num_parameters(self) -> int:
+        return self._num_qubits * self._reps
+
+    @property
+    def num_layers(self) -> int:
+        return self._reps
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        if self._num_features != len(features):
+            raise ValueError("Wrong number of features!")
+
+        circuit = QuantumCircuit(self._num_qubits)
+        ioff = 0
+        for _ in range(self._reps):
+            for i in range(self._num_qubits):
+                circuit.h(i)
+                circuit.p(parameters[ioff] * features[i], i)
+                ioff += 1
+            if self._reps % 2 == 0:
+                for j in range(self._num_qubits - 1):
+                    circuit.cx(j, j + 1)
+            else:
+                for j in range(1, self._num_qubits - 1, 2):
+                    circuit.cx(j, j + 1)
+
+        return circuit
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/pruned_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/pruned_feature_map.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,244 +1,244 @@
-import numpy as np
-from qiskit.circuit import ParameterVector
-from qiskit.circuit.parametervector import ParameterVectorElement
-from qiskit.circuit.parameterexpression import ParameterExpression
-from qiskit.utils import QuantumInstance
-import warnings
-from typing import Union
-from qiskit import QuantumCircuit
-
-from .feature_map_base import FeatureMapBase
-
-from ..util.data_preprocessing import adjust_input
-from ..util.quantum_fisher import get_quantum_fisher
-
-
-class PrunedFeatureMap(FeatureMapBase):
-
-    """
-    Class for generating a new feature map from an existing one without the pruned parameters.
-    Relabels the parameters.
-    """
-
-    def __init__(self, feature_map: FeatureMapBase, pruned_parameters):
-        """
-        Constructor of the pruned pqc
-
-        Args:
-            feature_map : pqc from which the parameters are removed
-            pruned_parameters: list with indices of the redundant parameters
-        """
-
-        self.feature_map = feature_map
-        self.pruned_parameters = pruned_parameters
-
-        # Read in the original pqc
-        self.x_base = ParameterVector("x_base", self.feature_map.num_features)
-        self.p_base = ParameterVector("p_base", self.feature_map.num_parameters)
-        self.base_pqc = self.feature_map.get_circuit(self.x_base, self.p_base)
-
-        # create pruned circuit
-        del_list = []
-        for i in range(len(self.p_base)):
-            if i in self.pruned_parameters:
-                del_list.append(self.p_base[i])
-
-        # Create circuit from the base circuit, but empty
-        self.pruned_pqc = self.base_pqc.copy()
-        self.pruned_pqc.clear()
-
-        # Loop through all gates in the circuits and copy the ones which are kept
-        for i in range(len(self.base_pqc._data)):
-            if len(self.base_pqc._data[i].operation.params) == 1:
-                # Compare pruning list with parameters in gate
-                if isinstance(
-                    self.base_pqc._data[i].operation.params[0], ParameterExpression
-                ) or isinstance(
-                    self.base_pqc._data[i].operation.params[0], ParameterVectorElement
-                ):
-                    if (
-                        len(
-                            set(del_list).intersection(
-                                self.base_pqc._data[i].operation.params[0].parameters
-                            )
-                        )
-                        <= 0
-                    ):
-                        self.pruned_pqc.append(self.base_pqc._data[i])
-                else:
-                    self.pruned_pqc.append(self.base_pqc._data[i])
-            else:
-                self.pruned_pqc.append(self.base_pqc._data[i])
-
-        # Parameter indexing is not the same, since ordering can change -> renumber variables
-        # Get all used parameters in the pruned circuit
-        used_param = self.pruned_pqc._parameter_table.get_keys()
-
-        # Renumber parameters
-        used_old_param = [p for p in self.p_base if p in used_param]
-        self.p = ParameterVector("p_", len(used_old_param))
-        exchange_dict_p = dict(zip(used_old_param, self.p))
-
-        # Renumber x vector
-        used_old_x = [x for x in self.x_base if x in used_param]
-        self.x = ParameterVector("x_", len(used_old_x))
-        exchange_dict_x = dict(zip(used_old_x, self.x))
-
-        # Replace variables by the relabeled ones
-        exchange_both = exchange_dict_x
-        exchange_both.update(exchange_dict_p)
-        self.pruned_pqc.assign_parameters(exchange_both, inplace=True)
-        self._num_qubits = self.feature_map.num_qubits
-        self._num_features = len(self.x)
-        if self._num_features != self.feature_map._num_features:
-            warnings.warn("Number of features changed in the pruning process!", RuntimeWarning)
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns number of parameters in the pruned pqc"""
-        return len(self.p)
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """Returns the circuit of the pruned pqc"""
-        exchange_dict_x = dict(zip(self.x, features))
-        exchange_dict_p = dict(zip(self.p, parameters))
-        exchange_both = exchange_dict_x
-        exchange_both.update(exchange_dict_p)
-        return self.pruned_pqc.assign_parameters(exchange_both)
-
-
-def automated_pruning(
-    feature_map: FeatureMapBase,
-    QI: QuantumInstance,
-    n_sample=1,
-    pruning_thresh=1e-10,
-    x_lim=None,
-    p_lim=None,
-    x_val=None,
-    p_val=None,
-    verbose=1,
-    seed=0,
-) -> FeatureMapBase:
-    """
-    Function for automated pruning of the parameters in the inputted parameterized quantum circuit.
-
-    Args:
-        feature_map : Parameterized quantum circuit that will be pruned. Has to be in the feature_map format of quantum_fit!
-        QI : Quantum Instance for evaluating the Quantum Fisher Information Matrix
-        n_sample=1 (optional) : Number of random parameter values and input data that is generated.
-                               (if x_val=None and p_val=None, the number of evaluated Fisher matrices is n_sample^2)
-        pruning_thresh=1e-10 (optional) : threshold for pruning, eigenvalues lower that value are considered to be redundant.
-        x_lim=None (optional) : Limits for the random input data values; default limits are (-pi,pi).
-        p_lim=None (optional) : Limits for the random parameter values; default limits are (-pi,pi).
-        x_val=None (optional) : Array with input data values. If specified, no random input data is generated.
-        p_val=None (optional) : Array with parameter values. If specified, no random parameter values are generated.
-        verbose=1 (optional) : Verbosity of the algorithm, as default only the redundant parameters are printed.
-        seed=0 (optional) : Seed for the random input data and parameters generation.
-
-    Returns:
-        Pruned feature_map in the feature_map format
-    """
-
-    # Set-up default limits
-    if x_lim is None:
-        x_lim = (-np.pi, np.pi)
-    if p_lim is None:
-        p_lim = (-np.pi, np.pi)
-
-    # Set-up numpy seed (backup old one)
-    seed_backup = np.random.get_state()
-    np.random.seed(seed)
-
-    # Process x-values
-    if x_val is not None:
-        x_val, multi = adjust_input(x_val, feature_map.num_features)
-        if not isinstance(x_val, np.ndarray):
-            x = np.array(x_val)
-        else:
-            x = x_val
-        if x.shape[1] != feature_map.num_features:
-            raise ValueError("Wrong size of the input x_val")
-    else:
-        x = np.random.uniform(
-            low=x_lim[0], high=x_lim[1], size=(n_sample, feature_map.num_features)
-        )
-
-    # Process p-values
-    if p_val is not None:
-        p_val, multi = adjust_input(p_val, feature_map.num_parameters)
-        if not isinstance(p_val, np.ndarray):
-            p = np.array(p_val)
-        else:
-            p = p_val
-        if p.shape[1] != feature_map.num_parameters:
-            raise ValueError("Wrong size of the input p_val")
-    else:
-        p = np.random.uniform(
-            low=p_lim[0], high=p_lim[1], size=(n_sample, feature_map.num_parameters)
-        )
-
-    # Reset numpy random state
-    np.random.set_state(seed_backup)
-
-    # Calculate QIF for all x and parameter combinations and average over all fishers
-    fishers = np.zeros([feature_map.num_parameters, feature_map.num_parameters])
-    count = 0
-    for x_ in x:
-        for p_ in p:
-            if verbose >= 2:
-                print("Calc fisher number ", count + 1)
-            fishers += get_quantum_fisher(feature_map, x_, p_, QI)
-            count += 1
-    if count > 0:
-        fishers = fishers / count
-
-    # Build pruning list
-    pruning_list = pruning_from_QFI(fishers, pruning_thresh)
-    if verbose >= 1:
-        print("Pruned parameters:", np.sort(pruning_list))
-
-    # Return pruned feature_map
-    return PrunedFeatureMap(feature_map, pruning_list)
-
-
-def pruning_from_QFI(QFI, pruning_thresh=1e-10):
-    """
-    Algorithm for determining the redundant parameters from the QFI.
-    (see doi:10.1103/PRXQuantum.2.040309)
-
-    Args:
-        QFI: Quantum Fisher Information Matrix as numpy matrix.
-        pruning_thresh=1e-10 (optional) : threshold for pruning, eigenvalues lower that value are considered to be redundant.
-    Returns:
-        List of redundant parameters (as indices)
-    """
-
-    # Symmetrization
-    QFI_val = 0.5 * (QFI + QFI.transpose())
-    # Eigenvalue decomposition
-    W, V = np.linalg.eigh(QFI_val)
-    pruning_list = []
-    index_list = np.arange(0, len(W))
-    # Pruning algorithm from doi:10.1103/PRXQuantum.2.040309
-    while abs(W[0]) <= pruning_thresh:
-        vec = np.zeros(len(W))
-        icount = 0
-        while abs(W[icount]) <= pruning_thresh:
-            vec = vec + np.square(V[:, icount])
-            icount = icount + 1
-            if icount >= len(W):
-                break
-
-        i = np.argmax(vec)
-        pruning_list.append(index_list[i])
-        index_list = np.delete(index_list, i, 0)
-        QFI_val = np.delete(QFI_val, i, 0)
-        QFI_val = np.delete(QFI_val, i, 1)
-        if QFI_val.ndim <= 0:
-            break
-        W, V = np.linalg.eigh(QFI_val)
-    return pruning_list
+import numpy as np
+from qiskit.circuit import ParameterVector
+from qiskit.circuit.parametervector import ParameterVectorElement
+from qiskit.circuit.parameterexpression import ParameterExpression
+from qiskit.utils import QuantumInstance
+import warnings
+from typing import Union
+from qiskit import QuantumCircuit
+
+from .feature_map_base import FeatureMapBase
+
+from ..util.data_preprocessing import adjust_input
+from ..util.quantum_fisher import get_quantum_fisher
+
+
+class PrunedFeatureMap(FeatureMapBase):
+
+    """
+    Class for generating a new feature map from an existing one without the pruned parameters.
+    Relabels the parameters.
+    """
+
+    def __init__(self, feature_map: FeatureMapBase, pruned_parameters):
+        """
+        Constructor of the pruned pqc
+
+        Args:
+            feature_map : pqc from which the parameters are removed
+            pruned_parameters: list with indices of the redundant parameters
+        """
+
+        self.feature_map = feature_map
+        self.pruned_parameters = pruned_parameters
+
+        # Read in the original pqc
+        self.x_base = ParameterVector("x_base", self.feature_map.num_features)
+        self.p_base = ParameterVector("p_base", self.feature_map.num_parameters)
+        self.base_pqc = self.feature_map.get_circuit(self.x_base, self.p_base)
+
+        # create pruned circuit
+        del_list = []
+        for i in range(len(self.p_base)):
+            if i in self.pruned_parameters:
+                del_list.append(self.p_base[i])
+
+        # Create circuit from the base circuit, but empty
+        self.pruned_pqc = self.base_pqc.copy()
+        self.pruned_pqc.clear()
+
+        # Loop through all gates in the circuits and copy the ones which are kept
+        for i in range(len(self.base_pqc._data)):
+            if len(self.base_pqc._data[i].operation.params) == 1:
+                # Compare pruning list with parameters in gate
+                if isinstance(
+                    self.base_pqc._data[i].operation.params[0], ParameterExpression
+                ) or isinstance(
+                    self.base_pqc._data[i].operation.params[0], ParameterVectorElement
+                ):
+                    if (
+                        len(
+                            set(del_list).intersection(
+                                self.base_pqc._data[i].operation.params[0].parameters
+                            )
+                        )
+                        <= 0
+                    ):
+                        self.pruned_pqc.append(self.base_pqc._data[i])
+                else:
+                    self.pruned_pqc.append(self.base_pqc._data[i])
+            else:
+                self.pruned_pqc.append(self.base_pqc._data[i])
+
+        # Parameter indexing is not the same, since ordering can change -> renumber variables
+        # Get all used parameters in the pruned circuit
+        used_param = self.pruned_pqc._parameter_table.get_keys()
+
+        # Renumber parameters
+        used_old_param = [p for p in self.p_base if p in used_param]
+        self.p = ParameterVector("p_", len(used_old_param))
+        exchange_dict_p = dict(zip(used_old_param, self.p))
+
+        # Renumber x vector
+        used_old_x = [x for x in self.x_base if x in used_param]
+        self.x = ParameterVector("x_", len(used_old_x))
+        exchange_dict_x = dict(zip(used_old_x, self.x))
+
+        # Replace variables by the relabeled ones
+        exchange_both = exchange_dict_x
+        exchange_both.update(exchange_dict_p)
+        self.pruned_pqc.assign_parameters(exchange_both, inplace=True)
+        self._num_qubits = self.feature_map.num_qubits
+        self._num_features = len(self.x)
+        if self._num_features != self.feature_map._num_features:
+            warnings.warn("Number of features changed in the pruning process!", RuntimeWarning)
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns number of parameters in the pruned pqc"""
+        return len(self.p)
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """Returns the circuit of the pruned pqc"""
+        exchange_dict_x = dict(zip(self.x, features))
+        exchange_dict_p = dict(zip(self.p, parameters))
+        exchange_both = exchange_dict_x
+        exchange_both.update(exchange_dict_p)
+        return self.pruned_pqc.assign_parameters(exchange_both)
+
+
+def automated_pruning(
+    feature_map: FeatureMapBase,
+    QI: QuantumInstance,
+    n_sample=1,
+    pruning_thresh=1e-10,
+    x_lim=None,
+    p_lim=None,
+    x_val=None,
+    p_val=None,
+    verbose=1,
+    seed=0,
+) -> FeatureMapBase:
+    """
+    Function for automated pruning of the parameters in the inputted parameterized quantum circuit.
+
+    Args:
+        feature_map : Parameterized quantum circuit that will be pruned. Has to be in the feature_map format of quantum_fit!
+        QI : Quantum Instance for evaluating the Quantum Fisher Information Matrix
+        n_sample=1 (optional) : Number of random parameter values and input data that is generated.
+                               (if x_val=None and p_val=None, the number of evaluated Fisher matrices is n_sample^2)
+        pruning_thresh=1e-10 (optional) : threshold for pruning, eigenvalues lower that value are considered to be redundant.
+        x_lim=None (optional) : Limits for the random input data values; default limits are (-pi,pi).
+        p_lim=None (optional) : Limits for the random parameter values; default limits are (-pi,pi).
+        x_val=None (optional) : Array with input data values. If specified, no random input data is generated.
+        p_val=None (optional) : Array with parameter values. If specified, no random parameter values are generated.
+        verbose=1 (optional) : Verbosity of the algorithm, as default only the redundant parameters are printed.
+        seed=0 (optional) : Seed for the random input data and parameters generation.
+
+    Returns:
+        Pruned feature_map in the feature_map format
+    """
+
+    # Set-up default limits
+    if x_lim is None:
+        x_lim = (-np.pi, np.pi)
+    if p_lim is None:
+        p_lim = (-np.pi, np.pi)
+
+    # Set-up numpy seed (backup old one)
+    seed_backup = np.random.get_state()
+    np.random.seed(seed)
+
+    # Process x-values
+    if x_val is not None:
+        x_val, multi = adjust_input(x_val, feature_map.num_features)
+        if not isinstance(x_val, np.ndarray):
+            x = np.array(x_val)
+        else:
+            x = x_val
+        if x.shape[1] != feature_map.num_features:
+            raise ValueError("Wrong size of the input x_val")
+    else:
+        x = np.random.uniform(
+            low=x_lim[0], high=x_lim[1], size=(n_sample, feature_map.num_features)
+        )
+
+    # Process p-values
+    if p_val is not None:
+        p_val, multi = adjust_input(p_val, feature_map.num_parameters)
+        if not isinstance(p_val, np.ndarray):
+            p = np.array(p_val)
+        else:
+            p = p_val
+        if p.shape[1] != feature_map.num_parameters:
+            raise ValueError("Wrong size of the input p_val")
+    else:
+        p = np.random.uniform(
+            low=p_lim[0], high=p_lim[1], size=(n_sample, feature_map.num_parameters)
+        )
+
+    # Reset numpy random state
+    np.random.set_state(seed_backup)
+
+    # Calculate QIF for all x and parameter combinations and average over all fishers
+    fishers = np.zeros([feature_map.num_parameters, feature_map.num_parameters])
+    count = 0
+    for x_ in x:
+        for p_ in p:
+            if verbose >= 2:
+                print("Calc fisher number ", count + 1)
+            fishers += get_quantum_fisher(feature_map, x_, p_, QI)
+            count += 1
+    if count > 0:
+        fishers = fishers / count
+
+    # Build pruning list
+    pruning_list = pruning_from_QFI(fishers, pruning_thresh)
+    if verbose >= 1:
+        print("Pruned parameters:", np.sort(pruning_list))
+
+    # Return pruned feature_map
+    return PrunedFeatureMap(feature_map, pruning_list)
+
+
+def pruning_from_QFI(QFI, pruning_thresh=1e-10):
+    """
+    Algorithm for determining the redundant parameters from the QFI.
+    (see doi:10.1103/PRXQuantum.2.040309)
+
+    Args:
+        QFI: Quantum Fisher Information Matrix as numpy matrix.
+        pruning_thresh=1e-10 (optional) : threshold for pruning, eigenvalues lower that value are considered to be redundant.
+    Returns:
+        List of redundant parameters (as indices)
+    """
+
+    # Symmetrization
+    QFI_val = 0.5 * (QFI + QFI.transpose())
+    # Eigenvalue decomposition
+    W, V = np.linalg.eigh(QFI_val)
+    pruning_list = []
+    index_list = np.arange(0, len(W))
+    # Pruning algorithm from doi:10.1103/PRXQuantum.2.040309
+    while abs(W[0]) <= pruning_thresh:
+        vec = np.zeros(len(W))
+        icount = 0
+        while abs(W[icount]) <= pruning_thresh:
+            vec = vec + np.square(V[:, icount])
+            icount = icount + 1
+            if icount >= len(W):
+                break
+
+        i = np.argmax(vec)
+        pruning_list.append(index_list[i])
+        index_list = np.delete(index_list, i, 0)
+        QFI_val = np.delete(QFI_val, i, 0)
+        QFI_val = np.delete(QFI_val, i, 1)
+        if QFI_val.ndim <= 0:
+            break
+        W, V = np.linalg.eigh(QFI_val)
+    return pruning_list
```

### Comparing `squlearn-0.1.0/src/squlearn/feature_map/transpiled_feature_map.py` & `squlearn-0.2.0/src/squlearn/feature_map/transpiled_feature_map.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import numpy as np
-from typing import Union
-
-from qiskit.circuit import ParameterVector
-from qiskit import QuantumCircuit
-from qiskit.compiler import transpile
-
-from .feature_map_base import FeatureMapBase
-
-
-class TranspiledFeatureMap(FeatureMapBase):
-    """
-    Feature map base class
-
-    Args:
-        num_qubits (int): Number of Qubits of the feature map
-        num_features (int): Dimension of the feature vector
-    """
-
-    def __init__(
-        self,
-        feature_map: FeatureMapBase,
-        backend,
-        transpile_func=None,
-    ) -> None:
-        self._feature_map = feature_map
-        self._backend = backend
-        self._transpile_func = transpile_func
-
-        self.x = ParameterVector("x", self._feature_map.num_features)
-        self.p = ParameterVector("p", self._feature_map.num_parameters)
-
-        self._circuit = self._feature_map.get_circuit(self.x, self.p)
-
-        if self._transpile_func is not None:
-            self._transpiled_circuit = self._transpile_func(self._circuit, self._backend)
-        else:
-            self._transpiled_circuit = transpile(
-                self._circuit, self._backend, optimization_level=3, seed_transpiler=0
-            )
-
-        self._qubit_map = _gen_qubit_mapping(self._transpiled_circuit)
-
-    @property
-    def num_qubits(self) -> int:
-        """Returns the number of qubits of the feature map."""
-        return self._feature_map.num_qubits
-
-    @property
-    def num_all_qubits(self) -> int:
-        """Returns the number of qubits of the feature map."""
-        return self._transpiled_circuit.num_qubits
-
-    @property
-    def qubit_map(self):
-        return self._qubit_map
-
-    @property
-    def backend(self) -> int:
-        """Returns the dimension of features of the feature map."""
-        return self._backend
-
-    @property
-    def num_features(self) -> int:
-        """Returns the dimension of features of the feature map."""
-        return self._feature_map.num_features
-
-    @property
-    def num_parameters(self) -> int:
-        """Returns the number of trainable parameters of the feature map."""
-        return self._feature_map.num_parameters
-
-    def get_circuit(
-        self,
-        features: Union[ParameterVector, np.ndarray],
-        parameters: Union[ParameterVector, np.ndarray],
-    ) -> QuantumCircuit:
-        """
-        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
-
-        Args:
-            features Union[ParameterVector,np.ndarray]: Input vector of the features
-                from which the gate inputs are obtained
-            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
-                from which the gate inputs are obtained
-
-        Return:
-            Returns the circuit in qiskit QuantumCircuit format
-        """
-
-        exchange_dict_x = dict(zip(self.x, features))
-        exchange_dict_p = dict(zip(self.p, parameters))
-        exchange_both = exchange_dict_x
-        exchange_both.update(exchange_dict_p)
-        return self._transpiled_circuit.assign_parameters(exchange_both)
-
-
-def _gen_qubit_mapping(circuit):
-    """
-    Returns dictionary that maps virtual qubits to the physical ones
-
-    Args:
-        circ : quantum circuit (ideally transpiled)
-
-    Returns:
-        Dictionary which maps virtual to physical qubits
-    """
-    dic = {}
-    try:
-        from qiskit.transpiler.layout import TranspileLayout
-
-        if isinstance(circuit._layout, TranspileLayout):
-            layout = circuit._layout.initial_layout
-        else:
-            layout = circuit._layout
-        bit_locations = {
-            bit: {"register": register, "index": index}
-            for register in layout.get_registers()
-            for index, bit in enumerate(register)
-        }
-        for index, qubit in enumerate(layout.get_virtual_bits()):
-            if qubit not in bit_locations:
-                bit_locations[qubit] = {"register": None, "index": index}
-        for key, val in layout.get_virtual_bits().items():
-            bit_register = bit_locations[key]["register"]
-            if bit_register is None or bit_register.name != "ancilla":
-                dic[bit_locations[key]["index"]] = val
-    except:
-        for i in range(circuit.num_qubits):
-            dic[i] = i
-    return dic
+import numpy as np
+from typing import Union
+
+from qiskit.circuit import ParameterVector
+from qiskit import QuantumCircuit
+from qiskit.compiler import transpile
+
+from .feature_map_base import FeatureMapBase
+
+
+class TranspiledFeatureMap(FeatureMapBase):
+    """
+    Feature map base class
+
+    Args:
+        num_qubits (int): Number of Qubits of the feature map
+        num_features (int): Dimension of the feature vector
+    """
+
+    def __init__(
+        self,
+        feature_map: FeatureMapBase,
+        backend,
+        transpile_func=None,
+    ) -> None:
+        self._feature_map = feature_map
+        self._backend = backend
+        self._transpile_func = transpile_func
+
+        self.x = ParameterVector("x", self._feature_map.num_features)
+        self.p = ParameterVector("p", self._feature_map.num_parameters)
+
+        self._circuit = self._feature_map.get_circuit(self.x, self.p)
+
+        if self._transpile_func is not None:
+            self._transpiled_circuit = self._transpile_func(self._circuit, self._backend)
+        else:
+            self._transpiled_circuit = transpile(
+                self._circuit, self._backend, optimization_level=3, seed_transpiler=0
+            )
+
+        self._qubit_map = _gen_qubit_mapping(self._transpiled_circuit)
+
+    @property
+    def num_qubits(self) -> int:
+        """Returns the number of qubits of the feature map."""
+        return self._feature_map.num_qubits
+
+    @property
+    def num_all_qubits(self) -> int:
+        """Returns the number of qubits of the feature map."""
+        return self._transpiled_circuit.num_qubits
+
+    @property
+    def qubit_map(self):
+        return self._qubit_map
+
+    @property
+    def backend(self) -> int:
+        """Returns the dimension of features of the feature map."""
+        return self._backend
+
+    @property
+    def num_features(self) -> int:
+        """Returns the dimension of features of the feature map."""
+        return self._feature_map.num_features
+
+    @property
+    def num_parameters(self) -> int:
+        """Returns the number of trainable parameters of the feature map."""
+        return self._feature_map.num_parameters
+
+    def get_circuit(
+        self,
+        features: Union[ParameterVector, np.ndarray],
+        parameters: Union[ParameterVector, np.ndarray],
+    ) -> QuantumCircuit:
+        """
+        Return the circuit feature map (has to be overwritten, otherwise a NotImplementedError is thrown)
+
+        Args:
+            features Union[ParameterVector,np.ndarray]: Input vector of the features
+                from which the gate inputs are obtained
+            param_vec Union[ParameterVector,np.ndarray]: Input vector of the parameters
+                from which the gate inputs are obtained
+
+        Return:
+            Returns the circuit in qiskit QuantumCircuit format
+        """
+
+        exchange_dict_x = dict(zip(self.x, features))
+        exchange_dict_p = dict(zip(self.p, parameters))
+        exchange_both = exchange_dict_x
+        exchange_both.update(exchange_dict_p)
+        return self._transpiled_circuit.assign_parameters(exchange_both)
+
+
+def _gen_qubit_mapping(circuit):
+    """
+    Returns dictionary that maps virtual qubits to the physical ones
+
+    Args:
+        circ : quantum circuit (ideally transpiled)
+
+    Returns:
+        Dictionary which maps virtual to physical qubits
+    """
+    dic = {}
+    try:
+        from qiskit.transpiler.layout import TranspileLayout
+
+        if isinstance(circuit._layout, TranspileLayout):
+            layout = circuit._layout.initial_layout
+        else:
+            layout = circuit._layout
+        bit_locations = {
+            bit: {"register": register, "index": index}
+            for register in layout.get_registers()
+            for index, bit in enumerate(register)
+        }
+        for index, qubit in enumerate(layout.get_virtual_bits()):
+            if qubit not in bit_locations:
+                bit_locations[qubit] = {"register": None, "index": index}
+        for key, val in layout.get_virtual_bits().items():
+            bit_register = bit_locations[key]["register"]
+            if bit_register is None or bit_register.name != "ancilla":
+                dic[bit_locations[key]["index"]] = val
+    except:
+        for i in range(circuit.num_qubits):
+            dic[i] = i
+    return dic
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/matrix/fidelity_kernel.py` & `squlearn-0.2.0/src/squlearn/kernel/matrix/fidelity_kernel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,127 +1,138 @@
-import numpy as np
-from typing import Union
-from .kernel_matrix_base import KernelMatrixBase
-from ...feature_map.feature_map_base import FeatureMapBase
-from ...util.executor import Executor
-
-from qiskit_machine_learning.kernels import QuantumKernel
-from qiskit_machine_learning.kernels.fidelity_quantum_kernel import (
-    FidelityQuantumKernel,
-)
-from qiskit_machine_learning.kernels import TrainableFidelityQuantumKernel
-from qiskit.utils import QuantumInstance
-from qiskit.algorithms.state_fidelities import ComputeUncompute
-from qiskit.circuit import ParameterVector
-from qiskit.primitives import BaseSampler, BaseEstimator
-
-
-class FidelityKernel(KernelMatrixBase):
-    """
-    Add documentation.
-
-    Args:
-        mit_depol_noise (Union[str, None]), default=None:
-            Option for mitigating depolarizing noise ('msplit' or 'mmean') after 
-            `http://arxiv.org/pdf/2105.02276v1´. Only meaningful for 
-            FQKs computed on a real backend.
-    """
-    def __init__(
-        self,
-        feature_map: FeatureMapBase,
-        executor: Executor,
-        initial_parameters=None,
-        evaluate_duplicates: str = "off_diagonal",
-        mit_depol_noise: Union[str, None] = None
-    ) -> None:
-        super().__init__(feature_map, executor, initial_parameters)
-
-        self._quantum_kernel = None
-        self._evaluate_duplicates = evaluate_duplicates.lower()
-        self._mit_depol_noise = mit_depol_noise
-
-        self._feature_vector = ParameterVector("x", self.num_features)
-        if self.num_parameters > 0:
-            self._parameter_vector = ParameterVector("θ", self.num_parameters)
-        else:
-            self._parameter_vector = None
-
-        self._fmap_circuit = self._feature_map.get_circuit(
-            self._feature_vector, self._parameter_vector
-        )
-
-        if self._executor.execution == "Sampler":
-            fidelity = ComputeUncompute(sampler=self._executor.get_sampler())
-            if self._parameter_vector is None:
-                    # Fidelity Quantum Kernel without any parameters
-                    self._quantum_kernel = FidelityQuantumKernel(
-                        feature_map=self._fmap_circuit,
-                        fidelity=fidelity,
-                        evaluate_duplicates=self._evaluate_duplicates,
-                    )
-            else:
-                # Fidelity Quantum Kernel with any parameters -> TrainableFidelityQuantumKernel
-                self._quantum_kernel = TrainableFidelityQuantumKernel(
-                    feature_map=self._fmap_circuit,
-                    fidelity=fidelity,
-                    training_parameters=self._parameter_vector,
-                    evaluate_duplicates=self._evaluate_duplicates,
-                )
-        else:
-            self._quantum_kernel = QuantumKernel(
-                feature_map=self._fmap_circuit,
-                quantum_instance=self._executor.backend,
-                training_parameters=self._parameter_vector,
-                evaluate_duplicates=self._evaluate_duplicates,
-            )
-
-    def evaluate(self, x: np.ndarray, y: Union[np.ndarray, None] = None) -> np.ndarray:
-        if y is None:
-            y = x
-        kernel_matrix = np.zeros((x.shape[0], y.shape[0]))
-        if self._parameter_vector is not None:
-            if self._parameters is None:
-                raise ValueError(
-                    "Parameters have to been set with assign_parameters or as initial parameters!"
-                )
-
-            self._quantum_kernel.assign_training_parameters(self._parameters)
-        
-        kernel_matrix = self._quantum_kernel.evaluate(x, y)
-        if self._mit_depol_noise is not None:
-            print("WARNING: Adavnced option. Do not use it within an squlearn.kernel.ml workflow")
-            if not np.array_equal(x, y):
-                raise ValueError("Mitigating depolarizing noise works only for square matrices computed on real backend")
-            else:
-                if self._mit_depol_noise == 'msplit':
-                    kernel_matrix = self._get_msplit_kernel(kernel_matrix)
-                elif self._mit_depol_noise == 'mmean':
-                    kernel_matrix = self._get_mmean_kernel(kernel_matrix)
-
-        return kernel_matrix
-        #return self._quantum_kernel.evaluate(x, y)
-
-    ###########
-    ## Mitigating depolarizing noise after http://arxiv.org/pdf/2105.02276v1 
-    ###########
-    def _get_msplit_kernel(self, kernel: np.ndarray) -> np.ndarray:
-        msplit_kernel_matrix = np.zeros((kernel.shape[0], kernel.shape[1]))
-        survival_prob = self._survival_probability(kernel)
-        for i in range(kernel.shape[0]):
-            for j in range(kernel.shape[1]):
-                msplit_kernel_matrix[i, j] = (kernel[i, j] - 2 ** (-1.0 * self._num_qubits) * (1 - survival_prob[i] * survival_prob[j]) ) / (survival_prob[i] * survival_prob[j])
-        return msplit_kernel_matrix
-
-    def _get_mmean_kernel(self, kernel: np.ndarray) -> np.ndarray:
-        mmean_kernel_matrix = np.zeros((kernel.shape[0], kernel.shape[1]))
-        survival_prob_mean = self._survival_probability_mean(kernel)
-        mmean_kernel_matrix = (kernel - 2 ** (-1.0 * self._num_qubits) * (1 - survival_prob_mean ** 2) ) / survival_prob_mean ** 2
-        return mmean_kernel_matrix
-    
-    def _survival_probability(self, kernel: np.ndarray) -> np.ndarray:
-        kernel_diagonal = np.diag(kernel)
-        surv_prob = np.sqrt( (kernel_diagonal - 2 ** (-1.0 * self._num_qubits)) / (1 - 2 ** (-1.0 * self._num_qubits)) )
-        return surv_prob
-    
-    def _survival_probability_mean(self, kernel: np.ndarray) -> float:
-        surv_prob = self._survival_probability(kernel)
-        return np.mean(surv_prob)
+import numpy as np
+from typing import Union
+from .kernel_matrix_base import KernelMatrixBase
+from ...feature_map.feature_map_base import FeatureMapBase
+from ...util.executor import Executor
+
+from qiskit_machine_learning.kernels import QuantumKernel
+from qiskit_machine_learning.kernels.fidelity_quantum_kernel import (
+    FidelityQuantumKernel,
+)
+from qiskit_machine_learning.kernels import TrainableFidelityQuantumKernel
+from qiskit.utils import QuantumInstance
+from qiskit.algorithms.state_fidelities import ComputeUncompute
+from qiskit.circuit import ParameterVector
+from qiskit.primitives import BaseSampler, BaseEstimator
+
+
+class FidelityKernel(KernelMatrixBase):
+    """
+    Add documentation.
+
+    Args:
+        mit_depol_noise (Union[str, None]), default=None:
+            Option for mitigating depolarizing noise ('msplit' or 'mmean') after
+            `http://arxiv.org/pdf/2105.02276v1´. Only meaningful for
+            FQKs computed on a real backend.
+    """
+
+    def __init__(
+        self,
+        feature_map: FeatureMapBase,
+        executor: Executor,
+        initial_parameters=None,
+        evaluate_duplicates: str = "off_diagonal",
+        mit_depol_noise: Union[str, None] = None,
+    ) -> None:
+        super().__init__(feature_map, executor, initial_parameters)
+
+        self._quantum_kernel = None
+        self._evaluate_duplicates = evaluate_duplicates.lower()
+        self._mit_depol_noise = mit_depol_noise
+
+        self._feature_vector = ParameterVector("x", self.num_features)
+        if self.num_parameters > 0:
+            self._parameter_vector = ParameterVector("θ", self.num_parameters)
+        else:
+            self._parameter_vector = None
+
+        self._fmap_circuit = self._feature_map.get_circuit(
+            self._feature_vector, self._parameter_vector
+        )
+
+        if self._executor.execution == "Sampler":
+            fidelity = ComputeUncompute(sampler=self._executor.get_sampler())
+            if self._parameter_vector is None:
+                # Fidelity Quantum Kernel without any parameters
+                self._quantum_kernel = FidelityQuantumKernel(
+                    feature_map=self._fmap_circuit,
+                    fidelity=fidelity,
+                    evaluate_duplicates=self._evaluate_duplicates,
+                )
+            else:
+                # Fidelity Quantum Kernel with any parameters -> TrainableFidelityQuantumKernel
+                self._quantum_kernel = TrainableFidelityQuantumKernel(
+                    feature_map=self._fmap_circuit,
+                    fidelity=fidelity,
+                    training_parameters=self._parameter_vector,
+                    evaluate_duplicates=self._evaluate_duplicates,
+                )
+        else:
+            self._quantum_kernel = QuantumKernel(
+                feature_map=self._fmap_circuit,
+                quantum_instance=self._executor.backend,
+                training_parameters=self._parameter_vector,
+                evaluate_duplicates=self._evaluate_duplicates,
+            )
+
+    def evaluate(self, x: np.ndarray, y: Union[np.ndarray, None] = None) -> np.ndarray:
+        if y is None:
+            y = x
+        kernel_matrix = np.zeros((x.shape[0], y.shape[0]))
+        if self._parameter_vector is not None:
+            if self._parameters is None:
+                raise ValueError(
+                    "Parameters have to been set with assign_parameters or as initial parameters!"
+                )
+
+            self._quantum_kernel.assign_training_parameters(self._parameters)
+
+        kernel_matrix = self._quantum_kernel.evaluate(x, y)
+        if self._mit_depol_noise is not None:
+            print("WARNING: Adavnced option. Do not use it within an squlearn.kernel.ml workflow")
+            if not np.array_equal(x, y):
+                raise ValueError(
+                    "Mitigating depolarizing noise works only for square matrices computed on real backend"
+                )
+            else:
+                if self._mit_depol_noise == "msplit":
+                    kernel_matrix = self._get_msplit_kernel(kernel_matrix)
+                elif self._mit_depol_noise == "mmean":
+                    kernel_matrix = self._get_mmean_kernel(kernel_matrix)
+
+        return kernel_matrix
+        # return self._quantum_kernel.evaluate(x, y)
+
+    ###########
+    ## Mitigating depolarizing noise after http://arxiv.org/pdf/2105.02276v1
+    ###########
+    def _get_msplit_kernel(self, kernel: np.ndarray) -> np.ndarray:
+        msplit_kernel_matrix = np.zeros((kernel.shape[0], kernel.shape[1]))
+        survival_prob = self._survival_probability(kernel)
+        for i in range(kernel.shape[0]):
+            for j in range(kernel.shape[1]):
+                msplit_kernel_matrix[i, j] = (
+                    kernel[i, j]
+                    - 2 ** (-1.0 * self._num_qubits) * (1 - survival_prob[i] * survival_prob[j])
+                ) / (survival_prob[i] * survival_prob[j])
+        return msplit_kernel_matrix
+
+    def _get_mmean_kernel(self, kernel: np.ndarray) -> np.ndarray:
+        mmean_kernel_matrix = np.zeros((kernel.shape[0], kernel.shape[1]))
+        survival_prob_mean = self._survival_probability_mean(kernel)
+        mmean_kernel_matrix = (
+            kernel - 2 ** (-1.0 * self._num_qubits) * (1 - survival_prob_mean**2)
+        ) / survival_prob_mean**2
+        return mmean_kernel_matrix
+
+    def _survival_probability(self, kernel: np.ndarray) -> np.ndarray:
+        kernel_diagonal = np.diag(kernel)
+        surv_prob = np.sqrt(
+            (kernel_diagonal - 2 ** (-1.0 * self._num_qubits))
+            / (1 - 2 ** (-1.0 * self._num_qubits))
+        )
+        return surv_prob
+
+    def _survival_probability_mean(self, kernel: np.ndarray) -> float:
+        surv_prob = self._survival_probability(kernel)
+        return np.mean(surv_prob)
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/matrix/kernel_matrix_base.py` & `squlearn-0.2.0/src/squlearn/kernel/matrix/kernel_matrix_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-import numpy as np
-
-from ...feature_map.feature_map_base import FeatureMapBase
-from ...util.executor import Executor
-
-
-class KernelMatrixBase: 
-    def __init__(
-        self,
-        feature_map: FeatureMapBase,
-        executor: Executor,
-        initial_parameters=None,
-    ) -> None:
-        self._feature_map = feature_map
-        self._num_qubits = self._feature_map.num_qubits
-        self._num_features = self._feature_map.num_features
-        self._num_parameters = self._feature_map.num_parameters
-        self._executor = executor
-        self._parameters = initial_parameters
-
-    @property
-    def feature_map(self) -> FeatureMapBase:
-        """
-        Returns the feature map from which the kernel matrix is constructed
-        """
-        return self._feature_map
-
-    @property
-    def num_qubits(self) -> int:
-        return self._num_qubits
-
-    @property
-    def num_features(self) -> int:
-        return self._num_features
-
-    @property
-    def num_parameters(self) -> int:
-        return self._num_parameters
-
-    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
-        raise NotImplementedError()
-
-    def evaluate_pairwise(self, x: np.ndarray, y: np.ndarray = None) -> float:
-        if y is not None:
-            return self.evaluate([x], [y])[0, 0]
-        else:
-            return self.evaluate([x], None)[0, 0]
-
-    def assign_parameters(self, parameters):
-        self._parameters = parameters
-
-    def evaluate_with_parameters(
-        self, x: np.ndarray, y: np.ndarray, parameters: np.ndarray
-    ) -> np.ndarray:
-        self.assign_parameters(parameters)
-        return self.evaluate(x, y)
-
-    def __add__(self, x):
-        return _ComposedKernelMatrix(self, x, "+")
-
-    def __mul__(self, x):
-        return _ComposedKernelMatrix(self, x, "*")
-
-    def __sub__(self, x):
-        return _ComposedKernelMatrix(self, x, "-")
-
-    def __div__(self, x):
-        return _ComposedKernelMatrix(self, x, "/")
-
-    def get_params(self, deep=True):
-        return {
-            'feature_map': self._feature_map,
-            'executor': self._executor,
-            'initial_parameters': self._parameters
-        }
-
-    def set_params(self, **params):
-        for param, value in params.items():
-            setattr(self, '_' + param, value)
-        return self
-
-
-class _ComposedKernelMatrix(KernelMatrixBase):
-    def __init__(self, km1: KernelMatrixBase, km2: KernelMatrixBase, composition: str = "*"):
-        if km1.num_features != km2.num_features:
-            raise ValueError("Feature dimension is not equal in both feature maps.")
-
-        self._km1 = km1
-        self._km2 = km2
-        self._composition = composition
-
-    @property
-    def feature_map(self) -> FeatureMapBase:
-        """
-        Returns the feature map from which the kernel matrix is constructed
-        """
-        raise RuntimeError("The feature map is not available for composed kernel matrices")
-
-    @property
-    def num_qubits(self) -> int:
-        raise RuntimeError("The number of qubits is not available for composed kernel matrices")
-
-    @property
-    def num_features(self) -> int:
-        return self._km1.num_features
-
-    @property
-    def num_parameters(self) -> int:
-        return self._km1.num_parameters + self._km2.num_parameters
-
-    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
-        K1 = self._km1.evaluate(x, y)
-        K2 = self._km2.evaluate(x, y)
-
-        if self._composition == "*":
-            return np.multiply(K1, K2)
-        elif self._composition == "/":
-            return np.divide(K1, K2)
-        elif self._composition == "+":
-            return np.add(K1, K2)
-        elif self._composition == "-":
-            return np.subtract(K1, K2)
-        else:
-            raise ValueError("Unknown composition: ", self._composition)
-
-    def assign_parameters(self, parameters):
-        self._km1.assign_parameters(parameters[: self._km1.num_parameters])
-        self._km2.assign_parameters(parameters[self._km1.num_parameters :])
+import numpy as np
+
+from ...feature_map.feature_map_base import FeatureMapBase
+from ...util.executor import Executor
+
+
+class KernelMatrixBase:
+    def __init__(
+        self,
+        feature_map: FeatureMapBase,
+        executor: Executor,
+        initial_parameters=None,
+    ) -> None:
+        self._feature_map = feature_map
+        self._num_qubits = self._feature_map.num_qubits
+        self._num_features = self._feature_map.num_features
+        self._num_parameters = self._feature_map.num_parameters
+        self._executor = executor
+        self._parameters = initial_parameters
+
+    @property
+    def feature_map(self) -> FeatureMapBase:
+        """
+        Returns the feature map from which the kernel matrix is constructed
+        """
+        return self._feature_map
+
+    @property
+    def num_qubits(self) -> int:
+        return self._num_qubits
+
+    @property
+    def num_features(self) -> int:
+        return self._num_features
+
+    @property
+    def num_parameters(self) -> int:
+        return self._num_parameters
+
+    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
+        raise NotImplementedError()
+
+    def evaluate_pairwise(self, x: np.ndarray, y: np.ndarray = None) -> float:
+        if y is not None:
+            return self.evaluate([x], [y])[0, 0]
+        else:
+            return self.evaluate([x], None)[0, 0]
+
+    def assign_parameters(self, parameters):
+        self._parameters = parameters
+
+    def evaluate_with_parameters(
+        self, x: np.ndarray, y: np.ndarray, parameters: np.ndarray
+    ) -> np.ndarray:
+        self.assign_parameters(parameters)
+        return self.evaluate(x, y)
+
+    def __add__(self, x):
+        return _ComposedKernelMatrix(self, x, "+")
+
+    def __mul__(self, x):
+        return _ComposedKernelMatrix(self, x, "*")
+
+    def __sub__(self, x):
+        return _ComposedKernelMatrix(self, x, "-")
+
+    def __div__(self, x):
+        return _ComposedKernelMatrix(self, x, "/")
+
+    def get_params(self, deep=True):
+        return {
+            "feature_map": self._feature_map,
+            "executor": self._executor,
+            "initial_parameters": self._parameters,
+        }
+
+    def set_params(self, **params):
+        for param, value in params.items():
+            setattr(self, "_" + param, value)
+        return self
+
+
+class _ComposedKernelMatrix(KernelMatrixBase):
+    def __init__(self, km1: KernelMatrixBase, km2: KernelMatrixBase, composition: str = "*"):
+        if km1.num_features != km2.num_features:
+            raise ValueError("Feature dimension is not equal in both feature maps.")
+
+        self._km1 = km1
+        self._km2 = km2
+        self._composition = composition
+
+    @property
+    def feature_map(self) -> FeatureMapBase:
+        """
+        Returns the feature map from which the kernel matrix is constructed
+        """
+        raise RuntimeError("The feature map is not available for composed kernel matrices")
+
+    @property
+    def num_qubits(self) -> int:
+        raise RuntimeError("The number of qubits is not available for composed kernel matrices")
+
+    @property
+    def num_features(self) -> int:
+        return self._km1.num_features
+
+    @property
+    def num_parameters(self) -> int:
+        return self._km1.num_parameters + self._km2.num_parameters
+
+    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
+        K1 = self._km1.evaluate(x, y)
+        K2 = self._km2.evaluate(x, y)
+
+        if self._composition == "*":
+            return np.multiply(K1, K2)
+        elif self._composition == "/":
+            return np.divide(K1, K2)
+        elif self._composition == "+":
+            return np.add(K1, K2)
+        elif self._composition == "-":
+            return np.subtract(K1, K2)
+        else:
+            raise ValueError("Unknown composition: ", self._composition)
+
+    def assign_parameters(self, parameters):
+        self._km1.assign_parameters(parameters[: self._km1.num_parameters])
+        self._km2.assign_parameters(parameters[self._km1.num_parameters :])
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py` & `squlearn-0.2.0/src/squlearn/kernel/matrix/projected_quantum_kernel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,370 +1,382 @@
-"""Projected Quantum Kernel class"""
-
-from typing import Union, List
-import numpy as np
-from abc import abstractmethod
-
-from sklearn.gaussian_process.kernels import (
-    RBF,
-    Matern,
-    ExpSineSquared,
-    RationalQuadratic,
-    DotProduct,
-    PairwiseKernel,
-)
-
-from sklearn.gaussian_process.kernels import Kernel as SklearnKernel
-
-from .kernel_matrix_base import KernelMatrixBase
-from ...feature_map.feature_map_base import FeatureMapBase
-from ...util import Executor
-from ...qnn.qnn import QNN
-from ...expectation_operator import SinglePauli, ExpectationOperatorBase
-
-
-class OuterKernelBase:
-    """
-    Class for creating outer kernels for the projected quantum kernel
-    """
-    def __init__(self):
-        self._num_hyper_parameters = 0
-        self._name_hyper_parameters = []
-
-    @abstractmethod
-    def __call__(
-        self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None
-    ) -> np.ndarray:
-        """
-        Args:
-            qnn: QNN object
-            parameters: parameters of the QNN
-            x: first input
-            y: second optional input
-
-        Returns:
-            Evaluated projected kernel matrix
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def get_params(self) -> dict:
-        """Returns the hyper parameters of the outer kernel"""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def set_params(self,**kwarg):
-        """Sets the hyper parameters of the outer kernel"""
-        raise NotImplementedError()
-
-    @property
-    def num_hyper_parameters(self) -> int:
-        """Returns the number of hyper parameters of the outer kernel"""
-        return self._num_hyper_parameters
-
-    @property
-    def name_hyper_parameters(self) -> List[str]:
-        """Returns the names of the hyper parameters of the outer kernel"""
-        return self._name_hyper_parameters
-
-    @classmethod
-    def from_sklearn_kernel(cls,kernel:SklearnKernel,**kwarg):
-        """Converts a sklearn kernel into a squlearn kernel
-
-        Args:
-            kernel: sklearn kernel
-            kwarg: arguments for the sklearn kernel parameters
-        """
-        class SklearnOuterKernel(BaseException):
-            """
-            Class for creating outer kernels for the projected quantum kernel from sklearn kernels
-
-            Args:
-                kernel: sklearn kernel
-                kwarg: arguments for the sklearn kernel parameters
-            """
-            def __init__(self, kernel:SklearnKernel, **kwarg):
-                super().__init__()
-                self._kernel = kernel(**kwarg)
-                self._name_hyper_parameters = [ p.name for p in self._kernel.hyperparameters]
-                self._num_hyper_parameters = len(self._name_hyper_parameters)
-            def __call__(self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
-                """ Evaluates the outer kernel
-
-                Args:
-                    qnn: QNN object
-                    parameters: parameters of the QNN
-                    x: first input
-                    y: second optional input
-                """
-                # Evaluate QNN
-                param = parameters[: qnn.num_parameters]
-                param_op = parameters[qnn.num_parameters :]
-                x_result = qnn.evaluate_f(x, param, param_op)
-                if y is not None:
-                    y_result = qnn.evaluate_f(y, param, param_op)
-                else:
-                    y_result = None
-                # Evaluate kernel
-                return self._kernel(x_result, y_result)
-            def get_params(self) -> dict:
-                """ Returns the hyper parameters of the outer kernel as a dictionary. """
-                return self._kernel.get_params()
-            def set_params(self,**kwarg):
-                """ Sets the hyper parameters of the outer kernel. """
-                self._kernel.set_params(**kwarg)
-
-        return SklearnOuterKernel(kernel,**kwarg)
-
-
-class ProjectedQuantumKernel(KernelMatrixBase):
-
-    """ Projected Quantum Kernel
-
-    The projected quantum kernel embeds classical data into a quantum Hilbert space and
-    than projects down into a real space by measurements. The kernel is than evaluated in the
-    real space. The implementation is based on the paper https://doi.org/10.1038/s41467-021-22539-9
-
-    Args:
-        feature_map (FeatureMapBase): PQC feature map
-        executor (Executor): Executor object
-        measurement (Union[str, ExpectationOperatorBase, list]): Measurements that are
-            performed on the PQC. Possible string values: "Z", "XYZ"
-        outer_kernel (Union[str, OuterKernelBase]): OuterKernel that is applied to the PQC output.
-            Possible string values are: "Gaussian", "Matern", "ExpSineSquared",
-            "RationalQuadratic", "DotProduct", "PairwiseKernel"
-        initial_parameters (np.ndarray): initial parameters of the QNN
-
-    Outer Kernels that are implemented:
-
-    Gaussian:
-    ---------
-    .. math::
-        k(x_i, x_j) = \text{exp}\left(-\\gamma |(QNN(x_i)- QNN(x_j)|^2 \right)
-
-    Args:
-        gamma (float): hyperparameter :math:`\\gamma` of the Gaussian kernel
-
-    Matern:
-    -------
-    .. math::
-         k(x_i, x_j) =  \\frac{1}{\\Gamma(\\nu)2^{\\nu-1}}\\Bigg(
-         \\frac{\\sqrt{2\\nu}}{l} d(QNN(x_i) , QNN(x_j) )
-         \\Bigg)^\\nu K_\\nu\\Bigg(
-         \\frac{\\sqrt{2\\nu}}{l} d(QNN(x_i) , QNN(x_j) )\\Bigg)
-
-    Args:
-        nu (float): hyperparameter :math:`\\nu` of the Matern kernel (Typically 0.5, 1.5 or 2.5)
-        length_scale (float): hyperparameter :math:`l` of the Matern kernel
-
-    ExpSineSquared:
-    ---------------
-    .. math::
-        k(x_i, x_j) = \text{exp}\left(-
-        \frac{ 2\sin^2(\pi d(QNN(x_i), QNN(x_j))/p) }{ l^ 2} \right)
-
-    Args:
-        periodicity (float): hyperparameter :math:`p` of the ExpSineSquared kernel
-        length_scale (float): hyperparameter :math:`l` of the ExpSineSquared kernel
-
-    RationalQuadratic:
-    ------------------
-    .. math::
-        k(x_i, x_j) = \\left(
-        1 + \\frac{d(QNN(x_i), QNN(x_j))^2 }{ 2\\alpha  l^2}\\right)^{-\\alpha}s
-
-    Args:
-        alpha (float): hyperparameter :math:`\\alpha` of the RationalQuadratic kernel
-        length_scale (float): hyperparameter :math:`l` of the RationalQuadratic kernel
-
-    DotProduct:
-    -----------
-    .. math::
-        k(x_i, x_j) = \sigma_0 ^ 2 + x_i \cdot x_j
-
-    Args:
-        sigma_0 (float): hyperparameter :math:`\sigma_0` of the DotProduct kernel
-
-    PairwiseKernel:
-    ---------------
-    Args:
-        gamma (float): Hyperparameter gamma of the PairwiseKernel kernel, specified by the metric
-        metric (str): Metric of the PairwiseKernel kernel, can be "linear", "additive_chi2",
-              "chi2", "poly", "polynomial", "rbf", "laplacian", "sigmoid", "cosine"
-
-    """
-
-    def __init__(
-        self,
-        feature_map: FeatureMapBase,
-        executor: Executor,
-        measurement: Union[str, ExpectationOperatorBase, list] = "XYZ",
-        outer_kernel: Union[str, OuterKernelBase] = "gaussian",
-        initial_parameters: np.ndarray = None,
-        **kwargs
-    ) -> None:
-        super().__init__(feature_map, executor, initial_parameters)
-
-        # Set-up measurement operator
-        if isinstance(measurement, str):
-            if measurement == "Z":
-                # Measure Z at all qubits
-                self._measurement = []
-                for i in range(self.num_qubits):
-                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Z"))
-            elif measurement == "XYZ":
-                # Measure X, Y, and Z at all qubits
-                self._measurement = []
-                for i in range(self.num_qubits):
-                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="X"))
-                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Y"))
-                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Z"))
-            else:
-                raise ValueError("Unknown measurement string: {}".format(measurement))
-        elif isinstance(measurement, ExpectationOperatorBase) or isinstance(measurement, list):
-            self._measurement = measurement
-        else:
-            raise ValueError("Unknown type of measurement: {}".format(type(measurement)))
-
-        # Set-up of the QNN
-        self._qnn = QNN(self._feature_map, self._measurement, executor)
-        self._num_param = self._qnn.num_parameters
-        self._num_param_op = self._qnn.num_parameters_operator
-        self._num_parameters = self._num_param + self._num_param_op
-
-        # Set-up of the outer kernel
-        if isinstance(outer_kernel, str):
-            if outer_kernel.lower() == "gaussian":
-                self._outer_kernel = GaussianOuterKernel(**kwargs)
-            elif outer_kernel.lower() == "matern":
-                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(Matern,**kwargs)
-            elif outer_kernel.lower() == "expsinesquared":
-                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(ExpSineSquared,**kwargs)
-            elif outer_kernel.lower() == "rationalquadratic":
-                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(RationalQuadratic,**kwargs)
-            elif outer_kernel.lower() == "dotproduct":
-                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(DotProduct,**kwargs)
-            elif outer_kernel.lower() == "pairwisekernel":
-                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(PairwiseKernel,**kwargs)
-            else:
-                raise ValueError("Unknown outer kernel: {}".format(outer_kernel))
-        elif isinstance(outer_kernel, OuterKernelBase):
-            self._outer_kernel = outer_kernel
-        else:
-            raise ValueError("Unknown type of outer kernel: {}".format(type(outer_kernel)))
-
-        # Check if the number of parameters is correct
-        if self._parameters is not None:
-            if len(self._parameters) != self._num_parameters:
-                raise ValueError(
-                    "Number of inital parameters is wrong, expected number: {}".format(
-                        self._num_parameters
-                    )
-                )
-
-    @property
-    def num_features(self) -> int:
-        return self._num_features
-
-    @property
-    def num_parameters(self) -> int:
-        return self._num_parameters
-
-    @property
-    def measurement(self):
-        return self._measurement
-
-    @property
-    def outer_kernel(self):
-        return self._outer_kernel
-
-    def evaluate_qnn(self, x: np.ndarray) -> np.ndarray:
-        # Copy parameters in QNN form
-        if self._parameters is None:
-            raise ValueError("Parameters have not been set yet!")
-        param = self._parameters[: self._qnn.num_parameters]
-        param_op = self._parameters[self._qnn.num_parameters :]
-        return self._qnn.evaluate_f(x, param, param_op)
-
-    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
-        """Evaluates the Projected Quantum Kernel for the given data points x and y.
-
-        Args:
-            x (np.ndarray): Data points x
-            y (np.ndarray): Data points y, if None y = x is used
-
-        Returns:
-            The evaluated projected quantum kernel as numpy array
-        """
-        if self._parameters is None:
-            raise ValueError("Parameters have not been set yet!")
-
-        return self._outer_kernel(self._qnn, self._parameters, x, y)
-
-    def get_params(self) -> dict:
-        """Returns the hyper parameters of the outer kernel"""
-        return self._outer_kernel.get_params()
-
-    def set_params(self,**kwarg):
-        """Sets the hyper parameters of the outer kernel"""
-        self._outer_kernel.set_params(**kwarg)
-
-    @property
-    def num_hyper_parameters(self) -> int:
-        """Returns the number of hyper parameters of the outer kernel"""
-        return self._outer_kernel.num_hyper_parameters
-
-    @property
-    def name_hyper_parameters(self) -> List[str]:
-        """Returns the names of the hyper parameters of the outer kernel"""
-        return self._outer_kernel.name_hyper_parameters
-
-class GaussianOuterKernel(OuterKernelBase):
-    """
-    Implementation of the Gaussian outer kernel:
-
-    .. math::
-        k(x_i, x_j) = \text{exp}\left(-\\gamma |(QNN(x_i)- QNN(x_j)|^2 \right)
-
-    Args:
-        gamma (float): hyperparameter :math:`\\gamma` of the Gaussian kernel
-    """
-
-    def __init__(self, gamma=1.0):
-        super().__init__()
-        self._gamma = gamma
-        self._num_hyper_parameters = 1
-        self._name_hyper_parameters = ["gamma"]
-
-    def __call__(
-        self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None
-    ) -> np.ndarray:
-        """Evaluates the QNN and returns the Gaussian projected kernel
-
-        Args:
-            qnn (QNN): QNN to be evaluated
-            parameters (np.ndarray): parameters of the QNN
-            x (np.ndarray): input data
-            y (np.ndarray): second optional input data
-
-        Returns:
-            np.ndarray: Gaussian projected kernel
-        """
-
-        # Evaluate QNN
-        param = parameters[: qnn.num_parameters]
-        param_op = parameters[qnn.num_parameters :]
-        x_result = qnn.evaluate_f(x, param, param_op)
-        if y is not None:
-            y_result = qnn.evaluate_f(y, param, param_op)
-        else:
-            y_result = None
-
-        return RBF(length_scale = 1.0 / np.sqrt(2.0 * self._gamma))(x_result, y_result)
-
-    def get_params(self) -> dict:
-        """ Returns the hyper parameters of the outer kernel. """
-        return {'gamma': self._gamma}
-
-    def set_params(self, gamma) -> None:
-        """ Sets the hyper parameters of the outer kernel. """
-        self._gamma = gamma
+"""Projected Quantum Kernel class"""
+
+from typing import Union, List
+import numpy as np
+from abc import abstractmethod
+
+from sklearn.gaussian_process.kernels import (
+    RBF,
+    Matern,
+    ExpSineSquared,
+    RationalQuadratic,
+    DotProduct,
+    PairwiseKernel,
+)
+
+from sklearn.gaussian_process.kernels import Kernel as SklearnKernel
+
+from .kernel_matrix_base import KernelMatrixBase
+from ...feature_map.feature_map_base import FeatureMapBase
+from ...util import Executor
+from ...qnn.qnn import QNN
+from ...expectation_operator import SinglePauli
+from ...expectation_operator.expectation_operator_base import ExpectationOperatorBase
+
+
+class OuterKernelBase:
+    """
+    Class for creating outer kernels for the projected quantum kernel
+    """
+
+    def __init__(self):
+        self._num_hyper_parameters = 0
+        self._name_hyper_parameters = []
+
+    @abstractmethod
+    def __call__(
+        self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None
+    ) -> np.ndarray:
+        """
+        Args:
+            qnn: QNN object
+            parameters: parameters of the QNN
+            x: first input
+            y: second optional input
+
+        Returns:
+            Evaluated projected kernel matrix
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def get_params(self) -> dict:
+        """Returns the hyper parameters of the outer kernel"""
+        raise NotImplementedError()
+
+    @abstractmethod
+    def set_params(self, **kwarg):
+        """Sets the hyper parameters of the outer kernel"""
+        raise NotImplementedError()
+
+    @property
+    def num_hyper_parameters(self) -> int:
+        """Returns the number of hyper parameters of the outer kernel"""
+        return self._num_hyper_parameters
+
+    @property
+    def name_hyper_parameters(self) -> List[str]:
+        """Returns the names of the hyper parameters of the outer kernel"""
+        return self._name_hyper_parameters
+
+    @classmethod
+    def from_sklearn_kernel(cls, kernel: SklearnKernel, **kwarg):
+        """Converts a sklearn kernel into a squlearn kernel
+
+        Args:
+            kernel: sklearn kernel
+            kwarg: arguments for the sklearn kernel parameters
+        """
+
+        class SklearnOuterKernel(BaseException):
+            """
+            Class for creating outer kernels for the projected quantum kernel from sklearn kernels
+
+            Args:
+                kernel: sklearn kernel
+                kwarg: arguments for the sklearn kernel parameters
+            """
+
+            def __init__(self, kernel: SklearnKernel, **kwarg):
+                super().__init__()
+                self._kernel = kernel(**kwarg)
+                self._name_hyper_parameters = [p.name for p in self._kernel.hyperparameters]
+                self._num_hyper_parameters = len(self._name_hyper_parameters)
+
+            def __call__(
+                self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None
+            ) -> np.ndarray:
+                """Evaluates the outer kernel
+
+                Args:
+                    qnn: QNN object
+                    parameters: parameters of the QNN
+                    x: first input
+                    y: second optional input
+                """
+                # Evaluate QNN
+                param = parameters[: qnn.num_parameters]
+                param_op = parameters[qnn.num_parameters :]
+                x_result = qnn.evaluate_f(x, param, param_op)
+                if y is not None:
+                    y_result = qnn.evaluate_f(y, param, param_op)
+                else:
+                    y_result = None
+                # Evaluate kernel
+                return self._kernel(x_result, y_result)
+
+            def get_params(self) -> dict:
+                """Returns the hyper parameters of the outer kernel as a dictionary."""
+                return self._kernel.get_params()
+
+            def set_params(self, **kwarg):
+                """Sets the hyper parameters of the outer kernel."""
+                self._kernel.set_params(**kwarg)
+
+        return SklearnOuterKernel(kernel, **kwarg)
+
+
+class ProjectedQuantumKernel(KernelMatrixBase):
+
+    """Projected Quantum Kernel
+
+    The projected quantum kernel embeds classical data into a quantum Hilbert space and
+    than projects down into a real space by measurements. The kernel is than evaluated in the
+    real space. The implementation is based on the paper https://doi.org/10.1038/s41467-021-22539-9
+
+    Args:
+        feature_map (FeatureMapBase): PQC feature map
+        executor (Executor): Executor object
+        measurement (Union[str, ExpectationOperatorBase, list]): Measurements that are
+            performed on the PQC. Possible string values: "Z", "XYZ"
+        outer_kernel (Union[str, OuterKernelBase]): OuterKernel that is applied to the PQC output.
+            Possible string values are: "Gaussian", "Matern", "ExpSineSquared",
+            "RationalQuadratic", "DotProduct", "PairwiseKernel"
+        initial_parameters (np.ndarray): initial parameters of the QNN
+
+    Outer Kernels that are implemented:
+
+    Gaussian:
+    ---------
+    .. math::
+        k(x_i, x_j) = \text{exp}\left(-\\gamma |(QNN(x_i)- QNN(x_j)|^2 \right)
+
+    Args:
+        gamma (float): hyperparameter :math:`\\gamma` of the Gaussian kernel
+
+    Matern:
+    -------
+    .. math::
+         k(x_i, x_j) =  \\frac{1}{\\Gamma(\\nu)2^{\\nu-1}}\\Bigg(
+         \\frac{\\sqrt{2\\nu}}{l} d(QNN(x_i) , QNN(x_j) )
+         \\Bigg)^\\nu K_\\nu\\Bigg(
+         \\frac{\\sqrt{2\\nu}}{l} d(QNN(x_i) , QNN(x_j) )\\Bigg)
+
+    Args:
+        nu (float): hyperparameter :math:`\\nu` of the Matern kernel (Typically 0.5, 1.5 or 2.5)
+        length_scale (float): hyperparameter :math:`l` of the Matern kernel
+
+    ExpSineSquared:
+    ---------------
+    .. math::
+        k(x_i, x_j) = \text{exp}\left(-
+        \frac{ 2\sin^2(\pi d(QNN(x_i), QNN(x_j))/p) }{ l^ 2} \right)
+
+    Args:
+        periodicity (float): hyperparameter :math:`p` of the ExpSineSquared kernel
+        length_scale (float): hyperparameter :math:`l` of the ExpSineSquared kernel
+
+    RationalQuadratic:
+    ------------------
+    .. math::
+        k(x_i, x_j) = \\left(
+        1 + \\frac{d(QNN(x_i), QNN(x_j))^2 }{ 2\\alpha  l^2}\\right)^{-\\alpha}s
+
+    Args:
+        alpha (float): hyperparameter :math:`\\alpha` of the RationalQuadratic kernel
+        length_scale (float): hyperparameter :math:`l` of the RationalQuadratic kernel
+
+    DotProduct:
+    -----------
+    .. math::
+        k(x_i, x_j) = \sigma_0 ^ 2 + x_i \cdot x_j
+
+    Args:
+        sigma_0 (float): hyperparameter :math:`\sigma_0` of the DotProduct kernel
+
+    PairwiseKernel:
+    ---------------
+    Args:
+        gamma (float): Hyperparameter gamma of the PairwiseKernel kernel, specified by the metric
+        metric (str): Metric of the PairwiseKernel kernel, can be "linear", "additive_chi2",
+              "chi2", "poly", "polynomial", "rbf", "laplacian", "sigmoid", "cosine"
+
+    """
+
+    def __init__(
+        self,
+        feature_map: FeatureMapBase,
+        executor: Executor,
+        measurement: Union[str, ExpectationOperatorBase, list] = "XYZ",
+        outer_kernel: Union[str, OuterKernelBase] = "gaussian",
+        initial_parameters: np.ndarray = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(feature_map, executor, initial_parameters)
+
+        # Set-up measurement operator
+        if isinstance(measurement, str):
+            if measurement == "Z":
+                # Measure Z at all qubits
+                self._measurement = []
+                for i in range(self.num_qubits):
+                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Z"))
+            elif measurement == "XYZ":
+                # Measure X, Y, and Z at all qubits
+                self._measurement = []
+                for i in range(self.num_qubits):
+                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="X"))
+                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Y"))
+                    self._measurement.append(SinglePauli(self.num_qubits, i, op_str="Z"))
+            else:
+                raise ValueError("Unknown measurement string: {}".format(measurement))
+        elif isinstance(measurement, ExpectationOperatorBase) or isinstance(measurement, list):
+            self._measurement = measurement
+        else:
+            raise ValueError("Unknown type of measurement: {}".format(type(measurement)))
+
+        # Set-up of the QNN
+        self._qnn = QNN(self._feature_map, self._measurement, executor)
+        self._num_param = self._qnn.num_parameters
+        self._num_param_op = self._qnn.num_parameters_operator
+        self._num_parameters = self._num_param + self._num_param_op
+
+        # Set-up of the outer kernel
+        if isinstance(outer_kernel, str):
+            if outer_kernel.lower() == "gaussian":
+                self._outer_kernel = GaussianOuterKernel(**kwargs)
+            elif outer_kernel.lower() == "matern":
+                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(Matern, **kwargs)
+            elif outer_kernel.lower() == "expsinesquared":
+                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(ExpSineSquared, **kwargs)
+            elif outer_kernel.lower() == "rationalquadratic":
+                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(
+                    RationalQuadratic, **kwargs
+                )
+            elif outer_kernel.lower() == "dotproduct":
+                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(DotProduct, **kwargs)
+            elif outer_kernel.lower() == "pairwisekernel":
+                self._outer_kernel = OuterKernelBase.from_sklearn_kernel(PairwiseKernel, **kwargs)
+            else:
+                raise ValueError("Unknown outer kernel: {}".format(outer_kernel))
+        elif isinstance(outer_kernel, OuterKernelBase):
+            self._outer_kernel = outer_kernel
+        else:
+            raise ValueError("Unknown type of outer kernel: {}".format(type(outer_kernel)))
+
+        # Check if the number of parameters is correct
+        if self._parameters is not None:
+            if len(self._parameters) != self._num_parameters:
+                raise ValueError(
+                    "Number of inital parameters is wrong, expected number: {}".format(
+                        self._num_parameters
+                    )
+                )
+
+    @property
+    def num_features(self) -> int:
+        return self._num_features
+
+    @property
+    def num_parameters(self) -> int:
+        return self._num_parameters
+
+    @property
+    def measurement(self):
+        return self._measurement
+
+    @property
+    def outer_kernel(self):
+        return self._outer_kernel
+
+    def evaluate_qnn(self, x: np.ndarray) -> np.ndarray:
+        # Copy parameters in QNN form
+        if self._parameters is None:
+            raise ValueError("Parameters have not been set yet!")
+        param = self._parameters[: self._qnn.num_parameters]
+        param_op = self._parameters[self._qnn.num_parameters :]
+        return self._qnn.evaluate_f(x, param, param_op)
+
+    def evaluate(self, x: np.ndarray, y: np.ndarray = None) -> np.ndarray:
+        """Evaluates the Projected Quantum Kernel for the given data points x and y.
+
+        Args:
+            x (np.ndarray): Data points x
+            y (np.ndarray): Data points y, if None y = x is used
+
+        Returns:
+            The evaluated projected quantum kernel as numpy array
+        """
+        if self._parameters is None:
+            raise ValueError("Parameters have not been set yet!")
+
+        return self._outer_kernel(self._qnn, self._parameters, x, y)
+
+    def get_params(self) -> dict:
+        """Returns the hyper parameters of the outer kernel"""
+        return self._outer_kernel.get_params()
+
+    def set_params(self, **kwarg):
+        """Sets the hyper parameters of the outer kernel"""
+        self._outer_kernel.set_params(**kwarg)
+
+    @property
+    def num_hyper_parameters(self) -> int:
+        """Returns the number of hyper parameters of the outer kernel"""
+        return self._outer_kernel.num_hyper_parameters
+
+    @property
+    def name_hyper_parameters(self) -> List[str]:
+        """Returns the names of the hyper parameters of the outer kernel"""
+        return self._outer_kernel.name_hyper_parameters
+
+
+class GaussianOuterKernel(OuterKernelBase):
+    """
+    Implementation of the Gaussian outer kernel:
+
+    .. math::
+        k(x_i, x_j) = \text{exp}\left(-\\gamma |(QNN(x_i)- QNN(x_j)|^2 \right)
+
+    Args:
+        gamma (float): hyperparameter :math:`\\gamma` of the Gaussian kernel
+    """
+
+    def __init__(self, gamma=1.0):
+        super().__init__()
+        self._gamma = gamma
+        self._num_hyper_parameters = 1
+        self._name_hyper_parameters = ["gamma"]
+
+    def __call__(
+        self, qnn: QNN, parameters: np.ndarray, x: np.ndarray, y: np.ndarray = None
+    ) -> np.ndarray:
+        """Evaluates the QNN and returns the Gaussian projected kernel
+
+        Args:
+            qnn (QNN): QNN to be evaluated
+            parameters (np.ndarray): parameters of the QNN
+            x (np.ndarray): input data
+            y (np.ndarray): second optional input data
+
+        Returns:
+            np.ndarray: Gaussian projected kernel
+        """
+
+        # Evaluate QNN
+        param = parameters[: qnn.num_parameters]
+        param_op = parameters[qnn.num_parameters :]
+        x_result = qnn.evaluate_f(x, param, param_op)
+        if y is not None:
+            y_result = qnn.evaluate_f(y, param, param_op)
+        else:
+            y_result = None
+
+        return RBF(length_scale=1.0 / np.sqrt(2.0 * self._gamma))(x_result, y_result)
+
+    def get_params(self) -> dict:
+        """Returns the hyper parameters of the outer kernel."""
+        return {"gamma": self._gamma}
+
+    def set_params(self, gamma) -> None:
+        """Sets the hyper parameters of the outer kernel."""
+        self._gamma = gamma
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/ml/kernel_util.py` & `squlearn-0.2.0/src/squlearn/kernel/ml/kernel_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,55 +1,59 @@
-# kernel util 
-import numpy as np
-import scipy
-from sklearn.gaussian_process.kernels import Kernel
-from ..matrix import KernelMatrixBase
-
-def kernel_wrapper(kernel_matrix: KernelMatrixBase):
-    class CustomKernel(Kernel):
-        def __init__(self, kernel_matrix: KernelMatrixBase):
-            self.kernel_matrix = kernel_matrix
-            super().__init__()
-
-        def __call__(self, X, Y=None, eval_gradient=False):
-            if Y is None:
-                Y = X
-            kernel_matrix = self.kernel_matrix.evaluate(X, Y)
-            if eval_gradient:
-                raise NotImplementedError("Gradient not yet implemented for this kernel.")
-            else:
-                return kernel_matrix
-
-        def diag(self, X):
-            return np.diag(self.kernel_matrix.evaluate(X))
-
-        @property
-        def requires_vector_input(self):
-            return True
-        
-        def is_stationary(self):
-            return self.kernel_matrix.is_stationary()
-    return CustomKernel(kernel_matrix)
-
-
-def regularize_kernel(gram_matrix):
-    evals, evecs = scipy.linalg.eig(gram_matrix)
-    reconstruction = evecs @ np.diag(evals.clip(min=0)) @ evecs.T
-    return np.real(reconstruction)
-
-# deprecated regularization technique
-def tikhonov_regularization(gram_matrix):
-    evals = scipy.linalg.eigvals(gram_matrix)
-    if np.min(np.real(evals)) < 0:
-        gram_matrix -= np.min(np.real(evals)) * np.identity(gram_matrix.shape[0])
-    return gram_matrix
-
-def regularize_full_kernel(K_train, K_testtrain, K_test):
-    gram_matrix_total = np.block([[K_train, K_testtrain.T], [K_testtrain, K_test]])
-    reconstruction = regularize_kernel(gram_matrix_total)
-    print(f"Reconstruction error {np.sum(reconstruction - gram_matrix_total)}")
-
-    K_train = reconstruction[: K_train.shape[0], : K_train.shape[1]]
-    K_testtrain = reconstruction[K_train.shape[0] :, : K_testtrain.shape[1]]
-    K_test = reconstruction[-K_test.shape[0] :, -K_test.shape[1] :]
-
-    return K_train, K_testtrain, K_test
+# kernel util
+import numpy as np
+import scipy
+from sklearn.gaussian_process.kernels import Kernel
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+
+def kernel_wrapper(kernel_matrix: KernelMatrixBase):
+    class CustomKernel(Kernel):
+        def __init__(self, kernel_matrix: KernelMatrixBase):
+            self.kernel_matrix = kernel_matrix
+            super().__init__()
+
+        def __call__(self, X, Y=None, eval_gradient=False):
+            if Y is None:
+                Y = X
+            kernel_matrix = self.kernel_matrix.evaluate(X, Y)
+            if eval_gradient:
+                raise NotImplementedError("Gradient not yet implemented for this kernel.")
+            else:
+                return kernel_matrix
+
+        def diag(self, X):
+            return np.diag(self.kernel_matrix.evaluate(X))
+
+        @property
+        def requires_vector_input(self):
+            return True
+
+        def is_stationary(self):
+            return self.kernel_matrix.is_stationary()
+
+    return CustomKernel(kernel_matrix)
+
+
+def regularize_kernel(gram_matrix):
+    evals, evecs = scipy.linalg.eig(gram_matrix)
+    reconstruction = evecs @ np.diag(evals.clip(min=0)) @ evecs.T
+    return np.real(reconstruction)
+
+
+# deprecated regularization technique
+def tikhonov_regularization(gram_matrix):
+    evals = scipy.linalg.eigvals(gram_matrix)
+    if np.min(np.real(evals)) < 0:
+        gram_matrix -= np.min(np.real(evals)) * np.identity(gram_matrix.shape[0])
+    return gram_matrix
+
+
+def regularize_full_kernel(K_train, K_testtrain, K_test):
+    gram_matrix_total = np.block([[K_train, K_testtrain.T], [K_testtrain, K_test]])
+    reconstruction = regularize_kernel(gram_matrix_total)
+    print(f"Reconstruction error {np.sum(reconstruction - gram_matrix_total)}")
+
+    K_train = reconstruction[: K_train.shape[0], : K_train.shape[1]]
+    K_testtrain = reconstruction[K_train.shape[0] :, : K_testtrain.shape[1]]
+    K_test = reconstruction[-K_test.shape[0] :, -K_test.shape[1] :]
+
+    return K_train, K_testtrain, K_test
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/ml/qgpc.py` & `squlearn-0.2.0/src/squlearn/kernel/ml/qgpc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-# QGPC
-import numpy as np
-from ..matrix import KernelMatrixBase
-from .kernel_util import kernel_wrapper
-from sklearn.gaussian_process import GaussianProcessClassifier
-
-class QGPC(GaussianProcessClassifier):
-    """Quantum Gaussian process regression (QGPC).
-
-    Args:
-    ---------
-    quantum_kernel: KernelMatrixBase class quantum kernel object
-    (either a fidelity kernel or the PQK must be provided)
-    """
-
-    def __init__(
-            self,
-            quantum_kernel: KernelMatrixBase,
-            **kwargs
-    ):
-        self._quantum_kernel = quantum_kernel
-        super().__init__(**kwargs)
-        self.kernel = kernel_wrapper(quantum_kernel)
-
-    @property
-    def quantum_kernel(self) -> KernelMatrixBase:
-        """Returns quantum kernel"""
-        return self._quantum_kernel
-
-    @quantum_kernel.setter
-    def quantum_kernel(self, quantum_kernel: KernelMatrixBase):
-        """Sets quantum kernel"""
-        self._quantum_kernel = quantum_kernel
-        self.kernel = kernel_wrapper(quantum_kernel)
+# QGPC
+import numpy as np
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+from .kernel_util import kernel_wrapper
+from sklearn.gaussian_process import GaussianProcessClassifier
+
+
+class QGPC(GaussianProcessClassifier):
+    """Quantum Gaussian process regression (QGPC).
+
+    Args:
+    ---------
+    quantum_kernel: KernelMatrixBase class quantum kernel object
+    (either a fidelity kernel or the PQK must be provided)
+    """
+
+    def __init__(self, quantum_kernel: KernelMatrixBase, **kwargs):
+        self._quantum_kernel = quantum_kernel
+        super().__init__(**kwargs)
+        self.kernel = kernel_wrapper(quantum_kernel)
+
+    @property
+    def quantum_kernel(self) -> KernelMatrixBase:
+        """Returns quantum kernel"""
+        return self._quantum_kernel
+
+    @quantum_kernel.setter
+    def quantum_kernel(self, quantum_kernel: KernelMatrixBase):
+        """Sets quantum kernel"""
+        self._quantum_kernel = quantum_kernel
+        self.kernel = kernel_wrapper(quantum_kernel)
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/ml/qkrr.py` & `squlearn-0.2.0/src/squlearn/kernel/ml/qkrr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,96 +1,88 @@
-"""Quantum Kernel Ridge Regressor"""
-from ..matrix import KernelMatrixBase
-
-import scipy
-import numpy as np
-from typing import Optional, Union
-from sklearn.base import BaseEstimator, RegressorMixin
-
-from .kernel_util import regularize_kernel, tikhonov_regularization
-
-#from ..kernel_util import KernelRegularizer, DepolarizingNoiseMitigation
-
-class QKRR(BaseEstimator, RegressorMixin):
-    """
-    Quantum Kernel Ridge Regression
-
-    This class implements the kernel ridge regression analogous to sklearn
-    but is not a wrapper.
-
-    Args:
-        quantum_kernel (KernelMatrixBase): The quantum kernel matrix to be used in the KRR pipeline
-            (either a fidelity quantum kernel (FQK) or projected quantum kernel (PQK) must be provided)
-        alpha (Union[float, np.ndarray]), default=1.e-6: Hyperparameter for the regularization strength; must be a positive float.
-            This regularization improves the conditioning of the problem and assure the solvability of the resulting
-            linear system. Larger values specify stronger regularization (cf., e.g., `https://en.wikipedia.org/wiki/Ridge_regression´)
-        regularize (Union[str, None]), default=None: Option for choosing different regularization techniques ('thresholding' or 'tikhonov')
-            after `http://arxiv.org/pdf/2105.02276v1´ for the training kernel matrix, prior to solving the linear system in the fit() procedure
-    """
-    def __init__(
-            self,
-            quantum_kernel: Optional[KernelMatrixBase] = None,
-            alpha: Union[float, np.ndarray] = 1.e-6,
-            regularize: Union[str, None] = None
-    ) -> None:
-        self._quantum_kernel = quantum_kernel # May be worth to set FQK as default here?
-        self.alpha = alpha
-        self._regularize = regularize
-        self.x_train = None
-        self.k_testtrain = None
-        self.k_train = None
-        self.dual_coeff_ = None
-        self.num_qubits = self._quantum_kernel.num_qubits
-
-    def fit(self, x_train: np.ndarray, y_train: np.ndarray):
-        if self._quantum_kernel.num_features > 1:
-            self.x_train = np.repeat(x_train.reshape(-1,1),
-                                     repeats=self._quantum_kernel.num_features,
-                                     axis=1)
-        else:
-            self.x_train = x_train
-        self.k_train = self._quantum_kernel.evaluate(x=self.x_train)  # set up kernel matrix
-        # check if regularize argument is set and define corresponding method
-        if self._regularize is not None:
-            if self._regularize == 'thresholding':
-                self.k_train = regularize_kernel(self.k_train)
-            elif self._regularize == 'tikhonov':
-                self.k_train = tikhonov_regularization(self.k_train)
-        
-        self.k_train = self.k_train + self.alpha * np.eye(self.k_train.shape[0])
-
-        # solution of KRR problem obtained by solving linear system K*\alpha = y
-        # using Cholesky decomposition for providing numerical stability
-        try:
-            L = scipy.linalg.cholesky(self.k_train, lower=True)
-            self.dual_coeff_ = scipy.linalg.cho_solve((L, True), y_train)
-        except np.linalg.LinAlgError:
-            print("Increase regularization parameter alpha")
-
-        return self
-
-    def predict(self, x_test: np.ndarray) -> np.ndarray:
-        if self.k_train is None:
-            raise ValueError("The fit() method has to be called beforehand.")
-        if self._quantum_kernel.num_features > 1:
-            x_test = np.repeat(
-                x_test.reshape(-1,1),
-                repeats=self._quantum_kernel.num_features,
-                axis=1
-            )
-        self.k_testtrain = self._quantum_kernel.evaluate(x_test, self.x_train)
-        prediction = np.dot(self.k_testtrain, self.dual_coeff_)
-        return prediction
-    
-    # All scikit-learn estimators have get_params and set_params 
-    # (cf. https://scikit-learn.org/stable/developers/develop.html)
-    def get_params(self, deep: bool = True):
-        return {
-            "quantum_kernel":self._quantum_kernel,
-            "alpha":self.alpha,
-            "regularize":self._regularize
-            }
-    
-    def set_params(self, **parameters):
-        for parameter, value in parameters.items():
-            setattr(self, parameter, value)
-        return self
+"""Quantum Kernel Ridge Regressor"""
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+import scipy
+import numpy as np
+from typing import Optional, Union
+from sklearn.base import BaseEstimator, RegressorMixin
+
+from .kernel_util import regularize_kernel, tikhonov_regularization
+
+# from ..kernel_util import KernelRegularizer, DepolarizingNoiseMitigation
+
+
+class QKRR(BaseEstimator, RegressorMixin):
+    """
+    Quantum Kernel Ridge Regression
+
+    This class implements the kernel ridge regression analogous to sklearn
+    but is not a wrapper.
+
+    Args:
+        quantum_kernel (KernelMatrixBase): The quantum kernel matrix to be used in the KRR pipeline
+            (either a fidelity quantum kernel (FQK) or projected quantum kernel (PQK) must be provided)
+        alpha (Union[float, np.ndarray]), default=1.e-6: Hyperparameter for the regularization strength; must be a positive float.
+            This regularization improves the conditioning of the problem and assure the solvability of the resulting
+            linear system. Larger values specify stronger regularization (cf., e.g., `https://en.wikipedia.org/wiki/Ridge_regression´)
+        regularize (Union[str, None]), default=None: Option for choosing different regularization techniques ('thresholding' or 'tikhonov')
+            after `http://arxiv.org/pdf/2105.02276v1´ for the training kernel matrix, prior to solving the linear system in the fit() procedure
+    """
+
+    def __init__(
+        self,
+        quantum_kernel: Optional[KernelMatrixBase] = None,
+        alpha: Union[float, np.ndarray] = 1.0e-6,
+        regularize: Union[str, None] = None,
+    ) -> None:
+        self._quantum_kernel = quantum_kernel  # May be worth to set FQK as default here?
+        self.alpha = alpha
+        self._regularize = regularize
+        self.x_train = None
+        self.k_testtrain = None
+        self.k_train = None
+        self.dual_coeff_ = None
+        self.num_qubits = self._quantum_kernel.num_qubits
+
+    def fit(self, x_train: np.ndarray, y_train: np.ndarray):
+        self.x_train = x_train
+        self.k_train = self._quantum_kernel.evaluate(x=self.x_train)  # set up kernel matrix
+        # check if regularize argument is set and define corresponding method
+        if self._regularize is not None:
+            if self._regularize == "thresholding":
+                self.k_train = regularize_kernel(self.k_train)
+            elif self._regularize == "tikhonov":
+                self.k_train = tikhonov_regularization(self.k_train)
+
+        self.k_train = self.k_train + self.alpha * np.eye(self.k_train.shape[0])
+
+        # solution of KRR problem obtained by solving linear system K*\alpha = y
+        # using Cholesky decomposition for providing numerical stability
+        try:
+            L = scipy.linalg.cholesky(self.k_train, lower=True)
+            self.dual_coeff_ = scipy.linalg.cho_solve((L, True), y_train)
+        except np.linalg.LinAlgError:
+            print("Increase regularization parameter alpha")
+
+        return self
+
+    def predict(self, x_test: np.ndarray) -> np.ndarray:
+        if self.k_train is None:
+            raise ValueError("The fit() method has to be called beforehand.")
+
+        self.k_testtrain = self._quantum_kernel.evaluate(x_test, self.x_train)
+        prediction = np.dot(self.k_testtrain, self.dual_coeff_)
+        return prediction
+
+    # All scikit-learn estimators have get_params and set_params
+    # (cf. https://scikit-learn.org/stable/developers/develop.html)
+    def get_params(self, deep: bool = True):
+        return {
+            "quantum_kernel": self._quantum_kernel,
+            "alpha": self.alpha,
+            "regularize": self._regularize,
+        }
+
+    def set_params(self, **parameters):
+        for parameter, value in parameters.items():
+            setattr(self, parameter, value)
+        return self
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/ml/qsvc.py` & `squlearn-0.2.0/src/squlearn/kernel/ml/qsvc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from ..matrix import KernelMatrixBase
-
-from sklearn.svm import SVC
-
-
-class QSVC(SVC):
-    """
-    Quantum Support Vector Classification
-
-    This class is a wrapper of sklearn.svm.SVC. It uses a quantum kernel matrix
-    to replace the kernel matrix in the sklearn.svm.SVC class.
-
-    Args:
-        quantum_kernel: The quantum kernel matrix to be used in the SVC.
-        **kwargs: Other parameters that are passed to sklearn.svm.SVC.
-
-    Attributes:
-        quantum_kernel: The quantum kernel matrix to be used in the SVC.
-
-    """
-    def __init__(self, *, quantum_kernel: KernelMatrixBase, **kwargs) -> None:
-
-        self.quantum_kernel = quantum_kernel
-        super().__init__(kernel=self.quantum_kernel.evaluate, **kwargs)
-
-    @classmethod
-    def _get_param_names(cls):
-        names = SVC._get_param_names()
-        names.remove("kernel")
-        names.remove("gamma")
-        names.remove("degree")
-        names.remove("coef0")
-        return sorted(names + ["quantum_kernel"])
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+from sklearn.svm import SVC
+
+
+class QSVC(SVC):
+    """
+    Quantum Support Vector Classification
+
+    This class is a wrapper of sklearn.svm.SVC. It uses a quantum kernel matrix
+    to replace the kernel matrix in the sklearn.svm.SVC class.
+
+    Args:
+        quantum_kernel: The quantum kernel matrix to be used in the SVC.
+        **kwargs: Other parameters that are passed to sklearn.svm.SVC.
+
+    Attributes:
+        quantum_kernel: The quantum kernel matrix to be used in the SVC.
+
+    """
+
+    def __init__(self, *, quantum_kernel: KernelMatrixBase, **kwargs) -> None:
+        self.quantum_kernel = quantum_kernel
+        super().__init__(kernel=self.quantum_kernel.evaluate, **kwargs)
+
+    @classmethod
+    def _get_param_names(cls):
+        names = SVC._get_param_names()
+        names.remove("kernel")
+        names.remove("gamma")
+        names.remove("degree")
+        names.remove("coef0")
+        return sorted(names + ["quantum_kernel"])
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/ml/qsvr.py` & `squlearn-0.2.0/src/squlearn/kernel/ml/qsvr.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from ..matrix import KernelMatrixBase
-
-from sklearn.svm import SVR
-
-
-class QSVR(SVR):
-    """
-    Quantum Support Vector Regression
-
-    This class is a wrapper of sklearn.svm.SVR. It uses a quantum kernel matrix
-    to replace the kernel matrix in the sklearn.svm.SVR class.
-
-    Args:
-        quantum_kernel: The quantum kernel matrix to be used in the SVR.
-        **kwargs: Other parameters that are passed to sklearn.svm.SVR.
-
-    Attributes:
-        quantum_kernel: The quantum kernel matrix to be used in the SVR.
-    """
-    def __init__(self, *, quantum_kernel: KernelMatrixBase, **kwargs) -> None:
-
-        self.quantum_kernel = quantum_kernel
-        super().__init__(kernel=self.quantum_kernel.evaluate, **kwargs)
-
-    @classmethod
-    def _get_param_names(cls):
-        names = SVR._get_param_names()
-        names.remove("kernel")
-        names.remove("gamma")
-        names.remove("degree")
-        names.remove("coef0")
-        return sorted(names + ["quantum_kernel"])
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+from sklearn.svm import SVR
+
+
+class QSVR(SVR):
+    """
+    Quantum Support Vector Regression
+
+    This class is a wrapper of sklearn.svm.SVR. It uses a quantum kernel matrix
+    to replace the kernel matrix in the sklearn.svm.SVR class.
+
+    Args:
+        quantum_kernel: The quantum kernel matrix to be used in the SVR.
+        **kwargs: Other parameters that are passed to sklearn.svm.SVR.
+
+    Attributes:
+        quantum_kernel: The quantum kernel matrix to be used in the SVR.
+    """
+
+    def __init__(self, *, quantum_kernel: KernelMatrixBase, **kwargs) -> None:
+        self.quantum_kernel = quantum_kernel
+        super().__init__(kernel=self.quantum_kernel.evaluate, **kwargs)
+
+    @classmethod
+    def _get_param_names(cls):
+        names = SVR._get_param_names()
+        names.remove("kernel")
+        names.remove("gamma")
+        names.remove("degree")
+        names.remove("coef0")
+        return sorted(names + ["quantum_kernel"])
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/optimization/kernel_optimization_base.py` & `squlearn-0.2.0/src/squlearn/kernel/optimization/kernel_optimization_base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import numpy as np
-from typing import Optional, Sequence
-from .kernel_loss_base import KernelLossBase
-from ...optimizers import OptimizerBase
-
-
-class KernelOptimizerBase:
-    def __init__(
-        self,
-        loss: KernelLossBase = None,
-        optimizer: OptimizerBase = None,
-        initial_parameters: Optional[Sequence[float]] = None,
-    ) -> None:
-        self._loss = loss
-        self._optimizer = optimizer
-        self._initial_parameters = initial_parameters
-
-    def run_optimization(self, x: np.ndarray, y: np.ndarray = None):
-        raise NotImplementedError
+import numpy as np
+from typing import Optional, Sequence
+from .kernel_loss_base import KernelLossBase
+from ...optimizers.optimizer_base import OptimizerBase
+
+
+class KernelOptimizerBase:
+    def __init__(
+        self,
+        loss: KernelLossBase = None,
+        optimizer: OptimizerBase = None,
+        initial_parameters: Optional[Sequence[float]] = None,
+    ) -> None:
+        self._loss = loss
+        self._optimizer = optimizer
+        self._initial_parameters = initial_parameters
+
+    def run_optimization(self, x: np.ndarray, y: np.ndarray = None):
+        raise NotImplementedError
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/optimization/kernel_optimizer.py` & `squlearn-0.2.0/src/squlearn/kernel/optimization/kernel_optimizer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
-import numpy as np
-from functools import partial
-from typing import Optional, Sequence
-from .kernel_optimization_base import KernelOptimizerBase
-from .kernel_loss_base import KernelLossBase
-from ..ml.helper_functions import stack_input
-from ...optimizers import OptimizerBase
-
-
-class KernelOptimizer(KernelOptimizerBase):
-    def __init__(
-        self,
-        loss: KernelLossBase = None,
-        optimizer: OptimizerBase = None,
-        initial_parameters: Optional[Sequence[float]] = None,
-    ) -> None:
-        super().__init__(loss, optimizer, initial_parameters)
-        self._quantum_kernel = loss._quantum_kernel
-        self._opt_result = None
-        self._optimier_evals = None
-        self._optimal_value = None
-        self._optimal_point = None
-        self._optimal_parameters = None
-
-    def run_optimization(self, x: np.ndarray, y: np.ndarray = None):
-        if self._quantum_kernel.num_features > 1:
-            x = stack_input(x_vec=x, num_features=self._quantum_kernel.num_features)
-        num_params = self._quantum_kernel.num_parameters
-        if num_params == 0:
-            raise ValueError(
-                "Quantum kernel cannot be fit because there are no training parameters specified."
-            )
-
-        # Perform kernel optimization
-        loss_function = partial(self._loss.compute, data=x, labels=y)
-        opt_result = self._optimizer.minimize(fun=loss_function, x0=self._initial_parameters)
-        self._optimal_value = opt_result.fun
-        self._optimal_point = opt_result.x
-        self._opt_result = opt_result
-
-        return self._opt_result
+import numpy as np
+from functools import partial
+from typing import Optional, Sequence
+from .kernel_optimization_base import KernelOptimizerBase
+from .kernel_loss_base import KernelLossBase
+from ...optimizers.optimizer_base import OptimizerBase
+
+
+class KernelOptimizer(KernelOptimizerBase):
+    def __init__(
+        self,
+        loss: KernelLossBase = None,
+        optimizer: OptimizerBase = None,
+        initial_parameters: Optional[Sequence[float]] = None,
+    ) -> None:
+        super().__init__(loss, optimizer, initial_parameters)
+        self._quantum_kernel = loss._quantum_kernel
+        self._opt_result = None
+        self._optimier_evals = None
+        self._optimal_value = None
+        self._optimal_point = None
+        self._optimal_parameters = None
+
+    def run_optimization(self, x: np.ndarray, y: np.ndarray = None):
+        num_params = self._quantum_kernel.num_parameters
+        if num_params == 0:
+            raise ValueError(
+                "Quantum kernel cannot be fit because there are no training parameters specified."
+            )
+
+        # Perform kernel optimization
+        loss_function = partial(self._loss.compute, data=x, labels=y)
+        opt_result = self._optimizer.minimize(fun=loss_function, x0=self._initial_parameters)
+        self._optimal_value = opt_result.fun
+        self._optimal_point = opt_result.x
+        self._opt_result = opt_result
+
+        return self._opt_result
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/optimization/negative_log_likelihood.py` & `squlearn-0.2.0/src/squlearn/kernel/optimization/negative_log_likelihood.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import scipy
-import numpy as np
-
-from typing import Sequence
-from .kernel_loss_base import KernelLossBase
-from ..matrix import KernelMatrixBase
-
-
-class NLL(KernelLossBase):
-    def __init__(self, quantum_kernel: KernelMatrixBase, sigma=0.0):
-        super().__init__(quantum_kernel)
-        self._sigma = sigma
-
-    # ProjectedQuantumKernel might cause errors since its not present in original KernelLoss
-    def compute(
-        self, parameter_values: Sequence[float], data: np.ndarray, labels: np.ndarray
-    ) -> float:
-        # Bind training parameters
-        self._quantum_kernel.assign_parameters(parameter_values)
-
-        # TODO: implement the equivalent for the pqk here @JSL?
-        # get estimated kernel matrix
-        kmatrix = self._quantum_kernel.evaluate(data)
-        # ensure invertability -> TODO: check this step
-        kmatrix = kmatrix + self._sigma * np.eye(kmatrix.shape[0])
-
-        # Cholesky decomposition since numerically more stable
-        L = scipy.linalg.cholesky(kmatrix, lower=True)
-        S1 = scipy.linalg.solve_triangular(L, labels, lower=True)
-        S2 = scipy.linalg.solve_triangular(L.T, S1, lower=False)
-        neg_log_lh = (
-            np.sum(np.log(np.diagonal(L)))
-            + 0.5 * labels.T @ S2
-            + 0.5 * len(data) * np.log(2.0 * np.pi)
-        )
-        neg_log_lh = neg_log_lh.reshape(-1)
-
-        return neg_log_lh
+import scipy
+import numpy as np
+
+from typing import Sequence
+from .kernel_loss_base import KernelLossBase
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+
+class NLL(KernelLossBase):
+    def __init__(self, quantum_kernel: KernelMatrixBase, sigma=0.0):
+        super().__init__(quantum_kernel)
+        self._sigma = sigma
+
+    # ProjectedQuantumKernel might cause errors since its not present in original KernelLoss
+    def compute(
+        self, parameter_values: Sequence[float], data: np.ndarray, labels: np.ndarray
+    ) -> float:
+        # Bind training parameters
+        self._quantum_kernel.assign_parameters(parameter_values)
+
+        # TODO: implement the equivalent for the pqk here @JSL?
+        # get estimated kernel matrix
+        kmatrix = self._quantum_kernel.evaluate(data)
+        # ensure invertability -> TODO: check this step
+        kmatrix = kmatrix + self._sigma * np.eye(kmatrix.shape[0])
+
+        # Cholesky decomposition since numerically more stable
+        L = scipy.linalg.cholesky(kmatrix, lower=True)
+        S1 = scipy.linalg.solve_triangular(L, labels, lower=True)
+        S2 = scipy.linalg.solve_triangular(L.T, S1, lower=False)
+        neg_log_lh = (
+            np.sum(np.log(np.diagonal(L)))
+            + 0.5 * labels.T @ S2
+            + 0.5 * len(data) * np.log(2.0 * np.pi)
+        )
+        neg_log_lh = neg_log_lh.reshape(-1)
+
+        return neg_log_lh
```

### Comparing `squlearn-0.1.0/src/squlearn/kernel/optimization/target_alignment.py` & `squlearn-0.2.0/src/squlearn/kernel/optimization/target_alignment.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-import numpy as np
-
-from typing import Sequence
-from sklearn.preprocessing._data import _handle_zeros_in_scale
-from .kernel_loss_base import KernelLossBase
-from ..matrix import KernelMatrixBase
-
-
-class TargetAlignment(KernelLossBase):
-    def __init__(self, quantum_kernel: KernelMatrixBase, sigma=0.0):
-        super().__init__(quantum_kernel)
-        self._sigma = sigma
-
-    def compute(
-        self, parameter_values: Sequence[float], data: np.ndarray, labels: np.ndarray
-    ) -> float:
-        # Bind training parameters
-        self._quantum_kernel.assign_parameters(parameter_values)
-        # Training parameters are handeled differently when using QuantumInstance and PQK.
-        # This is checked here. @ JSL?
-
-        # Get estimated kernel matrix
-        kmatrix = self._quantum_kernel.evaluate(data)
-        # regularize ->  TODO: Check if necessary
-        kmatrix = kmatrix + self._sigma * np.eye(kmatrix.shape[0])
-
-        labels_mean = np.mean(labels)
-        labels_std = _handle_zeros_in_scale(np.std(labels, axis=0))
-        labels = (labels - labels_mean) / labels_std
-        kmatrix_opt = labels @ labels.T
-        numerator = np.multiply(kmatrix_opt, kmatrix)
-        denominator = np.multiply(kmatrix, kmatrix)
-        alignment = np.sum(numerator) / (kmatrix.shape[0] * np.sqrt(np.sum(denominator)))
-        return -alignment
+import numpy as np
+
+from typing import Sequence
+from .kernel_loss_base import KernelLossBase
+from ..matrix.kernel_matrix_base import KernelMatrixBase
+
+
+class TargetAlignment(KernelLossBase):
+    def __init__(self, quantum_kernel: KernelMatrixBase, sigma=0.0):
+        super().__init__(quantum_kernel)
+        self._sigma = sigma
+
+    def compute(
+        self,
+        parameter_values: Sequence[float],
+        data: np.ndarray,
+        labels: np.ndarray,
+        rescale_class_labels=True,
+    ) -> float:
+        # Bind training parameters
+        self._quantum_kernel.assign_parameters(parameter_values)
+
+        # Get estimated kernel matrix
+        kmatrix = self._quantum_kernel.evaluate(data)
+        if rescale_class_labels:
+            nplus = np.count_nonzero(np.array(labels) == 1)
+            nminus = len(labels) - nplus
+            _Y = np.array([y / nplus if y == 1 else y / nminus for y in labels])
+        else:
+            _Y = np.array(labels)
+
+        T = np.outer(_Y, _Y)
+        inner_product = np.sum(kmatrix * T)
+        norm = np.sqrt(np.sum(kmatrix * kmatrix) * np.sum(T * T))
+        alignment = inner_product / norm
+        return -alignment
```

### Comparing `squlearn-0.1.0/src/squlearn/optimizers/optimizer_base.py` & `squlearn-0.2.0/src/squlearn/optimizers/optimizer_base.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-"""Optimization methods for QNNs
-"""
-
-# Authors: Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
-# License: ...
-
-import abc
-import numpy as np
-
-
-class OptimizerResult:  # TODO: maybe scipy class?
-    """Class for holding the final result of the optimization"""
-
-    def __init__(self):
-        self.x = None
-        self.nit = 0
-        self.fun = 0.0
-
-
-class OptimizerBase(abc.ABC):
-    """Base class for QNN optimizers."""
-
-    def minimize(
-        self, fun, x0, grad=None, bounds=None  # pylint: disable=invalid-name
-    ) -> OptimizerResult:
-        """Minimize a function"""
-        raise NotImplementedError()
-
-
-class IterativeOptimizerMixin:
-    """Mixin for iterative optimizers."""
-
-    def __init__(self) -> None:
-        self.iteration = 0
-
-    def step(self, **kwargs):
-        """Perform one update step."""
-        raise NotImplementedError()
-
-
-class SGDMixin(IterativeOptimizerMixin, abc.ABC):
-    """Mixin for stochastic gradient descent based optimizers."""
-
-    def step(self, **kwargs):
-        """ "
-
-        Args:
-            x: Current value
-            grad: Precomputed gradient
-
-        Returns:
-            Updated x
-        """
-        if "x" in kwargs:
-            x = kwargs["x"]
-        else:
-            raise TypeError("x argument is missing in step function.")
-        if "grad" in kwargs:
-            grad = kwargs["grad"]
-        else:
-            raise TypeError("grad argument is missing in step function.")
-
-        update = self._get_update(grad)
-        x_return = x + update
-        self.iteration += 1
-        self._update_lr()
-        return x_return
-
-    @abc.abstractmethod
-    def _get_update(self, grad: np.ndarray) -> np.ndarray:
-        raise NotImplementedError()
-
-    @abc.abstractmethod
-    def _update_lr(self) -> None:
-        raise NotImplementedError()
+"""Optimization methods for QNNs
+"""
+
+# Authors: Moritz Willmann <moritz.willmann@ipa.fraunhofer.de>
+# License: ...
+
+import abc
+import numpy as np
+
+
+class OptimizerResult:  # TODO: maybe scipy class?
+    """Class for holding the final result of the optimization"""
+
+    def __init__(self):
+        self.x = None
+        self.nit = 0
+        self.fun = 0.0
+
+
+class OptimizerBase(abc.ABC):
+    """Base class for QNN optimizers."""
+
+    def minimize(
+        self, fun, x0, grad=None, bounds=None  # pylint: disable=invalid-name
+    ) -> OptimizerResult:
+        """Minimize a function"""
+        raise NotImplementedError()
+
+
+class IterativeOptimizerMixin:
+    """Mixin for iterative optimizers."""
+
+    def __init__(self) -> None:
+        self.iteration = 0
+
+    def step(self, **kwargs):
+        """Perform one update step."""
+        raise NotImplementedError()
+
+
+class SGDMixin(IterativeOptimizerMixin, abc.ABC):
+    """Mixin for stochastic gradient descent based optimizers."""
+
+    def step(self, **kwargs):
+        """ "
+
+        Args:
+            x: Current value
+            grad: Precomputed gradient
+
+        Returns:
+            Updated x
+        """
+        if "x" in kwargs:
+            x = kwargs["x"]
+        else:
+            raise TypeError("x argument is missing in step function.")
+        if "grad" in kwargs:
+            grad = kwargs["grad"]
+        else:
+            raise TypeError("grad argument is missing in step function.")
+
+        update = self._get_update(grad)
+        x_return = x + update
+        self.iteration += 1
+        self._update_lr()
+        return x_return
+
+    @abc.abstractmethod
+    def _get_update(self, grad: np.ndarray) -> np.ndarray:
+        raise NotImplementedError()
+
+    @abc.abstractmethod
+    def _update_lr(self) -> None:
+        raise NotImplementedError()
```

### Comparing `squlearn-0.1.0/src/squlearn/optimizers/optimizers_wrapper.py` & `squlearn-0.2.0/src/squlearn/optimizers/optimizers_wrapper.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-""" Various optimization methods that are implemented via wrappers
-"""
-
-import qiskit.algorithms.optimizers as qiskit_optimizers
-from scipy.optimize import minimize
-
-from .optimizer_base import OptimizerBase, OptimizerResult
-
-
-class SLSQP(OptimizerBase):
-    """Wrapper class for scpiy's SLSQP implementation."""
-
-    def __init__(self, options: dict = None):
-        if options is None:
-            options = {}
-
-        self.tol = options.get("tol", 1e-6)
-        if "tol" in options:
-            options.pop("tol")
-        self.options = options
-
-    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
-        scipy_result = minimize(
-            fun, jac=grad, x0=x0, method="SLSQP", options=self.options, bounds=bounds, tol=self.tol
-        )
-        result = OptimizerResult()
-        result.x = scipy_result.x
-        result.nit = scipy_result.nit
-        result.fun = scipy_result.fun
-        return result
-
-
-class LBFGSB(OptimizerBase):
-    """Wrapper class for scpiy's L-BFGS-B implementation."""
-
-    def __init__(self, options: dict = None):
-        if options is None:
-            options = {}
-
-        self.tol = options.get("tol", 1e-6)
-        if "tol" in options:
-            options.pop("tol")
-        self.options = options
-
-    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
-        scipy_result = minimize(
-            fun,
-            jac=grad,
-            x0=x0,
-            method="L-BFGS-B",
-            options=self.options,
-            bounds=bounds,
-            tol=self.tol,
-        )
-        result = OptimizerResult()
-        result.x = scipy_result.x
-        result.nit = scipy_result.nit
-        result.fun = scipy_result.fun
-        return result
-
-
-class SPSA(OptimizerBase):
-    """Wrapper class for qiskit's SPSA implementation."""
-
-    def __init__(self, options: dict = None):
-        if options is None:
-            options = {}
-
-        self.maxiter = options.get("maxiter", 100)
-        self.blocking = options.get("blocking", False)
-        self.allowed_increase = options.get("allowed_increase", None)
-        self.trust_region = options.get("trust_region", False)
-        self.learning_rate = options.get("learning_rate", None)
-        self.perturbation = options.get("perturbation", None)
-        self.last_avg = options.get("last_avg", None)
-        self.resamplings = options.get("resamplings", 1)
-        self.perturbation_dims = options.get("perturbation_dims", None)
-        self.second_order = options.get("second_order", False)
-        self.regularization = options.get("regularization", None)
-        self.hessian_delay = options.get("hessian_delay", 0)
-        self.lse_solver = options.get("lse_solver", None)
-        self.initial_hessian = options.get("initial_hessian", None)
-
-    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
-        spsa = qiskit_optimizers.SPSA(
-            maxiter=self.maxiter,
-            blocking=self.blocking,
-            allowed_increase=self.allowed_increase,
-            trust_region=self.trust_region,
-            learning_rate=self.learning_rate,
-            perturbation=self.perturbation,
-            last_avg=self.last_avg,
-            resamplings=self.resamplings,
-            perturbation_dims=self.perturbation_dims,
-            second_order=self.second_order,
-            regularization=self.regularization,
-            hessian_delay=self.hessian_delay,
-            lse_solver=self.lse_solver,
-            initial_hessian=self.initial_hessian,
-        )
-
-        result_qiskit = spsa.minimize(fun=fun, x0=x0, jac=grad, bounds=bounds)
-
-        result = OptimizerResult()
-        result.x = result_qiskit.x
-        result.nit = result_qiskit.nit
-        result.fun = result_qiskit.fun
-        return result
+""" Various optimization methods that are implemented via wrappers
+"""
+
+import qiskit.algorithms.optimizers as qiskit_optimizers
+from scipy.optimize import minimize
+
+from .optimizer_base import OptimizerBase, OptimizerResult
+
+
+class SLSQP(OptimizerBase):
+    """Wrapper class for scpiy's SLSQP implementation."""
+
+    def __init__(self, options: dict = None):
+        if options is None:
+            options = {}
+
+        self.tol = options.get("tol", 1e-6)
+        if "tol" in options:
+            options.pop("tol")
+        self.options = options
+
+    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
+        scipy_result = minimize(
+            fun, jac=grad, x0=x0, method="SLSQP", options=self.options, bounds=bounds, tol=self.tol
+        )
+        result = OptimizerResult()
+        result.x = scipy_result.x
+        result.nit = scipy_result.nit
+        result.fun = scipy_result.fun
+        return result
+
+
+class LBFGSB(OptimizerBase):
+    """Wrapper class for scpiy's L-BFGS-B implementation."""
+
+    def __init__(self, options: dict = None):
+        if options is None:
+            options = {}
+
+        self.tol = options.get("tol", 1e-6)
+        if "tol" in options:
+            options.pop("tol")
+        self.options = options
+
+    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
+        scipy_result = minimize(
+            fun,
+            jac=grad,
+            x0=x0,
+            method="L-BFGS-B",
+            options=self.options,
+            bounds=bounds,
+            tol=self.tol,
+        )
+        result = OptimizerResult()
+        result.x = scipy_result.x
+        result.nit = scipy_result.nit
+        result.fun = scipy_result.fun
+        return result
+
+
+class SPSA(OptimizerBase):
+    """Wrapper class for qiskit's SPSA implementation."""
+
+    def __init__(self, options: dict = None):
+        if options is None:
+            options = {}
+
+        self.maxiter = options.get("maxiter", 100)
+        self.blocking = options.get("blocking", False)
+        self.allowed_increase = options.get("allowed_increase", None)
+        self.trust_region = options.get("trust_region", False)
+        self.learning_rate = options.get("learning_rate", None)
+        self.perturbation = options.get("perturbation", None)
+        self.last_avg = options.get("last_avg", None)
+        self.resamplings = options.get("resamplings", 1)
+        self.perturbation_dims = options.get("perturbation_dims", None)
+        self.second_order = options.get("second_order", False)
+        self.regularization = options.get("regularization", None)
+        self.hessian_delay = options.get("hessian_delay", 0)
+        self.lse_solver = options.get("lse_solver", None)
+        self.initial_hessian = options.get("initial_hessian", None)
+
+    def minimize(self, fun, x0, grad=None, bounds=None) -> OptimizerResult:
+        spsa = qiskit_optimizers.SPSA(
+            maxiter=self.maxiter,
+            blocking=self.blocking,
+            allowed_increase=self.allowed_increase,
+            trust_region=self.trust_region,
+            learning_rate=self.learning_rate,
+            perturbation=self.perturbation,
+            last_avg=self.last_avg,
+            resamplings=self.resamplings,
+            perturbation_dims=self.perturbation_dims,
+            second_order=self.second_order,
+            regularization=self.regularization,
+            hessian_delay=self.hessian_delay,
+            lse_solver=self.lse_solver,
+            initial_hessian=self.initial_hessian,
+        )
+
+        result_qiskit = spsa.minimize(fun=fun, x0=x0, jac=grad, bounds=bounds)
+
+        result = OptimizerResult()
+        result.x = result_qiskit.x
+        result.nit = result_qiskit.nit
+        result.fun = result_qiskit.fun
+        return result
```

### Comparing `squlearn-0.1.0/src/squlearn/qnn/barren_plateau_analysis.py` & `squlearn-0.2.0/src/squlearn/qnn/barren_plateau_analysis.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,242 +1,242 @@
-import numpy as np
-from sklearn.linear_model import LinearRegression
-
-from .qnn import QNN
-
-from ..util.data_preprocessing import adjust_input
-
-
-def calc_var_dg(
-    qnn,
-    x,
-    param_op,
-    n_sample=100,
-    p_lim=None,
-    p_val=None,
-    p_index=None,
-    verbose=1,
-    seed=0,
-):
-    """
-    Calculates the variance and the mean of the gradient of the given qnn.
-
-    Args:
-        qnn : QNN object from which the variance of the gradient is calculated
-        x : Single value or array of the x values of the QNN
-        param_op : Values of the cost-operator
-        n_sample = 100 : Number of samples considered for the variance computation of the gradient
-        p_lim = None : Limits of the unified sampling of parameters for the variance calculation
-        p_val = None : Array containing the parameters for sampling.
-                       If equal None, the parameters are chosen randomly (default).
-        p_index = None : Array of indices of the parameters chosen for the derivative.
-                         If equal None (default), the parameters are chosen randomly
-        verbose = 1 : Verbosity of the method.
-        seed = 0: Random seed the random operations.
-
-    Returns:
-        Variance of the gradient values
-        Mean value of the absolute values of the gradient
-    """
-
-    seed_backup = np.random.get_state()
-    np.random.seed(seed)
-
-    # Set-up default limits
-    if p_lim is None:
-        p_lim = (-np.pi, np.pi)
-
-    # Process p-values
-    if p_val is not None:
-        p_val, multi = adjust_input(p_val, qnn.num_parameters)
-        if not isinstance(p_val, np.ndarray):
-            p = np.array(p_val)
-        else:
-            p = p_val
-        if p.shape[1] != qnn.num_parameters:
-            raise ValueError("Wrong size of the input p_val")
-    else:
-        p = np.random.uniform(low=p_lim[0], high=p_lim[1], size=(n_sample, qnn.num_parameters))
-
-    if p_index is None:
-        p_index = np.random.randint(0, qnn.num_parameters, size=n_sample)
-
-    np.random.set_state(seed_backup)
-
-    # Radom sampling of the gradient derivatives
-    grad_val = []
-    for iter in range(p.shape[0]):
-        grad_val.append(
-            qnn.evaluate_diff_tuple((qnn.parameters[p_index[iter]],), x, p[iter], param_op)
-        )
-
-    # Returns variance and absolute mean value of all sampled gradient entries
-    np_array = np.array(grad_val).flatten()
-    return np.var(np_array), np.mean(np.abs(np_array))
-
-
-def get_barren_slope(pqc_func, cost_op_func, x, QI, num_qubits, layer_fac=5, n_sample=100):
-    """
-    Calculates the variance of the gradient for different number of qubits.
-    Returns a linear regression model to the data
-
-    Args:
-        pqc_func : function which returns the initialized pqc class for a given number of qubits and layers
-                   pqc_func(number_of_qubits, number_of_layers)
-        cost_op_func : function which returns the initialized cost_op class for a given number of qubits
-                       cost_op_func(number_of_qubits)
-        x : single value or array of the x values
-        QI : Quantum Instance for evaluating the quantum circuits
-        num_qubits : Either a list containing the considered qubits or
-                     an integer value that triggers a list of [2,...,num_qubits] qubits
-        layer_fac = 5 : (optional) Number of layer is  given by number of qubits times layer_fac
-        n_sample = 100 : (optional) Number of samples considered for the variance computation of the gradient
-
-    Returns:
-        Model containing the linear regression (based on sklearn.linear_model.LinearRegression)
-        Numpy array with the variance values
-    """
-
-    if isinstance(num_qubits, int):
-        num_qubits_ = np.arange(2, num_qubits + 1)
-    else:
-        num_qubits_ = num_qubits
-
-    var = []
-    mean = []
-
-    for iqubits in num_qubits_:
-        number_of_layers = layer_fac * iqubits
-        pqc_ = pqc_func(iqubits, number_of_layers)
-        cost_op_ = cost_op_func(iqubits)
-        qnn = QNN(pqc_, cost_op_, QI)
-        mean_val, var_val = calc_var_dg(
-            qnn,
-            x=x,
-            param_op=np.ones(cost_op_.get_number_of_parameters()),
-            n_sample=n_sample,
-        )
-        var.append(var_val)
-        mean.append(mean_val)
-
-    model = LinearRegression()
-    model.fit(np.array(num_qubits_).reshape((-1, 1)), np.log(np.array(var)))
-    model.x_val = np.array(num_qubits_).reshape((-1, 1))
-    model.y_val = np.log(np.array(var))
-    return model, np.array(var)
-
-
-def get_barren_slop_from_model(model):
-    """
-    Returns the slop of the linear regression of the barren plateau fit
-
-    Args:
-        model : linear regression model created by get_barren_slope
-
-    Returns:
-        slop of the linear regression
-    """
-    return model.coef_[0]
-
-
-def get_barren_plot_from_model(model, plt):
-    """
-    Plots the regression output and the measured numbers into a semilogarithmic plot-
-
-    Args:
-        model : linear regression model created by get_barren_slope
-        plt : matplotplib.pyplot object
-
-    Returns:
-        matplotlib handles to the two plots
-    """
-    y = np.exp(model.predict(model.x_val))
-    handle = []
-    handle.append(plt.semilogy(model.x_val, y))
-    handle.append(plt.semilogy(model.x_val, np.exp(model.y_val)))
-    return handle
-
-
-def get_barren_layer(pqc_func, cost_op_func, x, QI, num_qubits, num_layers, n_sample=100):
-    """
-    Calculate the variance of the gradient for different number of qubits and layers.
-    Can be used to create a plot for visualizing the plateauing for specific number of layers.
-
-    Args:
-        pqc_func : function which returns the initialized pqc class for a given number of qubits and layers
-                   pqc_func(number_of_qubits, number_of_layers)
-        cost_op_func : function which returns the initialized cost_op class for a given number of qubits
-                       cost_op_func(number_of_qubits)
-        x : single value or array of the x values
-        QI : Quantum Instance for evaluating the quantum circuits
-        num_qubits : Either a list containing the considered qubits or
-                     an integer value that triggers a list of [2,...,num_qubits] qubits
-        num_layers : Either a list containing the considered qubits or
-                     an integer value that triggers a list of [2,...,num_qubits] qubits
-        n_sample = 100 : (optional) Number of samples considered for the variance computation of the gradient
-
-    Returns:
-        Returns two dictionaries with the variance and the mean absolute value for the given layers
-    """
-
-    if isinstance(num_qubits, int):
-        num_qubits_ = np.arange(2, num_qubits + 1)
-    else:
-        num_qubits_ = num_qubits
-
-    if isinstance(num_layers, int):
-        num_layers_ = np.arange(1, num_layers + 1, 5)
-    else:
-        num_layers_ = num_layers
-
-    var = {}
-    mean = {}
-
-    for iqubits in num_qubits_:
-        qubit_var = []
-        qubit_mean = []
-        for ilayers in num_layers_:
-            number_of_layers = ilayers
-            pqc_ = pqc_func(iqubits, number_of_layers)
-            cost_op_ = cost_op_func(iqubits)
-            qnn = QNN(pqc_, cost_op_, QI)
-            mean_val, var_val = calc_var_dg(
-                qnn,
-                x=x,
-                param_op=np.ones(cost_op_.get_number_of_parameters()),
-                n_sample=n_sample,
-            )
-            qubit_var.append(var_val)
-            qubit_mean.append(mean_val)
-        var[iqubits] = qubit_var
-        mean[iqubits] = qubit_mean
-
-    return var, mean
-
-
-def get_barren_layer_plot(var, num_layers, plt):
-    """
-    Creates a barren plateau visualization with the
-    number of layers on the X-axis. Returns a semilogarithmic
-    plot of the variance of the gradient (see get_barren_layer).
-
-    Args:
-        var : dictionary containing the variance connecting qubits
-            and the variance for the layers
-        num_layers : Either a list containing the considered
-            number of layers or an integer value that triggers a list of
-            [1,5,num_layers] qubits
-        plt : matplotplib.pyplot object
-
-    Returns:
-        Handles of the different curves
-    """
-
-    if isinstance(num_layers, int):
-        num_layers_ = np.arange(1, num_layers + 1, 5)
-    else:
-        num_layers_ = num_layers
-
-    handles = {}
-    for i in var.keys():
-        handles[i] = plt.semilogy(num_layers_, var[i])
-    return handles
+import numpy as np
+from sklearn.linear_model import LinearRegression
+
+from .qnn import QNN
+
+from ..util.data_preprocessing import adjust_input
+
+
+def calc_var_dg(
+    qnn,
+    x,
+    param_op,
+    n_sample=100,
+    p_lim=None,
+    p_val=None,
+    p_index=None,
+    verbose=1,
+    seed=0,
+):
+    """
+    Calculates the variance and the mean of the gradient of the given qnn.
+
+    Args:
+        qnn : QNN object from which the variance of the gradient is calculated
+        x : Single value or array of the x values of the QNN
+        param_op : Values of the cost-operator
+        n_sample = 100 : Number of samples considered for the variance computation of the gradient
+        p_lim = None : Limits of the unified sampling of parameters for the variance calculation
+        p_val = None : Array containing the parameters for sampling.
+                       If equal None, the parameters are chosen randomly (default).
+        p_index = None : Array of indices of the parameters chosen for the derivative.
+                         If equal None (default), the parameters are chosen randomly
+        verbose = 1 : Verbosity of the method.
+        seed = 0: Random seed the random operations.
+
+    Returns:
+        Variance of the gradient values
+        Mean value of the absolute values of the gradient
+    """
+
+    seed_backup = np.random.get_state()
+    np.random.seed(seed)
+
+    # Set-up default limits
+    if p_lim is None:
+        p_lim = (-np.pi, np.pi)
+
+    # Process p-values
+    if p_val is not None:
+        p_val, multi = adjust_input(p_val, qnn.num_parameters)
+        if not isinstance(p_val, np.ndarray):
+            p = np.array(p_val)
+        else:
+            p = p_val
+        if p.shape[1] != qnn.num_parameters:
+            raise ValueError("Wrong size of the input p_val")
+    else:
+        p = np.random.uniform(low=p_lim[0], high=p_lim[1], size=(n_sample, qnn.num_parameters))
+
+    if p_index is None:
+        p_index = np.random.randint(0, qnn.num_parameters, size=n_sample)
+
+    np.random.set_state(seed_backup)
+
+    # Radom sampling of the gradient derivatives
+    grad_val = []
+    for iter in range(p.shape[0]):
+        grad_val.append(
+            qnn.evaluate_diff_tuple((qnn.parameters[p_index[iter]],), x, p[iter], param_op)
+        )
+
+    # Returns variance and absolute mean value of all sampled gradient entries
+    np_array = np.array(grad_val).flatten()
+    return np.var(np_array), np.mean(np.abs(np_array))
+
+
+def get_barren_slope(pqc_func, cost_op_func, x, QI, num_qubits, layer_fac=5, n_sample=100):
+    """
+    Calculates the variance of the gradient for different number of qubits.
+    Returns a linear regression model to the data
+
+    Args:
+        pqc_func : function which returns the initialized pqc class for a given number of qubits and layers
+                   pqc_func(number_of_qubits, number_of_layers)
+        cost_op_func : function which returns the initialized cost_op class for a given number of qubits
+                       cost_op_func(number_of_qubits)
+        x : single value or array of the x values
+        QI : Quantum Instance for evaluating the quantum circuits
+        num_qubits : Either a list containing the considered qubits or
+                     an integer value that triggers a list of [2,...,num_qubits] qubits
+        layer_fac = 5 : (optional) Number of layer is  given by number of qubits times layer_fac
+        n_sample = 100 : (optional) Number of samples considered for the variance computation of the gradient
+
+    Returns:
+        Model containing the linear regression (based on sklearn.linear_model.LinearRegression)
+        Numpy array with the variance values
+    """
+
+    if isinstance(num_qubits, int):
+        num_qubits_ = np.arange(2, num_qubits + 1)
+    else:
+        num_qubits_ = num_qubits
+
+    var = []
+    mean = []
+
+    for iqubits in num_qubits_:
+        number_of_layers = layer_fac * iqubits
+        pqc_ = pqc_func(iqubits, number_of_layers)
+        cost_op_ = cost_op_func(iqubits)
+        qnn = QNN(pqc_, cost_op_, QI)
+        mean_val, var_val = calc_var_dg(
+            qnn,
+            x=x,
+            param_op=np.ones(cost_op_.get_number_of_parameters()),
+            n_sample=n_sample,
+        )
+        var.append(var_val)
+        mean.append(mean_val)
+
+    model = LinearRegression()
+    model.fit(np.array(num_qubits_).reshape((-1, 1)), np.log(np.array(var)))
+    model.x_val = np.array(num_qubits_).reshape((-1, 1))
+    model.y_val = np.log(np.array(var))
+    return model, np.array(var)
+
+
+def get_barren_slop_from_model(model):
+    """
+    Returns the slop of the linear regression of the barren plateau fit
+
+    Args:
+        model : linear regression model created by get_barren_slope
+
+    Returns:
+        slop of the linear regression
+    """
+    return model.coef_[0]
+
+
+def get_barren_plot_from_model(model, plt):
+    """
+    Plots the regression output and the measured numbers into a semilogarithmic plot-
+
+    Args:
+        model : linear regression model created by get_barren_slope
+        plt : matplotplib.pyplot object
+
+    Returns:
+        matplotlib handles to the two plots
+    """
+    y = np.exp(model.predict(model.x_val))
+    handle = []
+    handle.append(plt.semilogy(model.x_val, y))
+    handle.append(plt.semilogy(model.x_val, np.exp(model.y_val)))
+    return handle
+
+
+def get_barren_layer(pqc_func, cost_op_func, x, QI, num_qubits, num_layers, n_sample=100):
+    """
+    Calculate the variance of the gradient for different number of qubits and layers.
+    Can be used to create a plot for visualizing the plateauing for specific number of layers.
+
+    Args:
+        pqc_func : function which returns the initialized pqc class for a given number of qubits and layers
+                   pqc_func(number_of_qubits, number_of_layers)
+        cost_op_func : function which returns the initialized cost_op class for a given number of qubits
+                       cost_op_func(number_of_qubits)
+        x : single value or array of the x values
+        QI : Quantum Instance for evaluating the quantum circuits
+        num_qubits : Either a list containing the considered qubits or
+                     an integer value that triggers a list of [2,...,num_qubits] qubits
+        num_layers : Either a list containing the considered qubits or
+                     an integer value that triggers a list of [2,...,num_qubits] qubits
+        n_sample = 100 : (optional) Number of samples considered for the variance computation of the gradient
+
+    Returns:
+        Returns two dictionaries with the variance and the mean absolute value for the given layers
+    """
+
+    if isinstance(num_qubits, int):
+        num_qubits_ = np.arange(2, num_qubits + 1)
+    else:
+        num_qubits_ = num_qubits
+
+    if isinstance(num_layers, int):
+        num_layers_ = np.arange(1, num_layers + 1, 5)
+    else:
+        num_layers_ = num_layers
+
+    var = {}
+    mean = {}
+
+    for iqubits in num_qubits_:
+        qubit_var = []
+        qubit_mean = []
+        for ilayers in num_layers_:
+            number_of_layers = ilayers
+            pqc_ = pqc_func(iqubits, number_of_layers)
+            cost_op_ = cost_op_func(iqubits)
+            qnn = QNN(pqc_, cost_op_, QI)
+            mean_val, var_val = calc_var_dg(
+                qnn,
+                x=x,
+                param_op=np.ones(cost_op_.get_number_of_parameters()),
+                n_sample=n_sample,
+            )
+            qubit_var.append(var_val)
+            qubit_mean.append(mean_val)
+        var[iqubits] = qubit_var
+        mean[iqubits] = qubit_mean
+
+    return var, mean
+
+
+def get_barren_layer_plot(var, num_layers, plt):
+    """
+    Creates a barren plateau visualization with the
+    number of layers on the X-axis. Returns a semilogarithmic
+    plot of the variance of the gradient (see get_barren_layer).
+
+    Args:
+        var : dictionary containing the variance connecting qubits
+            and the variance for the layers
+        num_layers : Either a list containing the considered
+            number of layers or an integer value that triggers a list of
+            [1,5,num_layers] qubits
+        plt : matplotplib.pyplot object
+
+    Returns:
+        Handles of the different curves
+    """
+
+    if isinstance(num_layers, int):
+        num_layers_ = np.arange(1, num_layers + 1, 5)
+    else:
+        num_layers_ = num_layers
+
+    handles = {}
+    for i in var.keys():
+        handles[i] = plt.semilogy(num_layers_, var[i])
+    return handles
```

### Comparing `squlearn-0.1.0/src/squlearn/qnn/qnn.py` & `squlearn-0.2.0/src/squlearn/qnn/qnn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,1057 +1,1056 @@
-from qiskit.circuit import ParameterVector, ParameterExpression
-from qiskit.circuit.parametervector import ParameterVectorElement
-from qiskit.opflow import OperatorBase, CircuitStateFn, OperatorStateFn
-from qiskit.opflow import ListOp, SummedOp, ComposedOp, TensoredOp
-from qiskit.opflow import Zero, One
-from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
-from qiskit.opflow.expectations import PauliExpectation
-from qiskit.utils import QuantumInstance
-
-from typing import Union
-import numpy as np
-
-from ..expectation_operator import (
-    ExpectationOperatorBase,
-    ExpectationOperatorDerivatives,
-)
-from ..feature_map import (
-    FeatureMapBase,
-    FeatureMapDerivatives,
-    measure_feature_map_derivative,
-    TranspiledFeatureMap,
-)
-
-from ..util.data_preprocessing import adjust_input
-
-from ..util import Executor
-
-
-class expec:
-    """Data structure that holds the set-up of derivative of the expectation value.
-
-    Args:
-        wavefunction (Union[str, tuple, ParameterVectorElement]): Describes the wavefuction or its
-            derivative. If tuple or ParameterVectorElement the differentiation with respect to the
-            parameters in the tuple or with respect to the ParameterVectorElement is considered
-        operator (str): String for the expectation value operator (O, OO, dop, dopdop, var).
-        label (str): Label that is used for displaying or in the value dict of the QNN class.
-
-    """
-
-    def __init__(
-        self,
-        wavefunction: Union[str, tuple, ParameterVectorElement],
-        operator: str,
-        label: str = "",
-    ):
-        self.wavefunction = wavefunction
-        self.operator = operator
-        self.label = label
-
-    def __var_to_str(self, val: Union[str, tuple, ParameterExpression, ParameterVector]) -> str:
-        """Converter for variables to string.
-
-        Args:
-            val (Union[str, tuple, ParameterExpression, ParameterVector]): Input that is converted
-                to string
-
-        Returns:
-            String that contains the converted val variable
-
-        """
-        if isinstance(val, ParameterExpression):
-            out_str = str(val.name)
-        elif isinstance(val, ParameterVector):
-            out_str = str(val.name)
-        elif isinstance(val, tuple):
-            out_str = "("
-            for x in val:
-                out_str += self.__var_to_str(x) + ","
-            out_str += ")"
-        elif isinstance(val, str):
-            out_str = val
-        else:
-            out_str = str(val)
-        return out_str
-
-    def __repr__(self) -> str:
-        """Build-in string conversion for expec class."""
-        return self.__str__()
-
-    def __str__(self) -> str:
-        """Build-in string conversion for expec class."""
-        return (
-            "expec("
-            + self.__var_to_str(self.wavefunction)
-            + ","
-            + self.__var_to_str(self.operator)
-            + ","
-            + self.__var_to_str(self.label)
-            + ")"
-        )
-
-    def __len__(self) -> int:
-        """Build-in length of expec class (return 1)."""
-        return 1
-
-    def __eq__(self, other) -> bool:
-        """Build-in comparison of two expec class objects."""
-        return (
-            isinstance(other, self.__class__)
-            and self.wavefunction == other.wavefunction
-            and self.operator == other.operator
-        )
-
-    def __hash__(self) -> int:
-        """Build-in hash function for expec class."""
-        return hash((self.wavefunction, self.operator))
-
-    @classmethod
-    def from_string(cls, val: str):
-        """Converts an input string to the expec data structure.
-
-        Args:
-            String that defines the expectation value derivative
-
-        Returns:
-            Associated expec object
-
-        """
-
-        if isinstance(val, str):
-            if val == "f":
-                return cls("I", "O", "f")
-            elif val == "dfdx":
-                return cls("dx", "O", "dfdx")
-            elif val == "dfdxdx":
-                return cls("dxdx", "O", "dfdxdx")
-            elif val == "laplace":
-                return cls("laplace", "O", "laplace")
-            elif val == "laplace_dp":
-                return cls("laplace_dp", "O", "laplace_dp")
-            elif val == "laplace_dop":
-                return cls("laplace", "dop", "laplace_dop")
-            elif val == "dfdp":
-                return cls("dp", "O", "dfdp")
-            elif val == "dfdpdp":
-                return cls("dpdp", "O", "dfdpdp")
-            elif val == "dfdopdp":
-                return cls("dp", "dop", "dfdop")
-            elif val == "dfdop":
-                return cls("I", "dop", "dfdop")
-            elif val == "dfdopdop":
-                return cls("I", "dopdop", "dfdop")
-            elif val == "dfdpdx":
-                return cls("dpdx", "O", "dfdpdx")
-            elif val == "dfdopdx":
-                return cls("dx", "dop", "dfdopdx")
-            elif val == "dfdopdxdx":
-                return cls("dxdx", "dop", "dfdopdxdx")
-            elif val == "fcc":
-                return cls("I", "OO", "fcc")
-            elif val == "dfccdx":
-                return cls("dx", "OO", "dfccdx")
-            elif val == "dfccdxdx":
-                return cls("dxdx", "OO", "dfccdxdx")
-            elif val == "dfccdp":
-                return cls("dp", "OO", "dfccdp")
-            elif val == "dfccdpdp":
-                return cls("dpdp", "OO", "dfccdpdp")
-            elif val == "dfccdopdx":
-                return cls("dx", "OOdop", "dfccdpdp")
-            elif val == "dfccdop":
-                return cls("I", "OOdop", "dfccdop")
-            elif val == "dfccdopdop":
-                return cls("I", "OOdopdop", "dfccdopdop")
-            elif val in ("var", "varf"):
-                return cls("I", "var", val)
-            elif val in ("dvardx", "dvarfdx"):
-                return cls("dx", "var", val)
-            elif val in ("dvardp", "dvarfdp"):
-                return cls("dp", "var", val)
-            elif val in ("dvardop", "dvarfdop"):
-                return cls("I", "dvardop", val)
-            elif val == "fischer":
-                return cls("I", "fischer", val)
-            else:
-                raise ValueError("Unknown input string:", val)
-        else:
-            raise TypeError("String expected, found type:", type(val))
-
-    @classmethod
-    def from_tuple(cls, val: tuple, operator: str = "O"):
-        """Creates an expec object from an input tuple
-
-        Args:
-            val (tuple): Tuple for the differentiation of the wavefunction.
-            operator (str): String for the operator, default='O'.
-
-        Returns
-            Associated expec object
-        """
-        return cls(val, operator, val)
-
-    @classmethod
-    def from_parameter(cls, val: ParameterVectorElement, operator: str = "O"):
-        """Creates an expec object from an inputted parameter
-
-        Args:
-            val (ParameterVectorElement): Parameter that is used in the differentiation.
-            operator (str): String for the operator, default='O'.
-
-        Returns
-            Associated expec object
-        """
-        return cls((val,), operator, (val,))
-
-    @classmethod
-    def from_variable(cls, val):
-        """Creates an expec object from an inputted value
-
-        Args:
-            val (Union[expec,str,tuple,ParameterVectorElement]): value that defines the derivative
-
-        Returns
-            Associated expec object
-        """
-
-        if isinstance(val, expec):
-            return val
-        elif isinstance(val, str):
-            return cls.from_string(val)
-        elif isinstance(val, tuple):
-            return cls.from_tuple(val)
-        elif isinstance(val, ParameterVectorElement):
-            return cls.from_parameter(val)
-        else:
-            raise TypeError("Unsupported type:", type(val))
-
-
-class QNN:
-    """A class for working with QNNs and its derivatives
-
-    Args:
-        pqc (FeatureMapBase) : parameterized quantum circuit in feature map format
-        operator (Union[ExpectationOperatorBase,list]): Operator that are used in the expectation value
-            of the QNN. Can be a list for multiple outputs.
-        executor (Executor) : Executor that is used for the evaluation of the QNN
-        opflow_caching : Caching of the opflow expressions (default = True recommended)
-        result_caching : Caching of the result for each x,param,param_op combination
-            (default = True)
-    """
-
-    def __init__(
-        self,
-        pqc: FeatureMapBase,
-        operator: Union[ExpectationOperatorBase, list],
-        executor: Executor,
-        opflow_caching=True,
-        result_caching=True,
-    ) -> None:
-        # Potential TODO: move executor into extra util class
-        # Executer set-up
-        self.executor = executor
-        self.backend = self.executor.backend
-
-        # Storing the input data # TODO: custom transpilation function
-        self.pqc = TranspiledFeatureMap(pqc, self.backend)
-        self.operator = operator
-        num_qubits_operator = 0
-        if isinstance(self.operator, list):
-            for i in range(len(self.operator)):
-                self.operator[i].set_map(self.pqc.qubit_map, self.pqc.num_all_qubits)
-                num_qubits_operator = max(num_qubits_operator, self.operator[i].num_qubits)
-        else:
-            self.operator.set_map(self.pqc.qubit_map, self.pqc.num_all_qubits)
-            num_qubits_operator = self.operator.num_qubits
-
-        self.operator_derivatives = ExpectationOperatorDerivatives(self.operator, opflow_caching)
-        self.pqc_derivatives = FeatureMapDerivatives(self.pqc, opflow_caching)
-
-        if self.pqc.num_qubits != num_qubits_operator:
-            raise ValueError("Number of Qubits are not the same!")
-        else:
-            self._num_qubits = self.pqc.num_qubits
-
-        if self.executor.get_opflow_executor() in ("sampler", "quantum_instance"):
-            # For Quantum Instance or the Sampler primitive, X and Y Pauli matrices have to be treated extra
-            # This is very inefficient!
-            operator_string = str(self.operator)
-            if "X" in operator_string or "Y" in operator_string:
-                self.split_paulis = True
-                print(
-                    "The expectation operator includes X and Y gates, consider switching"
-                    + " to the Estimator primitive for a faster performance!"
-                )
-            else:
-                self.split_paulis = False
-        else:
-            self.split_paulis = False
-
-        # Set-up shots from backend
-        self._inital_shots = self.executor.get_shots()
-
-        # Initialize result cache
-        self._result_caching = result_caching
-        self.result_container = {}
-
-    def set_shots(self, num_shots: int) -> None:
-        """Sets the number shots for the next evaluations.
-
-        Args:
-            num_shots (int): Number of shots that are set
-        """
-
-        self.executor.set_shots(num_shots)
-
-    def get_shots(self) -> int:
-        """Getter for the number of shots.
-
-        Returns:
-            Returns the number of shots that are used for the current evaluation."""
-        return self.executor.get_shots()
-
-    def reset_shots(self) -> None:
-        """Function for resetting the number of shots to the inital ones"""
-        self.executor.reset_shots()
-
-    @property
-    def num_qubits(self) -> int:
-        """Return the number of qubits of the QNN"""
-        return self._num_qubits
-
-    @property
-    def num_features(self) -> int:
-        """Return the dimension of the features of the PQC"""
-        return self.pqc_derivatives.num_features
-
-    @property
-    def num_parameters(self) -> int:
-        """Return the number of trainable parameters of the PQC"""
-        return self.pqc_derivatives.num_parameters
-
-    @property
-    def num_operator(self) -> int:
-        """Return the number outputs"""
-        return self.operator_derivatives.num_operators
-
-    @property
-    def num_parameters_operator(self) -> int:
-        """Return the number of trainable parameters of the expectation value operator"""
-        return self.operator_derivatives.num_parameters
-
-    @property
-    def multiple_output(self) -> bool:
-        """Return true if multiple outputs are used"""
-        return self.operator_derivatives.multiple_output
-
-    @property
-    def parameters(self):
-        """Return the parameter vector of the PQC."""
-        return self.pqc_derivatives.p
-
-    @property
-    def features(self):
-        """Return the feature vector of the PQC."""
-        return self.pqc_derivatives.x
-
-    @property
-    def parameters_operator(self):
-        """Return the parameter vector of the cost operator."""
-        return self.operator_derivatives.parameters
-
-    def get_opflow_from_string(self, input_string: str):
-        """Return the opflow expression of the given PQC
-
-        Args:
-            input_string (str): String from which the opflow is obtained.
-
-        Returns:
-            Opflow structure created from the string.
-        """
-        return self.get_opflow_from_expec(expec.from_string(input_string))
-
-    def get_opflow_from_expec(self, input_expec: expec):
-        """Returns the opflow expression for the given expec object.
-
-        Args:
-            input_expec (expec): Expec pbject from which the opflow is obtained
-
-        Returns:
-            Opflow structure created from the expec object.
-        """
-        return measure_feature_map_derivative(
-            self.pqc_derivatives.get_derivate(input_expec.wavefunction),
-            self.operator_derivatives.get_derivate(input_expec.operator),
-        )
-
-    def evaluate_diff_tuple(
-        self,
-        diff_tuple,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluate the given tuple of derivatives of the PQC.
-
-        Args:
-            diff_tuple: Tuple with parameters used in the differentiation
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Differentiated values of the QNN
-        """
-        return self.evaluate((diff_tuple,), x, param, param_op)[diff_tuple]
-
-    def evaluate_from_string(
-        self,
-        input_string: str,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluate the given PQC from an input string
-
-        Args:
-            input_string (str): Input string that determines the evaluated value(s)
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Values from the QNN defined by the string
-        """
-        return self.evaluate(input_string, x, param, param_op)[input_string]
-
-    def evaluate_f(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Values from the QNN
-        """
-        return self.evaluate_from_string("f", x, param, param_op)
-
-    def evaluate_dfdx(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d/dx of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d/dx of the the QNN
-        """
-        return self.evaluate_from_string("dfdx", x, param, param_op)
-
-    def evaluate_dfdxdx(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d^2/dxdx of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d^2/dxdx of the the QNN
-        """
-        return self.evaluate_from_string("dfdxdx", x, param, param_op)
-
-    def evaluate_laplace(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates laplace(x) of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated laplace(x) of the the QNN
-        """
-        return self.evaluate_from_string("laplace", x, param, param_op)
-
-    def evaluate_laplace_dp(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d laplace(x)/dp of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d laplace(x)/dp of the the QNN
-        """
-        return self.evaluate_from_string("laplace_dp", x, param, param_op)
-
-    def evaluate_laplace_dop(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d laplace(x)/dop of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d laplace(x)/dop of the the QNN
-        """
-        return self.evaluate_from_string("laplace_dop", x, param, param_op)
-
-    def evaluate_dfdp(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d/dp of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d/dp of the the QNN
-        """
-        return self.evaluate_from_string("dfdp", x, param, param_op)
-
-    def evaluate_dfdop(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d/dop of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d/dop of the the QNN
-        """
-        return self.evaluate_from_string("dfdop", x, param, param_op)
-
-    def evaluate_dfdpdx(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d^2/dpdx of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d^2/dpdx of the the QNN
-        """
-        return self.evaluate_from_string("dfdpdx", x, param, param_op)
-
-    def evaluate_dfdopdx(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates d^2/dopdx of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated d^2/dopdx of the the QNN
-        """
-        return self.evaluate_from_string("dfdopdx", x, param, param_op)
-
-    def evaluate_variance(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates the variance (<OO>-<O>^2) of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated variance of the the QNN
-        """
-        return self.evaluate_from_string("var", x, param, param_op)
-
-    def evaluate_var(
-        self,
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> Union[float, np.ndarray]:
-        """Evaluates the variance (<OO>-<O>^2) of the QNN
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-            param_op (Union[float,np.ndarray]): Parameter values of the operator
-
-        Returns:
-            Evaluated variance of the the QNN
-        """
-        return self.evaluate_variance(x, param, param_op)
-
-    def evaluate_probabilities(self, x: Union[float, np.ndarray], param: Union[float, np.ndarray]):
-        """Evaluate the probabilities of the feature map / PQC.
-
-        The function only works with the QuantumInstance executer.
-
-        Args:
-            x (Union[float,np.ndarray]): Input data values
-            param (Union[float,np.ndarray]): Parameter values of the PQC
-
-        Returns:
-            List of probabilities stored in the SparseVectorStateFn format.
-            (dictionary can be obtained by .to_dict_fn() or to_dict_fn().primitive)
-        """
-        # TODO: Implementation with Sampler
-        opflow = self.get_opflow_from_string("f")
-        opflow_with_param = self.pqc_derivatives.assign_parameters(opflow, x, param)
-        if self.quantum_instance is not None:
-            return evaluate_opflow_qi(self.quantum_instance, opflow_with_param)
-        else:
-            raise RuntimeError("Probabilities are only implemented for Quantum Instances!")
-
-    def evaluate(
-        self,
-        values,  # TODO: data type definition missing Union[str,expec,tuple,...]
-        x: Union[float, np.ndarray],
-        param: Union[float, np.ndarray],
-        param_op: Union[float, np.ndarray],
-    ) -> dict:
-        """General function for evaluating the output of derivatives of the QNN.
-
-        Evaluation works for given combination of
-        input features x and parameters param and param_op.
-        The function includes caching of results
-
-        If x, param, and/or param_op are given as a nested list
-        (for example multiple sets of parameters),
-        the values are returned in a nested list.
-
-        Args:
-            values : list of what values and derivatives of the qnn are eveluated.
-                Multiple inputs have to be a tuple.
-            x (np.ndarray): Values of the input feature data.
-            param (np.ndarray): Parameter values of the PQC parameters
-            param_op (np.ndarray): Parameter values of the operator parameters
-
-
-        Results:
-            Returns a dictionary with the computed values.
-            The keys of the dictionary are given by the entries in the values tuple
-
-        """
-
-        def generate_real_todo_dic(values, value_dict):
-            """Converts the input values into a sorted dictionary
-            of of expec items"""
-
-            # helper function for adding elemets to the real todo dict
-            def add_to_real_todo_dic(item: expec, real_todo_dic, value_dict):
-                if item not in value_dict:
-                    if item.wavefunction in real_todo_dic:
-                        #  check if i is already in the real todo list
-                        if item not in real_todo_dic[item.wavefunction]:
-                            real_todo_dic[item.wavefunction].append(item)
-                    else:
-                        real_todo_dic[item.wavefunction] = [item]
-                return real_todo_dic
-
-            # labels can be overwritten
-            try:
-                expec_list = [expec.from_variable(i) for i in values]
-            except TypeError:
-                expec_list = [expec.from_variable(values)]
-            # build dictionary for later use
-            real_todo_dic = {}
-            for i in expec_list:
-                # special cases of variance computation for post-processing:
-                if i.operator == "var" and i.wavefunction == "I":
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "OO"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "O"), real_todo_dic, value_dict
-                    )
-                elif i.operator == "var" and i.wavefunction == "dx":
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("dx", "OO"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "O"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("dx", "O"), real_todo_dic, value_dict
-                    )
-                elif i.operator == "var" and i.wavefunction == "dp":
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("dp", "OO"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "O"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("dp", "O"), real_todo_dic, value_dict
-                    )
-                elif i.operator == "dvardop" and i.wavefunction == "I":
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "OOdop"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "O"), real_todo_dic, value_dict
-                    )
-                    real_todo_dic = add_to_real_todo_dic(
-                        expec("I", "dop"), real_todo_dic, value_dict
-                    )
-                else:
-                    real_todo_dic = add_to_real_todo_dic(i, real_todo_dic, value_dict)
-            return real_todo_dic
-
-        def to_tuple(x):
-            """helper function for converting data into hashable tuples"""
-
-            def flatten(container):
-                for i in container:
-                    if isinstance(i, (list, tuple, np.ndarray)):
-                        for j in flatten(i):
-                            yield j
-                    else:
-                        yield i
-
-            if isinstance(x, float):
-                return tuple([x])
-            elif len(np.shape(x)) == 1:
-                return tuple(list(x))
-            else:
-                return tuple(flatten(x))
-
-        def measure_to_list(measure_op, offset=0):
-            """
-            Creates a list the numbers multpile measuremnt operators for later resorting
-            """
-
-            measure_list = []
-            global countervar
-            countervar = offset - 1
-
-            def build_circuit_list(operator: OperatorBase):
-                if isinstance(operator, CircuitStateFn):
-                    raise RuntimeError("No circuits are allows at this point!")
-                elif isinstance(operator, OperatorStateFn):
-                    global countervar
-                    countervar = countervar + 1
-                    measure_list.append(operator)
-                    return countervar
-                elif isinstance(operator, ListOp):
-                    list = []
-                    for op in operator.oplist:
-                        list.append(build_circuit_list(op))
-                    return list
-
-            index_list = build_circuit_list(measure_op)
-
-            return index_list, measure_list
-
-        def sort_back_to_nparray(index_list, val):
-            """
-            Uses the list generated by measure_to_list to sort back the values into the nested
-            output list structure
-            """
-
-            def sort_back_val(index_list):
-                if isinstance(index_list, list):
-                    return [sort_back_val(op) for op in index_list]
-                elif isinstance(index_list, int):
-                    return val[index_list]
-                else:
-                    raise RuntimeError("Wrong format of inputed index list")
-
-            return sort_back_val(index_list)
-
-        # Done with the helper functions, start of the evaluate function
-
-        # input adjustments for x, param, param_op to get correct stacking of values
-        x_inp, multi_x = adjust_input(x, self.num_features)
-        param_inp, multi_param = adjust_input(param, self.num_parameters)
-        param_op_inp, multi_param_op = adjust_input(param_op, self.num_parameters_operator)
-
-        # If values is not a tuple, convert it
-        if not isinstance(values, tuple):
-            values = (values,)
-
-        # return dictionary for input data, it will be empty
-        # if the combination of x,param,param_op is touched the first time
-        if self._result_caching == True:
-            caching_tuple = (to_tuple(x), to_tuple(param), to_tuple(param_op))
-            value_dict = self.result_container.get(caching_tuple, {})
-        else:
-            value_dict = {}
-
-        # create dictionary sorted w.r.t. the circuits
-        # expectation values with the same circuits are evaluated only once
-        # variance set-up is created here
-        real_todo_dic = generate_real_todo_dic(values, value_dict)
-
-        for key, op_list in real_todo_dic.items():
-            # creates list of operators that can be evaluated for the same circuit
-            measure_list = []  #  listoff all considered measure operators
-            index_list = []  # list for index counting
-            offset = 0
-            for expec_ in op_list:
-                # Obtained the derivative from the operator module
-                operator = self.operator_derivatives.get_derivate(expec_.operator)
-                # Assign parameters and convert to sparse Pauli representation
-                op_with_param = self.operator_derivatives.assign_parameters(operator, param_op_inp)
-
-                # flatten the measurement operator list,
-                # but keep the nested list structure in index_list for later reconstruction
-                index_list_op, measure_list_op = measure_to_list(op_with_param, offset)
-                offset = offset + len(measure_list_op)
-                measure_list = measure_list + measure_list_op
-                index_list.append(index_list_op)
-
-            # get the circuits of the PQC derivatives from the feature map module
-            pqc_opflow = self.pqc_derivatives.get_derivate(key)
-
-            # check for multiple circuits (e.g. gradient)
-            if isinstance(pqc_opflow, ListOp):
-                array_circ = True
-            else:
-                array_circ = False
-
-            # add operator measurments to the circuits
-            opflow_measured = measure_feature_map_derivative(pqc_opflow, ListOp(measure_list))
-
-            if self.split_paulis:
-                # If necessary, split the measurements containing X and Y operators
-                # into extra measurements
-                opflow_measured = _split_paulis(opflow_measured, len(measure_list) == 1)
-
-            # assign parameters of the circuit
-            opflow_with_param = self.pqc_derivatives.assign_parameters(
-                opflow_measured, x_inp, param_inp
-            )
-
-            # evaluate the list of opflows
-            val = self.executor.opflow_exec(opflow_with_param)
-
-            # In case of multiple circuits, swapp measurment operator to index 2 for a clearer nesting
-            if array_circ:
-                swapp_list = list(np.arange(len(val.shape), dtype=int))
-                swapp_list = [swapp_list[0]] + [swapp_list[1]] + swapp_list[-1:] + swapp_list[2:-1]
-                val = np.transpose(val, axes=swapp_list)
-
-            # store results in value_dict
-            # if get rid of unncessary arrays to fit the input vector nesting
-            ioff = 0
-            for iexpec, expec_ in enumerate(op_list):
-                val_x = []
-                for i in range(len(val)):
-                    val_param = []
-                    for j in range(len(val[i])):
-                        val_param.append(
-                            np.array(sort_back_to_nparray(index_list[iexpec], val[i][j]))
-                        )
-                    val_x.append(np.array(val_param))
-                val_final = np.array(val_x)
-
-                reshape_list = []
-                shape = val_final.shape
-                if multi_x:
-                    reshape_list.append(shape[0])
-                if multi_param:
-                    reshape_list.append(shape[1])
-                if multi_param_op:
-                    reshape_list.append(shape[2])
-                if len(shape) == 4:
-                    reshape_list.append(shape[3])
-                if len(shape) > 4:
-                    reshape_list += list(shape[3:])
-                if len(reshape_list) == 0:
-                    value_dict[expec_] = val_final.reshape(-1)[0]
-                else:
-                    value_dict[expec_] = val_final.reshape(reshape_list)
-                ioff = ioff + 1
-
-        # Set-up lables from the input list
-        for todo in values:
-            todo_expec = expec.from_variable(todo)
-
-            # post-processing of the variance
-            # variance
-            if todo_expec.operator == "var" and todo_expec.wavefunction == "I":
-                value_dict[todo_expec] = value_dict[expec("I", "OO")] - np.square(
-                    value_dict[expec("I", "O")]
-                )
-            # d/dx variance
-            elif todo_expec.operator == "var" and todo_expec.wavefunction == "dx":
-                if self.num_features == 1:
-                    value_dict[todo_expec] = value_dict[expec("dx", "OO")] - 2.0 * (
-                        np.multiply(value_dict[expec("dx", "O")], value_dict[expec("I", "O")])
-                    )
-                else:
-                    value_dict[todo_expec] = np.zeros(value_dict[expec("dx", "OO")].shape)
-                    for i in range(value_dict[expec("dx", "OO")].shape[-1]):
-                        value_dict[todo_expec][..., i] = value_dict[expec("dx", "OO")][
-                            ..., i
-                        ] - 2.0 * (
-                            np.multiply(
-                                value_dict[expec("dx", "O")][..., i],
-                                value_dict[expec("I", "O")],
-                            )
-                        )
-            # d/dp variance
-            elif todo_expec.operator == "var" and todo_expec.wavefunction == "dp":
-                if self.num_parameters == 1:
-                    value_dict[todo_expec] = value_dict[expec("dp", "OO")] - 2.0 * (
-                        np.multiply(value_dict[expec("dp", "O")], value_dict[expec("I", "O")])
-                    )
-                else:
-                    value_dict[todo_expec] = np.zeros(value_dict[expec("dp", "OO")].shape)
-                    for i in range(value_dict[expec("dp", "OO")].shape[-1]):
-                        value_dict[todo_expec][..., i] = value_dict[expec("dp", "OO")][
-                            ..., i
-                        ] - 2.0 * (
-                            np.multiply(
-                                value_dict[expec("dp", "O")][..., i],
-                                value_dict[expec("I", "O")],
-                            )
-                        )
-            # d/dop variance
-            elif todo_expec.operator == "dvardop" and todo_expec.wavefunction == "I":
-                if self.num_parameters_operator == 1:
-                    value_dict[todo_expec] = value_dict[expec("I", "OOdop")] - 2.0 * (
-                        np.multiply(value_dict[expec("I", "dop")], value_dict[expec("I", "O")])
-                    )
-                else:
-                    value_dict[todo_expec] = np.zeros(value_dict[expec("I", "OOdop")].shape)
-                    for i in range(value_dict[expec("I", "OOdop")].shape[-1]):
-                        value_dict[todo_expec][..., i] = value_dict[expec("I", "OOdop")][
-                            ..., i
-                        ] - 2.0 * (
-                            np.multiply(
-                                value_dict[expec("I", "dop")][..., i],
-                                value_dict[expec("I", "O")],
-                            )
-                        )
-
-            # assign values to the label of the expectation value
-            value_dict[todo] = value_dict[todo_expec]
-            if isinstance(todo, expec) and todo.label != "":
-                value_dict[todo.label] = value_dict[todo_expec]
-
-        # Add x, param, and param_op to the dictionary as default
-        value_dict["x"] = x
-        value_dict["param"] = param
-        value_dict["param_op"] = param_op
-
-        # Store the updated dictionary for the theta value
-        if self._result_caching:
-            self.result_container[caching_tuple] = value_dict
-
-        return value_dict
-
-
-def _split_paulis(operator: OperatorBase, single_measure: bool) -> OperatorBase:
-    """
-    Split the opflow such that it can be measured in Z basis.
-
-    Splits up the opflow expression such that the meaurement operators can be evaluated
-    in the Z-basis. The routine is needed, if Y and X operators are present in the measurement
-
-    Args:
-        operator (OperatorBase) : Opflow expression that is checked
-        single_measure (bool): Is true if there is only a single
-            measurement in the opflow structure, otherwise a ListOp is considered
-    Returns:
-        New opflow expression where measurements are correctly split
-        into seprate circuits
-    """
-    # We reached a ComposedOp term -> seprate the different measurment operators
-    # using qiskit's PauliExpectation
-    if isinstance(operator, ComposedOp):
-        coeff = operator.coeff
-        operator_splitted = PauliExpectation().convert(operator)
-        operator_splitted._coeff = coeff
-        if single_measure == True:
-            return ListOp([operator_splitted])
-        else:
-            return operator_splitted
-
-    # We reached a CircuitStateFn term that should not be present in this routine
-    elif isinstance(operator, CircuitStateFn):
-        raise ValueError("CircuitStateFn type is not allowed!")
-
-    # We reached a list of opflow terms, recursive call of
-    # the function to all children in the list
-    elif isinstance(operator, ListOp):
-        op_list = [_split_paulis(op, single_measure) for op in operator.oplist]
-        if isinstance(operator, SummedOp):
-            return SummedOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, TensoredOp):
-            return TensoredOp(
-                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
-            )
-        elif isinstance(operator, real_ListOp):
-            return ListOp(
-                oplist=[op for op in op_list if op != ~Zero @ One],
-                coeff=operator.coeff,
-                combo_fn=operator.combo_fn,
-            )
-        else:
-            raise ValueError("Unknown ListOp type in _split_paulis:", type(operator))
-    else:
-        raise ValueError("Unknown type in _split_paulis:", type(operator))
+from qiskit.circuit import ParameterVector, ParameterExpression
+from qiskit.circuit.parametervector import ParameterVectorElement
+from qiskit.opflow import OperatorBase, CircuitStateFn, OperatorStateFn
+from qiskit.opflow import ListOp, SummedOp, ComposedOp, TensoredOp
+from qiskit.opflow import Zero, One
+from qiskit.opflow.list_ops.list_op import ListOp as real_ListOp
+from qiskit.opflow.expectations import PauliExpectation
+from qiskit.utils import QuantumInstance
+
+from typing import Union
+import numpy as np
+
+from ..expectation_operator.expectation_operator_base import ExpectationOperatorBase
+from ..expectation_operator.expectation_operator_derivatives import ExpectationOperatorDerivatives
+
+from ..feature_map.feature_map_base import FeatureMapBase
+from ..feature_map.feature_map_derivatives import (
+    FeatureMapDerivatives,
+    measure_feature_map_derivative,
+)
+from ..feature_map.transpiled_feature_map import TranspiledFeatureMap
+
+from ..util.data_preprocessing import adjust_input
+
+from ..util import Executor
+
+
+class expec:
+    """Data structure that holds the set-up of derivative of the expectation value.
+
+    Args:
+        wavefunction (Union[str, tuple, ParameterVectorElement]): Describes the wavefuction or its
+            derivative. If tuple or ParameterVectorElement the differentiation with respect to the
+            parameters in the tuple or with respect to the ParameterVectorElement is considered
+        operator (str): String for the expectation value operator (O, OO, dop, dopdop, var).
+        label (str): Label that is used for displaying or in the value dict of the QNN class.
+
+    """
+
+    def __init__(
+        self,
+        wavefunction: Union[str, tuple, ParameterVectorElement],
+        operator: str,
+        label: str = "",
+    ):
+        self.wavefunction = wavefunction
+        self.operator = operator
+        self.label = label
+
+    def __var_to_str(self, val: Union[str, tuple, ParameterExpression, ParameterVector]) -> str:
+        """Converter for variables to string.
+
+        Args:
+            val (Union[str, tuple, ParameterExpression, ParameterVector]): Input that is converted
+                to string
+
+        Returns:
+            String that contains the converted val variable
+
+        """
+        if isinstance(val, ParameterExpression):
+            out_str = str(val.name)
+        elif isinstance(val, ParameterVector):
+            out_str = str(val.name)
+        elif isinstance(val, tuple):
+            out_str = "("
+            for x in val:
+                out_str += self.__var_to_str(x) + ","
+            out_str += ")"
+        elif isinstance(val, str):
+            out_str = val
+        else:
+            out_str = str(val)
+        return out_str
+
+    def __repr__(self) -> str:
+        """Build-in string conversion for expec class."""
+        return self.__str__()
+
+    def __str__(self) -> str:
+        """Build-in string conversion for expec class."""
+        return (
+            "expec("
+            + self.__var_to_str(self.wavefunction)
+            + ","
+            + self.__var_to_str(self.operator)
+            + ","
+            + self.__var_to_str(self.label)
+            + ")"
+        )
+
+    def __len__(self) -> int:
+        """Build-in length of expec class (return 1)."""
+        return 1
+
+    def __eq__(self, other) -> bool:
+        """Build-in comparison of two expec class objects."""
+        return (
+            isinstance(other, self.__class__)
+            and self.wavefunction == other.wavefunction
+            and self.operator == other.operator
+        )
+
+    def __hash__(self) -> int:
+        """Build-in hash function for expec class."""
+        return hash((self.wavefunction, self.operator))
+
+    @classmethod
+    def from_string(cls, val: str):
+        """Converts an input string to the expec data structure.
+
+        Args:
+            String that defines the expectation value derivative
+
+        Returns:
+            Associated expec object
+
+        """
+
+        if isinstance(val, str):
+            if val == "f":
+                return cls("I", "O", "f")
+            elif val == "dfdx":
+                return cls("dx", "O", "dfdx")
+            elif val == "dfdxdx":
+                return cls("dxdx", "O", "dfdxdx")
+            elif val == "laplace":
+                return cls("laplace", "O", "laplace")
+            elif val == "laplace_dp":
+                return cls("laplace_dp", "O", "laplace_dp")
+            elif val == "laplace_dop":
+                return cls("laplace", "dop", "laplace_dop")
+            elif val == "dfdp":
+                return cls("dp", "O", "dfdp")
+            elif val == "dfdpdp":
+                return cls("dpdp", "O", "dfdpdp")
+            elif val == "dfdopdp":
+                return cls("dp", "dop", "dfdop")
+            elif val == "dfdop":
+                return cls("I", "dop", "dfdop")
+            elif val == "dfdopdop":
+                return cls("I", "dopdop", "dfdop")
+            elif val == "dfdpdx":
+                return cls("dpdx", "O", "dfdpdx")
+            elif val == "dfdopdx":
+                return cls("dx", "dop", "dfdopdx")
+            elif val == "dfdopdxdx":
+                return cls("dxdx", "dop", "dfdopdxdx")
+            elif val == "fcc":
+                return cls("I", "OO", "fcc")
+            elif val == "dfccdx":
+                return cls("dx", "OO", "dfccdx")
+            elif val == "dfccdxdx":
+                return cls("dxdx", "OO", "dfccdxdx")
+            elif val == "dfccdp":
+                return cls("dp", "OO", "dfccdp")
+            elif val == "dfccdpdp":
+                return cls("dpdp", "OO", "dfccdpdp")
+            elif val == "dfccdopdx":
+                return cls("dx", "OOdop", "dfccdpdp")
+            elif val == "dfccdop":
+                return cls("I", "OOdop", "dfccdop")
+            elif val == "dfccdopdop":
+                return cls("I", "OOdopdop", "dfccdopdop")
+            elif val in ("var", "varf"):
+                return cls("I", "var", val)
+            elif val in ("dvardx", "dvarfdx"):
+                return cls("dx", "var", val)
+            elif val in ("dvardp", "dvarfdp"):
+                return cls("dp", "var", val)
+            elif val in ("dvardop", "dvarfdop"):
+                return cls("I", "dvardop", val)
+            elif val == "fischer":
+                return cls("I", "fischer", val)
+            else:
+                raise ValueError("Unknown input string:", val)
+        else:
+            raise TypeError("String expected, found type:", type(val))
+
+    @classmethod
+    def from_tuple(cls, val: tuple, operator: str = "O"):
+        """Creates an expec object from an input tuple
+
+        Args:
+            val (tuple): Tuple for the differentiation of the wavefunction.
+            operator (str): String for the operator, default='O'.
+
+        Returns
+            Associated expec object
+        """
+        return cls(val, operator, val)
+
+    @classmethod
+    def from_parameter(cls, val: ParameterVectorElement, operator: str = "O"):
+        """Creates an expec object from an inputted parameter
+
+        Args:
+            val (ParameterVectorElement): Parameter that is used in the differentiation.
+            operator (str): String for the operator, default='O'.
+
+        Returns
+            Associated expec object
+        """
+        return cls((val,), operator, (val,))
+
+    @classmethod
+    def from_variable(cls, val):
+        """Creates an expec object from an inputted value
+
+        Args:
+            val (Union[expec,str,tuple,ParameterVectorElement]): value that defines the derivative
+
+        Returns
+            Associated expec object
+        """
+
+        if isinstance(val, expec):
+            return val
+        elif isinstance(val, str):
+            return cls.from_string(val)
+        elif isinstance(val, tuple):
+            return cls.from_tuple(val)
+        elif isinstance(val, ParameterVectorElement):
+            return cls.from_parameter(val)
+        else:
+            raise TypeError("Unsupported type:", type(val))
+
+
+class QNN:
+    """A class for working with QNNs and its derivatives
+
+    Args:
+        pqc (FeatureMapBase) : parameterized quantum circuit in feature map format
+        operator (Union[ExpectationOperatorBase,list]): Operator that are used in the expectation value
+            of the QNN. Can be a list for multiple outputs.
+        executor (Executor) : Executor that is used for the evaluation of the QNN
+        opflow_caching : Caching of the opflow expressions (default = True recommended)
+        result_caching : Caching of the result for each x,param,param_op combination
+            (default = True)
+    """
+
+    def __init__(
+        self,
+        pqc: FeatureMapBase,
+        operator: Union[ExpectationOperatorBase, list],
+        executor: Executor,
+        opflow_caching=True,
+        result_caching=True,
+    ) -> None:
+        # Potential TODO: move executor into extra util class
+        # Executer set-up
+        self.executor = executor
+        self.backend = self.executor.backend
+
+        # Storing the input data # TODO: custom transpilation function
+        self.pqc = TranspiledFeatureMap(pqc, self.backend)
+        self.operator = operator
+        num_qubits_operator = 0
+        if isinstance(self.operator, list):
+            for i in range(len(self.operator)):
+                self.operator[i].set_map(self.pqc.qubit_map, self.pqc.num_all_qubits)
+                num_qubits_operator = max(num_qubits_operator, self.operator[i].num_qubits)
+        else:
+            self.operator.set_map(self.pqc.qubit_map, self.pqc.num_all_qubits)
+            num_qubits_operator = self.operator.num_qubits
+
+        self.operator_derivatives = ExpectationOperatorDerivatives(self.operator, opflow_caching)
+        self.pqc_derivatives = FeatureMapDerivatives(self.pqc, opflow_caching)
+
+        if self.pqc.num_qubits != num_qubits_operator:
+            raise ValueError("Number of Qubits are not the same!")
+        else:
+            self._num_qubits = self.pqc.num_qubits
+
+        if self.executor.get_opflow_executor() in ("sampler", "quantum_instance"):
+            # For Quantum Instance or the Sampler primitive, X and Y Pauli matrices have to be treated extra
+            # This is very inefficient!
+            operator_string = str(self.operator)
+            if "X" in operator_string or "Y" in operator_string:
+                self.split_paulis = True
+                print(
+                    "The expectation operator includes X and Y gates, consider switching"
+                    + " to the Estimator primitive for a faster performance!"
+                )
+            else:
+                self.split_paulis = False
+        else:
+            self.split_paulis = False
+
+        # Set-up shots from backend
+        self._inital_shots = self.executor.get_shots()
+
+        # Initialize result cache
+        self._result_caching = result_caching
+        self.result_container = {}
+
+    def set_shots(self, num_shots: int) -> None:
+        """Sets the number shots for the next evaluations.
+
+        Args:
+            num_shots (int): Number of shots that are set
+        """
+
+        self.executor.set_shots(num_shots)
+
+    def get_shots(self) -> int:
+        """Getter for the number of shots.
+
+        Returns:
+            Returns the number of shots that are used for the current evaluation."""
+        return self.executor.get_shots()
+
+    def reset_shots(self) -> None:
+        """Function for resetting the number of shots to the inital ones"""
+        self.executor.reset_shots()
+
+    @property
+    def num_qubits(self) -> int:
+        """Return the number of qubits of the QNN"""
+        return self._num_qubits
+
+    @property
+    def num_features(self) -> int:
+        """Return the dimension of the features of the PQC"""
+        return self.pqc_derivatives.num_features
+
+    @property
+    def num_parameters(self) -> int:
+        """Return the number of trainable parameters of the PQC"""
+        return self.pqc_derivatives.num_parameters
+
+    @property
+    def num_operator(self) -> int:
+        """Return the number outputs"""
+        return self.operator_derivatives.num_operators
+
+    @property
+    def num_parameters_operator(self) -> int:
+        """Return the number of trainable parameters of the expectation value operator"""
+        return self.operator_derivatives.num_parameters
+
+    @property
+    def multiple_output(self) -> bool:
+        """Return true if multiple outputs are used"""
+        return self.operator_derivatives.multiple_output
+
+    @property
+    def parameters(self):
+        """Return the parameter vector of the PQC."""
+        return self.pqc_derivatives.p
+
+    @property
+    def features(self):
+        """Return the feature vector of the PQC."""
+        return self.pqc_derivatives.x
+
+    @property
+    def parameters_operator(self):
+        """Return the parameter vector of the cost operator."""
+        return self.operator_derivatives.parameters
+
+    def get_opflow_from_string(self, input_string: str):
+        """Return the opflow expression of the given PQC
+
+        Args:
+            input_string (str): String from which the opflow is obtained.
+
+        Returns:
+            Opflow structure created from the string.
+        """
+        return self.get_opflow_from_expec(expec.from_string(input_string))
+
+    def get_opflow_from_expec(self, input_expec: expec):
+        """Returns the opflow expression for the given expec object.
+
+        Args:
+            input_expec (expec): Expec pbject from which the opflow is obtained
+
+        Returns:
+            Opflow structure created from the expec object.
+        """
+        return measure_feature_map_derivative(
+            self.pqc_derivatives.get_derivate(input_expec.wavefunction),
+            self.operator_derivatives.get_derivate(input_expec.operator),
+        )
+
+    def evaluate_diff_tuple(
+        self,
+        diff_tuple,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluate the given tuple of derivatives of the PQC.
+
+        Args:
+            diff_tuple: Tuple with parameters used in the differentiation
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Differentiated values of the QNN
+        """
+        return self.evaluate((diff_tuple,), x, param, param_op)[diff_tuple]
+
+    def evaluate_from_string(
+        self,
+        input_string: str,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluate the given PQC from an input string
+
+        Args:
+            input_string (str): Input string that determines the evaluated value(s)
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Values from the QNN defined by the string
+        """
+        return self.evaluate(input_string, x, param, param_op)[input_string]
+
+    def evaluate_f(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Values from the QNN
+        """
+        return self.evaluate_from_string("f", x, param, param_op)
+
+    def evaluate_dfdx(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d/dx of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d/dx of the the QNN
+        """
+        return self.evaluate_from_string("dfdx", x, param, param_op)
+
+    def evaluate_dfdxdx(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d^2/dxdx of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d^2/dxdx of the the QNN
+        """
+        return self.evaluate_from_string("dfdxdx", x, param, param_op)
+
+    def evaluate_laplace(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates laplace(x) of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated laplace(x) of the the QNN
+        """
+        return self.evaluate_from_string("laplace", x, param, param_op)
+
+    def evaluate_laplace_dp(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d laplace(x)/dp of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d laplace(x)/dp of the the QNN
+        """
+        return self.evaluate_from_string("laplace_dp", x, param, param_op)
+
+    def evaluate_laplace_dop(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d laplace(x)/dop of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d laplace(x)/dop of the the QNN
+        """
+        return self.evaluate_from_string("laplace_dop", x, param, param_op)
+
+    def evaluate_dfdp(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d/dp of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d/dp of the the QNN
+        """
+        return self.evaluate_from_string("dfdp", x, param, param_op)
+
+    def evaluate_dfdop(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d/dop of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d/dop of the the QNN
+        """
+        return self.evaluate_from_string("dfdop", x, param, param_op)
+
+    def evaluate_dfdpdx(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d^2/dpdx of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d^2/dpdx of the the QNN
+        """
+        return self.evaluate_from_string("dfdpdx", x, param, param_op)
+
+    def evaluate_dfdopdx(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates d^2/dopdx of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated d^2/dopdx of the the QNN
+        """
+        return self.evaluate_from_string("dfdopdx", x, param, param_op)
+
+    def evaluate_variance(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates the variance (<OO>-<O>^2) of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated variance of the the QNN
+        """
+        return self.evaluate_from_string("var", x, param, param_op)
+
+    def evaluate_var(
+        self,
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> Union[float, np.ndarray]:
+        """Evaluates the variance (<OO>-<O>^2) of the QNN
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+            param_op (Union[float,np.ndarray]): Parameter values of the operator
+
+        Returns:
+            Evaluated variance of the the QNN
+        """
+        return self.evaluate_variance(x, param, param_op)
+
+    def evaluate_probabilities(self, x: Union[float, np.ndarray], param: Union[float, np.ndarray]):
+        """Evaluate the probabilities of the feature map / PQC.
+
+        The function only works with the QuantumInstance executer.
+
+        Args:
+            x (Union[float,np.ndarray]): Input data values
+            param (Union[float,np.ndarray]): Parameter values of the PQC
+
+        Returns:
+            List of probabilities stored in the SparseVectorStateFn format.
+            (dictionary can be obtained by .to_dict_fn() or to_dict_fn().primitive)
+        """
+        # TODO: Implementation with Sampler
+        opflow = self.get_opflow_from_string("f")
+        opflow_with_param = self.pqc_derivatives.assign_parameters(opflow, x, param)
+        if self.quantum_instance is not None:
+            return evaluate_opflow_qi(self.quantum_instance, opflow_with_param)
+        else:
+            raise RuntimeError("Probabilities are only implemented for Quantum Instances!")
+
+    def evaluate(
+        self,
+        values,  # TODO: data type definition missing Union[str,expec,tuple,...]
+        x: Union[float, np.ndarray],
+        param: Union[float, np.ndarray],
+        param_op: Union[float, np.ndarray],
+    ) -> dict:
+        """General function for evaluating the output of derivatives of the QNN.
+
+        Evaluation works for given combination of
+        input features x and parameters param and param_op.
+        The function includes caching of results
+
+        If x, param, and/or param_op are given as a nested list
+        (for example multiple sets of parameters),
+        the values are returned in a nested list.
+
+        Args:
+            values : list of what values and derivatives of the qnn are eveluated.
+                Multiple inputs have to be a tuple.
+            x (np.ndarray): Values of the input feature data.
+            param (np.ndarray): Parameter values of the PQC parameters
+            param_op (np.ndarray): Parameter values of the operator parameters
+
+
+        Results:
+            Returns a dictionary with the computed values.
+            The keys of the dictionary are given by the entries in the values tuple
+
+        """
+
+        def generate_real_todo_dic(values, value_dict):
+            """Converts the input values into a sorted dictionary
+            of of expec items"""
+
+            # helper function for adding elemets to the real todo dict
+            def add_to_real_todo_dic(item: expec, real_todo_dic, value_dict):
+                if item not in value_dict:
+                    if item.wavefunction in real_todo_dic:
+                        #  check if i is already in the real todo list
+                        if item not in real_todo_dic[item.wavefunction]:
+                            real_todo_dic[item.wavefunction].append(item)
+                    else:
+                        real_todo_dic[item.wavefunction] = [item]
+                return real_todo_dic
+
+            # labels can be overwritten
+            try:
+                expec_list = [expec.from_variable(i) for i in values]
+            except TypeError:
+                expec_list = [expec.from_variable(values)]
+            # build dictionary for later use
+            real_todo_dic = {}
+            for i in expec_list:
+                # special cases of variance computation for post-processing:
+                if i.operator == "var" and i.wavefunction == "I":
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "OO"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "O"), real_todo_dic, value_dict
+                    )
+                elif i.operator == "var" and i.wavefunction == "dx":
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("dx", "OO"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "O"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("dx", "O"), real_todo_dic, value_dict
+                    )
+                elif i.operator == "var" and i.wavefunction == "dp":
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("dp", "OO"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "O"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("dp", "O"), real_todo_dic, value_dict
+                    )
+                elif i.operator == "dvardop" and i.wavefunction == "I":
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "OOdop"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "O"), real_todo_dic, value_dict
+                    )
+                    real_todo_dic = add_to_real_todo_dic(
+                        expec("I", "dop"), real_todo_dic, value_dict
+                    )
+                else:
+                    real_todo_dic = add_to_real_todo_dic(i, real_todo_dic, value_dict)
+            return real_todo_dic
+
+        def to_tuple(x):
+            """helper function for converting data into hashable tuples"""
+
+            def flatten(container):
+                for i in container:
+                    if isinstance(i, (list, tuple, np.ndarray)):
+                        for j in flatten(i):
+                            yield j
+                    else:
+                        yield i
+
+            if isinstance(x, float):
+                return tuple([x])
+            elif len(np.shape(x)) == 1:
+                return tuple(list(x))
+            else:
+                return tuple(flatten(x))
+
+        def measure_to_list(measure_op, offset=0):
+            """
+            Creates a list the numbers multpile measuremnt operators for later resorting
+            """
+
+            measure_list = []
+            global countervar
+            countervar = offset - 1
+
+            def build_circuit_list(operator: OperatorBase):
+                if isinstance(operator, CircuitStateFn):
+                    raise RuntimeError("No circuits are allows at this point!")
+                elif isinstance(operator, OperatorStateFn):
+                    global countervar
+                    countervar = countervar + 1
+                    measure_list.append(operator)
+                    return countervar
+                elif isinstance(operator, ListOp):
+                    list = []
+                    for op in operator.oplist:
+                        list.append(build_circuit_list(op))
+                    return list
+
+            index_list = build_circuit_list(measure_op)
+
+            return index_list, measure_list
+
+        def sort_back_to_nparray(index_list, val):
+            """
+            Uses the list generated by measure_to_list to sort back the values into the nested
+            output list structure
+            """
+
+            def sort_back_val(index_list):
+                if isinstance(index_list, list):
+                    return [sort_back_val(op) for op in index_list]
+                elif isinstance(index_list, int):
+                    return val[index_list]
+                else:
+                    raise RuntimeError("Wrong format of inputed index list")
+
+            return sort_back_val(index_list)
+
+        # Done with the helper functions, start of the evaluate function
+
+        # input adjustments for x, param, param_op to get correct stacking of values
+        x_inp, multi_x = adjust_input(x, self.num_features)
+        param_inp, multi_param = adjust_input(param, self.num_parameters)
+        param_op_inp, multi_param_op = adjust_input(param_op, self.num_parameters_operator)
+
+        # If values is not a tuple, convert it
+        if not isinstance(values, tuple):
+            values = (values,)
+
+        # return dictionary for input data, it will be empty
+        # if the combination of x,param,param_op is touched the first time
+        if self._result_caching == True:
+            caching_tuple = (to_tuple(x), to_tuple(param), to_tuple(param_op))
+            value_dict = self.result_container.get(caching_tuple, {})
+        else:
+            value_dict = {}
+
+        # create dictionary sorted w.r.t. the circuits
+        # expectation values with the same circuits are evaluated only once
+        # variance set-up is created here
+        real_todo_dic = generate_real_todo_dic(values, value_dict)
+
+        for key, op_list in real_todo_dic.items():
+            # creates list of operators that can be evaluated for the same circuit
+            measure_list = []  #  listoff all considered measure operators
+            index_list = []  # list for index counting
+            offset = 0
+            for expec_ in op_list:
+                # Obtained the derivative from the operator module
+                operator = self.operator_derivatives.get_derivate(expec_.operator)
+                # Assign parameters and convert to sparse Pauli representation
+                op_with_param = self.operator_derivatives.assign_parameters(operator, param_op_inp)
+
+                # flatten the measurement operator list,
+                # but keep the nested list structure in index_list for later reconstruction
+                index_list_op, measure_list_op = measure_to_list(op_with_param, offset)
+                offset = offset + len(measure_list_op)
+                measure_list = measure_list + measure_list_op
+                index_list.append(index_list_op)
+
+            # get the circuits of the PQC derivatives from the feature map module
+            pqc_opflow = self.pqc_derivatives.get_derivate(key)
+
+            # check for multiple circuits (e.g. gradient)
+            if isinstance(pqc_opflow, ListOp):
+                array_circ = True
+            else:
+                array_circ = False
+
+            # add operator measurments to the circuits
+            opflow_measured = measure_feature_map_derivative(pqc_opflow, ListOp(measure_list))
+
+            if self.split_paulis:
+                # If necessary, split the measurements containing X and Y operators
+                # into extra measurements
+                opflow_measured = _split_paulis(opflow_measured, len(measure_list) == 1)
+
+            # assign parameters of the circuit
+            opflow_with_param = self.pqc_derivatives.assign_parameters(
+                opflow_measured, x_inp, param_inp
+            )
+
+            # evaluate the list of opflows
+            val = self.executor.opflow_exec(opflow_with_param)
+
+            # In case of multiple circuits, swapp measurment operator to index 2 for a clearer nesting
+            if array_circ:
+                swapp_list = list(np.arange(len(val.shape), dtype=int))
+                swapp_list = [swapp_list[0]] + [swapp_list[1]] + swapp_list[-1:] + swapp_list[2:-1]
+                val = np.transpose(val, axes=swapp_list)
+
+            # store results in value_dict
+            # if get rid of unncessary arrays to fit the input vector nesting
+            ioff = 0
+            for iexpec, expec_ in enumerate(op_list):
+                val_x = []
+                for i in range(len(val)):
+                    val_param = []
+                    for j in range(len(val[i])):
+                        val_param.append(
+                            np.array(sort_back_to_nparray(index_list[iexpec], val[i][j]))
+                        )
+                    val_x.append(np.array(val_param))
+                val_final = np.array(val_x)
+
+                reshape_list = []
+                shape = val_final.shape
+                if multi_x:
+                    reshape_list.append(shape[0])
+                if multi_param:
+                    reshape_list.append(shape[1])
+                if multi_param_op:
+                    reshape_list.append(shape[2])
+                if len(shape) == 4:
+                    reshape_list.append(shape[3])
+                if len(shape) > 4:
+                    reshape_list += list(shape[3:])
+                if len(reshape_list) == 0:
+                    value_dict[expec_] = val_final.reshape(-1)[0]
+                else:
+                    value_dict[expec_] = val_final.reshape(reshape_list)
+                ioff = ioff + 1
+
+        # Set-up lables from the input list
+        for todo in values:
+            todo_expec = expec.from_variable(todo)
+
+            # post-processing of the variance
+            # variance
+            if todo_expec.operator == "var" and todo_expec.wavefunction == "I":
+                value_dict[todo_expec] = value_dict[expec("I", "OO")] - np.square(
+                    value_dict[expec("I", "O")]
+                )
+            # d/dx variance
+            elif todo_expec.operator == "var" and todo_expec.wavefunction == "dx":
+                if self.num_features == 1:
+                    value_dict[todo_expec] = value_dict[expec("dx", "OO")] - 2.0 * (
+                        np.multiply(value_dict[expec("dx", "O")], value_dict[expec("I", "O")])
+                    )
+                else:
+                    value_dict[todo_expec] = np.zeros(value_dict[expec("dx", "OO")].shape)
+                    for i in range(value_dict[expec("dx", "OO")].shape[-1]):
+                        value_dict[todo_expec][..., i] = value_dict[expec("dx", "OO")][
+                            ..., i
+                        ] - 2.0 * (
+                            np.multiply(
+                                value_dict[expec("dx", "O")][..., i],
+                                value_dict[expec("I", "O")],
+                            )
+                        )
+            # d/dp variance
+            elif todo_expec.operator == "var" and todo_expec.wavefunction == "dp":
+                if self.num_parameters == 1:
+                    value_dict[todo_expec] = value_dict[expec("dp", "OO")] - 2.0 * (
+                        np.multiply(value_dict[expec("dp", "O")], value_dict[expec("I", "O")])
+                    )
+                else:
+                    value_dict[todo_expec] = np.zeros(value_dict[expec("dp", "OO")].shape)
+                    for i in range(value_dict[expec("dp", "OO")].shape[-1]):
+                        value_dict[todo_expec][..., i] = value_dict[expec("dp", "OO")][
+                            ..., i
+                        ] - 2.0 * (
+                            np.multiply(
+                                value_dict[expec("dp", "O")][..., i],
+                                value_dict[expec("I", "O")],
+                            )
+                        )
+            # d/dop variance
+            elif todo_expec.operator == "dvardop" and todo_expec.wavefunction == "I":
+                if self.num_parameters_operator == 1:
+                    value_dict[todo_expec] = value_dict[expec("I", "OOdop")] - 2.0 * (
+                        np.multiply(value_dict[expec("I", "dop")], value_dict[expec("I", "O")])
+                    )
+                else:
+                    value_dict[todo_expec] = np.zeros(value_dict[expec("I", "OOdop")].shape)
+                    for i in range(value_dict[expec("I", "OOdop")].shape[-1]):
+                        value_dict[todo_expec][..., i] = value_dict[expec("I", "OOdop")][
+                            ..., i
+                        ] - 2.0 * (
+                            np.multiply(
+                                value_dict[expec("I", "dop")][..., i],
+                                value_dict[expec("I", "O")],
+                            )
+                        )
+
+            # assign values to the label of the expectation value
+            value_dict[todo] = value_dict[todo_expec]
+            if isinstance(todo, expec) and todo.label != "":
+                value_dict[todo.label] = value_dict[todo_expec]
+
+        # Add x, param, and param_op to the dictionary as default
+        value_dict["x"] = x
+        value_dict["param"] = param
+        value_dict["param_op"] = param_op
+
+        # Store the updated dictionary for the theta value
+        if self._result_caching:
+            self.result_container[caching_tuple] = value_dict
+
+        return value_dict
+
+
+def _split_paulis(operator: OperatorBase, single_measure: bool) -> OperatorBase:
+    """
+    Split the opflow such that it can be measured in Z basis.
+
+    Splits up the opflow expression such that the meaurement operators can be evaluated
+    in the Z-basis. The routine is needed, if Y and X operators are present in the measurement
+
+    Args:
+        operator (OperatorBase) : Opflow expression that is checked
+        single_measure (bool): Is true if there is only a single
+            measurement in the opflow structure, otherwise a ListOp is considered
+    Returns:
+        New opflow expression where measurements are correctly split
+        into seprate circuits
+    """
+    # We reached a ComposedOp term -> seprate the different measurment operators
+    # using qiskit's PauliExpectation
+    if isinstance(operator, ComposedOp):
+        coeff = operator.coeff
+        operator_splitted = PauliExpectation().convert(operator)
+        operator_splitted._coeff = coeff
+        if single_measure == True:
+            return ListOp([operator_splitted])
+        else:
+            return operator_splitted
+
+    # We reached a CircuitStateFn term that should not be present in this routine
+    elif isinstance(operator, CircuitStateFn):
+        raise ValueError("CircuitStateFn type is not allowed!")
+
+    # We reached a list of opflow terms, recursive call of
+    # the function to all children in the list
+    elif isinstance(operator, ListOp):
+        op_list = [_split_paulis(op, single_measure) for op in operator.oplist]
+        if isinstance(operator, SummedOp):
+            return SummedOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, TensoredOp):
+            return TensoredOp(
+                oplist=[op for op in op_list if op != ~Zero @ One], coeff=operator.coeff
+            )
+        elif isinstance(operator, real_ListOp):
+            return ListOp(
+                oplist=[op for op in op_list if op != ~Zero @ One],
+                coeff=operator.coeff,
+                combo_fn=operator.combo_fn,
+            )
+        else:
+            raise ValueError("Unknown ListOp type in _split_paulis:", type(operator))
+    else:
+        raise ValueError("Unknown type in _split_paulis:", type(operator))
```

### Comparing `squlearn-0.1.0/src/squlearn/util/data_preprocessing.py` & `squlearn-0.2.0/src/squlearn/util/data_preprocessing.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import numpy as np
-
-
-def assign_all_parameters(
-    opflow,
-    x=None,
-    param=None,
-    param_op=None,
-    x_values=None,
-    param_values=None,
-    param_op_values=None,
-):
-    """
-    Assigns circuit parameters
-    """
-
-    todo_list = []  # list for the variables
-    multi_list = []  # list of return ListOp or no list
-    param_list = []  # list of parameters that are substituted
-
-    # check shape of the x and adjust to [[]] form if necessary
-    if x is not None:
-        xx, multi_x = adjust_input(x_values, len(x))
-        todo_list.append(xx)
-        param_list.append(x)
-        multi_list.append(multi_x)
-    if param is not None:
-        pp, multi_p = adjust_input(param_values, len(param))
-        todo_list.append(pp)
-        param_list.append(param)
-        multi_list.append(multi_p)
-    if param_op is not None:
-        pp_op, multi_op = adjust_input(param_op_values, len(param_op))
-        todo_list.append(pp_op)
-        param_list.append(param_op)
-        multi_list.append(multi_op)
-
-    # Recursive construction of the assignment dictionary and list structure
-    def rec_assign(dic, todo_list, param_list, multi_list):
-        if len(todo_list) <= 0:
-            return None
-        return_list = []
-        for x_ in todo_list[0]:
-            for A, B in zip(param_list[0], x_):
-                dic[A] = B
-            if len(multi_list[1:]) > 0:
-                return_list.append(
-                    rec_assign(dic.copy(), todo_list[1:], param_list[1:], multi_list[1:])
-                )
-            else:
-                return_list.append(opflow.assign_parameters(dic))
-
-        if multi_list[0]:
-            from qiskit.opflow import ListOp
-
-            return ListOp(return_list)
-        else:
-            return return_list[0]
-
-    return rec_assign({}, todo_list, param_list, multi_list)
-
-
-def adjust_input(x, x_length: int):
-    # check shape of the x and adjust to [[]] form if necessary
-    multiple_inputs = False
-    error = False
-    shape = np.shape(x)
-    if shape == () and x_length == 1:
-        # Single floating point number
-        xx = np.array([[x]])
-    elif len(shape) == 1:
-        if x_length == 1:
-            xx = np.array([np.array([xx]) for xx in x])
-            multiple_inputs = True
-        else:
-            # We have a single multi dimensional x (e.g. parameter vector)
-            if len(x) == x_length:
-                xx = np.array([x])
-            else:
-                error = True
-    elif len(shape) == 2:
-        if shape[1] == x_length:
-            xx = x
-            multiple_inputs = True
-        else:
-            error = True
-    else:
-        error = True
-
-    if error:
-        raise ValueError("Wrong format of an input variable.")
-
-    return xx, multiple_inputs
+import numpy as np
+
+
+def assign_all_parameters(
+    opflow,
+    x=None,
+    param=None,
+    param_op=None,
+    x_values=None,
+    param_values=None,
+    param_op_values=None,
+):
+    """
+    Assigns circuit parameters
+    """
+
+    todo_list = []  # list for the variables
+    multi_list = []  # list of return ListOp or no list
+    param_list = []  # list of parameters that are substituted
+
+    # check shape of the x and adjust to [[]] form if necessary
+    if x is not None:
+        xx, multi_x = adjust_input(x_values, len(x))
+        todo_list.append(xx)
+        param_list.append(x)
+        multi_list.append(multi_x)
+    if param is not None:
+        pp, multi_p = adjust_input(param_values, len(param))
+        todo_list.append(pp)
+        param_list.append(param)
+        multi_list.append(multi_p)
+    if param_op is not None:
+        pp_op, multi_op = adjust_input(param_op_values, len(param_op))
+        todo_list.append(pp_op)
+        param_list.append(param_op)
+        multi_list.append(multi_op)
+
+    # Recursive construction of the assignment dictionary and list structure
+    def rec_assign(dic, todo_list, param_list, multi_list):
+        if len(todo_list) <= 0:
+            return None
+        return_list = []
+        for x_ in todo_list[0]:
+            for A, B in zip(param_list[0], x_):
+                dic[A] = B
+            if len(multi_list[1:]) > 0:
+                return_list.append(
+                    rec_assign(dic.copy(), todo_list[1:], param_list[1:], multi_list[1:])
+                )
+            else:
+                return_list.append(opflow.assign_parameters(dic))
+
+        if multi_list[0]:
+            from qiskit.opflow import ListOp
+
+            return ListOp(return_list)
+        else:
+            return return_list[0]
+
+    return rec_assign({}, todo_list, param_list, multi_list)
+
+
+def adjust_input(x, x_length: int):
+    # check shape of the x and adjust to [[]] form if necessary
+    multiple_inputs = False
+    error = False
+    shape = np.shape(x)
+    if shape == () and x_length == 1:
+        # Single floating point number
+        xx = np.array([[x]])
+    elif len(shape) == 1:
+        if x_length == 1:
+            xx = np.array([np.array([xx]) for xx in x])
+            multiple_inputs = True
+        else:
+            # We have a single multi dimensional x (e.g. parameter vector)
+            if len(x) == x_length:
+                xx = np.array([x])
+            else:
+                error = True
+    elif len(shape) == 2:
+        if shape[1] == x_length:
+            xx = x
+            multiple_inputs = True
+        else:
+            error = True
+    else:
+        error = True
+
+    if error:
+        raise ValueError("Wrong format of an input variable.")
+
+    return xx, multiple_inputs
```

### Comparing `squlearn-0.1.0/src/squlearn/util/evaluate_opflow.py` & `squlearn-0.2.0/src/squlearn/util/evaluate_opflow.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,262 +1,320 @@
-from qiskit.opflow import CircuitSampler
-from qiskit.opflow import OperatorBase
-from qiskit.opflow import StateFn, CircuitStateFn, OperatorStateFn, DictStateFn
-from qiskit.opflow import SummedOp, ComposedOp
-from qiskit.opflow import ListOp
-from functools import partial
-import numpy as np
-import time
-
-
-def evaluate_opflow_qi_slow(QuantumInstance, opflow):
-    Sampler = CircuitSampler(QuantumInstance, caching="last")
-    Sampler._transpile_before_bind = False
-    eval_conv = Sampler.convert(opflow)
-    return np.real(eval_conv.eval())
-
-
-def evaluate_opflow_qi(QuantumInstance, opflow, mitigation_func=None):
-    # build a list of circuits which have to be executed
-    circuit_list = []
-
-    def build_circuit_list(operator: OperatorBase) -> None:
-        if isinstance(operator, CircuitStateFn):
-            if QuantumInstance.is_statevector:
-                circuit_list.append(operator.to_circuit(meas=False))
-            else:
-                circuit_list.append(operator.to_circuit(meas=True))
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_circuit_list(op)
-
-    build_circuit_list(opflow)
-
-    # build a list in the same order as circuit containing the associated operators
-    CircuitStateFn_list = []
-
-    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
-        if isinstance(operator, CircuitStateFn):
-            CircuitStateFn_list.append(operator)
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_CircuitStateFn_list(op)
-
-    build_CircuitStateFn_list(opflow)
-
-    # Execute circuits
-    start = time.time()
-    results = QuantumInstance.execute(circuit_list, had_transpiled=True)
-    #print("exec:", time.time() - start)
-
-    # build StateFns from the results (copied from qiskit source code)
-    sampled_statefn_dicts = {}
-    for i, op_c in enumerate(CircuitStateFn_list):
-        # Taking square root because we're replacing a statevector
-        # representation of probabilities.
-
-        circ_results = results.data(i)
-
-        if "expval_measurement" in circ_results:
-            avg = circ_results["expval_measurement"]
-            # Will be replaced with just avg when eval is called later
-            num_qubits = opflow[0].num_qubits
-            result_sfn = DictStateFn(
-                "0" * num_qubits,
-                coeff=avg * op_c.coeff,
-                is_measurement=op_c.is_measurement,
-                from_operator=op_c.from_operator,
-            )
-        elif QuantumInstance.is_statevector:
-            result_sfn = StateFn(
-                op_c.coeff * results.get_statevector(i),
-                is_measurement=op_c.is_measurement,
-            )
-        else:
-            QI_shots = QuantumInstance._run_config.shots
-
-            if mitigation_func is not None:
-                proba = mitigation_func(results.get_counts(i).items())
-            else:
-                proba = {b: (v / QI_shots) for (b, v) in results.get_counts(i).items()}
-            result_sfn = DictStateFn(
-                {b: np.abs(p) ** 0.5 * op_c.coeff for (b, p) in proba.items()},
-                is_measurement=op_c.is_measurement,
-                from_operator=op_c.from_operator,
-            )
-
-        sampled_statefn_dicts[id(op_c)] = result_sfn
-
-    def replace_circuits_with_dicts(operator):
-        if isinstance(operator, CircuitStateFn):
-            return sampled_statefn_dicts[id(operator)]
-        elif isinstance(operator, ListOp):
-            return operator.traverse(partial(replace_circuits_with_dicts))
-        else:
-            return operator
-
-    # Restore original opflow structure with evaluated StateFn
-    start = time.time()
-    eval_circs = replace_circuits_with_dicts(opflow)
-    return_val = np.real(eval_circs.eval())
-    #print("eval:", time.time() - start)
-
-    return return_val
-
-
-def evaluate_opflow_estimator(estimator, opflow):
-    # build a list of circuits which have to be executed
-    circuit_list = []
-    measure_list = []
-    repeat_list = []
-
-    def build_circuit_list(operator: OperatorBase) -> None:
-        if isinstance(operator, ComposedOp):
-            len_measure = 0
-            for op in operator.oplist:
-                if isinstance(op, ListOp):
-                    for op2 in op.oplist:
-                        measure_list.append(op2.primitive)
-                        len_measure = len_measure + 1
-                elif isinstance(op, OperatorStateFn):
-                    measure_list.append(op.primitive)
-                    len_measure = len_measure + 1
-            repeat_list.append(len_measure)
-            for op in operator.oplist:
-                if isinstance(op, CircuitStateFn):
-                    for i in range(len_measure):
-                        circuit_list.append(op.to_circuit(meas=False))
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_circuit_list(op)
-
-    build_circuit_list(opflow)
-
-    if len(measure_list) != len(circuit_list):
-        raise ValueError("Non-equal number of circuits and measurement operators!")
-
-    # build a list in the same order as circuit containing the associated operators
-    CircuitStateFn_list = []
-
-    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
-        if (
-            isinstance(operator, CircuitStateFn)
-            or isinstance(operator, ComposedOp)
-            or isinstance(operator, OperatorStateFn)
-        ):
-            CircuitStateFn_list.append(operator)
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_CircuitStateFn_list(op)
-
-    build_CircuitStateFn_list(opflow)
-
-    try:
-        start = time.time()
-        job = estimator.run(circuit_list, measure_list)
-        #print("exec:", time.time() - start)
-        job_result = job.result()
-    except:
-        # second try
-        start = time.time()
-        job = estimator.run(circuit_list, measure_list)
-        #print("exec:", time.time() - start)
-        job_result = job.result()
-
-    sampled_statefn_dicts = {}
-
-    repeat_list2 = []
-    ioff = 0
-    for i in range(len(repeat_list) - 1):
-        ioff = ioff + repeat_list[i]
-        repeat_list2.append(ioff)
-    values = np.split(job_result.values, repeat_list2)
-
-    for i, op_c in enumerate(CircuitStateFn_list):
-        sampled_statefn_dicts[id(op_c)] = values[i]
-
-    def replace_circuits_with_dicts(operator):
-        if (
-            isinstance(operator, CircuitStateFn)
-            or isinstance(operator, ComposedOp)
-            or isinstance(operator, OperatorStateFn)
-        ):
-            return sampled_statefn_dicts[id(operator)] * operator.coeff
-        elif isinstance(operator, ListOp):
-            value_list = np.array([replace_circuits_with_dicts(op) for op in operator.oplist])
-            if isinstance(operator, SummedOp):
-                return np.sum(value_list, axis=0) * operator.coeff
-            else:
-                return np.array(value_list) * operator.coeff
-        else:
-            raise RuntimeError("Wrong operator in result list!")
-
-    return_val = replace_circuits_with_dicts(opflow)
-    return return_val
-
-
-def evaluate_opflow_sampler(sampler, opflow):
-    # build a list of circuits which have to be executed
-    circuit_list = []
-
-    def build_circuit_list(operator: OperatorBase) -> None:
-        if isinstance(operator, CircuitStateFn):
-            circuit_list.append(operator.to_circuit(meas=True))
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_circuit_list(op)
-
-    build_circuit_list(opflow)
-
-    # build a list in the same order as circuit containing the associated operators
-    CircuitStateFn_list = []
-
-    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
-        if isinstance(operator, CircuitStateFn):
-            CircuitStateFn_list.append(operator)
-        elif isinstance(operator, ListOp):
-            for op in operator.oplist:
-                build_CircuitStateFn_list(op)
-
-    build_CircuitStateFn_list(opflow)
-
-    # Execute circuits
-    try:
-        start = time.time()
-        job = sampler.run(circuit_list)
-        results = job.result()
-        #print("exec:", time.time() - start)
-    except:
-        # second try
-        start = time.time()
-        job = sampler.run(circuit_list)
-        results = job.result()
-        #print("exec:", time.time() - start)
-
-    # build StateFns from the results (copied from qiskit source code)
-    sampled_statefn_dicts = {}
-    for i, op_c in enumerate(CircuitStateFn_list):
-        # Taking square root because we're replacing a statevector
-        # representation of probabilities.
-        circ_results = results.quasi_dists[i]
-        proba = circ_results.binary_probabilities()
-        result_sfn = DictStateFn(
-            {b: np.abs(p) ** 0.5 * op_c.coeff for (b, p) in proba.items()},
-            is_measurement=op_c.is_measurement,
-            from_operator=op_c.from_operator,
-        )
-        sampled_statefn_dicts[id(op_c)] = result_sfn
-
-    def replace_circuits_with_dicts(operator):
-        if isinstance(operator, CircuitStateFn):
-            return sampled_statefn_dicts[id(operator)]
-        elif isinstance(operator, ListOp):
-            return operator.traverse(partial(replace_circuits_with_dicts))
-        else:
-            return operator
-
-    # Restore original opflow structure with evaluated StateFn
-    start = time.time()
-    eval_circs = replace_circuits_with_dicts(opflow)
-    return_val = np.real(eval_circs.eval())
-    #print("eval:", time.time() - start)
-    return return_val
+from qiskit.opflow import CircuitSampler
+from qiskit.opflow import OperatorBase
+from qiskit.opflow import StateFn, CircuitStateFn, OperatorStateFn, DictStateFn
+from qiskit.opflow import SummedOp, ComposedOp
+from qiskit.opflow import ListOp
+from functools import partial
+import numpy as np
+import time
+
+from qiskit.primitives import Estimator as qiskit_primitives_Estimator
+from qiskit.primitives import BackendEstimator as qiskit_primitives_BackendEstimator
+from qiskit.primitives import Sampler as qiskit_primitives_Sampler
+from qiskit.primitives import BackendSampler as qiskit_primitives_BackendSampler
+
+
+def evaluate_opflow_qi_slow(QuantumInstance, opflow):
+    Sampler = CircuitSampler(QuantumInstance, caching="last")
+    Sampler._transpile_before_bind = False
+    eval_conv = Sampler.convert(opflow)
+    return np.real(eval_conv.eval())
+
+
+def evaluate_opflow_qi(QuantumInstance, opflow, mitigation_func=None):
+    # build a list of circuits which have to be executed
+    circuit_list = []
+
+    def build_circuit_list(operator: OperatorBase) -> None:
+        if isinstance(operator, CircuitStateFn):
+            if QuantumInstance.is_statevector:
+                circuit_list.append(operator.to_circuit(meas=False))
+            else:
+                circuit_list.append(operator.to_circuit(meas=True))
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_circuit_list(op)
+
+    build_circuit_list(opflow)
+
+    # build a list in the same order as circuit containing the associated operators
+    CircuitStateFn_list = []
+
+    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
+        if isinstance(operator, CircuitStateFn):
+            CircuitStateFn_list.append(operator)
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_CircuitStateFn_list(op)
+
+    build_CircuitStateFn_list(opflow)
+
+    # Execute circuits
+    start = time.time()
+    results = QuantumInstance.execute(circuit_list, had_transpiled=True)
+    # print("exec:", time.time() - start)
+
+    # build StateFns from the results (copied from qiskit source code)
+    sampled_statefn_dicts = {}
+    for i, op_c in enumerate(CircuitStateFn_list):
+        # Taking square root because we're replacing a statevector
+        # representation of probabilities.
+
+        circ_results = results.data(i)
+
+        if "expval_measurement" in circ_results:
+            avg = circ_results["expval_measurement"]
+            # Will be replaced with just avg when eval is called later
+            num_qubits = opflow[0].num_qubits
+            result_sfn = DictStateFn(
+                "0" * num_qubits,
+                coeff=avg * op_c.coeff,
+                is_measurement=op_c.is_measurement,
+                from_operator=op_c.from_operator,
+            )
+        elif QuantumInstance.is_statevector:
+            result_sfn = StateFn(
+                op_c.coeff * results.get_statevector(i),
+                is_measurement=op_c.is_measurement,
+            )
+        else:
+            QI_shots = QuantumInstance._run_config.shots
+
+            if mitigation_func is not None:
+                proba = mitigation_func(results.get_counts(i).items())
+            else:
+                proba = {b: (v / QI_shots) for (b, v) in results.get_counts(i).items()}
+            result_sfn = DictStateFn(
+                {b: np.abs(p) ** 0.5 * op_c.coeff for (b, p) in proba.items()},
+                is_measurement=op_c.is_measurement,
+                from_operator=op_c.from_operator,
+            )
+
+        sampled_statefn_dicts[id(op_c)] = result_sfn
+
+    def replace_circuits_with_dicts(operator):
+        if isinstance(operator, CircuitStateFn):
+            return sampled_statefn_dicts[id(operator)]
+        elif isinstance(operator, ListOp):
+            return operator.traverse(partial(replace_circuits_with_dicts))
+        else:
+            return operator
+
+    # Restore original opflow structure with evaluated StateFn
+    start = time.time()
+    eval_circs = replace_circuits_with_dicts(opflow)
+    return_val = np.real(eval_circs.eval())
+    # print("eval:", time.time() - start)
+
+    return return_val
+
+
+def evaluate_opflow_estimator(estimator, opflow):
+    from .executor import ExecutorEstimator
+
+    # build a list of circuits which have to be executed
+    circuit_list = []
+    measure_list = []
+    repeat_list = []
+
+    def build_circuit_list(operator: OperatorBase) -> None:
+        if isinstance(operator, ComposedOp):
+            len_measure = 0
+            for op in operator.oplist:
+                if isinstance(op, ListOp):
+                    for op2 in op.oplist:
+                        measure_list.append(op2.primitive)
+                        len_measure = len_measure + 1
+                elif isinstance(op, OperatorStateFn):
+                    measure_list.append(op.primitive)
+                    len_measure = len_measure + 1
+            repeat_list.append(len_measure)
+            for op in operator.oplist:
+                if isinstance(op, CircuitStateFn):
+                    for i in range(len_measure):
+                        circuit_list.append(op.to_circuit(meas=False))
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_circuit_list(op)
+
+    build_circuit_list(opflow)
+
+    if len(measure_list) != len(circuit_list):
+        raise ValueError("Non-equal number of circuits and measurement operators!")
+
+    # build a list in the same order as circuit containing the associated operators
+    CircuitStateFn_list = []
+
+    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
+        if (
+            isinstance(operator, CircuitStateFn)
+            or isinstance(operator, ComposedOp)
+            or isinstance(operator, OperatorStateFn)
+        ):
+            CircuitStateFn_list.append(operator)
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_CircuitStateFn_list(op)
+
+    build_CircuitStateFn_list(opflow)
+
+    try:
+        start = time.time()
+        job = estimator.run(circuit_list, measure_list)
+        # print("exec:", time.time() - start)
+        job_result = job.result()
+
+        # Clear cache of estimator, otherwise memory leak
+        if isinstance(estimator, qiskit_primitives_Estimator) or isinstance(
+            estimator, qiskit_primitives_BackendEstimator
+        ):
+            estimator._circuits = []
+            estimator._observables = []
+            estimator._parameters = []
+            estimator._circuit_ids = {}
+            estimator._observable_ids = {}
+
+        elif isinstance(estimator, ExecutorEstimator):
+            estimator.clear_cache()
+
+    except:
+        # second try
+        start = time.time()
+        job = estimator.run(circuit_list, measure_list)
+        # print("exec:", time.time() - start)
+        job_result = job.result()
+
+        # Clear cache of estimator, otherwise memory leak
+        if isinstance(estimator, qiskit_primitives_Estimator) or isinstance(
+            estimator, qiskit_primitives_BackendEstimator
+        ):
+            estimator._circuits = []
+            estimator._observables = []
+            estimator._parameters = []
+            estimator._circuit_ids = {}
+            estimator._observable_ids = {}
+
+        elif isinstance(estimator, ExecutorEstimator):
+            estimator.clear_cache()
+
+    sampled_statefn_dicts = {}
+
+    repeat_list2 = []
+    ioff = 0
+    for i in range(len(repeat_list) - 1):
+        ioff = ioff + repeat_list[i]
+        repeat_list2.append(ioff)
+    values = np.split(job_result.values, repeat_list2)
+
+    for i, op_c in enumerate(CircuitStateFn_list):
+        sampled_statefn_dicts[id(op_c)] = values[i]
+
+    def replace_circuits_with_dicts(operator):
+        if (
+            isinstance(operator, CircuitStateFn)
+            or isinstance(operator, ComposedOp)
+            or isinstance(operator, OperatorStateFn)
+        ):
+            return sampled_statefn_dicts[id(operator)] * operator.coeff
+        elif isinstance(operator, ListOp):
+            value_list = np.array([replace_circuits_with_dicts(op) for op in operator.oplist])
+            if isinstance(operator, SummedOp):
+                return np.sum(value_list, axis=0) * operator.coeff
+            else:
+                return np.array(value_list) * operator.coeff
+        else:
+            raise RuntimeError("Wrong operator in result list!")
+
+    return_val = replace_circuits_with_dicts(opflow)
+    return return_val
+
+
+def evaluate_opflow_sampler(sampler, opflow):
+    from .executor import ExecutorSampler
+
+    # build a list of circuits which have to be executed
+    circuit_list = []
+
+    def build_circuit_list(operator: OperatorBase) -> None:
+        if isinstance(operator, CircuitStateFn):
+            circuit_list.append(operator.to_circuit(meas=True))
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_circuit_list(op)
+
+    build_circuit_list(opflow)
+
+    # build a list in the same order as circuit containing the associated operators
+    CircuitStateFn_list = []
+
+    def build_CircuitStateFn_list(operator: OperatorBase) -> None:
+        if isinstance(operator, CircuitStateFn):
+            CircuitStateFn_list.append(operator)
+        elif isinstance(operator, ListOp):
+            for op in operator.oplist:
+                build_CircuitStateFn_list(op)
+
+    build_CircuitStateFn_list(opflow)
+
+    # Execute circuits
+    try:
+        start = time.time()
+        job = sampler.run(circuit_list)
+        results = job.result()
+
+        # Clear cache of estimator, otherwise memory leak
+        if isinstance(sampler, qiskit_primitives_Sampler) or isinstance(
+            sampler, qiskit_primitives_BackendSampler
+        ):
+            sampler._circuits = []
+            sampler._parameters = []
+            sampler._circuit_ids = {}
+            sampler._qargs_list = []
+
+        elif isinstance(sampler, ExecutorSampler):
+            sampler.clear_cache()
+
+    except:
+        start = time.time()
+        job = sampler.run(circuit_list)
+        results = job.result()
+
+        # Clear cache of estimator, otherwise memory leak
+        if isinstance(sampler, qiskit_primitives_Sampler) or isinstance(
+            sampler, qiskit_primitives_BackendSampler
+        ):
+            sampler._circuits = []
+            sampler._parameters = []
+            sampler._circuit_ids = {}
+            sampler._qargs_list = []
+
+        elif isinstance(sampler, ExecutorSampler):
+            sampler.clear_cache()
+
+    # build StateFns from the results (copied from qiskit source code)
+    sampled_statefn_dicts = {}
+    for i, op_c in enumerate(CircuitStateFn_list):
+        # Taking square root because we're replacing a statevector
+        # representation of probabilities.
+        circ_results = results.quasi_dists[i]
+        proba = circ_results.binary_probabilities()
+        result_sfn = DictStateFn(
+            {b: np.abs(p) ** 0.5 * op_c.coeff for (b, p) in proba.items()},
+            is_measurement=op_c.is_measurement,
+            from_operator=op_c.from_operator,
+        )
+        sampled_statefn_dicts[id(op_c)] = result_sfn
+
+    def replace_circuits_with_dicts(operator):
+        if isinstance(operator, CircuitStateFn):
+            return sampled_statefn_dicts[id(operator)]
+        elif isinstance(operator, ListOp):
+            return operator.traverse(partial(replace_circuits_with_dicts))
+        else:
+            return operator
+
+    # Restore original opflow structure with evaluated StateFn
+    start = time.time()
+    eval_circs = replace_circuits_with_dicts(opflow)
+    return_val = np.real(eval_circs.eval())
+    # print("eval:", time.time() - start)
+    return return_val
```

### Comparing `squlearn-0.1.0/src/squlearn/util/executor.py` & `squlearn-0.2.0/src/squlearn/util/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,1092 +1,1116 @@
-import logging
-from logging.handlers import RotatingFileHandler
-from logging import handlers
-import copy
-from pathlib import Path
-from hashlib import blake2b
-from typing import Any, Union
-import traceback
-from dataclasses import asdict
-
-import dill as pickle
-
-from qiskit.primitives import Estimator as qiskit_primitives_Estimator
-from qiskit.primitives import BackendEstimator as qiskit_primitives_BackendEstimator
-from qiskit.primitives import Sampler as qiskit_primitives_Sampler
-from qiskit.primitives import BackendSampler as qiskit_primitives_BackendSampler
-from qiskit.primitives import BaseEstimator, BaseSampler
-from qiskit.primitives.base import SamplerResult, EstimatorResult
-from qiskit.utils import QuantumInstance
-from qiskit import Aer
-from qiskit_ibm_runtime import QiskitRuntimeService, Session
-from qiskit.opflow import OperatorBase
-from qiskit.providers import Options
-from qiskit.providers import JobV1 as Job
-from qiskit.providers.backend import Backend
-from qiskit.providers.jobstatus import JobStatus, JOB_FINAL_STATES
-from qiskit_ibm_runtime import Estimator as qiskit_ibm_runtime_Estimator
-from qiskit_ibm_runtime import Sampler as qiskit_ibm_runtime_Sampler
-from qiskit_ibm_runtime.exceptions import IBMRuntimeError, RuntimeJobFailureError
-from qiskit_ibm_runtime.options import Options as qiskit_ibm_runtime_Options
-
-from .evaluate_opflow import *
-
-
-class Executor:
-    """
-    Executor class to run Qiskit jobs on IBM Quantum systems or simulators.
-
-    The Executor class is a wrapper around the Qiskit Runtime service, simulators, and primitives
-    Sessions and primitves are automatically created and managed by the Executor class.
-    Results can be cached to avoid re-running the same jobs.
-
-    Args:
-        execution (Union[str, Backend, QuantumInstance, QiskitRuntimeService, Session,
-            BaseEstimator, BaseSampler]): The execution environment, it can be:
-            - A string, that specifics the simulator backend, e.g. 'qasm_simulator'.
-            - A Qiskit backend, to run the jobs on IBM Quantum systems or simulators.
-            - A QuantumInstance, that includes the backend and some options.
-            - A QiskitRuntimeService, to run the jobs on the Qiskit Runtime service.
-                The backend has to be provided separately.
-            - A Session, to run the jobs on the Qiskit Runtime service.
-            - A Estimator primitive (either simulator or Qiskit Runtime primitive)
-            - A Sampler primitive (either simulator or Qiskit Runtime primitive)
-        backend (Optional[Backend]): The backend to run the jobs on.
-            It is only used  if execution is a service.
-        options_estimator (Optional[Options]): The options for the created estimator primitives.
-        options_sampler (Optional[Options]): The options for the created sampler primitives.
-        log_file (str): The name of the log file, if empty, no log file is created.
-        caching (Optional[bool]): Whether to cache the results of the jobs.
-        cache_dir (str): The directory where to cache the results of the jobs.
-        max_session_time (str): The maximum time for a session, similar input as in qiskit.
-        max_jobs_retries (int): The maximum number of retries for a job
-            until the execution is aborted.
-        wait_restart (int): The time to wait before restarting a job in seconds.
-
-    """
-
-    def __init__(
-        self,
-        execution: Union[
-            str,
-            Backend,
-            QuantumInstance,
-            QiskitRuntimeService,
-            Session,
-            BaseEstimator,
-            BaseSampler,
-        ],
-        backend=None,
-        options_estimator=None,
-        options_sampler=None,
-        log_file="",
-        caching=None,
-        cache_dir="_cache",
-        max_session_time="8h",
-        max_jobs_retries=10,
-        wait_restart=1,
-    ) -> None:
-        # Default values for internal variables
-        self._backend = None
-        self._session = None
-        self._service = None
-        self._estimator = None
-        self._sampler = None
-        self._quantum_instance = None
-        self._remote = False
-        self._session_active = False
-        self._execution_origin = ""
-
-        # Copy estimator options and make a dict
-        self._options_estimator = options_estimator
-        if self._options_estimator is None:
-            self._options_estimator = {}
-
-        # Copy sampler options and make a dict
-        self._options_sampler = options_sampler
-        if self._options_sampler is None:
-            self._options_sampler = {}
-
-        # Copy Executor options
-        self._log_file = log_file
-        self._caching = caching
-        self._max_session_time = max_session_time
-        self._max_jobs_retries = max_jobs_retries
-        self._wait_restart = wait_restart
-
-        if self._log_file != "":
-            fh = handlers.RotatingFileHandler(
-                self._log_file, maxBytes=(1048576 * 5), backupCount=100
-            )
-            log_format = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
-            fh.setFormatter(log_format)
-            self._logger = logging.getLogger("executor")
-            self._logger.addHandler(fh)
-            self._logger.setLevel(logging.INFO)
-        else:
-            self._logger = logging.getLogger("executor")
-            self._logger.setLevel(logging.INFO)
-
-        if execution is None and backend is not None:
-            # Only backend is given
-            execution = backend
-
-        if isinstance(execution, str):
-            # Execution is a string -> get backend
-            if execution == "statevector_simulator":
-                self._backend = Aer.get_backend(execution)
-            elif execution == "qasm_simulator":
-                self._backend = Aer.get_backend(execution)
-            elif "ibm" in execution:
-                raise ValueError(
-                    "IBM backend are not supported by string input, since credentials are missing "
-                    + execution
-                )
-            else:
-                raise ValueError("Unknown backend string: " + execution)
-            self._execution_origin = "Simulator"
-        elif isinstance(execution, Backend):
-            # Execution is a backend class
-            if hasattr(execution, "service"):
-                self._service = execution.service
-            self._backend = execution
-            self._execution_origin = "Backend"
-        elif isinstance(execution, QuantumInstance):
-            # Execution is a QuantumInstance
-            self._quantum_instance = execution
-            self._backend = execution.backend
-            self._execution_origin = "QuantumInstance"
-        elif isinstance(execution, QiskitRuntimeService):
-            self._service = execution
-            if isinstance(backend, str):
-                self._backend = self._service.get_backend(backend)
-            elif isinstance(backend, Backend):
-                self._backend = backend
-            elif backend is None:
-                raise ValueError("Backend has to be specified for QiskitRuntimeService")
-            else:
-                raise ValueError("Unknown backend type: " + backend)
-            self._execution_origin = "QiskitRuntimeService"
-        elif isinstance(execution, Session):
-            # Execution is a active? session
-            self._session = execution
-            self._service = self._session.service
-            self._backend = self._session.service.get_backend(self._session.backend())
-            self._session_active = True
-            self._execution_origin = "Session"
-        elif isinstance(execution, BaseEstimator):
-            self._estimator = execution
-            if isinstance(self._estimator, qiskit_primitives_Estimator):
-                # this is only a hack, there is no real backend in the Primitive Estimator class
-                self._backend = Aer.get_backend("statevector_simulator")
-            elif isinstance(self._estimator, qiskit_primitives_BackendEstimator):
-                self._backend = self._estimator._backend
-            # Real Backend
-            elif hasattr(self._estimator, "session"):
-                self._session = self._estimator.session
-                self._service = self._estimator.session.service
-                self._backend = self._estimator.session.service.get_backend(
-                    self._estimator.session.backend()
-                )
-                self._session_active = True
-            else:
-                raise RuntimeError("No backend found in the given Estimator Primitive!")
-
-            if self._options_estimator is None:
-                self._options_estimator = self._estimator.options
-            else:
-                self._estimator.options.update_options(**self._options_estimator)
-            self._execution_origin = "Estimator"
-        elif isinstance(execution, BaseSampler):
-            self._sampler = execution
-
-            if isinstance(self._sampler, qiskit_primitives_Sampler):
-                # this is only a hack, there is no real backend in the Primitive Sampler class
-                self._backend = Aer.get_backend("statevector_simulator")
-            elif isinstance(self._sampler, qiskit_primitives_BackendSampler):
-                self._backend = self._sampler._backend
-            elif hasattr(self._sampler, "session"):
-                self._session = self._sampler.session
-                self._service = self._sampler.session.service
-                self._backend = self._sampler.session.service.get_backend(
-                    self._sampler.session.backend()
-                )
-                self._session_active = True
-            else:
-                raise RuntimeError("No backend found in the given Sampler Primitive!")
-
-            if self._options_sampler is None:
-                self._options_sampler = self._sampler.options
-            else:
-                self._sampler.options.update_options(**self._options_sampler)
-            self._execution_origin = "Sampler"
-        else:
-            raise ValueError("Unknown execution type: " + str(type(execution)))
-
-        # Check if execution is on a remote IBM backend
-        if "ibm" in str(self._backend):
-            self._remote = True
-        else:
-            self._remote = False
-
-        self._inital_num_shots = self.get_shots()
-
-        if self._caching is None:
-            self._caching = self._remote
-
-        if self._caching:
-            self._cache = ExecutorCache(self._logger,cache_dir)
-
-        self._logger.info(f"Executor initialized with backend: {{}}".format(self._backend))
-        self._logger.info(f"Executor initialized with service: {{}}".format(self._service))
-        if self._session is not None:
-            self._logger.info(
-                f"Executor initialized with session: {{}}".format(self._session.session_id)
-            )
-        else:
-            self._logger.info(f"Executor initialized with session: {{}}".format(self._session))
-        self._logger.info(f"Executor initialized with estimator: {{}}".format(self._estimator))
-        self._logger.info(f"Executor initialized with sampler: {{}}".format(self._sampler))
-        self._logger.info(
-            f"Executor initialized with quantum instance: {{}}".format(self._quantum_instance)
-        )
-        self._logger.info(f"Executor intial shots: {{}}".format(self._inital_num_shots))
-
-    @property
-    def execution(self) -> str:
-        """Returns a string that of the executor that is used initializing the executor class."""
-        return self._execution_origin
-
-    @property
-    def backend(self):
-        """Returns the backend that is used for the execution."""
-        return self._backend
-
-    @property
-    def session(self):
-        """Returns the session that is used for the execution."""
-        return self._session
-
-    @property
-    def service(self):
-        """Returns the service that is used for the execution."""
-        return self._service
-
-    @property
-    def estimator(self):
-        """Returns the estimator primitive that is used for the execution.
-
-        This function created automatically estimators and checks for an expired session and
-        creates a new one if necessary.
-
-        The estimator that is created depends on the backend that is used for the execution.
-        """
-        if self._estimator is not None:
-            if self._session is not None and self._session_active is False:
-                # Session is expired, create a new session and a new estimator
-                self.create_session()
-                self._estimator = qiskit_ibm_runtime_Estimator(
-                    session=self._session, options=self._options_estimator
-                )
-            estimator = self._estimator
-        else:
-            # Create a new Estimator
-            shots = self.get_shots()
-            if self._session is not None:
-                if self._session_active is False:
-                    self.create_session()
-                self._estimator = qiskit_ibm_runtime_Estimator(
-                    session=self._session, options=self._options_estimator
-                )
-            elif self._service is not None:
-                # No session but service -> create a new session
-                self.create_session()
-                self._estimator = qiskit_ibm_runtime_Estimator(
-                    session=self._session, options=self._options_estimator
-                )
-            else:
-                if str(self._backend) == "statevector_simulator":
-                    # No session, no service, but state_vector simulator -> Estimator
-                    self._estimator = qiskit_primitives_Estimator(options=self._options_estimator)
-                else:
-                    # No session, no service and no state_vector simulator -> BackendEstimator
-                    self._estimator = qiskit_primitives_BackendEstimator(
-                        backend=self._backend, options=self._options_estimator
-                    )
-            if not self._options_estimator:
-                self.set_shots(shots)
-            estimator = self._estimator
-
-        return estimator
-
-    @property
-    def sampler(self):
-        """Returns the sampler primitive that is used for the execution.
-
-        This function created automatically estimators and checks for an expired session and
-        creates a new one if necessary.
-
-        The estimator that is created depends on the backend that is used for the execution.
-        """
-        if self._sampler is not None:
-            if self._session is not None and self._session_active is False:
-                # Session is expired, create a new one and a new estimator
-                self.create_session()
-                self._sampler = qiskit_ibm_runtime_Sampler(
-                    session=self._session, options=self._options_sampler
-                )
-            sampler = self._sampler
-        else:
-            # Create a new Sampler
-            shots = self.get_shots()
-            if self._session is not None:
-                if self._session_active is False:
-                    self.create_session()
-                self._sampler = qiskit_ibm_runtime_Sampler(
-                    session=self._session, options=self._options_sampler
-                )
-
-            elif self._service is not None:
-                # No session but service -> create a new session
-                self.create_session()
-                self._sampler = qiskit_ibm_runtime_Sampler(
-                    session=self._session,
-                    options=self._options_sampler,
-                )
-            else:
-                if str(self._backend) == "statevector_simulator":
-                    # No session, no service, but state_vector simulator -> Sampler
-                    self._sampler = qiskit_primitives_Sampler(options=self._options_sampler)
-                else:
-                    # No session, no service and no state_vector simulator -> BackendSampler
-                    self._sampler = qiskit_primitives_BackendSampler(
-                        backend=self._backend, options=self._options_sampler
-                    )
-            if not self._options_sampler:
-                self.set_shots(shots)
-            sampler = self._sampler
-
-        return sampler
-
-    @property
-    def quantum_instance(self):
-        """Returns the quantum instance that is used for the execution.
-
-        Creates a new one if none is set.
-        """
-
-        if self._quantum_instance is not None:
-            return self._quantum_instance
-        else:
-            self._quantum_instance = QuantumInstance(self._backend, shots=self.get_shots)
-            self._logger.info(
-                f"Executor created new QuantumInstance: {{}}".format(self._quantum_instance)
-            )
-            return self._quantum_instance
-
-    def _primitive_run(self, run, label: str, hash_value: Union[str, None] = None):
-        """Run function that allow restarting, session handling and caching.
-
-        Parent implementation that is used for Estimator and Sampler.
-
-        Args:
-            run (function): Function that is executed.
-            label (str): Label that is used for logging.
-            hash_value (str,None): Hash value that is used for caching.
-
-        Returns:
-            A qiskit job containing the results of the run.
-        """
-        success = False
-
-        for repeat in range(self._max_jobs_retries):
-            try:
-                job = None
-                cached = False
-                if hash_value is not None and self._caching:
-                    # TODO: except cache errors
-                    job = self._cache.get_file(hash_value)
-
-                if job is None:
-                    job = run()
-                    self._logger.info(
-                        f"Executor runs " + label + f" with job: {{}}".format(job.job_id())
-                    )
-                else:
-                    self._logger.info(f"Cached job found with hash value: {{}}".format(hash_value))
-                    cached = True
-
-            except IBMRuntimeError as e:
-                if '"code":1217' in e.message:
-                    self._logger.info(
-                        f"Executor failed to run "
-                        + label
-                        + f" because the session has been closed!"
-                    )
-                    self._session_active = False
-                    continue
-            except Exception as e:
-                self._logger.info(
-                    f"Executor failed to run " + label + f" because of unknown error!"
-                )
-                self._logger.info(f"Error message: {{}}".format(e))
-                self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
-                continue
-
-            # Wait for the job to complete
-            if not cached:
-                status = JobStatus.QUEUED
-                last_status = None
-            else:
-                status = JobStatus.DONE
-            while status not in JOB_FINAL_STATES:
-                try:
-                    status = job.status()
-                    if status != last_status:
-                        self._logger.info(f"Job status: {{}}".format(status))
-                    last_status = status
-                except Exception as e:
-                    self._logger.info(
-                        f"Executor failed to get job status because of unknown error!"
-                    )
-                    self._logger.info(f"Error message: {{}}".format(e))
-                    self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
-                    break
-
-                if self._remote:
-                    time.sleep(1)
-                else:
-                    time.sleep(0.01)
-
-            # Job is completed, check if it was successful
-            if status == JobStatus.ERROR:
-                self._logger.info(f"Failed executation of the job!")
-                self._logger.info(f"Error message: {{}}".format(job.error_message()))
-            elif status == JobStatus.CANCELLED:
-                self._logger.info(f"Throwing RuntimeError, since the job is manually canceled!")
-                raise RuntimeError(f"Job manually canceled!")
-            else:
-                success = True
-                result_success = False
-                for retry_result in range(3):
-                    # check if result is available
-                    try:
-                        result = job.result()
-                        result_success = True
-                    except RuntimeJobFailureError as e:
-                        self._logger.info(f"Executor unable to retriev job result!")
-                        self._logger.info(f"Error message: {{}}".format(e))
-                        self._logger.info(f"Error message: {{}}".format(e))
-                    except Exception as e:
-                        self._logger.info(
-                            f"Executor failed to get job result because of unknown error!"
-                        )
-                        self._logger.info(f"Error message: {{}}".format(e))
-                        self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
-                    if result_success:
-                        break
-                    else:
-                        self._logger.info(f"Retrying to get job result")
-                        time.sleep(self._wait_restart)
-
-            if success and result_success:
-                break
-            else:
-                self._logger.info(f"Restarting " + label + f" run")
-                success = False
-                result_success = False
-
-        if success is not True:
-            raise RuntimeError(
-                f"Could not run job successfully after {{}} retries".format(self._max_jobs_retries)
-            )
-
-        if self._caching and not cached:
-
-            job_pickle = copy.copy(job)
-            # remove _future and _function from job since this creates massive file sizes
-            # and the information is not really needed.
-            job_pickle._future = None
-            job_pickle._function = None
-            job_pickle._api_client = None
-            job_pickle._service = None
-            job_pickle._ws_client_future = None
-            job_pickle._ws_client = None
-            job_pickle._backend = str(job.backend())
-
-            # overwrite result function with the obtained result
-            def result_():
-                return result
-
-            job_pickle.result = result_
-            self._cache.store_file(hash_value, job_pickle)
-            self._logger.info(f"Stored job in cache with hash value: {{}}".format(hash_value))
-
-        return job
-
-    def estimator_run(self, circuits, observables, parameter_values=None, **kwargs: Any):
-        """
-        Function that overwrites the estimator run function.
-
-        Args:
-            circuits: Quantum circuits to execute.
-            observables: Observable to measure.
-            parameter_values: Values for the parameters in circuits.
-            kwargs (Any): Additional arguments that are passed to the estimator.
-
-        Returns:
-            A qiskit job containing the results of the run.
-        """
-
-        def run():
-            return self.estimator.run(circuits, observables, parameter_values, **kwargs)
-
-        if self._caching:
-            # Generate hash value for caching
-            hash_value = self._cache.hash_variable(
-                [
-                    "estimator",
-                    circuits,
-                    observables,
-                    parameter_values,
-                    kwargs,
-                    self._options_estimator,
-                    self._backend,
-                ]
-            )
-        else:
-            hash_value = None
-
-        return self._primitive_run(run, "estimator", hash_value)
-
-    def sampler_run(self, circuits, parameter_values=None, **kwargs: Any):
-        """
-        Function that overwrites the sampler run function.
-
-        Args:
-            circuits: Quantum circuits to execute.
-            parameter_values: Values for the parameters in circuits.
-            kwargs (Any): Additional arguments that are passed to the estimator.
-
-        Returns:
-            A qiskit job containing the results of the run.
-        """
-
-        def run():
-            return self.sampler.run(circuits, parameter_values, **kwargs)
-
-        if self._caching:
-            # Generate hash value for caching
-            hash_value = self._cache.hash_variable(
-                [
-                    "sampler",
-                    circuits,
-                    parameter_values,
-                    kwargs,
-                    self._options_sampler,
-                    self._backend,
-                ]
-            )
-        else:
-            hash_value = None
-
-        return self._primitive_run(run, "sampler", hash_value)
-
-    def get_estimator(self):
-        """
-        Returns a Estimator primitive that uses the Executor for running jobs.
-        Includes caching and automatic session handling.
-        """
-        return ExecutorEstimator(executor=self,options=self._options_estimator)
-
-    def get_sampler(self):
-        """
-        Returns a Sampler primitive that uses the Executor for running jobs.
-        Includes caching and automatic session handling.
-        """
-        return ExecutorSampler(executor=self,options=self._options_sampler)
-
-    def opflow_exec(self, opflow: OperatorBase):
-        """
-        Function for executing an opflow structur.
-
-        This function automatically detects if an estimator, sampler or quantum instance is set and uses
-        The emthod is very likely deprecated very soon.
-
-        Args:
-            opflow: Operator to evaluate.
-
-        Returns:
-            The evaluated opflow structure.
-        """
-        if self._estimator is not None:
-            return evaluate_opflow_estimator(self.get_estimator(), opflow)
-        elif self._sampler is not None:
-            return evaluate_opflow_sampler(self.get_sampler(), opflow)
-        elif self._quantum_instance is not None:
-            return evaluate_opflow_qi(self.quantum_instance, opflow)
-        else:  #  default if nothing is set -> use estimator
-            return evaluate_opflow_estimator(self.get_estimator(), opflow)
-
-    def get_opflow_executor(self) -> str:
-        """Returns a string that indicates which executor is used for opflow execution."""
-        if self._estimator is not None:
-            return "estimator"
-        elif self._sampler is not None:
-            return "sampler"
-        elif self._quantum_instance is not None:
-            return "quantum_instance"
-        else:  #  default if nothing is set -> use estimator
-            return "estimator"
-
-    def backend_run(self, circuits, **run_options: Any):
-        return self.backend.run(circuits, **run_options)
-
-    def set_shots(self, num_shots: Union[int, None]) -> None:
-        """Sets the number shots for the next evaluations.
-
-        Args:
-            num_shots (int or None): Number of shots that are set
-        """
-        if num_shots is None:
-            return None
-
-        if str(self._backend) == "statevector_simulator":
-            # Skip setting shots for statevector simulator
-            return None
-
-        # Update shots in estimator primitive
-        if self._estimator is not None:
-            try:
-                execution = self._estimator.options.get("execution")
-                execution["shots"] = num_shots
-                self._estimator.set_options(execution=execution)
-            except:
-                try:
-                    self._estimator.set_options(shots=num_shots)
-                except:
-                    pass
-
-        # Update shots in sampler primitive
-        if self._sampler is not None:
-            try:
-                execution = self._sampler.options.get("execution")
-                execution["shots"] = num_shots
-                self._sampler.set_options(execution=execution)
-            except:
-                try:
-                    self._sampler.set_options(shots=num_shots)
-                except:
-                    pass
-
-        # Update shots in estimator options for not yet created estimators
-        if self._options_estimator is not None:
-            try:
-                self._options_estimator["execution"]["shots"] = num_shots
-            except:
-                try:
-                    self._options_estimator["shots"] = num_shots
-                except:
-                    pass
-
-        # Update shots in sampler options for not yet created samplers
-        if self._options_sampler is not None:
-            try:
-                self._options_sampler["execution"]["shots"] = num_shots
-            except:
-                try:
-                    self._options_sampler["shots"] = num_shots
-                except:
-                    pass
-
-        # Upate shots in quantum instance
-        if self._quantum_instance is not None:
-            self._quantum_instance.set_config(shots=num_shots)
-
-        # Update shots in backend
-        if self._backend is not None:
-            self._backend.options.shots = num_shots
-
-        self._logger.info("Set shots to {}".format(num_shots))
-
-    def get_shots(self) -> int:
-        """Getter for the number of shots.
-
-        Returns:
-            Returns the number of shots that are used for the current evaluation."""
-        if self._estimator is not None or self._sampler is not None:
-            shots_estimator = 0
-            shots_sampler = 0
-            if self._estimator is not None:
-                try:
-                    execution = self._estimator.options.get("execution")
-                    shots_estimator = execution["shots"]
-                except:
-                    try:
-                        shots_estimator = self._estimator.options.get("shots", 0)
-                    except:
-                        shots_estimator = 0
-            if self._sampler is not None:
-                try:
-                    execution = self._sampler.options.get("execution")
-                    shots_sampler = execution["shots"]
-                except:
-                    try:
-                        shots_sampler = self._sampler.options.get("shots", 0)
-                    except:
-                        shots_sampler = 0
-
-            if self._estimator is not None and self._sampler is not None:
-                if shots_estimator != shots_sampler:
-                    raise ValueError(
-                        "The number of shots of the given \
-                                      Estimator and Sampler is not equal!"
-                    )
-
-            shots = max(shots_estimator, shots_sampler)
-
-        elif self._quantum_instance is not None:
-            shots = self._quantum_instance.run_config.shots
-        elif self._backend is not None:
-            shots = self._backend.options.shots
-        else:
-            return None  # No shots available
-
-        return shots
-
-    def reset_shots(self) -> None:
-        """Resets the shots to the initial values when the executor was created."""
-        self.set_shots(self._inital_num_shots)
-
-    def create_session(self):
-        """Creates a new session"""
-        if self._service is not None:
-            self._session = Session(
-                self._service, backend=self._backend, max_time=self._max_session_time
-            )
-            self._session_active = True
-            self._logger.info(f"Executor created a new session.")
-        else:
-            raise RuntimeError("Session can not started because of missing service!")
-
-    def close_session(self):
-        """Closes the current session"""
-        if self._session is not None:
-            self._logger.info(f"Executor closed session: {{}}".format(self._session.session_id))
-            self._session.close()
-            self._session = None
-        else:
-            raise RuntimeError("No session found!")
-
-    def __del__(self):
-        """Terminate the session in case the executor is deleted"""
-        if self._session is not None:
-            try:
-                self.close_session()
-            except:
-                pass
-
-
-class ExecutorEstimator(BaseEstimator):
-    """
-    Special Estimator Primitive that uses the Executor service.
-
-    Usefull for automatic restarting sessions and caching results.
-    The object is created by the Executor method get_estimator()
-
-    Args:
-        executor (Executor): The executor service to use
-        options: Options for the estimator
-
-    """
-
-    def __init__(self, executor: Executor, options=None):
-
-        if isinstance(options, Options) or isinstance(options, qiskit_ibm_runtime_Options):
-            options_ini = asdict(copy.deepcopy(options))
-        else:
-            options_ini = options
-
-        super().__init__(options=options_ini)
-        self._executor = executor
-
-    def _call(
-        self,
-        circuits,
-        observables,
-        parameter_values=None,
-        **run_options,
-    ) -> EstimatorResult:
-        """Has to be passed through, otherwise python will complain about the abstract method.
-        Input arguments are the same as in qiskit's estimator.call()
-        """
-        return self._executor.estimator._call(
-            circuits, observables, parameter_values, **run_options
-        )
-
-    def _run(
-        self,
-        circuits,
-        observables,
-        parameter_values,
-        **run_options,
-    ) -> Job:
-        """Has to be passed through, otherwise python will complain about the abstract method.
-        Input arguments are the same as in qiskit's estimator.run().
-        """
-        return self._executor.estimator_run(
-            circuits=circuits,
-            observables=observables,
-            parameter_values=parameter_values,
-            **run_options,
-        )
-
-    def run(
-        self,
-        circuits,
-        observables,
-        parameter_values=None,
-        **run_options,
-    ) -> Job:
-        """
-        Overwrites the sampler primitive run method, to evaluate expectation values.
-        Uses the Executor class for automatic session handling.
-
-        Input arguments are the same as in qiskit's estimator.run()
-
-        """
-        return self._executor.estimator_run(
-            circuits=circuits,
-            observables=observables,
-            parameter_values=parameter_values,
-            **run_options,
-        )
-
-    @property
-    def circuits(self):
-        """Quantum circuits that represents quantum states.
-
-        Returns:
-            The quantum circuits.
-        """
-        return tuple(self._executor.estimator.circuits)
-
-    @property
-    def observables(self):
-        """Observables to be estimated.
-
-        Returns:
-            The observables.
-        """
-        return tuple(self._executor.estimator.observables)
-
-    @property
-    def parameters(self):
-        """Parameters of the quantum circuits.
-
-        Returns:
-            Parameters, where ``parameters[i][j]`` is the j-th parameter of the i-th circuit.
-        """
-        return tuple(self._executor.estimator.parameters)
-
-    @property
-    def options(self) -> Options:
-        """Return options values for the estimator.
-
-        Returns:
-            options
-        """
-        return self._executor.estimator.options
-
-    def set_options(self, **fields):
-        """Set options values for the estimator.
-
-        Args:
-            **fields: The fields to update the options
-        """
-        self._executor.estimator.set_options(**fields)
-        self._executor._options_estimator = self._executor.estimator.options
-
-
-class ExecutorSampler(BaseSampler):
-    """
-    Special Sampler Primitive that uses the Executor service.
-
-    Useful for automatic restarting sessions and caching the results.
-    The object is created by the executor method get_sampler()
-
-    Args:
-        executor (Executor): The executor service to use
-        options: Options for the sampler
-
-    """
-
-    def __init__(self, executor: Executor, options=None):
-
-        if isinstance(options, Options) or isinstance(options, qiskit_ibm_runtime_Options):
-            options_ini = asdict(copy.deepcopy(options))
-        else:
-            options_ini = options
-
-        super().__init__(options=options_ini)
-        self._executor = executor
-
-    def run(
-        self,
-        circuits,
-        parameter_values=None,
-        **run_options,
-    ) -> Job:
-        """
-        Overwrites the sampler primitive run method, to evaluate circuits.
-        Uses the Executor class for automatic session handling.
-
-        Input arguments are the same as in qiskit's sampler.run()
-
-        """
-        return self._executor.sampler_run(
-            circuits=circuits,
-            parameter_values=parameter_values,
-            **run_options,
-        )
-
-    def _run(
-        self,
-        circuits,
-        parameter_values=None,
-        **run_options,
-    ) -> Job:
-        """
-        Overwrites the sampler primitive run method, to evaluate circuits.
-        Uses the Executor class for automatic session handling.
-
-        Input arguments are the same as in qiskit's sampler.run()
-
-        """
-        return self._executor.sampler_run(
-            circuits=circuits,
-            parameter_values=parameter_values,
-            **run_options,
-        )
-
-    def _call(
-        self,
-        circuits,
-        parameter_values=None,
-        **run_options,
-    ) -> SamplerResult:
-        """Has to be passed through, otherwise python will complain about the abstract method"""
-        return self._executor.sampler._call(circuits, parameter_values, **run_options)
-
-    @property
-    def circuits(self):
-        """Quantum circuits to be sampled.
-
-        Returns:
-            The quantum circuits to be sampled.
-        """
-        return tuple(self._executor.sampler.circuits)
-
-    @property
-    def parameters(self):
-        """Parameters of quantum circuits.
-
-        Returns:
-            List of the parameters in each quantum circuit.
-        """
-        return tuple(self._executor.sampler.parameters)
-
-    @property
-    def options(self) -> Options:
-        """Return options values for the estimator.
-
-        Returns:
-            options
-        """
-        return self._executor.sampler.options
-
-    def set_options(self, **fields):
-        """Set options values for the estimator.
-
-        Args:
-            **fields: The fields to update the options
-        """
-        self._executor.sampler.set_options(**fields)
-        self._executor._options_sampler = self._executor.sampler.options
-
-
-class ExecutorCache:
-    """Cache for jobs that are created by Primitives
-
-    Args:
-        folder (str): Folder to store the cache
-
-    """
-
-    def __init__(self,logger, folder: str = ""):
-        self._folder = folder
-        # Check if folder exist, creates the folder otherwise
-        try:
-            import os
-
-            if not os.path.exists(self._folder):
-                os.makedirs(self._folder)
-        except:
-            raise RuntimeError("Could not create folder for cache")
-
-        self._logger = logger
-
-    def hash_variable(self, variable: Any):
-        """
-        Creates a hash value for a list of circuits, parameters, operators.
-
-        The hash value is used as the filename for the cached file.
-        """
-
-        def make_recursive_str(variable_):
-            """creates a string from a list"""
-            if type(variable_) == list:
-                text = ""
-                for i in variable_:
-                    text += make_recursive_str(i)
-                return text
-            else:
-                return str(variable_)
-
-        return blake2b(make_recursive_str(variable).encode("utf-8"), digest_size=20).hexdigest()
-
-    def get_file(self, hash_value: str):
-        """
-        Searches for the cahced file and returns the file otherwise return None.
-
-        Args:
-            hash_value (str): Hash value of the file
-        """
-        try:
-            file = Path(self._folder + "/" + str(hash_value) + ".p")
-            if file.exists():
-                file = open(self._folder + "/" + str(hash_value) + ".p", "rb")
-                data = pickle.load(file)
-                file.close()
-                return data
-            else:
-                return None
-        except:
-            self._logger.info("Could not load job from cache!")
-            self._logger.info("File: " + self._folder + "/" + str(hash_value) + ".p")
-            return None
-
-    def store_file(self, hash_value: str, job_data):
-        """
-        Store the data of a finsihed job.
-
-        Args:
-            hash_value (str): Hash value of the job that is used as a file name
-            job_data: Data of the job
-        """
-        try:
-            file = open(self._folder + "/" + str(hash_value) + ".p", "wb")
-            pickle.dump(job_data, file)
-            file.close()
-        except:
-            raise RuntimeError("Could not store job in cache")
+import logging
+from logging.handlers import RotatingFileHandler
+from logging import handlers
+import copy
+from pathlib import Path
+from hashlib import blake2b
+from typing import Any, Union
+import traceback
+from dataclasses import asdict
+import time
+import dill as pickle
+
+from qiskit.primitives import Estimator as qiskit_primitives_Estimator
+from qiskit.primitives import BackendEstimator as qiskit_primitives_BackendEstimator
+from qiskit.primitives import Sampler as qiskit_primitives_Sampler
+from qiskit.primitives import BackendSampler as qiskit_primitives_BackendSampler
+from qiskit.primitives import BaseEstimator, BaseSampler
+from qiskit.primitives.base import SamplerResult, EstimatorResult
+from qiskit.utils import QuantumInstance
+from qiskit import Aer
+from qiskit_ibm_runtime import QiskitRuntimeService, Session
+from qiskit.opflow import OperatorBase
+from qiskit.providers import Options
+from qiskit.providers import JobV1 as Job
+from qiskit.providers.backend import Backend
+from qiskit.providers.jobstatus import JobStatus, JOB_FINAL_STATES
+from qiskit_ibm_runtime import Estimator as qiskit_ibm_runtime_Estimator
+from qiskit_ibm_runtime import Sampler as qiskit_ibm_runtime_Sampler
+from qiskit_ibm_runtime.exceptions import IBMRuntimeError, RuntimeJobFailureError
+from qiskit_ibm_runtime.options import Options as qiskit_ibm_runtime_Options
+
+from .evaluate_opflow import evaluate_opflow_qi, evaluate_opflow_estimator, evaluate_opflow_sampler
+
+
+class Executor:
+    """
+    Executor class to run Qiskit jobs on IBM Quantum systems or simulators.
+
+    The Executor class is a wrapper around the Qiskit Runtime service, simulators, and primitives
+    Sessions and primitves are automatically created and managed by the Executor class.
+    Results can be cached to avoid re-running the same jobs.
+
+    Args:
+        execution (Union[str, Backend, QuantumInstance, QiskitRuntimeService, Session,
+            BaseEstimator, BaseSampler]): The execution environment, it can be:
+            - A string, that specifics the simulator backend, e.g. 'qasm_simulator'.
+            - A Qiskit backend, to run the jobs on IBM Quantum systems or simulators.
+            - A QuantumInstance, that includes the backend and some options.
+            - A QiskitRuntimeService, to run the jobs on the Qiskit Runtime service.
+                The backend has to be provided separately.
+            - A Session, to run the jobs on the Qiskit Runtime service.
+            - A Estimator primitive (either simulator or Qiskit Runtime primitive)
+            - A Sampler primitive (either simulator or Qiskit Runtime primitive)
+        backend (Optional[Backend]): The backend to run the jobs on.
+            It is only used  if execution is a service.
+        options_estimator (Optional[Options]): The options for the created estimator primitives.
+        options_sampler (Optional[Options]): The options for the created sampler primitives.
+        log_file (str): The name of the log file, if empty, no log file is created.
+        caching (Optional[bool]): Whether to cache the results of the jobs.
+        cache_dir (str): The directory where to cache the results of the jobs.
+        max_session_time (str): The maximum time for a session, similar input as in qiskit.
+        max_jobs_retries (int): The maximum number of retries for a job
+            until the execution is aborted.
+        wait_restart (int): The time to wait before restarting a job in seconds.
+
+    """
+
+    def __init__(
+        self,
+        execution: Union[
+            str,
+            Backend,
+            QuantumInstance,
+            QiskitRuntimeService,
+            Session,
+            BaseEstimator,
+            BaseSampler,
+        ],
+        backend=None,
+        options_estimator=None,
+        options_sampler=None,
+        log_file="",
+        caching=None,
+        cache_dir="_cache",
+        max_session_time="8h",
+        max_jobs_retries=10,
+        wait_restart=1,
+    ) -> None:
+        # Default values for internal variables
+        self._backend = None
+        self._session = None
+        self._service = None
+        self._estimator = None
+        self._sampler = None
+        self._quantum_instance = None
+        self._remote = False
+        self._session_active = False
+        self._execution_origin = ""
+
+        # Copy estimator options and make a dict
+        self._options_estimator = options_estimator
+        if self._options_estimator is None:
+            self._options_estimator = {}
+
+        # Copy sampler options and make a dict
+        self._options_sampler = options_sampler
+        if self._options_sampler is None:
+            self._options_sampler = {}
+
+        # Copy Executor options
+        self._log_file = log_file
+        self._caching = caching
+        self._max_session_time = max_session_time
+        self._max_jobs_retries = max_jobs_retries
+        self._wait_restart = wait_restart
+
+        if self._log_file != "":
+            fh = handlers.RotatingFileHandler(
+                self._log_file, maxBytes=(1048576 * 5), backupCount=100
+            )
+            log_format = logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s")
+            fh.setFormatter(log_format)
+            self._logger = logging.getLogger("executor")
+            self._logger.addHandler(fh)
+            self._logger.setLevel(logging.INFO)
+        else:
+            self._logger = logging.getLogger("executor")
+            self._logger.setLevel(logging.INFO)
+
+        if execution is None and backend is not None:
+            # Only backend is given
+            execution = backend
+
+        if isinstance(execution, str):
+            # Execution is a string -> get backend
+            if execution == "statevector_simulator":
+                self._backend = Aer.get_backend(execution)
+            elif execution == "qasm_simulator":
+                self._backend = Aer.get_backend(execution)
+            elif "ibm" in execution:
+                raise ValueError(
+                    "IBM backend are not supported by string input, since credentials are missing "
+                    + execution
+                )
+            else:
+                raise ValueError("Unknown backend string: " + execution)
+            self._execution_origin = "Simulator"
+        elif isinstance(execution, Backend):
+            # Execution is a backend class
+            if hasattr(execution, "service"):
+                self._service = execution.service
+            self._backend = execution
+            self._execution_origin = "Backend"
+        elif isinstance(execution, QuantumInstance):
+            # Execution is a QuantumInstance
+            self._quantum_instance = execution
+            self._backend = execution.backend
+            self._execution_origin = "QuantumInstance"
+        elif isinstance(execution, QiskitRuntimeService):
+            self._service = execution
+            if isinstance(backend, str):
+                self._backend = self._service.get_backend(backend)
+            elif isinstance(backend, Backend):
+                self._backend = backend
+            elif backend is None:
+                raise ValueError("Backend has to be specified for QiskitRuntimeService")
+            else:
+                raise ValueError("Unknown backend type: " + backend)
+            self._execution_origin = "QiskitRuntimeService"
+        elif isinstance(execution, Session):
+            # Execution is a active? session
+            self._session = execution
+            self._service = self._session.service
+            self._backend = self._session.service.get_backend(self._session.backend())
+            self._session_active = True
+            self._execution_origin = "Session"
+        elif isinstance(execution, BaseEstimator):
+            self._estimator = execution
+            if isinstance(self._estimator, qiskit_primitives_Estimator):
+                # this is only a hack, there is no real backend in the Primitive Estimator class
+                self._backend = Aer.get_backend("statevector_simulator")
+            elif isinstance(self._estimator, qiskit_primitives_BackendEstimator):
+                self._backend = self._estimator._backend
+            # Real Backend
+            elif hasattr(self._estimator, "session"):
+                self._session = self._estimator.session
+                self._service = self._estimator.session.service
+                self._backend = self._estimator.session.service.get_backend(
+                    self._estimator.session.backend()
+                )
+                self._session_active = True
+            else:
+                raise RuntimeError("No backend found in the given Estimator Primitive!")
+
+            if self._options_estimator is None:
+                self._options_estimator = self._estimator.options
+            else:
+                self._estimator.options.update_options(**self._options_estimator)
+            self._execution_origin = "Estimator"
+        elif isinstance(execution, BaseSampler):
+            self._sampler = execution
+
+            if isinstance(self._sampler, qiskit_primitives_Sampler):
+                # this is only a hack, there is no real backend in the Primitive Sampler class
+                self._backend = Aer.get_backend("statevector_simulator")
+            elif isinstance(self._sampler, qiskit_primitives_BackendSampler):
+                self._backend = self._sampler._backend
+            elif hasattr(self._sampler, "session"):
+                self._session = self._sampler.session
+                self._service = self._sampler.session.service
+                self._backend = self._sampler.session.service.get_backend(
+                    self._sampler.session.backend()
+                )
+                self._session_active = True
+            else:
+                raise RuntimeError("No backend found in the given Sampler Primitive!")
+
+            if self._options_sampler is None:
+                self._options_sampler = self._sampler.options
+            else:
+                self._sampler.options.update_options(**self._options_sampler)
+            self._execution_origin = "Sampler"
+        else:
+            raise ValueError("Unknown execution type: " + str(type(execution)))
+
+        # Check if execution is on a remote IBM backend
+        if "ibm" in str(self._backend):
+            self._remote = True
+        else:
+            self._remote = False
+
+        self._inital_num_shots = self.get_shots()
+
+        if self._caching is None:
+            self._caching = self._remote
+
+        if self._caching:
+            self._cache = ExecutorCache(self._logger, cache_dir)
+
+        self._logger.info(f"Executor initialized with backend: {{}}".format(self._backend))
+        self._logger.info(f"Executor initialized with service: {{}}".format(self._service))
+        if self._session is not None:
+            self._logger.info(
+                f"Executor initialized with session: {{}}".format(self._session.session_id)
+            )
+        else:
+            self._logger.info(f"Executor initialized with session: {{}}".format(self._session))
+        self._logger.info(f"Executor initialized with estimator: {{}}".format(self._estimator))
+        self._logger.info(f"Executor initialized with sampler: {{}}".format(self._sampler))
+        self._logger.info(
+            f"Executor initialized with quantum instance: {{}}".format(self._quantum_instance)
+        )
+        self._logger.info(f"Executor intial shots: {{}}".format(self._inital_num_shots))
+
+    @property
+    def execution(self) -> str:
+        """Returns a string that of the executor that is used initializing the executor class."""
+        return self._execution_origin
+
+    @property
+    def backend(self):
+        """Returns the backend that is used for the execution."""
+        return self._backend
+
+    @property
+    def session(self):
+        """Returns the session that is used for the execution."""
+        return self._session
+
+    @property
+    def service(self):
+        """Returns the service that is used for the execution."""
+        return self._service
+
+    @property
+    def estimator(self):
+        """Returns the estimator primitive that is used for the execution.
+
+        This function created automatically estimators and checks for an expired session and
+        creates a new one if necessary.
+
+        The estimator that is created depends on the backend that is used for the execution.
+        """
+        if self._estimator is not None:
+            if self._session is not None and self._session_active is False:
+                # Session is expired, create a new session and a new estimator
+                self.create_session()
+                self._estimator = qiskit_ibm_runtime_Estimator(
+                    session=self._session, options=self._options_estimator
+                )
+            estimator = self._estimator
+        else:
+            # Create a new Estimator
+            shots = self.get_shots()
+            if self._session is not None:
+                if self._session_active is False:
+                    self.create_session()
+                self._estimator = qiskit_ibm_runtime_Estimator(
+                    session=self._session, options=self._options_estimator
+                )
+            elif self._service is not None:
+                # No session but service -> create a new session
+                self.create_session()
+                self._estimator = qiskit_ibm_runtime_Estimator(
+                    session=self._session, options=self._options_estimator
+                )
+            else:
+                if str(self._backend) == "statevector_simulator":
+                    # No session, no service, but state_vector simulator -> Estimator
+                    self._estimator = qiskit_primitives_Estimator(options=self._options_estimator)
+                else:
+                    # No session, no service and no state_vector simulator -> BackendEstimator
+                    self._estimator = qiskit_primitives_BackendEstimator(
+                        backend=self._backend, options=self._options_estimator
+                    )
+            if not self._options_estimator:
+                self.set_shots(shots)
+            estimator = self._estimator
+
+        return estimator
+
+    def clear_estimator_cache(self):
+        if self._estimator is not None:
+            if isinstance(self._estimator, qiskit_primitives_Estimator) or isinstance(
+                self._estimator, qiskit_primitives_BackendEstimator
+            ):
+                self._estimator._circuits = []
+                self._estimator._observables = []
+                self._estimator._parameters = []
+                self._estimator._circuit_ids = {}
+                self._estimator._observable_ids = {}
+
+    @property
+    def sampler(self):
+        """Returns the sampler primitive that is used for the execution.
+
+        This function created automatically estimators and checks for an expired session and
+        creates a new one if necessary.
+
+        The estimator that is created depends on the backend that is used for the execution.
+        """
+        if self._sampler is not None:
+            if self._session is not None and self._session_active is False:
+                # Session is expired, create a new one and a new estimator
+                self.create_session()
+                self._sampler = qiskit_ibm_runtime_Sampler(
+                    session=self._session, options=self._options_sampler
+                )
+            sampler = self._sampler
+        else:
+            # Create a new Sampler
+            shots = self.get_shots()
+            if self._session is not None:
+                if self._session_active is False:
+                    self.create_session()
+                self._sampler = qiskit_ibm_runtime_Sampler(
+                    session=self._session, options=self._options_sampler
+                )
+
+            elif self._service is not None:
+                # No session but service -> create a new session
+                self.create_session()
+                self._sampler = qiskit_ibm_runtime_Sampler(
+                    session=self._session,
+                    options=self._options_sampler,
+                )
+            else:
+                if str(self._backend) == "statevector_simulator":
+                    # No session, no service, but state_vector simulator -> Sampler
+                    self._sampler = qiskit_primitives_Sampler(options=self._options_sampler)
+                else:
+                    # No session, no service and no state_vector simulator -> BackendSampler
+                    self._sampler = qiskit_primitives_BackendSampler(
+                        backend=self._backend, options=self._options_sampler
+                    )
+            if not self._options_sampler:
+                self.set_shots(shots)
+            sampler = self._sampler
+
+        return sampler
+
+    def clear_sampler_cache(self):
+        if self._sampler is not None:
+            if isinstance(self._sampler, qiskit_primitives_Sampler) or isinstance(
+                self._sampler, qiskit_primitives_BackendSampler
+            ):
+                self._sampler._circuits = []
+                self._sampler._parameters = []
+                self._sampler._circuit_ids = {}
+                self._sampler._qargs_list = []
+
+    @property
+    def quantum_instance(self):
+        """Returns the quantum instance that is used for the execution.
+
+        Creates a new one if none is set.
+        """
+
+        if self._quantum_instance is not None:
+            return self._quantum_instance
+        else:
+            self._quantum_instance = QuantumInstance(self._backend, shots=self.get_shots)
+            self._logger.info(
+                f"Executor created new QuantumInstance: {{}}".format(self._quantum_instance)
+            )
+            return self._quantum_instance
+
+    def _primitive_run(self, run, label: str, hash_value: Union[str, None] = None):
+        """Run function that allow restarting, session handling and caching.
+
+        Parent implementation that is used for Estimator and Sampler.
+
+        Args:
+            run (function): Function that is executed.
+            label (str): Label that is used for logging.
+            hash_value (str,None): Hash value that is used for caching.
+
+        Returns:
+            A qiskit job containing the results of the run.
+        """
+        success = False
+
+        for repeat in range(self._max_jobs_retries):
+            try:
+                job = None
+                cached = False
+                if hash_value is not None and self._caching:
+                    # TODO: except cache errors
+                    job = self._cache.get_file(hash_value)
+
+                if job is None:
+                    job = run()
+                    self._logger.info(
+                        f"Executor runs " + label + f" with job: {{}}".format(job.job_id())
+                    )
+                else:
+                    self._logger.info(f"Cached job found with hash value: {{}}".format(hash_value))
+                    cached = True
+
+            except IBMRuntimeError as e:
+                if '"code":1217' in e.message:
+                    self._logger.info(
+                        f"Executor failed to run "
+                        + label
+                        + f" because the session has been closed!"
+                    )
+                    self._session_active = False
+                    continue
+            except Exception as e:
+                self._logger.info(
+                    f"Executor failed to run " + label + f" because of unknown error!"
+                )
+                self._logger.info(f"Error message: {{}}".format(e))
+                self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
+                continue
+
+            # Wait for the job to complete
+            if not cached:
+                status = JobStatus.QUEUED
+                last_status = None
+            else:
+                status = JobStatus.DONE
+            while status not in JOB_FINAL_STATES:
+                try:
+                    status = job.status()
+                    if status != last_status:
+                        self._logger.info(f"Job status: {{}}".format(status))
+                    last_status = status
+                except Exception as e:
+                    self._logger.info(
+                        f"Executor failed to get job status because of unknown error!"
+                    )
+                    self._logger.info(f"Error message: {{}}".format(e))
+                    self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
+                    break
+
+                if self._remote:
+                    time.sleep(1)
+                else:
+                    time.sleep(0.01)
+
+            # Job is completed, check if it was successful
+            if status == JobStatus.ERROR:
+                self._logger.info(f"Failed executation of the job!")
+                self._logger.info(f"Error message: {{}}".format(job.error_message()))
+            elif status == JobStatus.CANCELLED:
+                self._logger.info(f"Throwing RuntimeError, since the job is manually canceled!")
+                raise RuntimeError(f"Job manually canceled!")
+            else:
+                success = True
+                result_success = False
+                for retry_result in range(3):
+                    # check if result is available
+                    try:
+                        result = job.result()
+                        result_success = True
+                    except RuntimeJobFailureError as e:
+                        self._logger.info(f"Executor unable to retriev job result!")
+                        self._logger.info(f"Error message: {{}}".format(e))
+                        self._logger.info(f"Error message: {{}}".format(e))
+                    except Exception as e:
+                        self._logger.info(
+                            f"Executor failed to get job result because of unknown error!"
+                        )
+                        self._logger.info(f"Error message: {{}}".format(e))
+                        self._logger.info(f"Traceback: {{}}".format(traceback.print_exc()))
+                    if result_success:
+                        break
+                    else:
+                        self._logger.info(f"Retrying to get job result")
+                        time.sleep(self._wait_restart)
+
+            if success and result_success:
+                break
+            else:
+                self._logger.info(f"Restarting " + label + f" run")
+                success = False
+                result_success = False
+
+        if success is not True:
+            raise RuntimeError(
+                f"Could not run job successfully after {{}} retries".format(self._max_jobs_retries)
+            )
+
+        if self._caching and not cached:
+            job_pickle = copy.copy(job)
+            # remove _future and _function from job since this creates massive file sizes
+            # and the information is not really needed.
+            job_pickle._future = None
+            job_pickle._function = None
+            job_pickle._api_client = None
+            job_pickle._service = None
+            job_pickle._ws_client_future = None
+            job_pickle._ws_client = None
+            job_pickle._backend = str(job.backend())
+
+            # overwrite result function with the obtained result
+            def result_():
+                return result
+
+            job_pickle.result = result_
+            self._cache.store_file(hash_value, job_pickle)
+            self._logger.info(f"Stored job in cache with hash value: {{}}".format(hash_value))
+
+        return job
+
+    def estimator_run(self, circuits, observables, parameter_values=None, **kwargs: Any):
+        """
+        Function that overwrites the estimator run function.
+
+        Args:
+            circuits: Quantum circuits to execute.
+            observables: Observable to measure.
+            parameter_values: Values for the parameters in circuits.
+            kwargs (Any): Additional arguments that are passed to the estimator.
+
+        Returns:
+            A qiskit job containing the results of the run.
+        """
+
+        def run():
+            return self.estimator.run(circuits, observables, parameter_values, **kwargs)
+
+        if self._caching:
+            # Generate hash value for caching
+            hash_value = self._cache.hash_variable(
+                [
+                    "estimator",
+                    circuits,
+                    observables,
+                    parameter_values,
+                    kwargs,
+                    self._options_estimator,
+                    self._backend,
+                ]
+            )
+        else:
+            hash_value = None
+
+        return self._primitive_run(run, "estimator", hash_value)
+
+    def sampler_run(self, circuits, parameter_values=None, **kwargs: Any):
+        """
+        Function that overwrites the sampler run function.
+
+        Args:
+            circuits: Quantum circuits to execute.
+            parameter_values: Values for the parameters in circuits.
+            kwargs (Any): Additional arguments that are passed to the estimator.
+
+        Returns:
+            A qiskit job containing the results of the run.
+        """
+
+        def run():
+            return self.sampler.run(circuits, parameter_values, **kwargs)
+
+        if self._caching:
+            # Generate hash value for caching
+            hash_value = self._cache.hash_variable(
+                [
+                    "sampler",
+                    circuits,
+                    parameter_values,
+                    kwargs,
+                    self._options_sampler,
+                    self._backend,
+                ]
+            )
+        else:
+            hash_value = None
+
+        return self._primitive_run(run, "sampler", hash_value)
+
+    def get_estimator(self):
+        """
+        Returns a Estimator primitive that uses the Executor for running jobs.
+        Includes caching and automatic session handling.
+        """
+        return ExecutorEstimator(executor=self, options=self._options_estimator)
+
+    def get_sampler(self):
+        """
+        Returns a Sampler primitive that uses the Executor for running jobs.
+        Includes caching and automatic session handling.
+        """
+        return ExecutorSampler(executor=self, options=self._options_sampler)
+
+    def opflow_exec(self, opflow: OperatorBase):
+        """
+        Function for executing an opflow structur.
+
+        This function automatically detects if an estimator, sampler or quantum instance is set and uses
+        The emthod is very likely deprecated very soon.
+
+        Args:
+            opflow: Operator to evaluate.
+
+        Returns:
+            The evaluated opflow structure.
+        """
+        if self._estimator is not None:
+            return evaluate_opflow_estimator(self.get_estimator(), opflow)
+        elif self._sampler is not None:
+            return evaluate_opflow_sampler(self.get_sampler(), opflow)
+        elif self._quantum_instance is not None:
+            return evaluate_opflow_qi(self.quantum_instance, opflow)
+        else:  #  default if nothing is set -> use estimator
+            return evaluate_opflow_estimator(self.get_estimator(), opflow)
+
+    def get_opflow_executor(self) -> str:
+        """Returns a string that indicates which executor is used for opflow execution."""
+        if self._estimator is not None:
+            return "estimator"
+        elif self._sampler is not None:
+            return "sampler"
+        elif self._quantum_instance is not None:
+            return "quantum_instance"
+        else:  #  default if nothing is set -> use estimator
+            return "estimator"
+
+    def backend_run(self, circuits, **run_options: Any):
+        return self.backend.run(circuits, **run_options)
+
+    def set_shots(self, num_shots: Union[int, None]) -> None:
+        """Sets the number shots for the next evaluations.
+
+        Args:
+            num_shots (int or None): Number of shots that are set
+        """
+        if num_shots is None:
+            return None
+
+        if str(self._backend) == "statevector_simulator":
+            # Skip setting shots for statevector simulator
+            return None
+
+        # Update shots in estimator primitive
+        if self._estimator is not None:
+            try:
+                execution = self._estimator.options.get("execution")
+                execution["shots"] = num_shots
+                self._estimator.set_options(execution=execution)
+            except:
+                try:
+                    self._estimator.set_options(shots=num_shots)
+                except:
+                    pass
+
+        # Update shots in sampler primitive
+        if self._sampler is not None:
+            try:
+                execution = self._sampler.options.get("execution")
+                execution["shots"] = num_shots
+                self._sampler.set_options(execution=execution)
+            except:
+                try:
+                    self._sampler.set_options(shots=num_shots)
+                except:
+                    pass
+
+        # Update shots in estimator options for not yet created estimators
+        if self._options_estimator is not None:
+            try:
+                self._options_estimator["execution"]["shots"] = num_shots
+            except:
+                try:
+                    self._options_estimator["shots"] = num_shots
+                except:
+                    pass
+
+        # Update shots in sampler options for not yet created samplers
+        if self._options_sampler is not None:
+            try:
+                self._options_sampler["execution"]["shots"] = num_shots
+            except:
+                try:
+                    self._options_sampler["shots"] = num_shots
+                except:
+                    pass
+
+        # Upate shots in quantum instance
+        if self._quantum_instance is not None:
+            self._quantum_instance.set_config(shots=num_shots)
+
+        # Update shots in backend
+        if self._backend is not None:
+            self._backend.options.shots = num_shots
+
+        self._logger.info("Set shots to {}".format(num_shots))
+
+    def get_shots(self) -> int:
+        """Getter for the number of shots.
+
+        Returns:
+            Returns the number of shots that are used for the current evaluation."""
+        if self._estimator is not None or self._sampler is not None:
+            shots_estimator = 0
+            shots_sampler = 0
+            if self._estimator is not None:
+                try:
+                    execution = self._estimator.options.get("execution")
+                    shots_estimator = execution["shots"]
+                except:
+                    try:
+                        shots_estimator = self._estimator.options.get("shots", 0)
+                    except:
+                        shots_estimator = 0
+            if self._sampler is not None:
+                try:
+                    execution = self._sampler.options.get("execution")
+                    shots_sampler = execution["shots"]
+                except:
+                    try:
+                        shots_sampler = self._sampler.options.get("shots", 0)
+                    except:
+                        shots_sampler = 0
+
+            if self._estimator is not None and self._sampler is not None:
+                if shots_estimator != shots_sampler:
+                    raise ValueError(
+                        "The number of shots of the given \
+                                      Estimator and Sampler is not equal!"
+                    )
+
+            shots = max(shots_estimator, shots_sampler)
+
+        elif self._quantum_instance is not None:
+            shots = self._quantum_instance.run_config.shots
+        elif self._backend is not None:
+            shots = self._backend.options.shots
+        else:
+            return None  # No shots available
+
+        return shots
+
+    def reset_shots(self) -> None:
+        """Resets the shots to the initial values when the executor was created."""
+        self.set_shots(self._inital_num_shots)
+
+    def create_session(self):
+        """Creates a new session"""
+        if self._service is not None:
+            self._session = Session(
+                self._service, backend=self._backend, max_time=self._max_session_time
+            )
+            self._session_active = True
+            self._logger.info(f"Executor created a new session.")
+        else:
+            raise RuntimeError("Session can not started because of missing service!")
+
+    def close_session(self):
+        """Closes the current session"""
+        if self._session is not None:
+            self._logger.info(f"Executor closed session: {{}}".format(self._session.session_id))
+            self._session.close()
+            self._session = None
+        else:
+            raise RuntimeError("No session found!")
+
+    def __del__(self):
+        """Terminate the session in case the executor is deleted"""
+        if self._session is not None:
+            try:
+                self.close_session()
+            except:
+                pass
+
+
+class ExecutorEstimator(BaseEstimator):
+    """
+    Special Estimator Primitive that uses the Executor service.
+
+    Usefull for automatic restarting sessions and caching results.
+    The object is created by the Executor method get_estimator()
+
+    Args:
+        executor (Executor): The executor service to use
+        options: Options for the estimator
+
+    """
+
+    def __init__(self, executor: Executor, options=None):
+        if isinstance(options, Options) or isinstance(options, qiskit_ibm_runtime_Options):
+            options_ini = asdict(copy.deepcopy(options))
+        else:
+            options_ini = options
+
+        super().__init__(options=options_ini)
+        self._executor = executor
+
+    def _call(
+        self,
+        circuits,
+        observables,
+        parameter_values=None,
+        **run_options,
+    ) -> EstimatorResult:
+        """Has to be passed through, otherwise python will complain about the abstract method.
+        Input arguments are the same as in qiskit's estimator.call()
+        """
+        return self._executor.estimator._call(
+            circuits, observables, parameter_values, **run_options
+        )
+
+    def _run(
+        self,
+        circuits,
+        observables,
+        parameter_values,
+        **run_options,
+    ) -> Job:
+        """Has to be passed through, otherwise python will complain about the abstract method.
+        Input arguments are the same as in qiskit's estimator.run().
+        """
+        return self._executor.estimator_run(
+            circuits=circuits,
+            observables=observables,
+            parameter_values=parameter_values,
+            **run_options,
+        )
+
+    def run(
+        self,
+        circuits,
+        observables,
+        parameter_values=None,
+        **run_options,
+    ) -> Job:
+        """
+        Overwrites the sampler primitive run method, to evaluate expectation values.
+        Uses the Executor class for automatic session handling.
+
+        Input arguments are the same as in qiskit's estimator.run()
+
+        """
+        return self._executor.estimator_run(
+            circuits=circuits,
+            observables=observables,
+            parameter_values=parameter_values,
+            **run_options,
+        )
+
+    @property
+    def circuits(self):
+        """Quantum circuits that represents quantum states.
+
+        Returns:
+            The quantum circuits.
+        """
+        return tuple(self._executor.estimator.circuits)
+
+    @property
+    def observables(self):
+        """Observables to be estimated.
+
+        Returns:
+            The observables.
+        """
+        return tuple(self._executor.estimator.observables)
+
+    @property
+    def parameters(self):
+        """Parameters of the quantum circuits.
+
+        Returns:
+            Parameters, where ``parameters[i][j]`` is the j-th parameter of the i-th circuit.
+        """
+        return tuple(self._executor.estimator.parameters)
+
+    @property
+    def options(self) -> Options:
+        """Return options values for the estimator.
+
+        Returns:
+            options
+        """
+        return self._executor.estimator.options
+
+    def clear_cache(self):
+        self._executor.clear_estimator_cache()
+
+    def set_options(self, **fields):
+        """Set options values for the estimator.
+
+        Args:
+            **fields: The fields to update the options
+        """
+        self._executor.estimator.set_options(**fields)
+        self._executor._options_estimator = self._executor.estimator.options
+
+
+class ExecutorSampler(BaseSampler):
+    """
+    Special Sampler Primitive that uses the Executor service.
+
+    Useful for automatic restarting sessions and caching the results.
+    The object is created by the executor method get_sampler()
+
+    Args:
+        executor (Executor): The executor service to use
+        options: Options for the sampler
+
+    """
+
+    def __init__(self, executor: Executor, options=None):
+        if isinstance(options, Options) or isinstance(options, qiskit_ibm_runtime_Options):
+            options_ini = asdict(copy.deepcopy(options))
+        else:
+            options_ini = options
+
+        super().__init__(options=options_ini)
+        self._executor = executor
+
+    def run(
+        self,
+        circuits,
+        parameter_values=None,
+        **run_options,
+    ) -> Job:
+        """
+        Overwrites the sampler primitive run method, to evaluate circuits.
+        Uses the Executor class for automatic session handling.
+
+        Input arguments are the same as in qiskit's sampler.run()
+
+        """
+        return self._executor.sampler_run(
+            circuits=circuits,
+            parameter_values=parameter_values,
+            **run_options,
+        )
+
+    def _run(
+        self,
+        circuits,
+        parameter_values=None,
+        **run_options,
+    ) -> Job:
+        """
+        Overwrites the sampler primitive run method, to evaluate circuits.
+        Uses the Executor class for automatic session handling.
+
+        Input arguments are the same as in qiskit's sampler.run()
+
+        """
+        return self._executor.sampler_run(
+            circuits=circuits,
+            parameter_values=parameter_values,
+            **run_options,
+        )
+
+    def _call(
+        self,
+        circuits,
+        parameter_values=None,
+        **run_options,
+    ) -> SamplerResult:
+        """Has to be passed through, otherwise python will complain about the abstract method"""
+        return self._executor.sampler._call(circuits, parameter_values, **run_options)
+
+    @property
+    def circuits(self):
+        """Quantum circuits to be sampled.
+
+        Returns:
+            The quantum circuits to be sampled.
+        """
+        return tuple(self._executor.sampler.circuits)
+
+    @property
+    def parameters(self):
+        """Parameters of quantum circuits.
+
+        Returns:
+            List of the parameters in each quantum circuit.
+        """
+        return tuple(self._executor.sampler.parameters)
+
+    @property
+    def options(self) -> Options:
+        """Return options values for the estimator.
+
+        Returns:
+            options
+        """
+        return self._executor.sampler.options
+
+    def set_options(self, **fields):
+        """Set options values for the estimator.
+
+        Args:
+            **fields: The fields to update the options
+        """
+        self._executor.sampler.set_options(**fields)
+        self._executor._options_sampler = self._executor.sampler.options
+
+    def clear_cache(self):
+        self._executor.clear_sampler_cache()
+
+
+class ExecutorCache:
+    """Cache for jobs that are created by Primitives
+
+    Args:
+        folder (str): Folder to store the cache
+
+    """
+
+    def __init__(self, logger, folder: str = ""):
+        self._folder = folder
+        # Check if folder exist, creates the folder otherwise
+        try:
+            import os
+
+            if not os.path.exists(self._folder):
+                os.makedirs(self._folder)
+        except:
+            raise RuntimeError("Could not create folder for cache")
+
+        self._logger = logger
+
+    def hash_variable(self, variable: Any):
+        """
+        Creates a hash value for a list of circuits, parameters, operators.
+
+        The hash value is used as the filename for the cached file.
+        """
+
+        def make_recursive_str(variable_):
+            """creates a string from a list"""
+            if type(variable_) == list:
+                text = ""
+                for i in variable_:
+                    text += make_recursive_str(i)
+                return text
+            else:
+                return str(variable_)
+
+        return blake2b(make_recursive_str(variable).encode("utf-8"), digest_size=20).hexdigest()
+
+    def get_file(self, hash_value: str):
+        """
+        Searches for the cahced file and returns the file otherwise return None.
+
+        Args:
+            hash_value (str): Hash value of the file
+        """
+        try:
+            file = Path(self._folder + "/" + str(hash_value) + ".p")
+            if file.exists():
+                file = open(self._folder + "/" + str(hash_value) + ".p", "rb")
+                data = pickle.load(file)
+                file.close()
+                return data
+            else:
+                return None
+        except:
+            self._logger.info("Could not load job from cache!")
+            self._logger.info("File: " + self._folder + "/" + str(hash_value) + ".p")
+            return None
+
+    def store_file(self, hash_value: str, job_data):
+        """
+        Store the data of a finsihed job.
+
+        Args:
+            hash_value (str): Hash value of the job that is used as a file name
+            job_data: Data of the job
+        """
+        try:
+            file = open(self._folder + "/" + str(hash_value) + ".p", "wb")
+            pickle.dump(job_data, file)
+            file.close()
+        except:
+            raise RuntimeError("Could not store job in cache")
```

### Comparing `squlearn-0.1.0/src/squlearn/util/quantum_fisher.py` & `squlearn-0.2.0/src/squlearn/util/quantum_fisher.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-import numpy as np
-from qiskit.circuit import ParameterVector
-from qiskit.utils import QuantumInstance
-from qiskit.opflow.gradients import QFI
-from qiskit.opflow import CircuitStateFn
-from qiskit.opflow import CircuitSampler
-
-from ..feature_map import FeatureMapBase
-from ..util.data_preprocessing import adjust_input, assign_all_parameters
-
-
-def get_quantum_fisher(pqc: FeatureMapBase, x, param, QI: QuantumInstance):
-    """
-    Function for evaluating the Quantum Fisher Information Matrix for an
-    inputted parameterized quantum circuit.
-
-    Args:
-        pqc : Parameterized quantum circuit that will be pruned. Has to be in the pqc format of quantum_fit!
-        x : Input data values for replacing the features in the pqc (can also be an array for multiple Fishers)
-        param : Parameter values for replacing the parameters in the pqc (can also be an array for multiple Fishers)
-        QI : Quantum Instance for evaluating the Quantum Fisher Information Matrix
-
-    Returns: Numpy matrix with the quantum Fisher matrix
-             (or matrices for multi dimensional x and param)
-
-    """
-
-    x_ = ParameterVector("x", pqc.num_features)
-    p_ = ParameterVector("p", pqc.num_parameters)
-    opflow_circ = CircuitStateFn(primitive=pqc.get_circuit(x_, p_), coeff=1.0)
-    qfi = QFI(qfi_method="lin_comb_full").convert(operator=opflow_circ, params=p_)
-    qfi_with_param = assign_all_parameters(qfi, x=x_, param=p_, x_values=x, param_values=param)
-    sampler = CircuitSampler(QI)
-    eval_conv = sampler.convert(qfi_with_param)
-    return np.real(eval_conv.eval())
-
-
-# WORK IN PROGRESS:
-
-
-# def regression_fisher(qnn : qfit, x, y, param, param_op):
-#     # empirical log-likelihood Fischer log p(y|f) = log exp(-0.5(y-f)^2)
-#     # see for example doi:10.5555/3454287.3454661
-#     # F(p) = sum_n (f(x_n)-y_n)^2 grad f(x_n) grad f(x_n)'
-
-#     x_,multi_x = _adjust_input_(x,qnn.get_num_x())
-#     param_,multi_param = _adjust_input_(param,qnn.num_parameters)
-#     param_op_,multi_param_op = _adjust_input_(param_op,qnn.get_num_param_op())
-
-#     print("x_",x_)
-#     print("param_",param_)
-#     print("param_op_",param_op_)
-
-#     f = qnn.eval_f(x_,param_,param_op_)
-#     dfdp = qnn.eval_dfdp(x_,param_,param_op_)
-#     dfdop = qnn.eval_dfdop(x_,param_,param_op_)
-
-#     print("f",f)
-#     print("dfdp",dfdp)
-#     print("dfdop",dfdop)
-
-#     if multi_x:
-#         prefac = []
-#         for i in range(len(y)):
-#             prefac.append(np.square((f[i]-y[i])))
-#     else:
-#         prefac = []
-#         prefac.append(np.square(f[0]-y))
-#     prefac = np.array(prefac)
-
-#     print("prefac",prefac)
-#     ax = 2
-#     if multi_param_op:
-#         ax = 3
-#     dp_dop = np.concatenate((dfdp,dfdop),axis=ax)
-
-#     print("dp_dop",dp_dop)
-
-#     dp_dop_multi = dp_dop.copy()
-
-#     for i in range(len(x_)):
-#         for j in range(len(param_)):
-#             for k in range(len(param_op_)):
-#                 dp_dop_multi[i,j,k] = np.multiply(dp_dop_multi[i,j,k],prefac[i,j,k])
-
-#     print("dp_dop_multi",dp_dop_multi)
-
-#     fischers = np.einsum('ijm,ijn->ijmn',dp_dop,dp_dop_multi)
-
-#     print("fischers",fischers)
-
-#     return np.sum(fischers,axis=0)
-
-
-# def calculate_fhat(qnn : qfit, x,
-#                             param_min,param_max,num_param,
-#                             param_op_min,param_op_max,num_param_op,
-#                             param_op=True, seed = 0):
-
-#     # averaging over x!!!
-
-#     # is all wrong
-
-#     # Create Random variables
-#     state = np.random.get_state()
-#     np.random.seed(seed)
-#     param_rand = np.random.uniform(param_min, param_max, size=(num_param, qnn.num_parameters))
-#     param_op_rand = np.random.uniform(param_op_min, param_op_max, size=(num_param_op, qnn.get_num_param_op()))
-#     np.random.set_state(state)
-
-#     volume_param = (param_max - param_min) * qnn.num_parameters + (param_op_max - param_op_min)*qnn.get_num_param_op()
-
-#     fischers = qnn.eval_fischer(x,param_rand,param_op_rand)
-#     fischer_trace = np.trace(np.average(fischers,axis=(0,1,2)))
-#     fischers_avrg = np.average(np.reshape(fischers, (len(x), num_param*num_param_op,
-#     qnn.num_parameters+qnn.get_num_param_op(),
-#     qnn.num_parameters+qnn.get_num_param_op())),axis=0)
-
-#     f_hat = fischers_avrg / fischer_trace * volume_param
-#     return f_hat,fischer_trace,volume_param
-
-# def calculate_effective_dimension(f_hat,n,gamma,volume_param):
-#     #n?
-
-#     if gamma <= 0.0 or gamma > 1.0:
-#         raise ValueError("Gamma out of range (0,1]: gamma = ",gamma)
-
-#     for f in f_hat:
-#         w,v = np.linalg.eig(f)
-#         print("eigenvalues",w)
-
-
-#     factor = gamma*float(n)/(2.0*np.pi*np.log(float(n)))
-#     print("factor",factor)
-#     print("det(f_hat)",np.linalg.det(f_hat))
-#     print("det(f_hat*factor)",np.linalg.det(f_hat*factor))
-#     # rewriting of the original formular, since this is more robust
-#     # following the code of Abbas et al:
-#     # log(1/V sum sqrt(det(A)) ) = log(sum exp(log(det(A))/2)-log(V)
-#     # special more robust function for log(det(A)) -> slogdet
-#     IplusF = np.eye(f_hat.shape[1]) + f_hat*factor
-#     print("det(IplusF)",np.linalg.det(IplusF))
-#     print("np.linalg.slogdet(IplusF)[0]",np.linalg.slogdet(IplusF)[0])
-#     print("np.linalg.slogdet(IplusF)[1]",np.linalg.slogdet(IplusF)[1])
-#     logdet = logsumexp(np.linalg.slogdet(IplusF)[1]/2)
-#     print("logdet",logdet)
-#     print("np.log(volume_param)",np.log(volume_param))
-#     print("np.log(factor)",np.log(factor))
-#     value = 2 * (logdet - np.log(volume_param))/np.log(factor)
-#     print("eff dim",value)
-#     return value
+import numpy as np
+from qiskit.circuit import ParameterVector
+from qiskit.utils import QuantumInstance
+from qiskit.opflow.gradients import QFI
+from qiskit.opflow import CircuitStateFn
+from qiskit.opflow import CircuitSampler
+
+from ..feature_map.feature_map_base import FeatureMapBase
+from ..util.data_preprocessing import adjust_input, assign_all_parameters
+
+
+def get_quantum_fisher(pqc: FeatureMapBase, x, param, QI: QuantumInstance):
+    """
+    Function for evaluating the Quantum Fisher Information Matrix for an
+    inputted parameterized quantum circuit.
+
+    Args:
+        pqc : Parameterized quantum circuit that will be pruned. Has to be in the pqc format of quantum_fit!
+        x : Input data values for replacing the features in the pqc (can also be an array for multiple Fishers)
+        param : Parameter values for replacing the parameters in the pqc (can also be an array for multiple Fishers)
+        QI : Quantum Instance for evaluating the Quantum Fisher Information Matrix
+
+    Returns: Numpy matrix with the quantum Fisher matrix
+             (or matrices for multi dimensional x and param)
+
+    """
+
+    x_ = ParameterVector("x", pqc.num_features)
+    p_ = ParameterVector("p", pqc.num_parameters)
+    opflow_circ = CircuitStateFn(primitive=pqc.get_circuit(x_, p_), coeff=1.0)
+    qfi = QFI(qfi_method="lin_comb_full").convert(operator=opflow_circ, params=p_)
+    qfi_with_param = assign_all_parameters(qfi, x=x_, param=p_, x_values=x, param_values=param)
+    sampler = CircuitSampler(QI)
+    eval_conv = sampler.convert(qfi_with_param)
+    return np.real(eval_conv.eval())
+
+
+# WORK IN PROGRESS:
+
+
+# def regression_fisher(qnn : qfit, x, y, param, param_op):
+#     # empirical log-likelihood Fischer log p(y|f) = log exp(-0.5(y-f)^2)
+#     # see for example doi:10.5555/3454287.3454661
+#     # F(p) = sum_n (f(x_n)-y_n)^2 grad f(x_n) grad f(x_n)'
+
+#     x_,multi_x = _adjust_input_(x,qnn.get_num_x())
+#     param_,multi_param = _adjust_input_(param,qnn.num_parameters)
+#     param_op_,multi_param_op = _adjust_input_(param_op,qnn.get_num_param_op())
+
+#     print("x_",x_)
+#     print("param_",param_)
+#     print("param_op_",param_op_)
+
+#     f = qnn.eval_f(x_,param_,param_op_)
+#     dfdp = qnn.eval_dfdp(x_,param_,param_op_)
+#     dfdop = qnn.eval_dfdop(x_,param_,param_op_)
+
+#     print("f",f)
+#     print("dfdp",dfdp)
+#     print("dfdop",dfdop)
+
+#     if multi_x:
+#         prefac = []
+#         for i in range(len(y)):
+#             prefac.append(np.square((f[i]-y[i])))
+#     else:
+#         prefac = []
+#         prefac.append(np.square(f[0]-y))
+#     prefac = np.array(prefac)
+
+#     print("prefac",prefac)
+#     ax = 2
+#     if multi_param_op:
+#         ax = 3
+#     dp_dop = np.concatenate((dfdp,dfdop),axis=ax)
+
+#     print("dp_dop",dp_dop)
+
+#     dp_dop_multi = dp_dop.copy()
+
+#     for i in range(len(x_)):
+#         for j in range(len(param_)):
+#             for k in range(len(param_op_)):
+#                 dp_dop_multi[i,j,k] = np.multiply(dp_dop_multi[i,j,k],prefac[i,j,k])
+
+#     print("dp_dop_multi",dp_dop_multi)
+
+#     fischers = np.einsum('ijm,ijn->ijmn',dp_dop,dp_dop_multi)
+
+#     print("fischers",fischers)
+
+#     return np.sum(fischers,axis=0)
+
+
+# def calculate_fhat(qnn : qfit, x,
+#                             param_min,param_max,num_param,
+#                             param_op_min,param_op_max,num_param_op,
+#                             param_op=True, seed = 0):
+
+#     # averaging over x!!!
+
+#     # is all wrong
+
+#     # Create Random variables
+#     state = np.random.get_state()
+#     np.random.seed(seed)
+#     param_rand = np.random.uniform(param_min, param_max, size=(num_param, qnn.num_parameters))
+#     param_op_rand = np.random.uniform(param_op_min, param_op_max, size=(num_param_op, qnn.get_num_param_op()))
+#     np.random.set_state(state)
+
+#     volume_param = (param_max - param_min) * qnn.num_parameters + (param_op_max - param_op_min)*qnn.get_num_param_op()
+
+#     fischers = qnn.eval_fischer(x,param_rand,param_op_rand)
+#     fischer_trace = np.trace(np.average(fischers,axis=(0,1,2)))
+#     fischers_avrg = np.average(np.reshape(fischers, (len(x), num_param*num_param_op,
+#     qnn.num_parameters+qnn.get_num_param_op(),
+#     qnn.num_parameters+qnn.get_num_param_op())),axis=0)
+
+#     f_hat = fischers_avrg / fischer_trace * volume_param
+#     return f_hat,fischer_trace,volume_param
+
+# def calculate_effective_dimension(f_hat,n,gamma,volume_param):
+#     #n?
+
+#     if gamma <= 0.0 or gamma > 1.0:
+#         raise ValueError("Gamma out of range (0,1]: gamma = ",gamma)
+
+#     for f in f_hat:
+#         w,v = np.linalg.eig(f)
+#         print("eigenvalues",w)
+
+
+#     factor = gamma*float(n)/(2.0*np.pi*np.log(float(n)))
+#     print("factor",factor)
+#     print("det(f_hat)",np.linalg.det(f_hat))
+#     print("det(f_hat*factor)",np.linalg.det(f_hat*factor))
+#     # rewriting of the original formular, since this is more robust
+#     # following the code of Abbas et al:
+#     # log(1/V sum sqrt(det(A)) ) = log(sum exp(log(det(A))/2)-log(V)
+#     # special more robust function for log(det(A)) -> slogdet
+#     IplusF = np.eye(f_hat.shape[1]) + f_hat*factor
+#     print("det(IplusF)",np.linalg.det(IplusF))
+#     print("np.linalg.slogdet(IplusF)[0]",np.linalg.slogdet(IplusF)[0])
+#     print("np.linalg.slogdet(IplusF)[1]",np.linalg.slogdet(IplusF)[1])
+#     logdet = logsumexp(np.linalg.slogdet(IplusF)[1]/2)
+#     print("logdet",logdet)
+#     print("np.log(volume_param)",np.log(volume_param))
+#     print("np.log(factor)",np.log(factor))
+#     value = 2 * (logdet - np.log(volume_param))/np.log(factor)
+#     print("eff dim",value)
+#     return value
```

