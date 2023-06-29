# Comparing `tmp/qibo-0.1.8rc0.tar.gz` & `tmp/qibo-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibo-0.1.8rc0.tar", last modified: Wed Jul 20 07:09:53 2022, max compression
+gzip compressed data, was "qibo-0.1.9.tar", last modified: Wed Nov  9 14:41:30 2022, max compression
```

## Comparing `qibo-0.1.8rc0.tar` & `qibo-0.1.9.tar`

### file list

```diff
@@ -1,103 +1,108 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.044426 qibo-0.1.8rc0/
--rw-r--r--   0 runner     (501) staff       (20)    11342 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     2971 2022-07-20 07:09:53.043890 qibo-0.1.8rc0/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2497 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/README.md
--rw-r--r--   0 runner     (501) staff       (20)       38 2022-07-20 07:09:53.044549 qibo-0.1.8rc0/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     2140 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:52.997478 qibo-0.1.8rc0/src/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.004275 qibo-0.1.8rc0/src/qibo/
--rw-r--r--   0 runner     (501) staff       (20)      566 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/__init__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.009792 qibo-0.1.8rc0/src/qibo/backends/
--rw-r--r--   0 runner     (501) staff       (20)     4333 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    13772 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/abstract.py
--rw-r--r--   0 runner     (501) staff       (20)     2794 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/einsum_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     6672 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/matrices.py
--rw-r--r--   0 runner     (501) staff       (20)    28246 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/numpy.py
--rw-r--r--   0 runner     (501) staff       (20)    11822 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/backends/tensorflow.py
--rw-r--r--   0 runner     (501) staff       (20)    11249 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/callbacks.py
--rw-r--r--   0 runner     (501) staff       (20)     3096 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/config.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.012794 qibo-0.1.8rc0/src/qibo/gates/
--rw-r--r--   0 runner     (501) staff       (20)      135 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    12325 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/abstract.py
--rw-r--r--   0 runner     (501) staff       (20)    12117 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/channels.py
--rw-r--r--   0 runner     (501) staff       (20)    33821 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/gates.py
--rw-r--r--   0 runner     (501) staff       (20)     9627 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/measurements.py
--rw-r--r--   0 runner     (501) staff       (20)     5381 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/gates/special.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.015644 qibo-0.1.8rc0/src/qibo/hamiltonians/
--rw-r--r--   0 runner     (501) staff       (20)      109 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3758 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/abstract.py
--rw-r--r--   0 runner     (501) staff       (20)     5925 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/adiabatic.py
--rw-r--r--   0 runner     (501) staff       (20)    28277 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/hamiltonians.py
--rw-r--r--   0 runner     (501) staff       (20)     6457 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/models.py
--rw-r--r--   0 runner     (501) staff       (20)    13088 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/hamiltonians/terms.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.020324 qibo-0.1.8rc0/src/qibo/models/
--rw-r--r--   0 runner     (501) staff       (20)      335 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    54259 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/circuit.py
--rw-r--r--   0 runner     (501) staff       (20)    13687 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/distcircuit.py
--rw-r--r--   0 runner     (501) staff       (20)    13231 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/evolution.py
--rw-r--r--   0 runner     (501) staff       (20)    11284 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/grover.py
--rw-r--r--   0 runner     (501) staff       (20)     9088 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/hep.py
--rw-r--r--   0 runner     (501) staff       (20)     2873 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/qft.py
--rw-r--r--   0 runner     (501) staff       (20)    14570 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/qgan.py
--rw-r--r--   0 runner     (501) staff       (20)     6804 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/tsp.py
--rw-r--r--   0 runner     (501) staff       (20)    24409 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/models/variational.py
--rw-r--r--   0 runner     (501) staff       (20)     3781 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/noise.py
--rw-r--r--   0 runner     (501) staff       (20)    12696 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/optimizers.py
--rw-r--r--   0 runner     (501) staff       (20)     4402 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/parallel.py
--rw-r--r--   0 runner     (501) staff       (20)     4995 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/solvers.py
--rw-r--r--   0 runner     (501) staff       (20)     9296 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/states.py
--rw-r--r--   0 runner     (501) staff       (20)     4774 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/symbols.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.041896 qibo-0.1.8rc0/src/qibo/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2709 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/conftest.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.042538 qibo-0.1.8rc0/src/qibo/tests/regressions/
--rw-r--r--   0 runner     (501) staff       (20)        0 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/regressions/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     3829 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_backends.py
--rw-r--r--   0 runner     (501) staff       (20)    15126 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_callbacks.py
--rw-r--r--   0 runner     (501) staff       (20)    12104 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_cirq.py
--rw-r--r--   0 runner     (501) staff       (20)     3590 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_dill.py
--rw-r--r--   0 runner     (501) staff       (20)    10349 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_gates_abstract.py
--rw-r--r--   0 runner     (501) staff       (20)     6792 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_gates_channels.py
--rw-r--r--   0 runner     (501) staff       (20)     7455 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_gates_density_matrix.py
--rw-r--r--   0 runner     (501) staff       (20)    24532 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_gates_gates.py
--rw-r--r--   0 runner     (501) staff       (20)     1011 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_gates_special.py
--rw-r--r--   0 runner     (501) staff       (20)     2487 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_global_backend.py
--rw-r--r--   0 runner     (501) staff       (20)    13170 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians.py
--rw-r--r--   0 runner     (501) staff       (20)     9269 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_from_symbols.py
--rw-r--r--   0 runner     (501) staff       (20)     2121 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_models.py
--rw-r--r--   0 runner     (501) staff       (20)    11564 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_symbolic.py
--rw-r--r--   0 runner     (501) staff       (20)     8845 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_terms.py
--rw-r--r--   0 runner     (501) staff       (20)     5854 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_trotter.py
--rw-r--r--   0 runner     (501) staff       (20)    12847 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_measurements.py
--rw-r--r--   0 runner     (501) staff       (20)     8833 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_measurements_collapse.py
--rw-r--r--   0 runner     (501) staff       (20)     5352 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_measurements_probabilistic.py
--rw-r--r--   0 runner     (501) staff       (20)    21609 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit.py
--rw-r--r--   0 runner     (501) staff       (20)     2053 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_backpropagation.py
--rw-r--r--   0 runner     (501) staff       (20)     3261 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_execution.py
--rw-r--r--   0 runner     (501) staff       (20)    11723 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_features.py
--rw-r--r--   0 runner     (501) staff       (20)     6597 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_fuse.py
--rw-r--r--   0 runner     (501) staff       (20)     6651 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_noise.py
--rw-r--r--   0 runner     (501) staff       (20)     7640 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_parametrized.py
--rw-r--r--   0 runner     (501) staff       (20)    13070 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_qasm.py
--rw-r--r--   0 runner     (501) staff       (20)     6267 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_qasm_cirq.py
--rw-r--r--   0 runner     (501) staff       (20)     6575 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_distcircuit.py
--rw-r--r--   0 runner     (501) staff       (20)     6521 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_distcircuit_execution.py
--rw-r--r--   0 runner     (501) staff       (20)    13485 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_evolution.py
--rw-r--r--   0 runner     (501) staff       (20)     3945 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_grover.py
--rw-r--r--   0 runner     (501) staff       (20)     1670 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_hep.py
--rw-r--r--   0 runner     (501) staff       (20)     2377 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_qft.py
--rw-r--r--   0 runner     (501) staff       (20)     4933 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_qgan.py
--rw-r--r--   0 runner     (501) staff       (20)     1776 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_tsp.py
--rw-r--r--   0 runner     (501) staff       (20)    11446 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_models_variational.py
--rw-r--r--   0 runner     (501) staff       (20)     4628 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_noise.py
--rw-r--r--   0 runner     (501) staff       (20)     1848 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_parallel.py
--rw-r--r--   0 runner     (501) staff       (20)     3594 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_prints.py
--rw-r--r--   0 runner     (501) staff       (20)     1944 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/test_states.py
--rw-r--r--   0 runner     (501) staff       (20)     1306 2022-07-20 07:09:47.000000 qibo-0.1.8rc0/src/qibo/tests/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-07-20 07:09:53.006823 qibo-0.1.8rc0/src/qibo.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     2971 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2958 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/not-zip-safe
--rw-r--r--   0 runner     (501) staff       (20)      220 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        5 2022-07-20 07:09:52.000000 qibo-0.1.8rc0/src/qibo.egg-info/top_level.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.323714 qibo-0.1.9/
+-rw-r--r--   0 runner     (501) staff       (20)    11342 2022-11-09 14:41:19.000000 qibo-0.1.9/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     3634 2022-11-09 14:41:30.323315 qibo-0.1.9/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3163 2022-11-09 14:41:19.000000 qibo-0.1.9/README.md
+-rw-r--r--   0 runner     (501) staff       (20)       38 2022-11-09 14:41:30.323860 qibo-0.1.9/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     2243 2022-11-09 14:41:19.000000 qibo-0.1.9/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.272707 qibo-0.1.9/src/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.279997 qibo-0.1.9/src/qibo/
+-rw-r--r--   0 runner     (501) staff       (20)      419 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/__init__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.286157 qibo-0.1.9/src/qibo/backends/
+-rw-r--r--   0 runner     (501) staff       (20)     4401 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14021 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/abstract.py
+-rw-r--r--   0 runner     (501) staff       (20)     2779 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/einsum_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     7480 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/npmatrices.py
+-rw-r--r--   0 runner     (501) staff       (20)    28860 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/numpy.py
+-rw-r--r--   0 runner     (501) staff       (20)    12470 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/backends/tensorflow.py
+-rw-r--r--   0 runner     (501) staff       (20)    11329 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/callbacks.py
+-rw-r--r--   0 runner     (501) staff       (20)     3097 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/config.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.289246 qibo-0.1.9/src/qibo/gates/
+-rw-r--r--   0 runner     (501) staff       (20)      136 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    12497 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/abstract.py
+-rw-r--r--   0 runner     (501) staff       (20)    14025 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/channels.py
+-rw-r--r--   0 runner     (501) staff       (20)    37716 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/gates.py
+-rw-r--r--   0 runner     (501) staff       (20)     9642 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/measurements.py
+-rw-r--r--   0 runner     (501) staff       (20)     5357 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/gates/special.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.292458 qibo-0.1.9/src/qibo/hamiltonians/
+-rw-r--r--   0 runner     (501) staff       (20)      109 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4466 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/abstract.py
+-rw-r--r--   0 runner     (501) staff       (20)     5995 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/adiabatic.py
+-rw-r--r--   0 runner     (501) staff       (20)    31214 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/hamiltonians.py
+-rw-r--r--   0 runner     (501) staff       (20)     6490 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/models.py
+-rw-r--r--   0 runner     (501) staff       (20)    13154 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/hamiltonians/terms.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.297710 qibo-0.1.9/src/qibo/models/
+-rw-r--r--   0 runner     (501) staff       (20)      312 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    56235 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/circuit.py
+-rw-r--r--   0 runner     (501) staff       (20)    13591 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/distcircuit.py
+-rw-r--r--   0 runner     (501) staff       (20)    13302 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/evolution.py
+-rw-r--r--   0 runner     (501) staff       (20)    11726 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/grover.py
+-rw-r--r--   0 runner     (501) staff       (20)     9161 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/hep.py
+-rw-r--r--   0 runner     (501) staff       (20)     2868 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/qft.py
+-rw-r--r--   0 runner     (501) staff       (20)    16015 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/qgan.py
+-rw-r--r--   0 runner     (501) staff       (20)     7004 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/tsp.py
+-rw-r--r--   0 runner     (501) staff       (20)    24798 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/models/variational.py
+-rw-r--r--   0 runner     (501) staff       (20)     4172 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/noise.py
+-rw-r--r--   0 runner     (501) staff       (20)    13262 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/optimizers.py
+-rw-r--r--   0 runner     (501) staff       (20)     4432 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/parallel.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.299219 qibo-0.1.9/src/qibo/quantum_info/
+-rw-r--r--   0 runner     (501) staff       (20)       78 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/quantum_info/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    10704 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/quantum_info/metrics.py
+-rw-r--r--   0 runner     (501) staff       (20)     4821 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/quantum_info/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     5088 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/solvers.py
+-rw-r--r--   0 runner     (501) staff       (20)    10199 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/states.py
+-rw-r--r--   0 runner     (501) staff       (20)     5010 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/symbols.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.322347 qibo-0.1.9/src/qibo/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2763 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/conftest.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.322877 qibo-0.1.9/src/qibo/tests/regressions/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/regressions/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     3842 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_backends.py
+-rw-r--r--   0 runner     (501) staff       (20)    15227 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_callbacks.py
+-rw-r--r--   0 runner     (501) staff       (20)    11925 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_cirq.py
+-rw-r--r--   0 runner     (501) staff       (20)     3598 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_dill.py
+-rw-r--r--   0 runner     (501) staff       (20)    10049 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_gates_abstract.py
+-rw-r--r--   0 runner     (501) staff       (20)     7489 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_gates_channels.py
+-rw-r--r--   0 runner     (501) staff       (20)     7366 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_gates_density_matrix.py
+-rw-r--r--   0 runner     (501) staff       (20)    25960 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_gates_gates.py
+-rw-r--r--   0 runner     (501) staff       (20)     1013 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_gates_special.py
+-rw-r--r--   0 runner     (501) staff       (20)     2490 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_global_backend.py
+-rw-r--r--   0 runner     (501) staff       (20)    14483 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians.py
+-rw-r--r--   0 runner     (501) staff       (20)     9381 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians_from_symbols.py
+-rw-r--r--   0 runner     (501) staff       (20)     2127 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians_models.py
+-rw-r--r--   0 runner     (501) staff       (20)    13114 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians_symbolic.py
+-rw-r--r--   0 runner     (501) staff       (20)     8843 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians_terms.py
+-rw-r--r--   0 runner     (501) staff       (20)     5859 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_hamiltonians_trotter.py
+-rw-r--r--   0 runner     (501) staff       (20)    12890 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_measurements.py
+-rw-r--r--   0 runner     (501) staff       (20)     8881 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_measurements_collapse.py
+-rw-r--r--   0 runner     (501) staff       (20)     5261 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_measurements_probabilistic.py
+-rw-r--r--   0 runner     (501) staff       (20)    21914 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit.py
+-rw-r--r--   0 runner     (501) staff       (20)     2077 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_backpropagation.py
+-rw-r--r--   0 runner     (501) staff       (20)     3238 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_execution.py
+-rw-r--r--   0 runner     (501) staff       (20)    11694 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_features.py
+-rw-r--r--   0 runner     (501) staff       (20)     6565 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_fuse.py
+-rw-r--r--   0 runner     (501) staff       (20)     6555 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_noise.py
+-rw-r--r--   0 runner     (501) staff       (20)     8422 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_parametrized.py
+-rw-r--r--   0 runner     (501) staff       (20)    13072 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_qasm.py
+-rw-r--r--   0 runner     (501) staff       (20)     6371 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_circuit_qasm_cirq.py
+-rw-r--r--   0 runner     (501) staff       (20)     6573 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_distcircuit.py
+-rw-r--r--   0 runner     (501) staff       (20)     6533 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_distcircuit_execution.py
+-rw-r--r--   0 runner     (501) staff       (20)    13257 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_evolution.py
+-rw-r--r--   0 runner     (501) staff       (20)     4017 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_grover.py
+-rw-r--r--   0 runner     (501) staff       (20)     2786 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_hep.py
+-rw-r--r--   0 runner     (501) staff       (20)     2376 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_qft.py
+-rw-r--r--   0 runner     (501) staff       (20)     4955 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_qgan.py
+-rw-r--r--   0 runner     (501) staff       (20)     1689 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_tsp.py
+-rw-r--r--   0 runner     (501) staff       (20)    11337 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_models_variational.py
+-rw-r--r--   0 runner     (501) staff       (20)     6436 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_noise.py
+-rw-r--r--   0 runner     (501) staff       (20)     1997 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_parallel.py
+-rw-r--r--   0 runner     (501) staff       (20)     3648 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_prints.py
+-rw-r--r--   0 runner     (501) staff       (20)    11424 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_quantum_info.py
+-rw-r--r--   0 runner     (501) staff       (20)     3143 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/test_states.py
+-rw-r--r--   0 runner     (501) staff       (20)     1300 2022-11-09 14:41:19.000000 qibo-0.1.9/src/qibo/tests/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2022-11-09 14:41:30.282881 qibo-0.1.9/src/qibo.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3634 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     3094 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/not-zip-safe
+-rw-r--r--   0 runner     (501) staff       (20)      236 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        5 2022-11-09 14:41:30.000000 qibo-0.1.9/src/qibo.egg-info/top_level.txt
```

### Comparing `qibo-0.1.8rc0/LICENSE` & `qibo-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qibo-0.1.8rc0/PKG-INFO` & `qibo-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: qibo
-Version: 0.1.8rc0
-Summary: A framework for quantum computing with hardware acceleration.
-Home-page: https://github.com/qiboteam/qibo
-Author: The Qibo team
-Author-email: 
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7.0
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE
-
 ![](doc/source/qibo_logo.svg)
 
 ![Tests](https://github.com/qiboteam/qibo/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/qiboteam/qibo/branch/master/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibo)
 [![Documentation Status](https://readthedocs.org/projects/qibo/badge/?version=latest)](https://qibo.readthedocs.io/en/latest/?badge=latest)
 [![DOI](https://zenodo.org/badge/241307936.svg)](https://zenodo.org/badge/latestdoi/241307936)
 
@@ -71,8 +54,21 @@
 
 In both cases, the simulation will run in a single device CPU or GPU in double precision `complex128`.
 
 ## Citation policy
 
 If you use the package please refer to [the documentation](https://qibo.readthedocs.io/en/stable/appendix/citing-qibo.html) for citation instructions.
 
+## Supporters and collaborators
 
+- Quantum Research Center, Technology Innovation Institute (TII), United Arab Emirates
+- Università degli Studi di Milano (UNIMI), Italy.
+- Istituto Nazionale di Fisica Nucleare (INFN), Italy.
+- European Organization for Nuclear research (CERN), Switzerland.
+- Universitat de Barcelona (UB), Spain.
+- Barcelona Supercomputing Center (BSC), Spain.
+- Qilimanjaro Quantum Tech, Spain.
+- Centre for Quantum Technologies (CQT), Singapore.
+- Institute of High Performance Computing (IHPC), Singapore.
+- National Supercomputing Centre (NSCC), Singapore.
+- RIKEN Center for Computational Science (R-CCS), Japan.
+- NVIDIA (cuQuantum), USA.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qibo-0.1.8rc0/setup.py` & `qibo-0.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Installation script for python
-from setuptools import setup, find_packages
 import os
 import re
 
+from setuptools import find_packages, setup
+
 PACKAGE = "qibo"
 
 
 # Returns the qibo version
 def get_version():
-    """ Gets the version from the package's __init__ file
-    if there is some problem, let it happily fail """
+    """Gets the version from the package's __init__ file
+    if there is some problem, let it happily fail"""
     VERSIONFILE = os.path.join("src", PACKAGE, "__init__.py")
-    initfile_lines = open(VERSIONFILE, "rt").readlines()
+    initfile_lines = open(VERSIONFILE).readlines()
     VSRE = r"^__version__ = ['\"]([^'\"]*)['\"]"
     for line in initfile_lines:
         mo = re.search(VSRE, line, re.M)
         if mo:
             return mo.group(1)
 
 
@@ -23,18 +24,18 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 # read Tensorflow version requirement
 BACKENDFILE = os.path.join("src", PACKAGE, "config.py")
-with open(BACKENDFILE, 'r') as f:
+with open(BACKENDFILE) as f:
     content = f.readlines()
     for line in content:
-        if 'TF_MIN_VERSION' in line:
+        if "TF_MIN_VERSION" in line:
             TF_MIN_VERSION = str(line.split()[2].replace("'", ""))
             break
 
 
 setup(
     name="qibo",
     version=get_version(),
@@ -56,17 +57,25 @@
         "sympy",
         "cma",
         "joblib",
         "matplotlib",
         "psutil",
         "pyyaml",
         "importlib_metadata",
-        "tabulate"
+        "tabulate",
     ],
     extras_require={
-        "docs": ["sphinx", "sphinx_rtd_theme", "recommonmark", "sphinxcontrib-bibtex", "sphinx_markdown_tables", "nbsphinx", "IPython"],
-        "tests": ["pytest", "cirq", "ply", "sklearn", "dill"],
+        "docs": [
+            "sphinx",
+            "sphinx_rtd_theme",
+            "recommonmark",
+            "sphinxcontrib-bibtex",
+            "sphinx_markdown_tables",
+            "nbsphinx",
+            "IPython",
+        ],
+        "tests": ["pytest", "cirq", "ply", "scikit-learn", "dill", "pre-commit"],
     },
     python_requires=">=3.7.0",
     long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description_content_type="text/markdown",
 )
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/__init__.py` & `qibo-0.1.9/src/qibo/backends/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
-from qibo.config import log, raise_error
+
 from qibo.backends.abstract import Backend
+from qibo.backends.npmatrices import NumpyMatrices
 from qibo.backends.numpy import NumpyBackend
 from qibo.backends.tensorflow import TensorflowBackend
-from qibo.backends.matrices import Matrices
+from qibo.config import log, raise_error
 
 
 def construct_backend(backend, platform=None, runcard=None):
     if backend == "qibojit":
         from qibojit.backends import CupyBackend, CuQuantumBackend, NumbaBackend
+
         if platform == "cupy":  # pragma: no cover
             return CupyBackend()
         elif platform == "cuquantum":  # pragma: no cover
             return CuQuantumBackend()
         elif platform == "numba":
             return NumbaBackend()
         else:  # pragma: no cover
@@ -24,15 +26,16 @@
     elif backend == "tensorflow":
         return TensorflowBackend()
 
     elif backend == "numpy":
         return NumpyBackend()
 
     elif backend == "qibolab":  # pragma: no cover
-        from qibolab.backends import QibolabBackend # pylint: disable=E0401
+        from qibolab.backends import QibolabBackend  # pylint: disable=E0401
+
         return QibolabBackend(platform, runcard)
 
     else:  # pragma: no cover
         raise_error(ValueError, f"Backend {backend} is not available.")
 
 
 class GlobalBackend(NumpyBackend):
@@ -40,15 +43,15 @@
 
     _instance = None
     _dtypes = {"double": "complex128", "single": "complex64"}
     _default_order = [
         {"backend": "qibojit", "platform": "cupy"},
         {"backend": "qibojit", "platform": "numba"},
         {"backend": "tensorflow"},
-        {"backend": "numpy"}
+        {"backend": "numpy"},
     ]
 
     def __new__(cls):
         if cls._instance is not None:
             return cls._instance
 
         backend = os.environ.get("QIBO_BACKEND")
@@ -61,34 +64,37 @@
             for kwargs in cls._default_order:
                 try:
                     cls._instance = construct_backend(**kwargs)
                     break
                 except (ModuleNotFoundError, ImportError):
                     pass
 
-        if cls._instance is None: # pragma: no cover
+        if cls._instance is None:  # pragma: no cover
             raise_error(RuntimeError, "No backends available.")
 
         log.info(f"Using {cls._instance} backend on {cls._instance.device}")
         return cls._instance
 
     @classmethod
     def set_backend(cls, backend, platform=None, runcard=None):  # pragma: no cover
-        if cls._instance is None or cls._instance.name != backend or cls._instance.platform != platform:
+        if (
+            cls._instance is None
+            or cls._instance.name != backend
+            or cls._instance.platform != platform
+        ):
             cls._instance = construct_backend(backend, platform, runcard)
         log.info(f"Using {cls._instance} backend on {cls._instance.device}")
 
 
 class QiboMatrices:
-
     def __init__(self, dtype="complex128"):
         self.create(dtype)
 
     def create(self, dtype):
-        self.matrices = Matrices(dtype)
+        self.matrices = NumpyMatrices(dtype)
         self.I = self.matrices.I(2)
         self.X = self.matrices.X
         self.Y = self.matrices.Y
         self.Z = self.matrices.Z
 
 
 matrices = QiboMatrices()
@@ -114,16 +120,18 @@
 def get_device():
     return GlobalBackend().device
 
 
 def set_device(device):
     parts = device[1:].split(":")
     if device[0] != "/" or len(parts) < 2 or len(parts) > 3:
-        raise_error(ValueError, "Device name should follow the pattern: "
-                                "/{device type}:{device number}.")
+        raise_error(
+            ValueError,
+            "Device name should follow the pattern: " "/{device type}:{device number}.",
+        )
     backend = GlobalBackend()
     backend.set_device(device)
     log.info(f"Using {backend} backend on {backend.device}")
 
 
 def get_threads():
     return GlobalBackend().nthreads
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/abstract.py` & `qibo-0.1.9/src/qibo/backends/abstract.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
+
 from qibo.config import raise_error
 
 
 class Backend(abc.ABC):
-
     def __init__(self):
         super().__init__()
         self.name = "backend"
         self.platform = None
 
         self.precision = "double"
         self.dtype = "complex128"
@@ -21,184 +21,194 @@
     def __repr__(self):
         if self.platform is None:
             return self.name
         else:
             return f"{self.name} ({self.platform})"
 
     @abc.abstractmethod
-    def set_precision(self, precision): # pragma: no cover
+    def set_precision(self, precision):  # pragma: no cover
         """Set complex number precision.
 
         Args:
             precision (str): 'single' or 'double'.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def set_device(self, device): # pragma: no cover
+    def set_device(self, device):  # pragma: no cover
         """Set simulation device.
 
         Args:
             device (str): Device such as '/CPU:0', '/GPU:0', etc.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def set_threads(self, nthreads): # pragma: no cover
+    def set_threads(self, nthreads):  # pragma: no cover
         """Set number of threads for CPU simulation.
 
         Args:
             nthreads (int): Number of threads.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def cast(self, x, copy=False): # pragma: no cover
+    def cast(self, x, copy=False):  # pragma: no cover
         """Cast an object as the array type of the current backend.
 
         Args:
             x: Object to cast to array.
             copy (bool): If ``True`` a copy of the object is created in memory.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def issparse(self, x): # pragma: no cover
+    def issparse(self, x):  # pragma: no cover
         """Determine if a given array is a sparse tensor."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def to_numpy(self, x): # pragma: no cover
+    def to_numpy(self, x):  # pragma: no cover
         """Cast a given array to numpy."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def compile(self, func): # pragma: no cover
+    def compile(self, func):  # pragma: no cover
         """Compile the given method.
 
         Available only for the tensorflow backend.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def zero_state(self, nqubits): # pragma: no cover
+    def zero_state(self, nqubits):  # pragma: no cover
         """Generate |000...0> state vector as an array."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def zero_density_matrix(self, nqubits): # pragma: no cover
+    def zero_density_matrix(self, nqubits):  # pragma: no cover
         """Generate |000...0><000...0| density matrix as an array."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def plus_state(self, nqubits): # pragma: no cover
+    def plus_state(self, nqubits):  # pragma: no cover
         """Generate |+++...+> state vector as an array."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def plus_density_matrix(self, nqubits): # pragma: no cover
+    def plus_density_matrix(self, nqubits):  # pragma: no cover
         """Generate |+++...+><+++...+| density matrix as an array."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def asmatrix(self, gate): # pragma: no cover
+    def asmatrix(self, gate):  # pragma: no cover
         """Convert a :class:`qibo.gates.Gate` to the corresponding matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def asmatrix_parametrized(self, gate): # pragma: no cover
+    def asmatrix_parametrized(self, gate):  # pragma: no cover
         """Equivalent to :meth:`qibo.backends.abstract.Backend.asmatrix` for parametrized gates."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def asmatrix_fused(self, gate): # pragma: no cover
+    def asmatrix_fused(self, gate):  # pragma: no cover
         """Fuse matrices of multiple gates."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def control_matrix(self, gate): # pragma: no cover
-        """"Calculate full matrix representation of a controlled gate."""
+    def control_matrix(self, gate):  # pragma: no cover
+        """ "Calculate full matrix representation of a controlled gate."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def apply_gate(self, gate, state, nqubits): # pragma: no cover
+    def apply_gate(self, gate, state, nqubits):  # pragma: no cover
         """Apply a gate to state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def apply_gate_density_matrix(self, gate, state, nqubits): # pragma: no cover
+    def apply_gate_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         """Apply a gate to density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def apply_gate_half_density_matrix(self, gate, state, nqubits): # pragma: no cover
+    def apply_gate_half_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         """Apply a gate to one side of the density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def apply_channel(self, channel, state, nqubits): # pragma: no cover
+    def apply_channel(self, channel, state, nqubits):  # pragma: no cover
         """Apply a channel to state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def apply_channel_density_matrix(self, channel, state, nqubits): # pragma: no cover
+    def apply_channel_density_matrix(self, channel, state, nqubits):  # pragma: no cover
         """Apply a channel to density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def collapse_state(self, state, qubits, shot, nqubits, normalize=True): # pragma: no cover
+    def collapse_state(
+        self, state, qubits, shot, nqubits, normalize=True
+    ):  # pragma: no cover
         """Collapse state vector according to measurement shot."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def collapse_density_matrix(self, state, qubits, shot, nqubits, normalize=True): # pragma: no cover
+    def collapse_density_matrix(
+        self, state, qubits, shot, nqubits, normalize=True
+    ):  # pragma: no cover
         """Collapse density matrix according to measurement shot."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def reset_error_density_matrix(self, gate, state, nqubits): # pragma: no cover
+    def reset_error_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         """Apply reset error to density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def thermal_error_density_matrix(self, gate, state, nqubits): # pragma: no cover
+    def thermal_error_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         """Apply thermal relaxation error to density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def execute_circuit(self, circuit, initial_state=None, nshots=None): # pragma: no cover
+    def execute_circuit(
+        self, circuit, initial_state=None, nshots=None
+    ):  # pragma: no cover
         """Execute a :class:`qibo.models.circuit.Circuit`."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def execute_circuit_repeated(self, circuit, initial_state=None, nshots=None): # pragma: no cover
+    def execute_circuit_repeated(
+        self, circuit, initial_state=None, nshots=None
+    ):  # pragma: no cover
         """Execute a :class:`qibo.models.circuit.Circuit` multiple times.
 
         Useful for noise simulation using state vectors or for simulating gates
         controlled by measurement outcomes.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def execute_distributed_circuit(self, circuit, initial_state=None, nshots=None): # pragma: no cover
+    def execute_distributed_circuit(
+        self, circuit, initial_state=None, nshots=None
+    ):  # pragma: no cover
         """Execute a :class:`qibo.models.circuit.Circuit` using multiple GPUs."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def circuit_result_representation(self, result): # pragma: no cover
+    def circuit_result_representation(self, result):  # pragma: no cover
         """Represent a quantum state based on circuit execution results.
 
         Args:
             result (:class:`qibo.states.CircuitResult`): Result object that contains
                 the data required to represent the state.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def circuit_result_tensor(self, result): # pragma: no cover
+    def circuit_result_tensor(self, result):  # pragma: no cover
         """State vector or density matrix representing a quantum state as an array.
 
         Args:
             result (:class:`qibo.states.CircuitResult`): Result object that contains
                 the data required to represent the state.
         """
         raise_error(NotImplementedError)
@@ -211,148 +221,164 @@
             result (:class:`qibo.states.CircuitResult`): Result object that contains
                 the data required to represent the state.
             qubits (list, set): Set of qubits that are measured.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_symbolic(self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20): # pragma: no cover
+    def calculate_symbolic(
+        self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20
+    ):  # pragma: no cover
         """Dirac representation of a state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_symbolic_density_matrix(self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20): # pragma: no cover
+    def calculate_symbolic_density_matrix(
+        self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20
+    ):  # pragma: no cover
         """Dirac representation of a density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_probabilities(self, state, qubits, nqubits): # pragma: no cover
+    def calculate_probabilities(self, state, qubits, nqubits):  # pragma: no cover
         """Calculate probabilities given a state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_probabilities_density_matrix(self, state, qubits, nqubits): # pragma: no cover
+    def calculate_probabilities_density_matrix(
+        self, state, qubits, nqubits
+    ):  # pragma: no cover
         """Calculate probabilities given a density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def set_seed(self, seed): # pragma: no cover
+    def set_seed(self, seed):  # pragma: no cover
         """Set the seed of the random number generator."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def sample_shots(self, probabilities, nshots): # pragma: no cover
+    def sample_shots(self, probabilities, nshots):  # pragma: no cover
         """Sample measurement shots according to a probability distribution."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def aggregate_shots(self, shots): # pragma: no cover
+    def aggregate_shots(self, shots):  # pragma: no cover
         """Collect shots to a single array."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def samples_to_binary(self, samples, nqubits): # pragma: no cover
+    def samples_to_binary(self, samples, nqubits):  # pragma: no cover
         """Convert samples from decimal representation to binary."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def samples_to_decimal(self, samples, nqubits): # pragma: no cover
+    def samples_to_decimal(self, samples, nqubits):  # pragma: no cover
         """Convert samples from binary representation to decimal."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_frequencies(self, samples): # pragma: no cover
+    def calculate_frequencies(self, samples):  # pragma: no cover
         """Calculate measurement frequencies from shots."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def update_frequencies(self, frequencies, probabilities, nsamples): # pragma: no cover
+    def update_frequencies(
+        self, frequencies, probabilities, nsamples
+    ):  # pragma: no cover
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def sample_frequencies(self, probabilities, nshots): # pragma: no cover
+    def sample_frequencies(self, probabilities, nshots):  # pragma: no cover
         """Sample measurement frequencies according to a probability distribution."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def partial_trace(self, state, qubits, nqubits): # pragma: no cover
+    def partial_trace(self, state, qubits, nqubits):  # pragma: no cover
         """Trace out specific qubits of a state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def partial_trace_density_matrix(self, state, qubits, nqubits): # pragma: no cover
+    def partial_trace_density_matrix(self, state, qubits, nqubits):  # pragma: no cover
         """Trace out specific qubits of a density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def entanglement_entropy(self, rho): # pragma: no cover
+    def entanglement_entropy(self, rho):  # pragma: no cover
         """Calculate entangelement entropy of a reduced density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_norm(self, state): # pragma: no cover
+    def calculate_norm(self, state):  # pragma: no cover
         """Calculate norm of a state vector."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_norm_density_matrix(self, state): # pragma: no cover
+    def calculate_norm_density_matrix(self, state):  # pragma: no cover
         """Calculate norm (trace) of a density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_overlap(self, state1, state2): # pragma: no cover
+    def calculate_overlap(self, state1, state2):  # pragma: no cover
         """Calculate overlap of two state vectors."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_overlap_density_matrix(self, state1, state2): # pragma: no cover
+    def calculate_overlap_density_matrix(self, state1, state2):  # pragma: no cover
         """Calculate norm of two density matrices."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_eigenvalues(self, matrix, k=6): # pragma: no cover
+    def calculate_eigenvalues(self, matrix, k=6):  # pragma: no cover
         """Calculate eigenvalues of a matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_eigenvectors(self, matrix, k=6): # pragma: no cover
+    def calculate_eigenvectors(self, matrix, k=6):  # pragma: no cover
         """Calculate eigenvectors of a matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_matrix_exp(self, matrix, a, eigenvectors=None, eigenvalues=None): # pragma: no cover
+    def calculate_matrix_exp(
+        self, matrix, a, eigenvectors=None, eigenvalues=None
+    ):  # pragma: no cover
         """Calculate matrix exponential of a matrix.
 
         If the eigenvectors and eigenvalues are given the matrix diagonalization is
         used for exponentiation.
         """
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_expectation_state(self, matrix, state, normalize): # pragma: no cover
+    def calculate_expectation_state(
+        self, hamiltonian, state, normalize
+    ):  # pragma: no cover
         """Calculate expectation value of a state vector given the observable matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_expectation_density_matrix(self, matrix, state, normalize): # pragma: no cover
+    def calculate_expectation_density_matrix(
+        self, hamiltonian, state, normalize
+    ):  # pragma: no cover
         """Calculate expectation value of a density matrix given the observable matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_hamiltonian_matrix_product(self, matrix1, matrix2): # pragma: no cover
+    def calculate_hamiltonian_matrix_product(
+        self, matrix1, matrix2
+    ):  # pragma: no cover
         """Multiply two matrices."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def calculate_hamiltonian_state_product(self, matrix, state): # pragma: no cover
+    def calculate_hamiltonian_state_product(self, matrix, state):  # pragma: no cover
         """Multiply a matrix to a state vector or density matrix."""
         raise_error(NotImplementedError)
 
     @abc.abstractmethod
-    def assert_allclose(self, value, target, rtol=1e-7, atol=0.0): # pragma: no cover
+    def assert_allclose(self, value, target, rtol=1e-7, atol=0.0):  # pragma: no cover
         raise_error(NotImplementedError)
 
     def assert_circuitclose(self, circuit, target_circuit, rtol=1e-7, atol=0.0):
         value = self.execute_circuit(circuit)
         target = self.execute_circuit(target_circuit)
         self.assert_allclose(value, target, rtol=rtol, atol=atol)
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/einsum_utils.py` & `qibo-0.1.9/src/qibo/backends/einsum_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 """
 Gates use ``einsum`` to apply gates to state vectors. The einsum string that
-specifies the contraction indices is created using the following methods and 
+specifies the contraction indices is created using the following methods and
 used by :meth:`qibo.backends.numpy.NumpyEngine.apply_gate`.
 """
-from qibo.config import raise_error, EINSUM_CHARS
+from qibo.config import EINSUM_CHARS, raise_error
 
 
 def prepare_strings(qubits, nqubits):
-    if nqubits + len(qubits) > len(EINSUM_CHARS): # pragma: no cover
+    if nqubits + len(qubits) > len(EINSUM_CHARS):  # pragma: no cover
         raise_error(NotImplementedError, "Not enough einsum characters.")
 
     inp = list(EINSUM_CHARS[:nqubits])
     out = inp[:]
     trans = list(EINSUM_CHARS[nqubits : nqubits + len(qubits)])
     for i, q in enumerate(qubits):
         trans.append(inp[q])
         out[q] = trans[i]
 
     inp = "".join(inp)
     out = "".join(out)
     trans = "".join(trans)
-    rest = EINSUM_CHARS[nqubits + len(qubits):]
+    rest = EINSUM_CHARS[nqubits + len(qubits) :]
     return inp, out, trans, rest
 
 
 def apply_gate_string(qubits, nqubits):
     inp, out, trans, _ = prepare_strings(qubits, nqubits)
     return f"{inp},{trans}->{out}"
 
 
 def apply_gate_density_matrix_string(qubits, nqubits):
     inp, out, trans, rest = prepare_strings(qubits, nqubits)
-    if nqubits > len(rest): # pragma: no cover
+    if nqubits > len(rest):  # pragma: no cover
         raise_error(NotImplementedError, "Not enough einsum characters.")
-    
+
     trest = rest[:nqubits]
     left = f"{inp}{trest},{trans}->{out}{trest}"
     right = f"{trest}{inp},{trans}->{trest}{out}"
     return left, right
 
 
 def apply_gate_density_matrix_controlled_string(qubits, nqubits):
     inp, out, trans, rest = prepare_strings(qubits, nqubits)
-    if nqubits > len(rest): # pragma: no cover
+    if nqubits > len(rest):  # pragma: no cover
         raise_error(NotImplementedError, "Not enough einsum characters.")
-    
+
     trest, c = rest[:nqubits], rest[nqubits]
     left = f"{c}{inp}{trest},{trans}->{c}{out}{trest}"
     right = f"{c}{trest}{inp},{trans}->{c}{trest}{out}"
     return left, right
 
 
 def control_order(gate, nqubits):
@@ -67,18 +67,20 @@
     return order, targets
 
 
 def control_order_density_matrix(gate, nqubits):
     ncontrol = len(gate.control_qubits)
     order, targets = control_order(gate, nqubits)
     additional_order = [x + len(order) for x in order]
-    order_dm = (order[:ncontrol] +
-                list(additional_order[:ncontrol]) +
-                order[ncontrol:] +
-                list(additional_order[ncontrol:]))
+    order_dm = (
+        order[:ncontrol]
+        + list(additional_order[:ncontrol])
+        + order[ncontrol:]
+        + list(additional_order[ncontrol:])
+    )
     return order_dm, targets
 
 
 def reverse_order(order):
     rorder = len(order) * [0]
     for i, r in enumerate(order):
         rorder[r] = i
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/matrices.py` & `qibo-0.1.9/src/qibo/backends/npmatrices.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 import sys
+
 from qibo.config import raise_error
 
 if sys.version_info.minor >= 8:
     from functools import cached_property  # pylint: disable=E0611
 else:  # pragma: no cover
     # Custom ``cached_property`` because it is not available for Python < 3.8
     from functools import lru_cache
+
     def cached_property(func):
         @property
         def wrapper(self):
             return lru_cache()(func)(self)
+
         return wrapper
 
 
-class Matrices:
+class NumpyMatrices:
     """Matrix representation of every gate as a numpy array."""
 
     def __init__(self, dtype):
         import numpy as np
+
         self.dtype = dtype
         self.np = np
 
     @cached_property
     def H(self):
-        return self.np.array([
-            [1, 1],
-            [1, -1]
-        ], dtype=self.dtype) / self.np.sqrt(2)
+        return self.np.array([[1, 1], [1, -1]], dtype=self.dtype) / self.np.sqrt(2)
 
     @cached_property
     def X(self):
-        return self.np.array([
-            [0, 1],
-            [1, 0]
-        ], dtype=self.dtype)
+        return self.np.array([[0, 1], [1, 0]], dtype=self.dtype)
 
     @cached_property
     def Y(self):
-        return self.np.array([
-            [0, -1j],
-            [1j, 0]
-        ], dtype=self.dtype)
+        return self.np.array([[0, -1j], [1j, 0]], dtype=self.dtype)
 
     @cached_property
     def Z(self):
-        return self.np.array([
-            [1, 0],
-            [0, -1]
-        ], dtype=self.dtype)
+        return self.np.array([[1, 0], [0, -1]], dtype=self.dtype)
 
     @cached_property
     def S(self):
-        return self.np.array([
-            [1, 0],
-            [0, 1j]
-        ], dtype=self.dtype)
+        return self.np.array([[1, 0], [0, 1j]], dtype=self.dtype)
 
     @cached_property
     def SDG(self):
         return self.np.conj(self.S)
 
     @cached_property
     def T(self):
-        return self.np.array([
-            [1, 0],
-            [0, self.np.exp(1j * self.np.pi / 4.0)]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [[1, 0], [0, self.np.exp(1j * self.np.pi / 4.0)]], dtype=self.dtype
+        )
 
     @cached_property
     def TDG(self):
         return self.np.conj(self.T)
 
     def I(self, n=2):
         return self.np.eye(n, dtype=self.dtype)
@@ -79,76 +67,61 @@
 
     def M(self):  # pragma: no cover
         raise_error(NotImplementedError)
 
     def RX(self, theta):
         cos = self.np.cos(theta / 2.0) + 0j
         isin = -1j * self.np.sin(theta / 2.0)
-        return self.np.array([
-            [cos, isin],
-            [isin, cos]
-        ], dtype=self.dtype)
+        return self.np.array([[cos, isin], [isin, cos]], dtype=self.dtype)
 
     def RY(self, theta):
         cos = self.np.cos(theta / 2.0) + 0j
         sin = self.np.sin(theta / 2.0)
-        return self.np.array([
-            [cos, -sin],
-            [sin, cos]
-        ], dtype=self.dtype)
+        return self.np.array([[cos, -sin], [sin, cos]], dtype=self.dtype)
 
     def RZ(self, theta):
         phase = self.np.exp(0.5j * theta)
-        return self.np.array([
-            [self.np.conj(phase), 0],
-            [0, phase]
-        ], dtype=self.dtype)
+        return self.np.array([[self.np.conj(phase), 0], [0, phase]], dtype=self.dtype)
 
     def U1(self, theta):
         phase = self.np.exp(1j * theta)
-        return self.np.array([
-            [1, 0],
-            [0, phase]
-        ], dtype=self.dtype)
+        return self.np.array([[1, 0], [0, phase]], dtype=self.dtype)
 
     def U2(self, phi, lam):
         eplus = self.np.exp(1j * (phi + lam) / 2.0)
         eminus = self.np.exp(1j * (phi - lam) / 2.0)
-        return self.np.array([
-            [self.np.conj(eplus), - self.np.conj(eminus)],
-            [eminus, eplus]
-        ], dtype=self.dtype) / self.np.sqrt(2)
+        return self.np.array(
+            [[self.np.conj(eplus), -self.np.conj(eminus)], [eminus, eplus]],
+            dtype=self.dtype,
+        ) / self.np.sqrt(2)
 
     def U3(self, theta, phi, lam):
         cost = self.np.cos(theta / 2)
         sint = self.np.sin(theta / 2)
         eplus = self.np.exp(1j * (phi + lam) / 2.0)
         eminus = self.np.exp(1j * (phi - lam) / 2.0)
-        return self.np.array([
-            [self.np.conj(eplus) * cost, - self.np.conj(eminus) * sint],
-            [eminus * sint, eplus * cost]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [
+                [self.np.conj(eplus) * cost, -self.np.conj(eminus) * sint],
+                [eminus * sint, eplus * cost],
+            ],
+            dtype=self.dtype,
+        )
 
     @cached_property
     def CNOT(self):
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, 0, 1],
-            [0, 0, 1, 0]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]], dtype=self.dtype
+        )
 
     @cached_property
     def CZ(self):
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, 1, 0],
-            [0, 0, 0, -1]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]], dtype=self.dtype
+        )
 
     def CRX(self, theta):
         m = self.np.eye(4, dtype=self.dtype)
         m[2:, 2:] = self.RX(theta)
         return m
 
     def CRY(self, theta):
@@ -174,62 +147,102 @@
     def CU3(self, theta, phi, lam):
         m = self.np.eye(4, dtype=self.dtype)
         m[2:, 2:] = self.U3(theta, phi, lam)
         return m
 
     @cached_property
     def SWAP(self):
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, 0, 1, 0],
-            [0, 1, 0, 0],
-            [0, 0, 0, 1]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]], dtype=self.dtype
+        )
 
     @cached_property
     def FSWAP(self):
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, 0, 1, 0],
-            [0, 1, 0, 0],
-            [0, 0, 0, -1]
-        ], dtype=self.dtype)
+        return self.np.array(
+            [[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, -1]], dtype=self.dtype
+        )
 
     def fSim(self, theta, phi):
         cost = self.np.cos(theta) + 0j
         isint = -1j * self.np.sin(theta)
         phase = self.np.exp(-1j * phi)
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, cost, isint, 0],
-            [0, isint, cost, 0],
-            [0, 0, 0, phase],
-        ], dtype=self.dtype)
+        return self.np.array(
+            [
+                [1, 0, 0, 0],
+                [0, cost, isint, 0],
+                [0, isint, cost, 0],
+                [0, 0, 0, phase],
+            ],
+            dtype=self.dtype,
+        )
 
     def GeneralizedfSim(self, u, phi):
         phase = self.np.exp(-1j * phi)
-        return self.np.array([
-            [1, 0, 0, 0],
-            [0, u[0, 0], u[0, 1], 0],
-            [0, u[1, 0], u[1, 1], 0],
-            [0, 0, 0, phase],
-        ], dtype=self.dtype)
+        return self.np.array(
+            [
+                [1, 0, 0, 0],
+                [0, u[0, 0], u[0, 1], 0],
+                [0, u[1, 0], u[1, 1], 0],
+                [0, 0, 0, phase],
+            ],
+            dtype=self.dtype,
+        )
+
+    def RXX(self, theta):
+        cos = self.np.cos(theta / 2.0) + 0j
+        isin = -1j * self.np.sin(theta / 2.0)
+        return self.np.array(
+            [
+                [cos, 0, 0, isin],
+                [0, cos, isin, 0],
+                [0, isin, cos, 0],
+                [isin, 0, 0, cos],
+            ],
+            dtype=self.dtype,
+        )
+
+    def RYY(self, theta):
+        cos = self.np.cos(theta / 2.0) + 0j
+        isin = -1j * self.np.sin(theta / 2.0)
+        return self.np.array(
+            [
+                [cos, 0, 0, -isin],
+                [0, cos, isin, 0],
+                [0, isin, cos, 0],
+                [-isin, 0, 0, cos],
+            ],
+            dtype=self.dtype,
+        )
+
+    def RZZ(self, theta):
+        phase = self.np.exp(0.5j * theta)
+        return self.np.array(
+            [
+                [self.np.conj(phase), 0, 0, 0],
+                [0, phase, 0, 0],
+                [0, 0, phase, 0],
+                [0, 0, 0, self.np.conj(phase)],
+            ],
+            dtype=self.dtype,
+        )
 
     @cached_property
     def TOFFOLI(self):
-        return self.np.array([
-            [1, 0, 0, 0, 0, 0, 0, 0],
-            [0, 1, 0, 0, 0, 0, 0, 0],
-            [0, 0, 1, 0, 0, 0, 0, 0],
-            [0, 0, 0, 1, 0, 0, 0, 0],
-            [0, 0, 0, 0, 1, 0, 0, 0],
-            [0, 0, 0, 0, 0, 1, 0, 0],
-            [0, 0, 0, 0, 0, 0, 0, 1],
-            [0, 0, 0, 0, 0, 0, 1, 0],
-        ])
+        return self.np.array(
+            [
+                [1, 0, 0, 0, 0, 0, 0, 0],
+                [0, 1, 0, 0, 0, 0, 0, 0],
+                [0, 0, 1, 0, 0, 0, 0, 0],
+                [0, 0, 0, 1, 0, 0, 0, 0],
+                [0, 0, 0, 0, 1, 0, 0, 0],
+                [0, 0, 0, 0, 0, 1, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0, 1],
+                [0, 0, 0, 0, 0, 0, 1, 0],
+            ]
+        )
 
     def Unitary(self, u):
         return self.np.array(u, dtype=self.dtype, copy=False)
 
     def CallbackGate(self):  # pragma: no cover
         raise_error(NotImplementedError)
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/numpy.py` & `qibo-0.1.9/src/qibo/backends/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,40 @@
-import numpy as np
 import collections
-from qibo.config import raise_error, log
-from qibo.gates import FusedGate
-from qibo.states import CircuitResult
+
+import numpy as np
+
+from qibo import __version__
 from qibo.backends import einsum_utils
 from qibo.backends.abstract import Backend
-from qibo.backends.matrices import Matrices
+from qibo.backends.npmatrices import NumpyMatrices
+from qibo.config import log, raise_error
+from qibo.gates import FusedGate
 from qibo.gates.abstract import ParametrizedGate, SpecialGate
+from qibo.states import CircuitResult
 
 
 class NumpyBackend(Backend):
-
     def __init__(self):
         super().__init__()
         self.np = np
         self.name = "numpy"
-        self.matrices = Matrices(self.dtype)
+        self.matrices = NumpyMatrices(self.dtype)
         self.tensor_types = np.ndarray
-        self.numeric_types = (int, float, complex, np.int32,
-                              np.int64, np.float32, np.float64,
-                              np.complex64, np.complex128)
+        self.versions = {"qibo": __version__, "numpy": self.np.__version__}
+        self.numeric_types = (
+            int,
+            float,
+            complex,
+            np.int32,
+            np.int64,
+            np.float32,
+            np.float64,
+            np.complex64,
+            np.complex128,
+        )
 
     def set_precision(self, precision):
         if precision != self.precision:
             if precision == "single":
                 self.precision = precision
                 self.dtype = "complex64"
             elif precision == "double":
@@ -32,15 +43,17 @@
             else:
                 raise_error(ValueError, f"Unknown precision {precision}.")
             if self.matrices:
                 self.matrices = self.matrices.__class__(self.dtype)
 
     def set_device(self, device):
         if device != "/CPU:0":
-            raise_error(ValueError, f"Device {device} is not available for {self} backend.")
+            raise_error(
+                ValueError, f"Device {device} is not available for {self} backend."
+            )
 
     def set_threads(self, nthreads):
         if nthreads > 1:
             raise_error(ValueError, "numpy does not support more than one thread.")
 
     def cast(self, x, dtype=None, copy=False):
         if dtype is None:
@@ -49,57 +62,58 @@
             return x.astype(dtype, copy=copy)
         elif self.issparse(x):
             return x.astype(dtype, copy=copy)
         return np.array(x, dtype=dtype, copy=copy)
 
     def issparse(self, x):
         from scipy import sparse
+
         return sparse.issparse(x)
 
     def to_numpy(self, x):
         if self.issparse(x):
             return x.toarray()
         return x
 
     def compile(self, func):
         return func
 
     def zero_state(self, nqubits):
-        state = self.np.zeros(2 ** nqubits, dtype=self.dtype)
+        state = self.np.zeros(2**nqubits, dtype=self.dtype)
         state[0] = 1
         return state
 
     def zero_density_matrix(self, nqubits):
-        state = self.np.zeros(2 * (2 ** nqubits,), dtype=self.dtype)
+        state = self.np.zeros(2 * (2**nqubits,), dtype=self.dtype)
         state[0, 0] = 1
         return state
 
     def plus_state(self, nqubits):
-        state = self.np.ones(2 ** nqubits, dtype=self.dtype)
-        state /= self.np.sqrt(2 ** nqubits)
+        state = self.np.ones(2**nqubits, dtype=self.dtype)
+        state /= self.np.sqrt(2**nqubits)
         return state
 
     def plus_density_matrix(self, nqubits):
-        state = self.np.ones(2 * (2 ** nqubits,), dtype=self.dtype)
-        state /= 2 ** nqubits
+        state = self.np.ones(2 * (2**nqubits,), dtype=self.dtype)
+        state /= 2**nqubits
         return state
 
     def asmatrix(self, gate):
         """Convert a gate to its matrix representation in the computational basis."""
         name = gate.__class__.__name__
         return getattr(self.matrices, name)
 
     def asmatrix_parametrized(self, gate):
         """Convert a parametrized gate to its matrix representation in the computational basis."""
         name = gate.__class__.__name__
         return getattr(self.matrices, name)(*gate.parameters)
 
     def asmatrix_fused(self, fgate):
         rank = len(fgate.target_qubits)
-        matrix = np.eye(2 ** rank, dtype=self.dtype)
+        matrix = np.eye(2**rank, dtype=self.dtype)
         for gate in fgate.gates:
             # transfer gate matrix to numpy as it is more efficient for
             # small tensor calculations
             gmatrix = gate.asmatrix(self)
             # Kronecker product with identity is needed to make the
             # original matrix have shape (2**rank x 2**rank)
             eye = np.eye(2 ** (rank - len(gate.qubits)), dtype=self.dtype)
@@ -117,108 +131,127 @@
             gmatrix = np.reshape(gmatrix, original_shape)
             # fuse the individual gate matrix to the total ``FusedGate`` matrix
             matrix = gmatrix @ matrix
         return matrix
 
     def control_matrix(self, gate):
         if len(gate.control_qubits) > 1:
-            raise_error(NotImplementedError, "Cannot calculate controlled "
-                                             "unitary for more than two "
-                                             "control qubits.")
+            raise_error(
+                NotImplementedError,
+                "Cannot calculate controlled "
+                "unitary for more than two "
+                "control qubits.",
+            )
         matrix = gate.asmatrix(self)
         shape = matrix.shape
         if shape != (2, 2):
-            raise_error(ValueError, "Cannot use ``control_unitary`` method on "
-                                    "gate matrix of shape {}.".format(shape))
+            raise_error(
+                ValueError,
+                "Cannot use ``control_unitary`` method on "
+                "gate matrix of shape {}.".format(shape),
+            )
         zeros = self.np.zeros((2, 2), dtype=self.dtype)
         part1 = self.np.concatenate([self.np.eye(2, dtype=self.dtype), zeros], axis=0)
         part2 = self.np.concatenate([zeros, matrix], axis=0)
         return self.np.concatenate([part1, part2], axis=1)
 
     def apply_gate(self, gate, state, nqubits):
         state = self.cast(state)
         state = self.np.reshape(state, nqubits * (2,))
         matrix = gate.asmatrix(self)
         if gate.is_controlled_by:
-            matrix = self.np.reshape(matrix, 2  * len(gate.target_qubits) * (2,))
+            matrix = self.np.reshape(matrix, 2 * len(gate.target_qubits) * (2,))
             ncontrol = len(gate.control_qubits)
             nactive = nqubits - ncontrol
             order, targets = einsum_utils.control_order(gate, nqubits)
             state = self.np.transpose(state, order)
             # Apply `einsum` only to the part of the state where all controls
             # are active. This should be `state[-1]`
-            state = self.np.reshape(state, (2 ** ncontrol,) + nactive * (2,))
+            state = self.np.reshape(state, (2**ncontrol,) + nactive * (2,))
             opstring = einsum_utils.apply_gate_string(targets, nactive)
             updates = self.np.einsum(opstring, state[-1], matrix)
             # Concatenate the updated part of the state `updates` with the
             # part of of the state that remained unaffected `state[:-1]`.
             state = self.np.concatenate([state[:-1], updates[self.np.newaxis]], axis=0)
             state = self.np.reshape(state, nqubits * (2,))
             # Put qubit indices back to their proper places
             state = self.np.transpose(state, einsum_utils.reverse_order(order))
         else:
-            matrix = self.np.reshape(matrix, 2  * len(gate.qubits) * (2,))
+            matrix = self.np.reshape(matrix, 2 * len(gate.qubits) * (2,))
             opstring = einsum_utils.apply_gate_string(gate.qubits, nqubits)
             state = self.np.einsum(opstring, state, matrix)
-        return self.np.reshape(state, (2 ** nqubits,))
+        return self.np.reshape(state, (2**nqubits,))
 
     def apply_gate_density_matrix(self, gate, state, nqubits):
         state = self.cast(state)
         state = self.np.reshape(state, 2 * nqubits * (2,))
         matrix = gate.asmatrix(self)
         if gate.is_controlled_by:
-            matrix = self.np.reshape(matrix, 2  * len(gate.target_qubits) * (2,))
+            matrix = self.np.reshape(matrix, 2 * len(gate.target_qubits) * (2,))
             matrixc = self.np.conj(matrix)
             ncontrol = len(gate.control_qubits)
             nactive = nqubits - ncontrol
-            n = 2 ** ncontrol
+            n = 2**ncontrol
 
             order, targets = einsum_utils.control_order_density_matrix(gate, nqubits)
             state = self.np.transpose(state, order)
             state = self.np.reshape(state, 2 * (n,) + 2 * nactive * (2,))
 
-            leftc, rightc = einsum_utils.apply_gate_density_matrix_controlled_string(targets, nactive)
-            state01 = state[:n - 1, n - 1]
+            leftc, rightc = einsum_utils.apply_gate_density_matrix_controlled_string(
+                targets, nactive
+            )
+            state01 = state[: n - 1, n - 1]
             state01 = self.np.einsum(rightc, state01, matrixc)
-            state10 = state[n - 1, :n - 1]
+            state10 = state[n - 1, : n - 1]
             state10 = self.np.einsum(leftc, state10, matrix)
 
-            left, right = einsum_utils.apply_gate_density_matrix_string(targets, nactive)
+            left, right = einsum_utils.apply_gate_density_matrix_string(
+                targets, nactive
+            )
             state11 = state[n - 1, n - 1]
             state11 = self.np.einsum(right, state11, matrixc)
             state11 = self.np.einsum(left, state11, matrix)
 
             state00 = state[range(n - 1)]
             state00 = state00[:, range(n - 1)]
-            state01 = self.np.concatenate([state00, state01[:, self.np.newaxis]], axis=1)
+            state01 = self.np.concatenate(
+                [state00, state01[:, self.np.newaxis]], axis=1
+            )
             state10 = self.np.concatenate([state10, state11[self.np.newaxis]], axis=0)
             state = self.np.concatenate([state01, state10[self.np.newaxis]], axis=0)
             state = self.np.reshape(state, 2 * nqubits * (2,))
             state = self.np.transpose(state, einsum_utils.reverse_order(order))
         else:
             matrix = self.np.reshape(matrix, 2 * len(gate.qubits) * (2,))
             matrixc = self.np.conj(matrix)
-            left, right = einsum_utils.apply_gate_density_matrix_string(gate.qubits, nqubits)
+            left, right = einsum_utils.apply_gate_density_matrix_string(
+                gate.qubits, nqubits
+            )
             state = self.np.einsum(right, state, matrixc)
             state = self.np.einsum(left, state, matrix)
-        return self.np.reshape(state, 2 * (2 ** nqubits,))
+        return self.np.reshape(state, 2 * (2**nqubits,))
 
     def apply_gate_half_density_matrix(self, gate, state, nqubits):
         state = self.cast(state)
         state = np.reshape(state, 2 * nqubits * (2,))
         matrix = gate.asmatrix(self)
-        if gate.is_controlled_by: # pragma: no cover
-            raise_error(NotImplementedError, "Gate density matrix half call is "
-                                             "not implemented for ``controlled_by``"
-                                             "gates.")
+        if gate.is_controlled_by:  # pragma: no cover
+            raise_error(
+                NotImplementedError,
+                "Gate density matrix half call is "
+                "not implemented for ``controlled_by``"
+                "gates.",
+            )
         else:
             matrix = np.reshape(matrix, 2 * len(gate.qubits) * (2,))
-            left, _ = einsum_utils.apply_gate_density_matrix_string(gate.qubits, nqubits)
+            left, _ = einsum_utils.apply_gate_density_matrix_string(
+                gate.qubits, nqubits
+            )
             state = np.einsum(left, state, matrix)
-        return np.reshape(state, 2 * (2 ** nqubits,))
+        return np.reshape(state, 2 * (2**nqubits,))
 
     def apply_channel(self, channel, state, nqubits):
         for coeff, gate in zip(channel.coefficients, channel.gates):
             if self.np.random.random() < coeff:
                 state = self.apply_gate(gate, state, nqubits)
         return state
 
@@ -271,14 +304,15 @@
             state = state / norm
         qubits = qubits + [q + nqubits for q in qubits]
         state = self._append_zeros(state, qubits, 2 * binshot)
         return self.np.reshape(state, shape)
 
     def reset_error_density_matrix(self, gate, state, nqubits):
         from qibo.gates import X
+
         state = self.cast(state)
         shape = state.shape
         q = gate.target_qubits[0]
         p0, p1 = gate.coefficients[:2]
         trace = self.partial_trace_density_matrix(state, (q,), nqubits)
         trace = self.np.reshape(trace, 2 * (nqubits - 1) * (2,))
         zero = self.zero_density_matrix(1)
@@ -292,15 +326,17 @@
 
     def thermal_error_density_matrix(self, gate, state, nqubits):
         state = self.cast(state)
         shape = state.shape
         state = self.apply_gate(gate, state.ravel(), 2 * nqubits)
         return self.np.reshape(state, shape)
 
-    def execute_circuit(self, circuit, initial_state=None, nshots=None, return_array=False):
+    def execute_circuit(
+        self, circuit, initial_state=None, nshots=None, return_array=False
+    ):
         if circuit.repeated_execution:
             return self.execute_circuit_repeated(circuit, initial_state, nshots)
 
         if circuit.accelerators:  # pragma: no cover
             return self.execute_distributed_circuit(circuit, initial_state, nshots)
 
         try:
@@ -331,17 +367,20 @@
             if return_array:
                 return state
             else:
                 circuit._final_state = CircuitResult(self, circuit, state, nshots)
                 return circuit._final_state
 
         except self.oom_error:
-            raise_error(RuntimeError, f"State does not fit in {self.device} memory."
-                                       "Please switch the execution device to a "
-                                       "different one using ``qibo.set_device``.")
+            raise_error(
+                RuntimeError,
+                f"State does not fit in {self.device} memory."
+                "Please switch the execution device to a "
+                "different one using ``qibo.set_device``.",
+            )
 
     def execute_circuit_repeated(self, circuit, initial_state=None, nshots=None):
         if nshots is None:
             nshots = 1
 
         results = []
         nqubits = circuit.nqubits
@@ -355,15 +394,17 @@
                 for gate in circuit.queue:
                     if gate.symbolic_parameters:
                         gate.substitute_symbols()
                     state = gate.apply_density_matrix(self, state, nqubits)
 
             else:
                 if circuit.accelerators:  # pragma: no cover
-                    state = self.execute_distributed_circuit(circuit, initial_state, return_array=True) # pylint: disable=E1111
+                    state = self.execute_distributed_circuit(
+                        circuit, initial_state, return_array=True
+                    )  # pylint: disable=E1111
                 else:
                     if initial_state is None:
                         state = self.zero_state(nqubits)
                     else:
                         state = self.cast(initial_state, copy=True)
 
                     for gate in circuit.queue:
@@ -382,47 +423,57 @@
             final_result._samples = self.aggregate_shots(results)
             circuit._final_state = final_result
             return final_result
         else:
             circuit._final_state = CircuitResult(self, circuit, results[-1], nshots)
             return results
 
-    def execute_distributed_circuit(self, circuit, initial_state=None, nshots=None, return_array=False):
-        raise_error(NotImplementedError, f"{self} does not support distributed execution.")
+    def execute_distributed_circuit(
+        self, circuit, initial_state=None, nshots=None, return_array=False
+    ):
+        raise_error(
+            NotImplementedError, f"{self} does not support distributed execution."
+        )
 
     def circuit_result_representation(self, result):
         return result.symbolic()
 
     def circuit_result_tensor(self, result):
         return result.execution_result
 
     def circuit_result_probabilities(self, result, qubits=None):
         if qubits is None:  # pragma: no cover
             qubits = result.circuit.measurement_gate.qubits
 
         state = self.circuit_result_tensor(result)
         if result.density_matrix:
-            return self.calculate_probabilities_density_matrix(state, qubits, result.nqubits)
+            return self.calculate_probabilities_density_matrix(
+                state, qubits, result.nqubits
+            )
         else:
             return self.calculate_probabilities(state, qubits, result.nqubits)
 
-    def calculate_symbolic(self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20):
+    def calculate_symbolic(
+        self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20
+    ):
         state = self.to_numpy(state)
         terms = []
         for i in np.nonzero(state)[0]:
             b = bin(i)[2:].zfill(nqubits)
             if np.abs(state[i]) >= cutoff:
                 x = round(state[i], decimals)
                 terms.append(f"{x}|{b}>")
             if len(terms) >= max_terms:
                 terms.append("...")
                 return terms
         return terms
 
-    def calculate_symbolic_density_matrix(self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20):
+    def calculate_symbolic_density_matrix(
+        self, state, nqubits, decimals=5, cutoff=1e-10, max_terms=20
+    ):
         state = self.to_numpy(state)
         terms = []
         indi, indj = np.nonzero(state)
         for i, j in zip(indi, indj):
             bi = bin(i)[2:].zfill(nqubits)
             bj = bin(j)[2:].zfill(nqubits)
             if np.abs(state[i, j]) >= cutoff:
@@ -462,26 +513,28 @@
         probs = self.np.reshape(probs, len(qubits) * (2,))
         return self._order_probabilities(probs, qubits, nqubits).ravel()
 
     def set_seed(self, seed):
         self.np.random.seed(seed)
 
     def sample_shots(self, probabilities, nshots):
-        return self.np.random.choice(range(len(probabilities)), size=nshots, p=probabilities)
+        return self.np.random.choice(
+            range(len(probabilities)), size=nshots, p=probabilities
+        )
 
     def aggregate_shots(self, shots):
         return self.np.array(shots, dtype=shots[0].dtype)
 
     def samples_to_binary(self, samples, nqubits):
         qrange = self.np.arange(nqubits - 1, -1, -1, dtype="int32")
         return self.np.mod(self.np.right_shift(samples[:, self.np.newaxis], qrange), 2)
 
     def samples_to_decimal(self, samples, nqubits):
         qrange = self.np.arange(nqubits - 1, -1, -1, dtype="int32")
-        qrange = (2 ** qrange)[:, self.np.newaxis]
+        qrange = (2**qrange)[:, self.np.newaxis]
         return self.np.matmul(samples, qrange)[:, 0]
 
     def calculate_frequencies(self, samples):
         res, counts = self.np.unique(samples, return_counts=True)
         res, counts = self.np.array(res), self.np.array(counts)
         return collections.Counter({k: v for k, v in zip(res, counts)})
 
@@ -489,19 +542,22 @@
         samples = self.sample_shots(probabilities, nsamples)
         res, counts = self.np.unique(samples, return_counts=True)
         frequencies[res] += counts
         return frequencies
 
     def sample_frequencies(self, probabilities, nshots):
         from qibo.config import SHOT_BATCH_SIZE
+
         nprobs = probabilities / self.np.sum(probabilities)
         frequencies = self.np.zeros(len(nprobs), dtype="int64")
         for _ in range(nshots // SHOT_BATCH_SIZE):
             frequencies = self.update_frequencies(frequencies, nprobs, SHOT_BATCH_SIZE)
-        frequencies = self.update_frequencies(frequencies, nprobs, nshots % SHOT_BATCH_SIZE)
+        frequencies = self.update_frequencies(
+            frequencies, nprobs, nshots % SHOT_BATCH_SIZE
+        )
         return collections.Counter({i: f for i, f in enumerate(frequencies) if f > 0})
 
     def apply_bitflips(self, noiseless_samples, bitflip_probabilities):
         fprobs = self.np.array(bitflip_probabilities, dtype="float64")
         sprobs = self.np.random.random(noiseless_samples.shape)
         flip0 = self.np.array(sprobs < fprobs[0], dtype=noiseless_samples.dtype)
         flip1 = self.np.array(sprobs < fprobs[1], dtype=noiseless_samples.dtype)
@@ -528,14 +584,15 @@
 
         state = self.np.transpose(state, order)
         state = self.np.reshape(state, shape)
         return self.np.einsum("abac->bc", state)
 
     def entanglement_entropy(self, rho):
         from qibo.config import EIGVAL_CUTOFF
+
         # Diagonalize
         eigvals = self.np.linalg.eigvalsh(rho).real
         # Treating zero and negative eigenvalues
         masked_eigvals = eigvals[eigvals > EIGVAL_CUTOFF]
         spectrum = -1 * self.np.log(masked_eigvals)
         entropy = self.np.sum(masked_eigvals * spectrum) / self.np.log(2.0)
         return entropy, spectrum
@@ -554,24 +611,27 @@
         return self.np.abs(self.np.sum(self.np.conj(state1) * state2))
 
     def calculate_overlap_density_matrix(self, state1, state2):
         raise_error(NotImplementedError)
 
     def calculate_eigenvalues(self, matrix, k=6):
         if self.issparse(matrix):
-            log.warning("Calculating sparse matrix eigenvectors because "
-                        "sparse modules do not provide ``eigvals`` method.")
+            log.warning(
+                "Calculating sparse matrix eigenvectors because "
+                "sparse modules do not provide ``eigvals`` method."
+            )
             return self.calculate_eigenvectors(matrix, k=k)[0]
         return np.linalg.eigvalsh(matrix)
 
     def calculate_eigenvectors(self, matrix, k=6):
         if self.issparse(matrix):
             if k < matrix.shape[0]:
                 from scipy.sparse.linalg import eigsh
-                return eigsh(matrix, k=k, which='SA')
+
+                return eigsh(matrix, k=k, which="SA")
             else:  # pragma: no cover
                 matrix = self.to_numpy(matrix)
         return np.linalg.eigh(matrix)
 
     def calculate_matrix_exp(self, a, matrix, eigenvectors=None, eigenvalues=None):
         if eigenvectors is None or self.issparse(matrix):
             if self.issparse(matrix):
@@ -580,59 +640,62 @@
                 from scipy.linalg import expm
             return expm(-1j * a * matrix)
         else:
             expd = self.np.diag(self.np.exp(-1j * a * eigenvalues))
             ud = self.np.transpose(self.np.conj(eigenvectors))
             return self.np.matmul(eigenvectors, self.np.matmul(expd, ud))
 
-    def calculate_expectation_state(self, matrix, state, normalize):
+    def calculate_expectation_state(self, hamiltonian, state, normalize):
         statec = self.np.conj(state)
-        hstate = matrix @ state
+        hstate = hamiltonian @ state
         ev = self.np.real(self.np.sum(statec * hstate))
         if normalize:
             norm = self.np.sum(self.np.square(self.np.abs(state)))
             ev = ev / norm
         return ev
 
-    def calculate_expectation_density_matrix(self, matrix, state, normalize):
-        ev = self.np.real(self.np.trace(matrix @ state))
+    def calculate_expectation_density_matrix(self, hamiltonian, state, normalize):
+        ev = self.np.real(self.np.trace(hamiltonian @ state))
         if normalize:
             norm = self.np.real(self.np.trace(state))
             ev = ev / norm
         return ev
 
     def calculate_hamiltonian_matrix_product(self, matrix1, matrix2):
         return self.np.dot(matrix1, matrix2)
 
     def calculate_hamiltonian_state_product(self, matrix, state):
         rank = len(tuple(state.shape))
         state = self.cast(state)
-        if rank == 1: # vector
+        if rank == 1:  # vector
             return matrix.dot(state[:, np.newaxis])[:, 0]
-        elif rank == 2: # matrix
+        elif rank == 2:  # matrix
             return matrix.dot(state)
         else:
-            raise_error(ValueError, "Cannot multiply Hamiltonian with "
-                                    "rank-{} tensor.".format(rank))
+            raise_error(
+                ValueError,
+                "Cannot multiply Hamiltonian with " "rank-{} tensor.".format(rank),
+            )
 
     def assert_allclose(self, value, target, rtol=1e-7, atol=0.0):
         value = self.to_numpy(value)
         target = self.to_numpy(target)
         np.testing.assert_allclose(value, target, rtol=rtol, atol=atol)
 
     def test_regressions(self, name):
         if name == "test_measurementresult_apply_bitflips":
             return [
                 [0, 0, 0, 0, 2, 3, 0, 0, 0, 0],
                 [0, 0, 0, 0, 2, 3, 0, 0, 0, 0],
                 [0, 0, 0, 0, 0, 1, 0, 0, 0, 0],
-                [0, 0, 0, 0, 2, 0, 0, 0, 0, 0]
+                [0, 0, 0, 0, 2, 0, 0, 0, 0, 0],
             ]
         elif name == "test_probabilistic_measurement":
             return {0: 249, 1: 231, 2: 253, 3: 267}
         elif name == "test_unbalanced_probabilistic_measurement":
             return {0: 171, 1: 148, 2: 161, 3: 520}
         elif name == "test_post_measurement_bitflips_on_circuit":
             return [
-                {5: 30}, {5: 18, 4: 5, 7: 4, 1: 2, 6: 1},
-                {4: 8, 2: 6, 5: 5, 1: 3, 3: 3, 6: 2, 7: 2, 0: 1}
+                {5: 30},
+                {5: 18, 4: 5, 7: 4, 1: 2, 6: 1},
+                {4: 8, 2: 6, 5: 5, 1: 3, 3: 3, 6: 2, 7: 2, 0: 1},
             ]
```

### Comparing `qibo-0.1.8rc0/src/qibo/backends/tensorflow.py` & `qibo-0.1.9/src/qibo/backends/tensorflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,189 +1,219 @@
-import os
 import collections
+import os
+
 import numpy as np
+
+from qibo import __version__
+from qibo.backends.npmatrices import NumpyMatrices
 from qibo.backends.numpy import NumpyBackend
-from qibo.backends.matrices import Matrices
-from qibo.config import log, raise_error, TF_LOG_LEVEL
+from qibo.config import TF_LOG_LEVEL, log, raise_error
 
 
-class TensorflowMatrices(Matrices):
+class TensorflowMatrices(NumpyMatrices):
     # Redefine parametrized gate matrices for backpropagation to work
 
     def __init__(self, dtype):
         super().__init__(dtype)
         import tensorflow as tf
         import tensorflow.experimental.numpy as tnp  # pylint: disable=E0401
+
         self.tf = tf
         self.np = tnp
 
     def RX(self, theta):
         cos = self.np.cos(theta / 2.0) + 0j
         isin = -1j * self.np.sin(theta / 2.0)
-        return self.tf.cast([
-            [cos, isin],
-            [isin, cos]
-        ], dtype=self.dtype)
+        return self.tf.cast([[cos, isin], [isin, cos]], dtype=self.dtype)
 
     def RY(self, theta):
         cos = self.np.cos(theta / 2.0) + 0j
         sin = self.np.sin(theta / 2.0) + 0j
-        return self.tf.cast([
-            [cos, -sin],
-            [sin, cos]
-        ], dtype=self.dtype)
+        return self.tf.cast([[cos, -sin], [sin, cos]], dtype=self.dtype)
 
     def RZ(self, theta):
         phase = self.np.exp(0.5j * theta)
-        return self.tf.cast([
-            [self.np.conj(phase), 0],
-            [0, phase]
-        ], dtype=self.dtype)
+        return self.tf.cast([[self.np.conj(phase), 0], [0, phase]], dtype=self.dtype)
 
     def U1(self, theta):
         phase = self.np.exp(1j * theta)
-        return self.tf.cast([
-            [1, 0],
-            [0, phase]
-        ], dtype=self.dtype)
+        return self.tf.cast([[1, 0], [0, phase]], dtype=self.dtype)
 
     def U2(self, phi, lam):
         eplus = self.np.exp(1j * (phi + lam) / 2.0)
         eminus = self.np.exp(1j * (phi - lam) / 2.0)
-        return self.tf.cast([
-            [self.np.conj(eplus), - self.np.conj(eminus)],
-            [eminus, eplus]
-        ], dtype=self.dtype) / self.np.sqrt(2)
+        return self.tf.cast(
+            [[self.np.conj(eplus), -self.np.conj(eminus)], [eminus, eplus]],
+            dtype=self.dtype,
+        ) / self.np.sqrt(2)
 
     def U3(self, theta, phi, lam):
         cost = self.np.cos(theta / 2)
         sint = self.np.sin(theta / 2)
         eplus = self.np.exp(1j * (phi + lam) / 2.0)
         eminus = self.np.exp(1j * (phi - lam) / 2.0)
-        return self.tf.cast([
-            [self.np.conj(eplus) * cost, - self.np.conj(eminus) * sint],
-            [eminus * sint, eplus * cost]
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [self.np.conj(eplus) * cost, -self.np.conj(eminus) * sint],
+                [eminus * sint, eplus * cost],
+            ],
+            dtype=self.dtype,
+        )
 
     def CRX(self, theta):
         r = self.RX(theta)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def CRY(self, theta):
         r = self.RY(theta)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def CRZ(self, theta):
         r = self.RZ(theta)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def CU1(self, theta):
         r = self.U1(theta)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def CU2(self, phi, lam):
         r = self.U2(phi, lam)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def CU3(self, theta, phi, lam):
         r = self.U3(theta, phi, lam)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, 1, 0, 0],
-            [0, 0, r[0, 0], r[0, 1]],
-            [0, 0, r[1, 0], r[1, 1]],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, 1, 0, 0],
+                [0, 0, r[0, 0], r[0, 1]],
+                [0, 0, r[1, 0], r[1, 1]],
+            ],
+            dtype=self.dtype,
+        )
 
     def fSim(self, theta, phi):
         cost = self.np.cos(theta) + 0j
         isint = -1j * self.np.sin(theta)
         phase = self.np.exp(-1j * phi)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, cost, isint, 0],
-            [0, isint, cost, 0],
-            [0, 0, 0, phase],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, cost, isint, 0],
+                [0, isint, cost, 0],
+                [0, 0, 0, phase],
+            ],
+            dtype=self.dtype,
+        )
 
     def GeneralizedfSim(self, u, phi):
         phase = self.np.exp(-1j * phi)
-        return self.tf.cast([
-            [1, 0, 0, 0],
-            [0, u[0, 0], u[0, 1], 0],
-            [0, u[1, 0], u[1, 1], 0],
-            [0, 0, 0, phase],
-        ], dtype=self.dtype)
+        return self.tf.cast(
+            [
+                [1, 0, 0, 0],
+                [0, u[0, 0], u[0, 1], 0],
+                [0, u[1, 0], u[1, 1], 0],
+                [0, 0, 0, phase],
+            ],
+            dtype=self.dtype,
+        )
 
     def Unitary(self, u):
         return self.tf.cast(u, dtype=self.dtype)
 
 
 class TensorflowBackend(NumpyBackend):
-
     def __init__(self):
         super().__init__()
         self.name = "tensorflow"
         os.environ["TF_CPP_MIN_LOG_LEVEL"] = str(TF_LOG_LEVEL)
         import tensorflow as tf
         import tensorflow.experimental.numpy as tnp  # pylint: disable=E0401
+
         tnp.experimental_enable_numpy_behavior()
         self.tf = tf
         self.np = tnp
+
+        self.versions = {
+            "qibo": __version__,
+            "numpy": np.__version__,
+            "tensorflow": tf.__version__,
+        }
+
         self.matrices = TensorflowMatrices(self.dtype)
 
         from tensorflow.python.framework import errors_impl  # pylint: disable=E0611
+
         self.oom_error = errors_impl.ResourceExhaustedError
 
         cpu_devices = tf.config.list_logical_devices("CPU")
         gpu_devices = tf.config.list_logical_devices("GPU")
-        if gpu_devices: # pragma: no cover
+        if gpu_devices:  # pragma: no cover
             # CI does not use GPUs
             self.device = gpu_devices[0].name
         elif cpu_devices:
             self.device = cpu_devices[0].name
 
         import psutil
+
         self.nthreads = psutil.cpu_count(logical=True)
 
         self.tensor_types = (np.ndarray, tf.Tensor, tf.Variable)
 
     def set_device(self, device):  # pragma: no cover
         self.device = device
 
     def set_threads(self, nthreads):
-        log.warning("`set_threads` is not supported by the tensorflow "
-                    "backend. Please use tensorflow's thread setters: "
-                    "`tf.config.threading.set_inter_op_parallelism_threads` "
-                    "or `tf.config.threading.set_intra_op_parallelism_threads` "
-                    "to switch the number of threads.")
+        log.warning(
+            "`set_threads` is not supported by the tensorflow "
+            "backend. Please use tensorflow's thread setters: "
+            "`tf.config.threading.set_inter_op_parallelism_threads` "
+            "or `tf.config.threading.set_intra_op_parallelism_threads` "
+            "to switch the number of threads."
+        )
 
     def cast(self, x, dtype=None, copy=False):
         if dtype is None:
             dtype = self.dtype
         x = self.tf.cast(x, dtype=dtype)
         if copy:
             return self.tf.identity(x)
@@ -196,40 +226,41 @@
         return np.array(x)
 
     def compile(self, func):
         return self.tf.function(func)
 
     def zero_state(self, nqubits):
         idx = self.tf.constant([[0]], dtype="int32")
-        state = self.tf.zeros((2 ** nqubits,), dtype=self.dtype)
+        state = self.tf.zeros((2**nqubits,), dtype=self.dtype)
         update = self.tf.constant([1], dtype=self.dtype)
         state = self.tf.tensor_scatter_nd_update(state, idx, update)
         return state
 
     def zero_density_matrix(self, nqubits):
         idx = self.tf.constant([[0, 0]], dtype="int32")
-        state = self.tf.zeros(2 * (2 ** nqubits,), dtype=self.dtype)
+        state = self.tf.zeros(2 * (2**nqubits,), dtype=self.dtype)
         update = self.tf.constant([1], dtype=self.dtype)
         state = self.tf.tensor_scatter_nd_update(state, idx, update)
         return state
 
-
     def asmatrix(self, gate):
         npmatrix = super().asmatrix(gate)
         return self.tf.cast(npmatrix, dtype=self.dtype)
 
     def asmatrix_parametrized(self, gate):
         npmatrix = super().asmatrix_parametrized(gate)
         return self.tf.cast(npmatrix, dtype=self.dtype)
 
     def asmatrix_fused(self, gate):
         npmatrix = super().asmatrix_fused(gate)
         return self.tf.cast(npmatrix, dtype=self.dtype)
 
-    def execute_circuit(self, circuit, initial_state=None, nshots=None, return_array=False):
+    def execute_circuit(
+        self, circuit, initial_state=None, nshots=None, return_array=False
+    ):
         with self.tf.device(self.device):
             return super().execute_circuit(circuit, initial_state, nshots, return_array)
 
     def execute_circuit_repeated(self, circuit, initial_state=None, nshots=None):
         with self.tf.device(self.device):
             return super().execute_circuit_repeated(circuit, initial_state, nshots)
 
@@ -252,20 +283,23 @@
         res, counts = self.np.array(res), self.np.array(counts)
         return collections.Counter({int(k): int(v) for k, v in zip(res, counts)})
 
     def update_frequencies(self, frequencies, probabilities, nsamples):
         # redefining this because ``tnp.unique`` and tensor update is not available
         samples = self.sample_shots(probabilities, nsamples)
         res, _, counts = self.tf.unique_with_counts(samples, out_idx="int64")
-        frequencies = self.tf.tensor_scatter_nd_add(frequencies, res[:, self.tf.newaxis], counts)
+        frequencies = self.tf.tensor_scatter_nd_add(
+            frequencies, res[:, self.tf.newaxis], counts
+        )
         return frequencies
 
     def entanglement_entropy(self, rho):
         # redefining this because ``tnp.linalg`` is not available
         from qibo.config import EIGVAL_CUTOFF
+
         # Diagonalize
         eigvals = self.np.real(self.tf.linalg.eigvalsh(rho))
         # Treating zero and negative eigenvalues
         masked_eigvals = eigvals[eigvals > EIGVAL_CUTOFF]
         spectrum = -1 * self.np.log(masked_eigvals)
         entropy = self.np.sum(masked_eigvals * spectrum) / self.np.log(2.0)
         return entropy, spectrum
@@ -280,43 +314,49 @@
         if eigenvectors is None or self.issparse(matrix):
             return self.tf.linalg.expm(-1j * a * matrix)
         else:
             return super().calculate_matrix_exp(a, matrix, eigenvectors, eigenvalues)
 
     def calculate_hamiltonian_matrix_product(self, matrix1, matrix2):
         if self.issparse(matrix1) or self.issparse(matrix2):
-            raise_error(NotImplementedError, "Multiplication of sparse matrices is not supported with Tensorflow.")
+            raise_error(
+                NotImplementedError,
+                "Multiplication of sparse matrices is not supported with Tensorflow.",
+            )
         return super().calculate_hamiltonian_matrix_product(matrix1, matrix2)
 
     def calculate_hamiltonian_state_product(self, matrix, state):
         rank = len(tuple(state.shape))
-        if rank == 1: # vector
+        if rank == 1:  # vector
             return self.np.matmul(matrix, state[:, self.np.newaxis])[:, 0]
-        elif rank == 2: # matrix
+        elif rank == 2:  # matrix
             return self.np.matmul(matrix, state)
         else:
-            raise_error(ValueError, "Cannot multiply Hamiltonian with "
-                                    "rank-{} tensor.".format(rank))
+            raise_error(
+                ValueError,
+                "Cannot multiply Hamiltonian with " "rank-{} tensor.".format(rank),
+            )
 
     def test_regressions(self, name):
         if name == "test_measurementresult_apply_bitflips":
             return [
                 [4, 0, 0, 1, 0, 2, 2, 4, 4, 0],
                 [4, 0, 0, 1, 0, 2, 2, 4, 4, 0],
                 [4, 0, 0, 1, 0, 0, 0, 4, 4, 0],
-                [4, 0, 0, 0, 0, 0, 0, 4, 4, 0]
+                [4, 0, 0, 0, 0, 0, 0, 4, 4, 0],
             ]
         elif name == "test_probabilistic_measurement":
             if "GPU" in self.device:  # pragma: no cover
                 return {0: 273, 1: 233, 2: 242, 3: 252}
             else:
                 return {0: 271, 1: 239, 2: 242, 3: 248}
         elif name == "test_unbalanced_probabilistic_measurement":
             if "GPU" in self.device:  # pragma: no cover
                 return {0: 196, 1: 153, 2: 156, 3: 495}
             else:
                 return {0: 168, 1: 188, 2: 154, 3: 490}
         elif name == "test_post_measurement_bitflips_on_circuit":
             return [
-                {5: 30}, {5: 16, 7: 10, 6: 2, 3: 1, 4: 1},
-                {3: 6, 5: 6, 7: 5, 2: 4, 4: 3, 0: 2, 1: 2, 6: 2}
+                {5: 30},
+                {5: 16, 7: 10, 6: 2, 3: 1, 4: 1},
+                {3: 6, 5: 6, 7: 5, 2: 4, 4: 3, 0: 2, 1: 2, 6: 2},
             ]
```

### Comparing `qibo-0.1.8rc0/src/qibo/callbacks.py` & `qibo-0.1.9/src/qibo/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from qibo.config import raise_error
 from typing import List, Optional, Set, Union
 
+from qibo.config import raise_error
+
 
 class Callback:
     """Base callback class.
 
     Results of a callback can be accessed by indexing the corresponding object.
     """
 
     def __init__(self):
         self._results = []
         self._nqubits = None
 
     @property
-    def nqubits(self): # pragma: no cover
+    def nqubits(self):  # pragma: no cover
         """Total number of qubits in the circuit that the callback was added in."""
         # abstract method
         return self._nqubits
 
     @nqubits.setter
-    def nqubits(self, n: int): # pragma: no cover
+    def nqubits(self, n: int):  # pragma: no cover
         # abstract method
         self._nqubits = n
 
     @property
     def results(self):
         return self._results
 
@@ -32,26 +33,29 @@
 
     def extend(self, x):
         self._results.extend(x)
 
     def __getitem__(self, k):
         if not isinstance(k, (int, slice, list, tuple)):
             raise_error(IndexError, "Unrecognized type for index {}.".format(k))
-        
+
         if isinstance(k, int) and k >= len(self._results):
-            raise_error(IndexError, "Attempting to access callbacks {} run but "
-                                    "the callback has been used in {} executions."
-                                    "".format(k, len(self._results)))
-        
+            raise_error(
+                IndexError,
+                "Attempting to access callbacks {} run but "
+                "the callback has been used in {} executions."
+                "".format(k, len(self._results)),
+            )
+
         return self._results[k]
 
-    def apply(self, backend, state): # pragma: no cover
+    def apply(self, backend, state):  # pragma: no cover
         pass
 
-    def apply_density_matrix(self, backend, state): # pragma: no cover
+    def apply_density_matrix(self, backend, state):  # pragma: no cover
         pass
 
 
 class EntanglementEntropy(Callback):
     """Von Neumann entanglement entropy callback.
 
     .. math::
@@ -87,32 +91,38 @@
             # Print the entanglement spectrum.
         .. testoutput::
             :hide:
 
             ...
     """
 
-    def __init__(self, partition: Optional[List[int]] = None,
-                 compute_spectrum: bool = False):
+    def __init__(
+        self, partition: Optional[List[int]] = None, compute_spectrum: bool = False
+    ):
         super().__init__()
         self.partition = partition
         self.compute_spectrum = compute_spectrum
         self.spectrum = list()
 
     @Callback.nqubits.setter
     def nqubits(self, n: int):
         from qibo import gates
+
         if self._nqubits is not None and self._nqubits != n:
-            raise_error(RuntimeError,
-                        f"Changing EntanglementEntropy nqubits from {self._nqubits} to {n}.")
+            raise_error(
+                RuntimeError,
+                f"Changing EntanglementEntropy nqubits from {self._nqubits} to {n}.",
+            )
         self._nqubits = n
         if self.partition is None:
             self.partition = list(range(n // 2 + n % 2))
         if len(self.partition) <= self.nqubits // 2:
-            self.partition = [i for i in range(self.nqubits) if i not in set(self.partition)]
+            self.partition = [
+                i for i in range(self.nqubits) if i not in set(self.partition)
+            ]
 
     def apply(self, backend, state):
         rho = backend.partial_trace(state, self.partition, self.nqubits)
         entropy, spectrum = backend.entanglement_entropy(rho)
         self.append(entropy)
         if self.compute_spectrum:
             self.spectrum.append(spectrum)
@@ -162,15 +172,15 @@
     .. math::
         \\mathrm{Norm} = \\left \\langle \\Psi | \\Psi \\right \\rangle
         = \\mathrm{Tr} (\\rho )
     """
 
     def apply(self, backend, state):
         return backend.calculate_norm(state)
-    
+
     def apply_density_matrix(self, backend, state):
         return backend.calculate_norm_density_matrix(state)
 
 
 class Overlap(Callback):
     """State overlap callback.
 
@@ -180,22 +190,22 @@
         \\mathrm{Overlap} = |\\left \\langle \\Phi | \\Psi \\right \\rangle |
 
     Args:
         state (np.ndarray): Target state to calculate overlap with.
         normalize (bool): If ``True`` the states are normalized for the overlap
             calculation.
     """
-    
+
     def __init__(self, state):
         super().__init__()
         self.state = state
-    
+
     def apply(self, backend, state):
         return backend.calculate_overlap(self.state, state)
-    
+
     def apply_density_matrix(self, backend, state):
         return backend.calculate_overlap_density_matrix(self.state, state)
 
 
 class Energy(Callback):
     """Energy expectation value callback.
 
@@ -273,28 +283,35 @@
 
             ...
     """
 
     def __init__(self, mode: Union[str, int] = "gap", check_degenerate: bool = True):
         super().__init__()
         if not isinstance(mode, (int, str)):
-            raise_error(TypeError, "Gap callback mode should be integer or "
-                                   "string but is {}.".format(type(mode)))
+            raise_error(
+                TypeError,
+                "Gap callback mode should be integer or "
+                "string but is {}.".format(type(mode)),
+            )
         elif isinstance(mode, str) and mode != "gap":
-            raise_error(ValueError, "Unsupported mode {} for gap callback."
-                                    "".format(mode))
+            raise_error(
+                ValueError, "Unsupported mode {} for gap callback." "".format(mode)
+            )
         self.mode = mode
         self.check_degenerate = check_degenerate
         self.evolution = None
 
     def apply(self, backend, state):
-        from qibo.config import log, EIGVAL_CUTOFF
+        from qibo.config import EIGVAL_CUTOFF, log
+
         if self.evolution is None:
-            raise_error(RuntimeError, "Gap callback can only be used in "
-                                      "adiabatic evolution models.")
+            raise_error(
+                RuntimeError,
+                "Gap callback can only be used in " "adiabatic evolution models.",
+            )
         hamiltonian = self.evolution.solver.current_hamiltonian  # pylint: disable=E1101
         assert type(hamiltonian.backend) == type(backend)
         # Call the eigenvectors so that they are cached for the ``exp`` call
         hamiltonian.eigenvectors()
         eigvals = hamiltonian.eigenvalues()
         if isinstance(self.mode, int):
             return backend.np.real(eigvals[self.mode])
@@ -305,14 +322,18 @@
         if not self.check_degenerate:
             return gap
 
         while backend.np.less(gap, EIGVAL_CUTOFF):
             gap = backend.np.real(eigvals[excited] - eigvals[0])
             excited += 1
         if excited > 1:
-            log.warning("The Hamiltonian is degenerate. Using eigenvalue {} "
-                        "to calculate gap.".format(excited))
+            log.warning(
+                "The Hamiltonian is degenerate. Using eigenvalue {} "
+                "to calculate gap.".format(excited)
+            )
         return gap
 
     def apply_density_matrix(self, backend, state):
-        raise_error(NotImplementedError, "Gap callback is not implemented for "
-                                         "density matrices.")
+        raise_error(
+            NotImplementedError,
+            "Gap callback is not implemented for " "density matrices.",
+        )
```

### Comparing `qibo-0.1.8rc0/src/qibo/config.py` & `qibo-0.1.9/src/qibo/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
 Define the default circuit, constants and types.
 """
-import os
 import logging
+import os
 
 # Logging level from 0 (all) to 4 (errors) (see https://docs.python.org/3/library/logging.html#logging-levels)
 QIBO_LOG_LEVEL = 1
-if "QIBO_LOG_LEVEL" in os.environ: # pragma: no cover
+if "QIBO_LOG_LEVEL" in os.environ:  # pragma: no cover
     QIBO_LOG_LEVEL = 10 * int(os.environ.get("QIBO_LOG_LEVEL"))
 
 # Logging level from 0 (all) to 3 (errors) for TensorFlow
 TF_LOG_LEVEL = 3
-if "TF_LOG_LEVEL" in os.environ: # pragma: no cover
+if "TF_LOG_LEVEL" in os.environ:  # pragma: no cover
     TF_LOG_LEVEL = int(os.environ.get("TF_LOG_LEVEL"))
 
 # characters used in einsum strings
 EINSUM_CHARS = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
 
 # Entanglement entropy eigenvalue cut-off
 # Eigenvalues smaller than this cut-off are ignored in entropy calculation
 EIGVAL_CUTOFF = 1e-14
 
 # Tolerance for the probability sum check in the unitary channel
 PRECISION_TOL = 1e-8
 
 # Batch size for sampling shots in measurement frequencies calculation
-SHOT_BATCH_SIZE = 2 ** 18
+SHOT_BATCH_SIZE = 2**18
 
 # Threshold size for sampling shots in measurements frequencies with custom operator
 SHOT_METROPOLIS_THRESHOLD = 100000
 
 
 def raise_error(exception, message=None, args=None):
     """Raise exception with logging error.
@@ -45,47 +45,51 @@
         raise exception(message)
 
 
 def get_batch_size():
     """Returns batch size used for sampling measurement shots."""
     return SHOT_BATCH_SIZE
 
+
 def set_batch_size(batch_size):
     """Sets batch size used for sampling measurement shots."""
     if not isinstance(batch_size, int):
         raise_error(TypeError, "Shot batch size must be integer.")
     elif batch_size < 1:
         raise_error(ValueError, "Shot batch size must be a positive integer.")
-    elif batch_size > 2 ** 31:
-         raise_error(ValueError, "Shot batch size cannot be greater than 2^31.")
+    elif batch_size > 2**31:
+        raise_error(ValueError, "Shot batch size cannot be greater than 2^31.")
     global SHOT_BATCH_SIZE
     SHOT_BATCH_SIZE = batch_size
 
 
 def get_metropolis_threshold():
     """Returns threshold for using Metropolis algorithm for sampling measurement shots."""
     return SHOT_METROPOLIS_THRESHOLD
 
+
 def set_metropolis_threshold(threshold):
     """Sets threshold for using Metropolis algorithm for sampling measurement shots."""
     if not isinstance(threshold, int):
         raise_error(TypeError, "Shot threshold must be integer.")
     elif threshold < 1:
         raise_error(ValueError, "Shot threshold be a positive integer.")
     global SHOT_METROPOLIS_THRESHOLD
     SHOT_METROPOLIS_THRESHOLD = threshold
 
 
 # Configuration for logging mechanism
 class CustomHandler(logging.StreamHandler):
     """Custom handler for logging algorithm."""
+
     def format(self, record):
         """Format the record with specific format."""
         from qibo import __version__
-        fmt = f'[Qibo {__version__}|%(levelname)s|%(asctime)s]: %(message)s'
-        return logging.Formatter(fmt, datefmt='%Y-%m-%d %H:%M:%S').format(record)
+
+        fmt = f"[Qibo {__version__}|%(levelname)s|%(asctime)s]: %(message)s"
+        return logging.Formatter(fmt, datefmt="%Y-%m-%d %H:%M:%S").format(record)
 
 
 # allocate logger object
 log = logging.getLogger(__name__)
 log.setLevel(QIBO_LOG_LEVEL)
 log.addHandler(CustomHandler())
```

### Comparing `qibo-0.1.8rc0/src/qibo/gates/abstract.py` & `qibo-0.1.9/src/qibo/gates/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-# -*- coding: utf-8 -*-
 import collections
-import sympy
 from abc import ABC, abstractmethod
-from qibo.config import raise_error
 from collections.abc import Iterable
 from typing import List, Sequence, Tuple
 
+import sympy
+
+from qibo.config import raise_error
+
 
 class Gate:
     """The base class for gate implementation.
 
     All base gates should inherit this class.
     """
+
     def __init__(self):
         """
         Attributes:
             name (str): Name of the gate.
             is_controlled_by (bool): ``True`` if the gate was created using the
                 :meth:`qibo.gates.abstract.Gate.controlled_by` method,
                 otherwise ``False``.
             init_args (list): Arguments used to initialize the gate.
             init_kwargs (dict): Arguments used to initialize the gate.
             target_qubits (tuple): Tuple with ids of target qubits.
             control_qubits (tuple): Tuple with ids of control qubits sorted in
                 increasing order.
         """
         from qibo import config
+
         self.name = None
         self.is_controlled_by = False
         # args for creating gate
         self.init_args = []
         self.init_kwargs = {}
 
         self._target_qubits = tuple()
@@ -59,39 +62,46 @@
         return self.control_qubits + self.target_qubits
 
     def _set_target_qubits(self, qubits: Sequence[int]):
         """Helper method for setting target qubits."""
         self._target_qubits = tuple(qubits)
         if len(self._target_qubits) != len(set(qubits)):
             repeated = self._find_repeated(qubits)
-            raise_error(ValueError, "Target qubit {} was given twice for gate {}."
-                                    "".format(repeated, self.name))
+            raise_error(
+                ValueError,
+                "Target qubit {} was given twice for gate {}."
+                "".format(repeated, self.name),
+            )
 
     def _set_control_qubits(self, qubits: Sequence[int]):
         """Helper method for setting control qubits."""
         self._control_qubits = set(qubits)
         if len(self._control_qubits) != len(qubits):
             repeated = self._find_repeated(qubits)
-            raise_error(ValueError, "Control qubit {} was given twice for gate {}."
-                                    "".format(repeated, self.name))
+            raise_error(
+                ValueError,
+                "Control qubit {} was given twice for gate {}."
+                "".format(repeated, self.name),
+            )
 
     @target_qubits.setter
     def target_qubits(self, qubits: Sequence[int]):
         """Sets target qubits tuple."""
         self._set_target_qubits(qubits)
         self._check_control_target_overlap()
 
     @control_qubits.setter
     def control_qubits(self, qubits: Sequence[int]):
         """Sets control qubits set."""
         self._set_control_qubits(qubits)
         self._check_control_target_overlap()
 
-    def _set_targets_and_controls(self, target_qubits: Sequence[int],
-                                 control_qubits: Sequence[int]):
+    def _set_targets_and_controls(
+        self, target_qubits: Sequence[int], control_qubits: Sequence[int]
+    ):
         """Sets target and control qubits simultaneously.
 
         This is used for the reduced qubit updates in the distributed circuits
         because using the individual setters may raise errors due to temporary
         overlap of control and target qubits.
         """
         self._set_target_qubits(target_qubits)
@@ -107,16 +117,19 @@
                 return qubit
             temp_set.add(qubit)
 
     def _check_control_target_overlap(self):
         """Checks that there are no qubits that are both target and controls."""
         common = set(self._target_qubits) & self._control_qubits
         if common:
-            raise_error(ValueError, "{} qubits are both targets and controls for "
-                                    "gate {}.".format(common, self.name))
+            raise_error(
+                ValueError,
+                "{} qubits are both targets and controls for "
+                "gate {}.".format(common, self.name),
+            )
 
     @property
     def parameters(self):
         """Returns a tuple containing the current value of gate's parameters."""
         return self._parameters
 
     def commutes(self, gate: "Gate") -> bool:
@@ -190,22 +203,26 @@
             the original gate.
         """
         new_gate = self._dagger()
         new_gate.is_controlled_by = self.is_controlled_by
         new_gate.control_qubits = self.control_qubits
         return new_gate
 
-    def check_controls(func): # pylint: disable=E0213
+    def check_controls(func):  # pylint: disable=E0213
         def wrapper(self, *args):
             if self.control_qubits:
-                raise_error(RuntimeError, "Cannot use `controlled_by` method "
-                                          "on gate {} because it is already "
-                                          "controlled by {}."
-                                          "".format(self, self.control_qubits))
-            return func(self, *args) # pylint: disable=E1102
+                raise_error(
+                    RuntimeError,
+                    "Cannot use `controlled_by` method "
+                    "on gate {} because it is already "
+                    "controlled by {}."
+                    "".format(self, self.control_qubits),
+                )
+            return func(self, *args)  # pylint: disable=E1102
+
         return wrapper
 
     @check_controls
     def controlled_by(self, *qubits: int) -> "Gate":
         """Controls the gate on (arbitrarily many) qubits.
 
         Args:
@@ -239,14 +256,15 @@
 
     def asmatrix(self, backend):
         return backend.asmatrix(self)
 
     @property
     def matrix(self):
         from qibo.backends import GlobalBackend
+
         backend = GlobalBackend()
         return self.asmatrix(backend)
 
     def apply(self, backend, state, nqubits):
         return backend.apply_gate(self, state, nqubits)
 
     def apply_density_matrix(self, backend, state, nqubits):
@@ -256,20 +274,20 @@
 class SpecialGate(Gate):
     """Abstract class for special gates."""
 
     def commutes(self, gate):
         return False
 
     def on_qubits(self, qubit_map):
-        raise_error(NotImplementedError,
-                    "Cannot use special gates on subroutines.")
+        raise_error(NotImplementedError, "Cannot use special gates on subroutines.")
 
     def asmatrix(self, backend):  # pragma: no cover
-        raise_error(NotImplementedError,
-                    "Special gates do not have matrix representation.")
+        raise_error(
+            NotImplementedError, "Special gates do not have matrix representation."
+        )
 
 
 class ParametrizedGate(Gate):
     """Base class for parametrized gates.
 
     Implements the basic functionality of parameter setters and getters.
     """
@@ -289,39 +307,47 @@
                 x = [x]
             else:
                 # Captures the ``Unitary`` gate case where the given parameter
                 # can be an array
                 try:
                     if len(x) != 1:  # pragma: no cover
                         x = [x]
-                except TypeError: # tf.Variable case
+                except TypeError:  # tf.Variable case
                     s = tuple(x.shape)
                     if not s or s[0] != 1:
                         x = [x]
         else:
             nparams = len(self.parameter_names)
 
         if not self._parameters:
             params = nparams * [None]
         else:
             params = list(self._parameters)
         if len(x) != nparams:
-            raise_error(ValueError, "Parametrized gate has {} parameters "
-                                    "but {} update values were given."
-                                    "".format(nparams, len(x)))
+            raise_error(
+                ValueError,
+                "Parametrized gate has {} parameters "
+                "but {} update values were given."
+                "".format(nparams, len(x)),
+            )
         for i, v in enumerate(x):
             if isinstance(v, sympy.Expr):
                 self.symbolic_parameters[i] = v
             params[i] = v
         self._parameters = tuple(params)
 
         # set parameters in device gates
         for gate in self.device_gates:  # pragma: no cover
             gate.parameters = x
 
+    def on_qubits(self, qubit_map):
+        gate = super().on_qubits(qubit_map)
+        gate.parameters = self.parameters
+        return gate
+
     def substitute_symbols(self):
         params = list(self._parameters)
         for i, param in self.symbolic_parameters.items():
             for symbol in param.free_symbols:
                 param = symbol.evaluate(param)
             params[i] = float(param)
         self.parameters = tuple(params)
```

### Comparing `qibo-0.1.8rc0/src/qibo/gates/channels.py` & `qibo-0.1.9/src/qibo/gates/channels.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import abstractmethod
+from itertools import product
+
+from qibo.config import PRECISION_TOL, raise_error
 from qibo.gates.abstract import Gate
-from qibo.gates.gates import X, Y, Z, Unitary
+from qibo.gates.gates import I, Unitary, X, Y, Z
 from qibo.gates.measurements import M
-from qibo.config import raise_error, PRECISION_TOL
 
 
 class Channel(Gate):
     """Abstract class for channels."""
 
     def __init__(self):
         super().__init__()
@@ -15,19 +17,23 @@
 
     def controlled_by(self, *q):
         """"""
         raise_error(ValueError, "Noise channel cannot be controlled on qubits.")
 
     def on_qubits(self, qubit_map):  # pragma: no cover
         # future TODO
-        raise_error(NotImplementedError, "`on_qubits` method is not available "
-                                         "for the `Channel` gate.")
+        raise_error(
+            NotImplementedError,
+            "`on_qubits` method is not available " "for the `Channel` gate.",
+        )
 
     def apply(self, backend, state, nqubits):  # pragma: no cover
-        raise_error(NotImplementedError, f"{self.name} cannot be applied to state vector.")
+        raise_error(
+            NotImplementedError, f"{self.name} cannot be applied to state vector."
+        )
 
     def apply_density_matrix(self, backend, state, nqubits):
         return backend.apply_channel_density_matrix(self, state, nqubits)
 
 
 class KrausChannel(Channel):
     """General channel defined by arbitrary Kraus operators.
@@ -68,25 +74,29 @@
     """
 
     def __init__(self, ops):
         super().__init__()
         self.name = "KrausChannel"
         if isinstance(ops[0], Gate):
             self.gates = tuple(ops)
-            self.target_qubits = tuple(sorted(set(
-                q for gate in ops for q in gate.target_qubits)))
+            self.target_qubits = tuple(
+                sorted({q for gate in ops for q in gate.target_qubits})
+            )
         else:
             gates, qubitset = [], set()
             for qubits, matrix in ops:
                 rank = 2 ** len(qubits)
                 shape = tuple(matrix.shape)
                 if shape != (rank, rank):
-                    raise_error(ValueError, "Invalid Krauss operator shape {} for "
-                                            "acting on {} qubits."
-                                            "".format(shape, len(qubits)))
+                    raise_error(
+                        ValueError,
+                        "Invalid Krauss operator shape {} for "
+                        "acting on {} qubits."
+                        "".format(shape, len(qubits)),
+                    )
                 qubitset.update(qubits)
                 gates.append(Unitary(matrix, *list(qubits)))
             self.gates = tuple(gates)
             self.target_qubits = tuple(sorted(qubitset))
         self.init_args = [self.gates]
         self.coefficients = len(self.gates) * (1,)
         self.coefficient_sum = 1
@@ -114,29 +124,38 @@
             ``qubits`` refers the qubit ids that ``Uk`` acts on and ``Uk`` is
             the corresponding matrix as a ``np.ndarray``/``tf.Tensor``.
             Must have the same length as the given probabilities ``p``.
     """
 
     def __init__(self, probabilities, ops):
         if len(probabilities) != len(ops):
-            raise_error(ValueError, "Probabilities list has length {} while "
-                                    "{} gates were given."
-                                    "".format(len(probabilities), len(ops)))
+            raise_error(
+                ValueError,
+                "Probabilities list has length {} while "
+                "{} gates were given."
+                "".format(len(probabilities), len(ops)),
+            )
         for p in probabilities:
             if p < 0 or p > 1:
-                raise_error(ValueError, "Probabilities should be between 0 "
-                                        "and 1 but {} was given.".format(p))
+                raise_error(
+                    ValueError,
+                    "Probabilities should be between 0 "
+                    "and 1 but {} was given.".format(p),
+                )
         super().__init__(ops)
         self.name = "UnitaryChannel"
         self.coefficients = tuple(probabilities)
         self.coefficient_sum = sum(probabilities)
         if self.coefficient_sum > 1 + PRECISION_TOL or self.coefficient_sum <= 0:
-            raise_error(ValueError, "UnitaryChannel probability sum should be "
-                                    "between 0 and 1 but is {}."
-                                    "".format(self.coefficient_sum))
+            raise_error(
+                ValueError,
+                "UnitaryChannel probability sum should be "
+                "between 0 and 1 but is {}."
+                "".format(self.coefficient_sum),
+            )
 
         self.init_args = [probabilities, self.gates]
 
     def apply(self, backend, state, nqubits):
         return backend.apply_channel(self, state, nqubits)
 
 
@@ -172,22 +191,70 @@
         self.name = "PauliNoiseChannel"
         assert self.target_qubits == (q,)
 
         self.init_args = [q]
         self.init_kwargs = {"px": px, "py": py, "pz": pz}
 
 
+class DepolarizingChannel(UnitaryChannel):
+    """:math:`n`-qubit Depolarizing quantum error channel,
+
+    .. math::
+        \\mathcal{E}(\\rho ) = (1 - \\lambda) \\rho +\\lambda \\text{Tr}[\\rho] \\frac{I}{2^n}
+
+    where :math:`\\lambda` is the depolarizing error parameter and :math:`0 \\le \\lambda \\le 4^n / (4^n - 1)`.
+
+    * If :math:`\\lambda = 1` this is a completely depolarizing channel
+      :math:`E(\\rho) = I / 2^n`
+    * If :math:`\\lambda = 4^n / (4^n - 1)` this is a uniform Pauli
+      error channel: :math:`E(\\rho) = \\sum_j P_j \\rho P_j / (4^n - 1)` for
+      all :math:`P_j != I`.
+
+    Args:
+        q (tuple): Qubit ids that the noise acts on.
+        lam (float): Depolarizing error parameter.
+    """
+
+    def __init__(self, q, lam=0):
+        from qibo.models.circuit import Circuit
+
+        num_qubits = len(q)
+        num_terms = 4**num_qubits
+        max_param = num_terms / (num_terms - 1)
+        if lam < 0 or lam > max_param:
+            raise_error(
+                ValueError,
+                "Depolarizing parameter must be in between 0 and {}.".format(max_param),
+            )
+        prob_iden = 1 - lam / max_param
+        prob_pauli = lam / num_terms
+        probs = (num_terms - 1) * [prob_pauli]
+        gates = []
+        for pauli_list in list(product([I, X, Y, Z], repeat=num_qubits))[1::]:
+            qc = Circuit(num_qubits)
+            for j, pauli in enumerate(pauli_list):
+                qc.add(pauli(j))
+            gates.append(Unitary(qc.unitary(), *q))
+
+        super().__init__(probs, gates)
+        self.name = "DepolarizingChannel"
+        assert self.target_qubits == q
+
+        self.init_args = [q]
+        self.init_kwargs = {"lam": lam}
+
+
 class ResetChannel(Channel):
     """Single-qubit reset channel.
 
     Implements the following transformation:
 
     .. math::
         \\mathcal{E}(\\rho ) = (1 - p_0 - p_1) \\rho
-        +  \mathrm{Tr}\\rho \\otimes (p_0|0\\rangle \\langle 0| + p_1|1\\rangle \langle 1|)
+        +  \\mathrm{Tr}\\rho \\otimes (p_0|0\\rangle \\langle 0| + p_1|1\\rangle \\langle 1|)
 
     Args:
         q (int): Qubit id that the channel acts on.
         p0 (float): Probability to reset to 0.
         p1 (float): Probability to reset to 1.
     """
 
@@ -208,15 +275,15 @@
 
     Implements the following transformation:
 
     If :math:`T_1 \\geq T_2`:
 
     .. math::
         \\mathcal{E} (\\rho ) = (1 - p_z - p_0 - p_1)\\rho + p_zZ\\rho Z
-        +  \mathrm{Tr}\\rho \\otimes (p_0|0\\rangle \\langle 0| + p_1|1\\rangle \langle 1|)
+        +  \\mathrm{Tr}\\rho \\otimes (p_0|0\\rangle \\langle 0| + p_1|1\\rangle \\langle 1|)
 
 
     while if :math:`T_1 < T_2`:
 
     .. math::
         \\mathcal{E}(\\rho ) = \\mathrm{Tr} _\\mathcal{X}\\left [\\Lambda _{\\mathcal{X}\\mathcal{Y}}(\\rho _\\mathcal{X} ^T \\otimes \\mathbb{I}_\\mathcal{Y})\\right ]
 
@@ -252,53 +319,68 @@
         self.name = "ThermalRelaxationChannel"
         self.target_qubits = (q,)
         self.init_args = [q, t1, t2, time]
         self.init_kwargs = {"excited_population": excited_population}
 
         # check given parameters
         if excited_population < 0 or excited_population > 1:
-            raise_error(ValueError, "Invalid excited state population {}."
-                                    "".format(excited_population))
+            raise_error(
+                ValueError,
+                "Invalid excited state population {}." "".format(excited_population),
+            )
         if time < 0:
             raise_error(ValueError, "Invalid gate_time ({} < 0)".format(time))
         if t1 <= 0:
-            raise_error(ValueError, "Invalid T_1 relaxation time parameter: "
-                                    "T_1 <= 0.")
+            raise_error(
+                ValueError, "Invalid T_1 relaxation time parameter: " "T_1 <= 0."
+            )
         if t2 <= 0:
-            raise_error(ValueError, "Invalid T_2 relaxation time parameter: "
-                                    "T_2 <= 0.")
+            raise_error(
+                ValueError, "Invalid T_2 relaxation time parameter: " "T_2 <= 0."
+            )
         if t2 > 2 * t1:
-            raise_error(ValueError, "Invalid T_2 relaxation time parameter: "
-                                    "T_2 greater than 2 * T_1.")
+            raise_error(
+                ValueError,
+                "Invalid T_2 relaxation time parameter: " "T_2 greater than 2 * T_1.",
+            )
 
         # calculate probabilities
         import numpy as np
+
         self.t1, self.t2 = t1, t2
         p_reset = 1 - np.exp(-time / t1)
-        self.coefficients = [p_reset * (1 - excited_population),
-                             p_reset * excited_population]
+        self.coefficients = [
+            p_reset * (1 - excited_population),
+            p_reset * excited_population,
+        ]
         if t1 < t2:
             self.coefficients.append(np.exp(-time / t2))
         else:
             pz = p_reset + np.exp(-time / t2) * (1 - np.exp(time / t1))
             self.coefficients.append(pz)
 
     def apply_density_matrix(self, backend, state, nqubits):
         q = self.target_qubits[0]
         if self.t1 < self.t2:
             from qibo.gates import Unitary
+
             preset0, preset1, exp_t2 = self.coefficients
-            matrix = [[1 - preset1, 0, 0, preset1],
-                      [0, exp_t2, 0, 0],
-                      [0, 0, exp_t2, 0],
-                      [preset0, 0, 0, 1 - preset0]]
+            matrix = [
+                [1 - preset1, 0, 0, preset1],
+                [0, exp_t2, 0, 0],
+                [0, 0, exp_t2, 0],
+                [preset0, 0, 0, 1 - preset0],
+            ]
 
             qubits = (q, q + nqubits)
             gate = Unitary(matrix, *qubits)
             return backend.thermal_error_density_matrix(gate, state, nqubits)
 
         else:
             from qibo.gates import Z
+
             pz = self.coefficients[-1]
-            return (backend.reset_error_density_matrix(self, state, nqubits) -
-                    pz * backend.cast(state) +
-                    pz * backend.apply_gate_density_matrix(Z(0), state, nqubits))
+            return (
+                backend.reset_error_density_matrix(self, state, nqubits)
+                - pz * backend.cast(state)
+                + pz * backend.apply_gate_density_matrix(Z(0), state, nqubits)
+            )
```

### Comparing `qibo-0.1.8rc0/src/qibo/gates/gates.py` & `qibo-0.1.9/src/qibo/gates/gates.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,61 +1,97 @@
 import math
-from qibo.config import raise_error
 from typing import Dict, List, Optional, Tuple
-from qibo.gates.abstract import Gate, ParametrizedGate
 
+from qibo.config import raise_error
+from qibo.gates.abstract import Gate, ParametrizedGate
 
-QASM_GATES = {"h": "H", "x": "X", "y": "Y", "z": "Z",
-              "rx": "RX", "ry": "RY", "rz": "RZ",
-              "u1": "U1", "u2": "U2", "u3": "U3",
-              "cx": "CNOT", "swap": "SWAP", "fswap": "FSWAP", "cz": "CZ",
-              "crx": "CRX", "cry": "CRY", "crz": "CRZ",
-              "cu1": "CU1", "cu3": "CU3",
-              "ccx": "TOFFOLI", "id": "I", "s": "S",
-              "sdg": "SDG", "t": "T", "tdg": "TDG"}
-PARAMETRIZED_GATES = {"rx", "ry", "rz", "u1", "u2", "u3",
-                      "crx", "cry", "crz", "cu1", "cu3"}
+QASM_GATES = {
+    "h": "H",
+    "x": "X",
+    "y": "Y",
+    "z": "Z",
+    "rx": "RX",
+    "ry": "RY",
+    "rz": "RZ",
+    "u1": "U1",
+    "u2": "U2",
+    "u3": "U3",
+    "cx": "CNOT",
+    "swap": "SWAP",
+    "fswap": "FSWAP",
+    "rxx": "RXX",
+    "ryy": "RYY",
+    "rzz": "RZZ",
+    "cz": "CZ",
+    "crx": "CRX",
+    "cry": "CRY",
+    "crz": "CRZ",
+    "cu1": "CU1",
+    "cu3": "CU3",
+    "ccx": "TOFFOLI",
+    "id": "I",
+    "s": "S",
+    "sdg": "SDG",
+    "t": "T",
+    "tdg": "TDG",
+}
+PARAMETRIZED_GATES = {
+    "rx",
+    "ry",
+    "rz",
+    "rxx",
+    "ryy",
+    "rzz",
+    "u1",
+    "u2",
+    "u3",
+    "crx",
+    "cry",
+    "crz",
+    "cu1",
+    "cu3",
+}
 
 
 class H(Gate):
     """The Hadamard gate.
 
     Args:
         q (int): the qubit id number.
     """
 
     def __init__(self, q):
-        super(H, self).__init__()
+        super().__init__()
         self.name = "h"
         self.target_qubits = (q,)
         self.init_args = [q]
 
 
 class X(Gate):
     """The Pauli X gate.
 
     Args:
         q (int): the qubit id number.
     """
 
     def __init__(self, q):
-        super(X, self).__init__()
+        super().__init__()
         self.name = "x"
         self.target_qubits = (q,)
         self.init_args = [q]
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CNOT and Toffoli if there is one or two controls."""
         if len(q) == 1:
             gate = CNOT(q[0], self.target_qubits[0])
         elif len(q) == 2:
             gate = TOFFOLI(q[0], q[1], self.target_qubits[0])
         else:
-            gate = super(X, self).controlled_by(*q)
+            gate = super().controlled_by(*q)
         return gate
 
     def decompose(self, *free, use_toffolis=True):
         """Decomposes multi-control ``X`` gate to one-qubit, ``CNOT`` and ``TOFFOLI`` gates.
 
         Args:
             free: Ids of free qubits to use for the gate decomposition.
@@ -64,33 +100,38 @@
                 See :class:`qibo.gates.TOFFOLI` for more details on this representation.
 
         Returns:
             List with one-qubit, ``CNOT`` and ``TOFFOLI`` gates that have the
             same effect as applying the original multi-control gate.
         """
         if set(free) & set(self.qubits):
-            raise_error(ValueError, "Cannot decompose multi-control X gate if free "
-                                    "qubits coincide with target or controls.")
+            raise_error(
+                ValueError,
+                "Cannot decompose multi-control X gate if free "
+                "qubits coincide with target or controls.",
+            )
 
         controls = self.control_qubits
         target = self.target_qubits[0]
         m = len(controls)
         if m < 3:
             return [self.__class__(target).controlled_by(*controls)]
 
         decomp_gates = []
         n = m + 1 + len(free)
         if (n >= 2 * m - 1) and (m >= 3):
-            gates1 = [TOFFOLI(controls[m - 2 - i],
-                              free[m - 4 - i],
-                              free[m - 3 - i]
-                              ).congruent(use_toffolis=use_toffolis)
-                      for i in range(m - 3)]
-            gates2 = TOFFOLI(controls[0], controls[1], free[0]
-                             ).congruent(use_toffolis=use_toffolis)
+            gates1 = [
+                TOFFOLI(
+                    controls[m - 2 - i], free[m - 4 - i], free[m - 3 - i]
+                ).congruent(use_toffolis=use_toffolis)
+                for i in range(m - 3)
+            ]
+            gates2 = TOFFOLI(controls[0], controls[1], free[0]).congruent(
+                use_toffolis=use_toffolis
+            )
             first_toffoli = TOFFOLI(controls[m - 1], free[m - 3], target)
 
             decomp_gates.append(first_toffoli)
             for gates in gates1:
                 decomp_gates.extend(gates)
             decomp_gates.extend(gates2)
             for gates in gates1[::-1]:
@@ -105,57 +146,59 @@
             free2 = controls[:m1] + tuple(free[1:])
             controls2 = controls[m1:] + (free[0],)
             x2 = self.__class__(target).controlled_by(*controls2)
             part2 = x2.decompose(*free2, use_toffolis=use_toffolis)
 
             decomp_gates = [*part1, *part2]
 
-        else: # pragma: no cover
+        else:  # pragma: no cover
             # impractical case
-            raise_error(NotImplementedError, "X decomposition not implemented "
-                                             "for zero free qubits.")
+            raise_error(
+                NotImplementedError,
+                "X decomposition not implemented " "for zero free qubits.",
+            )
 
         decomp_gates.extend(decomp_gates)
         return decomp_gates
 
 
 class Y(Gate):
     """The Pauli Y gate.
 
     Args:
         q (int): the qubit id number.
     """
 
     def __init__(self, q):
-        super(Y, self).__init__()
+        super().__init__()
         self.name = "y"
         self.target_qubits = (q,)
         self.init_args = [q]
 
 
 class Z(Gate):
     """The Pauli Z gate.
 
     Args:
         q (int): the qubit id number.
     """
 
     def __init__(self, q):
-        super(Z, self).__init__()
+        super().__init__()
         self.name = "z"
         self.target_qubits = (q,)
         self.init_args = [q]
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CZ if there is only one control."""
         if len(q) == 1:
             gate = CZ(q[0], self.target_qubits[0])
         else:
-            gate = super(Z, self).controlled_by(*q)
+            gate = super().controlled_by(*q)
         return gate
 
 
 class S(Gate):
     """The S gate.
 
     Corresponds to the following unitary matrix
@@ -259,27 +302,26 @@
     """The identity gate.
 
     Args:
         *q (int): the qubit id numbers.
     """
 
     def __init__(self, *q):
-        super(I, self).__init__()
+        super().__init__()
         self.name = "id"
         self.target_qubits = tuple(q)
         self.init_args = q
         # save the number of target qubits as parameter
         # for proper identity matrix construction
         self.parameters = 2 ** len(self.target_qubits)
 
 
 class Align(ParametrizedGate):
-
     def __init__(self, *q):
-        super(Align, self).__init__()
+        super().__init__()
         self.name = "align"
         self.target_qubits = tuple(q)
         self.init_args = q
         # save the number of target qubits as parameter
         # for proper identity matrix construction
         self.parameters = 2 ** len(self.target_qubits)
 
@@ -303,22 +345,25 @@
 
         self.parameters = theta
         self.init_args = [q]
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
     def _dagger(self) -> "Gate":
         """"""
-        return self.__class__(self.target_qubits[0], -self.parameters[0]) # pylint: disable=E1130
+        return self.__class__(
+            self.target_qubits[0], -self.parameters[0]
+        )  # pylint: disable=E1130
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CRn if there is only one control."""
         if len(q) == 1:
-            gate = self._controlled_gate( # pylint: disable=E1102
-                q[0], self.target_qubits[0], **self.init_kwargs)
+            gate = self._controlled_gate(  # pylint: disable=E1102
+                q[0], self.target_qubits[0], **self.init_kwargs
+            )
         else:
             gate = super().controlled_by(*q)
         return gate
 
 
 class RX(_Rn_):
     """Rotation around the X-axis of the Bloch sphere.
@@ -418,16 +463,17 @@
         self.init_args = [q]
         self.init_kwargs = {"trainable": trainable}
 
     @Gate.check_controls
     def controlled_by(self, *q):
         """Fall back to CUn if there is only one control."""
         if len(q) == 1:
-            gate = self._controlled_gate( # pylint: disable=E1102
-              q[0], self.target_qubits[0], **self.init_kwargs)
+            gate = self._controlled_gate(  # pylint: disable=E1102
+                q[0], self.target_qubits[0], **self.init_kwargs
+            )
         else:
             gate = super().controlled_by(*q)
         return gate
 
 
 class U1(_Un_):
     """First general unitary gate.
@@ -453,16 +499,16 @@
         self.name = "u1"
         self._controlled_gate = CU1
         self.nparams = 1
         self.parameters = theta
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
     def _dagger(self) -> "Gate":
-        theta = - self.parameters[0]
-        return self.__class__(self.target_qubits[0], theta) # pylint: disable=E1130
+        theta = -self.parameters[0]
+        return self.__class__(self.target_qubits[0], theta)  # pylint: disable=E1130
 
 
 class U2(_Un_):
     """Second general unitary gate.
 
     Corresponds to the following unitary matrix
 
@@ -491,15 +537,15 @@
         self.init_kwargs = {"phi": phi, "lam": lam, "trainable": trainable}
         self.parameter_names = ["phi", "lam"]
         self.parameters = phi, lam
 
     def _dagger(self) -> "Gate":
         """"""
         phi, lam = self.parameters
-        phi, lam = math.pi - lam, - math.pi - phi
+        phi, lam = math.pi - lam, -math.pi - phi
         return self.__class__(self.target_qubits[0], phi, lam)
 
 
 class U3(_Un_):
     """Third general unitary gate.
 
     Corresponds to the following unitary matrix
@@ -522,22 +568,26 @@
 
     def __init__(self, q, theta, phi, lam, trainable=True):
         super().__init__(q, trainable=trainable)
         self.name = "u3"
         self._controlled_gate = CU3
         self.nparams = 3
         self._theta, self._phi, self._lam = None, None, None
-        self.init_kwargs = {"theta": theta, "phi": phi, "lam": lam,
-                            "trainable": trainable}
+        self.init_kwargs = {
+            "theta": theta,
+            "phi": phi,
+            "lam": lam,
+            "trainable": trainable,
+        }
         self.parameter_names = ["theta", "phi", "lam"]
         self.parameters = theta, phi, lam
 
     def _dagger(self) -> "Gate":
         """"""
-        theta, lam, phi = tuple(-x for x in self.parameters) # pylint: disable=E1130
+        theta, lam, phi = tuple(-x for x in self.parameters)  # pylint: disable=E1130
         return self.__class__(self.target_qubits[0], theta, phi, lam)
 
 
 class CNOT(Gate):
     """The Controlled-NOT gate.
 
     Corresponds to the following unitary matrix
@@ -552,15 +602,15 @@
 
     Args:
         q0 (int): the control qubit id number.
         q1 (int): the target qubit id number.
     """
 
     def __init__(self, q0, q1):
-        super(CNOT, self).__init__()
+        super().__init__()
         self.name = "cx"
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
 
     def decompose(self, *free, use_toffolis: bool = True) -> List[Gate]:
         q0, q1 = self.control_qubits[0], self.target_qubits[0]
@@ -582,15 +632,15 @@
 
     Args:
         q0 (int): the control qubit id number.
         q1 (int): the target qubit id number.
     """
 
     def __init__(self, q0, q1):
-        super(CZ, self).__init__()
+        super().__init__()
         self.name = "cz"
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
 
 
 class _CRn_(ParametrizedGate):
@@ -602,29 +652,29 @@
         theta (float): the rotation angle.
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
     """
 
     def __init__(self, q0, q1, theta, trainable=True):
-        super(_CRn_, self).__init__(trainable)
+        super().__init__(trainable)
         self.name = None
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.parameters = theta
 
         self.init_args = [q0, q1]
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
     def _dagger(self) -> "Gate":
         """"""
         q0 = self.control_qubits[0]
         q1 = self.target_qubits[0]
-        theta = - self.parameters[0]
-        return self.__class__(q0, q1, theta) # pylint: disable=E1130
+        theta = -self.parameters[0]
+        return self.__class__(q0, q1, theta)  # pylint: disable=E1130
 
 
 class CRX(_CRn_):
     """Controlled rotation around the X-axis for the Bloch sphere.
 
     Corresponds to the following unitary matrix
 
@@ -714,15 +764,15 @@
         q1 (int): the target qubit id number.
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
     """
 
     def __init__(self, q0, q1, trainable=True):
-        super(_CUn_, self).__init__(trainable)
+        super().__init__(trainable)
         self.name = None
         self.nparams = 0
         self.control_qubits = (q0,)
         self.target_qubits = (q1,)
         self.init_args = [q0, q1]
         self.init_kwargs = {"trainable": trainable}
 
@@ -758,16 +808,16 @@
         self.parameters = theta
         self.init_kwargs = {"theta": theta, "trainable": trainable}
 
     def _dagger(self) -> "Gate":
         """"""
         q0 = self.control_qubits[0]
         q1 = self.target_qubits[0]
-        theta = - self.parameters[0]
-        return self.__class__(q0, q1, theta) # pylint: disable=E1130
+        theta = -self.parameters[0]
+        return self.__class__(q0, q1, theta)  # pylint: disable=E1130
 
 
 class CU2(_CUn_):
     """Controlled second general unitary gate.
 
     Corresponds to the following unitary matrix
 
@@ -800,15 +850,15 @@
         self.parameters = phi, lam
 
     def _dagger(self) -> "Gate":
         """"""
         q0 = self.control_qubits[0]
         q1 = self.target_qubits[0]
         phi, lam = self.parameters
-        phi, lam = math.pi - lam, - math.pi - phi
+        phi, lam = math.pi - lam, -math.pi - phi
         return self.__class__(q0, q1, phi, lam)
 
 
 class CU3(_CUn_):
     """Controlled third general unitary gate.
 
     Corresponds to the following unitary matrix
@@ -829,28 +879,32 @@
         lamb (float): third rotation angle.
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
     """
 
     def __init__(self, q0, q1, theta, phi, lam, trainable=True):
-        super(CU3, self).__init__(q0, q1, trainable=trainable)
+        super().__init__(q0, q1, trainable=trainable)
         self.name = "cu3"
         self.nparams = 3
         self._theta, self._phi, self._lam = None, None, None
-        self.init_kwargs = {"theta": theta, "phi": phi, "lam": lam,
-                            "trainable": trainable}
+        self.init_kwargs = {
+            "theta": theta,
+            "phi": phi,
+            "lam": lam,
+            "trainable": trainable,
+        }
         self.parameter_names = ["theta", "phi", "lam"]
         self.parameters = theta, phi, lam
 
     def _dagger(self) -> "Gate":
         """"""
         q0 = self.control_qubits[0]
         q1 = self.target_qubits[0]
-        theta, lam, phi = tuple(-x for x in self.parameters) # pylint: disable=E1130
+        theta, lam, phi = tuple(-x for x in self.parameters)  # pylint: disable=E1130
         return self.__class__(q0, q1, theta, phi, lam)
 
 
 class SWAP(Gate):
     """The swap gate.
 
     Corresponds to the following unitary matrix
@@ -865,15 +919,15 @@
 
     Args:
         q0 (int): the first qubit to be swapped id number.
         q1 (int): the second qubit to be swapped id number.
     """
 
     def __init__(self, q0, q1):
-        super(SWAP, self).__init__()
+        super().__init__()
         self.name = "swap"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
 
 
 class FSWAP(Gate):
     """The fermionic swap gate.
@@ -890,15 +944,15 @@
 
     Args:
         q0 (int): the first qubit to be f-swapped id number.
         q1 (int): the second qubit to be f-swapped id number.
     """
 
     def __init__(self, q0, q1):
-        super(FSWAP, self).__init__()
+        super().__init__()
         self.name = "fswap"
         self.target_qubits = (q0, q1)
         self.init_args = [q0, q1]
 
 
 class fSim(ParametrizedGate):
     """The fSim gate defined in `arXiv:2001.08343 <https://arxiv.org/abs/2001.08343>`_.
@@ -918,32 +972,33 @@
         q1 (int): the second qubit to be swapped id number.
         theta (float): Angle for the one-qubit rotation.
         phi (float): Angle for the ``|11>`` phase.
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
     """
+
     # TODO: Check how this works with QASM.
 
     def __init__(self, q0, q1, theta, phi, trainable=True):
-        super(fSim, self).__init__(trainable)
+        super().__init__(trainable)
         self.name = "fsim"
         self.target_qubits = (q0, q1)
 
         self.parameter_names = ["theta", "phi"]
         self.parameters = theta, phi
         self.nparams = 2
 
         self.init_args = [q0, q1]
         self.init_kwargs = {"theta": theta, "phi": phi, "trainable": trainable}
 
     def _dagger(self) -> "Gate":
         """"""
         q0, q1 = self.target_qubits
-        params = (-x for x in self.parameters) # pylint: disable=E1130
+        params = (-x for x in self.parameters)  # pylint: disable=E1130
         return self.__class__(q0, q1, *params)
 
 
 class GeneralizedfSim(ParametrizedGate):
     """The fSim gate with a general rotation.
 
     Corresponds to the following unitary matrix
@@ -963,55 +1018,167 @@
         phi (float): Angle for the ``|11>`` phase.
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
     """
 
     def __init__(self, q0, q1, unitary, phi, trainable=True):
-        super(GeneralizedfSim, self).__init__(trainable)
+        super().__init__(trainable)
         self.name = "generalizedfsim"
         self.target_qubits = (q0, q1)
 
         self.parameter_names = ["u", "phi"]
         self.parameters = unitary, phi
         self.nparams = 5
 
         self.init_args = [q0, q1]
-        self.init_kwargs = {"unitary": unitary, "phi": phi,
-                            "trainable": trainable}
+        self.init_kwargs = {"unitary": unitary, "phi": phi, "trainable": trainable}
 
     def _dagger(self):
         import numpy as np
+
         q0, q1 = self.target_qubits
         u, phi = self.parameters
         init_kwargs = dict(self.init_kwargs)
         init_kwargs["unitary"] = np.conj(np.transpose(u))
         init_kwargs["phi"] = -phi
         return self.__class__(q0, q1, **init_kwargs)
 
     @Gate.parameters.setter
     def parameters(self, x):
         shape = tuple(x[0].shape)
         if shape != (2, 2):
-            raise_error(ValueError, "Invalid rotation shape {} for generalized "
-                                    "fSim gate".format(shape))
-        ParametrizedGate.parameters.fset(self, x) # pylint: disable=no-member
+            raise_error(
+                ValueError,
+                "Invalid rotation shape {} for generalized " "fSim gate".format(shape),
+            )
+        ParametrizedGate.parameters.fset(self, x)  # pylint: disable=no-member
+
+
+class _Rnn_(ParametrizedGate):
+    """Abstract class for defining the RXX, RYY and RZZ rotations.
+
+    Args:
+        q0 (int): the first entangled qubit id number.
+        q1 (int): the second entangled qubit id number.
+        theta (float): the rotation angle.
+        trainable (bool): whether gate parameters can be updated using
+            :meth:`qibo.models.circuit.AbstractCircuit.set_parameters`
+            (default is ``True``).
+    """
+
+    def __init__(self, q0, q1, theta, trainable=True):
+        super().__init__(trainable)
+        self.name = None
+        self._controlled_gate = None
+        self.target_qubits = (q0, q1)
+
+        self.parameters = theta
+        self.init_args = [q0, q1]
+        self.init_kwargs = {"theta": theta, "trainable": trainable}
+
+    def _dagger(self) -> "Gate":
+        """"""
+        q0, q1 = self.target_qubits
+        return self.__class__(q0, q1, -self.parameters[0])  # pylint: disable=E1130
+
+
+class RXX(_Rnn_):
+    """Parametric 2-qubit X \\otimes X interaction, or rotation about XX.
+
+    This is a symmetric gate.
+
+    Corresponds to the following unitary matrix
+
+    .. math::
+        \\begin{pmatrix}
+        \\cos \\frac{\\theta }{2} & 0 & 0 & -i\\sin \\frac{\\theta }{2} \\\\
+        0 & \\cos \\frac{\\theta }{2} & -i\\sin \\frac{\\theta }{2} & 0 \\\\
+        0 & -i\\sin \\frac{\\theta }{2} & \\cos \\frac{\\theta }{2} & 0 \\\\
+        -i\\sin \\frac{\\theta }{2} & 0 & 0 & \\cos \\frac{\\theta }{2} \\\\
+        \\end{pmatrix}
+
+    Args:
+        q0 (int): the first entangled qubit id number.
+        q1 (int): the second entangled qubit id number.
+        theta (float): the rotation angle.
+        trainable (bool): whether gate parameters can be updated using
+            :meth:`qibo.models.circuit.AbstractCircuit.set_parameters`
+            (default is ``True``).
+    """
+
+    def __init__(self, q0, q1, theta, trainable=True):
+        super().__init__(q0, q1, theta, trainable)
+        self.name = "rxx"
+
+
+class RYY(_Rnn_):
+    """Parametric 2-qubit Y \\otimes Y interaction, or rotation about YY.
+
+    Corresponds to the following unitary matrix
+
+    .. math::
+        \\begin{pmatrix}
+        \\cos \\frac{\\theta }{2} & 0 & 0 & i\\sin \\frac{\\theta }{2} \\\\
+        0 & \\cos \\frac{\\theta }{2} & -i\\sin \\frac{\\theta }{2} & 0 \\\\
+        0 & -i\\sin \\frac{\\theta }{2} & \\cos \\frac{\\theta }{2} & 0 \\\\
+        i\\sin \\frac{\\theta }{2} & 0 & 0 & \\cos \\frac{\\theta }{2} \\\\
+        \\end{pmatrix}
+
+    Args:
+        q0 (int): the first entangled qubit id number.
+        q1 (int): the second entangled qubit id number.
+        trainable (bool): whether gate parameters can be updated using
+            :meth:`qibo.models.circuit.Circuit.set_parameters`
+            (default is ``True``).
+    """
+
+    def __init__(self, q0, q1, theta, trainable=True):
+        super().__init__(q0, q1, theta, trainable)
+        self.name = "ryy"
+
+
+class RZZ(_Rnn_):
+    """Parametric 2-qubit Z \\otimes Z interaction, or rotation about ZZ.
+
+    Corresponds to the following unitary matrix
+
+    .. math::
+        \\begin{pmatrix}
+        e^{-i \\theta / 2} & 0 & 0 & 0 \\\\
+        0 & e^{i \\theta / 2} & 0 & 0 \\\\
+        0 & 0 & e^{i \\theta / 2} & 0 \\\\
+        0 & 0 & 0 & e^{-i \\theta / 2} \\\\
+        \\end{pmatrix}
+
+    Args:
+        q0 (int): the first entangled qubit id number.
+        q1 (int): the second entangled qubit id number.
+        theta (float): the rotation angle.
+        trainable (bool): whether gate parameters can be updated using
+            :meth:`qibo.models.circuit.Circuit.set_parameters`
+            (default is ``True``).
+    """
+
+    def __init__(self, q0, q1, theta, trainable=True):
+        super().__init__(q0, q1, theta, trainable)
+        self.name = "rzz"
 
 
 class TOFFOLI(Gate):
     """The Toffoli gate.
 
     Args:
         q0 (int): the first control qubit id number.
         q1 (int): the second control qubit id number.
         q2 (int): the target qubit id number.
     """
 
     def __init__(self, q0, q1, q2):
-        super(TOFFOLI, self).__init__()
+        super().__init__()
         self.name = "ccx"
         self.control_qubits = (q0, q1)
         self.target_qubits = (q2,)
         self.init_args = [q0, q1, q2]
 
     def decompose(self, *free, use_toffolis: bool = True) -> List[Gate]:
         c0, c1 = self.control_qubits
@@ -1035,20 +1202,26 @@
             List with ``RY`` and ``CNOT`` gates that have the same effect as
             applying the original ``TOFFOLI`` gate.
         """
         if use_toffolis:
             return self.decompose()
 
         import importlib
+
         control0, control1 = self.control_qubits
         target = self.target_qubits[0]
-        return [RY(target, -math.pi / 4), CNOT(control1, target),
-                RY(target, -math.pi / 4), CNOT(control0, target),
-                RY(target, math.pi / 4), CNOT(control1, target),
-                RY(target, math.pi / 4)]
+        return [
+            RY(target, -math.pi / 4),
+            CNOT(control1, target),
+            RY(target, -math.pi / 4),
+            CNOT(control0, target),
+            RY(target, math.pi / 4),
+            CNOT(control1, target),
+            RY(target, math.pi / 4),
+        ]
 
 
 class Unitary(ParametrizedGate):
     """Arbitrary unitary gate.
 
     Args:
         unitary: Unitary matrix as a tensor supported by the backend.
@@ -1058,40 +1231,43 @@
         trainable (bool): whether gate parameters can be updated using
             :meth:`qibo.models.circuit.Circuit.set_parameters`
             (default is ``True``).
         name (str): Optional name for the gate.
     """
 
     def __init__(self, unitary, *q, trainable=True, name=None):
-        super(Unitary, self).__init__(trainable)
+        super().__init__(trainable)
         self.name = "Unitary" if name is None else name
         self.target_qubits = tuple(q)
 
         # TODO: Check that given ``unitary`` has proper shape?
         self.parameter_names = "u"
         self._parameters = (unitary,)
         self.nparams = 4 ** len(self.target_qubits)
 
         self.init_args = [unitary] + list(q)
         self.init_kwargs = {"name": name, "trainable": trainable}
 
     @Gate.parameters.setter
     def parameters(self, x):
         import numpy as np
+
         shape = self.parameters[0].shape
         self._parameters = (np.reshape(x, shape),)
         for gate in self.device_gates:  # pragma: no cover
             gate.parameters = x
 
     def on_qubits(self, qubit_map):
         args = [self.init_args[0]]
-        args.extend((qubit_map.get(i) for i in self.target_qubits))
+        args.extend(qubit_map.get(i) for i in self.target_qubits)
         gate = self.__class__(*args, **self.init_kwargs)
         if self.is_controlled_by:
             controls = (qubit_map.get(i) for i in self.control_qubits)
             gate = gate.controlled_by(*controls)
+        gate.parameters = self.parameters
         return gate
 
     def _dagger(self):
         import numpy as np
+
         ud = np.conj(np.transpose(self.parameters[0]))
         return self.__class__(ud, *self.target_qubits, **self.init_kwargs)
```

### Comparing `qibo-0.1.8rc0/src/qibo/gates/measurements.py` & `qibo-0.1.9/src/qibo/gates/measurements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,44 @@
+from typing import Dict, Optional, Tuple
+
 import sympy
+
 from qibo.config import raise_error
 from qibo.gates.abstract import Gate
-from typing import Dict, Optional, Tuple
 
 
 class MeasurementResult:
-
     def __init__(self, qubits):
         self.qubits = qubits
         self.samples = []
 
     def append(self, shot):
         self.samples.append(shot)
 
 
 class MeasurementSymbol(sympy.Symbol):
     """``sympy.Symbol`` connected to measurement results.
 
     Used by :class:`qibo.gates.measurements.M` with ``collapse=True`` to allow
     controlling subsequent gates from the measurement results.
     """
+
     _counter = 0
 
     def __new__(cls, *args, **kwargs):
         name = "m{}".format(cls._counter)
         cls._counter += 1
         return super().__new__(cls=cls, name=name)
 
     def __init__(self, index, result):
         self.index = index
         self.result = result
 
     def __getstate__(self):
-        return {
-            "index": self.index,
-            "result": self.result,
-            "name": self.name
-        }
+        return {"index": self.index, "result": self.result, "name": self.name}
 
     def __setstate__(self, data):
         self.index = data.get("index")
         self.result = data.get("result")
         self.name = data.get("name")
 
     def outcome(self):
@@ -79,84 +77,102 @@
             for all qubits.
         p1 (dict): Optional bitflip probability map for asymmetric bitflips.
             Same as ``p0`` but controls the 1->0 bitflip probability.
             If ``p1`` is ``None`` then ``p0`` will be used both for 0->1 and
             1->0 bitflips.
     """
 
-    def __init__(self, *q, register_name: Optional[str] = None,
-                 collapse: bool = False,
-                 p0: Optional["ProbsType"] = None,
-                 p1: Optional["ProbsType"] = None):
+    def __init__(
+        self,
+        *q,
+        register_name: Optional[str] = None,
+        collapse: bool = False,
+        p0: Optional["ProbsType"] = None,
+        p1: Optional["ProbsType"] = None,
+    ):
         super().__init__()
         self.name = "measure"
         self.target_qubits = tuple(q)
         self.register_name = register_name
         self.collapse = collapse
         self.result = None
 
         self.init_args = q
-        self.init_kwargs = {"register_name": register_name,
-                            "collapse": collapse,
-                            "p0": p0, "p1": p1}
+        self.init_kwargs = {
+            "register_name": register_name,
+            "collapse": collapse,
+            "p0": p0,
+            "p1": p1,
+        }
         if collapse:
             if p0 is not None or p1 is not None:
-                raise_error(NotImplementedError, "Bitflip measurement noise is not "
-                                                "available when collapsing.")
+                raise_error(
+                    NotImplementedError,
+                    "Bitflip measurement noise is not " "available when collapsing.",
+                )
             self.result = MeasurementResult(self.target_qubits)
 
-        if p1 is None: p1 = p0
-        if p0 is None: p0 = p1
-        self.bitflip_map = (self._get_bitflip_map(p0),
-                            self._get_bitflip_map(p1))
+        if p1 is None:
+            p1 = p0
+        if p0 is None:
+            p0 = p1
+        self.bitflip_map = (self._get_bitflip_map(p0), self._get_bitflip_map(p1))
 
     def get_symbols(self):
         symbols = []
         for i, q in enumerate(self.target_qubits):
             symbols.append(MeasurementSymbol(i, self.result))
         if len(self.target_qubits) > 1:
             return symbols
         else:
             return symbols[0]
 
     @staticmethod
-    def _get_bitflip_tuple(qubits: Tuple[int], probs: "ProbsType"
-                           ) -> Tuple[float]:
+    def _get_bitflip_tuple(qubits: Tuple[int], probs: "ProbsType") -> Tuple[float]:
         if isinstance(probs, float):
             if probs < 0 or probs > 1:  # pragma: no cover
-                raise_error(ValueError, "Invalid bitflip probability {}."
-                                        "".format(probs))
+                raise_error(
+                    ValueError, "Invalid bitflip probability {}." "".format(probs)
+                )
             return len(qubits) * (probs,)
 
         if isinstance(probs, (tuple, list)):
             if len(probs) != len(qubits):
-                raise_error(ValueError, "{} qubits were measured but the given "
-                                        "bitflip probability list contains {} "
-                                        "values.".format(
-                                            len(qubits), len(probs)))
+                raise_error(
+                    ValueError,
+                    "{} qubits were measured but the given "
+                    "bitflip probability list contains {} "
+                    "values.".format(len(qubits), len(probs)),
+                )
             return tuple(probs)
 
         if isinstance(probs, dict):
             diff = set(probs.keys()) - set(qubits)
             if diff:
-                raise_error(KeyError, "Bitflip map contains {} qubits that are "
-                                      "not measured.".format(diff))
+                raise_error(
+                    KeyError,
+                    "Bitflip map contains {} qubits that are "
+                    "not measured.".format(diff),
+                )
             return tuple(probs[q] if q in probs else 0.0 for q in qubits)
 
         raise_error(TypeError, "Invalid type {} of bitflip map.".format(probs))
 
     def _get_bitflip_map(self, p: Optional["ProbsType"] = None) -> Dict[int, float]:
         """Creates dictionary with bitflip probabilities."""
         if p is None:
             return {q: 0 for q in self.qubits}
         pt = self._get_bitflip_tuple(self.qubits, p)
         return {q: p for q, p in zip(self.qubits, pt)}
 
     def has_bitflip_noise(self):
-        return sum(self.bitflip_map[0].values()) > 0 or sum(self.bitflip_map[1].values()) > 0
+        return (
+            sum(self.bitflip_map[0].values()) > 0
+            or sum(self.bitflip_map[1].values()) > 0
+        )
 
     @staticmethod
     def einsum_string(qubits, nqubits, measuring=False):
         """Generates einsum string for partial trace of density matrices.
 
         Args:
             qubits (list): Set of qubit ids that are traced out.
@@ -167,15 +183,16 @@
 
         Returns:
             String to use in einsum for performing partial density of a
             density matrix.
         """
         # TODO: Move this somewhere else (if it is needed at all)
         from qibo.config import EINSUM_CHARS
-        if (2 - int(measuring)) * nqubits > len(EINSUM_CHARS): # pragma: no cover
+
+        if (2 - int(measuring)) * nqubits > len(EINSUM_CHARS):  # pragma: no cover
             # case not tested because it requires large instance
             raise_error(NotImplementedError, "Not enough einsum characters.")
 
         left_in, right_in, left_out, right_out = [], [], [], []
         for i in range(nqubits):
             left_in.append(EINSUM_CHARS[i])
             if i in qubits:
@@ -211,15 +228,17 @@
     def controlled_by(self, *q):
         """"""
         raise_error(NotImplementedError, "Measurement gates cannot be controlled.")
 
     @property
     def matrix(self):
         """"""
-        raise_error(NotImplementedError, "Measurement gates do not have matrix representation.")
+        raise_error(
+            NotImplementedError, "Measurement gates do not have matrix representation."
+        )
 
     def apply(self, backend, state, nqubits):
         qubits = sorted(self.target_qubits)
         # measure and get result
         probs = backend.calculate_probabilities(state, qubits, nqubits)
         shot = backend.sample_shots(probs, 1)
         # update the gate's result with the measurement outcome
```

### Comparing `qibo-0.1.8rc0/src/qibo/gates/special.py` & `qibo-0.1.9/src/qibo/gates/special.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     This gate performs the callback calulation without affecting the state vector.
 
     Args:
         callback (:class:`qibo.callbacks.Callback`): Callback object to calculate.
     """
 
     def __init__(self, callback: "Callback"):
-        super(CallbackGate, self).__init__()
+        super().__init__()
         self.name = callback.__class__.__name__
         self.callback = callback
         self.init_args = [callback]
 
     def apply(self, backend, state, nqubits):
         self.callback.nqubits = nqubits
         self.callback.apply(backend, state)
@@ -109,28 +109,28 @@
             return
 
         qubits = self.qubit_set & gate.qubit_set
         # the gate with most neighbors different than the two gates to
         # fuse will be the parent
         if len(left_gates) > len(right_gates):
             parent, child = self, gate
-            between_gates = set(parent.right_neighbors.get(q) for q in qubits)
+            between_gates = {parent.right_neighbors.get(q) for q in qubits}
             if between_gates == {child}:
                 child.marked = True
                 parent.append(child)
                 for q in qubits:
                     neighbor = child.right_neighbors.get(q)
                     if neighbor is not None:
                         parent.right_neighbors[q] = neighbor
                         neighbor.left_neighbors[q] = parent
                     else:
                         parent.right_neighbors.pop(q)
         else:
             parent, child = gate, self
-            between_gates = set(parent.left_neighbors.get(q) for q in qubits)
+            between_gates = {parent.left_neighbors.get(q) for q in qubits}
             if between_gates == {child}:
                 child.marked = True
                 parent.prepend(child)
                 for q in qubits:
                     neighbor = child.left_neighbors.get(q)
                     if neighbor is not None:
                         parent.left_neighbors[q] = neighbor
```

### Comparing `qibo-0.1.8rc0/src/qibo/hamiltonians/abstract.py` & `qibo-0.1.9/src/qibo/hamiltonians/abstract.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import abstractmethod
+
 from qibo.config import raise_error
 
 
 class AbstractHamiltonian:
     """Qibo abstraction for Hamiltonian objects."""
 
     def __init__(self):
@@ -11,36 +12,38 @@
     @property
     def nqubits(self):
         return self._nqubits
 
     @nqubits.setter
     def nqubits(self, n):
         if not isinstance(n, int):
-            raise_error(RuntimeError, "nqubits must be an integer but is "
-                                      "{}.".format(type(n)))
+            raise_error(
+                RuntimeError, "nqubits must be an integer but is " "{}.".format(type(n))
+            )
         if n < 1:
-            raise_error(ValueError, "nqubits must be a positive integer but is "
-                                    "{}".format(n))
+            raise_error(
+                ValueError, "nqubits must be a positive integer but is " "{}".format(n)
+            )
         self._nqubits = n
 
     @abstractmethod
-    def eigenvalues(self, k=6): # pragma: no cover
+    def eigenvalues(self, k=6):  # pragma: no cover
         """Computes the eigenvalues for the Hamiltonian.
 
         Args:
             k (int): Number of eigenvalues to calculate if the Hamiltonian
                 was created using a sparse matrix. This argument is ignored
                 if the Hamiltonian was created using a dense matrix.
                 See :meth:`qibo.backends.abstract.AbstractBackend.eigvalsh` for
                 more details.
         """
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def eigenvectors(self, k=6): # pragma: no cover
+    def eigenvectors(self, k=6):  # pragma: no cover
         """Computes a tensor with the eigenvectors for the Hamiltonian.
 
         Args:
             k (int): Number of eigenvalues to calculate if the Hamiltonian
                 was created using a sparse matrix. This argument is ignored
                 if the Hamiltonian was created using a dense matrix.
                 See :meth:`qibo.backends.abstract.AbstractBackend.eigh` for
@@ -53,62 +56,77 @@
 
         Uses :meth:`qibo.hamiltonians.AbstractHamiltonian.eigenvectors`
         and returns eigenvector corresponding to the lowest energy.
         """
         return self.eigenvectors()[:, 0]
 
     @abstractmethod
-    def exp(self, a): # pragma: no cover
+    def exp(self, a):  # pragma: no cover
         """Computes a tensor corresponding to exp(-1j * a * H).
 
         Args:
             a (complex): Complex number to multiply Hamiltonian before
                 exponentiation.
         """
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def expectation(self, state, normalize=False): # pragma: no cover
+    def expectation(self, state, normalize=False):  # pragma: no cover
         """Computes the real expectation value for a given state.
 
         Args:
             state (array): the expectation state.
             normalize (bool): If ``True`` the expectation value is divided
                 with the state's norm squared.
 
         Returns:
             Real number corresponding to the expectation value.
         """
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def __add__(self, o): # pragma: no cover
+    def expectation_from_samples(self, freq, qubit_map=None):  # pragma: no cover
+        """Computes the real expectation value of a diagonal observable given the frequencies when measuring in the computational basis.
+
+        Args:
+            freq (collections.Counter): the keys are the observed values in binary form
+            and the values the corresponding frequencies, that is the number
+            of times each measured value/bitstring appears.
+            qubit_map (tuple): Mapping between frequencies and qubits. If None, [1,...,len(key)]
+
+        Returns:
+            Real number corresponding to the expectation value.
+        """
+        raise_error(NotImplementedError)
+
+    @abstractmethod
+    def __add__(self, o):  # pragma: no cover
         """Add operator."""
         raise_error(NotImplementedError)
 
     def __radd__(self, o):
         """Right operator addition."""
         return self.__add__(o)
 
     @abstractmethod
-    def __sub__(self, o): # pragma: no cover
+    def __sub__(self, o):  # pragma: no cover
         """Subtraction operator."""
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def __rsub__(self, o): # pragma: no cover
+    def __rsub__(self, o):  # pragma: no cover
         """Right subtraction operator."""
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def __mul__(self, o): # pragma: no cover
+    def __mul__(self, o):  # pragma: no cover
         """Multiplication to scalar operator."""
         raise_error(NotImplementedError)
 
     def __rmul__(self, o):
         """Right scalar multiplication."""
         return self.__mul__(o)
 
     @abstractmethod
-    def __matmul__(self, o): # pragma: no cover
+    def __matmul__(self, o):  # pragma: no cover
         """Matrix multiplication with other Hamiltonians or state vectors."""
         raise_error(NotImplementedError)
```

### Comparing `qibo-0.1.8rc0/src/qibo/hamiltonians/adiabatic.py` & `qibo-0.1.9/src/qibo/hamiltonians/adiabatic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC, abstractmethod
+
 from qibo.config import raise_error
 from qibo.hamiltonians import hamiltonians, terms
 
 
 class AdiabaticHamiltonian(ABC):
     """Constructor for Hamiltonians used in adiabatic evolution.
 
@@ -12,54 +13,62 @@
 
     These objects allow constructing the adiabatic Hamiltonian of the
     form ``(1 - s) * H0 + s * H1`` efficiently.
     """
 
     def __new__(cls, h0, h1):
         if type(h1) != type(h0):
-            raise_error(TypeError, "h1 should be of the same type {} of h0 but "
-                                   "is {}.".format(type(h0), type(h1)))
+            raise_error(
+                TypeError,
+                "h1 should be of the same type {} of h0 but "
+                "is {}.".format(type(h0), type(h1)),
+            )
         if isinstance(h0, hamiltonians.Hamiltonian):
             return BaseAdiabaticHamiltonian(h0, h1)
         elif isinstance(h0, hamiltonians.SymbolicHamiltonian):
             return SymbolicAdiabaticHamiltonian(h0, h1)
         else:
-            raise_error(TypeError, "h0 should be a hamiltonians.Hamiltonian "
-                                   "object but is {}.".format(type(h0)))
+            raise_error(
+                TypeError,
+                "h0 should be a hamiltonians.Hamiltonian "
+                "object but is {}.".format(type(h0)),
+            )
 
-    def __init__(self, h0, h1): # pragma: no cover
+    def __init__(self, h0, h1):  # pragma: no cover
         self.h0, self.h1 = h0, h1
         self.schedule = None
         self.total_time = None
 
     @abstractmethod
-    def ground_state(self): # pragma: no cover
+    def ground_state(self):  # pragma: no cover
         """Returns the ground state of the ``H0`` Hamiltonian.
 
         Usually used as the initial state for adiabatic evolution.
         """
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def __call__(self, t): # pragma: no cover
+    def __call__(self, t):  # pragma: no cover
         """Hamiltonian object corresponding to the given time."""
         raise_error(NotImplementedError)
 
     @abstractmethod
-    def circuit(self, dt, accelerators=None, t=0): # pragma: no cover
+    def circuit(self, dt, accelerators=None, t=0):  # pragma: no cover
         raise_error(NotImplementedError)
 
 
 class BaseAdiabaticHamiltonian:
     """Adiabatic Hamiltonian that is a sum of :class:`qibo.hamiltonians.hamiltonians.Hamiltonian`."""
 
     def __init__(self, h0, h1):
         if h0.nqubits != h1.nqubits:
-            raise_error(ValueError, "H0 has {} qubits while H1 has {}."
-                                    "".format(h0.nqubits, h1.nqubits))
+            raise_error(
+                ValueError,
+                "H0 has {} qubits while H1 has {}." "".format(h0.nqubits, h1.nqubits),
+            )
         self.nqubits = h0.nqubits
         if h0.backend != h1.backend:  # pragma: no cover
             raise_error(ValueError, "H0 and H1 have different backend.")
         self.backend = h0.backend
         self.h0, self.h1 = h0, h1
         self.schedule = None
         self.total_time = None
@@ -73,40 +82,47 @@
         Returns:
             A :class:`qibo.hamiltonians.hamiltonians.Hamiltonian` object corresponding
             to the adiabatic Hamiltonian at a given time.
         """
         if t == 0:
             return self.h0
         if self.total_time is None or self.schedule is None:
-            raise_error(RuntimeError, "Cannot access adiabatic evolution "
-                                      "Hamiltonian before setting the "
-                                      "the total evolution time and "
-                                      "scheduling.")
-        st = self.schedule(t / self.total_time) # pylint: disable=E1102
+            raise_error(
+                RuntimeError,
+                "Cannot access adiabatic evolution "
+                "Hamiltonian before setting the "
+                "the total evolution time and "
+                "scheduling.",
+            )
+        st = self.schedule(t / self.total_time)  # pylint: disable=E1102
         return self.h0 * (1 - st) + self.h1 * st
 
-    def circuit(self, dt, accelerators=None, t=0): # pragma: no cover
-        raise_error(NotImplementedError, "Trotter circuit is not available "
-                                         "for full matrix Hamiltonians.")
+    def circuit(self, dt, accelerators=None, t=0):  # pragma: no cover
+        raise_error(
+            NotImplementedError,
+            "Trotter circuit is not available " "for full matrix Hamiltonians.",
+        )
 
 
 class TrotterCircuit(hamiltonians.TrotterCircuit):
     """Object that caches the Trotterized evolution circuit.
 
     See :class:`qibo.hamiltonians.hamiltonians.TrotterCircuit` for more details.
     """
 
     def set(self, dt, coefficients):
         """Updates the circuit parameters for different values of ``t`` and ``dt``.
 
         The update is done using the ``circuit.set_parameters`` method to avoid
         recreating the circuit and gates.
         """
-        params = {gate: group.to_term(coefficients).exp(dt / 2.0)
-                  for gate, group in self.gates.items()}
+        params = {
+            gate: group.to_term(coefficients).exp(dt / 2.0)
+            for gate, group in self.gates.items()
+        }
         self.dt = dt
         self.circuit.set_parameters(params)
 
 
 class SymbolicAdiabaticHamiltonian(BaseAdiabaticHamiltonian):
     """Adiabatic Hamiltonian that is sum of :class:`qibo.hamiltonians.hamiltonians.SymbolicHamiltonian`."""
 
@@ -135,13 +151,16 @@
                 circuits.
             t (float): Time that the Hamiltonian should be calculated.
 
         Returns:
             A :class:`qibo.models.Circuit` implementing the Trotterized evolution.
         """
         if self.trotter_circuit is None:
-            self.trotter_circuit = TrotterCircuit(self.groups, dt, self.nqubits,
-                                                  accelerators)
-        st = self.schedule(t / self.total_time) if t != 0 else 0 # pylint: disable=E1102
+            self.trotter_circuit = TrotterCircuit(
+                self.groups, dt, self.nqubits, accelerators
+            )
+        st = (
+            self.schedule(t / self.total_time) if t != 0 else 0
+        )  # pylint: disable=E1102
         coefficients = {self.h0: 1 - st, self.h1: st}
         self.trotter_circuit.set(dt, coefficients)
         return self.trotter_circuit.circuit
```

### Comparing `qibo-0.1.8rc0/src/qibo/hamiltonians/hamiltonians.py` & `qibo-0.1.9/src/qibo/hamiltonians/hamiltonians.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import sympy
-from qibo.config import raise_error, log, EINSUM_CHARS
+
+from qibo.config import EINSUM_CHARS, log, raise_error
 from qibo.hamiltonians.abstract import AbstractHamiltonian
+from qibo.symbols import Z
 
 
 class Hamiltonian(AbstractHamiltonian):
     """Hamiltonian based on a dense or sparse matrix representation.
 
     Args:
         nqubits (int): number of quantum bits.
         matrix (np.ndarray): Matrix representation of the Hamiltonian in the
             computational basis as an array of shape ``(2 ** nqubits, 2 ** nqubits)``.
             Sparse matrices based on ``scipy.sparse`` for numpy/qibojit backends
             or on ``tf.sparse`` for the tensorflow backend are also
             supported.
     """
+
     def __init__(self, nqubits, matrix=None, backend=None):
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             self.backend = GlobalBackend()
         else:
             self.backend = backend
 
-        if not (isinstance(matrix, self.backend.tensor_types) or self.backend.issparse(matrix)):
-            raise_error(TypeError, "Matrix of invalid type {} given during "
-                                   "Hamiltonian initialization"
-                                   "".format(type(matrix)))
+        if not (
+            isinstance(matrix, self.backend.tensor_types)
+            or self.backend.issparse(matrix)
+        ):
+            raise_error(
+                TypeError,
+                "Matrix of invalid type {} given during "
+                "Hamiltonian initialization"
+                "".format(type(matrix)),
+            )
         matrix = self.backend.cast(matrix)
 
         super().__init__()
         self.nqubits = nqubits
         self.matrix = matrix
         self._eigenvalues = None
         self._eigenvectors = None
@@ -42,18 +52,21 @@
         matrix, depending on how the Hamiltonian was created.
         """
         return self._matrix
 
     @matrix.setter
     def matrix(self, m):
         shape = tuple(m.shape)
-        if shape != 2 * (2 ** self.nqubits,):
-            raise_error(ValueError, "The Hamiltonian is defined for {} qubits "
-                                    "while the given matrix has shape {}."
-                                    "".format(self.nqubits, shape))
+        if shape != 2 * (2**self.nqubits,):
+            raise_error(
+                ValueError,
+                "The Hamiltonian is defined for {} qubits "
+                "while the given matrix has shape {}."
+                "".format(self.nqubits, shape),
+            )
         self._matrix = m
 
     @classmethod
     def from_symbolic(cls, symbolic_hamiltonian, symbol_map, backend=None):
         """Creates a ``Hamiltonian`` from a symbolic Hamiltonian.
 
         We refer to the :ref:`How to define custom Hamiltonians using symbols? <symbolicham-example>`
@@ -66,128 +79,179 @@
                 the Hamiltonian to a pair of (target, matrix).
 
         Returns:
             A :class:`qibo.hamiltonians.SymbolicHamiltonian` object
             that implements the Hamiltonian represented by the given symbolic
             expression.
         """
-        log.warning("`Hamiltonian.from_symbolic` and the use of symbol maps is "
-                    "deprecated. Please use `SymbolicHamiltonian` and Qibo symbols "
-                    "to construct Hamiltonians using symbols.")
+        log.warning(
+            "`Hamiltonian.from_symbolic` and the use of symbol maps is "
+            "deprecated. Please use `SymbolicHamiltonian` and Qibo symbols "
+            "to construct Hamiltonians using symbols."
+        )
         return SymbolicHamiltonian(symbolic_hamiltonian, symbol_map, backend=backend)
 
     def eigenvalues(self, k=6):
         if self._eigenvalues is None:
             self._eigenvalues = self.backend.calculate_eigenvalues(self.matrix, k)
         return self._eigenvalues
 
     def eigenvectors(self, k=6):
         if self._eigenvectors is None:
-            self._eigenvalues, self._eigenvectors = self.backend.calculate_eigenvectors(self.matrix, k)
+            self._eigenvalues, self._eigenvectors = self.backend.calculate_eigenvectors(
+                self.matrix, k
+            )
         return self._eigenvectors
 
     def exp(self, a):
         if self._exp.get("a") != a:
             self._exp["a"] = a
-            self._exp["result"] = self.backend.calculate_matrix_exp(a, self.matrix, self._eigenvectors,
-                                                             self._eigenvalues)
+            self._exp["result"] = self.backend.calculate_matrix_exp(
+                a, self.matrix, self._eigenvectors, self._eigenvalues
+            )
         return self._exp.get("result")
 
     def expectation(self, state, normalize=False):
         if isinstance(state, self.backend.tensor_types):
             shape = tuple(state.shape)
-            if len(shape) == 1: # state vector
-                return self.backend.calculate_expectation_state(self.matrix, state, normalize)
-            elif len(shape) == 2: # density matrix
-                return self.backend.calculate_expectation_density_matrix(self.matrix, state, normalize)
+            if len(shape) == 1:  # state vector
+                return self.backend.calculate_expectation_state(self, state, normalize)
+            elif len(shape) == 2:  # density matrix
+                return self.backend.calculate_expectation_density_matrix(
+                    self, state, normalize
+                )
             else:
-                raise_error(ValueError, "Cannot calculate Hamiltonian "
-                                        "expectation value for state of shape "
-                                        "{}.".format(shape))
-        else:
-            raise_error(TypeError, "Cannot calculate Hamiltonian expectation "
-                                   "value for state of type {}."
-                                   "".format(type(state)))
+                raise_error(
+                    ValueError,
+                    "Cannot calculate Hamiltonian "
+                    "expectation value for state of shape "
+                    "{}.".format(shape),
+                )
+        else:
+            raise_error(
+                TypeError,
+                "Cannot calculate Hamiltonian expectation "
+                "value for state of type {}."
+                "".format(type(state)),
+            )
+
+    def expectation_from_samples(self, freq, qubit_map=None):
+        import numpy as np
+
+        obs = self.matrix
+        if np.count_nonzero(obs - np.diag(np.diagonal(obs))) != 0:
+            raise_error(NotImplementedError, "Observable is not diagonal.")
+        keys = list(freq.keys())
+        if qubit_map is None:
+            qubit_map = list(range(int(np.log2(len(obs)))))
+        counts = np.array(list(freq.values())) / sum(freq.values())
+        expval = 0
+        kl = len(qubit_map)
+        for j, k in enumerate(keys):
+            index = 0
+            for i in qubit_map:
+                index += int(k[qubit_map.index(i)]) * 2 ** (kl - 1 - i)
+            expval += obs[index, index] * counts[j]
+        return expval
 
     def eye(self, n=None):
         if n is None:
             n = int(self.matrix.shape[0])
         return self.backend.cast(self.backend.matrices.I(n), dtype=self.matrix.dtype)
 
     def __add__(self, o):
         if isinstance(o, self.__class__):
             if self.nqubits != o.nqubits:
-                raise_error(RuntimeError, "Only hamiltonians with the same "
-                                          "number of qubits can be added.")
+                raise_error(
+                    RuntimeError,
+                    "Only hamiltonians with the same " "number of qubits can be added.",
+                )
             new_matrix = self.matrix + o.matrix
         elif isinstance(o, self.backend.numeric_types):
             new_matrix = self.matrix + o * self.eye()
         else:
-            raise_error(NotImplementedError, "Hamiltonian addition to {} not "
-                                             "implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian addition to {} not " "implemented.".format(type(o)),
+            )
         return self.__class__(self.nqubits, new_matrix, backend=self.backend)
 
     def __sub__(self, o):
         if isinstance(o, self.__class__):
             if self.nqubits != o.nqubits:
-                raise_error(RuntimeError, "Only hamiltonians with the same "
-                                          "number of qubits can be subtracted.")
+                raise_error(
+                    RuntimeError,
+                    "Only hamiltonians with the same "
+                    "number of qubits can be subtracted.",
+                )
             new_matrix = self.matrix - o.matrix
         elif isinstance(o, self.backend.numeric_types):
             new_matrix = self.matrix - o * self.eye()
         else:
-            raise_error(NotImplementedError, "Hamiltonian subtraction to {} "
-                                             "not implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian subtraction to {} " "not implemented.".format(type(o)),
+            )
         return self.__class__(self.nqubits, new_matrix, backend=self.backend)
 
     def __rsub__(self, o):
-        if isinstance(o, self.__class__): # pragma: no cover
+        if isinstance(o, self.__class__):  # pragma: no cover
             # impractical case because it will be handled by `__sub__`
             if self.nqubits != o.nqubits:
-                raise_error(RuntimeError, "Only hamiltonians with the same "
-                                          "number of qubits can be added.")
+                raise_error(
+                    RuntimeError,
+                    "Only hamiltonians with the same " "number of qubits can be added.",
+                )
             new_matrix = o.matrix - self.matrix
         elif isinstance(o, self.backend.numeric_types):
             new_matrix = o * self.eye() - self.matrix
         else:
-            raise_error(NotImplementedError, "Hamiltonian subtraction to {} "
-                                             "not implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian subtraction to {} " "not implemented.".format(type(o)),
+            )
         return self.__class__(self.nqubits, new_matrix, backend=self.backend)
 
     def __mul__(self, o):
         if isinstance(o, self.backend.tensor_types):
             o = complex(o)
         elif not isinstance(o, self.backend.numeric_types):
-            raise_error(NotImplementedError, "Hamiltonian multiplication to {} "
-                                             "not implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian multiplication to {} " "not implemented.".format(type(o)),
+            )
         new_matrix = self.matrix * o
         r = self.__class__(self.nqubits, new_matrix, backend=self.backend)
         if self._eigenvalues is not None:
-            if self.backend.np.real(o) >= 0: # TODO: check for side effects K.qnp
+            if self.backend.np.real(o) >= 0:  # TODO: check for side effects K.qnp
                 r._eigenvalues = o * self._eigenvalues
             elif not self.backend.issparse(self.matrix):
                 r._eigenvalues = o * self._eigenvalues[::-1]
         if self._eigenvectors is not None:
-            if self.backend.np.real(o) > 0: # TODO: see above
+            if self.backend.np.real(o) > 0:  # TODO: see above
                 r._eigenvectors = self._eigenvectors
             elif o == 0:
                 r._eigenvectors = self.eye(int(self._eigenvectors.shape[0]))
         return r
 
     def __matmul__(self, o):
         if isinstance(o, self.__class__):
-            matrix = self.backend.calculate_hamiltonian_matrix_product(self.matrix, o.matrix)
+            matrix = self.backend.calculate_hamiltonian_matrix_product(
+                self.matrix, o.matrix
+            )
             return self.__class__(self.nqubits, matrix, backend=self.backend)
 
         elif isinstance(o, self.backend.tensor_types):
             return self.backend.calculate_hamiltonian_state_product(self.matrix, o)
 
         else:
-            raise_error(NotImplementedError, "Hamiltonian matmul to {} not "
-                                         "implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian matmul to {} not " "implemented.".format(type(o)),
+            )
 
 
 class TrotterCircuit:
     """Object that caches the Trotterized evolution circuit.
 
     This object holds a reference to the circuit models and updates its
     parameters if a different time step ``dt`` is given without recreating
@@ -200,27 +264,31 @@
         dt (float): Time step for the Trotterization.
         nqubits (int): Number of qubits in the system that evolves.
         accelerators (dict): Dictionary with accelerators for distributed
             circuits.
     """
 
     def __init__(self, groups, dt, nqubits, accelerators):
-        from qibo.models import Circuit
         from itertools import chain
+
+        from qibo.models import Circuit
+
         self.gates = {}
         self.dt = dt
         self.circuit = Circuit(nqubits, accelerators=accelerators)
         for group in chain(groups, groups[::-1]):
             gate = group.term.expgate(dt / 2.0)
             self.gates[gate] = group
             self.circuit.add(gate)
 
     def set(self, dt):
         if self.dt != dt:
-            params = {gate: group.term.exp(dt / 2.0) for gate, group in self.gates.items()}
+            params = {
+                gate: group.term.exp(dt / 2.0) for gate, group in self.gates.items()
+            }
             self.dt = dt
             self.circuit.set_parameters(params)
 
 
 class SymbolicHamiltonian(AbstractHamiltonian):
     """Hamiltonian based on a symbolic representation.
 
@@ -250,35 +318,40 @@
             :meth:`qibo.hamiltonians.models.MaxCut` Hamiltonian.
     """
 
     def __init__(self, form=None, symbol_map={}, backend=None):
         super().__init__()
         self._form = None
         self._terms = None
-        self.constant = 0 # used only when we perform calculations using ``_terms``
+        self.constant = 0  # used only when we perform calculations using ``_terms``
         self._dense = None
         self.symbol_map = symbol_map
         # if a symbol in the given form is not a Qibo symbol it must be
         # included in the ``symbol_map``
         self.trotter_circuit = None
         from qibo.symbols import Symbol
-        self._qiboSymbol = Symbol # also used in ``self._get_symbol_matrix``
+
+        self._qiboSymbol = Symbol  # also used in ``self._get_symbol_matrix``
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             self.backend = GlobalBackend()
         else:
             self.backend = backend
         if form is not None:
             self.form = form
+
     @property
     def dense(self):
         """Creates the equivalent :class:`qibo.hamiltonians.MatrixHamiltonian`."""
         if self._dense is None:
-            log.warning("Calculating the dense form of a symbolic Hamiltonian. "
-                        "This operation is memory inefficient.")
+            log.warning(
+                "Calculating the dense form of a symbolic Hamiltonian. "
+                "This operation is memory inefficient."
+            )
             self.dense = self.calculate_dense()
         return self._dense
 
     @dense.setter
     def dense(self, hamiltonian):
         assert isinstance(hamiltonian, Hamiltonian)
         self._dense = hamiltonian
@@ -290,26 +363,30 @@
     def form(self):
         return self._form
 
     @form.setter
     def form(self, form):
         # Check that given form is a ``sympy`` expression
         if not isinstance(form, sympy.Expr):
-            raise_error(TypeError, "Symbolic Hamiltonian should be a ``sympy`` "
-                                   "expression but is {}.".format(type(form)))
+            raise_error(
+                TypeError,
+                "Symbolic Hamiltonian should be a ``sympy`` "
+                "expression but is {}.".format(type(form)),
+            )
         # Calculate number of qubits in the system described by the given
         # Hamiltonian formula
         nqubits = 0
         for symbol in form.free_symbols:
             if isinstance(symbol, self._qiboSymbol):
                 q = symbol.target_qubit
             elif isinstance(symbol, sympy.Expr):
                 if symbol not in self.symbol_map:
-                    raise_error(ValueError, "Symbol {} is not in symbol "
-                                            "map.".format(symbol))
+                    raise_error(
+                        ValueError, "Symbol {} is not in symbol " "map.".format(symbol)
+                    )
                 q, matrix = self.symbol_map.get(symbol)
                 if not isinstance(matrix, self.backend.tensor_types):
                     # ignore symbols that do not correspond to quantum operators
                     # for example parameters in the MaxCut Hamiltonian
                     q = 0
             if q > nqubits:
                 nqubits = q
@@ -319,23 +396,26 @@
 
     @property
     def terms(self):
         """List of :class:`qibo.core.terms.HamiltonianTerm` objects of which the Hamiltonian is a sum of."""
         if self._terms is None:
             # Calculate terms based on ``self.form``
             from qibo.hamiltonians.terms import SymbolicTerm
+
             form = sympy.expand(self.form)
             terms = []
             for f, c in form.as_coefficients_dict().items():
                 term = SymbolicTerm(c, f, self.symbol_map)
                 if term.target_qubits:
                     terms.append(term)
                 else:
                     self.constant += term.coefficient
-            assert self.nqubits == max(q for term in terms for q in term.target_qubits) + 1
+            assert (
+                self.nqubits == max(q for term in terms for q in term.target_qubits) + 1
+            )
             self._terms = terms
         return self._terms
 
     @terms.setter
     def terms(self, terms):
         self._terms = terms
         self.nqubits = max(q for term in self._terms for q in term.target_qubits) + 1
@@ -371,18 +451,20 @@
             term (sympy.Expr): Symbolic expression containing local operators.
 
         Returns:
             Numerical matrix corresponding to the given expression as a numpy
             array of size ``(2 ** self.nqubits, 2 ** self.nqubits).
         """
         from numpy import eye
+
         if isinstance(term, sympy.Add):
             # symbolic op for addition
-            result = sum(self._get_symbol_matrix(subterm)
-                         for subterm in term.as_ordered_terms())
+            result = sum(
+                self._get_symbol_matrix(subterm) for subterm in term.as_ordered_terms()
+            )
 
         elif isinstance(term, sympy.Mul):
             # symbolic op for multiplication
             # note that we need to use matrix multiplication even though
             # we use scalar symbols for convenience
             factors = term.as_ordered_factors()
             result = self._get_symbol_matrix(factors[0])
@@ -406,150 +488,218 @@
                 # implemented in :meth:`qibo.core.terms.SymbolicTerm.full_matrix`.
                 result = term.full_matrix(self.nqubits)
             else:
                 q, matrix = self.symbol_map.get(term)
                 if not isinstance(matrix, self.backend.tensor_types):
                     # symbols that do not correspond to quantum operators
                     # for example parameters in the MaxCut Hamiltonian
-                    result = complex(matrix) * eye(2 ** self.nqubits)
+                    result = complex(matrix) * eye(2**self.nqubits)
                 else:
                     # if we do not have a Qibo symbol we construct one and use
                     # :meth:`qibo.core.terms.SymbolicTerm.full_matrix`.
                     result = self._qiboSymbol(q, matrix).full_matrix(self.nqubits)
 
         elif term.is_number:
             # if the term is number we should return in the form of identity
             # matrix because in expressions like `1 + Z`, `1` is not correspond
             # to the float 1 but the identity operator (matrix)
-            result = complex(term) * eye(2 ** self.nqubits)
+            result = complex(term) * eye(2**self.nqubits)
 
         else:
-            raise_error(TypeError, "Cannot calculate matrix for symbolic term "
-                                   "of type {}.".format(type(term)))
+            raise_error(
+                TypeError,
+                "Cannot calculate matrix for symbolic term "
+                "of type {}.".format(type(term)),
+            )
 
         return result
 
     def _calculate_dense_from_form(self):
         """Calculates equivalent :class:`qibo.core.hamiltonians.Hamiltonian` using symbolic form.
         Useful when the term representation is not available.
         """
         matrix = self._get_symbol_matrix(self.form)
         return Hamiltonian(self.nqubits, matrix, backend=self.backend)
 
     def _calculate_dense_from_terms(self):
         """Calculates equivalent :class:`qibo.core.hamiltonians.Hamiltonian` using the term representation."""
         from itertools import chain
+
         import numpy as np
-        if 2 * self.nqubits > len(EINSUM_CHARS): # pragma: no cover
+
+        if 2 * self.nqubits > len(EINSUM_CHARS):  # pragma: no cover
             # case not tested because it only happens in large examples
             raise_error(NotImplementedError, "Not enough einsum characters.")
 
         matrix = 0
-        chars = EINSUM_CHARS[:2 * self.nqubits]
+        chars = EINSUM_CHARS[: 2 * self.nqubits]
         for term in self.terms:
             ntargets = len(term.target_qubits)
             tmat = np.reshape(term.matrix, 2 * ntargets * (2,))
             n = self.nqubits - ntargets
-            emat = np.reshape(np.eye(2 ** n, dtype=tmat.dtype), 2 * n * (2,))
+            emat = np.reshape(np.eye(2**n, dtype=tmat.dtype), 2 * n * (2,))
             gen = lambda x: (chars[i + x] for i in term.target_qubits)
             tc = "".join(chain(gen(0), gen(self.nqubits)))
-            ec = "".join((c for c in chars if c not in tc))
+            ec = "".join(c for c in chars if c not in tc)
             matrix += np.einsum(f"{tc},{ec}->{chars}", tmat, emat)
-        matrix = np.reshape(matrix, 2 * (2 ** self.nqubits,))
+        matrix = np.reshape(matrix, 2 * (2**self.nqubits,))
         return Hamiltonian(self.nqubits, matrix, backend=self.backend) + self.constant
 
     def calculate_dense(self):
         if self._terms is None:
             # calculate dense matrix directly using the form to avoid the
             # costly ``sympy.expand`` call
             return self._calculate_dense_from_form()
         return self._calculate_dense_from_terms()
 
     def expectation(self, state, normalize=False):
         return Hamiltonian.expectation(self, state, normalize)
 
+    def expectation_from_samples(self, freq, qubit_map=None):
+        import numpy as np
+
+        terms = self.terms
+        for term in terms:
+            for factor in term.factors:
+                if isinstance(factor, Z) == False:
+                    raise_error(
+                        NotImplementedError, "Observable is not a Z Pauli string."
+                    )
+            if len(term.factors) != len(set(term.factors)):
+                raise_error(NotImplementedError, "Z^k is not implemented since Z^2=I.")
+        keys = list(freq.keys())
+        counts = np.array(list(freq.values())) / sum(freq.values())
+        coeff = list(self.form.as_coefficients_dict().values())
+        qubits = []
+        for term in terms:
+            qubits_term = []
+            for k in term.target_qubits:
+                qubits_term.append(k)
+            qubits.append(qubits_term)
+        if qubit_map is None:
+            qubit_map = list(range(len(keys[0])))
+        expval = 0
+        for j, q in enumerate(qubits):
+            subk = []
+            expval_q = 0
+            for i, k in enumerate(keys):
+                subk = [int(k[qubit_map.index(s)]) for s in q]
+                expval_k = 1
+                if subk.count(1) % 2 == 1:
+                    expval_k = -1
+                expval_q += expval_k * counts[i]
+            expval += expval_q * float(coeff[j])
+        return expval
+
     def __add__(self, o):
         if isinstance(o, self.__class__):
             if self.nqubits != o.nqubits:
-                raise_error(RuntimeError, "Only hamiltonians with the same "
-                                          "number of qubits can be added.")
-            new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
+                raise_error(
+                    RuntimeError,
+                    "Only hamiltonians with the same " "number of qubits can be added.",
+                )
+            new_ham = self.__class__(
+                symbol_map=dict(self.symbol_map), backend=self.backend
+            )
             if self._form is not None and o._form is not None:
                 new_ham.form = self.form + o.form
                 new_ham.symbol_map.update(o.symbol_map)
             if self._terms is not None and o._terms is not None:
                 new_ham.terms = self.terms + o.terms
                 new_ham.constant = self.constant + o.constant
             if self._dense is not None and o._dense is not None:
                 new_ham.dense = self.dense + o.dense
 
         elif isinstance(o, self.backend.numeric_types):
-            new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
+            new_ham = self.__class__(
+                symbol_map=dict(self.symbol_map), backend=self.backend
+            )
             if self._form is not None:
                 new_ham.form = self.form + o
             if self._terms is not None:
                 new_ham.terms = self.terms
                 new_ham.constant = self.constant + o
             if self._dense is not None:
                 new_ham.dense = self.dense + o
 
         else:
-            raise_error(NotImplementedError, "SymbolicHamiltonian addition to {} not "
-                                             "implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "SymbolicHamiltonian addition to {} not "
+                "implemented.".format(type(o)),
+            )
         return new_ham
 
     def __sub__(self, o):
         if isinstance(o, self.__class__):
             if self.nqubits != o.nqubits:
-                raise_error(RuntimeError, "Only hamiltonians with the same "
-                                          "number of qubits can be subtracted.")
-            new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
+                raise_error(
+                    RuntimeError,
+                    "Only hamiltonians with the same "
+                    "number of qubits can be subtracted.",
+                )
+            new_ham = self.__class__(
+                symbol_map=dict(self.symbol_map), backend=self.backend
+            )
             if self._form is not None and o._form is not None:
                 new_ham.form = self.form - o.form
                 new_ham.symbol_map.update(o.symbol_map)
             if self._terms is not None and o._terms is not None:
                 new_ham.terms = self.terms + [-1 * x for x in o.terms]
                 new_ham.constant = self.constant - o.constant
             if self._dense is not None and o._dense is not None:
                 new_ham.dense = self.dense - o.dense
 
         elif isinstance(o, self.backend.numeric_types):
-            new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
+            new_ham = self.__class__(
+                symbol_map=dict(self.symbol_map), backend=self.backend
+            )
             if self._form is not None:
                 new_ham.form = self.form - o
             if self._terms is not None:
                 new_ham.terms = self.terms
                 new_ham.constant = self.constant - o
             if self._dense is not None:
                 new_ham.dense = self.dense - o
 
         else:
-            raise_error(NotImplementedError, "Hamiltonian subtraction to {} "
-                                             "not implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian subtraction to {} " "not implemented.".format(type(o)),
+            )
         return new_ham
 
     def __rsub__(self, o):
         if isinstance(o, self.backend.numeric_types):
-            new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
+            new_ham = self.__class__(
+                symbol_map=dict(self.symbol_map), backend=self.backend
+            )
             if self._form is not None:
                 new_ham.form = o - self.form
             if self._terms is not None:
                 new_ham.terms = [-1 * x for x in self.terms]
                 new_ham.constant = o - self.constant
             if self._dense is not None:
                 new_ham.dense = o - self.dense
         else:
-            raise_error(NotImplementedError, "Hamiltonian subtraction to {} "
-                                             "not implemented.".format(type(o)))
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian subtraction to {} " "not implemented.".format(type(o)),
+            )
         return new_ham
 
     def __mul__(self, o):
-        if not (isinstance(o, self.backend.numeric_types) or isinstance(o, self.backend.tensor_types)):
-            raise_error(NotImplementedError, "Hamiltonian multiplication to {} "
-                                             "not implemented.".format(type(o)))
+        if not (
+            isinstance(o, self.backend.numeric_types)
+            or isinstance(o, self.backend.tensor_types)
+        ):
+            raise_error(
+                NotImplementedError,
+                "Hamiltonian multiplication to {} " "not implemented.".format(type(o)),
+            )
         o = complex(o)
         new_ham = self.__class__(symbol_map=dict(self.symbol_map), backend=self.backend)
         if self._form is not None:
             new_ham.form = o * self.form
         if self._terms is not None:
             new_ham.terms = [o * x for x in self.terms]
             new_ham.constant = self.constant * o
@@ -559,63 +709,80 @@
 
     def apply_gates(self, state, density_matrix=False):
         """Applies gates corresponding to the Hamiltonian terms to a given state.
         Helper method for ``__matmul__``.
         """
         total = 0
         for term in self.terms:
-            total += term(self.backend, self.backend.cast(state, copy=True), self.nqubits, density_matrix)
+            total += term(
+                self.backend,
+                self.backend.cast(state, copy=True),
+                self.nqubits,
+                density_matrix=density_matrix,
+            )
         if self.constant:  # pragma: no cover
             total += self.constant * state
         return total
 
     def __matmul__(self, o):
         """Matrix multiplication with other Hamiltonians or state vectors."""
         if isinstance(o, self.__class__):
             if self._form is None or o._form is None:
-                raise_error(NotImplementedError, "Multiplication of symbolic Hamiltonians "
-                                                 "without symbolic form is not implemented.")
+                raise_error(
+                    NotImplementedError,
+                    "Multiplication of symbolic Hamiltonians "
+                    "without symbolic form is not implemented.",
+                )
             new_form = self.form * o.form
             new_symbol_map = dict(self.symbol_map)
             new_symbol_map.update(o.symbol_map)
-            new_ham = self.__class__(new_form, symbol_map=new_symbol_map, backend=self.backend)
+            new_ham = self.__class__(
+                new_form, symbol_map=new_symbol_map, backend=self.backend
+            )
             if self._dense is not None and o._dense is not None:
                 new_ham.dense = self.dense @ o.dense
             return new_ham
 
         if isinstance(o, self.backend.tensor_types):
             rank = len(tuple(o.shape))
-            if rank == 1: # state vector
+            if rank == 1:  # state vector
                 return self.apply_gates(o)
-            elif rank == 2: # density matrix
+            elif rank == 2:  # density matrix
                 return self.apply_gates(o, density_matrix=True)
             else:
-                raise_error(NotImplementedError, "Cannot multiply Hamiltonian with "
-                                                 "rank-{} tensor.".format(rank))
-
-        raise_error(NotImplementedError, "Hamiltonian matmul to {} not "
-                                         "implemented.".format(type(o)))
+                raise_error(
+                    NotImplementedError,
+                    "Cannot multiply Hamiltonian with " "rank-{} tensor.".format(rank),
+                )
+
+        raise_error(
+            NotImplementedError,
+            "Hamiltonian matmul to {} not " "implemented.".format(type(o)),
+        )
 
     def circuit(self, dt, accelerators=None):
         """Circuit that implements a Trotter step of this Hamiltonian for a given time step ``dt``."""
         if self.trotter_circuit is None:
             from qibo.hamiltonians.terms import TermGroup
+
             groups = TermGroup.from_terms(self.terms)
-            self.trotter_circuit = TrotterCircuit(groups, dt, self.nqubits,
-                                                  accelerators)
+            self.trotter_circuit = TrotterCircuit(
+                groups, dt, self.nqubits, accelerators
+            )
         self.trotter_circuit.set(dt)
         return self.trotter_circuit.circuit
 
 
 class TrotterHamiltonian:
     """"""
 
     def __init__(self, *parts):
-        raise_error(NotImplementedError,
-                    "`TrotterHamiltonian` is substituted by `SymbolicHamiltonian` "
-                    "and is no longer supported. Please check the documentation "
-                    "of `SymbolicHamiltonian` for more details.")
+        raise_error(
+            NotImplementedError,
+            "`TrotterHamiltonian` is substituted by `SymbolicHamiltonian` "
+            "and is no longer supported. Please check the documentation "
+            "of `SymbolicHamiltonian` for more details.",
+        )
 
     @classmethod
     def from_symbolic(cls, symbolic_hamiltonian, symbol_map):
         return cls()
-
```

### Comparing `qibo-0.1.8rc0/src/qibo/hamiltonians/models.py` & `qibo-0.1.9/src/qibo/hamiltonians/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-# -*- coding: utf-8 -*-
+from qibo.backends import matrices
 from qibo.config import raise_error
-from qibo import matrices
 from qibo.hamiltonians.hamiltonians import Hamiltonian, SymbolicHamiltonian
 from qibo.hamiltonians.terms import HamiltonianTerm
 
 
 def multikron(matrix_list):
     """Calculates Kronecker product of a list of matrices.
 
     Args:
         matrices (list): List of matrices as ``np.ndarray``s.
 
     Returns:
         ``np.ndarray`` of the Kronecker product of all ``matrices``.
     """
     import numpy as np
+
     h = 1
     for m in matrix_list:
         # TODO: check if we observe GPU deterioration
         h = np.kron(h, m)
     return h
 
 
 def _build_spin_model(nqubits, matrix, condition):
     """Helper method for building nearest-neighbor spin model Hamiltonians."""
-    h = sum(multikron(
-      (matrix if condition(i, j) else matrices.I for j in range(nqubits)))
-            for i in range(nqubits))
+    h = sum(
+        multikron(matrix if condition(i, j) else matrices.I for j in range(nqubits))
+        for i in range(nqubits)
+    )
     return h
 
 
 def XXZ(nqubits, delta=0.5, dense=True, backend=None):
     """Heisenberg XXZ model with periodic boundary conditions.
 
     .. math::
@@ -46,15 +47,15 @@
     Example:
         .. testcode::
 
             from qibo.hamiltonians import XXZ
             h = XXZ(3) # initialized XXZ model with 3 qubits
     """
     if dense:
-        condition = lambda i, j: i in {j % nqubits, (j+1) % nqubits}
+        condition = lambda i, j: i in {j % nqubits, (j + 1) % nqubits}
         hx = _build_spin_model(nqubits, matrices.X, condition)
         hy = _build_spin_model(nqubits, matrices.Y, condition)
         hz = _build_spin_model(nqubits, matrices.Z, condition)
         matrix = hx + hy + delta * hz
         return Hamiltonian(nqubits, matrix, backend=backend)
 
     hx = multikron([matrices.X, matrices.X])
@@ -71,15 +72,15 @@
 def _OneBodyPauli(nqubits, matrix, dense=True, backend=None):
     """Helper method for constracting non-interacting X, Y, Z Hamiltonians."""
     if dense:
         condition = lambda i, j: i == j % nqubits
         ham = -_build_spin_model(nqubits, matrix, condition)
         return Hamiltonian(nqubits, ham, backend=backend)
 
-    matrix = - matrix
+    matrix = -matrix
     terms = [HamiltonianTerm(matrix, i) for i in range(nqubits)]
     ham = SymbolicHamiltonian(backend=backend)
     ham.terms = terms
     return ham
 
 
 def X(nqubits, dense=True, backend=None):
@@ -137,22 +138,24 @@
         nqubits (int): number of quantum bits.
         h (float): value of the transverse field.
         dense (bool): If ``True`` it creates the Hamiltonian as a
             :class:`qibo.core.hamiltonians.Hamiltonian`, otherwise it creates
             a :class:`qibo.core.hamiltonians.SymbolicHamiltonian`.
     """
     if dense:
-        condition = lambda i, j: i in {j % nqubits, (j+1) % nqubits}
+        condition = lambda i, j: i in {j % nqubits, (j + 1) % nqubits}
         ham = -_build_spin_model(nqubits, matrices.Z, condition)
         if h != 0:
             condition = lambda i, j: i == j % nqubits
             ham -= h * _build_spin_model(nqubits, matrices.X, condition)
         return Hamiltonian(nqubits, ham, backend=backend)
 
-    matrix = -(multikron([matrices.Z, matrices.Z]) + h * multikron([matrices.X, matrices.I]))
+    matrix = -(
+        multikron([matrices.Z, matrices.Z]) + h * multikron([matrices.X, matrices.I])
+    )
     terms = [HamiltonianTerm(matrix, i, i + 1) for i in range(nqubits - 1)]
     terms.append(HamiltonianTerm(matrix, nqubits - 1, 0))
     ham = SymbolicHamiltonian(backend=backend)
     ham.terms = terms
     return ham
 
 
@@ -167,17 +170,21 @@
         dense (bool): If ``True`` it creates the Hamiltonian as a
             :class:`qibo.core.hamiltonians.Hamiltonian`, otherwise it creates
             a :class:`qibo.core.hamiltonians.SymbolicHamiltonian`.
     """
     import sympy as sp
     from numpy import ones
 
-    Z = sp.symbols(f'Z:{nqubits}')
-    V = sp.symbols(f'V:{nqubits**2}')
-    sham = - sum(V[i * nqubits + j] * (1 - Z[i] * Z[j]) for i in range(nqubits) for j in range(nqubits))
+    Z = sp.symbols(f"Z:{nqubits}")
+    V = sp.symbols(f"V:{nqubits**2}")
+    sham = -sum(
+        V[i * nqubits + j] * (1 - Z[i] * Z[j])
+        for i in range(nqubits)
+        for j in range(nqubits)
+    )
     sham /= 2
 
     v = ones(nqubits**2)
     smap = {s: (i, matrices.Z) for i, s in enumerate(Z)}
     smap.update({s: (i, v[i]) for i, s in enumerate(V)})
 
     ham = SymbolicHamiltonian(sham, smap, backend=backend)
```

### Comparing `qibo-0.1.8rc0/src/qibo/hamiltonians/terms.py` & `qibo-0.1.9/src/qibo/hamiltonians/terms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-import sympy
 import numpy as np
+import sympy
+
 from qibo import gates
 from qibo.config import raise_error
 
+
 class HamiltonianTerm:
     """Term of a :class:`qibo.hamiltonians.hamiltonians.SymbolicHamiltonian`.
 
     Symbolic Hamiltonians are represented by a list of
     :class:`qibo.hamiltonians.terms.HamiltonianTerm` objects storred in the
     ``SymbolicHamiltonian.terms`` attribute. The mathematical expression of
     the Hamiltonian is the sum of these terms.
@@ -17,25 +19,32 @@
             number of target qubits of this term.
         q (list): List of target qubit ids.
     """
 
     def __init__(self, matrix, *q):
         for qi in q:
             if qi < 0:
-                raise_error(ValueError, "Invalid qubit id {} < 0 was given "
-                                        "in Hamiltonian term".format(qi))
+                raise_error(
+                    ValueError,
+                    "Invalid qubit id {} < 0 was given "
+                    "in Hamiltonian term".format(qi),
+                )
         if not isinstance(matrix, np.ndarray):
-            raise_error(TypeError, "Invalid type {} of symbol matrix."
-                                   "".format(type(matrix)))
+            raise_error(
+                TypeError, "Invalid type {} of symbol matrix." "".format(type(matrix))
+            )
         dim = int(matrix.shape[0])
         if 2 ** len(q) != dim:
-            raise_error(ValueError, "Matrix dimension {} given in Hamiltonian "
-                                    "term is not compatible with the number "
-                                    "of target qubits {}."
-                                    "".format(dim, len(q)))
+            raise_error(
+                ValueError,
+                "Matrix dimension {} given in Hamiltonian "
+                "term is not compatible with the number "
+                "of target qubits {}."
+                "".format(dim, len(q)),
+            )
         self.target_qubits = tuple(q)
         self._gate = None
         self.hamiltonian = None
         self._matrix = matrix
 
     @property
     def matrix(self):
@@ -48,31 +57,35 @@
         if self._gate is None:
             self._gate = gates.Unitary(self.matrix, *self.target_qubits)
         return self._gate
 
     def exp(self, x):
         """Matrix exponentiation of the term."""
         from scipy.linalg import expm
+
         return expm(-1j * x * self.matrix)
 
     def expgate(self, x):
         """:class:`qibo.gates.gates.Unitary` gate implementing the action of exp(term) on states."""
         return gates.Unitary(self.exp(x), *self.target_qubits)
 
     def merge(self, term):
         """Creates a new term by merging the given term to the current one.
 
         The resulting term corresponds to the sum of the two original terms.
         The target qubits of the given term should be a subset of the target
         qubits of the current term.
         """
         if not set(term.target_qubits).issubset(set(self.target_qubits)):
-            raise_error(ValueError, "Cannot merge HamiltonianTerm acting on "
-                                    "qubits {} to term on qubits {}."
-                                    "".format(term.target_qubits, self.target_qubits))
+            raise_error(
+                ValueError,
+                "Cannot merge HamiltonianTerm acting on "
+                "qubits {} to term on qubits {}."
+                "".format(term.target_qubits, self.target_qubits),
+            )
         matrix = np.kron(term.matrix, np.eye(2 ** (len(self) - len(term))))
         matrix = np.reshape(matrix, 2 * len(self) * (2,))
         order = []
         i = len(term)
         for qubit in self.target_qubits:
             if qubit in term.target_qubits:
                 order.append(term.target_qubits.index(qubit))
@@ -91,20 +104,20 @@
         return HamiltonianTerm(x * self.matrix, *self.target_qubits)
 
     def __rmul__(self, x):
         return self.__mul__(x)
 
     def __call__(self, backend, state, nqubits, gate=None, density_matrix=False):
         """Applies the term on a given state vector or density matrix."""
-        #TODO: improve this and understand why it works
+        # TODO: improve this and understand why it works
         if isinstance(gate, bool) or gate is None:
             gate = self.gate
         if density_matrix:
             return backend.apply_gate_half_density_matrix(gate, state, nqubits)
-        return backend.apply_gate(gate, state, nqubits) # pylint: disable=E1102
+        return backend.apply_gate(gate, state, nqubits)  # pylint: disable=E1102
 
 
 class SymbolicTerm(HamiltonianTerm):
     """:class:`qibo.hamiltonians.terms.HamiltonianTerm` constructed using ``sympy`` expression.
 
     Example:
         .. testcode::
@@ -148,14 +161,15 @@
                 else:
                     pow = 1
 
                 # if the user is using ``symbol_map`` instead of qibo symbols,
                 # create the corresponding symbols
                 if factor in symbol_map:
                     from qibo.symbols import Symbol
+
                     q, matrix = symbol_map.get(factor)
                     factor = Symbol(q, matrix, name=factor.name)
 
                 if isinstance(factor, sympy.Symbol):
                     if isinstance(factor.matrix, np.ndarray):
                         self.factors.extend(pow * [factor])
                         q = factor.target_qubit
@@ -171,29 +185,30 @@
                             self.matrix_map[q] = pow * [factor.matrix]
                     else:
                         self.coefficient *= factor.matrix
                 elif factor == sympy.I:
                     self.coefficient *= 1j
                 elif factor.is_number:
                     self.coefficient *= complex(factor)
-                else: # pragma: no cover
+                else:  # pragma: no cover
                     raise_error(TypeError, "Cannot parse factor {}.".format(factor))
 
         self.target_qubits = tuple(sorted(self.matrix_map.keys()))
 
     @property
     def matrix(self):
         """Calculates the full matrix corresponding to this term.
 
         Returns:
             Matrix as a ``np.ndarray`` of shape ``(2 ** ntargets, 2 ** ntargets)``
             where ``ntargets`` is the number of qubits included in the factors
             of this term.
         """
         if self._matrix is None:
+
             def matrices_product(matrices):
                 """Product of matrices that act on the same tuple of qubits.
 
                 Args:
                     matrices (list): List of matrices to multiply, as exists in
                         the values of ``SymbolicTerm.matrix_map``.
                 """
@@ -224,15 +239,17 @@
         new.coefficient *= x
         if self._matrix is not None:
             new._matrix = x * self._matrix
         return new
 
     def __call__(self, backend, state, nqubits, density_matrix=False):
         for factor in self.factors:
-            state = super().__call__(backend, state, nqubits, factor.gate, density_matrix)
+            state = super().__call__(
+                backend, state, nqubits, factor.gate, density_matrix
+            )
         return self.coefficient * state
 
 
 class TermGroup(list):
     """Collection of multiple :class:`qibo.hamiltonians.terms.HamiltonianTerm` objects.
 
     Allows merging multiple terms to a single one for faster exponentiation
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/circuit.py` & `qibo-0.1.9/src/qibo/models/circuit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import collections
+from typing import Dict, List, Tuple, Union
+
 import numpy as np
+
 from qibo import gates
 from qibo import gates as gate_module
 from qibo.config import raise_error
-from typing import Dict, List, Tuple, Union
-NoiseMapType = Union[Tuple[int, int, int],
-                     Dict[int, Tuple[int, int, int]]]
+
+NoiseMapType = Union[Tuple[int, int, int], Dict[int, Tuple[int, int, int]]]
 
 
 class _ParametrizedGates(list):
     """Simple data structure for keeping track of parametrized gates.
 
     Useful for the ``circuit.set_parameters()`` method.
     Holds parametrized gates in a list and a set and also keeps track of the
@@ -31,15 +33,15 @@
     """List that holds the queue of gates of a circuit.
 
     In addition to the queue, it holds a list of gate moments, where each gate
     is placed in the earliest possible position depending for the qubits it acts.
     """
 
     def __init__(self, nqubits):
-        super(_Queue, self).__init__(self)
+        super().__init__(self)
         self.nqubits = nqubits
         self.moments = [nqubits * [None]]
         self.moment_index = nqubits * [0]
 
     def to_fused(self):
         """Transforms all gates in queue to :class:`qibo.gates.FusedGate`."""
         last_gate = {}
@@ -69,18 +71,18 @@
             elif not gate.qubits:
                 # special gates are marked by default so we need
                 # to add them manually
                 queue.append(gate.gates[0])
         return queue
 
     def append(self, gate: gates.Gate):
-        super(_Queue, self).append(gate)
+        super().append(gate)
         if gate.qubits:
             qubits = gate.qubits
-        else: # special gate acting on all qubits
+        else:  # special gate acting on all qubits
             qubits = tuple(range(self.nqubits))
 
         # calculate moment index for this gate
         idx = max(self.moment_index[q] for q in qubits)
         for q in qubits:
             if idx >= len(self.moments):
                 # Add a moment
@@ -97,22 +99,29 @@
 
     Args:
         nqubits (int): Total number of qubits in the circuit.
     """
 
     def __init__(self, nqubits, accelerators=None, density_matrix=False):
         if not isinstance(nqubits, int):
-            raise_error(TypeError, "Number of qubits must be an integer but "
-                                   "is {}.".format(nqubits))
+            raise_error(
+                TypeError,
+                "Number of qubits must be an integer but " "is {}.".format(nqubits),
+            )
         if nqubits < 1:
-            raise_error(ValueError, "Number of qubits must be positive but is "
-                                    "{}.".format(nqubits))
+            raise_error(
+                ValueError,
+                "Number of qubits must be positive but is " "{}.".format(nqubits),
+            )
         self.nqubits = nqubits
-        self.init_kwargs = {"nqubits": nqubits, "accelerators": accelerators,
-                            "density_matrix": density_matrix}
+        self.init_kwargs = {
+            "nqubits": nqubits,
+            "accelerators": accelerators,
+            "density_matrix": density_matrix,
+        }
         self.queue = _Queue(nqubits)
         # Keep track of parametrized gates for the ``set_parameters`` method
         self.parametrized_gates = _ParametrizedGates()
         self.trainable_gates = _ParametrizedGates()
 
         self.measurement_tuples = dict()
         self.measurement_gate = None
@@ -129,16 +138,18 @@
         self.ndevices = None
         self.nglobal = None
         self.nglobal = None
         self.nlocal = None
         self.queues = None
         if accelerators:  # pragma: no cover
             if density_matrix:
-                raise_error(NotImplementedError, "Distributed circuit is not implemented "
-                                                 "for density matrices.")
+                raise_error(
+                    NotImplementedError,
+                    "Distributed circuit is not implemented " "for density matrices.",
+                )
             self._distributed_init(nqubits, accelerators)
 
     def _distributed_init(self, nqubits, accelerators):  # pragma: no cover
         """Distributed implementation of :class:`qibo.models.circuit.Circuit`.
 
         Uses multiple `accelerator` devices (GPUs) for applying gates to the state vector.
         The full state vector is saved in the given `memory device` (usually the CPU)
@@ -167,38 +178,44 @@
             accelerators (dict): Dictionary that maps device names to the number of
                 times each device will be used.
                 The total number of logical devices must be a power of 2.
         """
         self.ndevices = sum(accelerators.values())
         self.nglobal = float(np.log2(self.ndevices))
         if not (self.nglobal.is_integer() and self.nglobal > 0):
-            raise_error(ValueError, "Number of calculation devices should be a power "
-                                    "of 2 but is {}.".format(self.ndevices))
+            raise_error(
+                ValueError,
+                "Number of calculation devices should be a power "
+                "of 2 but is {}.".format(self.ndevices),
+            )
         self.nglobal = int(self.nglobal)
         self.nlocal = self.nqubits - self.nglobal
 
         from qibo.models.distcircuit import DistributedQueues
+
         self.queues = DistributedQueues(self)
 
     def __add__(self, circuit):
         """Add circuits.
 
         Args:
             circuit: Circuit to be added to the current one.
 
         Returns:
             The resulting circuit from the addition.
         """
         for k, kwarg1 in self.init_kwargs.items():
             kwarg2 = circuit.init_kwargs[k]
             if kwarg1 != kwarg2:
-                raise_error(ValueError,
-                            "Cannot add circuits with different kwargs. "
-                            "{} is {} for first circuit and {} for the "
-                            "second.".format(k, kwarg1, kwarg2))
+                raise_error(
+                    ValueError,
+                    "Cannot add circuits with different kwargs. "
+                    "{} is {} for first circuit and {} for the "
+                    "second.".format(k, kwarg1, kwarg2),
+                )
 
         newcircuit = self.__class__(**self.init_kwargs)
         # Add gates from `self` to `newcircuit` (including measurements)
         for gate in self.queue:
             newcircuit.queue.append(gate)
             if isinstance(gate, gates.ParametrizedGate):
                 newcircuit.parametrized_gates.append(gate)
@@ -217,22 +234,26 @@
 
         if newcircuit.measurement_gate is None:
             newcircuit.measurement_gate = circuit.measurement_gate
             newcircuit.measurement_tuples = circuit.measurement_tuples
         elif circuit.measurement_gate is not None:
             for k, v in circuit.measurement_tuples.items():
                 if k in newcircuit.measurement_tuples:
-                    raise_error(KeyError, "Register name {} already exists in "
-                                          "circuit.".format(k))
+                    raise_error(
+                        KeyError,
+                        "Register name {} already exists in " "circuit.".format(k),
+                    )
                 newcircuit.check_measured(v)
                 newcircuit.measurement_tuples[k] = v
             newcircuit.measurement_gate.add(circuit.measurement_gate)
 
         # Re-execute full circuit when sampling if one of the circuit has repeated_execution True
-        newcircuit.repeated_execution = self.repeated_execution or circuit.repeated_execution
+        newcircuit.repeated_execution = (
+            self.repeated_execution or circuit.repeated_execution
+        )
 
         return newcircuit
 
     def on_qubits(self, *qubits):
         """Generator of gates contained in the circuit acting on specified qubits.
 
         Useful for adding a circuit as a subroutine in a larger circuit.
@@ -252,20 +273,26 @@
                 # create large circuit on 8 qubits
                 largec = models.Circuit(8)
                 largec.add((gates.RY(i, theta=0.1) for i in range(8)))
                 # add the small circuit to the even qubits of the large one
                 largec.add(smallc.on_qubits(*range(0, 8, 2)))
         """
         if len(qubits) != self.nqubits:
-            raise_error(ValueError, "Cannot return gates on {} qubits because "
-                                    "the circuit contains {} qubits."
-                                    "".format(len(qubits), self.nqubits))
+            raise_error(
+                ValueError,
+                "Cannot return gates on {} qubits because "
+                "the circuit contains {} qubits."
+                "".format(len(qubits), self.nqubits),
+            )
         if self.accelerators and self.queues.queues:  # pragma: no cover
-            raise_error(RuntimeError, "Cannot use distributed circuit as a "
-                                      "subroutine after it was executed.")
+            raise_error(
+                RuntimeError,
+                "Cannot use distributed circuit as a "
+                "subroutine after it was executed.",
+            )
 
         qubit_map = {i: q for i, q in enumerate(qubits)}
         for gate in self.queue:
             yield gate.on_qubits(qubit_map)
 
     def light_cone(self, *qubits):
         """Reduces circuit to the qubits relevant for an observable.
@@ -323,34 +350,40 @@
                 for the new circuit. If ``False``, the same gate objects of
                 ``circuit`` will be used.
 
         Returns:
             The copied circuit object.
         """
         import copy
+
         if deep:
             new_circuit = self.__class__(**self.init_kwargs)
             for gate in self.queue:
-                if isinstance(gate, gates.FusedGate): # pragma: no cover
+                if isinstance(gate, gates.FusedGate):  # pragma: no cover
                     # impractical case
-                    raise_error(NotImplementedError, "Cannot create deep copy "
-                                                     "of fused circuit.")
+                    raise_error(
+                        NotImplementedError,
+                        "Cannot create deep copy " "of fused circuit.",
+                    )
 
                 new_gate = copy.copy(gate)
                 new_circuit.queue.append(new_gate)
                 if isinstance(gate, gates.ParametrizedGate):
                     new_circuit.parametrized_gates.append(new_gate)
                     if gate.trainable:
                         new_circuit.trainable_gates.append(new_gate)
             new_circuit.measurement_gate = copy.copy(self.measurement_gate)
             new_circuit.measurement_tuples = dict(self.measurement_tuples)
         else:
             if self.accelerators:  # pragma: no cover
-                raise_error(ValueError, "Non-deep copy is not allowed for distributed "
-                                    "circuits because they modify gate objects.")
+                raise_error(
+                    ValueError,
+                    "Non-deep copy is not allowed for distributed "
+                    "circuits because they modify gate objects.",
+                )
             new_circuit = self._shallow_copy()
             new_circuit.queue = copy.copy(self.queue)
         return new_circuit
 
     def invert(self):
         """Creates a new ``Circuit`` that is the inverse of the original.
 
@@ -358,39 +391,51 @@
         If the original circuit contains measurement gates, these are included
         in the inverted circuit.
 
         Returns:
             The circuit inverse.
         """
         import copy
+
         new_circuit = self.__class__(**self.init_kwargs)
         for gate in self.queue[::-1]:
             new_circuit.add(gate.dagger())
         new_circuit.measurement_gate = copy.copy(self.measurement_gate)
         new_circuit.measurement_tuples = dict(self.measurement_tuples)
         return new_circuit
 
     def _check_noise_map(self, noise_map: NoiseMapType) -> NoiseMapType:
         if isinstance(noise_map, (tuple, list)):
             if len(noise_map) != 3:
-                raise_error(ValueError, "Noise map expects three probabilities "
-                                        "but received {}.".format(len(noise_map)))
+                raise_error(
+                    ValueError,
+                    "Noise map expects three probabilities "
+                    "but received {}.".format(len(noise_map)),
+                )
             return {q: noise_map for q in range(self.nqubits)}
         elif isinstance(noise_map, dict):
             if len(noise_map) != self.nqubits:
-                raise_error(ValueError, "Noise map has {} qubits while the circuit "
-                                        "has {}.".format(len(noise_map), self.nqubits))
+                raise_error(
+                    ValueError,
+                    "Noise map has {} qubits while the circuit "
+                    "has {}.".format(len(noise_map), self.nqubits),
+                )
             for v in noise_map.values():
                 if len(v) != 3:
-                    raise_error(ValueError, "Noise map expects three probabilities "
-                                            "but received {}.".format(v))
+                    raise_error(
+                        ValueError,
+                        "Noise map expects three probabilities "
+                        "but received {}.".format(v),
+                    )
             return noise_map
 
-        raise_error(TypeError, "Type {} of noise map is not recognized."
-                               "".format(type(noise_map)))
+        raise_error(
+            TypeError,
+            "Type {} of noise map is not recognized." "".format(type(noise_map)),
+        )
 
     def decompose(self, *free: int):
         """Decomposes circuit's gates to gates supported by OpenQASM.
 
         Args:
             free: Ids of free (work) qubits to use for gate decomposition.
 
@@ -445,31 +490,37 @@
                 c2.add(gates.H(1))
                 c2.add(gates.PauliNoiseChannel(1, 0.0, 0.2, 0.1))
                 c2.add(gates.CNOT(0, 1))
                 c2.add(gates.PauliNoiseChannel(0, 0.1, 0.0, 0.2))
                 c2.add(gates.PauliNoiseChannel(1, 0.0, 0.2, 0.1))
         """
         if self.accelerators:  # pragma: no cover
-            raise_error(NotImplementedError, "Distributed circuit does not support "
-                                         "density matrices yet.")
+            raise_error(
+                NotImplementedError,
+                "Distributed circuit does not support " "density matrices yet.",
+            )
 
         noise_map = self._check_noise_map(noise_map)
         # Generate noise gates
         noise_gates = []
         for gate in self.queue:
             if isinstance(gate, gates.KrausChannel):
-                raise_error(ValueError, "`.with_noise` method is not available "
-                                        "for circuits that already contain "
-                                        "channels.")
+                raise_error(
+                    ValueError,
+                    "`.with_noise` method is not available "
+                    "for circuits that already contain "
+                    "channels.",
+                )
             noise_gates.append([])
             for q in gate.qubits:
                 if q in noise_map and sum(noise_map[q]) > 0:
                     p = noise_map[q]
-                    noise_gates[-1].append(gate_module.PauliNoiseChannel(
-                            q, px=p[0], py=p[1], pz=p[2]))
+                    noise_gates[-1].append(
+                        gate_module.PauliNoiseChannel(q, px=p[0], py=p[1], pz=p[2])
+                    )
 
         # Create new circuit with noise gates inside
         noisy_circuit = self.__class__(**self.init_kwargs)
         for i, gate in enumerate(self.queue):
             noisy_circuit.add(gate)
             for noise_gate in noise_gates[i]:
                 noisy_circuit.add(noise_gate)
@@ -481,18 +532,23 @@
         """Helper method for `add`.
 
         Checks if the qubits that a gate acts are already measured and raises
         a `NotImplementedError` if they are because currently we do not allow
         measured qubits to be reused.
         """
         for qubit in gate_qubits:
-            if (self.measurement_gate is not None and
-                qubit in self.measurement_gate.target_qubits):
-                raise_error(ValueError, "Cannot reuse qubit {} because it is already "
-                                        "measured".format(qubit))
+            if (
+                self.measurement_gate is not None
+                and qubit in self.measurement_gate.target_qubits
+            ):
+                raise_error(
+                    ValueError,
+                    "Cannot reuse qubit {} because it is already "
+                    "measured".format(qubit),
+                )
 
     def add(self, gate):
         """Add a gate to a given queue.
 
         Args:
             gate (:class:`qibo.gates.Gate`): the gate object to add.
                 See :ref:`Gates` for a list of available gates.
@@ -507,33 +563,45 @@
         if isinstance(gate, collections.abc.Iterable):
             for g in gate:
                 self.add(g)
 
         else:
             if self.accelerators:  # pragma: no cover
                 if isinstance(gate, gates.KrausChannel):
-                    raise_error(NotImplementedError, "Distributed circuits do not "
-                                                    "support channels.")
-                elif self.nqubits - len(gate.target_qubits) < self.nglobal and not isinstance(gate, gates.M):
+                    raise_error(
+                        NotImplementedError,
+                        "Distributed circuits do not " "support channels.",
+                    )
+                elif self.nqubits - len(
+                    gate.target_qubits
+                ) < self.nglobal and not isinstance(gate, gates.M):
                     # Check if there is sufficient number of local qubits
-                    raise_error(ValueError, "Insufficient qubits to use for global in "
-                                            "distributed circuit.")
+                    raise_error(
+                        ValueError,
+                        "Insufficient qubits to use for global in "
+                        "distributed circuit.",
+                    )
 
             if not isinstance(gate, gates.Gate):
                 raise_error(TypeError, "Unknown gate type {}.".format(type(gate)))
 
             if self._final_state is not None:
-                raise_error(RuntimeError, "Cannot add gates to a circuit after it is "
-                                          "executed.")
+                raise_error(
+                    RuntimeError,
+                    "Cannot add gates to a circuit after it is " "executed.",
+                )
 
             for q in gate.target_qubits:
                 if q >= self.nqubits:
-                    raise_error(ValueError, "Attempting to add gate with target qubits {} "
-                                            "on a circuit of {} qubits."
-                                            "".format(gate.target_qubits, self.nqubits))
+                    raise_error(
+                        ValueError,
+                        "Attempting to add gate with target qubits {} "
+                        "on a circuit of {} qubits."
+                        "".format(gate.target_qubits, self.nqubits),
+                    )
 
             self.check_measured(gate.qubits)
             if isinstance(gate, gates.M) and not gate.collapse:
                 return self._add_measurement(gate)
             else:
                 return self._add_gate(gate)
 
@@ -558,16 +626,17 @@
         """
         # Set register's name and log the set of qubits in `self.measurement_tuples`
         name = gate.register_name
         if name is None:
             name = "register{}".format(len(self.measurement_tuples))
             gate.register_name = name
         elif name in self.measurement_tuples:
-            raise_error(KeyError, "Register name {} has already been used."
-                                  "".format(name))
+            raise_error(
+                KeyError, "Register name {} has already been used." "".format(name)
+            )
 
         # Update circuit's global measurement gate
         if self.measurement_gate is None:
             self.measurement_gate = gate
             self.measurement_tuples[name] = tuple(gate.target_qubits)
         else:
             self.measurement_gate.add(gate)
@@ -602,19 +671,17 @@
 
         Returns:
             List with all gates that are in the circuit and have the same type
             with the given ``gate``. The list contains tuples ``(i, g)`` where
             ``i`` is the index of the gate ``g`` in the circuit's gate queue.
         """
         if isinstance(gate, str):
-            return [(i, g) for i, g in enumerate(self.queue)
-                    if g.name == gate]
+            return [(i, g) for i, g in enumerate(self.queue) if g.name == gate]
         if isinstance(gate, type) and issubclass(gate, gates.Gate):
-            return [(i, g) for i, g in enumerate(self.queue)
-                    if isinstance(g, gate)]
+            return [(i, g) for i, g in enumerate(self.queue) if isinstance(g, gate)]
         raise_error(TypeError, "Gate identifier {} not recognized.".format(gate))
 
     def _set_parameters_list(self, parameters, n):
         """Helper method for ``set_parameters`` when a list is given.
 
         Also works if ``parameters`` is ``np.ndarray`` or ``tf.Tensor``.
         """
@@ -624,20 +691,23 @@
         elif n == self.trainable_gates.nparams:
             parameters = list(parameters)
             k = 0
             for i, gate in enumerate(self.trainable_gates):
                 if gate.nparams == 1:
                     gate.parameters = parameters[i + k]
                 else:
-                    gate.parameters = parameters[i + k: i + k + gate.nparams]
+                    gate.parameters = parameters[i + k : i + k + gate.nparams]
                 k += gate.nparams - 1
         else:
-            raise_error(ValueError, "Given list of parameters has length {} while "
-                                    "the circuit contains {} parametrized gates."
-                                    "".format(n, len(self.trainable_gates)))
+            raise_error(
+                ValueError,
+                "Given list of parameters has length {} while "
+                "the circuit contains {} parametrized gates."
+                "".format(n, len(self.trainable_gates)),
+            )
 
     def set_parameters(self, parameters):
         """Updates the parameters of the circuit's parametrized gates.
 
         For more information on how to use this method we refer to the
         :ref:`How to use parametrized gates?<params-examples>` example.
 
@@ -676,35 +746,42 @@
                           c.queue[3]: (0.789, 0.321)}
                 c.set_parameters(params)
                 # or using flat list (or an equivalent `np.array`/`tf.Tensor`)
                 params = [0.123, 0.456, 0.789, 0.321]
                 c.set_parameters(params)
         """
         from collections.abc import Iterable
+
         if isinstance(parameters, dict):
             diff = set(parameters.keys()) - self.trainable_gates.set
             if diff:
-                raise_error(KeyError, "Dictionary contains gates {} which are "
-                                      "not on the list of parametrized gates "
-                                      "of the circuit.".format(diff))
+                raise_error(
+                    KeyError,
+                    "Dictionary contains gates {} which are "
+                    "not on the list of parametrized gates "
+                    "of the circuit.".format(diff),
+                )
             for gate, params in parameters.items():
                 gate.parameters = params
-        elif isinstance(parameters, Iterable) and not isinstance(parameters, (set, str)):
+        elif isinstance(parameters, Iterable) and not isinstance(
+            parameters, (set, str)
+        ):
             try:
                 nparams = int(parameters.shape[0])
             except AttributeError:
                 nparams = len(parameters)
             self._set_parameters_list(parameters, nparams)
         else:
-            raise_error(TypeError, "Invalid type of parameters {}."
-                                   "".format(type(parameters)))
-
-    def get_parameters(self, format: str = "list",
-                       include_not_trainable: bool = False
-                       ) -> Union[List, Dict]: # pylint: disable=W0622
+            raise_error(
+                TypeError, "Invalid type of parameters {}." "".format(type(parameters))
+            )
+
+    def get_parameters(
+        self, format: str = "list", include_not_trainable: bool = False
+    ) -> Union[List, Dict]:  # pylint: disable=W0622
         """Returns the parameters of all parametrized gates in the circuit.
 
         Inverse method of :meth:`qibo.models.circuit.Circuit.set_parameters`.
 
         Args:
             format (str): How to return the variational parameters.
                 Available formats are ``'list'``, ``'dict'`` and ``'flatlist'``.
@@ -726,29 +803,32 @@
         elif format == "flatlist":
             params = []
             for gate in parametrized_gates:
                 gparams = gate.parameters
                 if len(gparams) == 1:
                     gparams = gparams[0]
                 if isinstance(gparams, np.ndarray):
+
                     def traverse(x):
                         if isinstance(x, np.ndarray):
                             for v1 in x:
-                                for v2 in traverse(v1):
-                                    yield v2
+                                yield from traverse(v1)
                         else:
                             yield x
+
                     params.extend(traverse(gparams))
                 elif isinstance(gparams, collections.abc.Iterable):
                     params.extend(gparams)
                 else:
                     params.append(gparams)
         else:
-            raise_error(ValueError, "Unknown format {} given in "
-                                    "``get_parameters``.".format(format))
+            raise_error(
+                ValueError,
+                "Unknown format {} given in " "``get_parameters``.".format(format),
+            )
         return params
 
     def summary(self) -> str:
         """Generates a summary of the circuit.
 
         The summary contains the circuit depths, total number of qubits and
         the all gates sorted in decreasing number of appearance.
@@ -784,18 +864,20 @@
                 Total number of gates = 6
                 Number of qubits = 3
                 Most common gates:
                 h: 3
                 cx: 2
                 ccx: 1
         """
-        logs = [f"Circuit depth = {self.depth}",
-                f"Total number of gates = {self.ngates}",
-                f"Number of qubits = {self.nqubits}",
-                "Most common gates:"]
+        logs = [
+            f"Circuit depth = {self.depth}",
+            f"Total number of gates = {self.ngates}",
+            f"Number of qubits = {self.nqubits}",
+            "Most common gates:",
+        ]
         common_gates = self.gate_types.most_common()
         logs.extend("{}: {}".format(g, n) for g, n in common_gates)
         return "\n".join(logs)
 
     def fuse(self, max_qubits=2):
         """Creates an equivalent circuit by fusing gates for increased simulation performance.
 
@@ -819,16 +901,18 @@
                 c.add([gates.Y(0), gates.Y(1)])
                 # create circuit with fused gates
                 fused_c = c.fuse()
                 # now ``fused_c`` contains a single ``FusedGate`` that is
                 # equivalent to applying the five original gates
         """
         if self.accelerators:  # pragma: no cover
-            raise_error(NotImplementedError, "Fusion is not implemented for "
-                                         "distributed circuits.")
+            raise_error(
+                NotImplementedError,
+                "Fusion is not implemented for " "distributed circuits.",
+            )
 
         queue = self.queue.to_fused()
         for gate in queue:
             if not gate.marked:
                 for q in gate.qubits:
                     # fuse nearest neighbors forth in time
                     neighbor = gate.right_neighbors.get(q)
@@ -846,101 +930,131 @@
     def unitary(self, backend=None):
         """Creates the unitary matrix corresponding to all circuit gates.
 
         This is a ``(2 ** nqubits, 2 ** nqubits)`` matrix obtained by
         multiplying all circuit gates.
         """
         from qibo import gates
+
         if backend is None:
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
         fgate = gates.FusedGate(*range(self.nqubits))
         for gate in self.queue:
             fgate.append(gate)
         return fgate.asmatrix(backend)
 
     @property
     def final_state(self):
         """Returns the final state after full simulation of the circuit.
 
         If the circuit is executed more than once, only the last final state
         is returned.
         """
         if self._final_state is None:
-            raise_error(RuntimeError, "Cannot access final state before the "
-                                      "circuit is executed.")
+            raise_error(
+                RuntimeError,
+                "Cannot access final state before the " "circuit is executed.",
+            )
         return self._final_state
 
     def compile(self, backend=None):
         if self.accelerators:  # pragma: no cover
-            raise_error(RuntimeError, "Cannot compile circuit that uses custom operators.")
+            raise_error(
+                RuntimeError, "Cannot compile circuit that uses custom operators."
+            )
 
         if self.compiled:
             raise_error(RuntimeError, "Circuit is already compiled.")
         if not self.queue:
             raise_error(RuntimeError, "Cannot compile circuit without gates.")
         for gate in self.queue:
             if isinstance(gate, gates.CallbackGate):  # pragma: no cover
-                raise_error(NotImplementedError, "Circuit compilation is not available with callbacks.")
+                raise_error(
+                    NotImplementedError,
+                    "Circuit compilation is not available with callbacks.",
+                )
         if backend is None:
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
 
         from qibo.states import CircuitResult
-        executor = lambda state, nshots: backend.execute_circuit(self, state, nshots, return_array=True)
+
+        executor = lambda state, nshots: backend.execute_circuit(
+            self, state, nshots, return_array=True
+        )
         self.compiled = type("CompiledExecutor", (), {})()
         self.compiled.executor = backend.compile(executor)
-        self.compiled.result = lambda state, nshots: CircuitResult(backend, self, state, nshots)
+        self.compiled.result = lambda state, nshots: CircuitResult(
+            backend, self, state, nshots
+        )
 
     def execute(self, initial_state=None, nshots=None):
         """Executes the circuit. Exact implementation depends on the backend.
 
         See :meth:`qibo.core.circuit.Circuit.execute` for more
         details.
         """
         if self.compiled:
-            state = self.compiled.executor(initial_state, nshots) # pylint: disable=E1101
-            self._final_state = self.compiled.result(state, nshots) # pylint: disable=E1101
+            state = self.compiled.executor(
+                initial_state, nshots
+            )  # pylint: disable=E1101
+            self._final_state = self.compiled.result(
+                state, nshots
+            )  # pylint: disable=E1101
             return self._final_state
         else:
             from qibo.backends import GlobalBackend
+
             if self.accelerators:  # pragma: no cover
-                return GlobalBackend().execute_distributed_circuit(self, initial_state, nshots)
+                return GlobalBackend().execute_distributed_circuit(
+                    self, initial_state, nshots
+                )
             else:
                 return GlobalBackend().execute_circuit(self, initial_state, nshots)
 
     def __call__(self, initial_state=None, nshots=None):
         """Equivalent to ``circuit.execute``."""
         return self.execute(initial_state=initial_state, nshots=nshots)
 
     def to_qasm(self):
         """Convert circuit to QASM.
 
         Args:
             filename (str): The filename where the code is saved.
         """
         from qibo import __version__
+
         code = [f"// Generated by QIBO {__version__}"]
         code += ["OPENQASM 2.0;"]
-        code += ["include \"qelib1.inc\";"]
+        code += ['include "qelib1.inc";']
         code += [f"qreg q[{self.nqubits}];"]
 
         # Set measurements
         for reg_name, reg_qubits in self.measurement_tuples.items():
             if not reg_name.islower():
-                raise_error(NameError, "OpenQASM does not support capital letters in "
-                                       "register names but {} was used".format(reg_name))
+                raise_error(
+                    NameError,
+                    "OpenQASM does not support capital letters in "
+                    "register names but {} was used".format(reg_name),
+                )
             code.append(f"creg {reg_name}[{len(reg_qubits)}];")
 
         # Add gates
         for gate in self.queue:
             if gate.name not in gates.QASM_GATES:
-                raise_error(ValueError, f"Gate {gate.name} is not supported by OpenQASM.")
+                raise_error(
+                    ValueError, f"Gate {gate.name} is not supported by OpenQASM."
+                )
             if gate.is_controlled_by:
-                raise_error(ValueError, "OpenQASM does not support multi-controlled gates.")
+                raise_error(
+                    ValueError, "OpenQASM does not support multi-controlled gates."
+                )
 
             qubits = ",".join(f"q[{i}]" for i in gate.qubits)
             if gate.name in gates.PARAMETRIZED_GATES:
                 params = (str(x) for x in gate.parameters)
                 name = "{}({})".format(gate.name, ", ".join(params))
             else:
                 name = gate.name
@@ -1009,35 +1123,41 @@
             gate_list: List that specifies the gates of the circuit.
                 Contains tuples of the form
                 (Qibo gate name, qubit IDs, optional additional parameter).
                 The additional parameter is the ``register_name`` for
                 measurement gates or ``theta`` for parametrized gates.
         """
         import re
+
         def read_args(args):
             _args = iter(re.split(r"[\[\],]", args))
             for name in _args:
                 if name:
                     index = next(_args)
                     if not index.isdigit():
                         raise_error(ValueError, "Invalid QASM qubit arguments:", args)
                     yield name, int(index)
 
         # Remove comment lines
-        lines = "".join(line for line in qasm_code.split("\n")
-                        if line and line[:2] != "//")
+        lines = "".join(
+            line for line in qasm_code.split("\n") if line and line[:2] != "//"
+        )
         lines = (line for line in lines.split(";") if line)
 
         if next(lines) != "OPENQASM 2.0":
             raise_error(ValueError, "QASM code should start with 'OPENQASM 2.0'.")
 
-        qubits = {} # Dict[Tuple[str, int], int]: map from qubit tuple to qubit id
-        cregs_size = {} # Dict[str, int]: map from `creg` name to its size
-        registers = {} # Dict[str, List[int]]: map from register names to target qubit ids
-        gate_list = [] # List[Tuple[str, List[int]]]: List of (gate name, list of target qubit ids)
+        qubits = {}  # Dict[Tuple[str, int], int]: map from qubit tuple to qubit id
+        cregs_size = {}  # Dict[str, int]: map from `creg` name to its size
+        registers = (
+            {}
+        )  # Dict[str, List[int]]: map from register names to target qubit ids
+        gate_list = (
+            []
+        )  # List[Tuple[str, List[int]]]: List of (gate name, list of target qubit ids)
         for line in lines:
             command, args = line.split(None, 1)
             # remove spaces
             command = command.replace(" ", "")
             args = args.replace(" ", "")
 
             if command == "include":
@@ -1054,77 +1174,98 @@
 
             elif command == "measure":
                 args = args.split("->")
                 if len(args) != 2:
                     raise_error(ValueError, "Invalid QASM measurement:", line)
                 qubit = next(read_args(args[0]))
                 if qubit not in qubits:
-                    raise_error(ValueError, "Qubit {} is not defined in QASM code."
-                                            "".format(qubit))
+                    raise_error(
+                        ValueError,
+                        "Qubit {} is not defined in QASM code." "".format(qubit),
+                    )
 
                 register, idx = next(read_args(args[1]))
                 if register not in cregs_size:
-                    raise_error(ValueError, "Classical register name {} is not defined "
-                                            "in QASM code.".format(register))
+                    raise_error(
+                        ValueError,
+                        "Classical register name {} is not defined "
+                        "in QASM code.".format(register),
+                    )
                 if idx >= cregs_size[register]:
-                    raise_error(ValueError, "Cannot access index {} of register {} "
-                                            "with {} qubits."
-                                            "".format(idx, register, cregs_size[register]))
+                    raise_error(
+                        ValueError,
+                        "Cannot access index {} of register {} "
+                        "with {} qubits."
+                        "".format(idx, register, cregs_size[register]),
+                    )
                 if register in registers:
                     if idx in registers[register]:
-                        raise_error(KeyError, "Key {} of register {} has already "
-                                              "been used.".format(idx, register))
+                        raise_error(
+                            KeyError,
+                            "Key {} of register {} has already "
+                            "been used.".format(idx, register),
+                        )
                     registers[register][idx] = qubits[qubit]
                 else:
                     registers[register] = {idx: qubits[qubit]}
                     gate_list.append(("M", register, None))
 
             else:
                 pieces = [x for x in re.split("[()]", command) if x]
                 if len(pieces) == 1:
                     gatename, params = pieces[0], None
                     if gatename not in gates.QASM_GATES:
-                        raise_error(ValueError, "QASM command {} is not recognized."
-                                                "".format(command))
+                        raise_error(
+                            ValueError,
+                            "QASM command {} is not recognized." "".format(command),
+                        )
                     if gatename in gates.PARAMETRIZED_GATES:
-                        raise_error(ValueError, "Missing parameters for QASM "
-                                                "gate {}.".format(gatename))
+                        raise_error(
+                            ValueError,
+                            "Missing parameters for QASM " "gate {}.".format(gatename),
+                        )
 
                 elif len(pieces) == 2:
                     gatename, params = pieces
                     if gatename not in gates.PARAMETRIZED_GATES:
-                        raise_error(ValueError, "Invalid QASM command {}."
-                                                "".format(command))
+                        raise_error(
+                            ValueError, "Invalid QASM command {}." "".format(command)
+                        )
                     params = params.replace(" ", "").split(",")
                     try:
                         for i, p in enumerate(params):
-                            if 'pi' in p:
-                                from operator import mul
+                            if "pi" in p:
                                 from functools import reduce
-                                s = p.replace('pi', str(np.pi)).split('*')
+                                from operator import mul
+
+                                s = p.replace("pi", str(np.pi)).split("*")
                                 p = reduce(mul, [float(j) for j in s], 1)
                             params[i] = float(p)
                     except ValueError:
-                        raise_error(ValueError, "Invalid value {} for gate parameters."
-                                                "".format(params))
+                        raise_error(
+                            ValueError,
+                            "Invalid value {} for gate parameters." "".format(params),
+                        )
 
                 else:
-                    raise_error(ValueError, "QASM command {} is not recognized."
-                                            "".format(command))
+                    raise_error(
+                        ValueError,
+                        "QASM command {} is not recognized." "".format(command),
+                    )
 
                 # Add gate to gate list
                 qubit_list = []
                 for qubit in read_args(args):
                     if qubit not in qubits:
-                        raise_error(ValueError, "Qubit {} is not defined in QASM "
-                                                "code.".format(qubit))
+                        raise_error(
+                            ValueError,
+                            "Qubit {} is not defined in QASM " "code.".format(qubit),
+                        )
                     qubit_list.append(qubits[qubit])
-                gate_list.append((gates.QASM_GATES[gatename],
-                                  list(qubit_list),
-                                  params))
+                gate_list.append((gates.QASM_GATES[gatename], list(qubit_list), params))
 
         # Create measurement gate qubit lists from registers
         for i, (gatename, register, _) in enumerate(gate_list):
             if gatename == "M":
                 qubit_list = registers[register]
                 qubit_list = [qubit_list[k] for k in sorted(qubit_list.keys())]
                 gate_list[i] = ("M", qubit_list, register)
@@ -1139,36 +1280,70 @@
                 split the circuit text diagram in chunks of line_wrap characters.
             legend (bool): If ``True`` prints a legend below the circuit for
                 callbacks and channels. Default is ``False``.
 
         Return:
             String containing text circuit diagram.
         """
-        labels = {"h": "H", "x": "X", "y": "Y", "z": "Z",
-                  "s": "S", "sdg": "SDG", "t": "T", "tdg": "TDG",
-                  "rx": "RX", "ry": "RY", "rz": "RZ",
-                  "u1": "U1", "u2": "U2", "u3": "U3",
-                  "cx": "X", "swap": "x", "cz": "Z",
-                  "crx": "RX", "cry": "RY", "crz": "RZ",
-                  "cu1": "U1", "cu3": "U3", "ccx": "X",
-                  "id": "I", "measure": "M", "fsim": "f",
-                  "generalizedfsim": "gf", "Unitary": "U", "fswap":"fx",
-                  "PauliNoiseChannel": "PN", "KrausChannel": "K",
-                  "UnitaryChannel": "U", "ThermalRelaxationChannel": "TR",
-                  "ResetChannel": "R", "PartialTrace": "PT",
-                  "EntanglementEntropy": "EE", "Norm": "N",
-                  "Overlap": "O", "Energy": "E"}
+        labels = {
+            "h": "H",
+            "x": "X",
+            "y": "Y",
+            "z": "Z",
+            "s": "S",
+            "sdg": "SDG",
+            "t": "T",
+            "tdg": "TDG",
+            "rx": "RX",
+            "ry": "RY",
+            "rz": "RZ",
+            "u1": "U1",
+            "u2": "U2",
+            "u3": "U3",
+            "cx": "X",
+            "swap": "x",
+            "cz": "Z",
+            "crx": "RX",
+            "cry": "RY",
+            "crz": "RZ",
+            "cu1": "U1",
+            "cu3": "U3",
+            "ccx": "X",
+            "id": "I",
+            "measure": "M",
+            "fsim": "f",
+            "generalizedfsim": "gf",
+            "rxx": "RXX",
+            "ryy": "RYY",
+            "rzz": "RZZ",
+            "Unitary": "U",
+            "fswap": "fx",
+            "PauliNoiseChannel": "PN",
+            "KrausChannel": "K",
+            "UnitaryChannel": "U",
+            "ThermalRelaxationChannel": "TR",
+            "DepolarizingChannel": "D",
+            "ResetChannel": "R",
+            "PartialTrace": "PT",
+            "EntanglementEntropy": "EE",
+            "Norm": "N",
+            "Overlap": "O",
+            "Energy": "E",
+        }
 
         # build string representation of gates
         matrix = [[] for _ in range(self.nqubits)]
         idx = [0] * self.nqubits
 
         for gate in self.queue:
             if gate.name not in labels:  # pragma: no cover
-                raise_error(NotImplementedError, f"{gate.name} gate is not supported by `circuit.draw`")
+                raise_error(
+                    NotImplementedError,
+                    f"{gate.name} gate is not supported by `circuit.draw`",
+                )
             gate_name = labels.get(gate.name)
             if isinstance(gate, gates.CallbackGate):
                 targets = list(range(self.nqubits))
             else:
                 targets = list(gate.target_qubits)
             controls = list(gate.control_qubits)
 
@@ -1179,83 +1354,104 @@
             max_qubits_id = qubits[-1]
 
             # identify column
             col = idx[targets[0]] if not controls and len(targets) == 1 else max(idx)
 
             # extend matrix
             for iq in range(self.nqubits):
-                matrix[iq].extend((1 + col - len(matrix[iq]))* [''])
+                matrix[iq].extend((1 + col - len(matrix[iq])) * [""])
 
             # fill
             for iq in range(min_qubits_id, max_qubits_id + 1):
                 if iq in targets:
                     matrix[iq][col] = gate_name
                 elif iq in controls:
-                    matrix[iq][col] = 'o'
+                    matrix[iq][col] = "o"
                 else:
-                    matrix[iq][col] = '|'
+                    matrix[iq][col] = "|"
 
             # update indexes
             if not controls and len(targets) == 1:
                 idx[targets[0]] += 1
             else:
                 idx = [col + 1] * self.nqubits
 
         # Include measurement gates
         if self.measurement_gate:
             for iq in range(self.nqubits):
-                matrix[iq].append('M' if iq in self.measurement_gate.target_qubits else '')
+                matrix[iq].append(
+                    "M" if iq in self.measurement_gate.target_qubits else ""
+                )
 
         # Add some spacers
         for col in range(len(matrix[0])):
-            maxlen = max([len(matrix[l][col]) for l in range(self.nqubits)])
+            maxlen = max(len(matrix[l][col]) for l in range(self.nqubits))
             for row in range(self.nqubits):
-                matrix[row][col] += '─' * (1 + maxlen - len(matrix[row][col]))
+                matrix[row][col] += "─" * (1 + maxlen - len(matrix[row][col]))
 
         # Print to terminal
         output = ""
         for q in range(self.nqubits):
-            output += f'q{q}' + ' ' * (len(str(self.nqubits))-len(str(q))) + \
-                       ': ─' + ''.join(matrix[q]) + '\n'
+            output += (
+                f"q{q}"
+                + " " * (len(str(self.nqubits)) - len(str(q)))
+                + ": ─"
+                + "".join(matrix[q])
+                + "\n"
+            )
 
         # legend
         if legend:
             from tabulate import tabulate
-            names = [i.name for i in self.queue \
-                     if isinstance(i,gates.CallbackGate) or "Channel" in i.name]
+
+            names = [
+                i.name
+                for i in self.queue
+                if isinstance(i, gates.CallbackGate) or "Channel" in i.name
+            ]
             names = list(dict.fromkeys(names))
-            table = tabulate([[i, labels[i]] for i in names],
-                              headers=['Gate', 'Symbol'],
-                              tablefmt='orgtbl')
-            table = '\n Legend for callbacks and channels: \n' + table
+            table = tabulate(
+                [[i, labels[i]] for i in names],
+                headers=["Gate", "Symbol"],
+                tablefmt="orgtbl",
+            )
+            table = "\n Legend for callbacks and channels: \n" + table
 
         # line wrap
         if line_wrap:
             loutput = output.splitlines()
+
             def chunkstring(string, length):
                 nchunks = range(0, len(string), length)
-                return (string[i:length+i] for i in nchunks), len(nchunks)
+                return (string[i : length + i] for i in nchunks), len(nchunks)
+
             for row in range(self.nqubits):
-                chunks, nchunks = chunkstring(loutput[row][3 + len(str(self.nqubits)):], line_wrap)
+                chunks, nchunks = chunkstring(
+                    loutput[row][3 + len(str(self.nqubits)) :], line_wrap
+                )
                 if nchunks == 1:
                     loutput = None
                     break
                 for i, c in enumerate(chunks):
-                    loutput += ['' for _ in range(self.nqubits)]
-                    suffix = ' ...\n'
-                    prefix = f'q{row}' + ' ' * (len(str(self.nqubits))-len(str(row))) + ': '
+                    loutput += ["" for _ in range(self.nqubits)]
+                    suffix = " ...\n"
+                    prefix = (
+                        f"q{row}"
+                        + " " * (len(str(self.nqubits)) - len(str(row)))
+                        + ": "
+                    )
                     if i == 0:
-                        prefix += ' ' * 4
+                        prefix += " " * 4
                     elif row == 0:
-                        prefix = '\n' + prefix + '... '
+                        prefix = "\n" + prefix + "... "
                     else:
-                        prefix += '... '
-                    if i == nchunks-1:
-                        suffix = '\n'
+                        prefix += "... "
+                    if i == nchunks - 1:
+                        suffix = "\n"
                     loutput[row + i * self.nqubits] = prefix + c + suffix
             if loutput is not None:
-                output = ''.join(loutput)
+                output = "".join(loutput)
 
         if legend:
             output += table
 
-        return output.rstrip('\n')
+        return output.rstrip("\n")
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/distcircuit.py` & `qibo-0.1.9/src/qibo/models/distcircuit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import collections
 import copy
 import math
-import collections
-from qibo.config import raise_error
+from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
+
 from qibo import gates
+from qibo.config import raise_error
+from qibo.gates.abstract import Gate, ParametrizedGate, SpecialGate
 from qibo.models.circuit import Circuit
-from qibo.gates.abstract import Gate, SpecialGate, ParametrizedGate
-from typing import Dict, List, Optional, Sequence, Set, Tuple, Union
 
 
 class DistributedQubits:
     """Data structure that holds lists related to global qubit IDs.
 
     Holds the following data:
     * ``list``: Sorted list with the ids of global qubits.
@@ -26,16 +27,15 @@
     """
 
     def __init__(self, qubits: Sequence[int], nqubits: int):
         self.set = set(qubits)
         self.list = sorted(qubits)
         self.local = [q for q in range(nqubits) if q not in self.set]
         self.reduced_global = {q: self.list.index(q) for q in self.list}
-        self.reduced_local = {q: q - self.reduction_number(q)
-                              for q in self.local}
+        self.reduced_local = {q: q - self.reduction_number(q) for q in self.local}
 
         self.transpose_order = self.list + self.local
         self.reverse_transpose_order = nqubits * [0]
         for i, v in enumerate(self.transpose_order):
             self.reverse_transpose_order[v] = i
 
     def reduction_number(self, q: int) -> int:
@@ -115,16 +115,17 @@
         new gate group will be defined for the new global qubit configuration.
 
         This method also creates the ``DistributedQubits`` object holding the
         global qubits list.
         """
         counter = self.count(queue, self.nqubits)
         if self.qubits is None:
-            self.qubits = DistributedQubits(counter.argsort()[:self.nglobal],
-                                            self.nqubits)
+            self.qubits = DistributedQubits(
+                counter.argsort()[: self.nglobal], self.nqubits
+            )
         if queue:
             transformed_queue = self.transform(queue, counter)
             self.create(transformed_queue)
 
     def _ids(self, accelerators: Dict[str, int]) -> Tuple[str, List[int]]:
         """Generator of device piece indices."""
         start = 0
@@ -144,19 +145,22 @@
 
         Returns:
             A :class:`qibo.gates.abstract.Gate` object with the proper target and
             control qubit indices for device-specific application.
         """
         devgate = copy.copy(gate)
         # Recompute the target/control indices considering only local qubits.
-        new_target_qubits = tuple(q - self.qubits.reduction_number(q)
-                                  for q in devgate.target_qubits)
-        new_control_qubits = tuple(q - self.qubits.reduction_number(q)
-                                   for q in devgate.control_qubits
-                                   if q not in self.qubits.set)
+        new_target_qubits = tuple(
+            q - self.qubits.reduction_number(q) for q in devgate.target_qubits
+        )
+        new_control_qubits = tuple(
+            q - self.qubits.reduction_number(q)
+            for q in devgate.control_qubits
+            if q not in self.qubits.set
+        )
         devgate._set_targets_and_controls(new_target_qubits, new_control_qubits)
         devgate.original_gate = gate
         devgate.device_gates = set()
         return devgate
 
     @staticmethod
     def count(queue: List[Gate], nqubits: int):
@@ -167,23 +171,24 @@
             nqubits: Number of total qubits in the circuit.
 
         Returns:
             Array of integers with shape (nqubits,) with the number of gates
             for each qubit id.
         """
         import numpy as np
+
         counter = np.zeros(nqubits, dtype=np.int64)
         for gate in queue:
             for qubit in gate.target_qubits:
                 counter[qubit] += 1
         return counter
 
-    def _transform(self, queue: List[Gate],
-                   remaining_queue: List[Gate],
-                   counter) -> List[Gate]:
+    def _transform(
+        self, queue: List[Gate], remaining_queue: List[Gate], counter
+    ) -> List[Gate]:
         """Helper recursive method for ``transform``."""
         new_remaining_queue = []
         for gate in remaining_queue:
             if isinstance(gate, (SpecialGate, gates.M)):  # pragma: no cover
                 gate.swap_reset = list(self.swaps_list)
 
             global_targets = set(gate.target_qubits) & self.qubits.set
@@ -203,21 +208,22 @@
         if not new_remaining_queue:
             return queue
 
         # Find which qubits to swap
         gate = new_remaining_queue[0]
         target_set = set(gate.target_qubits)
         global_targets = target_set & self.qubits.set
-        if isinstance(gate, gates.SWAP): # pragma: no cover
+        if isinstance(gate, gates.SWAP):  # pragma: no cover
             # special case of swap on two global qubits
             assert len(global_targets) == 2
             global_targets.remove(target_set.pop())
 
-        available_swaps = (q for q in counter.argsort()
-                           if q not in self.qubits.set | target_set)
+        available_swaps = (
+            q for q in counter.argsort() if q not in self.qubits.set | target_set
+        )
         qubit_map = {}
         for q in global_targets:
             qs = next(available_swaps)
             # Update qubit map that holds the swaps
             qubit_map[q] = qs
             qubit_map[qs] = q
             # Keep SWAPs in memory to reset them in the end
@@ -225,18 +231,20 @@
             # Add ``SWAP`` gate in ``queue``.
             queue.append(gates.SWAP(q, qs))
             #  Modify ``counter`` to take into account the swaps
             counter[q], counter[qs] = counter[qs], counter[q]
 
         # Modify gates to take into account the swaps
         for gate in new_remaining_queue:
-            new_target_qubits = tuple(qubit_map[q] if q in qubit_map else q
-                                       for q in gate.target_qubits)
-            new_control_qubits = tuple(qubit_map[q] if q in qubit_map else q
-                                        for q in gate.control_qubits)
+            new_target_qubits = tuple(
+                qubit_map[q] if q in qubit_map else q for q in gate.target_qubits
+            )
+            new_control_qubits = tuple(
+                qubit_map[q] if q in qubit_map else q for q in gate.control_qubits
+            )
             gate._set_targets_and_controls(new_target_qubits, new_control_qubits)
 
         return self._transform(queue, new_remaining_queue, counter)
 
     def transform(self, queue, counter=None):
         """Transforms gate queue to be compatible with distributed simulation.
 
@@ -252,15 +260,15 @@
             List of gates that have the same effect as the original queue but
             are compatible with distributed run (do not have global qubits as
             targets).
         """
         if counter is None:
             counter = self.count(queue, self.nqubits)
         new_queue = self._transform([], queue, counter)
-        new_queue.extend((gates.SWAP(*p) for p in reversed(self.swaps_list)))
+        new_queue.extend(gates.SWAP(*p) for p in reversed(self.swaps_list))
         return new_queue
 
     def create(self, queue: List[Gate]):
         """Creates the queues for each accelerator device.
 
         Args:
             queue (list): List of gates compatible with distributed run.
@@ -271,21 +279,25 @@
             is_collapse = isinstance(gate, gates.M) and gate.collapse
             if not gate.target_qubits or is_collapse:  # pragma: no cover
                 # special gate
                 gate.nqubits = self.nqubits
                 self.special_queue.append(gate)
                 self.queues.append([])
 
-            elif set(gate.target_qubits) & self.qubits.set: # global swap gate
+            elif set(gate.target_qubits) & self.qubits.set:  # global swap gate
                 global_qubits = set(gate.target_qubits) & self.qubits.set
                 if not isinstance(gate, gates.SWAP):
-                    raise_error(ValueError, "Only SWAP gates are supported for "
-                                            "global qubits.")
+                    raise_error(
+                        ValueError,
+                        "Only SWAP gates are supported for " "global qubits.",
+                    )
                 if len(global_qubits) > 1:
-                    raise_error(ValueError, "SWAPs between global qubits are not allowed.")
+                    raise_error(
+                        ValueError, "SWAPs between global qubits are not allowed."
+                    )
 
                 global_qubit = global_qubits.pop()
                 local_qubit = gate.target_qubits[0]
                 if local_qubit == global_qubit:
                     local_qubit = gate.target_qubits[1]
 
                 self.special_queue.append((global_qubit, local_qubit))
@@ -301,18 +313,17 @@
                     # device otherwise device parallelization will break
                     devgate.device = device
                     devgate.nqubits = self.nlocal
                     for i in ids:
                         flag = True
                         # If there are control qubits that are global then
                         # the gate should not be applied by all devices
-                        for control in (set(gate.control_qubits) &
-                                        self.qubits.set):
+                        for control in set(gate.control_qubits) & self.qubits.set:
                             ic = self.qubits.list.index(control)
                             ic = self.nglobal - ic - 1
-                            flag = bool((i // (2 ** ic)) % 2)
+                            flag = bool((i // (2**ic)) % 2)
                             if not flag:
                                 break
                         if flag:
                             self.queues[-1][i].append(devgate)
                             if isinstance(gate, ParametrizedGate):
                                 gate.device_gates.add(devgate)
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/evolution.py` & `qibo-0.1.9/src/qibo/models/evolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Models for time evolution of state vectors."""
-from qibo import solvers, optimizers
+from qibo import optimizers, solvers
+from qibo.callbacks import Gap, Norm
 from qibo.config import log, raise_error
-from qibo.callbacks import Norm, Gap
 from qibo.hamiltonians.abstract import AbstractHamiltonian
-from qibo.hamiltonians.adiabatic import BaseAdiabaticHamiltonian, AdiabaticHamiltonian
+from qibo.hamiltonians.adiabatic import AdiabaticHamiltonian, BaseAdiabaticHamiltonian
 from qibo.hamiltonians.hamiltonians import SymbolicHamiltonian
 
 
 class StateEvolution:
     """Unitary time evolution of a state vector under a Hamiltonian.
 
     Args:
@@ -43,59 +43,63 @@
             evolve = models.StateEvolution(hamiltonian, dt=1e-2)
             # initialize state to |+++>
             initial_state = np.ones(8) / np.sqrt(8)
             # execute evolution for total time T=2
             final_state2 = evolve(final_time=2, initial_state=initial_state)
     """
 
-    def __init__(self, hamiltonian, dt, solver="exp", callbacks=[],
-                 accelerators=None):
+    def __init__(self, hamiltonian, dt, solver="exp", callbacks=[], accelerators=None):
         hamtypes = (AbstractHamiltonian, BaseAdiabaticHamiltonian)
         if isinstance(hamiltonian, hamtypes):
             ham = hamiltonian
         else:
             ham = hamiltonian(0)
             if not isinstance(ham, AbstractHamiltonian):
-                raise TypeError("Hamiltonian type {} not understood."
-                                "".format(type(ham)))
+                raise TypeError(
+                    "Hamiltonian type {} not understood." "".format(type(ham))
+                )
         self.nqubits = ham.nqubits
         self.backend = ham.backend
         if dt <= 0:
             raise_error(ValueError, f"Time step dt should be positive but is {dt}.")
         self.dt = dt
 
         disthamtypes = (SymbolicHamiltonian, BaseAdiabaticHamiltonian)
         if accelerators is not None:  # pragma: no cover
             if not isinstance(ham, disthamtypes) or solver != "exp":
-                raise_error(NotImplementedError, "Distributed evolution is only "
-                                                 "implemented using the Trotter "
-                                                 "exponential solver.")
+                raise_error(
+                    NotImplementedError,
+                    "Distributed evolution is only "
+                    "implemented using the Trotter "
+                    "exponential solver.",
+                )
             ham.circuit(dt, accelerators)
         self.solver = solvers.get_solver(solver, self.dt, hamiltonian)
         self.callbacks = callbacks
         self.accelerators = accelerators
         self.normalize_state = self._create_normalize_state(solver)
         self.calculate_callbacks = self._create_calculate_callbacks(accelerators)
 
     def _create_normalize_state(self, solver):
         if "rk" in solver:
-            log.info('Normalizing state during RK solution.')
+            log.info("Normalizing state during RK solution.")
             return lambda s: s / self.backend.calculate_norm(s)
         else:
             return lambda s: s
 
     def _create_calculate_callbacks(self, accelerators):
         def calculate_callbacks(state):
             for callback in self.callbacks:
                 callback.append(callback.apply(self.backend, state))
 
         if accelerators is None:
             return calculate_callbacks
 
         else:  # pragma: no cover
+
             def calculate_callbacks_distributed(state):
                 if not isinstance(state, self.backend.tensor_types):
                     state = state.state()
                 calculate_callbacks(state)
 
             return calculate_callbacks_distributed
 
@@ -109,16 +113,17 @@
 
         Returns:
             Final state vector a ``tf.Tensor`` or a
             :class:`qibo.core.distutils.DistributedState` when a
             distributed execution is used.
         """
         if initial_state is None:
-            raise_error(ValueError, "StateEvolution cannot be used without "
-                                    "initial state.")
+            raise_error(
+                ValueError, "StateEvolution cannot be used without " "initial state."
+            )
         state = self.backend.cast(initial_state)
         self.solver.t = start_time
         nsteps = int((final_time - start_time) / self.solver.dt)
         self.calculate_callbacks(state)
         for _ in range(nsteps):
             state = self.solver(state)
             if self.callbacks:
@@ -161,46 +166,52 @@
             Runge-Kutta solvers use simple matrix multiplications of the
             Hamiltonian to the state and no exponentiation is involved.
         callbacks (list): List of callbacks to calculate during evolution.
         accelerators (dict): Dictionary of devices to use for distributed
             execution. This option is available only when the Trotter
             decomposition is used for the time evolution.
     """
-    ATOL = 1e-7 # Tolerance for checking s(0) = 0 and s(T) = 1.
 
-    def __init__(self, h0, h1, s, dt, solver="exp", callbacks=[],
-                 accelerators=None):
-        self.hamiltonian = AdiabaticHamiltonian(h0, h1) # pylint: disable=E0110
+    ATOL = 1e-7  # Tolerance for checking s(0) = 0 and s(T) = 1.
+
+    def __init__(self, h0, h1, s, dt, solver="exp", callbacks=[], accelerators=None):
+        self.hamiltonian = AdiabaticHamiltonian(h0, h1)  # pylint: disable=E0110
         super().__init__(self.hamiltonian, dt, solver, callbacks, accelerators)
 
         # Set evolution model to "Gap" callback if one exists
         for callback in self.callbacks:
             if isinstance(callback, Gap):
                 callback.evolution = self
 
         # Flag to control if loss messages are shown during optimization
         self.opt_messages = False
         self.opt_history = {"params": [], "loss": []}
 
         self.parametrized_schedule = None
         nparams = s.__code__.co_argcount
-        if nparams == 1: # given ``s`` is a function of time only
+        if nparams == 1:  # given ``s`` is a function of time only
             self.schedule = s
-        elif nparams == 2: # given ``s`` has undefined parameters
+        elif nparams == 2:  # given ``s`` has undefined parameters
             self.parametrized_schedule = s
         else:
-            raise_error(ValueError, f"Scheduling function shoud take one or "
-                                     "two arguments but it takes {nparams}.")
+            raise_error(
+                ValueError,
+                f"Scheduling function shoud take one or "
+                "two arguments but it takes {nparams}.",
+            )
 
     @property
     def schedule(self):
         """Returns scheduling as a function of time."""
         if self.hamiltonian.schedule is None:
-            raise_error(ValueError, "Cannot access scheduling function before "
-                                    "setting its free parameters.")
+            raise_error(
+                ValueError,
+                "Cannot access scheduling function before "
+                "setting its free parameters.",
+            )
         return self.hamiltonian.schedule
 
     @schedule.setter
     def schedule(self, f):
         """Sets scheduling s(t) function."""
         s0 = f(0)
         if abs(s0) > self.ATOL:
@@ -215,40 +226,43 @@
         if self.parametrized_schedule is not None:
             self.schedule = lambda t: self.parametrized_schedule(t, params[:-1])
         self.hamiltonian.total_time = params[-1]
 
     def execute(self, final_time, start_time=0.0, initial_state=None):
         """"""
         if start_time != 0:
-            raise_error(NotImplementedError, "Adiabatic evolution supports only t=0 "
-                                             "as initial time.")
+            raise_error(
+                NotImplementedError,
+                "Adiabatic evolution supports only t=0 " "as initial time.",
+            )
         self.hamiltonian.total_time = final_time - start_time
         if initial_state is None:
             initial_state = self.hamiltonian.ground_state()
-        return super(AdiabaticEvolution, self).execute(final_time, start_time, initial_state)
+        return super().execute(final_time, start_time, initial_state)
 
     @staticmethod
     def _loss(params, adiabatic_evolution, h1, opt_messages, opt_history):
         """Expectation value of H1 for a choice of scheduling parameters.
 
         Returns a ``tf.Tensor``.
         """
         adiabatic_evolution.set_parameters(params)
         ham = adiabatic_evolution.hamiltonian
         initial_state = ham.backend.cast(ham.h0.ground_state(), copy=True)
-        final_state = super(AdiabaticEvolution, adiabatic_evolution).execute(params[-1], initial_state=initial_state)
+        final_state = super(AdiabaticEvolution, adiabatic_evolution).execute(
+            params[-1], initial_state=initial_state
+        )
         loss = h1.expectation(final_state, normalize=True)
         if opt_messages:
             opt_history["params"].append(params)
             opt_history["loss"].append(loss)
             log.info(f"Params: {params}  -  <H1> = {loss}")
         return loss
 
-    def minimize(self, initial_parameters, method="BFGS", options=None,
-                 messages=False):
+    def minimize(self, initial_parameters, method="BFGS", options=None, messages=False):
         """Optimize the free parameters of the scheduling function.
 
         Args:
             initial_parameters (np.ndarray): Initial guess for the variational
                 parameters that are optimized.
                 The last element of the given array should correspond to the
                 guess for the total evolution time T.
@@ -260,17 +274,22 @@
             messages (bool): If ``True`` the loss evolution is shown during
                 optimization.
         """
         self.opt_messages = messages
         if method == "sgd":
             loss = self._loss
         else:
-            loss = lambda p, ae, h1, msg, hist: self.backend.to_numpy(self._loss(p, ae, h1, msg, hist))
+            loss = lambda p, ae, h1, msg, hist: self.backend.to_numpy(
+                self._loss(p, ae, h1, msg, hist)
+            )
 
         args = (self, self.hamiltonian.h1, self.opt_messages, self.opt_history)
         result, parameters, extra = optimizers.optimize(
-            loss, initial_parameters, args=args, method=method, options=options)
-        if isinstance(parameters, self.backend.tensor_types) and not len(parameters.shape): # pragma: no cover
+            loss, initial_parameters, args=args, method=method, options=options
+        )
+        if isinstance(parameters, self.backend.tensor_types) and not len(
+            parameters.shape
+        ):  # pragma: no cover
             # some optimizers like ``Powell`` return number instead of list
             parameters = [parameters]
         self.set_parameters(parameters)
         return result, parameters, extra
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/grover.py` & `qibo-0.1.9/src/qibo/models/grover.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import numpy as np
+
 from qibo import gates
 from qibo.config import log, raise_error
 from qibo.models.circuit import Circuit
 
 
-class Grover(object):
+class Grover:
     """Model that performs Grover's algorithm.
 
     For Grover's original search algorithm: `arXiv:quant-ph/9605043 <https://arxiv.org/abs/quant-ph/9605043>`_
     For the iterative version with unknown solutions:`arXiv:quant-ph/9605034 <https://arxiv.org/abs/quant-ph/9605034>`_
     For the Grover algorithm with any superposition:`arXiv:quant-ph/9712011 <https://arxiv.org/abs/quant-ph/9712011>`_
 
     Args:
@@ -49,87 +50,116 @@
             superposition = Circuit(5)
             superposition.add([gates.H(i) for i in range(5)])
             # Generate and execute Grover class
             grover = Grover(oracle, superposition_circuit=superposition, number_solutions=1)
             solution, iterations = grover()
     """
 
-    def __init__(self, oracle, superposition_circuit=None, initial_state_circuit=None,
-                 superposition_qubits=None, superposition_size=None, number_solutions=None,
-                 target_amplitude = None, check=None, check_args=(), iterative=False):
+    def __init__(
+        self,
+        oracle,
+        superposition_circuit=None,
+        initial_state_circuit=None,
+        superposition_qubits=None,
+        superposition_size=None,
+        number_solutions=None,
+        target_amplitude=None,
+        check=None,
+        check_args=(),
+        iterative=False,
+    ):
 
         self.oracle = oracle
         self.initial_state_circuit = initial_state_circuit
 
         if superposition_circuit:
             self.superposition = superposition_circuit
         else:
             if not superposition_qubits:
-                raise_error(ValueError, "Cannot create Grover model if the "
-                                        "superposition circuit or number of "
-                                        "qubits is not specified.")
+                raise_error(
+                    ValueError,
+                    "Cannot create Grover model if the "
+                    "superposition circuit or number of "
+                    "qubits is not specified.",
+                )
             self.superposition = Circuit(superposition_qubits)
             self.superposition.add([gates.H(i) for i in range(superposition_qubits)])
 
         if superposition_qubits:
             self.sup_qubits = superposition_qubits
         else:
             self.sup_qubits = self.superposition.nqubits
 
         if superposition_size:
             self.sup_size = superposition_size
         else:
-            self.sup_size = int(2 ** self.sup_qubits)
+            self.sup_size = int(2**self.sup_qubits)
 
         assert oracle.nqubits > self.sup_qubits
 
         self.anc_qubits_sup = self.superposition.nqubits - self.sup_qubits
         self.anc_qubits_ora = self.oracle.nqubits - self.sup_qubits - 1
 
-        self.nqubits = self.sup_qubits + max(self.anc_qubits_sup, self.anc_qubits_ora) + 1
+        self.nqubits = (
+            self.sup_qubits + max(self.anc_qubits_sup, self.anc_qubits_ora) + 1
+        )
 
         self.check = check
         self.check_args = check_args
         self.num_sol = number_solutions
         self.targ_a = target_amplitude
         self.iterative = iterative
 
         self.space_sup = list(range(self.sup_qubits + self.anc_qubits_sup))
-        self.space_ora = list(range(self.sup_qubits + self.anc_qubits_ora)) + [self.nqubits-1]
+        self.space_ora = list(range(self.sup_qubits + self.anc_qubits_ora)) + [
+            self.nqubits - 1
+        ]
 
     def initialize(self):
         """Initialize the Grover algorithm with the superposition and Grover ancilla."""
         c = Circuit(self.nqubits)
-        c.add(gates.X(self.nqubits-1))
-        c.add(gates.H(self.nqubits-1))
+        c.add(gates.X(self.nqubits - 1))
+        c.add(gates.H(self.nqubits - 1))
         if self.initial_state_circuit:
-            c.add(self.initial_state_circuit.invert().on_qubits(*range(self.initial_state_circuit.nqubits)))
+            c.add(
+                self.initial_state_circuit.invert().on_qubits(
+                    *range(self.initial_state_circuit.nqubits)
+                )
+            )
         c.add(self.superposition.on_qubits(*self.space_sup))
         return c
 
     def diffusion(self):
         """Construct the diffusion operator out of the superposition circuit."""
         nqubits = self.superposition.nqubits + 1
         c = Circuit(nqubits)
-        c.add(self.superposition.invert().on_qubits(*range(nqubits-1)))
+        c.add(self.superposition.invert().on_qubits(*range(nqubits - 1)))
         if self.initial_state_circuit:
-            c.add(self.initial_state_circuit.invert().on_qubits(*range(self.initial_state_circuit.nqubits)))
+            c.add(
+                self.initial_state_circuit.invert().on_qubits(
+                    *range(self.initial_state_circuit.nqubits)
+                )
+            )
         c.add([gates.X(i) for i in range(self.sup_qubits)])
-        c.add(gates.X(nqubits-1).controlled_by(*range(self.sup_qubits)))
+        c.add(gates.X(nqubits - 1).controlled_by(*range(self.sup_qubits)))
         c.add([gates.X(i) for i in range(self.sup_qubits)])
         if self.initial_state_circuit:
-            c.add(self.initial_state_circuit.on_qubits(*range(self.initial_state_circuit.nqubits)))
-        c.add(self.superposition.on_qubits(*range(nqubits-1)))
+            c.add(
+                self.initial_state_circuit.on_qubits(
+                    *range(self.initial_state_circuit.nqubits)
+                )
+            )
+        c.add(self.superposition.on_qubits(*range(nqubits - 1)))
         return c
 
     def step(self):
         """Combine oracle and diffusion for a Grover step."""
         c = Circuit(self.nqubits)
         c.add(self.oracle.on_qubits(*self.space_ora))
-        c.add(self.diffusion().on_qubits(*(self.space_sup+[self.nqubits-1])))
+        c.add(self.diffusion().on_qubits(*(self.space_sup + [self.nqubits - 1])))
         return c
 
     def circuit(self, iterations):
         """Creates circuit that performs Grover's algorithm with a set amount of iterations.
 
         Args:
             iterations (int): number of times to repeat the Grover step.
@@ -140,28 +170,29 @@
         c = Circuit(self.nqubits)
         c += self.initialize()
         for _ in range(iterations):
             c += self.step()
         c.add(gates.M(*range(self.sup_qubits)))
         return c
 
-    def iterative_grover(self, lamda_value=6/5, backend=None):
+    def iterative_grover(self, lamda_value=6 / 5, backend=None):
         """Iterative approach of Grover for when the number of solutions is not known.
 
         Args:
             lamda_value (real): parameter that controls the evolution of the iterative method.
                                 Must be between 1 and 4/3.
             backend (:class:`qibo.backends.abstract.Backend`): Backend to use for circuit execution.
 
         Returns:
             measured (str): bitstring measured and checked as a valid solution.
             total_iterations (int): number of times the oracle has been called.
         """
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
 
         k = 1
         lamda = lamda_value
         total_iterations = 0
         while True:
             it = np.random.randint(k + 1)
@@ -169,15 +200,15 @@
                 total_iterations += it
                 circuit = self.circuit(it)
                 result = backend.execute_circuit(circuit, nshots=1)
                 measured = result.frequencies(binary=True).most_common(1)[0][0]
                 if self.check(measured, *self.check_args):
                     return measured, total_iterations
             k = min(lamda * k, np.sqrt(self.sup_size))
-            if total_iterations > (9/4) * np.sqrt(self.sup_size):
+            if total_iterations > (9 / 4) * np.sqrt(self.sup_size):
                 log.warning("Too many total iterations, output might not be solution.")
                 return measured, total_iterations
 
     def execute(self, nshots=100, freq=False, logs=False, backend=None):
         """Execute Grover's algorithm.
 
         If the number of solutions is given, calculates iterations,
@@ -190,56 +221,60 @@
 
         Returns:
             solution (str): bitstring (or list of bitstrings) measured as solution of the search.
             iterations (int): number of oracle calls done to reach a solution.
         """
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
 
         if (self.num_sol or self.targ_a) and not self.iterative:
             if self.targ_a:
-                it = int(np.pi * (1/self.targ_a) / 4)
+                it = int(np.pi * (1 / self.targ_a) / 4)
             else:
                 it = int(np.pi * np.sqrt(self.sup_size / self.num_sol) / 4)
             circuit = self.circuit(it)
             result = backend.execute_circuit(circuit, nshots=nshots)
             result = result.frequencies(binary=True)
             if freq:
                 if logs:
                     log.info("Result of sampling Grover's algorihm")
                     log.info(result)
                 self.frequencies = result
             if logs:
-                log.info(f"Most common states found using Grover's algorithm with {it} iterations:")
+                log.info(
+                    f"Most common states found using Grover's algorithm with {it} iterations:"
+                )
             if self.targ_a:
                 most_common = result.most_common(1)
             else:
                 most_common = result.most_common(self.num_sol)
             self.solution = []
             self.iterations = it
             for i in most_common:
                 if logs:
                     log.info(i[0])
                 self.solution.append(i[0])
                 if logs:
                     if self.check:
                         if self.check(i[0], *self.check_args):
-                            log.info('Solution checked and successful.')
+                            log.info("Solution checked and successful.")
                         else:
-                            log.info('Not a solution of the problem. Something went wrong.')
+                            log.info(
+                                "Not a solution of the problem. Something went wrong."
+                            )
         else:
             if not self.check:
                 raise_error(ValueError, "Check function needed for iterative approach.")
             measured, total_iterations = self.iterative_grover(backend=backend)
             if logs:
-                log.info('Solution found in an iterative process.')
-                log.info(f'Solution: {measured}')
-                log.info(f'Total Grover iterations taken: {total_iterations}')
+                log.info("Solution found in an iterative process.")
+                log.info(f"Solution: {measured}")
+                log.info(f"Total Grover iterations taken: {total_iterations}")
             self.solution = measured
             self.iterations = total_iterations
         return self.solution, self.iterations
 
-
     def __call__(self, nshots=100, freq=False, logs=False, backend=None):
         """Equivalent to :meth:`qibo.models.grover.Grover.execute`."""
         return self.execute(nshots=nshots, freq=freq, logs=logs, backend=backend)
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/hep.py` & `qibo-0.1.9/src/qibo/models/hep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 import numpy as np
-from qibo import gates, matrices
+
+from qibo import gates
+from qibo.backends import matrices
+from qibo.config import raise_error
 from qibo.hamiltonians import Hamiltonian
 from qibo.models.circuit import Circuit
-from qibo.config import raise_error
 
 
 class qPDF:
     """Variational Circuit for Quantum PDFs (qPDF).
 
     Args:
         ansatz (str): the ansatz name, options are 'Weighted' and 'Fourier'.
         layers (int): the number of layers for the ansatz.
         nqubits (int): the number of qubits for the circuit.
         multi_output (bool): allocates a multi-output model per PDF flavour (default is False).
         backend (:class:`qibo.backends.abstract.Backend`): Backend object to use for execution.
             If ``None`` the currently active global backend is used.
             Default is ``None``.
     """
+
     def __init__(self, ansatz, layers, nqubits, multi_output=False, backend=None):
         """Initialize qPDF."""
-        if not isinstance(layers, int) or layers < 1: # pragma: no cover
+        if not isinstance(layers, int) or layers < 1:  # pragma: no cover
             raise_error(RuntimeError, "Layers must be positive and integer.")
-        if not isinstance(nqubits, int) or nqubits < 1: # pragma: no cover
+        if not isinstance(nqubits, int) or nqubits < 1:  # pragma: no cover
             raise_error(RuntimeError, "Number of qubits must be positive and integer.")
-        if not isinstance(multi_output, bool): # pragma: no cover
+        if not isinstance(multi_output, bool):  # pragma: no cover
             raise_error(TypeError, "multi-output must be a boolean.")
 
         # parse ansatz
-        if ansatz == 'Weighted':
+        if ansatz == "Weighted":
             ansatz_function = ansatz_Weighted
-        elif ansatz == 'Fourier':
+        elif ansatz == "Fourier":
             ansatz_function = ansatz_Fourier
-        else: # pragma: no cover
+        else:  # pragma: no cover
             raise_error(NotImplementedError, f"Ansatz {ansatz} not found.")
 
         # load ansatz
         self.circuit, self.rotation, self.nparams = ansatz_function(layers, nqubits)
 
         # load backend
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             self.backend = GlobalBackend()
         else:
             self.backend = backend
 
         # load hamiltonian
         if multi_output:
-            self.hamiltonian = [qpdf_hamiltonian(
-                nqubits, z_qubit=q, backend=self.backend) for q in range(nqubits)]
+            self.hamiltonian = [
+                qpdf_hamiltonian(nqubits, z_qubit=q, backend=self.backend)
+                for q in range(nqubits)
+            ]
         else:
             self.hamiltonian = [qpdf_hamiltonian(nqubits, backend=self.backend)]
 
     def _model(self, state, hamiltonian):
         """Internal function for the evaluation of PDFs.
 
         Args:
@@ -71,17 +77,18 @@
         Args:
             parameters (numpy.array): list of parameters for the gates.
             x (numpy.array): a numpy array with the points in x to be evaluated.
 
         Returns:
             A numpy array with the PDF values.
         """
-        if len(parameters) != self.nparams: # pragma: no cover
+        if len(parameters) != self.nparams:  # pragma: no cover
             raise_error(
-                RuntimeError, 'Mismatch between number of parameters and model size.')
+                RuntimeError, "Mismatch between number of parameters and model size."
+            )
         pdf = np.zeros(shape=(len(x), len(self.hamiltonian)))
         for i, x_value in enumerate(x):
             params = self.rotation(parameters, x_value)
             self.circuit.set_parameters(params)
             result = self.backend.execute_circuit(self.circuit)
             state = result.state()
             for flavour, flavour_hamiltonian in enumerate(self.hamiltonian):
@@ -126,15 +133,15 @@
 def map_to(x):
     """Auxiliary function"""
     return 2 * np.pi * x
 
 
 def maplog_to(x):
     """Auxiliary function"""
-    return - np.pi * np.log10(x)
+    return -np.pi * np.log10(x)
 
 
 def ansatz_Fourier(layers, qubits=1):
     """Fourier Ansatz implementation. It is composed by 3 parameters per layer
     and qubit: U3(a, b, c) Ry(x) || U3(a, b, c) Ry(log x).
 
     Args:
@@ -168,47 +175,47 @@
     def rotation(theta, x):
         p = circuit.get_parameters()
         i = 0
         j = 0
         for l in range(layers - 1):
             for q in range(qubits):
                 p[i] = map_to(x)
-                p[i + 1: i + 3] = theta[j: j + 2]
+                p[i + 1 : i + 3] = theta[j : j + 2]
                 i += 3
                 j += 2
 
-                p[i] = .5 * maplog_to(x)
-                p[i + 1: i + 3] = theta[j: j + 2]
+                p[i] = 0.5 * maplog_to(x)
+                p[i + 1 : i + 3] = theta[j : j + 2]
                 i += 3
                 j += 2
             if qubits > 1:
                 for q in range(0, qubits, 2):
                     p[i] = theta[j]
                     i += 1
                     j += 1
             if qubits > 2:
                 for q in range(1, qubits + 1, 2):
                     p[i] = theta[j]
                     i += 1
                     j += 1
         for q in range(qubits):
-            p[i] = .5 * map_to(x)
-            p[i + 1: i + 3] = theta[j: j + 2]
+            p[i] = 0.5 * map_to(x)
+            p[i + 1 : i + 3] = theta[j : j + 2]
             i += 3
             j += 2
 
-            p[i] = .5 * maplog_to(x)
-            p[i + 1: i + 3] = theta[j: j + 2]
+            p[i] = 0.5 * maplog_to(x)
+            p[i + 1 : i + 3] = theta[j : j + 2]
             i += 3
             j += 2
         return p
 
-    nparams = 4 * layers * qubits + \
-        (layers - 1) * int(np.ceil(qubits / 2)) * \
-        (int(qubits > 1) + int(qubits > 2))
+    nparams = 4 * layers * qubits + (layers - 1) * int(np.ceil(qubits / 2)) * (
+        int(qubits > 1) + int(qubits > 2)
+    )
 
     return circuit, rotation, nparams
 
 
 def ansatz_Weighted(layers, qubits=1):
     """Fourier Ansatz implementation. 4 parameters per layer and
     qubit: Ry(wx + a), Rz(v log(x) + b)
@@ -262,11 +269,11 @@
             p[i] = theta[j] + theta[j + 1] * map_to(x)
             p[i + 1] = theta[j + 2] + theta[j + 3] * maplog_to(x)
             i += 2
             j += 4
 
         return p
 
-    nparams = 4 * layers * qubits + \
-        (layers - 1) * int(np.ceil(qubits / 2)) * \
-        (int(qubits > 1) + int(qubits > 2))
+    nparams = 4 * layers * qubits + (layers - 1) * int(np.ceil(qubits / 2)) * (
+        int(qubits > 1) + int(qubits > 2)
+    )
     return circuit, rotation, nparams
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/qft.py` & `qibo-0.1.9/src/qibo/models/qft.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import math
+
 from qibo import gates
 from qibo.config import raise_error
 from qibo.models.circuit import Circuit
 
 
 def QFT(nqubits, with_swaps=True, accelerators=None) -> Circuit:
     """Creates a circuit that implements the Quantum Fourier Transform.
@@ -29,16 +30,18 @@
             init_state = np.random.random(2 ** nqubits) + 1j * np.random.random(2 ** nqubits)
             init_state = init_state / np.sqrt((np.abs(init_state)**2).sum())
             # Execute the circuit
             final_state = c(init_state)
     """
     if accelerators is not None:
         if not with_swaps:
-            raise_error(NotImplementedError, "Distributed QFT is only implemented "
-                                             "with SWAPs.")
+            raise_error(
+                NotImplementedError,
+                "Distributed QFT is only implemented " "with SWAPs.",
+            )
         return _DistributedQFT(nqubits, accelerators)
 
     circuit = Circuit(nqubits)
     for i1 in range(nqubits):
         circuit.add(gates.H(i1))
         for i2 in range(i1 + 1, nqubits):
             theta = math.pi / 2 ** (i2 - i1)
@@ -52,19 +55,22 @@
 
 
 def _DistributedQFT(nqubits, accelerators=None):
     """QFT with the order of gates optimized for reduced multi-device communication."""
     circuit = Circuit(nqubits, accelerators)
     icrit = nqubits // 2 + nqubits % 2
     if accelerators is not None:
-        circuit.global_qubits = range(circuit.nlocal, nqubits) # pylint: disable=E1101
-        if icrit < circuit.nglobal: # pylint: disable=E1101
-            raise_error(NotImplementedError, "Cannot implement QFT for {} qubits "
-                                             "using {} global qubits."
-                                             "".format(nqubits, circuit.nglobal)) # pylint: disable=E1101
+        circuit.global_qubits = range(circuit.nlocal, nqubits)  # pylint: disable=E1101
+        if icrit < circuit.nglobal:  # pylint: disable=E1101
+            raise_error(
+                NotImplementedError,
+                "Cannot implement QFT for {} qubits "
+                "using {} global qubits."
+                "".format(nqubits, circuit.nglobal),
+            )  # pylint: disable=E1101
 
     for i1 in range(nqubits):
         if i1 < icrit:
             i1eff = i1
         else:
             i1eff = nqubits - i1 - 1
             circuit.add(gates.SWAP(i1, i1eff))
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/qgan.py` & `qibo-0.1.9/src/qibo/models/qgan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 from numpy.random import randn
-from qibo import gates, hamiltonians, matrices, models
+
+from qibo import gates, hamiltonians, models
+from qibo.backends import matrices
 from qibo.config import raise_error
 
 
-class StyleQGAN(object):
+class StyleQGAN:
     """Model that implements and trains a style-based quantum generative adversarial network.
 
     For original manuscript: `arXiv:2110.06933 <https://arxiv.org/abs/2110.06933>`_
 
     Args:
         latent_dim (int): number of latent dimensions.
         layers (int): number of layers for the quantum generator. Provide this value only if not using
@@ -38,107 +40,167 @@
             s3 = np.reshape(z, (samples,1))
             reference_distribution = np.hstack((s1,s2,s3))
             # Train qGAN with your particular setup
             train_qGAN = StyleQGAN(latent_dim=1, layers=2)
             train_qGAN.fit(reference_distribution, n_epochs=1)
     """
 
-    def __init__(self, latent_dim, layers=None, circuit=None, set_parameters=None, discriminator=None):
+    def __init__(
+        self,
+        latent_dim,
+        layers=None,
+        circuit=None,
+        set_parameters=None,
+        discriminator=None,
+    ):
         # qgan works only with tensorflow
         from qibo.backends import TensorflowBackend
+
         self.backend = TensorflowBackend()
 
         if layers is not None and circuit is not None:
-            raise_error(ValueError, "Set the number of layers for the default quantum generator "
-                        "or use a custom quantum generator, do not define both.")
+            raise_error(
+                ValueError,
+                "Set the number of layers for the default quantum generator "
+                "or use a custom quantum generator, do not define both.",
+            )
         elif layers is None and circuit is None:
-            raise_error(ValueError, "Set the number of layers for the default quantum generator "
-                        "or use a custom quantum generator.")
+            raise_error(
+                ValueError,
+                "Set the number of layers for the default quantum generator "
+                "or use a custom quantum generator.",
+            )
 
         if set_parameters is None and circuit is not None:
-            raise_error(ValueError, "Set parameters function has to be given for your custom quantum generator.")
+            raise_error(
+                ValueError,
+                "Set parameters function has to be given for your custom quantum generator.",
+            )
         elif set_parameters is not None and circuit is None:
-            raise_error(ValueError, "Define the custom quantum generator to use custom set parameters function.")
+            raise_error(
+                ValueError,
+                "Define the custom quantum generator to use custom set parameters function.",
+            )
 
         self.discriminator = discriminator
         self.circuit = circuit
         self.layers = layers
         self.latent_dim = latent_dim
         if set_parameters is not None:
             self.set_parameters = set_parameters
         else:
             self.set_parameters = self.set_params
 
     def define_discriminator(self, alpha=0.2, dropout=0.2):
         """Define the standalone discriminator model."""
+        from tensorflow.keras.layers import (  # pylint: disable=E0611,E0401
+            Conv2D,
+            Dense,
+            Dropout,
+            Flatten,
+            LeakyReLU,
+            Reshape,
+        )
         from tensorflow.keras.models import Sequential  # pylint: disable=E0611,E0401
         from tensorflow.keras.optimizers import Adadelta  # pylint: disable=E0611,E0401
-        from tensorflow.keras.layers import Dense, Conv2D, Dropout, Reshape, LeakyReLU, Flatten  # pylint: disable=E0611,E0401
 
         model = Sequential()
         model.add(Dense(200, use_bias=False, input_dim=self.nqubits))
-        model.add(Reshape((10,10,2)))
-        model.add(Conv2D(64, kernel_size=3, strides=1, padding='same', kernel_initializer='glorot_normal'))
+        model.add(Reshape((10, 10, 2)))
+        model.add(
+            Conv2D(
+                64,
+                kernel_size=3,
+                strides=1,
+                padding="same",
+                kernel_initializer="glorot_normal",
+            )
+        )
         model.add(LeakyReLU(alpha=alpha))
-        model.add(Conv2D(32, kernel_size=3, strides=1, padding='same', kernel_initializer='glorot_normal'))
+        model.add(
+            Conv2D(
+                32,
+                kernel_size=3,
+                strides=1,
+                padding="same",
+                kernel_initializer="glorot_normal",
+            )
+        )
         model.add(LeakyReLU(alpha=alpha))
-        model.add(Conv2D(16, kernel_size=3, strides=1, padding='same', kernel_initializer='glorot_normal'))
+        model.add(
+            Conv2D(
+                16,
+                kernel_size=3,
+                strides=1,
+                padding="same",
+                kernel_initializer="glorot_normal",
+            )
+        )
         model.add(LeakyReLU(alpha=alpha))
-        model.add(Conv2D(8, kernel_size=3, strides=1, padding='same', kernel_initializer='glorot_normal'))
+        model.add(
+            Conv2D(
+                8,
+                kernel_size=3,
+                strides=1,
+                padding="same",
+                kernel_initializer="glorot_normal",
+            )
+        )
         model.add(Flatten())
         model.add(LeakyReLU(alpha=alpha))
         model.add(Dropout(dropout))
-        model.add(Dense(1, activation='sigmoid'))
+        model.add(Dense(1, activation="sigmoid"))
 
         # compile model
         opt = Adadelta(learning_rate=0.1)
-        model.compile(loss='binary_crossentropy', optimizer=opt, metrics=['accuracy'])
+        model.compile(loss="binary_crossentropy", optimizer=opt, metrics=["accuracy"])
         return model
 
     def set_params(self, circuit, params, x_input, i):
         """Set the parameters for the quantum generator circuit."""
         p = []
         index = 0
         noise = 0
         for l in range(self.layers):
             for q in range(self.nqubits):
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%self.latent_dim
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%self.latent_dim
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%self.latent_dim
-            for i in range(0, self.nqubits-1):
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%self.latent_dim
-            p.append(params[index]*x_input[noise][i] + params[index+1])
-            index+=2
-            noise=(noise+1)%self.latent_dim
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % self.latent_dim
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % self.latent_dim
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % self.latent_dim
+            for i in range(0, self.nqubits - 1):
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % self.latent_dim
+            p.append(params[index] * x_input[noise][i] + params[index + 1])
+            index += 2
+            noise = (noise + 1) % self.latent_dim
         for q in range(self.nqubits):
-            p.append(params[index]*x_input[noise][i] + params[index+1])
-            index+=2
-            noise=(noise+1)%self.latent_dim
+            p.append(params[index] * x_input[noise][i] + params[index + 1])
+            index += 2
+            noise = (noise + 1) % self.latent_dim
         circuit.set_parameters(p)
 
     def generate_latent_points(self, samples):
         """Generate points in latent space as input for the quantum generator."""
         # generate points in the latent space
         x_input = randn(self.latent_dim * samples)
         # reshape into a batch of inputs for the network
         x_input = x_input.reshape(samples, self.latent_dim)
         return x_input
 
     def generate_fake_samples(self, params, samples, circuit, hamiltonians_list):
         import tensorflow as tf
+
         """Use the generator to generate fake examples, with class labels."""
         # generate points in latent space
         x_input = self.generate_latent_points(samples)
         x_input = np.transpose(x_input)
         # generator outputs
         X = []
         for i in range(self.nqubits):
@@ -151,19 +213,24 @@
                 X[ii].append(hamiltonians_list[ii].expectation(final_state))
         # shape array
         X = tf.stack([X[i] for i in range(len(X))], axis=1)
         # create class labels
         y = np.zeros((samples, 1))
         return X, y
 
-    def define_cost_gan(self, params, discriminator, samples, circuit, hamiltonians_list):
+    def define_cost_gan(
+        self, params, discriminator, samples, circuit, hamiltonians_list
+    ):
         import tensorflow as tf
+
         """Define the combined generator and discriminator model, for updating the generator."""
         # generate fake samples
-        x_fake, y_fake = self.generate_fake_samples(params, samples, circuit, hamiltonians_list)
+        x_fake, y_fake = self.generate_fake_samples(
+            params, samples, circuit, hamiltonians_list
+        )
         # create inverted labels for the fake samples
         y_fake = np.ones((samples, 1))
         # evaluate discriminator on fake examples
         disc_output = discriminator(x_fake)
         loss = tf.keras.losses.binary_crossentropy(y_fake, disc_output)
         loss = tf.reduce_mean(loss)
         return loss
@@ -172,15 +239,15 @@
         """Train the quantum generator and classical discriminator."""
         import tensorflow as tf
 
         def generate_real_samples(samples, distribution, real_samples):
             """Generate real samples with class labels."""
             # generate samples from the distribution
             idx = np.random.randint(real_samples, size=samples)
-            X = distribution[idx,:]
+            X = distribution[idx, :]
             # generate class labels
             y = np.ones((samples, 1))
             return X, y
 
         d_loss = []
         g_loss = []
         # determine half the size of one batch, for updating the discriminator
@@ -192,39 +259,63 @@
             initial_params = tf.Variable(np.random.uniform(-0.15, 0.15, n))
         optimizer = tf.optimizers.Adadelta(learning_rate=self.lr)
         # prepare real samples
         s = self.reference
         # manually enumerate epochs
         for i in range(self.n_epochs):
             # prepare real samples
-            x_real, y_real = generate_real_samples(half_samples, s, self.training_samples)
+            x_real, y_real = generate_real_samples(
+                half_samples, s, self.training_samples
+            )
             # prepare fake examples
-            x_fake, y_fake = self.generate_fake_samples(initial_params, half_samples, circuit, hamiltonians_list)
+            x_fake, y_fake = self.generate_fake_samples(
+                initial_params, half_samples, circuit, hamiltonians_list
+            )
             # update discriminator
             d_loss_real, _ = d_model.train_on_batch(x_real, y_real)
             d_loss_fake, _ = d_model.train_on_batch(x_fake, y_fake)
-            d_loss.append((d_loss_real + d_loss_fake)/2)
+            d_loss.append((d_loss_real + d_loss_fake) / 2)
             # update generator
             with tf.GradientTape() as tape:
-                loss = self.define_cost_gan(initial_params, d_model, self.batch_samples, circuit, hamiltonians_list)
+                loss = self.define_cost_gan(
+                    initial_params,
+                    d_model,
+                    self.batch_samples,
+                    circuit,
+                    hamiltonians_list,
+                )
             grads = tape.gradient(loss, initial_params)
             optimizer.apply_gradients([(grads, initial_params)])
             g_loss.append(loss)
             if save:  # pragma: no cover
                 # saving is skipped in tests to avoid creating files
-                params = (self.nqubits, self.latent_dim, self.layers,
-                          self.training_samples, self.batch_samples, self.lr)
+                params = (
+                    self.nqubits,
+                    self.latent_dim,
+                    self.layers,
+                    self.training_samples,
+                    self.batch_samples,
+                    self.lr,
+                )
                 filename = "_".join(str(p) for p in params)
-                np.savetxt(f"PARAMS_{filename}", [initial_params.numpy()], newline='')
-                np.savetxt(f"dloss_{filename}", [d_loss], newline='')
-                np.savetxt(f"gloss_{filename}", [g_loss], newline='')
+                np.savetxt(f"PARAMS_{filename}", [initial_params.numpy()], newline="")
+                np.savetxt(f"dloss_{filename}", [d_loss], newline="")
+                np.savetxt(f"gloss_{filename}", [g_loss], newline="")
                 # serialize weights to HDF5
                 d_model.save_weights(f"discriminator_{filename}.h5")
 
-    def fit(self, reference, initial_params=None, batch_samples=128, n_epochs=20000, lr=0.5, save=True):
+    def fit(
+        self,
+        reference,
+        initial_params=None,
+        batch_samples=128,
+        n_epochs=20000,
+        lr=0.5,
+        save=True,
+    ):
         """Execute qGAN training.
 
         Args:
             reference (array): samples from the reference input distribution.
             initial_parameters (array): initial parameters for the quantum generator. If not provided,
                 the default initial parameters will be used.
             discriminator (:class:`tensorflow.keras.models`): custom classical discriminator. If not provided,
@@ -233,17 +324,23 @@
             n_epochs (int): number of training iterations.
             lr (float): initial learning rate for the quantum generator.
                 It controls how much to change the model each time the weights are updated.
             save (bool): If ``True`` the results of training (trained parameters and losses)
                 will be saved on disk. Default is ``True``.
         """
         if initial_params is None and self.circuit is not None:
-            raise_error(ValueError, "Set the initial parameters for your custom quantum generator.")
+            raise_error(
+                ValueError,
+                "Set the initial parameters for your custom quantum generator.",
+            )
         elif initial_params is not None and self.circuit is None:
-            raise_error(ValueError, "Define the custom quantum generator to use custom initial parameters.")
+            raise_error(
+                ValueError,
+                "Define the custom quantum generator to use custom initial parameters.",
+            )
 
         self.reference = reference
         self.nqubits = reference.shape[1]
         self.training_samples = reference.shape[0]
         self.initial_params = initial_params
         self.batch_samples = batch_samples
         self.n_epochs = n_epochs
@@ -252,51 +349,57 @@
         # create classical discriminator
         if self.discriminator is None:
             discriminator = self.define_discriminator()
         else:
             discriminator = self.discriminator
 
         if discriminator.input_shape[1] is not self.nqubits:
-                raise_error(ValueError, "The number of input neurons in the discriminator has to be equal to "
-                            "the number of qubits in the circuit (dimension of the input reference distribution).")
+            raise_error(
+                ValueError,
+                "The number of input neurons in the discriminator has to be equal to "
+                "the number of qubits in the circuit (dimension of the input reference distribution).",
+            )
 
         # create quantum generator
         if self.circuit is None:
             circuit = models.Circuit(self.nqubits)
             for l in range(self.layers):
                 for q in range(self.nqubits):
                     circuit.add(gates.RY(q, 0))
                     circuit.add(gates.RZ(q, 0))
                     circuit.add(gates.RY(q, 0))
                     circuit.add(gates.RZ(q, 0))
-                for i in range(0, self.nqubits-1):
-                    circuit.add(gates.CRY(i, i+1, 0))
-                circuit.add(gates.CRY(self.nqubits-1, 0, 0))
+                for i in range(0, self.nqubits - 1):
+                    circuit.add(gates.CRY(i, i + 1, 0))
+                circuit.add(gates.CRY(self.nqubits - 1, 0, 0))
             for q in range(self.nqubits):
                 circuit.add(gates.RY(q, 0))
         else:
             circuit = self.circuit
 
         if circuit.nqubits != self.nqubits:
-                raise_error(ValueError, "The number of qubits in the circuit has to be equal to "
-                            "the number of dimensions in the reference distribution.")
+            raise_error(
+                ValueError,
+                "The number of qubits in the circuit has to be equal to "
+                "the number of dimensions in the reference distribution.",
+            )
 
         # define hamiltonian to generate fake samples
         def hamiltonian(nqubits, position):
             kron = []
             for i in range(nqubits):
                 if i == position:
                     kron.append(matrices.Z)
                 else:
                     kron.append(matrices.I)
             for i in range(nqubits - 1):
-                if i==0:
-                    ham = np.kron(kron[i+1], kron[i])
+                if i == 0:
+                    ham = np.kron(kron[i + 1], kron[i])
                 else:
-                    ham = np.kron(kron[i+1], ham)
+                    ham = np.kron(kron[i + 1], ham)
             return hamiltonians.Hamiltonian(nqubits, ham, backend=self.backend)
 
         hamiltonians_list = []
         for i in range(self.nqubits):
             hamiltonians_list.append(hamiltonian(self.nqubits, i))
 
         # train model
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/tsp.py` & `qibo-0.1.9/src/qibo/models/tsp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 import numpy as np
+
 from qibo import gates
-from qibo.symbols import X, Y, Z
-from qibo.models import Circuit
 from qibo.hamiltonians import SymbolicHamiltonian
+from qibo.models.circuit import Circuit
+from qibo.symbols import X, Y, Z
 
 
 def calculate_two_to_one(num_cities):
-    return np.arange(num_cities ** 2).reshape(num_cities, num_cities)
+    return np.arange(num_cities**2).reshape(num_cities, num_cities)
 
 
 def tsp_phaser(distance_matrix, backend=None):
     num_cities = distance_matrix.shape[0]
     two_to_one = calculate_two_to_one(num_cities)
     form = 0
     for i in range(num_cities):
         for u in range(num_cities):
             for v in range(num_cities):
                 if u != v:
-                    form += distance_matrix[u, v] * Z(int(two_to_one[u, i]))* Z(
-                        int(two_to_one[v, (i + 1) % num_cities]))
+                    form += (
+                        distance_matrix[u, v]
+                        * Z(int(two_to_one[u, i]))
+                        * Z(int(two_to_one[v, (i + 1) % num_cities]))
+                    )
     ham = SymbolicHamiltonian(form, backend=backend)
     return ham
 
 
 def tsp_mixer(num_cities, backend=None):
     two_to_one = calculate_two_to_one(num_cities)
     splus = lambda u, i: X(int(two_to_one[u, i])) + 1j * Y(int(two_to_one[u, i]))
     sminus = lambda u, i: X(int(two_to_one[u, i])) - 1j * Y(int(two_to_one[u, i]))
     form = 0
     for i in range(num_cities):
         for u in range(num_cities):
             for v in range(num_cities):
                 if u != v:
-                    form += splus(u, i) * splus(v, (i + 1) % num_cities) * sminus(u, (
-                            i + 1) % num_cities) * sminus(v, i) + sminus(u, i) * sminus(v, (
-                            i + 1) % num_cities) * splus(u, (i + 1) % num_cities) * splus(
-                        v, i)
+                    form += splus(u, i) * splus(v, (i + 1) % num_cities) * sminus(
+                        u, (i + 1) % num_cities
+                    ) * sminus(v, i) + sminus(u, i) * sminus(
+                        v, (i + 1) % num_cities
+                    ) * splus(
+                        u, (i + 1) % num_cities
+                    ) * splus(
+                        v, i
+                    )
     ham = SymbolicHamiltonian(form, backend=backend)
     return ham
 
 
 class TSP:
     """
     The travelling salesman problem (also called the travelling salesperson problem or TSP)
@@ -124,30 +133,33 @@
             qaoa_function_of_layer(2, distance_matrix)
 
     """
 
     def __init__(self, distance_matrix, backend=None):
         if backend is None:  # pragma: no cover
             from qibo.backends import GlobalBackend
+
             self.backend = GlobalBackend()
         else:
             self.backend = backend
         self.distance_matrix = distance_matrix
         self.num_cities = distance_matrix.shape[0]
         self.two_to_one = calculate_two_to_one(self.num_cities)
 
     def hamiltonians(self):
         """
         Returns:
             The pair of Hamiltonian describes the phaser hamiltonian
             and the mixer hamiltonian.
 
         """
-        return (tsp_phaser(self.distance_matrix, backend=self.backend),
-                tsp_mixer(self.num_cities, backend=self.backend))
+        return (
+            tsp_phaser(self.distance_matrix, backend=self.backend),
+            tsp_mixer(self.num_cities, backend=self.backend),
+        )
 
     def prepare_initial_state(self, ordering):
         """
         To run QAOA by Hadsfield, we need to start from a valid permutation function to ensure feasibility.
 
         Args:
             ordering (array): A list describing permutation from 0 to n-1
```

### Comparing `qibo-0.1.8rc0/src/qibo/models/variational.py` & `qibo-0.1.9/src/qibo/models/variational.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from qibo.config import raise_error
 from qibo.models.circuit import Circuit
 from qibo.models.evolution import StateEvolution
 
 
-class VQE(object):
+class VQE:
     """This class implements the variational quantum eigensolver algorithm.
 
     Args:
         circuit (:class:`qibo.models.circuit.Circuit`): Circuit that
             implements the variaional ansatz.
         hamiltonian (:class:`qibo.hamiltonians.Hamiltonian`): Hamiltonian object.
 
@@ -23,24 +23,37 @@
             hamiltonian = hamiltonians.XXZ(2)
             # create VQE model for the circuit and Hamiltonian
             vqe = models.VQE(circuit, hamiltonian)
             # optimize using random initial variational parameters
             initial_parameters = np.random.uniform(0, 2, 1)
             vqe.minimize(initial_parameters)
     """
+
     from qibo import optimizers
 
     def __init__(self, circuit, hamiltonian):
         """Initialize circuit ansatz and hamiltonian."""
         self.circuit = circuit
         self.hamiltonian = hamiltonian
 
-    def minimize(self, initial_state, method='Powell', jac=None, hess=None,
-                 hessp=None, bounds=None, constraints=(), tol=None, callback=None,
-                 options=None, compile=False, processes=None):
+    def minimize(
+        self,
+        initial_state,
+        method="Powell",
+        jac=None,
+        hess=None,
+        hessp=None,
+        bounds=None,
+        constraints=(),
+        tol=None,
+        callback=None,
+        options=None,
+        compile=False,
+        processes=None,
+    ):
         """Search for parameters which minimizes the hamiltonian expectation.
 
         Args:
             initial_state (array): a initial guess for the parameters of the
                 variational circuit.
             method (str): the desired minimization method.
                 See :meth:`qibo.optimizers.optimize` for available optimization
@@ -60,45 +73,56 @@
         Return:
             The final expectation value.
             The corresponding best parameters.
             The optimization result object. For scipy methods it returns
             the ``OptimizeResult``, for ``'cma'`` the ``CMAEvolutionStrategy.result``,
             and for ``'sgd'`` the options used during the optimization.
         """
+
         def _loss(params, circuit, hamiltonian):
             circuit.set_parameters(params)
             result = hamiltonian.backend.execute_circuit(circuit)
             final_state = result.state()
             return hamiltonian.expectation(final_state)
 
         if compile:
             loss = self.hamiltonian.backend.compile(_loss)
         else:
             loss = _loss
 
         if method == "cma":
-            #TODO: check if we can use this shortcut
+            # TODO: check if we can use this shortcut
             # dtype = getattr(self.hamiltonian.backend.np, self.hamiltonian.backend._dtypes.get('DTYPE'))
             dtype = self.hamiltonian.backend.np.float64
             loss = lambda p, c, h: dtype(_loss(p, c, h))
         elif method != "sgd":
             loss = lambda p, c, h: self.hamiltonian.backend.to_numpy(_loss(p, c, h))
 
-        result, parameters, extra = self.optimizers.optimize(loss, initial_state,
-                                                             args=(self.circuit, self.hamiltonian),
-                                                             method=method, jac=jac, hess=hess, hessp=hessp,
-                                                             bounds=bounds, constraints=constraints,
-                                                             tol=tol, callback=callback, options=options,
-                                                             compile=compile, processes=processes,
-                                                             backend=self.hamiltonian.backend)
+        result, parameters, extra = self.optimizers.optimize(
+            loss,
+            initial_state,
+            args=(self.circuit, self.hamiltonian),
+            method=method,
+            jac=jac,
+            hess=hess,
+            hessp=hessp,
+            bounds=bounds,
+            constraints=constraints,
+            tol=tol,
+            callback=callback,
+            options=options,
+            compile=compile,
+            processes=processes,
+            backend=self.hamiltonian.backend,
+        )
         self.circuit.set_parameters(parameters)
         return result, parameters, extra
 
 
-class AAVQE(object):
+class AAVQE:
     """This class implements the Adiabatically Assisted Variational Quantum Eigensolver
     algorithm. See https://arxiv.org/abs/1806.02287.
 
     Args:
         circuit (:class:`qibo.models.circuit.Circuit`): variational ansatz.
         easy_hamiltonian (:class:`qibo.hamiltonians.Hamiltonian`): initial Hamiltonian object.
         problem_hamiltonian (:class:`qibo.hamiltonians.Hamiltonian`): problem Hamiltonian object.
@@ -129,77 +153,117 @@
                                 s, nsteps=10, t_max=1)
             # optimize using random initial variational parameters
             np.random.seed(0)
             initial_parameters = np.random.uniform(0, 2*np.pi, 2)
             ground_energy, params = aavqe.minimize(initial_parameters)
     """
 
-    def __init__(self, circuit, easy_hamiltonian, problem_hamiltonian, s, nsteps=10, t_max = 1, bounds_tolerance = 1e-7, time_tolerance = 1e-7):
-
-        if nsteps <= 0: # pragma: no cover
-            raise_error(ValueError, "Number of steps nsteps should be positive but is {}."
-                                    "".format(nsteps))
-        if t_max <= 0: # pragma: no cover
-            raise_error(ValueError, "Maximum time t_max should be positive but is {}."
-                                    "".format(t_max))
-        if easy_hamiltonian.nqubits != problem_hamiltonian.nqubits: # pragma: no cover
-            raise_error(ValueError, "The easy Hamiltonian has {} qubits while problem Hamiltonian has {}."
-                                    "".format(easy_hamiltonian.nqubits, problem_hamiltonian.nqubits))
+    def __init__(
+        self,
+        circuit,
+        easy_hamiltonian,
+        problem_hamiltonian,
+        s,
+        nsteps=10,
+        t_max=1,
+        bounds_tolerance=1e-7,
+        time_tolerance=1e-7,
+    ):
+
+        if nsteps <= 0:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "Number of steps nsteps should be positive but is {}."
+                "".format(nsteps),
+            )
+        if t_max <= 0:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "Maximum time t_max should be positive but is {}." "".format(t_max),
+            )
+        if easy_hamiltonian.nqubits != problem_hamiltonian.nqubits:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "The easy Hamiltonian has {} qubits while problem Hamiltonian has {}."
+                "".format(easy_hamiltonian.nqubits, problem_hamiltonian.nqubits),
+            )
 
         self.ATOL = bounds_tolerance
         self.ATOL_TIME = time_tolerance
 
         self._circuit = circuit
         self._h0 = easy_hamiltonian
         self._h1 = problem_hamiltonian
         self._nsteps = nsteps
         self._t_max = t_max
-        self._dt = 1./(nsteps-1)
+        self._dt = 1.0 / (nsteps - 1)
 
         self._schedule = None
         nparams = s.__code__.co_argcount
-        if not nparams == 1: # pragma: no cover
-            raise_error(ValueError,"Scheduling function must take only one argument,"
-                                   "but the function proposed takes {}.".format(nparams))
+        if not nparams == 1:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "Scheduling function must take only one argument,"
+                "but the function proposed takes {}.".format(nparams),
+            )
         self.set_schedule(s)
 
     def set_schedule(self, func):
-        """ Set scheduling function s(t) as func."""
-        #check boundary conditions
+        """Set scheduling function s(t) as func."""
+        # check boundary conditions
         s0 = func(0)
-        if abs(s0) > self.ATOL: # pragma: no cover
+        if abs(s0) > self.ATOL:  # pragma: no cover
             raise_error(ValueError, "s(0) should be 0 but it is {}.".format(s0))
         s1 = func(1)
-        if abs(s1 - 1) > self.ATOL: # pragma: no cover
+        if abs(s1 - 1) > self.ATOL:  # pragma: no cover
             raise_error(ValueError, "s(1) should be 1 but it is {}.".format(s1))
         self._schedule = func
 
     def schedule(self, t):
-        """ Returns scheduling function evaluated at time t: s(t/Tmax)."""
-        if self._schedule is None: # pragma: no cover
+        """Returns scheduling function evaluated at time t: s(t/Tmax)."""
+        if self._schedule is None:  # pragma: no cover
             raise_error(ValueError, "Cannot access scheduling before it is set.")
-        if (t - self._t_max) > self.ATOL_TIME: # pragma: no cover
-            raise_error(ValueError, "t cannot be greater than {}, but it is {}.".format(self._t_max, t))
+        if (t - self._t_max) > self.ATOL_TIME:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "t cannot be greater than {}, but it is {}.".format(self._t_max, t),
+            )
 
         s = self._schedule(t / self._t_max)
-        if (abs(s) - 1) > self.ATOL: # pragma: no cover
-            raise_error(ValueError, "s cannot be greater than 1 but it is {}.".format(s))
+        if (abs(s) - 1) > self.ATOL:  # pragma: no cover
+            raise_error(
+                ValueError, "s cannot be greater than 1 but it is {}.".format(s)
+            )
         return s
 
     def hamiltonian(self, t):
         """Returns the adiabatic evolution Hamiltonian at a given time."""
-        if (t - self._t_max) > self.ATOL: # pragma: no cover
-            raise_error(ValueError, "t cannot be greater than {}, but it is {}.".format(self._t_max, t))
+        if (t - self._t_max) > self.ATOL:  # pragma: no cover
+            raise_error(
+                ValueError,
+                "t cannot be greater than {}, but it is {}.".format(self._t_max, t),
+            )
         # boundary conditions  s(0)=0, s(total_time)=1
         st = self.schedule(t)
         return self._h0 * (1 - st) + self._h1 * st
 
-    def minimize(self, params, method="BFGS", jac=None, hess=None,
-                 hessp=None, bounds=None, constraints=(), tol=None,
-                 options=None, compile=False, processes=None):
+    def minimize(
+        self,
+        params,
+        method="BFGS",
+        jac=None,
+        hess=None,
+        hessp=None,
+        bounds=None,
+        constraints=(),
+        tol=None,
+        options=None,
+        compile=False,
+        processes=None,
+    ):
         """
         Performs minimization to find the ground state of the problem Hamiltonian.
 
         Args:
             params (np.ndarray or list): initial guess for the parameters of the variational circuit.
             method (str): optimizer to employ.
             jac (dict): Method for computing the gradient vector for scipy optimizers.
@@ -210,27 +274,38 @@
             constraints (dict): Constraints definition for scipy optimizers.
             tol (float): Tolerance of termination for scipy optimizers.
             options (dict): a dictionary with options for the different optimizers.
             compile (bool): whether the TensorFlow graph should be compiled.
             processes (int): number of processes when using the parallel BFGS method.
         """
         from qibo import models
-        t = 0.
-        while (t-self._t_max)<=self.ATOL_TIME:
+
+        t = 0.0
+        while (t - self._t_max) <= self.ATOL_TIME:
             H = self.hamiltonian(t)
             vqe = models.VQE(self._circuit, H)
-            best, params, _ = vqe.minimize(params, method=method, jac=jac, hess=hess, hessp=hessp,
-                                        bounds=bounds, constraints=constraints, tol=tol,
-                                        options=options, compile=compile, processes=processes)
+            best, params, _ = vqe.minimize(
+                params,
+                method=method,
+                jac=jac,
+                hess=hess,
+                hessp=hessp,
+                bounds=bounds,
+                constraints=constraints,
+                tol=tol,
+                options=options,
+                compile=compile,
+                processes=processes,
+            )
             t += self._dt
         return best, params
 
 
-class QAOA(object):
-    """ Quantum Approximate Optimization Algorithm (QAOA) model.
+class QAOA:
+    """Quantum Approximate Optimization Algorithm (QAOA) model.
 
     The QAOA is introduced in `arXiv:1411.4028 <https://arxiv.org/abs/1411.4028>`_.
 
     Args:
         hamiltonian (:class:`qibo.hamiltonians.Hamiltonian`): problem Hamiltonian
             whose ground state is sought.
         mixer (:class:`qibo.hamiltonians.Hamiltonian`): mixer Hamiltonian.
@@ -253,69 +328,86 @@
             # create QAOA model for this Hamiltonian
             qaoa = models.QAOA(hamiltonian)
             # optimize using random initial variational parameters
             # and default options and initial state
             initial_parameters = 0.01 * np.random.random(4)
             best_energy, final_parameters, extra = qaoa.minimize(initial_parameters, method="BFGS")
     """
+
     from qibo import hamiltonians, optimizers
 
-    def __init__(self, hamiltonian, mixer=None, solver="exp", callbacks=[],
-                 accelerators=None):
+    def __init__(
+        self, hamiltonian, mixer=None, solver="exp", callbacks=[], accelerators=None
+    ):
         from qibo.hamiltonians.abstract import AbstractHamiltonian
+
         # list of QAOA variational parameters (angles)
         self.params = None
         # problem hamiltonian
         if not isinstance(hamiltonian, AbstractHamiltonian):
-            raise_error(TypeError, "Invalid Hamiltonian type {}."
-                                   "".format(type(hamiltonian)))
+            raise_error(
+                TypeError, "Invalid Hamiltonian type {}." "".format(type(hamiltonian))
+            )
         self.hamiltonian = hamiltonian
         self.nqubits = hamiltonian.nqubits
         # mixer hamiltonian (default = -sum(sigma_x))
         if mixer is None:
             trotter = isinstance(
-                self.hamiltonian, self.hamiltonians.SymbolicHamiltonian)
-            self.mixer = self.hamiltonians.X(self.nqubits, dense=not trotter,
-                                             backend=self.hamiltonian.backend)
+                self.hamiltonian, self.hamiltonians.SymbolicHamiltonian
+            )
+            self.mixer = self.hamiltonians.X(
+                self.nqubits, dense=not trotter, backend=self.hamiltonian.backend
+            )
         else:
             if type(mixer) != type(hamiltonian):
-                  raise_error(TypeError, "Given Hamiltonian is of type {} "
-                                         "while mixer is of type {}."
-                                         "".format(type(hamiltonian),
-                                                   type(mixer)))
+                raise_error(
+                    TypeError,
+                    "Given Hamiltonian is of type {} "
+                    "while mixer is of type {}."
+                    "".format(type(hamiltonian), type(mixer)),
+                )
             if mixer.nqubits != hamiltonian.nqubits:
-                  raise_error(ValueError, "Given Hamiltonian acts on {} qubits "
-                                          "while mixer acts on {}."
-                                          "".format(hamiltonian.nqubits,
-                                                    mixer.nqubits))
+                raise_error(
+                    ValueError,
+                    "Given Hamiltonian acts on {} qubits "
+                    "while mixer acts on {}."
+                    "".format(hamiltonian.nqubits, mixer.nqubits),
+                )
             self.mixer = mixer
 
         # create circuits for Trotter Hamiltonians
-        if (accelerators is not None and (
+        if accelerators is not None and (
             not isinstance(self.hamiltonian, self.hamiltonians.SymbolicHamiltonian)
-            or solver != "exp")):
-            raise_error(NotImplementedError, "Distributed QAOA is implemented "
-                                             "only with SymbolicHamiltonian and "
-                                             "exponential solver.")
+            or solver != "exp"
+        ):
+            raise_error(
+                NotImplementedError,
+                "Distributed QAOA is implemented "
+                "only with SymbolicHamiltonian and "
+                "exponential solver.",
+            )
         if isinstance(self.hamiltonian, self.hamiltonians.SymbolicHamiltonian):
             self.hamiltonian.circuit(1e-2, accelerators)
             self.mixer.circuit(1e-2, accelerators)
 
         # evolution solvers
         from qibo.solvers import get_solver
+
         self.ham_solver = get_solver(solver, 1e-2, self.hamiltonian)
         self.mix_solver = get_solver(solver, 1e-2, self.mixer)
 
         self.callbacks = callbacks
-        self.backend = hamiltonian.backend # to avoid error with _create_calculate_callbacks
+        self.backend = (
+            hamiltonian.backend
+        )  # to avoid error with _create_calculate_callbacks
         self.accelerators = accelerators
-        self.normalize_state = StateEvolution._create_normalize_state(
-            self, solver)
-        self.calculate_callbacks = StateEvolution._create_calculate_callbacks(self,
-            accelerators)
+        self.normalize_state = StateEvolution._create_normalize_state(self, solver)
+        self.calculate_callbacks = StateEvolution._create_calculate_callbacks(
+            self, accelerators
+        )
 
     def set_parameters(self, p):
         """Sets the variational parameters.
 
         Args:
             p (np.ndarray): 1D-array holding the new values for the variational
                 parameters. Length should be an even number.
@@ -344,27 +436,38 @@
             state = self.hamiltonian.backend.plus_state(self.nqubits)
         else:
             state = self.hamiltonian.backend.cast(initial_state)
 
         self.calculate_callbacks(state)
         n = int(self.params.shape[0])
         for i in range(n // 2):
-            state = self._apply_exp(state, self.ham_solver,
-                                    self.params[2 * i])
-            state = self._apply_exp(state, self.mix_solver,
-                                    self.params[2 * i + 1])
+            state = self._apply_exp(state, self.ham_solver, self.params[2 * i])
+            state = self._apply_exp(state, self.mix_solver, self.params[2 * i + 1])
         return self.normalize_state(state)
 
     def __call__(self, initial_state=None):
         """Equivalent to :meth:`qibo.models.QAOA.execute`."""
         return self.execute(initial_state)
 
-    def minimize(self, initial_p, initial_state=None, method='Powell',
-                 jac=None, hess=None, hessp=None, bounds=None, constraints=(),
-                 tol=None, callback=None, options=None, compile=False, processes=None):
+    def minimize(
+        self,
+        initial_p,
+        initial_state=None,
+        method="Powell",
+        jac=None,
+        hess=None,
+        hessp=None,
+        bounds=None,
+        constraints=(),
+        tol=None,
+        callback=None,
+        options=None,
+        compile=False,
+        processes=None,
+    ):
         """Optimizes the variational parameters of the QAOA.
 
         Args:
             initial_p (np.ndarray): initial guess for the parameters.
             initial_state (np.ndarray): initial state vector of the QAOA.
             method (str): the desired minimization method.
                 See :meth:`qibo.optimizers.optimize` for available optimization
@@ -386,43 +489,58 @@
             The corresponding best parameters.
             The optimization result object. For scipy methods it
             returns the ``OptimizeResult``, for ``'cma'`` the
             ``CMAEvolutionStrategy.result``, and for ``'sgd'``
             the options used during the optimization.
         """
         if len(initial_p) % 2 != 0:
-            raise_error(ValueError, "Initial guess for the parameters must "
-                                    "contain an even number of values but "
-                                    "contains {}.".format(len(initial_p)))
+            raise_error(
+                ValueError,
+                "Initial guess for the parameters must "
+                "contain an even number of values but "
+                "contains {}.".format(len(initial_p)),
+            )
 
         def _loss(params, qaoa, hamiltonian, state):
             if state is not None:
                 state = hamiltonian.backend.cast(state, copy=True)
             qaoa.set_parameters(params)
             state = qaoa(state)
             return hamiltonian.expectation(state)
 
-
         if method == "sgd":
             loss = lambda p, c, h, s: _loss(self.hamiltonian.backend.cast(p), c, h, s)
         else:
-            loss = lambda p, c, h, s: self.hamiltonian.backend.to_numpy(_loss(p, c, h, s))
-
-        result, parameters, extra = self.optimizers.optimize(loss, initial_p, args=(self, self.hamiltonian, initial_state),
-                                                             method=method, jac=jac, hess=hess, hessp=hessp,
-                                                             bounds=bounds, constraints=constraints,
-                                                             tol=tol, callback=callback, options=options,
-                                                             compile=compile, processes=processes,
-                                                             backend=self.backend)
+            loss = lambda p, c, h, s: self.hamiltonian.backend.to_numpy(
+                _loss(p, c, h, s)
+            )
+
+        result, parameters, extra = self.optimizers.optimize(
+            loss,
+            initial_p,
+            args=(self, self.hamiltonian, initial_state),
+            method=method,
+            jac=jac,
+            hess=hess,
+            hessp=hessp,
+            bounds=bounds,
+            constraints=constraints,
+            tol=tol,
+            callback=callback,
+            options=options,
+            compile=compile,
+            processes=processes,
+            backend=self.backend,
+        )
         self.set_parameters(parameters)
         return result, parameters, extra
 
 
 class FALQON(QAOA):
-    """ Feedback-based ALgorithm for Quantum OptimizatioN (FALQON) model.
+    """Feedback-based ALgorithm for Quantum OptimizatioN (FALQON) model.
 
     The FALQON is introduced in `arXiv:2103.08619 <https://arxiv.org/abs/2103.08619>`_.
     It inherits the QAOA class.
 
     Args:
         hamiltonian (:class:`qibo.hamiltonians.Hamiltonian`): problem Hamiltonian
             whose ground state is sought.
@@ -447,20 +565,25 @@
             # optimize using random initial variational parameters
             # and default options and initial state
             delta_t = 0.01
             max_layers = 3
             best_energy, final_parameters, extra = falqon.minimize(delta_t, max_layers)
     """
 
-    def __init__(self, hamiltonian, mixer=None, solver="exp", callbacks=[],
-                 accelerators=None):
+    def __init__(
+        self, hamiltonian, mixer=None, solver="exp", callbacks=[], accelerators=None
+    ):
         super().__init__(hamiltonian, mixer, solver, callbacks, accelerators)
-        self.evol_hamiltonian = 1j * (self.hamiltonian @ self.mixer - self.mixer @ self.hamiltonian)
-
-    def minimize(self, delta_t, max_layers, initial_state=None, tol=None, callback=None):
+        self.evol_hamiltonian = 1j * (
+            self.hamiltonian @ self.mixer - self.mixer @ self.hamiltonian
+        )
+
+    def minimize(
+        self, delta_t, max_layers, initial_state=None, tol=None, callback=None
+    ):
         """Optimizes the variational parameters of the FALQON.
 
         Args:
             delta_t (float): initial guess for the time step. A too large delta_t will make the algorithm fail.
             max_layers (int): maximum number of layers allowed for the FALQON.
             initial_state (np.ndarray): initial state vector of the FALQON.
             tol (float): Tolerance of energy change. If not specified, no check is done.
@@ -469,33 +592,40 @@
 
         Return:
             The final energy (expectation value of the ``hamiltonian``).
             The corresponding best parameters.
             extra: variable with historical data for the energy and callbacks.
         """
         import numpy as np
+
         parameters = np.array([delta_t, 0])
 
         def _loss(params, falqon, hamiltonian):
             falqon.set_parameters(params)
             state = falqon(initial_state)
             return hamiltonian.expectation(state)
 
         energy = [np.inf]
         callback_result = []
         for it in range(1, max_layers + 1):
-            beta = self.hamiltonian.backend.to_numpy(_loss(parameters, self, self.evol_hamiltonian))
+            beta = self.hamiltonian.backend.to_numpy(
+                _loss(parameters, self, self.evol_hamiltonian)
+            )
 
             if tol is not None:
-                energy.append(self.hamiltonian.backend.to_numpy(_loss(parameters, self, self.hamiltonian)))
+                energy.append(
+                    self.hamiltonian.backend.to_numpy(
+                        _loss(parameters, self, self.hamiltonian)
+                    )
+                )
                 if abs(energy[-1] - energy[-2]) < tol:
                     break
 
             if callback is not None:
                 callback_result.append(callback(parameters))
 
             parameters = np.concatenate([parameters, [delta_t, delta_t * beta]])
 
         self.set_parameters(parameters)
         final_loss = _loss(parameters, self, self.hamiltonian)
-        extra = {'energies': energy, 'callbacks': callback_result}
+        extra = {"energies": energy, "callbacks": callback_result}
         return final_loss, parameters, extra
```

### Comparing `qibo-0.1.8rc0/src/qibo/noise.py` & `qibo-0.1.9/src/qibo/noise.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,109 +1,126 @@
 from qibo import gates
 
-class PauliError():
+
+class PauliError:
     """Quantum error associated with the :class:`qibo.gates.PauliNoiseChannel`.
 
-        Args:
-            options (tuple): see :class:`qibo.gates.PauliNoiseChannel`
+    Args:
+        options (tuple): see :class:`qibo.gates.PauliNoiseChannel`
     """
 
     def __init__(self, px=0, py=0, pz=0):
         self.options = px, py, pz
         self.channel = gates.PauliNoiseChannel
 
 
-class ThermalRelaxationError():
+class ThermalRelaxationError:
     """Quantum error associated with the :class:`qibo.gates.ThermalRelaxationChannel`.
 
-        Args:
-            options (tuple): see :class:`qibo.gates.ThermalRelaxationChannel`
+    Args:
+        options (tuple): see :class:`qibo.gates.ThermalRelaxationChannel`
     """
 
     def __init__(self, t1, t2, time, excited_population=0):
         self.options = t1, t2, time, excited_population
         self.channel = gates.ThermalRelaxationChannel
 
 
-class ResetError():
+class DepolarizingError:
+    """Quantum error associated with the :class:`qibo.gates.DepolarizingChannel`.
+
+    Args:
+        options (float): see :class:`qibo.gates.DepolarizingChannel`
+    """
+
+    def __init__(self, lam):
+        self.options = (lam,)
+        self.channel = gates.DepolarizingChannel
+
+
+class ResetError:
     """Quantum error associated with the `qibo.gates.ResetChannel`.
 
-        Args:
-            options (tuple): see :class:`qibo.gates.ResetChannel`
+    Args:
+        options (tuple): see :class:`qibo.gates.ResetChannel`
     """
 
     def __init__(self, p0, p1):
         self.options = p0, p1
         self.channel = gates.ResetChannel
 
 
-class NoiseModel():
+class NoiseModel:
     """Class for the implementation of a custom noise model.
 
-        Example:
+    Example:
 
-        .. testcode::
+    .. testcode::
 
-            from qibo import models, gates
-            from qibo.noise import NoiseModel, PauliError
+        from qibo import models, gates
+        from qibo.noise import NoiseModel, PauliError
 
-            # Build specific noise model with 2 quantum errors:
-            # - Pauli error on H only for qubit 1.
-            # - Pauli error on CNOT for all the qubits.
-            noise = NoiseModel()
-            noise.add(PauliError(px = 0.5), gates.H, 1)
-            noise.add(PauliError(py = 0.5), gates.CNOT)
-
-            # Generate noiseless circuit.
-            c = models.Circuit(2)
-            c.add([gates.H(0), gates.H(1), gates.CNOT(0, 1)])
+        # Build specific noise model with 2 quantum errors:
+        # - Pauli error on H only for qubit 1.
+        # - Pauli error on CNOT for all the qubits.
+        noise = NoiseModel()
+        noise.add(PauliError(px = 0.5), gates.H, 1)
+        noise.add(PauliError(py = 0.5), gates.CNOT)
+
+        # Generate noiseless circuit.
+        c = models.Circuit(2)
+        c.add([gates.H(0), gates.H(1), gates.CNOT(0, 1)])
 
-            # Apply noise to the circuit according to the noise model.
-            noisy_c = noise.apply(c)
+        # Apply noise to the circuit according to the noise model.
+        noisy_c = noise.apply(c)
     """
 
     def __init__(self):
         self.errors = {}
 
     def add(self, error, gate, qubits=None):
         """Add a quantum error for a specific gate and qubit to the noise model.
 
-            Args:
-                error: quantum error to associate with the gate. Possible choices
-                       are :class:`qibo.noise.PauliError`,
-                       :class:`qibo.noise.ThermalRelaxationError` and
-                       :class:`qibo.noise.ResetError`.
-                gate (:class:`qibo.gates.Gate`): gate after which the noise will be added.
-                qubits (tuple): qubits where the noise will be applied, if None the noise
-                                will be added after every instance of the gate.
+        Args:
+            error: quantum error to associate with the gate. Possible choices
+                   are :class:`qibo.noise.PauliError`,
+                   :class:`qibo.noise.ThermalRelaxationError`,
+                   :class:`qibo.noise.DepolarizingError` and
+                   :class:`qibo.noise.ResetError`.
+            gate (:class:`qibo.gates.Gate`): gate after which the noise will be added.
+            qubits (tuple): qubits where the noise will be applied, if None the noise
+                            will be added after every instance of the gate.
         """
 
         if isinstance(qubits, int):
-            qubits = (qubits, )
+            qubits = (qubits,)
 
         self.errors[gate] = (error, qubits)
 
     def apply(self, circuit):
         """Generate a noisy quantum circuit according to the noise model built.
 
-            Args:
-                circuit (:class:`qibo.models.circuit.Circuit`): quantum circuit
+        Args:
+            circuit (:class:`qibo.models.circuit.Circuit`): quantum circuit
 
-            Returns:
-                A (:class:`qibo.models.circuit.Circuit`) which corresponds
-                to the initial circuit with noise gates added according
-                to the noise model.
+        Returns:
+            A (:class:`qibo.models.circuit.Circuit`) which corresponds
+            to the initial circuit with noise gates added according
+            to the noise model.
         """
         noisy_circuit = circuit.__class__(**circuit.init_kwargs)
         for gate in circuit.queue:
             noisy_circuit.add(gate)
             if gate.__class__ in self.errors:
                 error, qubits = self.errors.get(gate.__class__)
                 if qubits is None:
                     qubits = gate.qubits
                 else:
                     qubits = tuple(set(gate.qubits) & set(qubits))
-                for q in qubits:
-                    noisy_circuit.add(error.channel(q, *error.options))
+                if isinstance(error, DepolarizingError) and qubits:
+                    noisy_circuit.add(error.channel(qubits, *error.options))
+                else:
+                    for q in qubits:
+                        noisy_circuit.add(error.channel(q, *error.options))
         noisy_circuit.measurement_tuples = dict(circuit.measurement_tuples)
         noisy_circuit.measurement_gate = circuit.measurement_gate
         return noisy_circuit
```

### Comparing `qibo-0.1.8rc0/src/qibo/optimizers.py` & `qibo-0.1.9/src/qibo/optimizers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,24 @@
-
-
-def optimize(loss, initial_parameters, args=(), method='Powell',
-             jac=None, hess=None, hessp=None, bounds=None, constraints=(),
-             tol=None, callback=None, options=None, compile=False, processes=None, backend=None):
+def optimize(
+    loss,
+    initial_parameters,
+    args=(),
+    method="Powell",
+    jac=None,
+    hess=None,
+    hessp=None,
+    bounds=None,
+    constraints=(),
+    tol=None,
+    callback=None,
+    options=None,
+    compile=False,
+    processes=None,
+    backend=None,
+):
     """Main optimization method. Selects one of the following optimizers:
         - :meth:`qibo.optimizers.cmaes`
         - :meth:`qibo.optimizers.newtonian`
         - :meth:`qibo.optimizers.sgd`
 
     Args:
         loss (callable): Loss as a function of ``parameters`` and optional extra
@@ -64,23 +76,38 @@
             circuit.set_parameters(params)
     """
     if method == "cma":
         return cmaes(loss, initial_parameters, args, options)
     elif method == "sgd":
         if backend is None:
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
         return sgd(loss, initial_parameters, args, options, compile, backend)
     else:
         if backend is None:
             from qibo.backends import GlobalBackend
+
             backend = GlobalBackend()
-        return newtonian(loss, initial_parameters, args, method,
-                         jac, hess, hessp, bounds, constraints, tol,
-                         callback, options, processes, backend)
+        return newtonian(
+            loss,
+            initial_parameters,
+            args,
+            method,
+            jac,
+            hess,
+            hessp,
+            bounds,
+            constraints,
+            tol,
+            callback,
+            options,
+            processes,
+            backend,
+        )
 
 
 def cmaes(loss, initial_parameters, args=(), options=None):
     """Genetic optimizer based on `pycma <https://github.com/CMA-ES/pycma>`_.
 
     Args:
         loss (callable): Loss as a function of variational parameters to be
@@ -89,21 +116,35 @@
             parameters.
         args (tuple): optional arguments for the loss function.
         options (dict): Dictionary with options accepted by the ``cma``
             optimizer. The user can use ``import cma; cma.CMAOptions()`` to view the
             available options.
     """
     import cma
+
     r = cma.fmin2(loss, initial_parameters, 1.7, options=options, args=args)
     return r[1].result.fbest, r[1].result.xbest, r
 
 
-def newtonian(loss, initial_parameters, args=(), method='Powell',
-              jac=None, hess=None, hessp=None, bounds=None, constraints=(),
-              tol=None, callback=None, options=None, processes=None, backend=None):
+def newtonian(
+    loss,
+    initial_parameters,
+    args=(),
+    method="Powell",
+    jac=None,
+    hess=None,
+    hessp=None,
+    bounds=None,
+    constraints=(),
+    tol=None,
+    callback=None,
+    options=None,
+    processes=None,
+    backend=None,
+):
     """Newtonian optimization approaches based on ``scipy.optimize.minimize``.
 
     For more details check the `scipy documentation <https://docs.scipy.org/doc/scipy/reference/generated/scipy.optimize.minimize.html>`_.
 
     .. note::
         When using the method ``parallel_L-BFGS-B`` the ``processes`` option controls the
         number of processes used by the parallel L-BFGS-B algorithm through the ``multiprocessing`` library.
@@ -130,23 +171,41 @@
         constraints (dict): Constraints definition for scipy optimizers.
         tol (float): Tolerance of termination for scipy optimizers.
         callback (callable): Called after each iteration for scipy optimizers.
         options (dict): Dictionary with options accepted by
             ``scipy.optimize.minimize``.
         processes (int): number of processes when using the parallel BFGS method.
     """
-    if method == 'parallel_L-BFGS-B':  # pragma: no cover
-        o = ParallelBFGS(loss, args=args, processes=processes,
-                         bounds=bounds, callback=callback, options=options)
+    if method == "parallel_L-BFGS-B":  # pragma: no cover
+        o = ParallelBFGS(
+            loss,
+            args=args,
+            processes=processes,
+            bounds=bounds,
+            callback=callback,
+            options=options,
+        )
         m = o.run(initial_parameters)
     else:
         from scipy.optimize import minimize
-        m = minimize(loss, initial_parameters, args=args, method=method,
-                     jac=jac, hess=hess, hessp=hessp, bounds=bounds, constraints=constraints,
-                     tol=tol, callback=callback, options=options)
+
+        m = minimize(
+            loss,
+            initial_parameters,
+            args=args,
+            method=method,
+            jac=jac,
+            hess=hess,
+            hessp=hessp,
+            bounds=bounds,
+            constraints=constraints,
+            tol=tol,
+            callback=callback,
+            options=options,
+        )
     return m.fun, m.x, m
 
 
 def sgd(loss, initial_parameters, args=(), options=None, compile=False, backend=None):
     """Stochastic Gradient Descent (SGD) optimizer using Tensorflow backpropagation.
 
     See `tf.keras.Optimizers <https://www.tensorflow.org/api_docs/python/tf/keras/optimizers>`_
@@ -164,28 +223,32 @@
             - ``'optimizer'`` (str, default: ``'Adagrad'``): Name of optimizer.
             - ``'learning_rate'`` (float, default: ``'1e-3'``): Learning rate.
             - ``'nepochs'`` (int, default: ``1e6``): Number of epochs for optimization.
             - ``'nmessage'`` (int, default: ``1e3``): Every how many epochs to print
               a message of the loss function.
     """
     from qibo.config import log, raise_error
-    if not backend.name == 'tensorflow':
+
+    if not backend.name == "tensorflow":
         raise_error(RuntimeError, "SGD optimizer requires Tensorflow backend.")
 
-    sgd_options = {"nepochs": 1000000,
-                   "nmessage": 1000,
-                   "optimizer": "Adagrad",
-                   "learning_rate": 0.001}
+    sgd_options = {
+        "nepochs": 1000000,
+        "nmessage": 1000,
+        "optimizer": "Adagrad",
+        "learning_rate": 0.001,
+    }
     if options is not None:
         sgd_options.update(options)
 
     # proceed with the training
     vparams = backend.tf.Variable(initial_parameters)
     optimizer = getattr(backend.tf.optimizers, sgd_options["optimizer"])(
-        learning_rate=sgd_options["learning_rate"])
+        learning_rate=sgd_options["learning_rate"]
+    )
 
     def opt_step():
         with backend.tf.GradientTape() as tape:
             l = loss(vparams, *args)
         grads = tape.gradient(l, [vparams])
         optimizer.apply_gradients(zip(grads, [vparams]))
         return l
@@ -193,15 +256,15 @@
     if compile:
         loss = backend.compile(loss)
         opt_step = backend.compile(opt_step)
 
     for e in range(sgd_options["nepochs"]):
         l = opt_step()
         if e % sgd_options["nmessage"] == 1:
-            log.info('ite %d : loss %f', e, l.numpy())
+            log.info("ite %d : loss %f", e, l.numpy())
 
     return loss(vparams, *args).numpy(), vparams.numpy(), sgd_options
 
 
 class ParallelBFGS:  # pragma: no cover
     """Computes the L-BFGS-B using parallel evaluation using multiprocessing.
     This implementation here is based on https://doi.org/10.32614/RJ-2019-030.
@@ -210,18 +273,26 @@
         function (function): loss function which returns a numpy object.
         args (tuple): optional arguments for the loss function.
         bounds (list): list of bound values for ``scipy.optimize.minimize`` L-BFGS-B.
         callback (function): function callback ``scipy.optimize.minimize`` L-BFGS-B.
         options (dict): follows ``scipy.optimize.minimize`` syntax for L-BFGS-B.
         processes (int): number of processes when using the paralle BFGS method.
     """
+
     import numpy as np
 
-    def __init__(self, function, args=(), bounds=None,
-                 callback=None, options=None, processes=None):
+    def __init__(
+        self,
+        function,
+        args=(),
+        bounds=None,
+        callback=None,
+        options=None,
+        processes=None,
+    ):
         self.function = function
         self.args = args
         self.xval = None
         self.function_value = None
         self.jacobian_value = None
         self.precision = self.np.finfo("float64").eps
         self.bounds = bounds
@@ -234,43 +305,58 @@
         Args:
             x0 (numpy.array): guess for initial solution.
 
         Returns:
             scipy.minimize result object
         """
         from scipy.optimize import minimize
-        out = minimize(fun=self.fun, x0=x0, jac=self.jac, method='L-BFGS-B',
-                        bounds=self.bounds, callback=self.callback, options=self.options)
+
+        out = minimize(
+            fun=self.fun,
+            x0=x0,
+            jac=self.jac,
+            method="L-BFGS-B",
+            bounds=self.bounds,
+            callback=self.callback,
+            options=self.options,
+        )
         out.hess_inv = out.hess_inv * self.np.identity(len(x0))
         return out
 
     @staticmethod
     def _eval_approx(eps_at, fun, x, eps):
         if eps_at == 0:
             x_ = x
         else:
             x_ = x.copy()
             if eps_at <= len(x):
-                x_[eps_at-1] += eps
+                x_[eps_at - 1] += eps
             else:
-                x_[eps_at-1-len(x)] -= eps
+                x_[eps_at - 1 - len(x)] -= eps
         return fun(x_)
 
     def evaluate(self, x, eps=1e-8):
-        if not (self.xval is not None and all(abs(self.xval - x) <= self.precision*2)):
-            eps_at = range(len(x)+1)
+        if not (
+            self.xval is not None and all(abs(self.xval - x) <= self.precision * 2)
+        ):
+            eps_at = range(len(x) + 1)
             self.xval = x.copy()
+
             def operation(epsi):
-                return self._eval_approx(epsi, lambda y: self.function(y, *self.args), x, eps)
+                return self._eval_approx(
+                    epsi, lambda y: self.function(y, *self.args), x, eps
+                )
 
             from joblib import Parallel, delayed
-            ret = Parallel(self.processes, prefer='threads')(delayed(operation)(epsi) for epsi in eps_at)
+
+            ret = Parallel(self.processes, prefer="threads")(
+                delayed(operation)(epsi) for epsi in eps_at
+            )
             self.function_value = ret[0]
-            self.jacobian_value = (
-                ret[1:(len(x)+1)] - self.function_value) / eps
+            self.jacobian_value = (ret[1 : (len(x) + 1)] - self.function_value) / eps
 
     def fun(self, x):
         self.evaluate(x)
         return self.function_value
 
     def jac(self, x):
         self.evaluate(x)
```

### Comparing `qibo-0.1.8rc0/src/qibo/parallel.py` & `qibo-0.1.9/src/qibo/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,31 +32,37 @@
         processes (int): number of processes for parallel evaluation.
 
     Returns:
         Circuit evaluation for input states.
     """
     if backend is None:  # pragma: no cover
         from qibo.backends import GlobalBackend
+
         backend = GlobalBackend()
 
     if states is None or not isinstance(states, list):  # pragma: no cover
         from qibo.config import raise_error
+
         raise_error(RuntimeError, "states must be a list.")
 
     def operation(state, circuit):
         return backend.execute_circuit(circuit, state)
 
     from joblib import Parallel, delayed
-    results = Parallel(n_jobs=processes, prefer='threads')(
-        delayed(operation)(state, circuit) for state in states)
+
+    results = Parallel(n_jobs=processes, prefer="threads")(
+        delayed(operation)(state, circuit) for state in states
+    )
 
     return results
 
 
-def parallel_parametrized_execution(circuit, parameters, initial_state=None, processes=None, backend=None):
+def parallel_parametrized_execution(
+    circuit, parameters, initial_state=None, processes=None, backend=None
+):
     """Execute circuit for multiple parameters and fixed initial_state.
 
     Example:
         .. code-block:: python
 
             import qibo
             original_backend = qibo.get_backend()
@@ -91,24 +97,29 @@
         processes (int): number of processes for parallel evaluation.
 
     Returns:
         Circuit evaluation for input parameters.
     """
     if backend is None:  # pragma: no cover
         from qibo.backends import GlobalBackend
+
         backend = GlobalBackend()
 
     if not isinstance(parameters, list):  # pragma: no cover
         from qibo.config import raise_error
+
         raise_error(RuntimeError, "parameters must be a list.")
 
     def operation(params, circuit, state):
         if state is not None:
             state = backend.cast(state, copy=True)
         circuit.set_parameters(params)
         return backend.execute_circuit(circuit, state)
 
     from joblib import Parallel, delayed
-    results = Parallel(n_jobs=processes, prefer='threads')(
-        delayed(operation)(param, circuit.copy(deep=True), initial_state) for param in parameters)
+
+    results = Parallel(n_jobs=processes, prefer="threads")(
+        delayed(operation)(param, circuit.copy(deep=True), initial_state)
+        for param in parameters
+    )
 
     return results
```

### Comparing `qibo-0.1.8rc0/src/qibo/solvers.py` & `qibo-0.1.9/src/qibo/solvers.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     @t.setter
     def t(self, new_t):
         """Updates solver's current time."""
         self._t = new_t
         self.current_hamiltonian = self.hamiltonian(self.t)
 
-    def __call__(self, state): # pragma: no cover
+    def __call__(self, state):  # pragma: no cover
         # abstract method
         raise_error(NotImplementedError)
 
 
 class TrotterizedExponential(BaseSolver):
     """Solver that uses Trotterized exponentials.
 
@@ -85,15 +85,15 @@
         ham2 = self.hamiltonian(self.t + self.dt / 2.0)
         ham3 = self.hamiltonian(self.t + self.dt)
         k1 = ham1 @ state
         k2 = ham2 @ (state + self.dt * k1 / 2.0)
         k3 = ham2 @ (state + self.dt * k2 / 2.0)
         k4 = ham3 @ (state + self.dt * k3)
         self.t += self.dt
-        return (state - 1j * self.dt * (k1 + 2 * k2 + 2 * k3 + k4) / 6.0)
+        return state - 1j * self.dt * (k1 + 2 * k2 + 2 * k3 + k4) / 6.0
 
 
 class RungeKutta45(BaseSolver):
     """Solver based on the 5th order Runge-Kutta method."""
 
     def __call__(self, state):
         ham1 = self.current_hamiltonian
@@ -101,23 +101,39 @@
         ham3 = self.hamiltonian(self.t + 3 * self.dt / 8.0)
         ham4 = self.hamiltonian(self.t + 12 * self.dt / 13.0)
         ham5 = self.hamiltonian(self.t + self.dt)
         ham6 = self.hamiltonian(self.t + self.dt / 2.0)
         k1 = ham1 @ state
         k2 = ham2 @ (state + self.dt * k1 / 4.0)
         k3 = ham3 @ (state + self.dt * (3 * k1 + 9 * k2) / 32.0)
-        k4 = ham4 @ (state + self.dt * (1932 * k1 -
-                                        7200 * k2 + 7296 * k3) / 2197.0)
-        k5 = ham5 @ (state + self.dt * (439 * k1 / 216.0 - 8 *
-                                        k2 + 3680 * k3 / 513.0 - 845 * k4 / 4104.0))
-        k6 = ham6 @ (state + self.dt * (-8 * k1 / 27.0 + 2 * k2 -
-                                        3544 * k3 / 2565 + 1859 * k4 / 4104 - 11 * k5 / 40.0))
+        k4 = ham4 @ (state + self.dt * (1932 * k1 - 7200 * k2 + 7296 * k3) / 2197.0)
+        k5 = ham5 @ (
+            state
+            + self.dt
+            * (439 * k1 / 216.0 - 8 * k2 + 3680 * k3 / 513.0 - 845 * k4 / 4104.0)
+        )
+        k6 = ham6 @ (
+            state
+            + self.dt
+            * (
+                -8 * k1 / 27.0
+                + 2 * k2
+                - 3544 * k3 / 2565
+                + 1859 * k4 / 4104
+                - 11 * k5 / 40.0
+            )
+        )
         self.t += self.dt
-        return (state - 1j * self.dt * (16 * k1 / 135.0 + 6656 * k3 / 12825.0 + 28561 * k4 / 56430.0 -
-                                        9 * k5 / 50.0 + 2 * k6 / 55.0))
+        return state - 1j * self.dt * (
+            16 * k1 / 135.0
+            + 6656 * k3 / 12825.0
+            + 28561 * k4 / 56430.0
+            - 9 * k5 / 50.0
+            + 2 * k6 / 55.0
+        )
 
 
 def get_solver(solver_name, dt, hamiltonian):
     if solver_name == "exp":
         if isinstance(hamiltonian, AbstractHamiltonian):
             h0 = hamiltonian
         elif isinstance(hamiltonian, BaseAdiabaticHamiltonian):
```

### Comparing `qibo-0.1.8rc0/src/qibo/states.py` & `qibo-0.1.9/src/qibo/states.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import collections
+
 from qibo.config import raise_error
 
 
 class CircuitResult:
-
     def __init__(self, backend, circuit, execution_result, nshots=None):
         self.backend = backend
         self.circuit = circuit
         self.nqubits = circuit.nqubits
         self.density_matrix = circuit.density_matrix
         self.execution_result = execution_result
         self.nshots = nshots
@@ -61,17 +61,21 @@
                 Default is 20.
 
         Returns:
             A string representing the state in the computational basis.
         """
         state = self.backend.circuit_result_tensor(self)
         if self.density_matrix:
-            terms = self.backend.calculate_symbolic_density_matrix(state, self.nqubits, decimals, cutoff, max_terms)
+            terms = self.backend.calculate_symbolic_density_matrix(
+                state, self.nqubits, decimals, cutoff, max_terms
+            )
         else:
-            terms = self.backend.calculate_symbolic(state, self.nqubits, decimals, cutoff, max_terms)
+            terms = self.backend.calculate_symbolic(
+                state, self.nqubits, decimals, cutoff, max_terms
+            )
         return " + ".join(terms)
 
     def __repr__(self):
         return self.backend.circuit_result_representation(self)
 
     def __array__(self):
         """State's tensor representation as an array."""
@@ -108,43 +112,53 @@
         """
         qubits = self.circuit.measurement_gate.qubits
         if self._samples is None:
             probs = self.probabilities(qubits)
             self._samples = self.backend.sample_shots(probs, self.nshots)
             if self.circuit.measurement_gate.has_bitflip_noise():
                 p0, p1 = self.circuit.measurement_gate.bitflip_map
-                bitflip_probabilities = [[p0.get(q) for q in qubits],
-                                         [p1.get(q) for q in qubits]]
-                noiseless_samples = self.backend.samples_to_binary(self._samples, len(qubits))
-                noisy_samples = self.backend.apply_bitflips(noiseless_samples, bitflip_probabilities)
-                self._samples = self.backend.samples_to_decimal(noisy_samples, len(qubits))
+                bitflip_probabilities = [
+                    [p0.get(q) for q in qubits],
+                    [p1.get(q) for q in qubits],
+                ]
+                noiseless_samples = self.backend.samples_to_binary(
+                    self._samples, len(qubits)
+                )
+                noisy_samples = self.backend.apply_bitflips(
+                    noiseless_samples, bitflip_probabilities
+                )
+                self._samples = self.backend.samples_to_decimal(
+                    noisy_samples, len(qubits)
+                )
 
         if registers:
             qubit_map = {q: i for i, q in enumerate(qubits)}
             reg_samples = {}
             samples = self.backend.samples_to_binary(self._samples, len(qubits))
             for name, rqubits in self.circuit.measurement_tuples.items():
                 rqubits = tuple(qubit_map.get(q) for q in rqubits)
                 rsamples = samples[:, rqubits]
                 if binary:
                     reg_samples[name] = rsamples
                 else:
-                    reg_samples[name] = self.backend.samples_to_decimal(rsamples, len(rqubits))
+                    reg_samples[name] = self.backend.samples_to_decimal(
+                        rsamples, len(rqubits)
+                    )
             return reg_samples
 
         if binary:
             return self.backend.samples_to_binary(self._samples, len(qubits))
         else:
             return self._samples
 
     @staticmethod
     def _frequencies_to_binary(frequencies, nqubits):
         return collections.Counter(
-                {"{0:b}".format(k).zfill(nqubits): v
-                 for k, v in frequencies.items()})
+            {"{:b}".format(k).zfill(nqubits): v for k, v in frequencies.items()}
+        )
 
     def frequencies(self, binary=True, registers=False):
         """Returns the frequencies of measured samples.
 
         Args:
             binary (bool): Return frequency keys in binary or decimal form.
             registers (bool): Group frequencies according to registers.
@@ -164,47 +178,69 @@
                 each register.
             If `registers` is `False`
                 a single `Counter` is returned which contains samples from all
                 the measured qubits, independently of their registers.
         """
         qubits = self.circuit.measurement_gate.qubits
         if self._frequencies is None:
-            if self.circuit.measurement_gate.has_bitflip_noise() and self._samples is None:
+            if (
+                self.circuit.measurement_gate.has_bitflip_noise()
+                and self._samples is None
+            ):
                 self._samples = self.samples(binary=False)
             if self._samples is None:
                 probs = self.probabilities(qubits)
                 self._frequencies = self.backend.sample_frequencies(probs, self.nshots)
             else:
                 self._frequencies = self.backend.calculate_frequencies(self._samples)
 
         if registers:
             qubit_map = {q: i for i, q in enumerate(qubits)}
             reg_frequencies = {}
-            binary_frequencies = self._frequencies_to_binary(self._frequencies, len(qubits))
+            binary_frequencies = self._frequencies_to_binary(
+                self._frequencies, len(qubits)
+            )
             for name, rqubits in self.circuit.measurement_tuples.items():
                 rfreqs = collections.Counter()
                 for bitstring, freq in binary_frequencies.items():
                     idx = 0
                     for i, q in enumerate(rqubits):
                         if int(bitstring[qubit_map.get(q)]):
                             idx += 2 ** (len(rqubits) - i - 1)
                     rfreqs[idx] += freq
                 if binary:
-                    reg_frequencies[name] = self._frequencies_to_binary(rfreqs, len(rqubits))
+                    reg_frequencies[name] = self._frequencies_to_binary(
+                        rfreqs, len(rqubits)
+                    )
                 else:
                     reg_frequencies[name] = rfreqs
             return reg_frequencies
 
         if binary:
             return self._frequencies_to_binary(self._frequencies, len(qubits))
         else:
             return self._frequencies
 
     def apply_bitflips(self, p0, p1=None):
         mgate = self.circuit.measurement_gate
         if p1 is None:
             probs = 2 * (mgate._get_bitflip_tuple(mgate.qubits, p0),)
         else:
-            probs = (mgate._get_bitflip_tuple(mgate.qubits, p0),
-                     mgate._get_bitflip_tuple(mgate.qubits, p1))
+            probs = (
+                mgate._get_bitflip_tuple(mgate.qubits, p0),
+                mgate._get_bitflip_tuple(mgate.qubits, p1),
+            )
         noiseless_samples = self.samples()
         return self.backend.apply_bitflips(noiseless_samples, probs)
+
+    def expectation_from_samples(self, observable):
+        """Computes the real expectation value of a diagonal observable from frequencies.
+
+        Args:
+            observable (Hamiltonian/SymbolicHamiltonian): diagonal observable in the computational basis.
+
+        Returns:
+            Real number corresponding to the expectation value.
+        """
+        freq = self.frequencies(binary=True)
+        qubit_map = self.circuit.measurement_gate.qubits
+        return observable.expectation_from_samples(freq, qubit_map)
```

### Comparing `qibo-0.1.8rc0/src/qibo/symbols.py` & `qibo-0.1.9/src/qibo/symbols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import sympy
 import numpy as np
-from qibo import gates, matrices
+import sympy
+
+from qibo import gates
+from qibo.backends import matrices
 from qibo.config import raise_error
 
 
 class Symbol(sympy.Symbol):
     """Qibo specialization for ``sympy`` symbols.
 
     These symbols can be used to create :class:`qibo.hamiltonians.hamiltonians.SymbolicHamiltonian`.
@@ -39,27 +41,42 @@
         name = "{}{}".format(name, q)
         assumptions["commutative"] = commutative
         return super().__new__(cls=cls, name=name, **assumptions)
 
     def __init__(self, q, matrix=None, name="Symbol", commutative=False):
         self.target_qubit = q
         self._gate = None
-        if not (matrix is None or isinstance(matrix, np.ndarray) or
-              isinstance(matrix, (np.int, np.float, np.complex, np.int32,
-                                  np.int64, np.float32, np.float64,
-                                  np.complex64, np.complex128))):
-            raise_error(TypeError, "Invalid type {} of symbol matrix."
-                                   "".format(type(matrix)))
+        if not (
+            matrix is None
+            or isinstance(matrix, np.ndarray)
+            or isinstance(
+                matrix,
+                (
+                    np.int,
+                    np.float,
+                    np.complex,
+                    np.int32,
+                    np.int64,
+                    np.float32,
+                    np.float64,
+                    np.complex64,
+                    np.complex128,
+                ),
+            )
+        ):
+            raise_error(
+                TypeError, "Invalid type {} of symbol matrix." "".format(type(matrix))
+            )
         self.matrix = matrix
 
     def __getstate__(self):
         return {
             "target_qubit": self.target_qubit,
             "matrix": self.matrix,
-            "name": self.name
+            "name": self.name,
         }
 
     def __setstate__(self, data):
         self.target_qubit = data.get("target_qubit")
         self.matrix = data.get("matrix")
         self.name = data.get("name")
         self._gate = None
@@ -81,23 +98,23 @@
             nqubits (int): Total number of qubits in the system.
 
         Returns:
             Matrix of dimension (2^nqubits, 2^nqubits) composed of the Kronecker
             product between identities and the symbol's single-qubit matrix.
         """
         from qibo.hamiltonians.models import multikron
+
         matrix_list = self.target_qubit * [matrices.I]
         matrix_list.append(self.matrix)
         n = nqubits - self.target_qubit - 1
         matrix_list.extend(matrices.I for _ in range(n))
         return multikron(matrix_list)
 
 
 class PauliSymbol(Symbol):
-
     def __new__(cls, q, commutative=False, **assumptions):
         matrix = getattr(matrices, cls.__name__)
         return super().__new__(cls, q, matrix, cls.__name__, commutative, **assumptions)
 
     def __init__(self, q, commutative=False):
         name = self.__class__.__name__
         matrix = getattr(matrices, name)
@@ -110,35 +127,39 @@
 
 class I(PauliSymbol):
     """Qibo symbol for the identity operator.
 
     Args:
         q (int): Target qubit id.
     """
+
     pass
 
 
 class X(PauliSymbol):
     """Qibo symbol for the Pauli-X operator.
 
     Args:
         q (int): Target qubit id.
     """
+
     pass
 
 
 class Y(PauliSymbol):
     """Qibo symbol for the Pauli-X operator.
 
     Args:
         q (int): Target qubit id.
     """
+
     pass
 
 
 class Z(PauliSymbol):
     """Qibo symbol for the Pauli-X operator.
 
     Args:
         q (int): Target qubit id.
     """
+
     pass
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/conftest.py` & `qibo-0.1.9/src/qibo/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """
 conftest.py
 
 Pytest fixtures.
 """
 import sys
+
 import pytest
-from qibo.backends import construct_backend
 
+from qibo.backends import construct_backend
 
 # backends to be tested
 BACKENDS = ["numpy", "tensorflow", "qibojit-numba", "qibojit-cupy", "qibojit-cuquantum"]
 # multigpu configurations to be tested (only with qibojit-cupy)
-ACCELERATORS = [{"/GPU:0": 1, "/GPU:1": 1}, {"/GPU:0": 2, "/GPU:1": 2},
-                {"/GPU:0": 1, "/GPU:1": 1, "/GPU:2": 1, "/GPU:3": 1}]
+ACCELERATORS = [
+    {"/GPU:0": 1, "/GPU:1": 1},
+    {"/GPU:0": 2, "/GPU:1": 2},
+    {"/GPU:0": 1, "/GPU:1": 1, "/GPU:2": 1, "/GPU:3": 1},
+]
 
 
 def get_backend(backend_name):
     if "-" in backend_name:
         name, platform = backend_name.split("-")
     else:
         name, platform = backend_name, None
     return construct_backend(name, platform=platform)
 
+
 # ignore backends that are not available in the current testing environment
 AVAILABLE_BACKENDS = []
 MULTIGPU_BACKENDS = []
 for backend_name in BACKENDS:
     try:
         _backend = get_backend(backend_name)
         AVAILABLE_BACKENDS.append(backend_name)
@@ -33,16 +38,15 @@
             MULTIGPU_BACKENDS.append(backend_name)
     except (ModuleNotFoundError, ImportError):
         pass
 
 
 def pytest_runtest_setup(item):
     ALL = {"darwin", "linux"}
-    supported_platforms = ALL.intersection(
-        mark.name for mark in item.iter_markers())
+    supported_platforms = ALL.intersection(mark.name for mark in item.iter_markers())
     plat = sys.platform
     if supported_platforms and plat not in supported_platforms:  # pragma: no cover
         # case not covered by workflows
         pytest.skip("Cannot run test on platform {}.".format(plat))
 
 
 def pytest_configure(config):
@@ -53,25 +57,30 @@
 def backend(backend_name):
     yield get_backend(backend_name)
 
 
 def pytest_generate_tests(metafunc):
     module_name = metafunc.module.__name__
 
-    if module_name == "qibo.tests.test_models_qgan" and "tensorflow" not in AVAILABLE_BACKENDS:  # pragma: no cover
+    if (
+        module_name == "qibo.tests.test_models_qgan"
+        and "tensorflow" not in AVAILABLE_BACKENDS
+    ):  # pragma: no cover
         pytest.skip("Skipping QGAN tests because tensorflow is not available.")
 
     if module_name == "qibo.tests.test_models_distcircuit_execution":
         config = [(bk, acc) for acc in ACCELERATORS for bk in MULTIGPU_BACKENDS]
         metafunc.parametrize("backend_name,accelerators", config)
 
     else:
         if "backend_name" in metafunc.fixturenames:
             if "accelerators" in metafunc.fixturenames:
                 config = [(backend, None) for backend in AVAILABLE_BACKENDS]
-                config.extend((bk, acc) for acc in ACCELERATORS for bk in MULTIGPU_BACKENDS)
+                config.extend(
+                    (bk, acc) for acc in ACCELERATORS for bk in MULTIGPU_BACKENDS
+                )
                 metafunc.parametrize("backend_name,accelerators", config)
             else:
                 metafunc.parametrize("backend_name", AVAILABLE_BACKENDS)
 
         elif "accelerators" in metafunc.fixturenames:
             metafunc.parametrize("accelerators", ACCELERATORS)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_backends.py` & `qibo-0.1.9/src/qibo/tests/test_backends.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,68 +1,103 @@
-import pytest
 import numpy as np
-from qibo import gates
+import pytest
 
+from qibo import gates
 
 ####################### Test `asmatrix` #######################
 GATES = [
     ("H", (0,), np.array([[1, 1], [1, -1]]) / np.sqrt(2)),
     ("X", (0,), np.array([[0, 1], [1, 0]])),
     ("Y", (0,), np.array([[0, -1j], [1j, 0]])),
     ("Z", (1,), np.array([[1, 0], [0, -1]])),
     ("S", (2,), np.array([[1, 0], [0, 1j]])),
     ("T", (2,), np.array([[1, 0], [0, np.exp(1j * np.pi / 4.0)]])),
-    ("CNOT", (0, 1), np.array([[1, 0, 0, 0], [0, 1, 0, 0],
-                               [0, 0, 0, 1], [0, 0, 1, 0]])),
-    ("CZ", (1, 3), np.array([[1, 0, 0, 0], [0, 1, 0, 0],
-                             [0, 0, 1, 0], [0, 0, 0, -1]])),
-    ("SWAP", (2, 4), np.array([[1, 0, 0, 0], [0, 0, 1, 0],
-                               [0, 1, 0, 0], [0, 0, 0, 1]])),
-    ("FSWAP", (2, 4), np.array([[1, 0, 0, 0], [0, 0, 1, 0],
-                               [0, 1, 0, 0], [0, 0, 0, -1]])),
-    ("TOFFOLI", (1, 2, 3), np.array([[1, 0, 0, 0, 0, 0, 0, 0],
-                                     [0, 1, 0, 0, 0, 0, 0, 0],
-                                     [0, 0, 1, 0, 0, 0, 0, 0],
-                                     [0, 0, 0, 1, 0, 0, 0, 0],
-                                     [0, 0, 0, 0, 1, 0, 0, 0],
-                                     [0, 0, 0, 0, 0, 1, 0, 0],
-                                     [0, 0, 0, 0, 0, 0, 0, 1],
-                                     [0, 0, 0, 0, 0, 0, 1, 0]]))
+    (
+        "CNOT",
+        (0, 1),
+        np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]),
+    ),
+    ("CZ", (1, 3), np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, -1]])),
+    (
+        "SWAP",
+        (2, 4),
+        np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, 1]]),
+    ),
+    (
+        "FSWAP",
+        (2, 4),
+        np.array([[1, 0, 0, 0], [0, 0, 1, 0], [0, 1, 0, 0], [0, 0, 0, -1]]),
+    ),
+    (
+        "TOFFOLI",
+        (1, 2, 3),
+        np.array(
+            [
+                [1, 0, 0, 0, 0, 0, 0, 0],
+                [0, 1, 0, 0, 0, 0, 0, 0],
+                [0, 0, 1, 0, 0, 0, 0, 0],
+                [0, 0, 0, 1, 0, 0, 0, 0],
+                [0, 0, 0, 0, 1, 0, 0, 0],
+                [0, 0, 0, 0, 0, 1, 0, 0],
+                [0, 0, 0, 0, 0, 0, 0, 1],
+                [0, 0, 0, 0, 0, 0, 1, 0],
+            ]
+        ),
+    ),
 ]
+
+
 @pytest.mark.parametrize("gate,qubits,target_matrix", GATES)
 def test_asmatrix(backend, gate, qubits, target_matrix):
     gate = getattr(gates, gate)(*qubits)
     backend.assert_allclose(gate.asmatrix(backend), target_matrix)
 
 
 GATES = [
-    ("RX", lambda x: np.array([[np.cos(x / 2.0), -1j * np.sin(x / 2.0)],
-                               [-1j * np.sin(x / 2.0), np.cos(x / 2.0)]])),
-    ("RY", lambda x: np.array([[np.cos(x / 2.0), -np.sin(x / 2.0)],
-                               [np.sin(x / 2.0), np.cos(x / 2.0)]])),
+    (
+        "RX",
+        lambda x: np.array(
+            [
+                [np.cos(x / 2.0), -1j * np.sin(x / 2.0)],
+                [-1j * np.sin(x / 2.0), np.cos(x / 2.0)],
+            ]
+        ),
+    ),
+    (
+        "RY",
+        lambda x: np.array(
+            [[np.cos(x / 2.0), -np.sin(x / 2.0)], [np.sin(x / 2.0), np.cos(x / 2.0)]]
+        ),
+    ),
     ("RZ", lambda x: np.diag([np.exp(-1j * x / 2.0), np.exp(1j * x / 2.0)])),
     ("U1", lambda x: np.diag([1, np.exp(1j * x)])),
-    ("CU1", lambda x: np.diag([1, 1, 1, np.exp(1j * x)]))
+    ("CU1", lambda x: np.diag([1, 1, 1, np.exp(1j * x)])),
 ]
+
+
 @pytest.mark.parametrize("gate,target_matrix", GATES)
 def test_asmatrix_rotations(backend, gate, target_matrix):
     """Check that `_construct_unitary` method constructs the proper matrix."""
     theta = 0.1234
     if gate == "CU1":
         gate = getattr(gates, gate)(0, 1, theta)
     else:
         gate = getattr(gates, gate)(0, theta)
     backend.assert_allclose(gate.asmatrix(backend), target_matrix(theta))
     backend.assert_allclose(gate.asmatrix(backend), target_matrix(theta))
 
 
 def test_control_matrix(backend):
     theta = 0.1234
-    rotation = np.array([[np.cos(theta / 2.0), -np.sin(theta / 2.0)],
-                         [np.sin(theta / 2.0), np.cos(theta / 2.0)]])
+    rotation = np.array(
+        [
+            [np.cos(theta / 2.0), -np.sin(theta / 2.0)],
+            [np.sin(theta / 2.0), np.cos(theta / 2.0)],
+        ]
+    )
     target_matrix = np.eye(4, dtype=rotation.dtype)
     target_matrix[2:, 2:] = rotation
     gate = gates.RY(0, theta).controlled_by(1)
     backend.assert_allclose(gate.asmatrix(backend), target_matrix)
 
     gate = gates.RY(0, theta).controlled_by(1, 2)
     with pytest.raises(NotImplementedError):
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_callbacks.py` & `qibo-0.1.9/src/qibo/tests/test_callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Test methods defined in `qibo/core/callbacks.py`."""
-import pytest
 import numpy as np
-from qibo import gates, callbacks
-from qibo.models import Circuit, AdiabaticEvolution
+import pytest
 
+from qibo import callbacks, gates
+from qibo.models import AdiabaticEvolution, Circuit
 
 # Absolute testing tolerance for the cases of zero entanglement entropy
 _atol = 1e-8
 
 
 def test_abstract_callback_properties():
     callback = callbacks.Callback()
@@ -65,53 +65,76 @@
     result = entropy.apply(backend, state)
     backend.assert_allclose(result, 1.0)
 
 
 def test_entropy_random_state(backend):
     """Check that entropy calculation agrees with numpy."""
     from qibo.config import EIGVAL_CUTOFF
+
     # Generate a random positive and hermitian density matrix
     rho = np.random.random((8, 8)) + 1j * np.random.random((8, 8))
     rho = rho + rho.conj().T
     _, u = np.linalg.eigh(rho)
     s = 5 * np.random.random(8)
     s = s / s.sum()
     rho = u.dot(np.diag(s)).dot(u.conj().T)
 
     result, spectrum = backend.entanglement_entropy(rho)
-    target = - (s * np.log2(s)).sum()
+    target = -(s * np.log2(s)).sum()
     backend.assert_allclose(result, target)
 
     target_eigvals = np.linalg.eigvalsh(rho)
     masked_eigvals = target_eigvals[np.where(target_eigvals > EIGVAL_CUTOFF)]
-    target_spectrum = - np.log(masked_eigvals)
+    target_spectrum = -np.log(masked_eigvals)
     backend.assert_allclose(spectrum, target_spectrum)
 
 
 def test_entropy_switch_partition(backend):
     """Check that partition is switched to the largest counterpart."""
     entropy = callbacks.EntanglementEntropy([0])
     entropy.nqubits = 5
     # Prepare ghz state of 5 qubits
-    state = np.zeros(2 ** 5)
+    state = np.zeros(2**5)
     state[0], state[-1] = 1, 1
     state = state / np.sqrt(2)
     result = entropy.apply(backend, state)
     backend.assert_allclose(result, 1.0)
 
 
 def test_entropy_numerical(backend):
     """Check that entropy calculation does not fail for tiny eigenvalues."""
-    eigvals = np.array([-1e-10, -1e-15, -2e-17, -1e-18, -5e-60, 1e-48, 4e-32,
-                        5e-14, 1e-14, 9.9e-13, 9e-13, 5e-13, 1e-13, 1e-12,
-                        1e-11, 1e-10, 1e-9, 1e-7, 1, 4, 10])
+    eigvals = np.array(
+        [
+            -1e-10,
+            -1e-15,
+            -2e-17,
+            -1e-18,
+            -5e-60,
+            1e-48,
+            4e-32,
+            5e-14,
+            1e-14,
+            9.9e-13,
+            9e-13,
+            5e-13,
+            1e-13,
+            1e-12,
+            1e-11,
+            1e-10,
+            1e-9,
+            1e-7,
+            1,
+            4,
+            10,
+        ]
+    )
     rho = np.diag(eigvals)
     result, _ = backend.entanglement_entropy(rho)
     mask = eigvals > 0
-    target = - (eigvals[mask] * np.log2(eigvals[mask])).sum()
+    target = -(eigvals[mask] * np.log2(eigvals[mask])).sum()
     backend.assert_allclose(result, target)
 
 
 @pytest.mark.parametrize("density_matrix", [False, True])
 def test_entropy_in_circuit(backend, density_matrix):
     """Check that entropy calculation works in circuit."""
     entropy = callbacks.EntanglementEntropy([0], compute_spectrum=True)
@@ -128,22 +151,28 @@
     backend.assert_allclose(values, target, atol=_atol)
 
     target_spectrum = [0, 0, np.log(2), np.log(2)]
     entropy_spectrum = np.concatenate(entropy.spectrum).ravel().tolist()
     backend.assert_allclose(entropy_spectrum, target_spectrum, atol=_atol)
 
 
-@pytest.mark.parametrize("gateconf,target_entropy",
-                         [(["H", "CNOT", "entropy"], [1.0]),
-                          (["H", "entropy", "CNOT"], [0.0]),
-                          (["entropy", "H", "CNOT"], [0.0]),
-                          (["entropy", "H", "CNOT", "entropy"], [0.0, 1.0]),
-                          (["H", "entropy", "CNOT", "entropy"], [0.0, 1.0]),
-                          (["entropy", "H", "entropy", "CNOT"], [0.0, 0.0])])
-def test_entropy_in_distributed_circuit(backend, accelerators, gateconf, target_entropy):
+@pytest.mark.parametrize(
+    "gateconf,target_entropy",
+    [
+        (["H", "CNOT", "entropy"], [1.0]),
+        (["H", "entropy", "CNOT"], [0.0]),
+        (["entropy", "H", "CNOT"], [0.0]),
+        (["entropy", "H", "CNOT", "entropy"], [0.0, 1.0]),
+        (["H", "entropy", "CNOT", "entropy"], [0.0, 1.0]),
+        (["entropy", "H", "entropy", "CNOT"], [0.0, 0.0]),
+    ],
+)
+def test_entropy_in_distributed_circuit(
+    backend, accelerators, gateconf, target_entropy
+):
     """Check that various entropy configurations work in distributed circuit."""
     target_c = Circuit(4)
     target_c.add([gates.H(0), gates.CNOT(0, 1)])
     target_state = backend.execute_circuit(target_c)
 
     entropy = callbacks.EntanglementEntropy([0])
     c = Circuit(4, accelerators)
@@ -186,15 +215,15 @@
     c.add(gates.CallbackGate(entropy))
     state = backend.execute_circuit(c)
     backend.assert_allclose(state, target_state)
 
     def target_entropy(t):
         cos = np.cos(t / 2.0) ** 2
         sin = np.sin(t / 2.0) ** 2
-        return - cos * np.log2(cos) - sin * np.log2(sin)
+        return -cos * np.log2(cos) - sin * np.log2(sin)
 
     target = [0, target_entropy(0.1234), 0, target_entropy(0.4321)]
     values = [backend.to_numpy(x) for x in entropy[:]]
     backend.assert_allclose(values, target, atol=_atol)
 
     c = Circuit(8, accelerators)
     with pytest.raises(RuntimeError):
@@ -204,55 +233,56 @@
 
 def test_entropy_large_circuit(backend, accelerators):
     """Check that entropy calculation works for variational like circuit."""
     thetas = np.pi * np.random.random((3, 8))
     target_entropy = callbacks.EntanglementEntropy([0, 2, 4, 5])
     target_entropy.nqubits = 8
     c1 = Circuit(8)
-    c1.add((gates.RY(i, thetas[0, i]) for i in range(8)))
-    c1.add((gates.CZ(i, i + 1) for i in range(0, 7, 2)))
+    c1.add(gates.RY(i, thetas[0, i]) for i in range(8))
+    c1.add(gates.CZ(i, i + 1) for i in range(0, 7, 2))
     state1 = backend.execute_circuit(c1).state()
     e1 = target_entropy.apply(backend, state1)
 
     c2 = Circuit(8)
-    c2.add((gates.RY(i, thetas[1, i]) for i in range(8)))
-    c2.add((gates.CZ(i, i + 1) for i in range(1, 7, 2)))
+    c2.add(gates.RY(i, thetas[1, i]) for i in range(8))
+    c2.add(gates.CZ(i, i + 1) for i in range(1, 7, 2))
     c2.add(gates.CZ(0, 7))
     state2 = backend.execute_circuit(c1 + c2).state()
     e2 = target_entropy.apply(backend, state2)
 
     c3 = Circuit(8)
-    c3.add((gates.RY(i, thetas[2, i]) for i in range(8)))
-    c3.add((gates.CZ(i, i + 1) for i in range(0, 7, 2)))
+    c3.add(gates.RY(i, thetas[2, i]) for i in range(8))
+    c3.add(gates.CZ(i, i + 1) for i in range(0, 7, 2))
     state3 = backend.execute_circuit(c1 + c2 + c3).state()
     e3 = target_entropy.apply(backend, state3)
 
     entropy = callbacks.EntanglementEntropy([0, 2, 4, 5])
     c = Circuit(8, accelerators)
     c.add(gates.CallbackGate(entropy))
-    c.add((gates.RY(i, thetas[0, i]) for i in range(8)))
-    c.add((gates.CZ(i, i + 1) for i in range(0, 7, 2)))
+    c.add(gates.RY(i, thetas[0, i]) for i in range(8))
+    c.add(gates.CZ(i, i + 1) for i in range(0, 7, 2))
     c.add(gates.CallbackGate(entropy))
-    c.add((gates.RY(i, thetas[1, i]) for i in range(8)))
-    c.add((gates.CZ(i, i + 1) for i in range(1, 7, 2)))
+    c.add(gates.RY(i, thetas[1, i]) for i in range(8))
+    c.add(gates.CZ(i, i + 1) for i in range(1, 7, 2))
     c.add(gates.CZ(0, 7))
     c.add(gates.CallbackGate(entropy))
-    c.add((gates.RY(i, thetas[2, i]) for i in range(8)))
-    c.add((gates.CZ(i, i + 1) for i in range(0, 7, 2)))
+    c.add(gates.RY(i, thetas[2, i]) for i in range(8))
+    c.add(gates.CZ(i, i + 1) for i in range(0, 7, 2))
     c.add(gates.CallbackGate(entropy))
     state = backend.execute_circuit(c)
 
     backend.assert_allclose(state3, state)
     values = [backend.to_numpy(x) for x in entropy[:]]
     targets = [backend.to_numpy(x) for x in [0, e1, e2, e3]]
     backend.assert_allclose(values, targets)
 
 
 def test_entropy_density_matrix(backend):
     from qibo.tests.utils import random_density_matrix
+
     rho = random_density_matrix(4)
     # this rho is not always positive. Make rho positive for this application
     _, u = np.linalg.eigh(rho)
     rho = u.dot(np.diag(5 * np.random.random(u.shape[0]))).dot(u.conj().T)
     # this is a positive rho
 
     entropy = callbacks.EntanglementEntropy([1, 3])
@@ -261,15 +291,15 @@
 
     rho = rho.reshape(8 * (2,))
     reduced_rho = np.einsum("abcdafch->bdfh", rho).reshape((4, 4))
     eigvals = np.linalg.eigvalsh(reduced_rho).real
     # assert that all eigenvalues are non-negative
     assert (eigvals >= 0).prod()
     mask = eigvals > 0
-    target_ent = - (eigvals[mask] * np.log2(eigvals[mask])).sum()
+    target_ent = -(eigvals[mask] * np.log2(eigvals[mask])).sum()
     backend.assert_allclose(final_ent, target_ent)
 
 
 @pytest.mark.parametrize("density_matrix", [False, True])
 @pytest.mark.parametrize("copy", [False, True])
 def test_state_callback(backend, density_matrix, copy):
     statec = callbacks.State(copy=copy)
@@ -323,34 +353,38 @@
         target_overlap = np.abs((state0.conj() * state1).sum())
         backend.assert_allclose(final_overlap, target_overlap)
 
 
 @pytest.mark.parametrize("density_matrix", [False, True])
 def test_energy(backend, density_matrix):
     from qibo import hamiltonians
+
     ham = hamiltonians.TFIM(4, h=1.0, backend=backend)
     energy = callbacks.Energy(ham)
     matrix = backend.to_numpy(ham.matrix)
     if density_matrix:
         from qibo.tests.utils import random_density_matrix
+
         state = random_density_matrix(4)
         target_energy = np.trace(matrix.dot(state))
         final_energy = energy.apply_density_matrix(backend, state)
     else:
         from qibo.tests.utils import random_state
+
         state = random_state(4)
         target_energy = state.conj().dot(matrix.dot(state))
         final_energy = energy.apply(backend, state)
     backend.assert_allclose(final_energy, target_energy)
 
 
 @pytest.mark.parametrize("dense", [False, True])
 @pytest.mark.parametrize("check_degenerate", [False, True])
 def test_gap(backend, dense, check_degenerate):
     from qibo import hamiltonians
+
     h0 = hamiltonians.X(4, dense=dense, backend=backend)
     if check_degenerate:
         # use h=0 to make this Hamiltonian degenerate
         h1 = hamiltonians.TFIM(4, h=0, dense=dense, backend=backend)
     else:
         h1 = hamiltonians.TFIM(4, h=1, dense=dense, backend=backend)
 
@@ -363,23 +397,24 @@
         targets["gap"].append(eigvals[1] - eigvals[0])
     if check_degenerate:
         targets["gap"][-1] = eigvals[3] - eigvals[0]
 
     gap = callbacks.Gap(check_degenerate=check_degenerate)
     ground = callbacks.Gap(0)
     excited = callbacks.Gap(1)
-    evolution = AdiabaticEvolution(h0, h1, lambda t: t, dt=1e-1,
-                                   callbacks=[gap, ground, excited])
+    evolution = AdiabaticEvolution(
+        h0, h1, lambda t: t, dt=1e-1, callbacks=[gap, ground, excited]
+    )
     final_state = evolution(final_time=1.0)
     targets = {k: np.stack(v) for k, v in targets.items()}
 
     values = {
         "ground": np.array([backend.to_numpy(x) for x in ground]),
         "excited": np.array([backend.to_numpy(x) for x in excited]),
-        "gap": np.array([backend.to_numpy(x) for x in gap])
+        "gap": np.array([backend.to_numpy(x) for x in gap]),
     }
     for k, v in values.items():
         backend.assert_allclose(v, targets.get(k))
 
 
 def test_gap_errors():
     """Check errors in gap callback instantiation."""
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_cirq.py` & `qibo-0.1.9/src/qibo/tests/test_cirq.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Test that Qibo gate execution agrees with Cirq."""
 import sys
-import numpy as np
+
 import cirq
+import numpy as np
 import pytest
+
 from qibo import gates, models
 from qibo.tests.utils import random_state
 
 
 def random_unitary_matrix(nqubits, dtype=np.complex128):
     """Generates a random unitary matrix of shape (2^nqubits, 2^nqubits)."""
     from scipy.linalg import expm
-    shape = 2 * (2 ** nqubits,)
+
+    shape = 2 * (2**nqubits,)
     m = np.random.random(shape) + 1j * np.random.random(shape)
     return expm(1j * (m + m.conj().T))
 
 
 def random_active_qubits(nqubits, nmin=None, nactive=None):
     """Generates random list of target and control qubits."""
     all_qubits = np.arange(nqubits)
@@ -28,32 +31,36 @@
     """Executes a Cirq circuit with the given list of gates."""
     c = cirq.Circuit()
     q = [cirq.LineQubit(i) for i in range(nqubits)]
     # apply identity gates to all qubits so that they become part of the circuit
     c.append([cirq.I(qi) for qi in q])
     for gate, targets in cirq_gates:
         c.append(gate(*[q[i] for i in targets]))
-    result = cirq.Simulator().simulate(c, initial_state=initial_state) # pylint: disable=no-member
+    result = cirq.Simulator().simulate(
+        c, initial_state=initial_state
+    )  # pylint: disable=no-member
     depth = len(cirq.Circuit(c.all_operations()))
     return result.final_state_vector, depth - 1
 
 
-def assert_gates_equivalent(backend, qibo_gate, cirq_gates, nqubits,
-                            ndevices=None, atol=1e-7):
+def assert_gates_equivalent(
+    backend, qibo_gate, cirq_gates, nqubits, ndevices=None, atol=1e-7
+):
     """Asserts that QIBO and Cirq gates have equivalent action on a random state.
 
     Args:
         qibo_gate: QIBO gate.
         cirq_gates: List of tuples (cirq gate, target qubit IDs).
         nqubits: Total number of qubits in the circuit.
         atol: Absolute tolerance in state vector comparsion.
     """
     initial_state = random_state(nqubits)
-    target_state, target_depth = execute_cirq(cirq_gates, nqubits,
-                                              np.copy(initial_state))
+    target_state, target_depth = execute_cirq(
+        cirq_gates, nqubits, np.copy(initial_state)
+    )
     accelerators = None
     if ndevices is not None:
         accelerators = {"/GPU:0": ndevices}
 
     c = models.Circuit(nqubits, accelerators)
     c.add(qibo_gate)
     assert c.depth == target_depth
@@ -91,39 +98,44 @@
 
     pieces = [x for x in re.split("[()]", "".join(clean_gate)) if x]
     if len(pieces) == 2:
         gatename, targets = pieces
         theta = None
     elif len(pieces) == 3:
         gatename, theta, targets = pieces
-    else: # pragma: no cover
+    else:  # pragma: no cover
         # case not tested because it fails
         raise RuntimeError("Cirq gate parsing failed with {}.".format(pieces))
 
     qubits = list(int(x) for x in targets.replace(" ", "").split(","))
     targets = (qubits.pop(),)
     controls = set(qubits)
 
     qibo_to_cirq = {"CNOT": "CNOT", "RY": "Ry", "TOFFOLI": "TOFFOLI"}
     assert qibo_to_cirq[qibo_gate.__class__.__name__] == gatename
     assert qibo_gate.target_qubits == targets
     assert set(qibo_gate.control_qubits) == controls
     if theta is not None:
         if "π" in theta:
             theta = np.pi * float(theta.replace("π", ""))
-        else: # pragma: no cover
+        else:  # pragma: no cover
             # case doesn't happen in tests (could remove)
             theta = float(theta)
         np.testing.assert_allclose(theta, qibo_gate.parameters)
 
 
-@pytest.mark.parametrize(("target", "controls", "free"),
-                         [(0, (1,), ()), (2, (0, 1), ()),
-                          (3, (0, 1, 4), (2, 5)),
-                          (7, (0, 1, 2, 3, 4), (5, 6))])
+@pytest.mark.parametrize(
+    ("target", "controls", "free"),
+    [
+        (0, (1,), ()),
+        (2, (0, 1), ()),
+        (3, (0, 1, 4), (2, 5)),
+        (7, (0, 1, 2, 3, 4), (5, 6)),
+    ],
+)
 def test_x_decompose_with_cirq(target, controls, free):
     """Check that decomposition of multi-control ``X`` agrees with Cirq."""
     gate = gates.X(target).controlled_by(*controls)
     qibo_decomp = gate.decompose(*free, use_toffolis=False)
 
     # Calculate the decomposition using Cirq.
     nqubits = max((target,) + controls + free) + 1
@@ -132,42 +144,49 @@
     free = [qubits[i] for i in free]
     cirq_decomp = cirq.decompose_multi_controlled_x(controls, qubits[target], free)
     assert len(qibo_decomp) == len(cirq_decomp)
     for qibo_gate, cirq_gate in zip(qibo_decomp, cirq_decomp):
         assert_cirq_gates_equivalent(qibo_gate, cirq_gate)
 
 
-@pytest.mark.parametrize(("gate_name", "nqubits", "ndevices"),
-                         [("H", 3, None), ("H", 3, 2),
-                          ("X", 2, None), ("X", 2, 2),
-                          ("Y", 1, None), ("Z", 1, None),
-                          ("S", 4, None), ("T", 4, None)])
+@pytest.mark.parametrize(
+    ("gate_name", "nqubits", "ndevices"),
+    [
+        ("H", 3, None),
+        ("H", 3, 2),
+        ("X", 2, None),
+        ("X", 2, 2),
+        ("Y", 1, None),
+        ("Z", 1, None),
+        ("S", 4, None),
+        ("T", 4, None),
+    ],
+)
 def test_one_qubit_gates(backend, gate_name, nqubits, ndevices):
     """Check simple one-qubit gates."""
     targets = random_active_qubits(nqubits, nactive=1)
     qibo_gate = getattr(gates, gate_name)(*targets)
     cirq_gate = [(getattr(cirq, gate_name), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("gate_name", "nqubits", "ndevices"),
-                         [("RX", 3, None), ("RX", 3, 4),
-                          ("RY", 2, None), ("RY", 2, 2),
-                          ("RZ", 1, None)])
+@pytest.mark.parametrize(
+    ("gate_name", "nqubits", "ndevices"),
+    [("RX", 3, None), ("RX", 3, 4), ("RY", 2, None), ("RY", 2, 2), ("RZ", 1, None)],
+)
 def test_one_qubit_parametrized_gates(backend, gate_name, nqubits, ndevices):
     """Check parametrized one-qubit rotations."""
     theta = 0.1234
     targets = random_active_qubits(nqubits, nactive=1)
     qibo_gate = getattr(gates, gate_name)(*targets, theta)
     cirq_gate = [(getattr(cirq, gate_name.lower())(theta), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("nqubits", "ndevices"),
-                         [(2, None), (3, 4), (2, 2)])
+@pytest.mark.parametrize(("nqubits", "ndevices"), [(2, None), (3, 4), (2, 2)])
 def test_u1_gate(backend, nqubits, ndevices):
     """Check U1 gate."""
     theta = 0.1234
     targets = random_active_qubits(nqubits, nactive=1)
     qibo_gate = gates.U1(*targets, theta)
     cirq_gate = [(cirq.ZPowGate(exponent=theta / np.pi), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
@@ -180,17 +199,17 @@
     """Check two-qubit gates."""
     targets = random_active_qubits(nqubits, nactive=2)
     qibo_gate = getattr(gates, gate_name)(*targets)
     cirq_gate = [(getattr(cirq, gate_name), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("nqubits", "ndevices"),
-                         [(2, None), (6, None), (6, 2),
-                          (7, None), (7, 4)])
+@pytest.mark.parametrize(
+    ("nqubits", "ndevices"), [(2, None), (6, None), (6, 2), (7, None), (7, 4)]
+)
 def test_two_qubit_parametrized_gates(backend, nqubits, ndevices):
     """Check ``CU1`` and ``fSim`` gate."""
     theta = 0.1234
     phi = 0.4321
 
     targets = random_active_qubits(nqubits, nactive=2)
     qibo_gate = gates.CU1(*targets, np.pi * theta)
@@ -199,17 +218,17 @@
 
     targets = random_active_qubits(nqubits, nactive=2)
     qibo_gate = gates.fSim(*targets, theta, phi)
     cirq_gate = [(cirq.FSimGate(theta=theta, phi=phi), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("nqubits", "ndevices"),
-                         [(5, None), (6, None), (9, None),
-                          (5, 2), (6, 4), (9, 8)])
+@pytest.mark.parametrize(
+    ("nqubits", "ndevices"), [(5, None), (6, None), (9, None), (5, 2), (6, 4), (9, 8)]
+)
 def test_unitary_matrix_gate(backend, nqubits, ndevices):
     """Check arbitrary unitary gate."""
     matrix = random_unitary_matrix(1)
     targets = random_active_qubits(nqubits, nactive=1)
     qibo_gate = gates.Unitary(matrix, *targets)
     cirq_gate = [(cirq.MatrixGate(matrix), targets)]
     assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits)
@@ -218,32 +237,54 @@
         matrix = random_unitary_matrix(2)
         targets = random_active_qubits(nqubits, nactive=2)
         qibo_gate = gates.Unitary(matrix, *targets)
         cirq_gate = [(cirq.MatrixGate(matrix), targets)]
         assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("gate_name", "nqubits", "ndevices"),
-                         [("H", 3, None), ("Z", 4, None), ("Y", 5, 4),
-                          ("X", 6, None), ("H", 7, 2), ("Z", 8, 8),
-                          ("Y", 12, 16), ("S", 13, 4), ("T", 9, 2)])
+@pytest.mark.parametrize(
+    ("gate_name", "nqubits", "ndevices"),
+    [
+        ("H", 3, None),
+        ("Z", 4, None),
+        ("Y", 5, 4),
+        ("X", 6, None),
+        ("H", 7, 2),
+        ("Z", 8, 8),
+        ("Y", 12, 16),
+        ("S", 13, 4),
+        ("T", 9, 2),
+    ],
+)
 def test_one_qubit_gates_controlled_by(backend, gate_name, nqubits, ndevices):
     """Check one-qubit gates controlled on arbitrary number of qubits."""
     all_qubits = np.arange(nqubits)
     for _ in range(5):
         activeq = random_active_qubits(nqubits, nmin=1)
         qibo_gate = getattr(gates, gate_name)(activeq[-1]).controlled_by(*activeq[:-1])
         cirq_gate = [(getattr(cirq, gate_name).controlled(len(activeq) - 1), activeq)]
         assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
-@pytest.mark.parametrize(("nqubits", "ndevices"),
-                         [(4, None), (5, None), (8, None),
-                          (12, None), (15, None), (17, None),
-                          (6, 2), (9, 2), (11, 4), (13, 8), (14, 16)])
+@pytest.mark.parametrize(
+    ("nqubits", "ndevices"),
+    [
+        (4, None),
+        (5, None),
+        (8, None),
+        (12, None),
+        (15, None),
+        (17, None),
+        (6, 2),
+        (9, 2),
+        (11, 4),
+        (13, 8),
+        (14, 16),
+    ],
+)
 def test_two_qubit_gates_controlled_by(backend, nqubits, ndevices):
     """Check ``SWAP`` and ``fSim`` gates controlled on arbitrary number of qubits."""
     all_qubits = np.arange(nqubits)
     for _ in range(5):
         activeq = random_active_qubits(nqubits, nmin=2)
         qibo_gate = gates.SWAP(*activeq[-2:]).controlled_by(*activeq[:-2])
         cirq_gate = [(cirq.SWAP.controlled(len(activeq) - 2), activeq)]
@@ -261,16 +302,20 @@
 @pytest.mark.parametrize("ndevices", [None, 2, 8])
 def test_unitary_matrix_gate_controlled_by(backend, nqubits, ntargets, ndevices):
     """Check arbitrary unitary gate controlled on arbitrary number of qubits."""
     all_qubits = np.arange(nqubits)
     for _ in range(10):
         activeq = random_active_qubits(nqubits, nactive=5)
         matrix = random_unitary_matrix(ntargets)
-        qibo_gate = gates.Unitary(matrix, *activeq[-ntargets:]).controlled_by(*activeq[:-ntargets])
-        cirq_gate = [(cirq.MatrixGate(matrix).controlled(len(activeq) - ntargets), activeq)]
+        qibo_gate = gates.Unitary(matrix, *activeq[-ntargets:]).controlled_by(
+            *activeq[:-ntargets]
+        )
+        cirq_gate = [
+            (cirq.MatrixGate(matrix).controlled(len(activeq) - ntargets), activeq)
+        ]
         assert_gates_equivalent(backend, qibo_gate, cirq_gate, nqubits, ndevices)
 
 
 @pytest.mark.parametrize("nqubits", [5, 6, 7, 11, 12])
 def test_qft(backend, accelerators, nqubits):
     c = models.QFT(nqubits, accelerators=accelerators)
     initial_state = random_state(nqubits)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_dill.py` & `qibo-0.1.9/src/qibo/tests/test_dill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,108 +1,116 @@
-import pytest
 import dill
 import numpy as np
+import pytest
 
 
 def test_dill_backends(backend):
     serial = dill.dumps(backend)
     new_backend = dill.loads(serial)
     assert type(new_backend) == type(backend)
     assert new_backend.name == backend.name
     assert new_backend.platform == backend.platform
     assert type(new_backend.matrices) == type(backend.matrices)
 
 
 def test_dill_global_backend():
     from qibo.backends import GlobalBackend
+
     backend = GlobalBackend()
     serial = dill.dumps(backend)
     new_backend = dill.loads(serial)
     assert type(new_backend) == type(backend)
     assert new_backend.name == backend.name
 
 
 def test_dill_circuit(accelerators):
     from qibo import gates
     from qibo.models import Circuit
+
     circuit = Circuit(5, accelerators=accelerators)
     circuit.add(gates.H(i) for i in range(5))
     serial = dill.dumps(circuit)
     new_circuit = dill.loads(serial)
     assert type(new_circuit) == type(circuit)
     assert new_circuit.nqubits == circuit.nqubits
     assert new_circuit.to_qasm() == circuit.to_qasm()
 
 
 def test_dill_circuit_result(backend):
     from qibo.models import QFT
+
     circuit = QFT(4)
     result = backend.execute_circuit(circuit)
     serial = dill.dumps(result)
     new_result = dill.loads(serial)
     assert type(new_result) == type(result)
     assert str(new_result) == str(result)
     backend.assert_allclose(new_result.state(), result.state())
 
 
 def test_dill_symbols():
     from qibo.symbols import Symbol, X
+
     matrix = np.random.random((2, 2))
     s = Symbol(0, matrix)
     x = X(1)
     ns = dill.loads(dill.dumps(s))
     nx = dill.loads(dill.dumps(x))
     assert type(ns) == type(s)
     assert type(nx) == type(x)
     np.testing.assert_allclose(nx.matrix, x.matrix)
     np.testing.assert_allclose(ns.matrix, s.matrix)
 
 
 def test_dill_measurement_symbol(backend):
     from qibo import gates
     from qibo.models import Circuit
+
     circuit = Circuit(1)
     circuit.add(gates.H(0))
     symbol = circuit.add(gates.M(0, collapse=True))
     result = backend.execute_circuit(circuit, nshots=1)
     nsymbol = dill.loads(dill.dumps(symbol))
     assert type(nsymbol) == type(symbol)
     backend.assert_allclose(nsymbol.outcome(), symbol.outcome())
 
 
 def test_dill_hamiltonian(backend):
     from qibo.hamiltonians import XXZ, Hamiltonian
+
     matrix = np.random.random((4, 4))
     ham1 = Hamiltonian(2, matrix, backend=backend)
     ham2 = XXZ(3, backend=backend)
     serial1 = dill.dumps(ham1)
     serial2 = dill.dumps(ham2)
     nham1 = dill.loads(serial1)
     nham2 = dill.loads(serial2)
     assert type(nham1) == type(ham1)
     assert type(nham2) == type(ham2)
     backend.assert_allclose(nham1.matrix, nham1.matrix)
     backend.assert_allclose(nham2.matrix, nham2.matrix)
 
 
 def test_dill_symbolic_hamiltonian(backend):
-    from qibo.symbols import X, Y, Z
     from qibo.hamiltonians import SymbolicHamiltonian
+    from qibo.symbols import X, Y, Z
+
     form = X(0) * X(1) + Y(0) * Y(1) + Z(0) * Z(1)
     ham = SymbolicHamiltonian(form, backend=backend)
     serial = dill.dumps(ham)
     nham = dill.loads(serial)
     assert type(nham) == type(ham)
     backend.assert_allclose(nham.matrix, ham.matrix)
 
 
 def test_dill_variational_models(backend):
     from qibo import gates
     from qibo.hamiltonians import TFIM
-    from qibo.models import Circuit, VQE, QAOA
+    from qibo.models import QAOA, VQE, Circuit
+
     ham = TFIM(4, backend=backend)
     circuit = Circuit(4)
     circuit.add(gates.RX(i, theta=0) for i in range(4))
     vqe = VQE(circuit, ham)
     qaoa = QAOA(ham)
     nvqe = dill.loads(dill.dumps(vqe))
     nqaoa = dill.loads(dill.dumps(qaoa))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_gates_abstract.py` & `qibo-0.1.9/src/qibo/tests/test_gates_abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Tests methods defined in `qibo/gates/abstract.py` and `qibo/gates/gates.py`."""
 import pytest
+
 from qibo import gates
 
 
-@pytest.mark.parametrize("gatename", ["H", "X", "Y", "Z",
-                                      "S", "SDG", "T", "TDG",
-                                      "I", "Align"])
+@pytest.mark.parametrize(
+    "gatename", ["H", "X", "Y", "Z", "S", "SDG", "T", "TDG", "I", "Align"]
+)
 def test_one_qubit_gates_init(gatename):
     gate = getattr(gates, gatename)(0)
     assert gate.target_qubits == (0,)
 
 
-@pytest.mark.parametrize("controls,instance",
-                         [((1,), "CNOT"), ((1, 2), "TOFFOLI"),
-                          ((1, 2, 4), "X")])
+@pytest.mark.parametrize(
+    "controls,instance", [((1,), "CNOT"), ((1, 2), "TOFFOLI"), ((1, 2, 4), "X")]
+)
 def test_x_controlled_by(controls, instance):
     gate = gates.X(0).controlled_by(*controls)
     assert gate.target_qubits == (0,)
     assert gate.control_qubits == controls
     assert isinstance(gate, getattr(gates, instance))
 
 
@@ -41,18 +42,18 @@
 def test_z_controlled_by(controls, instance):
     gate = gates.Z(0).controlled_by(*controls)
     assert gate.target_qubits == (0,)
     assert gate.control_qubits == controls
     assert isinstance(gate, getattr(gates, instance))
 
 
-@pytest.mark.parametrize("targets,p0,p1",
-                         [((0,), None, None),
-                          ((0, 1, 2), None, None),
-                          ((0, 3, 2), 0.2, 0.1)])
+@pytest.mark.parametrize(
+    "targets,p0,p1",
+    [((0,), None, None), ((0, 1, 2), None, None), ((0, 3, 2), 0.2, 0.1)],
+)
 def test_measurement_init(targets, p0, p1):
     # also tests `_get_bitflip_map`
     gate = gates.M(*targets, p0=p0, p1=p1)
     assert gate.target_qubits == targets
     p0map = {q: 0 if p0 is None else p0 for q in targets}
     p1map = {q: 0 if p1 is None else p1 for q in targets}
     assert gate.bitflip_map == (p0map, p1map)
@@ -72,40 +73,51 @@
 
 def test_measurement_add():
     gate = gates.M(0, 2)
     assert gate.target_qubits == (0, 2)
     assert gate.bitflip_map == 2 * ({0: 0, 2: 0},)
     gate.add(gates.M(1, 3, p0=0.3, p1=0.0))
     assert gate.target_qubits == (0, 2, 1, 3)
-    assert gate.bitflip_map == ({0: 0, 1: 0.3, 2: 0, 3: 0.3},
-                                {0: 0, 1: 0, 2: 0, 3: 0})
+    assert gate.bitflip_map == ({0: 0, 1: 0.3, 2: 0, 3: 0.3}, {0: 0, 1: 0, 2: 0, 3: 0})
 
 
 def test_measurement_errors():
     gate = gates.M(0)
     with pytest.raises(NotImplementedError):
         gate.controlled_by(1)
 
 
-@pytest.mark.parametrize("gatename,params",
-                         [("RX", (0.1234,)), ("RY", (0.1234,)),
-                          ("RZ", (0.1234,)), ("U1", (0.1234,)),
-                          ("U2", (0.1234, 0.4321)),
-                          ("U3", (0.1234, 0.4321, 0.5678))])
+@pytest.mark.parametrize(
+    "gatename,params",
+    [
+        ("RX", (0.1234,)),
+        ("RY", (0.1234,)),
+        ("RZ", (0.1234,)),
+        ("U1", (0.1234,)),
+        ("U2", (0.1234, 0.4321)),
+        ("U3", (0.1234, 0.4321, 0.5678)),
+    ],
+)
 def test_one_qubit_rotations_init(gatename, params):
     gate = getattr(gates, gatename)(0, *params)
     assert gate.target_qubits == (0,)
     assert gate.parameters == params
 
 
-@pytest.mark.parametrize("gatename,params",
-                         [("RX", (0.1234,)), ("RY", (0.1234,)),
-                          ("RZ", (0.1234,)), ("U1", (0.1234,)),
-                          ("U2", (0.1234, 0.4321)),
-                          ("U3", (0.1234, 0.4321, 0.5678))])
+@pytest.mark.parametrize(
+    "gatename,params",
+    [
+        ("RX", (0.1234,)),
+        ("RY", (0.1234,)),
+        ("RZ", (0.1234,)),
+        ("U1", (0.1234,)),
+        ("U2", (0.1234, 0.4321)),
+        ("U3", (0.1234, 0.4321, 0.5678)),
+    ],
+)
 def test_one_qubit_rotations_controlled_by(gatename, params):
     gate = getattr(gates, gatename)(0, *params).controlled_by(1)
     assert gate.target_qubits == (0,)
     assert gate.control_qubits == (1,)
     assert isinstance(gate, getattr(gates, f"C{gatename}"))
     gate = getattr(gates, gatename)(1, *params).controlled_by(0, 3)
     assert gate.target_qubits == (1,)
@@ -117,35 +129,44 @@
     gate = gates.CNOT(0, 1)
     assert gate.target_qubits == (1,)
     assert gate.control_qubits == (0,)
     gate = gates.CZ(3, 2)
     assert gate.target_qubits == (2,)
     assert gate.control_qubits == (3,)
 
+
 # :meth:`qibo.gates.CNOT.decompose` is tested in
 # ``test_x_decompose_with_cirq`` above
 
-@pytest.mark.parametrize("gatename,params",
-                         [("CRX", (0.1234,)), ("CRY", (0.1234,)),
-                          ("CRZ", (0.1234,)), ("CU1", (0.1234,)),
-                          ("CU2", (0.1234, 0.4321)),
-                          ("CU3", (0.1234, 0.4321, 0.5678))])
+
+@pytest.mark.parametrize(
+    "gatename,params",
+    [
+        ("CRX", (0.1234,)),
+        ("CRY", (0.1234,)),
+        ("CRZ", (0.1234,)),
+        ("CU1", (0.1234,)),
+        ("CU2", (0.1234, 0.4321)),
+        ("CU3", (0.1234, 0.4321, 0.5678)),
+    ],
+)
 def test_two_qubit_controlled_rotations_init(gatename, params):
     gate = getattr(gates, gatename)(0, 2, *params)
     assert gate.target_qubits == (2,)
     assert gate.control_qubits == (0,)
 
 
 def test_swap_init():
     gate = gates.SWAP(4, 3)
     assert gate.target_qubits == (4, 3)
 
 
 def test_fsim_init():
     import numpy as np
+
     gate = gates.fSim(0, 1, 0.1234, 0.4321)
     assert gate.target_qubits == (0, 1)
     matrix = np.random.random((2, 2))
     gate = gates.GeneralizedfSim(0, 1, matrix, 0.4321)
     assert gate.target_qubits == (0, 1)
     assert gate.parameters == (matrix, 0.4321)
     matrix = np.random.random((3, 3))
@@ -154,49 +175,58 @@
 
 
 def test_toffoli_init():
     gate = gates.TOFFOLI(0, 2, 1)
     assert gate.target_qubits == (1,)
     assert gate.control_qubits == (0, 2)
 
+
 # :meth:`qibo.gates.TOFFOLI.decompose` and
 # :meth:`qibo.gates.TOFFOLI.congruent`
 # are tested in `test_x_decompose_with_cirq`
 
+
 @pytest.mark.parametrize("targets", [(0,), (2, 0), (1, 3, 2)])
 def test_unitary_init(targets):
     import numpy as np
+
     matrix = np.random.random(2 * (2 ** len(targets),))
     gate = gates.Unitary(matrix, *targets)
     assert gate.target_qubits == targets
     assert gate.nparams == 4 ** len(targets)
 
 
 def test_kraus_channel_init():
     import numpy as np
-    ops = [((0,), np.random.random((2, 2))),
-           ((0, 1), np.random.random((4, 4))),
-           ((0, 2), np.random.random((4, 4))),
-           ((3,), np.random.random((2, 2)))]
+
+    ops = [
+        ((0,), np.random.random((2, 2))),
+        ((0, 1), np.random.random((4, 4))),
+        ((0, 2), np.random.random((4, 4))),
+        ((3,), np.random.random((2, 2))),
+    ]
     gate = gates.KrausChannel(ops)
     gate.target_qubits == (0, 1, 2, 3)
     for g in gate.gates:
         assert isinstance(g, gates.Unitary)
 
     ops.append(((4,), np.random.random((4, 4))))
     with pytest.raises(ValueError):
         gate = gates.KrausChannel(ops)
 
 
 def test_unitary_channel_init():
     import numpy as np
-    ops = [((0,), np.random.random((2, 2))),
-           ((0, 1), np.random.random((4, 4))),
-           ((0, 2), np.random.random((4, 4))),
-           ((3,), np.random.random((2, 2)))]
+
+    ops = [
+        ((0,), np.random.random((2, 2))),
+        ((0, 1), np.random.random((4, 4))),
+        ((0, 2), np.random.random((4, 4))),
+        ((3,), np.random.random((2, 2))),
+    ]
     gate = gates.UnitaryChannel(4 * [0.1], ops)
     gate.target_qubits == (0, 1, 2, 3)
     for g in gate.gates:
         assert isinstance(g, gates.Unitary)
 
     with pytest.raises(ValueError):
         gate = gates.UnitaryChannel(2 * [0.1], ops)
@@ -215,14 +245,15 @@
 def test_reset_channel_init():
     gate = gates.ResetChannel(0, 0.1, 0.2)
     assert gate.target_qubits == (0,)
 
 
 def test_qubit_getter_and_setter():
     from qibo.gates.abstract import Gate
+
     gate = Gate()
     gate.target_qubits = (0, 3)
     gate.control_qubits = (1, 4, 2)
     assert gate.qubits == (1, 2, 4, 0, 3)
 
     gate = Gate()
     with pytest.raises(ValueError):
@@ -234,14 +265,15 @@
     gate.target_qubits = (0, 1)
     with pytest.raises(ValueError):
         gate.control_qubits = (1,)
 
 
 def test_density_matrix_getter_and_setter():
     from qibo.gates.abstract import Gate
+
     gate = Gate()
     gate.target_qubits = (0, 1)
     gate.control_qubits = (2,)
     gate.density_matrix = True
 
 
 def test_gates_commute():
@@ -286,14 +318,15 @@
     decomp_gates = gates.H(0).decompose(1)
     assert len(decomp_gates) == 1
     assert isinstance(decomp_gates[0], gates.H)
 
 
 def test_special_gate():
     from qibo.gates.abstract import SpecialGate
+
     gate = SpecialGate()
     assert not gate.commutes(gates.H(0))
     with pytest.raises(NotImplementedError):
         gate.on_qubits({0: 0})
 
 
 def test_fused_gate():
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_gates_channels.py` & `qibo-0.1.9/src/qibo/tests/test_gates_channels.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 """Test channels defined in `qibo/gates.py`."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.tests.utils import random_density_matrix
 
 
 def test_general_channel(backend):
     a1 = np.sqrt(0.4) * np.array([[0, 1], [1, 0]])
-    a2 = np.sqrt(0.6) * np.array([[1, 0, 0, 0], [0, 1, 0, 0],
-                                  [0, 0, 0, 1], [0, 0, 1, 0]])
+    a2 = np.sqrt(0.6) * np.array(
+        [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]
+    )
     initial_rho = random_density_matrix(2)
     channel = gates.KrausChannel([((1,), a1), ((0, 1), a2)])
     assert channel.target_qubits == (0, 1)
     final_rho = backend.apply_channel_density_matrix(channel, np.copy(initial_rho), 2)
     m1 = np.kron(np.eye(2), backend.to_numpy(a1))
     m2 = backend.to_numpy(a2)
-    target_rho = (m1.dot(initial_rho).dot(m1.conj().T) +
-                  m2.dot(initial_rho).dot(m2.conj().T))
+    target_rho = m1.dot(initial_rho).dot(m1.conj().T) + m2.dot(initial_rho).dot(
+        m2.conj().T
+    )
     backend.assert_allclose(final_rho, target_rho)
 
 
 def test_krauss_channel_errors():
     a1 = np.sqrt(0.4) * np.array([[0, 1], [1, 0]])
     with pytest.raises(ValueError):
         gate = gates.KrausChannel([((0, 1), a1)])
 
 
+def test_depolarizing_channel_errors():
+    with pytest.raises(ValueError):
+        gate = gates.DepolarizingChannel((0, 1), 1.2)
+
+
 def test_controlled_by_channel_error():
     with pytest.raises(ValueError):
         gates.PauliNoiseChannel(0, px=0.5).controlled_by(1)
 
     a1 = np.sqrt(0.4) * np.array([[0, 1], [1, 0]])
-    a2 = np.sqrt(0.6) * np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1],
-                                  [0, 0, 1, 0]])
+    a2 = np.sqrt(0.6) * np.array(
+        [[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]]
+    )
     config = [((1,), a1), ((0, 1), a2)]
     with pytest.raises(ValueError):
         gates.KrausChannel(config).controlled_by(1)
 
 
 def test_unitary_channel(backend):
     a1 = np.array([[0, 1], [1, 0]])
     a2 = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
     probs = [0.4, 0.3]
     matrices = [((0,), a1), ((2, 3), a2)]
     initial_state = random_density_matrix(4)
     channel = gates.UnitaryChannel(probs, matrices)
-    final_state = backend.apply_channel_density_matrix(channel, np.copy(initial_state), 4)
+    final_state = backend.apply_channel_density_matrix(
+        channel, np.copy(initial_state), 4
+    )
 
     eye = np.eye(2)
     ma1 = np.kron(np.kron(a1, eye), np.kron(eye, eye))
     ma2 = np.kron(np.kron(eye, eye), a2)
-    target_state = (0.3 * initial_state
-                    + 0.4 * ma1.dot(initial_state.dot(ma1))
-                    + 0.3 * ma2.dot(initial_state.dot(ma2)))
+    target_state = (
+        0.3 * initial_state
+        + 0.4 * ma1.dot(initial_state.dot(ma1))
+        + 0.3 * ma2.dot(initial_state.dot(ma2))
+    )
     backend.assert_allclose(final_state, target_state)
 
 
 def test_unitary_channel_probability_tolerance(backend):
     """Create ``UnitaryChannel`` with probability sum within tolerance (see #562)."""
     nqubits = 2
     param = 0.006
@@ -94,14 +107,27 @@
     gate = gates.X(1)
     target_rho = backend.apply_gate_density_matrix(gate, np.copy(initial_rho), 2)
     target_rho = 0.3 * backend.to_numpy(target_rho)
     target_rho += 0.7 * initial_rho
     backend.assert_allclose(final_rho, target_rho)
 
 
+def test_depolarizing_channel(backend):
+    initial_rho = random_density_matrix(3)
+    lam = 0.3
+    initial_rho_r = np.einsum("ijik->jk", initial_rho.reshape([2, 4, 2, 4]))
+    channel = gates.DepolarizingChannel((1, 2), lam)
+    final_rho = backend.apply_channel_density_matrix(channel, np.copy(initial_rho), 3)
+    final_rho_r = np.einsum("ijik->jk", final_rho.reshape([2, 4, 2, 4]))
+    target_rho_r = (1 - lam) * initial_rho_r + lam * np.trace(
+        initial_rho_r
+    ) * np.identity(4) / 4
+    backend.assert_allclose(final_rho_r, target_rho_r)
+
+
 def test_reset_channel(backend):
     initial_rho = random_density_matrix(3)
     gate = gates.ResetChannel(0, p0=0.2, p1=0.2)
     final_rho = backend.reset_error_density_matrix(gate, np.copy(initial_rho), 3)
 
     trace = backend.to_numpy(backend.partial_trace_density_matrix(initial_rho, (0,), 3))
     trace = np.reshape(trace, 4 * (2,))
@@ -109,20 +135,23 @@
     ones = np.tensordot(trace, np.array([[0, 0], [0, 1]], dtype=trace.dtype), axes=0)
     zeros = np.transpose(zeros, [4, 0, 1, 5, 2, 3])
     ones = np.transpose(ones, [4, 0, 1, 5, 2, 3])
     target_rho = 0.6 * initial_rho + 0.2 * np.reshape(zeros + ones, initial_rho.shape)
     backend.assert_allclose(final_rho, target_rho)
 
 
-@pytest.mark.parametrize("t1,t2,time,excpop",
-                         [(0.8, 0.5, 1.0, 0.4), (0.5, 0.8, 1.0, 0.4)])
+@pytest.mark.parametrize(
+    "t1,t2,time,excpop", [(0.8, 0.5, 1.0, 0.4), (0.5, 0.8, 1.0, 0.4)]
+)
 def test_thermal_relaxation_channel(backend, t1, t2, time, excpop):
     """Check ``gates.ThermalRelaxationChannel`` on a 3-qubit random density matrix."""
     initial_rho = random_density_matrix(3)
-    gate = gates.ThermalRelaxationChannel(0, t1, t2, time=time, excited_population=excpop)
+    gate = gates.ThermalRelaxationChannel(
+        0, t1, t2, time=time, excited_population=excpop
+    )
     final_rho = gate.apply_density_matrix(backend, np.copy(initial_rho), 3)
 
     if t2 > t1:
         p0, p1, exp = gate.coefficients
         matrix = np.diag([1 - p1, p0, p1, 1 - p0])
         matrix[0, -1], matrix[-1, 0] = exp, exp
         matrix = matrix.reshape(4 * (2,))
@@ -131,29 +160,42 @@
         target_rho = np.einsum("abcd,aJKcjk->bJKdjk", matrix, target_rho)
         target_rho = target_rho.reshape(initial_rho.shape)
     else:
         p0, p1, pz = gate.coefficients
         mz = np.kron(np.array([[1, 0], [0, -1]]), np.eye(4))
         z_rho = mz.dot(initial_rho.dot(mz))
 
-        trace = backend.to_numpy(backend.partial_trace_density_matrix(initial_rho, (0,), 3))
+        trace = backend.to_numpy(
+            backend.partial_trace_density_matrix(initial_rho, (0,), 3)
+        )
         trace = np.reshape(trace, 4 * (2,))
-        zeros = np.tensordot(trace, np.array([[1, 0], [0, 0]], dtype=trace.dtype), axes=0)
-        ones = np.tensordot(trace, np.array([[0, 0], [0, 1]], dtype=trace.dtype), axes=0)
+        zeros = np.tensordot(
+            trace, np.array([[1, 0], [0, 0]], dtype=trace.dtype), axes=0
+        )
+        ones = np.tensordot(
+            trace, np.array([[0, 0], [0, 1]], dtype=trace.dtype), axes=0
+        )
         zeros = np.transpose(zeros, [4, 0, 1, 5, 2, 3])
         ones = np.transpose(ones, [4, 0, 1, 5, 2, 3])
 
         pi = 1 - p0 - p1 - pz
-        target_rho = pi * initial_rho + pz * z_rho 
+        target_rho = pi * initial_rho + pz * z_rho
         target_rho += np.reshape(p0 * zeros + p1 * ones, initial_rho.shape)
 
     backend.assert_allclose(final_rho, target_rho)
 
 
-@pytest.mark.parametrize("t1,t2,time,excpop",
-                         [(1.0, 0.5, 1.5, 1.5), (1.0, 0.5, -0.5, 0.5),
-                          (1.0, -0.5, 1.5, 0.5), (-1.0, 0.5, 1.5, 0.5),
-                          (1.0, 3.0, 1.5, 0.5)])
+@pytest.mark.parametrize(
+    "t1,t2,time,excpop",
+    [
+        (1.0, 0.5, 1.5, 1.5),
+        (1.0, 0.5, -0.5, 0.5),
+        (1.0, -0.5, 1.5, 0.5),
+        (-1.0, 0.5, 1.5, 0.5),
+        (1.0, 3.0, 1.5, 0.5),
+    ],
+)
 def test_thermal_relaxation_channel_errors(backend, t1, t2, time, excpop):
     with pytest.raises(ValueError):
         gate = gates.ThermalRelaxationChannel(
-            0, t1, t2, time, excited_population=excpop)
+            0, t1, t2, time, excited_population=excpop
+        )
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_gates_density_matrix.py` & `qibo-0.1.9/src/qibo/tests/test_gates_density_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Test gates acting on density matrices."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.config import raise_error
 from qibo.tests.utils import random_density_matrix
 
 _atol = 1e-8
 
+
 def apply_gates(backend, gatelist, nqubits=None, initial_state=None):
     state = backend.cast(np.copy(initial_state))
     for gate in gatelist:
         state = backend.apply_gate_density_matrix(gate, state, nqubits)
     return backend.to_numpy(state)
 
 
@@ -34,22 +36,35 @@
     phase = np.exp(1j * theta / 2.0)
     matrix = phase * np.array([[phase.real, -phase.imag], [phase.imag, phase.real]])
     target_rho = matrix.dot(initial_rho).dot(matrix.T.conj())
 
     backend.assert_allclose(final_rho, target_rho, atol=_atol)
 
 
-@pytest.mark.parametrize("gatename,gatekwargs",
-                         [("H", {}), ("X", {}), ("Y", {}), ("Z", {}),
-                          ("S", {}), ("SDG", {}), ("T", {}), ("TDG", {}),
-                          ("I", {}), ("Align", {}),
-                          ("RX", {"theta": 0.123}), ("RY", {"theta": 0.123}),
-                          ("RZ", {"theta": 0.123}), ("U1", {"theta": 0.123}),
-                          ("U2", {"phi": 0.123, "lam": 0.321}),
-                          ("U3", {"theta": 0.123, "phi": 0.321, "lam": 0.123})])
+@pytest.mark.parametrize(
+    "gatename,gatekwargs",
+    [
+        ("H", {}),
+        ("X", {}),
+        ("Y", {}),
+        ("Z", {}),
+        ("S", {}),
+        ("SDG", {}),
+        ("T", {}),
+        ("TDG", {}),
+        ("I", {}),
+        ("Align", {}),
+        ("RX", {"theta": 0.123}),
+        ("RY", {"theta": 0.123}),
+        ("RZ", {"theta": 0.123}),
+        ("U1", {"theta": 0.123}),
+        ("U2", {"phi": 0.123, "lam": 0.321}),
+        ("U3", {"theta": 0.123, "phi": 0.321, "lam": 0.123}),
+    ],
+)
 def test_one_qubit_gates(backend, gatename, gatekwargs):
     """Check applying one qubit gates to one qubit density matrix."""
     initial_rho = random_density_matrix(1)
     gate = getattr(gates, gatename)(0, **gatekwargs)
     final_rho = apply_gates(backend, [gate], 1, initial_rho)
 
     matrix = backend.to_numpy(gate.asmatrix(backend))
@@ -66,21 +81,29 @@
     matrix = backend.to_numpy(backend.asmatrix(getattr(gates, gatename)(1)))
     cmatrix = np.eye(4, dtype=matrix.dtype)
     cmatrix[2:, 2:] = matrix
     target_rho = np.einsum("ab,bc,cd->ad", cmatrix, initial_rho, cmatrix.conj().T)
     backend.assert_allclose(final_rho, target_rho)
 
 
-@pytest.mark.parametrize("gatename,gatekwargs",
-                         [("CNOT", {}), ("CZ", {}), ("SWAP", {}),
-                          ("CRX", {"theta": 0.123}), ("CRY", {"theta": 0.123}),
-                          ("CRZ", {"theta": 0.123}), ("CU1", {"theta": 0.123}),
-                          ("CU2", {"phi": 0.123, "lam": 0.321}),
-                          ("CU3", {"theta": 0.123, "phi": 0.321, "lam": 0.123}),
-                          ("fSim", {"theta": 0.123, "phi": 0.543})])
+@pytest.mark.parametrize(
+    "gatename,gatekwargs",
+    [
+        ("CNOT", {}),
+        ("CZ", {}),
+        ("SWAP", {}),
+        ("CRX", {"theta": 0.123}),
+        ("CRY", {"theta": 0.123}),
+        ("CRZ", {"theta": 0.123}),
+        ("CU1", {"theta": 0.123}),
+        ("CU2", {"phi": 0.123, "lam": 0.321}),
+        ("CU3", {"theta": 0.123, "phi": 0.321, "lam": 0.123}),
+        ("fSim", {"theta": 0.123, "phi": 0.543}),
+    ],
+)
 def test_two_qubit_gates(backend, gatename, gatekwargs):
     """Check applying two qubit gates to two qubit density matrix."""
     initial_rho = random_density_matrix(2)
     gate = getattr(gates, gatename)(0, 1, **gatekwargs)
     final_rho = apply_gates(backend, [gate], 2, initial_rho)
 
     matrix = backend.to_numpy(gate.asmatrix(backend))
@@ -98,15 +121,15 @@
     target_rho = np.einsum("ab,bc,cd->ad", matrix, initial_rho, matrix.conj().T)
     backend.assert_allclose(final_rho, target_rho)
 
 
 @pytest.mark.parametrize("nqubits", [1, 2, 3])
 def test_unitary_gate(backend, nqubits):
     """Check applying `gates.Unitary` to density matrix."""
-    shape = 2 * (2 ** nqubits,)
+    shape = 2 * (2**nqubits,)
     matrix = np.random.random(shape) + 1j * np.random.random(shape)
     initial_rho = random_density_matrix(nqubits)
     gate = gates.Unitary(matrix, *range(nqubits))
     final_rho = apply_gates(backend, [gate], nqubits, initial_rho)
     target_rho = np.einsum("ab,bc,cd->ad", matrix, initial_rho, matrix.conj().T)
     backend.assert_allclose(final_rho, target_rho)
 
@@ -125,14 +148,15 @@
     target_rho = matrix.dot(initial_rho).dot(matrix.T.conj())
     backend.assert_allclose(final_rho, target_rho)
 
 
 def test_controlled_by_no_effect(backend):
     """Check controlled_by SWAP that should not be applied."""
     from qibo.models import Circuit
+
     initial_rho = np.zeros((16, 16))
     initial_rho[0, 0] = 1
 
     c = Circuit(4, density_matrix=True)
     c.add(gates.X(0))
     c.add(gates.SWAP(1, 3).controlled_by(0, 2))
     final_rho = backend.execute_circuit(c, np.copy(initial_rho))
@@ -142,14 +166,15 @@
     target_rho = backend.execute_circuit(c, np.copy(initial_rho))
     backend.assert_allclose(final_rho, target_rho)
 
 
 def test_controlled_with_effect(backend):
     """Check controlled_by SWAP that should be applied."""
     from qibo.models import Circuit
+
     initial_rho = np.zeros((16, 16))
     initial_rho[0, 0] = 1
 
     c = Circuit(4, density_matrix=True)
     c.add(gates.X(0))
     c.add(gates.X(2))
     c.add(gates.SWAP(1, 3).controlled_by(0, 2))
@@ -164,14 +189,15 @@
 
 
 @pytest.mark.parametrize("nqubits", [4, 5])
 def test_controlled_by_random(backend, nqubits):
     """Check controlled_by method on gate."""
     from qibo.models import Circuit
     from qibo.tests.utils import random_state
+
     initial_psi = random_state(nqubits)
     initial_rho = np.outer(initial_psi, initial_psi.conj())
     c = Circuit(nqubits, density_matrix=True)
     c.add(gates.RX(1, theta=0.789).controlled_by(2))
     c.add(gates.fSim(0, 2, theta=0.123, phi=0.321).controlled_by(1, 3))
     final_rho = backend.execute_circuit(c, np.copy(initial_rho))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_gates_gates.py` & `qibo-0.1.9/src/qibo/tests/test_gates_gates.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Test gates defined in `qibo/gates/gates.py`."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.config import raise_error
 from qibo.tests.utils import random_state
 
 
 def apply_gates(backend, gatelist, nqubits=None, initial_state=None):
     if initial_state is None:
         state = backend.zero_state(nqubits)
     elif isinstance(initial_state, np.ndarray):
         state = backend.cast(np.copy(initial_state))
         if nqubits is None:
             nqubits = int(np.log2(len(state)))
-        else: # pragma: no cover
+        else:  # pragma: no cover
             assert nqubits == int(np.log2(len(state)))
-    else: # pragma: no cover
-        raise_error(TypeError, "Invalid initial state type {}."
-                               "".format(type(initial_state)))
+    else:  # pragma: no cover
+        raise_error(
+            TypeError, "Invalid initial state type {}." "".format(type(initial_state))
+        )
 
     for gate in gatelist:
         state = backend.apply_gate(gate, state, nqubits)
     return backend.to_numpy(state)
 
 
 def test_h(backend):
@@ -55,30 +57,32 @@
 def test_s(backend):
     final_state = apply_gates(backend, [gates.H(0), gates.H(1), gates.S(1)], nqubits=2)
     target_state = np.array([0.5, 0.5j, 0.5, 0.5j])
     backend.assert_allclose(final_state, target_state)
 
 
 def test_sdg(backend):
-    final_state = apply_gates(backend, [gates.H(0), gates.H(1), gates.SDG(1)], nqubits=2)
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.H(1), gates.SDG(1)], nqubits=2
+    )
     target_state = np.array([0.5, -0.5j, 0.5, -0.5j])
     backend.assert_allclose(final_state, target_state)
 
 
 def test_t(backend):
     final_state = apply_gates(backend, [gates.H(0), gates.H(1), gates.T(1)], nqubits=2)
-    target_state = np.array([0.5, (1 + 1j) / np.sqrt(8),
-                             0.5, (1 + 1j) / np.sqrt(8)])
+    target_state = np.array([0.5, (1 + 1j) / np.sqrt(8), 0.5, (1 + 1j) / np.sqrt(8)])
     backend.assert_allclose(final_state, target_state)
 
 
 def test_tdg(backend):
-    final_state = apply_gates(backend, [gates.H(0), gates.H(1), gates.TDG(1)], nqubits=2)
-    target_state = np.array([0.5, (1 - 1j) / np.sqrt(8),
-                             0.5, (1 - 1j) / np.sqrt(8)])
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.H(1), gates.TDG(1)], nqubits=2
+    )
+    target_state = np.array([0.5, (1 - 1j) / np.sqrt(8), 0.5, (1 - 1j) / np.sqrt(8)])
     backend.assert_allclose(final_state, target_state)
 
 
 def test_identity(backend):
     gatelist = [gates.H(0), gates.H(1), gates.I(0), gates.I(1)]
     final_state = apply_gates(backend, gatelist, nqubits=2)
     target_state = np.ones_like(final_state) / 2.0
@@ -96,30 +100,33 @@
     backend.assert_allclose(final_state, target_state)
     gate_matrix = gate.asmatrix(backend)
     backend.assert_allclose(gate_matrix, np.eye(4))
 
 
 # :class:`qibo.core.cgates.M` is tested seperately in `test_measurement_gate.py`
 
+
 def test_rx(backend):
     theta = 0.1234
-    final_state = apply_gates(backend, [gates.H(0), gates.RX(0, theta=theta)], nqubits=1)
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.RX(0, theta=theta)], nqubits=1
+    )
     phase = np.exp(1j * theta / 2.0)
-    gate = np.array([[phase.real, -1j * phase.imag],
-                    [-1j * phase.imag, phase.real]])
+    gate = np.array([[phase.real, -1j * phase.imag], [-1j * phase.imag, phase.real]])
     target_state = gate.dot(np.ones(2)) / np.sqrt(2)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_ry(backend):
     theta = 0.1234
-    final_state = apply_gates(backend, [gates.H(0), gates.RY(0, theta=theta)], nqubits=1)
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.RY(0, theta=theta)], nqubits=1
+    )
     phase = np.exp(1j * theta / 2.0)
-    gate = np.array([[phase.real, -phase.imag],
-                     [phase.imag, phase.real]])
+    gate = np.array([[phase.real, -phase.imag], [phase.imag, phase.real]])
     target_state = gate.dot(np.ones(2)) / np.sqrt(2)
     backend.assert_allclose(final_state, target_state)
 
 
 @pytest.mark.parametrize("applyx", [True, False])
 def test_rz(backend, applyx):
     theta = 0.1234
@@ -143,33 +150,39 @@
     backend.assert_allclose(final_state, target_state)
 
 
 def test_u2(backend):
     phi = 0.1234
     lam = 0.4321
     initial_state = random_state(1)
-    final_state = apply_gates(backend, [gates.U2(0, phi, lam)], initial_state=initial_state)
-    matrix = np.array([[np.exp(-1j * (phi + lam) / 2), -np.exp(-1j * (phi - lam) / 2)],
-                       [np.exp(1j * (phi - lam) / 2), np.exp(1j * (phi + lam) / 2)]])
+    final_state = apply_gates(
+        backend, [gates.U2(0, phi, lam)], initial_state=initial_state
+    )
+    matrix = np.array(
+        [
+            [np.exp(-1j * (phi + lam) / 2), -np.exp(-1j * (phi - lam) / 2)],
+            [np.exp(1j * (phi - lam) / 2), np.exp(1j * (phi + lam) / 2)],
+        ]
+    )
     target_state = matrix.dot(initial_state) / np.sqrt(2)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_u3(backend):
     theta = 0.1111
     phi = 0.1234
     lam = 0.4321
     initial_state = random_state(1)
-    final_state = apply_gates(backend, [gates.U3(0, theta, phi, lam)],
-                              initial_state=initial_state)
+    final_state = apply_gates(
+        backend, [gates.U3(0, theta, phi, lam)], initial_state=initial_state
+    )
     cost, sint = np.cos(theta / 2), np.sin(theta / 2)
     ep = np.exp(1j * (phi + lam) / 2)
     em = np.exp(1j * (phi - lam) / 2)
-    matrix = np.array([[ep.conj() * cost, - em.conj() * sint],
-                       [em * sint, ep * cost]])
+    matrix = np.array([[ep.conj() * cost, -em.conj() * sint], [em * sint, ep * cost]])
     target_state = matrix.dot(initial_state)
     backend.assert_allclose(final_state, target_state)
 
 
 @pytest.mark.parametrize("applyx", [False, True])
 def test_cnot(backend, applyx):
     if applyx:
@@ -194,21 +207,25 @@
     else:
         gate = gates.CZ(0, 1)
     final_state = apply_gates(backend, [gate], initial_state=initial_state)
     assert gate.name == "cz"
     backend.assert_allclose(final_state, target_state)
 
 
-@pytest.mark.parametrize("name,params",
-                         [("CRX", {"theta": 0.1}),
-                          ("CRY", {"theta": 0.2}),
-                          ("CRZ", {"theta": 0.3}),
-                          ("CU1", {"theta": 0.1}),
-                          ("CU2", {"phi": 0.1, "lam": 0.2}),
-                          ("CU3", {"theta": 0.1, "phi": 0.2, "lam": 0.3})])
+@pytest.mark.parametrize(
+    "name,params",
+    [
+        ("CRX", {"theta": 0.1}),
+        ("CRY", {"theta": 0.2}),
+        ("CRZ", {"theta": 0.3}),
+        ("CU1", {"theta": 0.1}),
+        ("CU2", {"phi": 0.1, "lam": 0.2}),
+        ("CU3", {"theta": 0.1, "phi": 0.2, "lam": 0.3}),
+    ],
+)
 def test_cun(backend, name, params):
     initial_state = random_state(2)
     gate = getattr(gates, name)(0, 1, **params)
     final_state = apply_gates(backend, [gate], initial_state=initial_state)
     target_state = np.dot(gate.asmatrix(backend), initial_state)
     backend.assert_allclose(final_state, target_state)
 
@@ -217,15 +234,17 @@
     final_state = apply_gates(backend, [gates.X(1), gates.SWAP(0, 1)], nqubits=2)
     target_state = np.zeros_like(final_state)
     target_state[2] = 1.0
     backend.assert_allclose(final_state, target_state)
 
 
 def test_fswap(backend):
-    final_state = apply_gates(backend, [gates.H(0), gates.X(1), gates.FSWAP(0, 1)], nqubits=2)
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.X(1), gates.FSWAP(0, 1)], nqubits=2
+    )
     target_state = np.zeros_like(final_state)
     target_state[2] = 1.0 / np.sqrt(2)
     target_state[3] = -1.0 / np.sqrt(2)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_multiple_swap(backend):
@@ -238,16 +257,17 @@
 
 def test_fsim(backend):
     theta = 0.1234
     phi = 0.4321
     gatelist = [gates.H(0), gates.H(1), gates.fSim(0, 1, theta, phi)]
     final_state = apply_gates(backend, gatelist, nqubits=2)
     target_state = np.ones_like(final_state) / 2.0
-    rotation = np.array([[np.cos(theta), -1j * np.sin(theta)],
-                         [-1j * np.sin(theta), np.cos(theta)]])
+    rotation = np.array(
+        [[np.cos(theta), -1j * np.sin(theta)], [-1j * np.sin(theta), np.cos(theta)]]
+    )
     matrix = np.eye(4, dtype=target_state.dtype)
     matrix[1:3, 1:3] = rotation
     matrix[3, 3] = np.exp(-1j * phi)
     target_state = matrix.dot(target_state)
     backend.assert_allclose(final_state, target_state)
 
 
@@ -273,14 +293,61 @@
     backend.assert_allclose(gate.parameters[0], matrix)
     assert gate.parameters[1] == phi
     matrix = np.random.random((4, 4))
     with pytest.raises(ValueError):
         gate = gates.GeneralizedfSim(0, 1, matrix, phi)
 
 
+def test_rxx(backend):
+    theta = 0.1234
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.H(1), gates.RXX(0, 1, theta=theta)], nqubits=2
+    )
+    phase = np.exp(1j * theta / 2.0)
+    gate = np.array(
+        [
+            [phase.real, 0, 0, -1j * phase.imag],
+            [0, phase.real, -1j * phase.imag, 0],
+            [0, -1j * phase.imag, phase.real, 0],
+            [-1j * phase.imag, 0, 0, phase.real],
+        ]
+    )
+    target_state = gate.dot(np.ones(4)) / 2.0
+    backend.assert_allclose(final_state, target_state)
+
+
+def test_ryy(backend):
+    theta = 0.1234
+    final_state = apply_gates(
+        backend, [gates.H(0), gates.H(1), gates.RYY(0, 1, theta=theta)], nqubits=2
+    )
+    phase = np.exp(1j * theta / 2.0)
+    gate = np.array(
+        [
+            [phase.real, 0, 0, 1j * phase.imag],
+            [0, phase.real, -1j * phase.imag, 0],
+            [0, -1j * phase.imag, phase.real, 0],
+            [1j * phase.imag, 0, 0, phase.real],
+        ]
+    )
+    target_state = gate.dot(np.ones(4)) / 2.0
+    backend.assert_allclose(final_state, target_state)
+
+
+# @pytest.mark.parametrize("applyx", [True, False])
+def test_rzz(backend):
+    theta = 0.1234
+    final_state = apply_gates(
+        backend, [gates.X(0), gates.X(1), gates.RZZ(0, 1, theta=theta)], nqubits=2
+    )
+    target_state = np.zeros_like(final_state)
+    target_state[3] = np.exp(-1j * theta / 2.0)
+    backend.assert_allclose(final_state, target_state)
+
+
 @pytest.mark.parametrize("applyx", [False, True])
 def test_toffoli(backend, applyx):
     if applyx:
         gatelist = [gates.X(0), gates.X(1), gates.TOFFOLI(0, 1, 2)]
     else:
         gatelist = [gates.X(1), gates.TOFFOLI(0, 1, 2)]
     final_state = apply_gates(backend, gatelist, nqubits=3)
@@ -290,15 +357,15 @@
     else:
         target_state[2] = 1
     backend.assert_allclose(final_state, target_state)
 
 
 @pytest.mark.parametrize("nqubits", [2, 3])
 def test_unitary(backend, nqubits):
-    initial_state = np.ones(2 ** nqubits) / np.sqrt(2 ** nqubits)
+    initial_state = np.ones(2**nqubits) / np.sqrt(2**nqubits)
     matrix = np.random.random(2 * (2 ** (nqubits - 1),))
     target_state = np.kron(np.eye(2), matrix).dot(initial_state)
     gatelist = [gates.H(i) for i in range(nqubits)]
     gatelist.append(gates.Unitary(matrix, *range(1, nqubits), name="random"))
     final_state = apply_gates(backend, gatelist, nqubits=nqubits)
     backend.assert_allclose(final_state, target_state)
 
@@ -307,32 +374,40 @@
     matrix = np.random.random((4, 4))
     gate = gates.Unitary(matrix, 0, 1)
     backend.assert_allclose(gate.parameters[0], matrix)
 
 
 def test_unitary_common_gates(backend):
     target_state = apply_gates(backend, [gates.X(0), gates.H(1)], nqubits=2)
-    gatelist = [gates.Unitary(np.array([[0, 1], [1, 0]]), 0),
-                gates.Unitary(np.array([[1, 1], [1, -1]]) / np.sqrt(2), 1)]
+    gatelist = [
+        gates.Unitary(np.array([[0, 1], [1, 0]]), 0),
+        gates.Unitary(np.array([[1, 1], [1, -1]]) / np.sqrt(2), 1),
+    ]
     final_state = apply_gates(backend, gatelist, nqubits=2)
     backend.assert_allclose(final_state, target_state)
 
     thetax = 0.1234
     thetay = 0.4321
-    gatelist = [gates.RX(0, theta=thetax), gates.RY(1, theta=thetay),
-                gates.CNOT(0, 1)]
+    gatelist = [gates.RX(0, theta=thetax), gates.RY(1, theta=thetay), gates.CNOT(0, 1)]
     target_state = apply_gates(backend, gatelist, nqubits=2)
 
-    rx = np.array([[np.cos(thetax / 2), -1j * np.sin(thetax / 2)],
-                   [-1j * np.sin(thetax / 2), np.cos(thetax / 2)]])
-    ry = np.array([[np.cos(thetay / 2), -np.sin(thetay / 2)],
-                   [np.sin(thetay / 2), np.cos(thetay / 2)]])
+    rx = np.array(
+        [
+            [np.cos(thetax / 2), -1j * np.sin(thetax / 2)],
+            [-1j * np.sin(thetax / 2), np.cos(thetax / 2)],
+        ]
+    )
+    ry = np.array(
+        [
+            [np.cos(thetay / 2), -np.sin(thetay / 2)],
+            [np.sin(thetay / 2), np.cos(thetay / 2)],
+        ]
+    )
     cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
-    gatelist = [gates.Unitary(rx, 0), gates.Unitary(ry, 1),
-                gates.Unitary(cnot, 0, 1)]
+    gatelist = [gates.Unitary(rx, 0), gates.Unitary(ry, 1), gates.Unitary(cnot, 0, 1)]
     final_state = apply_gates(backend, gatelist, nqubits=2)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_unitary_multiqubit(backend):
     gatelist = [gates.H(i) for i in range(4)]
     gatelist.append(gates.CNOT(0, 1))
@@ -349,18 +424,24 @@
     final_state = apply_gates(backend, [unitary], nqubits=4)
     target_state = apply_gates(backend, gatelist, nqubits=4)
     backend.assert_allclose(final_state, target_state)
 
 
 ############################# Test ``controlled_by`` #############################
 
+
 def test_controlled_x(backend):
-    gatelist = [gates.X(0), gates.X(1), gates.X(2),
-                gates.X(3).controlled_by(0, 1, 2),
-                gates.X(0), gates.X(2)]
+    gatelist = [
+        gates.X(0),
+        gates.X(1),
+        gates.X(2),
+        gates.X(3).controlled_by(0, 1, 2),
+        gates.X(0),
+        gates.X(2),
+    ]
     final_state = apply_gates(backend, gatelist, nqubits=4)
     gatelist = [gates.X(1), gates.X(3)]
     target_state = apply_gates(backend, gatelist, nqubits=4)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_controlled_x_vs_cnot(backend):
@@ -414,43 +495,51 @@
 def test_controlled_u2(backend):
     phi = 0.1234
     lam = 0.4321
     gatelist = [gates.X(0), gates.X(1)]
     gatelist.append(gates.U2(2, phi, lam).controlled_by(0, 1))
     gatelist.extend([gates.X(0), gates.X(1)])
     final_state = apply_gates(backend, gatelist, nqubits=3)
-    gatelist = [gates.X(0), gates.X(1), gates.U2(2, phi, lam),
-                gates.X(0), gates.X(1)]
+    gatelist = [gates.X(0), gates.X(1), gates.U2(2, phi, lam), gates.X(0), gates.X(1)]
     target_state = apply_gates(backend, gatelist, nqubits=3)
     backend.assert_allclose(final_state, target_state)
     # for coverage
     gate = gates.CU2(0, 1, phi, lam)
     assert gate.parameters == (phi, lam)
 
 
 def test_controlled_u3(backend):
     theta, phi, lam = 0.1, 0.1234, 0.4321
     initial_state = random_state(2)
-    final_state = apply_gates(backend, [gates.U3(1, theta, phi, lam).controlled_by(0)], 2, initial_state)
-    target_state = apply_gates(backend, [gates.CU3(0, 1, theta, phi, lam)], 2, initial_state)
+    final_state = apply_gates(
+        backend, [gates.U3(1, theta, phi, lam).controlled_by(0)], 2, initial_state
+    )
+    target_state = apply_gates(
+        backend, [gates.CU3(0, 1, theta, phi, lam)], 2, initial_state
+    )
     backend.assert_allclose(final_state, target_state)
     # for coverage
     gate = gates.U3(0, theta, phi, lam)
     assert gate.parameters == (theta, phi, lam)
 
 
 @pytest.mark.parametrize("applyx", [False, True])
 @pytest.mark.parametrize("free_qubit", [False, True])
 def test_controlled_swap(backend, applyx, free_qubit):
     f = int(free_qubit)
     gatelist = []
     if applyx:
         gatelist.append(gates.X(0))
-    gatelist.extend([gates.RX(1 + f, theta=0.1234), gates.RY(2 + f, theta=0.4321),
-                     gates.SWAP(1 + f, 2 + f).controlled_by(0)])
+    gatelist.extend(
+        [
+            gates.RX(1 + f, theta=0.1234),
+            gates.RY(2 + f, theta=0.4321),
+            gates.SWAP(1 + f, 2 + f).controlled_by(0),
+        ]
+    )
     final_state = apply_gates(backend, gatelist, 3 + f)
     gatelist = [gates.RX(1 + f, theta=0.1234), gates.RY(2 + f, theta=0.4321)]
     if applyx:
         gatelist.extend([gates.X(0), gates.SWAP(1 + f, 2 + f)])
     target_state = apply_gates(backend, gatelist, 3 + f)
     backend.assert_allclose(final_state, target_state)
 
@@ -475,31 +564,31 @@
 
 def test_controlled_fsim(backend):
     theta, phi = 0.1234, 0.4321
     gatelist = [gates.H(i) for i in range(6)]
     gatelist.append(gates.fSim(5, 3, theta, phi).controlled_by(0, 2, 1))
     final_state = apply_gates(backend, gatelist, 6)
 
-    target_state = np.ones_like(final_state) / np.sqrt(2 ** 6)
-    rotation = np.array([[np.cos(theta), -1j * np.sin(theta)],
-                         [-1j * np.sin(theta), np.cos(theta)]])
+    target_state = np.ones_like(final_state) / np.sqrt(2**6)
+    rotation = np.array(
+        [[np.cos(theta), -1j * np.sin(theta)], [-1j * np.sin(theta), np.cos(theta)]]
+    )
     matrix = np.eye(4, dtype=target_state.dtype)
     matrix[1:3, 1:3] = rotation
     matrix[3, 3] = np.exp(-1j * phi)
     ids = [56, 57, 60, 61]
     target_state[ids] = matrix.dot(target_state[ids])
     ids = [58, 59, 62, 63]
     target_state[ids] = matrix.dot(target_state[ids])
     backend.assert_allclose(final_state, target_state)
 
 
 def test_controlled_unitary(backend):
     matrix = np.random.random((2, 2))
-    gatelist = [gates.H(0), gates.H(1),
-                gates.Unitary(matrix, 1).controlled_by(0)]
+    gatelist = [gates.H(0), gates.H(1), gates.Unitary(matrix, 1).controlled_by(0)]
     final_state = apply_gates(backend, gatelist, 2)
     target_state = np.ones_like(final_state) / 2.0
     target_state[2:] = matrix.dot(target_state[2:])
     backend.assert_allclose(final_state, target_state)
 
     matrix = np.random.random((4, 4))
     gatelist = [gates.H(i) for i in range(4)]
@@ -516,14 +605,15 @@
     matrix = np.random.random((2, 2))
     gate = gates.Unitary(matrix, 1).controlled_by(0)
     target_state = apply_gates(backend, [gate], 2, initial_state)
     u = backend.control_matrix(gate)
     final_state = np.dot(u, initial_state)
     backend.assert_allclose(final_state, target_state)
 
+
 ###############################################################################
 
 ################################# Test dagger #################################
 GATES = [
     ("H", (0,)),
     ("X", (0,)),
     ("Y", (0,)),
@@ -540,16 +630,21 @@
     ("U3", (0, 0.1, 0.2, 0.3)),
     ("CNOT", (0, 1)),
     ("CRX", (0, 1, 0.1)),
     ("CRZ", (0, 1, 0.3)),
     ("CU1", (0, 1, 0.1)),
     ("CU2", (0, 1, 0.2, 0.3)),
     ("CU3", (0, 1, 0.1, 0.2, 0.3)),
-    ("fSim", (0, 1, 0.1, 0.2))
+    ("fSim", (0, 1, 0.1, 0.2)),
+    ("RXX", (0, 1, 0.1)),
+    ("RYY", (0, 1, 0.2)),
+    ("RZZ", (0, 1, 0.3)),
 ]
+
+
 @pytest.mark.parametrize("gate,args", GATES)
 def test_dagger(backend, gate, args):
     gate = getattr(gates, gate)(*args)
     nqubits = len(gate.qubits)
     initial_state = random_state(nqubits)
     final_state = apply_gates(backend, [gate, gate.dagger()], nqubits, initial_state)
     backend.assert_allclose(final_state, initial_state)
@@ -561,16 +656,18 @@
     ("Y", (3,)),
     ("S", (3,)),
     ("SDG", (3,)),
     ("T", (3,)),
     ("TDG", (3,)),
     ("RX", (3, 0.1)),
     ("U1", (3, 0.1)),
-    ("U3", (3, 0.1, 0.2, 0.3))
+    ("U3", (3, 0.1, 0.2, 0.3)),
 ]
+
+
 @pytest.mark.parametrize("gate,args", GATES)
 def test_controlled_dagger(backend, gate, args):
     gate = getattr(gates, gate)(*args).controlled_by(0, 1, 2)
     initial_state = random_state(4)
     final_state = apply_gates(backend, [gate, gate.dagger()], 4, initial_state)
     backend.assert_allclose(final_state, initial_state)
 
@@ -583,60 +680,70 @@
     initial_state = random_state(qubit + 1)
     final_state = apply_gates(backend, [gate_1, gate_2], qubit + 1, initial_state)
     backend.assert_allclose(final_state, initial_state)
 
 
 @pytest.mark.parametrize("nqubits", [1, 2])
 def test_unitary_dagger(backend, nqubits):
-    matrix = np.random.random((2 ** nqubits, 2 ** nqubits))
+    matrix = np.random.random((2**nqubits, 2**nqubits))
     gate = gates.Unitary(matrix, *range(nqubits))
     initial_state = random_state(nqubits)
     final_state = apply_gates(backend, [gate, gate.dagger()], nqubits, initial_state)
     target_state = np.dot(matrix, initial_state)
     target_state = np.dot(np.conj(matrix).T, target_state)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_controlled_unitary_dagger(backend):
     from scipy.linalg import expm
+
     matrix = np.random.random((2, 2))
     matrix = expm(1j * (matrix + matrix.T))
     gate = gates.Unitary(matrix, 0).controlled_by(1, 2, 3, 4)
     initial_state = random_state(5)
     final_state = apply_gates(backend, [gate, gate.dagger()], 5, initial_state)
     backend.assert_allclose(final_state, initial_state)
 
 
 def test_generalizedfsim_dagger(backend):
     from scipy.linalg import expm
+
     phi = 0.2
     matrix = np.random.random((2, 2))
     matrix = expm(1j * (matrix + matrix.T))
     gate = gates.GeneralizedfSim(0, 1, matrix, phi)
     initial_state = random_state(2)
     final_state = apply_gates(backend, [gate, gate.dagger()], 2, initial_state)
     backend.assert_allclose(final_state, initial_state)
 
+
 ###############################################################################
 
 ########################### Test gate decomposition ###########################
 
-@pytest.mark.parametrize(("target", "controls", "free"),
-                         [(0, (1,), ()), (2, (0, 1), ()),
-                          (3, (0, 1, 4), (2, 5)),
-                          (7, (0, 1, 2, 3, 4), (5, 6)),
-                          (5, (0, 2, 4, 6, 7), (1, 3)),
-                          (8, (0, 2, 4, 6, 9), (3, 5, 7))])
+
+@pytest.mark.parametrize(
+    ("target", "controls", "free"),
+    [
+        (0, (1,), ()),
+        (2, (0, 1), ()),
+        (3, (0, 1, 4), (2, 5)),
+        (7, (0, 1, 2, 3, 4), (5, 6)),
+        (5, (0, 2, 4, 6, 7), (1, 3)),
+        (8, (0, 2, 4, 6, 9), (3, 5, 7)),
+    ],
+)
 @pytest.mark.parametrize("use_toffolis", [True, False])
 def test_x_decomposition_execution(backend, target, controls, free, use_toffolis):
     """Check that applying the decomposition is equivalent to applying the multi-control gate."""
     gate = gates.X(target).controlled_by(*controls)
     nqubits = max((target,) + controls + free) + 1
     initial_state = random_state(nqubits)
     target_state = backend.apply_gate(gate, np.copy(initial_state), nqubits)
     dgates = gate.decompose(*free, use_toffolis=use_toffolis)
     final_state = np.copy(initial_state)
     for gate in dgates:
         final_state = backend.apply_gate(gate, final_state, nqubits)
     backend.assert_allclose(final_state, target_state, atol=1e-6)
 
+
 ###############################################################################
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_gates_special.py` & `qibo-0.1.9/src/qibo/tests/test_gates_special.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 from qibo.tests.utils import random_state
 
 
 def test_callback_gate_errors():
     from qibo import callbacks
+
     entropy = callbacks.EntanglementEntropy([0])
     gate = gates.CallbackGate(entropy)
     with pytest.raises(NotImplementedError):
         gate.on_qubits(2)
 
 
 @pytest.mark.parametrize("nqubits", [2, 3])
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_global_backend.py` & `qibo-0.1.9/src/qibo/tests/test_global_backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import pytest
+
 import qibo
 from qibo import matrices
 
 
 def test_set_backend():
     from qibo.backends import GlobalBackend
+
     backend = GlobalBackend()
     qibo.set_backend("numpy")
     assert qibo.get_backend() == "numpy"
     assert GlobalBackend().name == "numpy"
 
 
 def test_set_precision():
     import numpy as np
+
     assert qibo.get_precision() == "double"
     qibo.set_precision("single")
     assert matrices.I.dtype == np.complex64
     assert qibo.get_precision() == "single"
     qibo.set_precision("double")
     assert matrices.I.dtype == np.complex128
     assert qibo.get_precision() == "double"
@@ -47,29 +50,31 @@
 
 
 def test_set_shot_batch_size():
     original_batch_size = qibo.get_batch_size()
     qibo.set_batch_size(1024)
     assert qibo.get_batch_size() == 1024
     from qibo.config import SHOT_BATCH_SIZE
+
     assert SHOT_BATCH_SIZE == 1024
     with pytest.raises(TypeError):
         qibo.set_batch_size("test")
     with pytest.raises(ValueError):
         qibo.set_batch_size(-10)
     with pytest.raises(ValueError):
-        qibo.set_batch_size(2 ** 35)
+        qibo.set_batch_size(2**35)
     qibo.set_batch_size(original_batch_size)
 
 
 def test_set_metropolis_threshold():
     original_threshold = qibo.get_metropolis_threshold()
     qibo.set_metropolis_threshold(100)
     assert qibo.get_metropolis_threshold() == 100
     from qibo.config import SHOT_METROPOLIS_THRESHOLD
+
     assert SHOT_METROPOLIS_THRESHOLD == 100
     with pytest.raises(TypeError):
         qibo.set_metropolis_threshold("test")
     with pytest.raises(ValueError):
         qibo.set_metropolis_threshold(-10)
     qibo.set_metropolis_threshold(original_threshold)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,62 @@
 """Test methods in `qibo/core/hamiltonians.py`."""
-import pytest
 import numpy as np
-from qibo import hamiltonians
+import pytest
+
+from qibo import gates, hamiltonians
+from qibo.models import Circuit
+from qibo.symbols import I, Z
 from qibo.tests.utils import random_complex, random_sparse_matrix
 
 
 def test_hamiltonian_init(backend):
     with pytest.raises(TypeError):
         H = hamiltonians.Hamiltonian(2, "test", backend=backend)
     with pytest.raises(ValueError):
         H1 = hamiltonians.Hamiltonian(-2, np.eye(4), backend=backend)
     with pytest.raises(RuntimeError):
         H2 = hamiltonians.Hamiltonian(np.eye(2), np.eye(4), backend=backend)
     with pytest.raises(ValueError):
         H3 = hamiltonians.Hamiltonian(4, np.eye(10), backend=backend)
 
 
-@pytest.mark.parametrize("dtype", [np.int, np.float, np.complex, np.int32,
-                                   np.int64, np.float32, np.float64,
-                                   np.complex64, np.complex128])
+@pytest.mark.parametrize(
+    "dtype",
+    [
+        np.int,
+        np.float,
+        np.complex,
+        np.int32,
+        np.int64,
+        np.float32,
+        np.float64,
+        np.complex64,
+        np.complex128,
+    ],
+)
 @pytest.mark.parametrize("sparse_type", [None, "coo", "csr", "csc", "dia"])
 def test_hamiltonian_algebraic_operations(backend, dtype, sparse_type):
     """Test basic hamiltonian overloading."""
+
     def transformation_a(a, b):
         c1 = dtype(0.1)
         return a + c1 * b
+
     def transformation_b(a, b):
         c1 = dtype(2)
         c2 = dtype(3.5)
         return c1 * a - b * c2
+
     def transformation_c(a, b, use_eye=False):
         c1 = dtype(4.5)
         if use_eye:
             return a + c1 * backend.matrices.I(a.shape[0]) - b
         else:
             return a + c1 - b
+
     def transformation_d(a, b, use_eye=False):
         c1 = dtype(10.5)
         c2 = dtype(2)
         if use_eye:
             return c1 * backend.matrices.I(a.shape[0]) - a + c2 * b
         else:
             return c1 - a + c2 * b
@@ -75,18 +93,24 @@
 def test_hamiltonian_addition(backend, sparse_type):
     if sparse_type is None:
         H1 = hamiltonians.Y(nqubits=3, backend=backend)
         H2 = hamiltonians.TFIM(nqubits=3, h=1.0, backend=backend)
     else:
         if backend.name == "tensorflow":
             pytest.skip("Tensorflow does not support operations with sparse matrices.")
-        H1 = hamiltonians.Hamiltonian(6,random_sparse_matrix(backend, 64, sparse_type=sparse_type),
-                                      backend=backend)
-        H2 = hamiltonians.Hamiltonian(6, random_sparse_matrix(backend, 64, sparse_type=sparse_type),
-                                      backend=backend)
+        H1 = hamiltonians.Hamiltonian(
+            6,
+            random_sparse_matrix(backend, 64, sparse_type=sparse_type),
+            backend=backend,
+        )
+        H2 = hamiltonians.Hamiltonian(
+            6,
+            random_sparse_matrix(backend, 64, sparse_type=sparse_type),
+            backend=backend,
+        )
 
     H = H1 + H2
     matrix = H1.matrix + H2.matrix
     backend.assert_allclose(H.matrix, matrix)
     H = H1 - 0.5 * H2
     matrix = H1.matrix - 0.5 * H2.matrix
     backend.assert_allclose(H.matrix, matrix)
@@ -119,83 +143,98 @@
     """Test matrix multiplication between Hamiltonians."""
     if sparse_type is None:
         nqubits = 3
         H1 = hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
         H2 = hamiltonians.Y(nqubits, backend=backend)
     else:
         nqubits = 5
-        nstates = 2 ** nqubits
-        H1 = hamiltonians.Hamiltonian(nqubits, random_sparse_matrix(backend, nstates, sparse_type),
-                                      backend=backend)
-        H2 = hamiltonians.Hamiltonian(nqubits, random_sparse_matrix(backend, nstates, sparse_type),
-                                      backend=backend)
+        nstates = 2**nqubits
+        H1 = hamiltonians.Hamiltonian(
+            nqubits,
+            random_sparse_matrix(backend, nstates, sparse_type),
+            backend=backend,
+        )
+        H2 = hamiltonians.Hamiltonian(
+            nqubits,
+            random_sparse_matrix(backend, nstates, sparse_type),
+            backend=backend,
+        )
 
     m1 = backend.to_numpy(H1.matrix)
     m2 = backend.to_numpy(H2.matrix)
     if backend.name == "tensorflow" and sparse_type is not None:
         with pytest.raises(NotImplementedError):
             _ = H1 @ H2
     else:
         backend.assert_allclose((H1 @ H2).matrix, (m1 @ m2))
         backend.assert_allclose((H2 @ H1).matrix, (m2 @ m1))
 
     with pytest.raises(ValueError):
-        H1 @ np.zeros(3 * (2 ** nqubits,), dtype=m1.dtype)
+        H1 @ np.zeros(3 * (2**nqubits,), dtype=m1.dtype)
     with pytest.raises(NotImplementedError):
         H1 @ 2
 
 
 @pytest.mark.parametrize("sparse_type", [None, "coo", "csr", "csc", "dia"])
 def test_hamiltonian_matmul_states(backend, sparse_type):
     """Test matrix multiplication between Hamiltonian and states."""
     if sparse_type is None:
         nqubits = 3
         H = hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     else:
         if backend.name == "tensorflow":
             pytest.skip("Tensorflow does not support operations with sparse matrices.")
         nqubits = 5
-        nstates = 2 ** nqubits
+        nstates = 2**nqubits
         matrix = random_sparse_matrix(backend, nstates, sparse_type)
         H = hamiltonians.Hamiltonian(nqubits, matrix, backend=backend)
 
     hm = backend.to_numpy(H.matrix)
-    v = random_complex(2 ** nqubits, dtype=hm.dtype)
-    m = random_complex((2 ** nqubits, 2 ** nqubits), dtype=hm.dtype)
+    v = random_complex(2**nqubits, dtype=hm.dtype)
+    m = random_complex((2**nqubits, 2**nqubits), dtype=hm.dtype)
     Hv = H @ backend.cast(v)
     Hm = H @ backend.cast(m)
     backend.assert_allclose(Hv, hm.dot(v))
     backend.assert_allclose(Hm, (hm @ m))
 
     Hstate = H @ backend.cast(v)
     backend.assert_allclose(Hstate, hm.dot(v))
 
 
 @pytest.mark.parametrize("density_matrix", [True, False])
-@pytest.mark.parametrize("sparse_type,dense",
-                         [(None, True), (None, False),
-                          ("coo", True), ("csr", True),
-                          ("csc", True), ("dia", True)])
+@pytest.mark.parametrize(
+    "sparse_type,dense",
+    [
+        (None, True),
+        (None, False),
+        ("coo", True),
+        ("csr", True),
+        ("csc", True),
+        ("dia", True),
+    ],
+)
 def test_hamiltonian_expectation(backend, dense, density_matrix, sparse_type):
     """Test Hamiltonian expectation value calculation."""
     if sparse_type is None:
         h = hamiltonians.XXZ(nqubits=3, delta=0.5, dense=dense, backend=backend)
     else:
         if backend.name == "tensorflow":
             pytest.skip("Tensorflow does not support operations with sparse matrices.")
-        h = hamiltonians.Hamiltonian(6, random_sparse_matrix(backend, 64, sparse_type), backend=backend)
+        h = hamiltonians.Hamiltonian(
+            6, random_sparse_matrix(backend, 64, sparse_type), backend=backend
+        )
 
     matrix = backend.to_numpy(h.matrix)
     if density_matrix:
-        state = random_complex((2 ** h.nqubits, 2 ** h.nqubits))
+        state = random_complex((2**h.nqubits, 2**h.nqubits))
         state = state + state.T.conj()
         norm = np.trace(state)
         target_ev = np.trace(matrix.dot(state)).real
     else:
-        state = random_complex(2 ** h.nqubits)
+        state = random_complex(2**h.nqubits)
         norm = np.sum(np.abs(state) ** 2)
         target_ev = np.sum(state.conj() * matrix.dot(state)).real
 
     backend.assert_allclose(h.expectation(state), target_ev)
     backend.assert_allclose(h.expectation(state, True), target_ev / norm)
 
 
@@ -204,27 +243,66 @@
     state = random_complex((4, 4, 4))
     with pytest.raises(ValueError):
         h.expectation(state)
     with pytest.raises(TypeError):
         h.expectation("test")
 
 
+def test_hamiltonian_expectation_from_samples(backend):
+    """Test Hamiltonian expectation value calculation."""
+    obs0 = 2 * Z(0) * Z(1) + Z(0) * Z(2)
+    obs1 = 2 * Z(0) * Z(1) + Z(0) * Z(2) * I(3)
+    h0 = hamiltonians.SymbolicHamiltonian(obs0, backend=backend)
+    h1 = hamiltonians.SymbolicHamiltonian(obs1, backend=backend)
+    matrix = backend.to_numpy(h0.matrix)
+    c = Circuit(4)
+    c.add(gates.RX(0, np.random.rand()))
+    c.add(gates.RX(1, np.random.rand()))
+    c.add(gates.RX(2, np.random.rand()))
+    c.add(gates.RX(3, np.random.rand()))
+    c.add(gates.M(0, 1, 2, 3))
+    nshots = 10**5
+    result = c(nshots=nshots)
+    freq = result.frequencies(binary=True)
+    Obs0 = hamiltonians.Hamiltonian(3, matrix).expectation_from_samples(
+        freq, qubit_map=None
+    )
+    Obs1 = h1.expectation(result.state())
+
+    backend.assert_allclose(Obs0, Obs1, atol=10 / np.sqrt(nshots))
+
+
+def test_hamiltonian_expectation_from_samples_errors(backend):
+    obs = random_complex((4, 4))
+    h = hamiltonians.Hamiltonian(2, obs, backend=backend)
+    with pytest.raises(NotImplementedError):
+        h.expectation_from_samples(None, qubit_map=None)
+
+
 @pytest.mark.parametrize("dtype", [np.complex128, np.complex64])
-@pytest.mark.parametrize("sparse_type,dense",
-                         [(None, True), (None, False),
-                          ("coo", True), ("csr", True),
-                          ("csc", True), ("dia", True)])
+@pytest.mark.parametrize(
+    "sparse_type,dense",
+    [
+        (None, True),
+        (None, False),
+        ("coo", True),
+        ("csr", True),
+        ("csc", True),
+        ("dia", True),
+    ],
+)
 def test_hamiltonian_eigenvalues(backend, dtype, sparse_type, dense):
     """Testing hamiltonian eigenvalues scaling."""
     if sparse_type is None:
         H1 = hamiltonians.XXZ(nqubits=2, delta=0.5, dense=dense, backend=backend)
     else:
         if backend.name == "tensorflow":
             pytest.skip("Tensorflow does not support operations with sparse matrices.")
         from scipy import sparse
+
         H1 = hamiltonians.XXZ(nqubits=5, delta=0.5, backend=backend)
         m = getattr(sparse, f"{sparse_type}_matrix")(backend.to_numpy(H1.matrix))
         H1 = hamiltonians.Hamiltonian(5, m, backend=backend)
 
     H1_eigen = sorted(backend.to_numpy(H1.eigenvalues()))
     hH1_eigen = sorted(backend.to_numpy(backend.calculate_eigenvalues(H1.matrix)))
     backend.assert_allclose(sorted(H1_eigen), hH1_eigen)
@@ -235,15 +313,17 @@
     hH2_eigen = sorted(backend.to_numpy(backend.calculate_eigenvalues(c1 * H1.matrix)))
     backend.assert_allclose(H2_eigen, hH2_eigen)
 
     c2 = dtype(-11.1)
     H3 = H1 * c2
     if sparse_type is None:
         H3_eigen = sorted(backend.to_numpy(H3._eigenvalues))
-        hH3_eigen = sorted(backend.to_numpy(backend.calculate_eigenvalues(H1.matrix * c2)))
+        hH3_eigen = sorted(
+            backend.to_numpy(backend.calculate_eigenvalues(H1.matrix * c2))
+        )
         backend.assert_allclose(H3_eigen, hH3_eigen)
     else:
         assert H3._eigenvalues is None
 
 
 @pytest.mark.parametrize("dtype", [np.complex128, np.complex64])
 @pytest.mark.parametrize("dense", [True, False])
@@ -270,47 +350,66 @@
     c3 = dtype(0)
     H4 = c3 * H1
     V4 = backend.to_numpy(H4._eigenvectors)
     U4 = backend.to_numpy(H4._eigenvalues)
     backend.assert_allclose(H4.matrix, V4 @ np.diag(U4) @ V4.T)
 
 
-@pytest.mark.parametrize("sparse_type,dense",
-                         [(None, True), (None, False),
-                          ("coo", True), ("csr", True),
-                          ("csc", True), ("dia", True)])
+@pytest.mark.parametrize(
+    "sparse_type,dense",
+    [
+        (None, True),
+        (None, False),
+        ("coo", True),
+        ("csr", True),
+        ("csc", True),
+        ("dia", True),
+    ],
+)
 def test_hamiltonian_ground_state(backend, sparse_type, dense):
     """Test Hamiltonian ground state."""
     if sparse_type is None:
         H = hamiltonians.XXZ(nqubits=2, delta=0.5, dense=dense, backend=backend)
     else:
         if backend.name == "tensorflow":
             pytest.skip("Tensorflow does not support operations with sparse matrices.")
         from scipy import sparse
+
         H = hamiltonians.XXZ(nqubits=5, delta=0.5, backend=backend)
         m = getattr(sparse, f"{sparse_type}_matrix")(backend.to_numpy(H.matrix))
         H = hamiltonians.Hamiltonian(5, m, backend=backend)
     V = backend.to_numpy(H.eigenvectors())
     backend.assert_allclose(H.ground_state(), V[:, 0])
 
 
-@pytest.mark.parametrize("sparse_type,dense",
-                         [(None, True), (None, False),
-                          ("coo", True), ("csr", True),
-                          ("csc", True), ("dia", True)])
+@pytest.mark.parametrize(
+    "sparse_type,dense",
+    [
+        (None, True),
+        (None, False),
+        ("coo", True),
+        ("csr", True),
+        ("csc", True),
+        ("dia", True),
+    ],
+)
 def test_hamiltonian_exponentiation(backend, sparse_type, dense):
     """Test matrix exponentiation of Hamiltonians ``exp(1j * t * H)``."""
     from scipy.linalg import expm
+
     def construct_hamiltonian():
         if sparse_type is None:
             return hamiltonians.XXZ(nqubits=2, delta=0.5, dense=dense, backend=backend)
         else:
             if backend.name == "tensorflow":
-                pytest.skip("Tensorflow does not support operations with sparse matrices.")
+                pytest.skip(
+                    "Tensorflow does not support operations with sparse matrices."
+                )
             from scipy import sparse
+
             ham = hamiltonians.XXZ(nqubits=5, delta=0.5, backend=backend)
             m = getattr(sparse, f"{sparse_type}_matrix")(backend.to_numpy(ham.matrix))
             return hamiltonians.Hamiltonian(5, m, backend=backend)
 
     H = construct_hamiltonian()
     target_matrix = expm(-0.5j * backend.to_numpy(H.matrix))
     H1 = construct_hamiltonian()
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_from_symbols.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians_from_symbols.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test dense matrix of Hamiltonians constructed using symbols."""
-import pytest
 import numpy as np
+import pytest
 import sympy
+
 from qibo import hamiltonians, matrices
-from qibo.symbols import I, X, Y, Z, Symbol
+from qibo.symbols import I, Symbol, X, Y, Z
 from qibo.tests.utils import random_hermitian
 
 
 @pytest.mark.parametrize("nqubits", [4, 5])
 @pytest.mark.parametrize("hamtype", ["normal", "symbolic"])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_tfim_hamiltonian_from_symbols(backend, nqubits, hamtype, calcterms):
@@ -16,16 +17,16 @@
         h = 0.5
         symham = sum(Z(i) * Z(i + 1) for i in range(nqubits - 1))
         symham += Z(0) * Z(nqubits - 1)
         symham += h * sum(X(i) for i in range(nqubits))
         ham = hamiltonians.SymbolicHamiltonian(-symham, backend=backend)
     else:
         h = 0.5
-        z_symbols = sympy.symbols(" ".join((f"Z{i}" for i in range(nqubits))))
-        x_symbols = sympy.symbols(" ".join((f"X{i}" for i in range(nqubits))))
+        z_symbols = sympy.symbols(" ".join(f"Z{i}" for i in range(nqubits)))
+        x_symbols = sympy.symbols(" ".join(f"X{i}" for i in range(nqubits)))
 
         symham = sum(z_symbols[i] * z_symbols[i + 1] for i in range(nqubits - 1))
         symham += z_symbols[0] * z_symbols[-1]
         symham += h * sum(x_symbols)
         symmap = {z: (i, matrices.Z) for i, z in enumerate(z_symbols)}
         symmap.update({x: (i, matrices.X) for i, x in enumerate(x_symbols)})
         ham = hamiltonians.Hamiltonian.from_symbolic(-symham, symmap, backend=backend)
@@ -39,20 +40,25 @@
 
 @pytest.mark.parametrize("hamtype", ["normal", "symbolic"])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_from_symbolic_with_power(backend, hamtype, calcterms):
     """Check ``from_symbolic`` when the expression contains powers."""
     if hamtype == "symbolic":
         matrix = random_hermitian(1)
-        symham =  (Symbol(0, matrix) ** 2 - Symbol(1, matrix) ** 2 +
-                   3 * Symbol(1, matrix) - 2 * Symbol(0, matrix) * Symbol(2, matrix) + 1)
+        symham = (
+            Symbol(0, matrix) ** 2
+            - Symbol(1, matrix) ** 2
+            + 3 * Symbol(1, matrix)
+            - 2 * Symbol(0, matrix) * Symbol(2, matrix)
+            + 1
+        )
         ham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
     else:
-        z = sympy.symbols(" ".join((f"Z{i}" for i in range(3))))
-        symham =  z[0] ** 2 - z[1] ** 2 + 3 * z[1] - 2 * z[0] * z[2] + 1
+        z = sympy.symbols(" ".join(f"Z{i}" for i in range(3)))
+        symham = z[0] ** 2 - z[1] ** 2 + 3 * z[1] - 2 * z[0] * z[2] + 1
         matrix = random_hermitian(1)
         symmap = {x: (i, matrix) for i, x in enumerate(z)}
         ham = hamiltonians.Hamiltonian.from_symbolic(symham, symmap, backend=backend)
 
     if calcterms:
         _ = ham.terms
     final_matrix = ham.matrix
@@ -67,20 +73,30 @@
 
 
 @pytest.mark.parametrize("hamtype", ["normal", "symbolic"])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_from_symbolic_with_complex_numbers(backend, hamtype, calcterms):
     """Check ``from_symbolic`` when the expression contains imaginary unit."""
     if hamtype == "symbolic":
-        symham = (1 + 2j) * X(0) * X(1) + 2 * Y(0) * Y(1) - 3j * X(0) * Y(1) + 1j * Y(0) * X(1)
+        symham = (
+            (1 + 2j) * X(0) * X(1)
+            + 2 * Y(0) * Y(1)
+            - 3j * X(0) * Y(1)
+            + 1j * Y(0) * X(1)
+        )
         ham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
     else:
-        x = sympy.symbols(" ".join((f"X{i}" for i in range(2))))
-        y = sympy.symbols(" ".join((f"Y{i}" for i in range(2))))
-        symham = (1 + 2j) * x[0] * x[1] + 2 * y[0] * y[1] - 3j * x[0] * y[1] + 1j * y[0] * x[1]
+        x = sympy.symbols(" ".join(f"X{i}" for i in range(2)))
+        y = sympy.symbols(" ".join(f"Y{i}" for i in range(2)))
+        symham = (
+            (1 + 2j) * x[0] * x[1]
+            + 2 * y[0] * y[1]
+            - 3j * x[0] * y[1]
+            + 1j * y[0] * x[1]
+        )
         symmap = {s: (i, matrices.X) for i, s in enumerate(x)}
         symmap.update({s: (i, matrices.Y) for i, s in enumerate(y)})
         ham = hamiltonians.Hamiltonian.from_symbolic(symham, symmap, backend=backend)
 
     if calcterms:
         _ = ham.terms
     final_matrix = ham.matrix
@@ -92,20 +108,36 @@
 
 
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_from_symbolic_application_hamiltonian(backend, calcterms):
     """Check ``from_symbolic`` for a specific four-qubit Hamiltonian."""
     z1, z2, z3, z4 = sympy.symbols("z1 z2 z3 z4")
     symmap = {z: (i, matrices.Z) for i, z in enumerate([z1, z2, z3, z4])}
-    symham = (z1 * z2 - 0.5 * z1 * z3 + 2 * z2 * z3 + 0.35 * z2
-              + 0.25 * z3 * z4 + 0.5 * z3 + z4 - z1)
+    symham = (
+        z1 * z2
+        - 0.5 * z1 * z3
+        + 2 * z2 * z3
+        + 0.35 * z2
+        + 0.25 * z3 * z4
+        + 0.5 * z3
+        + z4
+        - z1
+    )
     # Check that Trotter dense matrix agrees will full Hamiltonian matrix
     fham = hamiltonians.Hamiltonian.from_symbolic(symham, symmap, backend=backend)
-    symham = (Z(0) * Z(1) - 0.5 * Z(0) * Z(2) + 2 * Z(1) * Z(2) + 0.35 * Z(1)
-              + 0.25 * Z(2) * Z(3) + 0.5 * Z(2) + Z(3) - Z(0))
+    symham = (
+        Z(0) * Z(1)
+        - 0.5 * Z(0) * Z(2)
+        + 2 * Z(1) * Z(2)
+        + 0.35 * Z(1)
+        + 0.25 * Z(2) * Z(3)
+        + 0.5 * Z(2)
+        + Z(3)
+        - Z(0)
+    )
     sham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
     if calcterms:
         _ = sham.terms
     backend.assert_allclose(sham.matrix, fham.matrix)
 
 
 @pytest.mark.parametrize("nqubits", [4, 5])
@@ -113,16 +145,16 @@
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_x_hamiltonian_from_symbols(backend, nqubits, hamtype, calcterms):
     """Check creating sum(X) Hamiltonian using sympy."""
     if hamtype == "symbolic":
         symham = -sum(X(i) for i in range(nqubits))
         ham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
     else:
-        x_symbols = sympy.symbols(" ".join((f"X{i}" for i in range(nqubits))))
-        symham =  -sum(x_symbols)
+        x_symbols = sympy.symbols(" ".join(f"X{i}" for i in range(nqubits)))
+        symham = -sum(x_symbols)
         symmap = {x: (i, matrices.X) for i, x in enumerate(x_symbols)}
         ham = hamiltonians.Hamiltonian.from_symbolic(symham, symmap, backend=backend)
     if calcterms:
         _ = ham.terms
     final_matrix = ham.matrix
     target_matrix = hamiltonians.X(nqubits, backend=backend).matrix
     backend.assert_allclose(final_matrix, target_matrix)
@@ -133,17 +165,17 @@
 def test_three_qubit_term_hamiltonian_from_symbols(backend, hamtype, calcterms):
     """Check creating Hamiltonian with three-qubit interaction using sympy."""
     if hamtype == "symbolic":
         symham = X(0) * Y(1) * Z(2) + 0.5 * Y(0) * Z(1) * X(3) + Z(0) * X(2)
         symham += Y(2) + 1.5 * Z(1) - 2 - 3 * X(1) * Y(3)
         ham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
     else:
-        x_symbols = sympy.symbols(" ".join((f"X{i}" for i in range(4))))
-        y_symbols = sympy.symbols(" ".join((f"Y{i}" for i in range(4))))
-        z_symbols = sympy.symbols(" ".join((f"Z{i}" for i in range(4))))
+        x_symbols = sympy.symbols(" ".join(f"X{i}" for i in range(4)))
+        y_symbols = sympy.symbols(" ".join(f"Y{i}" for i in range(4)))
+        z_symbols = sympy.symbols(" ".join(f"Z{i}" for i in range(4)))
         symmap = {x: (i, matrices.X) for i, x in enumerate(x_symbols)}
         symmap.update({x: (i, matrices.Y) for i, x in enumerate(y_symbols)})
         symmap.update({x: (i, matrices.Z) for i, x in enumerate(z_symbols)})
 
         symham = x_symbols[0] * y_symbols[1] * z_symbols[2]
         symham += 0.5 * y_symbols[0] * z_symbols[1] * x_symbols[3]
         symham += z_symbols[0] * x_symbols[2]
@@ -152,39 +184,48 @@
         symham += 1.5 * z_symbols[1]
         symham -= 2
         ham = hamiltonians.Hamiltonian.from_symbolic(symham, symmap, backend=backend)
 
     if calcterms:
         _ = ham.terms
     final_matrix = ham.matrix
-    target_matrix = np.kron(np.kron(matrices.X, matrices.Y),
-                            np.kron(matrices.Z, matrices.I))
-    target_matrix += 0.5 * np.kron(np.kron(matrices.Y, matrices.Z),
-                                   np.kron(matrices.I, matrices.X))
-    target_matrix += np.kron(np.kron(matrices.Z, matrices.I),
-                             np.kron(matrices.X, matrices.I))
-    target_matrix += -3 * np.kron(np.kron(matrices.I, matrices.X),
-                             np.kron(matrices.I, matrices.Y))
-    target_matrix += np.kron(np.kron(matrices.I, matrices.I),
-                             np.kron(matrices.Y, matrices.I))
-    target_matrix += 1.5 * np.kron(np.kron(matrices.I, matrices.Z),
-                                   np.kron(matrices.I, matrices.I))
+    target_matrix = np.kron(
+        np.kron(matrices.X, matrices.Y), np.kron(matrices.Z, matrices.I)
+    )
+    target_matrix += 0.5 * np.kron(
+        np.kron(matrices.Y, matrices.Z), np.kron(matrices.I, matrices.X)
+    )
+    target_matrix += np.kron(
+        np.kron(matrices.Z, matrices.I), np.kron(matrices.X, matrices.I)
+    )
+    target_matrix += -3 * np.kron(
+        np.kron(matrices.I, matrices.X), np.kron(matrices.I, matrices.Y)
+    )
+    target_matrix += np.kron(
+        np.kron(matrices.I, matrices.I), np.kron(matrices.Y, matrices.I)
+    )
+    target_matrix += 1.5 * np.kron(
+        np.kron(matrices.I, matrices.Z), np.kron(matrices.I, matrices.I)
+    )
     target_matrix -= 2 * np.eye(2**4, dtype=target_matrix.dtype)
     backend.assert_allclose(final_matrix, target_matrix)
 
 
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_hamiltonian_with_identity_symbol(backend, calcterms):
     """Check creating Hamiltonian from expression which contains the identity symbol."""
     symham = X(0) * I(1) * Z(2) + 0.5 * Y(0) * Z(1) * I(3) + Z(0) * I(1) * X(2)
     ham = hamiltonians.SymbolicHamiltonian(symham, backend=backend)
 
     if calcterms:
         _ = ham.terms
     final_matrix = ham.matrix
-    target_matrix = np.kron(np.kron(matrices.X, matrices.I),
-                            np.kron(matrices.Z, matrices.I))
-    target_matrix += 0.5 * np.kron(np.kron(matrices.Y, matrices.Z),
-                                   np.kron(matrices.I, matrices.I))
-    target_matrix += np.kron(np.kron(matrices.Z, matrices.I),
-                             np.kron(matrices.X, matrices.I))
+    target_matrix = np.kron(
+        np.kron(matrices.X, matrices.I), np.kron(matrices.Z, matrices.I)
+    )
+    target_matrix += 0.5 * np.kron(
+        np.kron(matrices.Y, matrices.Z), np.kron(matrices.I, matrices.I)
+    )
+    target_matrix += np.kron(
+        np.kron(matrices.Z, matrices.I), np.kron(matrices.X, matrices.I)
+    )
     backend.assert_allclose(final_matrix, target_matrix)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_models.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests methods from `qibo/src/hamiltonians/models.py`."""
-import pytest
 import numpy as np
-from qibo import hamiltonians, matrices
+import pytest
 
+from qibo import hamiltonians, matrices
 
 models_config = [
     ("TFIM", {"nqubits": 3, "h": 0.0}, "tfim_N3h0.0.out"),
     ("TFIM", {"nqubits": 3, "h": 0.5}, "tfim_N3h0.5.out"),
     ("TFIM", {"nqubits": 3, "h": 1.0}, "tfim_N3h1.0.out"),
     ("XXZ", {"nqubits": 3, "delta": 0.0}, "heisenberg_N3delta0.0.out"),
     ("XXZ", {"nqubits": 3, "delta": 0.5}, "heisenberg_N3delta0.5.out"),
@@ -14,36 +14,41 @@
     ("X", {"nqubits": 3}, "x_N3.out"),
     ("Y", {"nqubits": 4}, "y_N4.out"),
     ("Z", {"nqubits": 5}, "z_N5.out"),
     ("MaxCut", {"nqubits": 3}, "maxcut_N3.out"),
     ("MaxCut", {"nqubits": 4}, "maxcut_N4.out"),
     ("MaxCut", {"nqubits": 5}, "maxcut_N5.out"),
 ]
+
+
 @pytest.mark.parametrize(("model", "kwargs", "filename"), models_config)
 def test_hamiltonian_models(backend, model, kwargs, filename):
     """Test pre-coded Hamiltonian models generate the proper matrices."""
     from qibo.tests.test_models_variational import assert_regression_fixture
+
     H = getattr(hamiltonians, model)(**kwargs, backend=backend)
     matrix = backend.to_numpy(H.matrix).flatten().real
     assert_regression_fixture(backend, matrix, filename)
 
 
 @pytest.mark.parametrize("nqubits", [3, 4])
-@pytest.mark.parametrize("dense,calcterms", [(True, False), (False, False), (False, True)])
+@pytest.mark.parametrize(
+    "dense,calcterms", [(True, False), (False, False), (False, True)]
+)
 def test_maxcut(backend, nqubits, dense, calcterms):
-    size = 2 ** nqubits
+    size = 2**nqubits
     ham = np.zeros(shape=(size, size), dtype=np.complex128)
     for i in range(nqubits):
         for j in range(nqubits):
             h = np.eye(1)
             for k in range(nqubits):
                 if (k == i) ^ (k == j):
                     h = np.kron(h, matrices.Z)
                 else:
                     h = np.kron(h, matrices.I)
             M = np.eye(2**nqubits) - h
             ham += M
-    target_ham = backend.cast(- ham / 2)
+    target_ham = backend.cast(-ham / 2)
     final_ham = hamiltonians.MaxCut(nqubits, dense, backend=backend)
     if (not dense) and calcterms:
         _ = final_ham.terms
     backend.assert_allclose(final_ham.matrix, target_ham)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_symbolic.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians_symbolic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,67 @@
 """Test methods of :class:`qibo.core.hamiltonians.SymbolicHamiltonian`."""
-import pytest
 import numpy as np
+import pytest
 import sympy
-from qibo import hamiltonians
+
+from qibo import gates, hamiltonians
+from qibo.models import Circuit
+from qibo.symbols import I, Y, Z
 from qibo.tests.utils import random_complex
 
 
 def symbolic_tfim(nqubits, h=1.0):
     """Constructs symbolic Hamiltonian for TFIM."""
-    from qibo.symbols import Z, X
+    from qibo.symbols import X, Z
+
     sham = -sum(Z(i) * Z(i + 1) for i in range(nqubits - 1))
     sham -= Z(0) * Z(nqubits - 1)
     sham -= h * sum(X(i) for i in range(nqubits))
     return sham
 
 
 def test_symbolic_hamiltonian_errors(backend):
     # Wrong type of Symbol matrix
     from qibo.symbols import Symbol
+
     with pytest.raises(TypeError):
         s = Symbol(0, "test")
     # Wrong type of symbolic expression
     with pytest.raises(TypeError):
         ham = hamiltonians.SymbolicHamiltonian("test", backend=backend)
     # Passing form with symbol that is not in ``symbol_map``
     from qibo import matrices
+
     Z, X = sympy.Symbol("Z"), sympy.Symbol("X")
     symbol_map = {Z: (0, matrices.Z)}
     with pytest.raises(ValueError):
         ham = hamiltonians.SymbolicHamiltonian(Z * X, symbol_map, backend=backend)
     # Invalid operation in Hamiltonian expresion
     ham = hamiltonians.SymbolicHamiltonian(sympy.cos(Z), symbol_map, backend=backend)
     with pytest.raises(TypeError):
         dense = ham.dense
 
 
 @pytest.mark.parametrize("nqubits", [3, 4])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_symbolictfim_hamiltonian_to_dense(backend, nqubits, calcterms):
-    final_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1), backend=backend)
+    final_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1), backend=backend
+    )
     target_ham = hamiltonians.TFIM(nqubits, h=1, backend=backend)
     if calcterms:
         _ = final_ham.terms
     backend.assert_allclose(final_ham.matrix, target_ham.matrix, atol=1e-15)
 
 
 @pytest.mark.parametrize("nqubits", [3, 4])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_symbolicxxz_hamiltonian_to_dense(backend, nqubits, calcterms):
     from qibo.symbols import X, Y, Z
+
     sham = sum(X(i) * X(i + 1) for i in range(nqubits - 1))
     sham += sum(Y(i) * Y(i + 1) for i in range(nqubits - 1))
     sham += 0.5 * sum(Z(i) * Z(i + 1) for i in range(nqubits - 1))
     sham += X(0) * X(nqubits - 1) + Y(0) * Y(nqubits - 1) + 0.5 * Z(0) * Z(nqubits - 1)
     final_ham = hamiltonians.SymbolicHamiltonian(sham, backend=backend)
     target_ham = hamiltonians.XXZ(nqubits, backend=backend)
     if calcterms:
@@ -61,119 +70,147 @@
 
 
 @pytest.mark.parametrize("nqubits", [3])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
 def test_symbolic_hamiltonian_scalar_mul(backend, nqubits, calcterms, calcdense):
     """Test multiplication of Trotter Hamiltonian with scalar."""
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     target_ham = 2 * hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (2 * local_ham).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (local_ham * 2).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
 
 @pytest.mark.parametrize("nqubits", [4])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
 def test_symbolic_hamiltonian_scalar_add(backend, nqubits, calcterms, calcdense):
     """Test addition of Trotter Hamiltonian with scalar."""
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     target_ham = 2 + hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (2 + local_ham).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (local_ham + 2).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
 
 @pytest.mark.parametrize("nqubits", [3])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
 def test_symbolic_hamiltonian_scalar_sub(backend, nqubits, calcterms, calcdense):
     """Test subtraction of Trotter Hamiltonian with scalar."""
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     target_ham = 2 - hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (2 - local_ham).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
     target_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) - 2
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     local_dense = (local_ham - 2).dense
     backend.assert_allclose(local_dense.matrix, target_ham.matrix)
 
 
 @pytest.mark.parametrize("nqubits", [3])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
-def test_symbolic_hamiltonian_operator_add_and_sub(backend, nqubits, calcterms, calcdense):
+def test_symbolic_hamiltonian_operator_add_and_sub(
+    backend, nqubits, calcterms, calcdense
+):
     """Test addition and subtraction between Trotter Hamiltonians."""
-    local_ham1 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
-    local_ham2 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=0.5), backend=backend)
+    local_ham1 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
+    local_ham2 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=0.5), backend=backend
+    )
     if calcterms:
         _ = local_ham1.terms
         _ = local_ham2.terms
     if calcdense:
         _ = local_ham1.dense
         _ = local_ham2.dense
     local_ham = local_ham1 + local_ham2
-    target_ham = (hamiltonians.TFIM(nqubits, h=1.0, backend=backend) +
-                  hamiltonians.TFIM(nqubits, h=0.5, backend=backend))
+    target_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) + hamiltonians.TFIM(
+        nqubits, h=0.5, backend=backend
+    )
     dense = local_ham.dense
     backend.assert_allclose(dense.matrix, target_ham.matrix)
 
-    local_ham1 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
-    local_ham2 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=0.5), backend=backend)
+    local_ham1 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
+    local_ham2 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=0.5), backend=backend
+    )
     if calcterms:
         _ = local_ham1.terms
         _ = local_ham2.terms
     if calcdense:
         _ = local_ham1.dense
         _ = local_ham2.dense
     local_ham = local_ham1 - local_ham2
-    target_ham = (hamiltonians.TFIM(nqubits, h=1.0, backend=backend) -
-                  hamiltonians.TFIM(nqubits, h=0.5, backend=backend))
+    target_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) - hamiltonians.TFIM(
+        nqubits, h=0.5, backend=backend
+    )
     dense = local_ham.dense
     backend.assert_allclose(dense.matrix, target_ham.matrix)
 
 
 @pytest.mark.parametrize("nqubits", [5])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
 def test_symbolic_hamiltonian_hamiltonianmatmul(backend, nqubits, calcterms, calcdense):
-    local_ham1 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
-    local_ham2 = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=0.5), backend=backend)
+    local_ham1 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
+    local_ham2 = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=0.5), backend=backend
+    )
     dense_ham1 = hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     dense_ham2 = hamiltonians.TFIM(nqubits, h=0.5, backend=backend)
     if calcterms:
         _ = local_ham1.terms
         _ = local_ham2.terms
     if calcdense:
         _ = local_ham1.dense
@@ -184,57 +221,95 @@
 
 
 @pytest.mark.parametrize("nqubits", [3, 4])
 @pytest.mark.parametrize("density_matrix", [False, True])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_symbolic_hamiltonian_matmul(backend, nqubits, density_matrix, calcterms):
     if density_matrix:
-        #from qibo.core.states import MatrixState
-        shape = (2 ** nqubits, 2 ** nqubits)
-        #state = MatrixState.from_tensor(random_complex(shape))
+        # from qibo.core.states import MatrixState
+        shape = (2**nqubits, 2**nqubits)
+        # state = MatrixState.from_tensor(random_complex(shape))
     else:
-        #from qibo.core.states import VectorState
-        shape = (2 ** nqubits,)
-        #state = VectorState.from_tensor(random_complex(shape))
+        # from qibo.core.states import VectorState
+        shape = (2**nqubits,)
+        # state = VectorState.from_tensor(random_complex(shape))
     state = random_complex(shape)
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+    local_ham = hamiltonians.SymbolicHamiltonian(
+        symbolic_tfim(nqubits, h=1.0), backend=backend
+    )
     dense_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
     if calcterms:
         _ = local_ham.terms
     local_matmul = local_ham @ state
     target_matmul = dense_ham @ state
     backend.assert_allclose(local_matmul, target_matmul)
 
 
 @pytest.mark.parametrize("nqubits,normalize", [(3, False), (4, False)])
 @pytest.mark.parametrize("calcterms", [False, True])
 @pytest.mark.parametrize("calcdense", [False, True])
-def test_symbolic_hamiltonian_state_ev(backend, nqubits, normalize, calcterms, calcdense):
-    local_ham = hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend) + 2
+def test_symbolic_hamiltonian_state_ev(
+    backend, nqubits, normalize, calcterms, calcdense
+):
+    local_ham = (
+        hamiltonians.SymbolicHamiltonian(symbolic_tfim(nqubits, h=1.0), backend=backend)
+        + 2
+    )
     if calcterms:
         _ = local_ham.terms
     if calcdense:
         _ = local_ham.dense
     dense_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) + 2
 
-    state = backend.cast(random_complex((2 ** nqubits,)))
+    state = backend.cast(random_complex((2**nqubits,)))
     local_ev = local_ham.expectation(state, normalize)
     target_ev = dense_ham.expectation(state, normalize)
     backend.assert_allclose(local_ev, target_ev)
 
-    state = random_complex((2 ** nqubits,))
+    state = random_complex((2**nqubits,))
     local_ev = local_ham.expectation(state, normalize)
     target_ev = dense_ham.expectation(state, normalize)
     backend.assert_allclose(local_ev, target_ev)
 
 
+def test_hamiltonian_expectation_from_samples(backend):
+    """Test Hamiltonian expectation value calculation."""
+    obs0 = 2 * Z(0) * Z(1) + Z(0) * Z(2)
+    obs1 = 2 * Z(0) * Z(1) + Z(0) * Z(2) * I(3)
+    h0 = hamiltonians.SymbolicHamiltonian(obs0, backend=backend)
+    h1 = hamiltonians.SymbolicHamiltonian(obs1, backend=backend)
+    c = Circuit(4)
+    c.add(gates.RX(0, np.random.rand()))
+    c.add(gates.RX(1, np.random.rand()))
+    c.add(gates.RX(2, np.random.rand()))
+    c.add(gates.RX(3, np.random.rand()))
+    c.add(gates.M(0, 1, 2, 3))
+    nshots = 10**5
+    result = c(nshots=nshots)
+    freq = result.frequencies(binary=True)
+    Obs0 = h0.expectation_from_samples(freq, qubit_map=None)
+    Obs1 = h1.expectation(result.state())
+    backend.assert_allclose(Obs0, Obs1, atol=10 / np.sqrt(nshots))
+
+
+def test_hamiltonian_expectation_from_samples_errors(backend):
+    obs = [Z(0) * Y(1), Z(0) * Z(1) ** 3]
+    h1 = hamiltonians.SymbolicHamiltonian(obs[0], backend=backend)
+    h2 = hamiltonians.SymbolicHamiltonian(obs[1], backend=backend)
+    with pytest.raises(NotImplementedError):
+        h1.expectation_from_samples(None, qubit_map=None)
+    with pytest.raises(NotImplementedError):
+        h2.expectation_from_samples(None, qubit_map=None)
+
+
 @pytest.mark.parametrize("density_matrix", [False, True])
 @pytest.mark.parametrize("calcterms", [False, True])
 def test_symbolic_hamiltonian_abstract_symbol_ev(backend, density_matrix, calcterms):
-    from qibo.symbols import X, Symbol
+    from qibo.symbols import Symbol, X
+
     matrix = np.random.random((2, 2))
     form = X(0) * Symbol(1, matrix) + Symbol(0, matrix) * X(1)
     local_ham = hamiltonians.SymbolicHamiltonian(form, backend=backend)
     if calcterms:
         _ = local_ham.terms
     if density_matrix:
         state = backend.cast(random_complex((4, 4)))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_terms.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians_terms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Tests methods defined in `qibo/core/terms.py`."""
-import pytest
 import numpy as np
-from qibo import matrices, models, gates
+import pytest
+
+from qibo import gates, matrices, models
 from qibo.hamiltonians import terms
-from qibo.tests.utils import random_state, random_density_matrix
+from qibo.tests.utils import random_density_matrix, random_state
 
 
 def test_hamiltonian_term_initialization(backend):
     """Test initialization and matrix assignment of ``HamiltonianTerm``."""
     matrix = np.random.random((2, 2))
     term = terms.HamiltonianTerm(matrix, 0)
     assert term.target_qubits == (0,)
@@ -52,14 +53,15 @@
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(final_state, target_state)
 
 
 def test_hamiltonian_term_exponentiation(backend):
     """Test exp gate application of ``HamiltonianTerm``."""
     from scipy.linalg import expm
+
     matrix = np.random.random((2, 2))
     term = terms.HamiltonianTerm(matrix, 1)
     exp_matrix = expm(-0.5j * matrix)
     backend.assert_allclose(term.exp(0.5), exp_matrix)
 
     initial_state = random_state(2)
     final_state = term(backend, np.copy(initial_state), 2, term.expgate(0.5))
@@ -95,95 +97,106 @@
 
 
 @pytest.mark.parametrize("use_symbols", [True, False])
 def test_symbolic_term_creation(backend, use_symbols):
     """Test creating ``SymbolicTerm`` from sympy expression."""
     if use_symbols:
         from qibo.symbols import X, Y
+
         expression = X(0) * Y(1) * X(1)
         symbol_map = {}
     else:
         import sympy
+
         x0, x1, y1 = sympy.symbols("X0 X1 Y1", commutative=False)
         expression = x0 * y1 * x1
-        symbol_map = {x0: (0, matrices.X), x1: (1, matrices.X),
-                      y1: (1, matrices.Y)}
+        symbol_map = {x0: (0, matrices.X), x1: (1, matrices.X), y1: (1, matrices.Y)}
     term = terms.SymbolicTerm(2, expression, symbol_map)
     assert term.target_qubits == (0, 1)
     assert len(term.matrix_map) == 2
     backend.assert_allclose(term.matrix_map.get(0)[0], matrices.X)
     backend.assert_allclose(term.matrix_map.get(1)[0], matrices.Y)
     backend.assert_allclose(term.matrix_map.get(1)[1], matrices.X)
 
 
 def test_symbolic_term_with_power_creation(backend):
     """Test creating ``SymbolicTerm`` from sympy expression that contains powers."""
     from qibo.symbols import X, Z
+
     expression = X(0) ** 4 * Z(1) ** 2 * X(2)
     term = terms.SymbolicTerm(2, expression)
     assert term.target_qubits == (0, 1, 2)
     assert len(term.matrix_map) == 3
     assert term.coefficient == 2
     backend.assert_allclose(term.matrix_map.get(0), 4 * [matrices.X])
     backend.assert_allclose(term.matrix_map.get(1), 2 * [matrices.Z])
     backend.assert_allclose(term.matrix_map.get(2), [matrices.X])
 
 
 def test_symbolic_term_with_imag_creation(backend):
     """Test creating ``SymbolicTerm`` from sympy expression that contains imaginary coefficients."""
     from qibo.symbols import Y
+
     expression = 3j * Y(0)
     term = terms.SymbolicTerm(2, expression)
     assert term.target_qubits == (0,)
     assert term.coefficient == 6j
 
 
 def test_symbolic_term_matrix(backend):
     """Test matrix calculation of ``SymbolicTerm``."""
     from qibo.symbols import X, Y, Z
+
     expression = X(0) * Y(1) * Z(2) * X(1)
     term = terms.SymbolicTerm(2, expression)
     assert term.target_qubits == (0, 1, 2)
     target_matrix = np.kron(matrices.X, matrices.Y @ matrices.X)
     target_matrix = 2 * np.kron(target_matrix, matrices.Z)
     backend.assert_allclose(term.matrix, target_matrix)
 
 
 def test_symbolic_term_mul(backend):
     """Test multiplying scalar to ``SymbolicTerm``."""
     from qibo.symbols import X, Y, Z
+
     expression = Y(2) * Z(3) * X(2) * X(3)
     term = terms.SymbolicTerm(1, expression)
     assert term.target_qubits == (2, 3)
     target_matrix = np.kron(matrices.Y @ matrices.X, matrices.Z @ matrices.X)
     backend.assert_allclose(term.matrix, target_matrix)
     backend.assert_allclose((2 * term).matrix, 2 * target_matrix)
     backend.assert_allclose((term * 3).matrix, 3 * target_matrix)
 
 
 @pytest.mark.parametrize("density_matrix", [False])
 def test_symbolic_term_call(backend, density_matrix):
     """Test applying ``SymbolicTerm`` to state."""
     from qibo.symbols import X, Y, Z
+
     expression = Z(0) * X(1) * Y(2)
     term = terms.SymbolicTerm(2, expression)
-    matrixlist = [np.kron(matrices.Z, np.eye(4)),
-                  np.kron(np.kron(np.eye(2), matrices.X), np.eye(2)),
-                  np.kron(np.eye(4), matrices.Y)]
+    matrixlist = [
+        np.kron(matrices.Z, np.eye(4)),
+        np.kron(np.kron(np.eye(2), matrices.X), np.eye(2)),
+        np.kron(np.eye(4), matrices.Y),
+    ]
     initial_state = random_density_matrix(3) if density_matrix else random_state(3)
-    final_state = term(backend, np.copy(initial_state), 3, density_matrix=density_matrix)
+    final_state = term(
+        backend, np.copy(initial_state), 3, density_matrix=density_matrix
+    )
     target_state = 2 * np.copy(initial_state)
     for matrix in matrixlist:
         target_state = matrix @ target_state
     backend.assert_allclose(final_state, target_state)
 
 
 def test_symbolic_term_merge(backend):
     """Test merging ``SymbolicTerm`` to ``HamiltonianTerm``."""
     from qibo.symbols import X, Z
+
     matrix = np.random.random((4, 4))
     term1 = terms.HamiltonianTerm(matrix, 0, 1)
     term2 = terms.SymbolicTerm(1, X(0) * Z(1))
     term = term1.merge(term2)
     target_matrix = matrix + np.kron(matrices.X, matrices.Z)
     backend.assert_allclose(term.matrix, target_matrix)
 
@@ -202,14 +215,15 @@
     group.append(term3)
     assert group.target_qubits == {0, 1, 3}
 
 
 def test_term_group_to_term(backend):
     """Test ``GroupTerm.term`` property."""
     from qibo.symbols import X, Z
+
     matrix = np.random.random((8, 8))
     term1 = terms.HamiltonianTerm(matrix, 0, 1, 3)
     term2 = terms.SymbolicTerm(1, X(0) * Z(3))
     term3 = terms.SymbolicTerm(2, X(1))
     group = terms.TermGroup(term1)
     group.append(term2)
     group.append(term3)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_hamiltonians_trotter.py` & `qibo-0.1.9/src/qibo/tests/test_hamiltonians_trotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Test Trotter Hamiltonian methods from `qibo/core/hamiltonians.py`."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import hamiltonians
-from qibo.tests.utils import random_state, random_complex, random_hermitian
+from qibo.tests.utils import random_complex, random_hermitian, random_state
 
 
 @pytest.mark.parametrize("nqubits", [3, 4])
 @pytest.mark.parametrize("model", ["TFIM", "XXZ", "Y", "MaxCut"])
 def test_trotter_hamiltonian_to_dense(backend, nqubits, model):
     """Test that Trotter Hamiltonian dense form agrees with normal Hamiltonian."""
     local_ham = getattr(hamiltonians, model)(nqubits, dense=False, backend=backend)
@@ -54,57 +55,64 @@
 
 def test_trotter_hamiltonian_operator_add_and_sub(backend, nqubits=3):
     """Test addition and subtraction between Trotter Hamiltonians."""
     local_ham1 = hamiltonians.TFIM(nqubits, h=1.0, dense=False, backend=backend)
     local_ham2 = hamiltonians.TFIM(nqubits, h=0.5, dense=False, backend=backend)
 
     local_ham = local_ham1 + local_ham2
-    target_ham = (hamiltonians.TFIM(nqubits, h=1.0, backend=backend) +
-                  hamiltonians.TFIM(nqubits, h=0.5, backend=backend))
+    target_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) + hamiltonians.TFIM(
+        nqubits, h=0.5, backend=backend
+    )
     dense = local_ham.dense
     backend.assert_allclose(dense.matrix, target_ham.matrix)
 
     local_ham = local_ham1 - local_ham2
-    target_ham = (hamiltonians.TFIM(nqubits, h=1.0, backend=backend) -
-                  hamiltonians.TFIM(nqubits, h=0.5, backend=backend))
+    target_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend) - hamiltonians.TFIM(
+        nqubits, h=0.5, backend=backend
+    )
     dense = local_ham.dense
     backend.assert_allclose(dense.matrix, target_ham.matrix)
 
 
 @pytest.mark.parametrize("nqubits,normalize", [(3, False), (4, False)])
 def test_trotter_hamiltonian_matmul(backend, nqubits, normalize):
     """Test Trotter Hamiltonian expectation value."""
     local_ham = hamiltonians.TFIM(nqubits, h=1.0, dense=False, backend=backend)
     dense_ham = hamiltonians.TFIM(nqubits, h=1.0, backend=backend)
 
-    state = backend.cast(random_complex((2 ** nqubits,)))
+    state = backend.cast(random_complex((2**nqubits,)))
     trotter_ev = local_ham.expectation(state, normalize)
     target_ev = dense_ham.expectation(state, normalize)
     backend.assert_allclose(trotter_ev, target_ev)
 
-    state = random_complex((2 ** nqubits,))
+    state = random_complex((2**nqubits,))
     trotter_ev = local_ham.expectation(state, normalize)
     target_ev = dense_ham.expectation(state, normalize)
     backend.assert_allclose(trotter_ev, target_ev)
 
     trotter_matmul = local_ham @ state
     target_matmul = dense_ham @ state
     backend.assert_allclose(trotter_matmul, target_matmul)
 
 
 def test_trotter_hamiltonian_three_qubit_term(backend):
     """Test creating ``TrotterHamiltonian`` with three qubit term."""
     from scipy.linalg import expm
+
     from qibo.hamiltonians.terms import HamiltonianTerm
+
     m1 = random_hermitian(3)
     m2 = random_hermitian(2)
     m3 = random_hermitian(1)
 
-    terms = [HamiltonianTerm(m1, 0, 1, 2), HamiltonianTerm(m2, 2, 3),
-             HamiltonianTerm(m3, 1)]
+    terms = [
+        HamiltonianTerm(m1, 0, 1, 2),
+        HamiltonianTerm(m2, 2, 3),
+        HamiltonianTerm(m3, 1),
+    ]
     ham = hamiltonians.SymbolicHamiltonian(backend=backend)
     ham.terms = terms
 
     # Test that the `TrotterHamiltonian` dense matrix is correct
     eye = np.eye(2, dtype=m1.dtype)
     mm1 = np.kron(m1, eye)
     mm2 = np.kron(np.kron(eye, eye), m2)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_measurements.py` & `qibo-0.1.9/src/qibo/tests/test_measurements.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 """Test circuit result measurements and measurement gate and as part of circuit."""
-import pytest
 import numpy as np
-from qibo import models, gates
+import pytest
+
+from qibo import gates, models
 
 
-def assert_result(backend, result,
-                  decimal_samples=None, binary_samples=None,
-                  decimal_frequencies=None, binary_frequencies=None):
+def assert_result(
+    backend,
+    result,
+    decimal_samples=None,
+    binary_samples=None,
+    decimal_frequencies=None,
+    binary_frequencies=None,
+):
     if decimal_frequencies is not None:
         assert result.frequencies(False) == decimal_frequencies
     if binary_frequencies is not None:
         assert result.frequencies(True) == binary_frequencies
     if decimal_samples is not None:
         backend.assert_allclose(result.samples(False), decimal_samples)
     if binary_samples is not None:
@@ -22,17 +28,22 @@
     for k, v in d1.items():
         if isinstance(v, dict):
             assert v == d2[k]
         else:
             backend.assert_allclose(v, d2[k])
 
 
-def assert_register_result(backend, result,
-                           decimal_samples=None, binary_samples=None,
-                           decimal_frequencies=None, binary_frequencies=None):
+def assert_register_result(
+    backend,
+    result,
+    decimal_samples=None,
+    binary_samples=None,
+    decimal_frequencies=None,
+    binary_frequencies=None,
+):
     if decimal_samples:
         register_result = result.samples(binary=False, registers=True)
         assert_dicts_equal(backend, register_result, decimal_samples)
     if binary_samples:
         register_result = result.samples(binary=True, registers=True)
         assert_dicts_equal(backend, register_result, binary_samples)
     if decimal_frequencies:
@@ -47,27 +58,39 @@
 @pytest.mark.parametrize("nshots", [100, 1000000])
 def test_measurement_gate(backend, n, nshots):
     c = models.Circuit(2)
     if n:
         c.add(gates.X(1))
     c.add(gates.M(1))
     result = backend.execute_circuit(c, nshots=nshots)
-    assert_result(backend, result, n * np.ones(nshots), n * np.ones((nshots, 1)),
-                  {n: nshots}, {str(n): nshots})
+    assert_result(
+        backend,
+        result,
+        n * np.ones(nshots),
+        n * np.ones((nshots, 1)),
+        {n: nshots},
+        {str(n): nshots},
+    )
 
 
 def test_multiple_qubit_measurement_gate(backend):
     c = models.Circuit(2)
     c.add(gates.X(0))
     c.add(gates.M(0, 1))
     result = backend.execute_circuit(c, nshots=100)
     target_binary_samples = np.zeros((100, 2))
     target_binary_samples[:, 0] = 1
-    assert_result(backend, result, 2 * np.ones((100,)), target_binary_samples,
-                  {2: 100}, {"10": 100})
+    assert_result(
+        backend,
+        result,
+        2 * np.ones((100,)),
+        target_binary_samples,
+        {2: 100},
+        {"10": 100},
+    )
 
 
 def test_measurement_gate_errors(backend):
     gate = gates.M(0)
     # attempting to use `controlled_by`
     with pytest.raises(NotImplementedError):
         gate.controlled_by(1)
@@ -77,17 +100,17 @@
 
 
 def test_measurement_circuit(backend, accelerators):
     c = models.Circuit(4, accelerators)
     c.add(gates.X(0))
     c.add(gates.M(0))
     result = backend.execute_circuit(c, nshots=100)
-    assert_result(backend, result,
-                  np.ones((100,)), np.ones((100, 1)),
-                  {1: 100}, {"1": 100})
+    assert_result(
+        backend, result, np.ones((100,)), np.ones((100, 1)), {1: 100}, {"1": 100}
+    )
 
 
 def test_gate_after_measurement_error(backend, accelerators):
     c = models.Circuit(4, accelerators)
     c.add(gates.X(0))
     c.add(gates.M(0))
     c.add(gates.X(1))
@@ -105,66 +128,76 @@
     else:
         c.add(gates.M(1))
         c.add(gates.M(0))
     result = backend.execute_circuit(c, nshots=100)
 
     target_binary_samples = np.zeros((100, 2))
     target_binary_samples[:, 1] = 1
-    assert_result(backend, result,
-                  np.ones(100), target_binary_samples,
-                  {1: 100}, {"01": 100})
+    assert_result(
+        backend, result, np.ones(100), target_binary_samples, {1: 100}, {"01": 100}
+    )
 
 
 @pytest.mark.parametrize("nshots", [100, 1000000])
 def test_measurement_qubit_order(backend, accelerators, nshots):
     c = models.Circuit(6, accelerators)
     c.add(gates.X(0))
     c.add(gates.X(1))
     c.add(gates.M(1, 5, 2, 0))
     result = backend.execute_circuit(c, nshots=nshots)
 
     target_binary_samples = np.zeros((nshots, 4))
     target_binary_samples[:, 0] = 1
     target_binary_samples[:, 3] = 1
-    assert_result(backend, result,
-                  9 * np.ones(nshots), target_binary_samples,
-                  {9: nshots}, {"1001": nshots})
+    assert_result(
+        backend,
+        result,
+        9 * np.ones(nshots),
+        target_binary_samples,
+        {9: nshots},
+        {"1001": nshots},
+    )
 
 
 def test_multiple_measurement_gates_circuit(backend):
     c = models.Circuit(4)
     c.add(gates.X(1))
     c.add(gates.X(2))
     c.add(gates.M(0, 1))
     c.add(gates.M(2))
     c.add(gates.X(3))
     result = backend.execute_circuit(c, nshots=100)
 
     target_binary_samples = np.ones((100, 3))
     target_binary_samples[:, 0] = 0
-    assert_result(backend, result,
-                  3 * np.ones(100), target_binary_samples,
-                  {3: 100}, {"011": 100})
+    assert_result(
+        backend, result, 3 * np.ones(100), target_binary_samples, {3: 100}, {"011": 100}
+    )
 
 
 def test_circuit_with_unmeasured_qubits(backend, accelerators):
     c = models.Circuit(5, accelerators)
     c.add(gates.X(4))
     c.add(gates.X(2))
     c.add(gates.M(0, 2))
     c.add(gates.X(3))
     c.add(gates.M(1, 4))
     result = backend.execute_circuit(c, nshots=100)
 
     target_binary_samples = np.zeros((100, 4))
     target_binary_samples[:, 1] = 1
     target_binary_samples[:, 3] = 1
-    assert_result(backend, result,
-                  5 * np.ones(100), target_binary_samples,
-                  {5: 100}, {"0101": 100})
+    assert_result(
+        backend,
+        result,
+        5 * np.ones(100),
+        target_binary_samples,
+        {5: 100},
+        {"0101": 100},
+    )
 
 
 def test_circuit_addition_with_measurements(backend):
     c = models.Circuit(2)
     c.add(gates.H(0))
     c.add(gates.H(1))
 
@@ -231,17 +264,22 @@
     c.add(gates.X(0))
     c.add(gates.M(0))
     c.add(gates.M(1))
     c.compile(backend)
     result = c(nshots=100)
     target_binary_samples = np.zeros((100, 2))
     target_binary_samples[:, 0] = 1
-    assert_result(backend, result,
-                  2 * np.ones((100,)), target_binary_samples,
-                  {2: 100}, {"10": 100})
+    assert_result(
+        backend,
+        result,
+        2 * np.ones((100,)),
+        target_binary_samples,
+        {2: 100},
+        {"10": 100},
+    )
 
     target_state = np.zeros_like(c.final_state)
     target_state[2] = 1
     backend.assert_allclose(c.final_state, target_state)
 
 
 def test_final_state(backend, accelerators):
@@ -275,23 +313,27 @@
     c = models.Circuit(3)
     c.add(gates.X(0))
     c.add(gates.X(1))
     c.add(gates.M(0, 2))
     c.add(gates.M(1))
     result = backend.execute_circuit(c, nshots=100)
 
-    decimal_samples = {"register0": 2 * np.ones((100,)),
-                        "register1": np.ones((100,))}
-    binary_samples = {"register0": np.zeros((100, 2)),
-                      "register1": np.ones((100, 1))}
+    decimal_samples = {"register0": 2 * np.ones((100,)), "register1": np.ones((100,))}
+    binary_samples = {"register0": np.zeros((100, 2)), "register1": np.ones((100, 1))}
     binary_samples["register0"][:, 0] = 1
     decimal_frequencies = {"register0": {2: 100}, "register1": {1: 100}}
     binary_frequencies = {"register0": {"10": 100}, "register1": {"1": 100}}
-    assert_register_result(backend, result, decimal_samples, binary_samples,
-                           decimal_frequencies, binary_frequencies)
+    assert_register_result(
+        backend,
+        result,
+        decimal_samples,
+        binary_samples,
+        decimal_frequencies,
+        binary_frequencies,
+    )
 
 
 def test_register_name_error(backend):
     c = models.Circuit(2)
     c.add(gates.X(0))
     c.add(gates.M(0, register_name="a"))
     with pytest.raises(KeyError):
@@ -322,27 +364,38 @@
     result = backend.execute_circuit(c, nshots=100)
 
     # Check full result
     target_binary_samples = np.zeros((100, 5))
     target_binary_samples[:, 1] = 1
     target_binary_samples[:, 2] = 1
     target_binary_samples[:, 4] = 1
-    assert_result(backend, result,
-                  13 * np.ones((100,)), target_binary_samples,
-                  {13: 100}, {"01101": 100})
+    assert_result(
+        backend,
+        result,
+        13 * np.ones((100,)),
+        target_binary_samples,
+        {13: 100},
+        {"01101": 100},
+    )
 
     decimal_samples = {"a": 3 * np.ones((100,)), "b": np.ones((100,))}
     binary_samples = {"a": np.zeros((100, 3)), "b": np.zeros((100, 2))}
     binary_samples["a"][:, 1] = 1
     binary_samples["a"][:, 2] = 1
     binary_samples["b"][:, 1] = 1
     decimal_frequencies = {"a": {3: 100}, "b": {1: 100}}
     binary_frequencies = {"a": {"011": 100}, "b": {"01": 100}}
-    assert_register_result(backend, result, decimal_samples, binary_samples,
-                           decimal_frequencies, binary_frequencies)
+    assert_register_result(
+        backend,
+        result,
+        decimal_samples,
+        binary_samples,
+        decimal_frequencies,
+        binary_frequencies,
+    )
 
 
 def test_registers_in_circuit_with_unmeasured_qubits(backend, accelerators):
     """Check that register measurements are unaffected by unmeasured qubits."""
     c = models.Circuit(5, accelerators)
     c.add(gates.X(1))
     c.add(gates.X(2))
@@ -354,24 +407,32 @@
     target = {}
     decimal_samples = {"A": np.ones((100,)), "B": 2 * np.ones((100,))}
     binary_samples = {"A": np.zeros((100, 2)), "B": np.zeros((100, 2))}
     binary_samples["A"][:, 1] = 1
     binary_samples["B"][:, 0] = 1
     decimal_frequencies = {"A": {1: 100}, "B": {2: 100}}
     binary_frequencies = {"A": {"01": 100}, "B": {"10": 100}}
-    assert_register_result(backend, result,
-                           decimal_samples, binary_samples,
-                           decimal_frequencies, binary_frequencies)
+    assert_register_result(
+        backend,
+        result,
+        decimal_samples,
+        binary_samples,
+        decimal_frequencies,
+        binary_frequencies,
+    )
 
 
 def test_measurement_density_matrix(backend):
     c = models.Circuit(2, density_matrix=True)
     c.add(gates.X(0))
     c.add(gates.M(0, 1))
     result = backend.execute_circuit(c, nshots=100)
     target_binary_samples = np.zeros((100, 2))
     target_binary_samples[:, 0] = 1
-    assert_result(backend, result,
-                  decimal_samples=2 * np.ones((100,)),
-                  binary_samples=target_binary_samples,
-                  decimal_frequencies={2: 100},
-                  binary_frequencies={"10": 100})
+    assert_result(
+        backend,
+        result,
+        decimal_samples=2 * np.ones((100,)),
+        binary_samples=target_binary_samples,
+        decimal_frequencies={2: 100},
+        binary_frequencies={"10": 100},
+    )
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_measurements_collapse.py` & `qibo-0.1.9/src/qibo/tests/test_measurements_collapse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Test :class:`qibo.gates.M` as standalone and as part of circuit."""
-import pytest
 import numpy as np
-from qibo import models, gates
-from qibo.tests.utils import random_state, random_density_matrix
+import pytest
+
+from qibo import gates, models
+from qibo.tests.utils import random_density_matrix, random_state
 
 
-@pytest.mark.parametrize("nqubits,targets",
-                         [(2, [1]), (3, [1]), (4, [1, 3]), (5, [0, 3, 4]),
-                          (6, [1, 3]), (4, [0, 2])])
+@pytest.mark.parametrize(
+    "nqubits,targets",
+    [(2, [1]), (3, [1]), (4, [1, 3]), (5, [0, 3, 4]), (6, [1, 3]), (4, [0, 2])],
+)
 def test_measurement_collapse(backend, nqubits, targets):
     initial_state = random_state(nqubits)
     c = models.Circuit(nqubits)
     m = c.add(gates.M(*targets, collapse=True))
     final_state = backend.execute_circuit(c, np.copy(initial_state), nshots=1)[0]
     if len(targets) > 1:
         results = m[0].result.samples[0]
@@ -25,16 +27,17 @@
     target_state = np.zeros_like(initial_state)
     target_state[slicer] = initial_state[slicer]
     norm = (np.abs(target_state) ** 2).sum()
     target_state = target_state.ravel() / np.sqrt(norm)
     backend.assert_allclose(final_state, target_state)
 
 
-@pytest.mark.parametrize("nqubits,targets",
-                         [(2, [1]), (3, [1]), (4, [1, 3]), (5, [0, 3, 4])])
+@pytest.mark.parametrize(
+    "nqubits,targets", [(2, [1]), (3, [1]), (4, [1, 3]), (5, [0, 3, 4])]
+)
 def test_measurement_collapse_density_matrix(backend, nqubits, targets):
     initial_rho = random_density_matrix(nqubits)
     c = models.Circuit(nqubits, density_matrix=True)
     m = c.add(gates.M(*targets, collapse=True))
     final_rho = backend.execute_circuit(c, np.copy(initial_rho), nshots=1)[0]
 
     if len(targets) > 1:
@@ -84,20 +87,24 @@
 def test_measurement_result_parameters_random(backend):
     initial_state = random_state(4)
     backend.set_seed(123)
     c = models.Circuit(4)
     output = c.add(gates.M(1, collapse=True))
     c.add(gates.RY(0, theta=np.pi * output / 5))
     c.add(gates.RX(2, theta=np.pi * output / 4))
-    final_state = backend.execute_circuit(c, initial_state=np.copy(initial_state), nshots=1)[0]
+    final_state = backend.execute_circuit(
+        c, initial_state=np.copy(initial_state), nshots=1
+    )[0]
 
     backend.set_seed(123)
     c = models.Circuit(4)
     m = c.add(gates.M(1, collapse=True))
-    target_state = backend.execute_circuit(c, initial_state=np.copy(initial_state), nshots=1)[0]
+    target_state = backend.execute_circuit(
+        c, initial_state=np.copy(initial_state), nshots=1
+    )[0]
     if int(m.outcome()):
         c = models.Circuit(4)
         c.add(gates.RY(0, theta=np.pi / 5))
         c.add(gates.RX(2, theta=np.pi / 4))
         target_state = backend.execute_circuit(c, initial_state=target_state)
     backend.assert_allclose(final_state, target_state)
 
@@ -108,27 +115,33 @@
     backend.set_seed(123)
     c = models.Circuit(4)
     output = c.add(gates.M(1, collapse=True))
     c.add(gates.RX(2, theta=np.pi * output / 4))
     if use_loop:
         final_states = []
         for _ in range(20):
-            final_state = backend.execute_circuit(c, initial_state=np.copy(initial_state), nshots=1)
+            final_state = backend.execute_circuit(
+                c, initial_state=np.copy(initial_state), nshots=1
+            )
             final_states.append(final_state[0])
     else:
-        final_states = backend.execute_circuit(c, initial_state=np.copy(initial_state), nshots=20)
+        final_states = backend.execute_circuit(
+            c, initial_state=np.copy(initial_state), nshots=20
+        )
 
     backend.set_seed(123)
     target_states = []
     for _ in range(20):
         c = models.Circuit(4)
         m = c.add(gates.M(1, collapse=True))
         target_state = backend.execute_circuit(c, np.copy(initial_state), nshots=1)[0]
         if int(m.outcome()):
-            target_state = backend.apply_gate(gates.RX(2, theta=np.pi / 4), target_state, 4)
+            target_state = backend.apply_gate(
+                gates.RX(2, theta=np.pi / 4), target_state, 4
+            )
         target_states.append(backend.to_numpy(target_state))
 
     final_states = [backend.to_numpy(x) for x in final_states]
     backend.assert_allclose(final_states, target_states)
 
 
 def test_measurement_result_parameters_repeated_execution_final_measurements(backend):
@@ -169,17 +182,17 @@
 
     backend.set_seed(123)
     c = models.Circuit(4)
     m = c.add(gates.M(0, 1, 2, collapse=True))
     target_state = backend.execute_circuit(c, np.copy(initial_state), nshots=1)[0]
     # not including in coverage because outcomes are probabilistic and may
     # not occur for the CI run
-    if int(m[0].outcome()): # pragma: no cover
+    if int(m[0].outcome()):  # pragma: no cover
         target_state = backend.apply_gate(gates.RY(1, theta=np.pi / 5), target_state, 4)
-    if int(m[2].outcome()): # pragma: no cover
+    if int(m[2].outcome()):  # pragma: no cover
         target_state = backend.apply_gate(gates.RX(3, theta=np.pi / 3), target_state, 4)
     backend.assert_allclose(final_state, target_state)
 
 
 @pytest.mark.parametrize("nqubits,targets", [(5, [2, 4]), (6, [3, 5])])
 def test_measurement_collapse_distributed(backend, accelerators, nqubits, targets):
     initial_state = random_state(nqubits)
@@ -198,20 +211,20 @@
     target_state = target_state.ravel() / np.sqrt(norm)
     backend.assert_allclose(result[0], target_state)
 
 
 def test_collapse_after_measurement(backend):
     qubits = [0, 2, 3]
     c = models.Circuit(5)
-    c.add((gates.H(i) for i in range(5)))
+    c.add(gates.H(i) for i in range(5))
     output = c.add(gates.M(*qubits, collapse=True))
-    c.add((gates.H(i) for i in range(5)))
+    c.add(gates.H(i) for i in range(5))
     final_state = backend.execute_circuit(c, nshots=1)[0]
 
     ct = models.Circuit(5)
     bitstring = [r.outcome() for r in output]
     for i, r in zip(qubits, bitstring):
         if r:
             ct.add(gates.X(i))
-    ct.add((gates.H(i) for i in qubits))
+    ct.add(gates.H(i) for i in qubits)
     target_state = backend.execute_circuit(ct)
     backend.assert_allclose(final_state, target_state, atol=1e-15)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_measurements_probabilistic.py` & `qibo-0.1.9/src/qibo/tests/test_measurements_probabilistic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Test circuit measurements when outcome is probabilistic."""
 import sys
-import pytest
+
 import numpy as np
-from qibo import models, gates
+import pytest
+
+from qibo import gates, models
 from qibo.tests.test_measurements import assert_result
 
 
 @pytest.mark.parametrize("use_samples", [True, False])
 def test_probabilistic_measurement(backend, accelerators, use_samples):
     # set single-thread to fix the random values generated from the frequency custom op
     backend.set_threads(1)
@@ -39,26 +41,27 @@
 
     backend.set_seed(1234)
     if use_samples:
         # calculates sample tensor directly using `tf.random.categorical`
         # otherwise it uses the frequency-only calculation
         _ = result.samples()
     # update reference values based on backend and device
-    decimal_frequencies = backend.test_regressions("test_unbalanced_probabilistic_measurement")
+    decimal_frequencies = backend.test_regressions(
+        "test_unbalanced_probabilistic_measurement"
+    )
     assert sum(result.frequencies().values()) == 1000
     assert_result(backend, result, decimal_frequencies=decimal_frequencies)
 
 
 def test_measurements_with_probabilistic_noise(backend):
     """Check measurements when simulating noise with repeated execution."""
     thetas = np.random.random(5)
     c = models.Circuit(5)
     c.add((gates.RX(i, t) for i, t in enumerate(thetas)))
-    c.add((gates.PauliNoiseChannel(i, px=0.0, py=0.2, pz=0.4)
-           for i in range(5)))
+    c.add(gates.PauliNoiseChannel(i, px=0.0, py=0.2, pz=0.4) for i in range(5))
     c.add(gates.M(*range(5)))
     backend.set_seed(123)
     result = backend.execute_circuit(c, nshots=20)
     samples = result.samples()
 
     backend.set_seed(123)
     target_samples = []
@@ -73,17 +76,17 @@
         noiseless_c.add(gates.M(*range(5)))
         result = backend.execute_circuit(noiseless_c, nshots=1)
         target_samples.append(backend.to_numpy(result.samples()))
     target_samples = np.concatenate(target_samples, axis=0)
     backend.assert_allclose(samples, target_samples)
 
 
-@pytest.mark.parametrize("i,probs", [(0, [0.0, 0.0, 0.0]),
-                                     (1, [0.1, 0.3, 0.2]),
-                                     (2, [0.5, 0.5, 0.5])])
+@pytest.mark.parametrize(
+    "i,probs", [(0, [0.0, 0.0, 0.0]), (1, [0.1, 0.3, 0.2]), (2, [0.5, 0.5, 0.5])]
+)
 def test_post_measurement_bitflips_on_circuit(backend, accelerators, i, probs):
     """Check bitflip errors on circuit measurements."""
     backend.set_seed(123)
     c = models.Circuit(5, accelerators=accelerators)
     c.add([gates.X(0), gates.X(2), gates.X(3)])
     c.add(gates.M(0, 1, p0={0: probs[0], 1: probs[1]}))
     c.add(gates.M(3, p0=probs[2]))
@@ -104,20 +107,26 @@
     result = backend.execute_circuit(c, nshots=30)
     samples = result.samples(binary=True)
     register_samples = result.samples(binary=True, registers=True)
     backend.assert_allclose(register_samples["a"], samples[:, :2])
     backend.assert_allclose(register_samples["b"], samples[:, 2:])
 
 
-@pytest.mark.parametrize("i,p0,p1",
-                         [(0, 0.2, None), (1, 0.2, 0.1),
-                          (2, (0.1, 0.0, 0.2), None),
-                          (3, {0: 0.2, 1: 0.1, 2: 0.0}, None)])
+@pytest.mark.parametrize(
+    "i,p0,p1",
+    [
+        (0, 0.2, None),
+        (1, 0.2, 0.1),
+        (2, (0.1, 0.0, 0.2), None),
+        (3, {0: 0.2, 1: 0.1, 2: 0.0}, None),
+    ],
+)
 def test_measurementresult_apply_bitflips(backend, i, p0, p1):
     from qibo.states import CircuitResult
+
     c = models.Circuit(3)
     c.add(gates.M(*range(3)))
     result = CircuitResult(backend, c, None)
     result._samples = np.zeros(10, dtype="int64")
     backend.set_seed(123)
     noisy_samples = result.apply_bitflips(p0, p1)
     targets = backend.test_regressions("test_measurementresult_apply_bitflips")
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 """Test all methods defined in `qibo/models/circuit.py`."""
 import pytest
+
 from qibo import gates
-from qibo.models import Circuit
 from qibo.config import raise_error
+from qibo.models import Circuit
 
 
 def test_parametrizedgates_class():
     from qibo.models.circuit import _ParametrizedGates
+
     paramgates = _ParametrizedGates()
     paramgates.append(gates.RX(0, 0.1234))
     paramgates.append(gates.fSim(0, 1, 0.1234, 0.4321))
     assert len(paramgates.set) == 2
     assert paramgates.nparams == 3
 
 
 def test_queue_class():
     from qibo.models.circuit import _Queue
+
     queue = _Queue(4)
-    gatelist = [gates.H(0), gates.H(1), gates.X(0),
-                gates.H(2), gates.CNOT(1, 2), gates.Y(3)]
+    gatelist = [
+        gates.H(0),
+        gates.H(1),
+        gates.X(0),
+        gates.H(2),
+        gates.CNOT(1, 2),
+        gates.Y(3),
+    ]
     for g in gatelist:
         queue.append(g)
-    assert queue.moments == [[gatelist[0], gatelist[1], gatelist[3], gatelist[5]],
-                             [gatelist[2], gatelist[4], gatelist[4], None]]
+    assert queue.moments == [
+        [gatelist[0], gatelist[1], gatelist[3], gatelist[5]],
+        [gatelist[2], gatelist[4], gatelist[4], None],
+    ]
 
 
 def test_circuit_init():
     c = Circuit(2)
     assert c.nqubits == 2
 
 
@@ -84,32 +95,35 @@
     assert c.depth == 4
     assert c.ngates == 6
     assert isinstance(c.queue[-1], gates.CNOT)
 
 
 def test_circuit_add_generator():
     """Check if `circuit.add` works with generators."""
+
     def gen():
         yield gates.H(0)
         yield gates.H(1)
         yield gates.CNOT(0, 1)
+
     c = Circuit(2)
     c.add(gen())
     assert c.depth == 2
     assert c.ngates == 3
     assert isinstance(c.queue[-1], gates.CNOT)
 
 
 def test_circuit_add_nested_generator():
     def gen():
         yield gates.H(0)
         yield gates.H(1)
         yield gates.CNOT(0, 1)
+
     c = Circuit(2)
-    c.add((gen() for _ in range(3)))
+    c.add(gen() for _ in range(3))
     assert c.depth == 6
     assert c.ngates == 9
     assert isinstance(c.queue[2], gates.CNOT)
     assert isinstance(c.queue[5], gates.CNOT)
     assert isinstance(c.queue[7], gates.H)
 
 
@@ -124,16 +138,18 @@
     assert g2.target_qubits == (3,)
     with pytest.raises(KeyError):
         c.add(gates.M(4, register_name="b"))
 
 
 # :meth:`qibo.core.circuit.Circuit.fuse` is tested in `test_core_fusion.py`
 
+
 def test_gate_types():
     import collections
+
     c = Circuit(3)
     c.add(gates.H(0))
     c.add(gates.H(1))
     c.add(gates.X(2))
     c.add(gates.CNOT(0, 2))
     c.add(gates.CNOT(1, 2))
     c.add(gates.TOFFOLI(0, 1, 2))
@@ -163,19 +179,25 @@
     c = Circuit(3)
     c.add(gates.H(0))
     c.add(gates.H(1))
     c.add(gates.CNOT(0, 2))
     c.add(gates.CNOT(1, 2))
     c.add(gates.TOFFOLI(0, 1, 2))
     c.add(gates.H(2))
-    target_summary = "\n".join(["Circuit depth = 5",
-                                "Total number of gates = 6",
-                                "Number of qubits = 3",
-                                "Most common gates:",
-                                "h: 3", "cx: 2", "ccx: 1"])
+    target_summary = "\n".join(
+        [
+            "Circuit depth = 5",
+            "Total number of gates = 6",
+            "Number of qubits = 3",
+            "Most common gates:",
+            "h: 3",
+            "cx: 2",
+            "ccx: 1",
+        ]
+    )
     assert c.summary() == target_summary
 
 
 @pytest.mark.parametrize("measurements", [False, True])
 def test_circuit_addition(measurements):
     c1 = Circuit(2)
     g1, g2 = gates.H(0), gates.CNOT(0, 1)
@@ -225,27 +247,29 @@
     assert new_gates[4].control_qubits == (5,)
     assert new_gates[5].target_qubits == (5,)
     assert new_gates[5].control_qubits == (2, 4)
 
 
 def test_circuit_on_qubits_errors():
     smallc = Circuit(2)
-    smallc.add((gates.H(i) for i in range(2)))
+    smallc.add(gates.H(i) for i in range(2))
     with pytest.raises(ValueError):
         next(smallc.on_qubits(0, 1, 2))
 
     from qibo.callbacks import Callback
+
     smallc = Circuit(4)
     smallc.add(gates.CallbackGate(Callback()))
     with pytest.raises(NotImplementedError):
         next(smallc.on_qubits(0, 1, 2, 3))
 
 
 def test_circuit_light_cone():
     from qibo import __version__
+
     nqubits = 10
     c = Circuit(nqubits)
     c.add(gates.RY(i, theta=0) for i in range(nqubits))
     c.add(gates.CZ(i, i + 1) for i in range(0, nqubits - 1, 2))
     c.add(gates.RY(i, theta=0) for i in range(nqubits))
     c.add(gates.CZ(i, i + 1) for i in range(1, nqubits - 1, 2))
     c.add(gates.CZ(0, nqubits - 1))
@@ -315,16 +339,15 @@
     assert c2.measurement_gate is c1.measurement_gate
     assert c2.measurement_tuples == {"a": (0, 1), "b": (3,)}
 
 
 @pytest.mark.parametrize("measurements", [False, True])
 def test_circuit_invert(measurements):
     c = Circuit(3)
-    gatelist = [gates.H(0), gates.X(1), gates.Y(2),
-                gates.CNOT(0, 1), gates.CZ(1, 2)]
+    gatelist = [gates.H(0), gates.X(1), gates.Y(2), gates.CNOT(0, 1), gates.CZ(1, 2)]
     c.add(gatelist)
     if measurements:
         c.add(gates.M(0, 2))
     invc = c.invert()
     for g1, g2 in zip(invc.queue, gatelist[::-1]):
         g2 = g2.dagger()
         assert isinstance(g1, g2.__class__)
@@ -353,17 +376,17 @@
         assert g1.control_qubits == g2.control_qubits
     if measurements:
         assert decompc.measurement_gate.target_qubits == (0, 2)
         assert decompc.measurement_tuples == {"register0": (0, 2)}
 
 
 @pytest.mark.parametrize("measurements", [False, True])
-@pytest.mark.parametrize("noise_map",
-                         [(0.1, 0.2, 0.3),
-                          {0: (0.1, 0.0, 0.2), 1: (0.0, 0.2, 0.1)}])
+@pytest.mark.parametrize(
+    "noise_map", [(0.1, 0.2, 0.3), {0: (0.1, 0.0, 0.2), 1: (0.0, 0.2, 0.1)}]
+)
 def test_circuit_with_noise(measurements, noise_map):
     c = Circuit(2)
     c.add([gates.H(0), gates.H(1), gates.CNOT(0, 1)])
     if measurements:
         c.add(gates.M(0, 1))
     noisyc = c.with_noise(noise_map)
 
@@ -387,38 +410,42 @@
 
 
 @pytest.mark.parametrize("trainable", [True, False])
 @pytest.mark.parametrize("include_not_trainable", [True, False])
 @pytest.mark.parametrize("format", ["list", "dict", "flatlist"])
 def test_get_parameters(trainable, include_not_trainable, format):
     import numpy as np
+
     matrix = np.random.random((2, 2))
     c = Circuit(3)
     c.add(gates.RX(0, theta=0.123))
     c.add(gates.RY(1, theta=0.456, trainable=trainable))
     c.add(gates.CZ(1, 2))
     c.add(gates.Unitary(matrix, 2))
     c.add(gates.fSim(0, 2, theta=0.789, phi=0.987, trainable=trainable))
     c.add(gates.H(2))
     params = c.get_parameters(format, include_not_trainable)
     if trainable or include_not_trainable:
         target_params = {
             "list": [(0.123,), (0.456,), (0.789, 0.987)],
-            "dict": {c.queue[0]: (0.123,), c.queue[1]: (0.456,),
-                     c.queue[4]: (0.789, 0.987)},
-            "flatlist": [0.123, 0.456]
-            }
+            "dict": {
+                c.queue[0]: (0.123,),
+                c.queue[1]: (0.456,),
+                c.queue[4]: (0.789, 0.987),
+            },
+            "flatlist": [0.123, 0.456],
+        }
         target_params["flatlist"].extend(list(matrix.ravel()))
         target_params["flatlist"].extend([0.789, 0.987])
     else:
         target_params = {
             "list": [(0.123,)],
             "dict": {c.queue[0]: (0.123,)},
-            "flatlist": [0.123]
-            }
+            "flatlist": [0.123],
+        }
         target_params["flatlist"].extend(list(matrix.ravel()))
     if format == "list":
         i = len(target_params["list"]) // 2 + 1
         np.testing.assert_allclose(params.pop(i)[0], matrix)
     elif format == "dict":
         np.testing.assert_allclose(params.pop(c.queue[3])[0], matrix)
     assert params == target_params[format]
@@ -501,123 +528,139 @@
         c.set_parameters({0.3568})
     with pytest.raises(ValueError):
         c.queue[2].parameters = [0.1234, 0.4321, 0.156]
 
 
 def test_circuit_draw():
     """Test circuit text draw."""
-    ref = 'q0: ─H─U1─U1─U1─U1───────────────────────────x───\n' \
-          'q1: ───o──|──|──|──H─U1─U1─U1────────────────|─x─\n' \
-          'q2: ──────o──|──|────o──|──|──H─U1─U1────────|─|─\n' \
-          'q3: ─────────o──|───────o──|────o──|──H─U1───|─x─\n' \
-          'q4: ────────────o──────────o───────o────o──H─x───'
+    ref = (
+        "q0: ─H─U1─U1─U1─U1───────────────────────────x───\n"
+        "q1: ───o──|──|──|──H─U1─U1─U1────────────────|─x─\n"
+        "q2: ──────o──|──|────o──|──|──H─U1─U1────────|─|─\n"
+        "q3: ─────────o──|───────o──|────o──|──H─U1───|─x─\n"
+        "q4: ────────────o──────────o───────o────o──H─x───"
+    )
     circuit = Circuit(5)
     for i1 in range(5):
         circuit.add(gates.H(i1))
         for i2 in range(i1 + 1, 5):
             circuit.add(gates.CU1(i2, i1, theta=0))
     circuit.add(gates.SWAP(0, 4))
     circuit.add(gates.SWAP(1, 3))
     assert circuit.draw() == ref
 
 
 def test_circuit_draw_line_wrap():
     """Test circuit text draw with line wrap."""
-    ref_line_wrap_50 = \
-        'q0:     ─H─U1─U1─U1─U1───────────────────────────x───I───f ...\n' \
-        'q1:     ───o──|──|──|──H─U1─U1─U1────────────────|─x─I───| ...\n' \
-        'q2:     ──────o──|──|────o──|──|──H─U1─U1────────|─|─────| ...\n' \
-        'q3:     ─────────o──|───────o──|────o──|──H─U1───|─x───M─| ...\n' \
-        'q4:     ────────────o──────────o───────o────o──H─x───────f ...\n' \
-        '\n' \
-        'q0: ... ─o────gf───M─\n' \
-        'q1: ... ─U3───|──o─M─\n' \
-        'q2: ... ────X─gf─o─M─\n' \
-        'q3: ... ────o────o───\n' \
-        'q4: ... ────o────X───'
-
-    ref_line_wrap_30 = \
-        'q0:     ─H─U1─U1─U1─U1──────────────── ...\n' \
-        'q1:     ───o──|──|──|──H─U1─U1─U1───── ...\n' \
-        'q2:     ──────o──|──|────o──|──|──H─U1 ...\n' \
-        'q3:     ─────────o──|───────o──|────o─ ...\n' \
-        'q4:     ────────────o──────────o────── ...\n' \
-        '\n' \
-        'q0: ... ───────────x───I───f─o────gf── ...\n' \
-        'q1: ... ───────────|─x─I───|─U3───|──o ...\n' \
-        'q2: ... ─U1────────|─|─────|────X─gf─o ...\n' \
-        'q3: ... ─|──H─U1───|─x───M─|────o────o ...\n' \
-        'q4: ... ─o────o──H─x───────f────o────X ...\n' \
-        '\n' \
-        'q0: ... ─M─\n' \
-        'q1: ... ─M─\n' \
-        'q2: ... ─M─\n' \
-        'q3: ... ───\n' \
-        'q4: ... ───'
+    ref_line_wrap_50 = (
+        "q0:     ─H─U1─U1─U1─U1───────────────────────────x───I───f ...\n"
+        "q1:     ───o──|──|──|──H─U1─U1─U1────────────────|─x─I───| ...\n"
+        "q2:     ──────o──|──|────o──|──|──H─U1─U1────────|─|─────| ...\n"
+        "q3:     ─────────o──|───────o──|────o──|──H─U1───|─x───M─| ...\n"
+        "q4:     ────────────o──────────o───────o────o──H─x───────f ...\n"
+        "\n"
+        "q0: ... ─o────gf───M─\n"
+        "q1: ... ─U3───|──o─M─\n"
+        "q2: ... ────X─gf─o─M─\n"
+        "q3: ... ────o────o───\n"
+        "q4: ... ────o────X───"
+    )
+
+    ref_line_wrap_30 = (
+        "q0:     ─H─U1─U1─U1─U1──────────────── ...\n"
+        "q1:     ───o──|──|──|──H─U1─U1─U1───── ...\n"
+        "q2:     ──────o──|──|────o──|──|──H─U1 ...\n"
+        "q3:     ─────────o──|───────o──|────o─ ...\n"
+        "q4:     ────────────o──────────o────── ...\n"
+        "\n"
+        "q0: ... ───────────x───I───f─o────gf── ...\n"
+        "q1: ... ───────────|─x─I───|─U3───|──o ...\n"
+        "q2: ... ─U1────────|─|─────|────X─gf─o ...\n"
+        "q3: ... ─|──H─U1───|─x───M─|────o────o ...\n"
+        "q4: ... ─o────o──H─x───────f────o────X ...\n"
+        "\n"
+        "q0: ... ─M─\n"
+        "q1: ... ─M─\n"
+        "q2: ... ─M─\n"
+        "q3: ... ───\n"
+        "q4: ... ───"
+    )
 
     import numpy as np
+
     circuit = Circuit(5)
     for i1 in range(5):
         circuit.add(gates.H(i1))
         for i2 in range(i1 + 1, 5):
             circuit.add(gates.CU1(i2, i1, theta=0))
     circuit.add(gates.SWAP(0, 4))
     circuit.add(gates.SWAP(1, 3))
     circuit.add(gates.I(*range(2)))
     circuit.add(gates.M(3, collapse=True))
-    circuit.add(gates.fSim(0,4,0,0))
-    circuit.add(gates.CU3(0,1,0,0,0))
-    circuit.add(gates.TOFFOLI(4,3,2))
+    circuit.add(gates.fSim(0, 4, 0, 0))
+    circuit.add(gates.CU3(0, 1, 0, 0, 0))
+    circuit.add(gates.TOFFOLI(4, 3, 2))
     circuit.add(gates.GeneralizedfSim(0, 2, np.eye(2), 0))
-    circuit.add(gates.X(4).controlled_by(1,2,3))
+    circuit.add(gates.X(4).controlled_by(1, 2, 3))
     circuit.add(gates.M(*range(3)))
     assert circuit.draw(line_wrap=50) == ref_line_wrap_50
     assert circuit.draw(line_wrap=30) == ref_line_wrap_30
 
 
 @pytest.mark.parametrize("legend", [True, False])
 def test_circuit_draw_channels(legend):
     """Check that channels are drawn correctly"""
     from qibo.models import Circuit as circuit
+
     c = circuit(2, density_matrix=True)
     c.add(gates.H(0))
     c.add(gates.PauliNoiseChannel(0, 0.1, 0.0, 0.2))
     c.add(gates.H(1))
     c.add(gates.PauliNoiseChannel(1, 0.0, 0.2, 0.1))
     c.add(gates.CNOT(0, 1))
     c.add(gates.PauliNoiseChannel(0, 0.1, 0.0, 0.2))
     c.add(gates.PauliNoiseChannel(1, 0.0, 0.2, 0.1))
+    c.add(gates.CNOT(0, 1))
+    c.add(gates.DepolarizingChannel((0, 1), 0.1))
+    c.add(gates.CNOT(0, 1))
+    c.add(gates.DepolarizingChannel((0,), 0.1))
+    c.add(gates.CNOT(0, 1))
+    c.add(gates.DepolarizingChannel((1,), 0.1))
 
-    ref = 'q0: ─H─PN─o─PN─\n' \
-          'q1: ─H─PN─X─PN─'
+    ref = "q0: ─H─PN─o─PN─o─D─o─D─o───\n" "q1: ─H─PN─X─PN─X─D─X───X─D─"
 
     if legend:
-        ref += '\n\n Legend for callbacks and channels: \n' \
-               '| Gate              | Symbol   |\n' \
-               '|-------------------+----------|\n' \
-               '| PauliNoiseChannel | PN       |'
+        ref += (
+            "\n\n Legend for callbacks and channels: \n"
+            "| Gate                | Symbol   |\n"
+            "|---------------------+----------|\n"
+            "| PauliNoiseChannel   | PN       |\n"
+            "| DepolarizingChannel | D        |"
+        )
 
     assert c.draw(legend=legend) == ref
 
 
 @pytest.mark.parametrize("legend", [True, False])
 def test_circuit_draw_callbacks(legend):
     """Check that callbacks are drawn correcly"""
     from qibo.callbacks import EntanglementEntropy
+
     entropy = EntanglementEntropy([0])
     c = Circuit(2)
     c.add(gates.CallbackGate(entropy))
     c.add(gates.H(0))
     c.add(gates.CallbackGate(entropy))
     c.add(gates.CNOT(0, 1))
     c.add(gates.CallbackGate(entropy))
 
-    ref = 'q0: ─EE─H─EE─o─EE─\n' \
-          'q1: ─EE───EE─X─EE─'
+    ref = "q0: ─EE─H─EE─o─EE─\n" "q1: ─EE───EE─X─EE─"
 
     if legend:
-        ref += '\n\n Legend for callbacks and channels: \n' \
-               '| Gate                | Symbol   |\n'\
-               '|---------------------+----------|\n'\
-               '| EntanglementEntropy | EE       |'
+        ref += (
+            "\n\n Legend for callbacks and channels: \n"
+            "| Gate                | Symbol   |\n"
+            "|---------------------+----------|\n"
+            "| EntanglementEntropy | EE       |"
+        )
 
     assert c.draw(legend=legend) == ref
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_backpropagation.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_backpropagation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 """Tests Tensorflow's backpropagation when using `tf.Variable` parameters."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 
 
 def construct_tensorflow_backend():
     try:
         from qibo.backends import construct_backend
+
         backend = construct_backend("tensorflow")
-    except ModuleNotFoundError: # pragma: no cover
-        pytest.skip("Skipping backpropagation test because tensorflow is not available.")
+    except ModuleNotFoundError:  # pragma: no cover
+        pytest.skip(
+            "Skipping backpropagation test because tensorflow is not available."
+        )
     return backend
 
 
 def test_variable_backpropagation():
     backend = construct_tensorflow_backend()
     import tensorflow as tf
+
     theta = tf.Variable(0.1234, dtype="float64")
     # TODO: Fix parametrized gates so that `Circuit` can be defined outside
     # of the gradient tape
     with tf.GradientTape() as tape:
         c = Circuit(1)
         c.add(gates.X(0))
         c.add(gates.RZ(0, theta))
         result = backend.execute_circuit(c)
         loss = tf.math.real(result.state()[-1])
     grad = tape.gradient(loss, theta)
 
     target_loss = np.cos(theta / 2.0)
     backend.assert_allclose(loss, target_loss)
 
-    target_grad = - np.sin(theta / 2.0) / 2.0
+    target_grad = -np.sin(theta / 2.0) / 2.0
     backend.assert_allclose(grad, target_grad)
 
 
 def test_two_variables_backpropagation():
     backend = construct_tensorflow_backend()
     import tensorflow as tf
+
     theta = tf.Variable([0.1234, 0.4321], dtype="float64")
     # TODO: Fix parametrized gates so that `Circuit` can be defined outside
     # of the gradient tape
     with tf.GradientTape() as tape:
         c = Circuit(2)
         c.add(gates.RX(0, theta[0]))
         c.add(gates.RY(1, theta[1]))
@@ -49,11 +55,11 @@
         loss = tf.math.real(result.state()[0])
     grad = tape.gradient(loss, theta)
 
     t = np.array([0.1234, 0.4321]) / 2.0
     target_loss = np.cos(t[0]) * np.cos(t[1])
     backend.assert_allclose(loss, target_loss)
 
-    target_grad1 = - np.sin(t[0]) * np.cos(t[1])
-    target_grad2 = - np.cos(t[0]) * np.sin(t[1])
+    target_grad1 = -np.sin(t[0]) * np.cos(t[1])
+    target_grad2 = -np.cos(t[0]) * np.sin(t[1])
     target_grad = np.array([target_grad1, target_grad2]) / 2.0
     backend.assert_allclose(grad, target_grad)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_execution.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_execution.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 
 
 def test_eager_execute(backend, accelerators):
     c = Circuit(4, accelerators)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     final_state = backend.execute_circuit(c)
     target_state = np.ones(16) / 4.0
     backend.assert_allclose(final_state, target_state)
 
 
 def test_compiled_execute(backend):
-    def create_circuit(theta = 0.1234):
+    def create_circuit(theta=0.1234):
         c = Circuit(2)
         c.add(gates.X(0))
         c.add(gates.X(1))
         c.add(gates.CU1(0, 1, theta))
         return c
 
     # Try to compile circuit without gates
@@ -40,22 +41,24 @@
     """Check that compiling a circuit a second time raises error."""
     c = Circuit(2)
     c.add([gates.H(0), gates.H(1)])
     c.compile()
     with pytest.raises(RuntimeError):
         c.compile()
 
+
 # TODO: Test circuit execution with measurements
 # TODO: Test compiled circuit execution with measurements
 
+
 @pytest.mark.linux
 def test_memory_error(backend, accelerators):
     """Check that ``RuntimeError`` is raised if device runs out of memory."""
     c = Circuit(40, accelerators)
-    c.add((gates.H(i) for i in range(0, 40, 5)))
+    c.add(gates.H(i) for i in range(0, 40, 5))
     with pytest.raises(RuntimeError):
         final_state = backend.execute_circuit(c)
 
 
 def test_repeated_execute(backend, accelerators):
     c = Circuit(4, accelerators)
     thetas = np.random.random(4)
@@ -79,27 +82,27 @@
     backend.execute_circuit(c)
     target_state = np.ones(4) / 2
     backend.assert_allclose(c.final_state, target_state)
 
 
 def test_density_matrix_circuit(backend):
     from qibo.tests.utils import random_density_matrix
+
     theta = 0.1234
     initial_rho = random_density_matrix(3)
 
     c = Circuit(3, density_matrix=True)
     c.add(gates.H(0))
     c.add(gates.H(1))
     c.add(gates.CNOT(0, 1))
     c.add(gates.H(2))
     final_rho = backend.execute_circuit(c, np.copy(initial_rho))
 
     h = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
-    cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0],
-                     [0, 0, 0, 1], [0, 0, 1, 0]])
+    cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
     m1 = np.kron(np.kron(h, h), np.eye(2))
     m2 = np.kron(cnot, np.eye(2))
     m3 = np.kron(np.eye(4), h)
     target_rho = m1.dot(initial_rho).dot(m1.T.conj())
     target_rho = m2.dot(target_rho).dot(m2.T.conj())
     target_rho = m3.dot(target_rho).dot(m3.T.conj())
     backend.assert_allclose(final_rho, target_rho)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_features.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_features.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """Test how features defined in :class:`qibo.models.circuit.Circuit` work during circuit execution."""
 import numpy as np
 import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 
 
 def test_circuit_unitary(backend):
     from qibo import matrices
+
     c = Circuit(2)
     c.add(gates.H(0))
     c.add(gates.H(1))
     c.add(gates.CNOT(0, 1))
     c.add(gates.X(0))
     c.add(gates.Y(1))
     final_matrix = c.unitary(backend)
@@ -18,14 +20,15 @@
     cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
     target_matrix = np.kron(matrices.X, matrices.Y) @ cnot @ np.kron(h, h)
     backend.assert_allclose(final_matrix, target_matrix)
 
 
 def test_circuit_unitary_bigger(backend):
     from qibo import matrices
+
     c = Circuit(4)
     c.add(gates.H(i) for i in range(4))
     c.add(gates.CNOT(0, 1))
     c.add(gates.CZ(1, 2))
     c.add(gates.CNOT(0, 3))
     final_matrix = c.unitary(backend)
     h = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
@@ -115,15 +118,15 @@
     if fuse:
         if accelerators:  # pragma: no cover
             with pytest.raises(NotImplementedError):
                 c = c.fuse()
         else:
             c = c.fuse()
     invc = c.invert()
-    target_state = np.ones(2 ** 4) / 4
+    target_state = np.ones(2**4) / 4
     final_state = backend.execute_circuit(c, initial_state=np.copy(target_state))
     final_state = backend.execute_circuit(invc, initial_state=final_state)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_circuit_invert_and_addition_execution(backend, accelerators):
     subroutine = Circuit(6)
@@ -146,50 +149,50 @@
 
 @pytest.mark.parametrize("distribute_small", [False, True])
 def test_circuit_on_qubits_execution(backend, accelerators, distribute_small):
     if distribute_small:
         smallc = Circuit(3, accelerators=accelerators)
     else:
         smallc = Circuit(3)
-    smallc.add((gates.RX(i, theta=i + 0.1) for i in range(3)))
+    smallc.add(gates.RX(i, theta=i + 0.1) for i in range(3))
     smallc.add((gates.CNOT(0, 1), gates.CZ(1, 2)))
 
     largec = Circuit(6, accelerators=accelerators)
-    largec.add((gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2)))
+    largec.add(gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2))
     largec.add(smallc.on_qubits(1, 3, 5))
 
     targetc = Circuit(6)
-    targetc.add((gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2)))
-    targetc.add((gates.RX(i, theta=i // 2 + 0.1) for i in range(1, 6, 2)))
+    targetc.add(gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2))
+    targetc.add(gates.RX(i, theta=i // 2 + 0.1) for i in range(1, 6, 2))
     targetc.add((gates.CNOT(1, 3), gates.CZ(3, 5)))
     assert largec.depth == targetc.depth
     backend.assert_circuitclose(largec, targetc)
 
 
 @pytest.mark.parametrize("distribute_small", [False, True])
 def test_circuit_on_qubits_double_execution(backend, accelerators, distribute_small):
     if distribute_small:
         smallc = Circuit(3, accelerators=accelerators)
     else:
         smallc = Circuit(3)
-    smallc.add((gates.RX(i, theta=i + 0.1) for i in range(3)))
+    smallc.add(gates.RX(i, theta=i + 0.1) for i in range(3))
     smallc.add((gates.CNOT(0, 1), gates.CZ(1, 2)))
     # execute the small circuit before adding it to the large one
     _ = backend.execute_circuit(smallc)
 
     largec = Circuit(6, accelerators=accelerators)
-    largec.add((gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2)))
+    largec.add(gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2))
     if distribute_small and accelerators is not None:  # pragma: no cover
         with pytest.raises(RuntimeError):
             largec.add(smallc.on_qubits(1, 3, 5))
     else:
         largec.add(smallc.on_qubits(1, 3, 5))
         targetc = Circuit(6)
-        targetc.add((gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2)))
-        targetc.add((gates.RX(i, theta=i // 2 + 0.1) for i in range(1, 6, 2)))
+        targetc.add(gates.RY(i, theta=i + 0.2) for i in range(0, 6, 2))
+        targetc.add(gates.RX(i, theta=i // 2 + 0.1) for i in range(1, 6, 2))
         targetc.add((gates.CNOT(1, 3), gates.CZ(3, 5)))
         assert largec.depth == targetc.depth
         backend.assert_circuitclose(largec, targetc)
 
 
 def test_circuit_on_qubits_controlled_by_execution(backend, accelerators):
     smallc = Circuit(3)
@@ -248,28 +251,27 @@
     backend.assert_circuitclose(largec, targetc)
 
 
 def test_circuit_decompose_execution(backend):
     c = Circuit(6)
     c.add(gates.RX(0, 0.1234))
     c.add(gates.RY(1, 0.4321))
-    c.add((gates.H(i) for i in range(2, 6)))
+    c.add(gates.H(i) for i in range(2, 6))
     c.add(gates.CNOT(0, 1))
     c.add(gates.X(3).controlled_by(0, 1, 2, 4))
     decomp_c = c.decompose(5)
     backend.assert_circuitclose(c, decomp_c, atol=1e-6)
 
 
 def test_repeated_execute_pauli_noise_channel(backend):
     thetas = np.random.random(4)
     backend.set_seed(1234)
     c = Circuit(4)
     c.add((gates.RY(i, t) for i, t in enumerate(thetas)))
-    c.add((gates.PauliNoiseChannel(i, px=0.1, py=0.2, pz=0.3)
-          for i in range(4)))
+    c.add(gates.PauliNoiseChannel(i, px=0.1, py=0.2, pz=0.3) for i in range(4))
     final_state = backend.execute_circuit(c, nshots=20)
 
     backend.set_seed(1234)
     target_state = []
     for _ in range(20):
         noiseless_c = Circuit(4)
         noiseless_c.add((gates.RY(i, t) for i, t in enumerate(thetas)))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_fuse.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_fuse.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 
 
 @pytest.mark.parametrize("nqubits", [2, 3])
 def test_fused_gate_construct_unitary(backend, nqubits):
     gate = gates.FusedGate(0, 1)
@@ -32,41 +33,43 @@
     assert fgate.gates[0] == queue[1]
     assert fgate.gates[1] == queue[0]
     assert fgate.gates[2] == queue[2]
 
 
 def test_two_fusion_gate():
     """Check fusion that creates two ``FusedGate``s."""
-    queue = [gates.X(0), gates.H(1),
-             gates.RX(2, theta=0.1234).controlled_by(1),
-             gates.H(2), gates.Y(1),
-             gates.H(0)]
+    queue = [
+        gates.X(0),
+        gates.H(1),
+        gates.RX(2, theta=0.1234).controlled_by(1),
+        gates.H(2),
+        gates.Y(1),
+        gates.H(0),
+    ]
     c = Circuit(3)
     c.add(queue)
     c = c.fuse()
     assert len(c.queue) == 2
     fgate1, fgate2 = c.queue
     assert fgate2.gates[0] == queue[0]
     assert fgate2.gates[1] == queue[-1]
     assert fgate1.gates == [queue[1], queue[2], queue[4], queue[3]]
 
 
 def test_fusedgate_matrix_calculation(backend):
-    queue = [gates.H(0), gates.H(1), gates.CNOT(0, 1),
-             gates.X(0), gates.X(1)]
+    queue = [gates.H(0), gates.H(1), gates.CNOT(0, 1), gates.X(0), gates.X(1)]
     circuit = Circuit(2)
     circuit.add(queue)
     circuit = circuit.fuse()
     assert len(circuit.queue) == 1
     fused_gate = circuit.queue[0]
 
     x = np.array([[0, 1], [1, 0]])
     h = np.array([[1, 1], [1, -1]]) / np.sqrt(2)
-    cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1],
-                     [0, 0, 1, 0]])
+    cnot = np.array([[1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 0, 1], [0, 0, 1, 0]])
     target_matrix = np.kron(x, x) @ cnot @ np.kron(h, h)
     fused_matrix = fused_gate.asmatrix(backend)
     backend.assert_allclose(fused_matrix, target_matrix)
 
 
 def test_fuse_circuit_two_qubit_gates(backend):
     """Check circuit fusion in circuit with two-qubit gates only."""
@@ -80,20 +83,20 @@
     backend.assert_circuitclose(fused_c, c)
 
 
 @pytest.mark.parametrize("max_qubits", [2, 3, 4])
 def test_fuse_circuit_three_qubit_gate(backend, max_qubits):
     """Check circuit fusion in circuit with three-qubit gate."""
     c = Circuit(4)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     c.add(gates.CZ(0, 1))
     c.add(gates.CZ(2, 3))
     c.add(gates.TOFFOLI(0, 1, 2))
     c.add(gates.SWAP(1, 2))
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     c.add(gates.CNOT(0, 1))
     c.add(gates.CZ(2, 3))
     fused_c = c.fuse(max_qubits=max_qubits)
     backend.assert_circuitclose(fused_c, c, atol=1e-12)
 
 
 @pytest.mark.parametrize("nqubits", [4, 5, 10, 11])
@@ -102,18 +105,18 @@
 def test_variational_layer_fusion(backend, nqubits, nlayers, max_qubits):
     """Check fused variational layer execution."""
     theta = 2 * np.pi * np.random.random((2 * nlayers * nqubits,))
     theta_iter = iter(theta)
 
     c = Circuit(nqubits)
     for _ in range(nlayers):
-        c.add((gates.RY(i, next(theta_iter)) for i in range(nqubits)))
-        c.add((gates.CZ(i, i + 1) for i in range(0, nqubits - 1, 2)))
-        c.add((gates.RY(i, next(theta_iter)) for i in range(nqubits)))
-        c.add((gates.CZ(i, i + 1) for i in range(1, nqubits - 1, 2)))
+        c.add(gates.RY(i, next(theta_iter)) for i in range(nqubits))
+        c.add(gates.CZ(i, i + 1) for i in range(0, nqubits - 1, 2))
+        c.add(gates.RY(i, next(theta_iter)) for i in range(nqubits))
+        c.add(gates.CZ(i, i + 1) for i in range(1, nqubits - 1, 2))
         c.add(gates.CZ(0, nqubits - 1))
 
     fused_c = c.fuse(max_qubits=max_qubits)
     backend.assert_circuitclose(fused_c, c)
 
 
 @pytest.mark.parametrize("nqubits", [4, 5])
@@ -137,27 +140,28 @@
     fused_c = c.fuse(max_qubits=max_qubits)
     backend.assert_circuitclose(fused_c, c, atol=1e-7)
 
 
 def test_controlled_by_gates_fusion(backend):
     """Check circuit fusion that contains ``controlled_by`` gates."""
     c = Circuit(4)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     c.add(gates.RX(1, theta=0.1234).controlled_by(0))
     c.add(gates.RX(3, theta=0.4321).controlled_by(2))
-    c.add((gates.RY(i, theta=0.5678) for i in range(4)))
+    c.add(gates.RY(i, theta=0.5678) for i in range(4))
     c.add(gates.RX(1, theta=0.1234).controlled_by(0))
     c.add(gates.RX(3, theta=0.4321).controlled_by(2))
     fused_c = c.fuse()
     backend.assert_circuitclose(fused_c, c)
 
 
 def test_callbacks_fusion(backend):
     """Check entropy calculation in fused circuit."""
     from qibo import callbacks
+
     entropy = callbacks.EntanglementEntropy([0])
     c = Circuit(5)
     c.add(gates.H(0))
     c.add(gates.X(1))
     c.add(gates.CallbackGate(entropy))
     c.add(gates.CNOT(0, 1))
     c.add(gates.CallbackGate(entropy))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_noise.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Test :class:`qibo.models.circuit.Circuit` for density matrix and noise simulation."""
 import numpy as np
 import pytest
+
 import qibo
 from qibo import gates
 from qibo.models import Circuit
 
 
 def test_pauli_noise_channel(backend):
     from qibo import matrices
+
     c = Circuit(2, density_matrix=True)
     c.add(gates.H(0))
     c.add(gates.H(1))
     c.add(gates.PauliNoiseChannel(0, px=0.5, pz=0.3))
     c.add(gates.PauliNoiseChannel(1, py=0.1, pz=0.3))
     final_rho = backend.execute_circuit(c)
 
@@ -76,16 +78,15 @@
     target_c.add(gates.H(1))
     target_c.add(gates.PauliNoiseChannel(1, 0.1, 0.1, 0.1))
     target_state = backend.execute_circuit(target_c)
     backend.assert_allclose(final_state, target_state)
 
 
 def test_circuit_with_noise_noise_map(backend):
-    noise_map = {0: (0.1, 0.2, 0.1), 1: (0.2, 0.3, 0.0),
-                 2: (0.0, 0.0, 0.0)}
+    noise_map = {0: (0.1, 0.2, 0.1), 1: (0.2, 0.3, 0.0), 2: (0.0, 0.0, 0.0)}
 
     c = Circuit(3, density_matrix=True)
     c.add([gates.H(0), gates.H(1), gates.X(2)])
     c.add(gates.M(2))
     noisy_c = c.with_noise(noise_map)
     final_state = backend.execute_circuit(noisy_c)
 
@@ -114,40 +115,42 @@
         noisy_c = c.with_noise({0: (0.2, 0.3, 0.1)})
     with pytest.raises(TypeError):
         noisy_c = c.with_noise({0, 1})
 
 
 def test_density_matrix_circuit_measurement(backend):
     """Check measurement gate on density matrices using circuit."""
-    from qibo.tests.test_measurements import assert_result, assert_register_result
+    from qibo.tests.test_measurements import assert_register_result, assert_result
+
     state = np.zeros(16)
     state[0] = 1
     init_rho = np.outer(state, state.conj())
 
     c = Circuit(4, density_matrix=True)
     c.add(gates.X(1))
     c.add(gates.X(3))
     c.add(gates.M(0, 1, register_name="A"))
     c.add(gates.M(3, 2, register_name="B"))
     result = backend.execute_circuit(c, init_rho, nshots=100)
 
     target_binary_samples = np.zeros((100, 4))
     target_binary_samples[:, 1] = 1
     target_binary_samples[:, 2] = 1
-    assert_result(backend, result,
-                  decimal_samples=6 * np.ones((100,)),
-                  binary_samples=target_binary_samples,
-                  decimal_frequencies={6: 100},
-                  binary_frequencies={"0110": 100})
+    assert_result(
+        backend,
+        result,
+        decimal_samples=6 * np.ones((100,)),
+        binary_samples=target_binary_samples,
+        decimal_frequencies={6: 100},
+        binary_frequencies={"0110": 100},
+    )
 
     target = {}
-    target["decimal_samples"] = {"A": np.ones((100,)),
-                                 "B": 2 * np.ones((100,))}
-    target["binary_samples"] = {"A": np.zeros((100, 2)),
-                                "B": np.zeros((100, 2))}
+    target["decimal_samples"] = {"A": np.ones((100,)), "B": 2 * np.ones((100,))}
+    target["binary_samples"] = {"A": np.zeros((100, 2)), "B": np.zeros((100, 2))}
     target["binary_samples"]["A"][:, 1] = 1
     target["binary_samples"]["B"][:, 0] = 1
     target["decimal_frequencies"] = {"A": {1: 100}, "B": {2: 100}}
     target["binary_frequencies"] = {"A": {"01": 100}, "B": {"10": 100}}
     assert_register_result(backend, result, **target)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_parametrized.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_parametrized.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Test :meth:`qibo.models.circuit.Circuit.get_parameters` and :meth:`qibo.models.circuit.Circuit.set_parameters`."""
 import numpy as np
 import pytest
+
 import qibo
 from qibo import gates
 from qibo.models import Circuit
 
 
 def test_rx_parameter_setter(backend):
     """Check the parameter setter of RX gate."""
+
     def exact_state(theta):
         phase = np.exp(1j * theta / 2.0)
-        gate = np.array([[phase.real, -1j * phase.imag],
-                        [-1j * phase.imag, phase.real]])
+        gate = np.array(
+            [[phase.real, -1j * phase.imag], [-1j * phase.imag, phase.real]]
+        )
         return gate.dot(np.ones(2)) / np.sqrt(2)
 
     theta = 0.1234
     gate = gates.RX(0, theta=theta)
     initial_state = np.ones(2) / np.sqrt(2)
     final_state = backend.apply_gate(gate, initial_state, 1)
     target_state = exact_state(theta)
@@ -182,23 +185,46 @@
         new_params_list.append(new_params[8])
 
     c.set_parameters(new_params_list)
     fused_c.set_parameters(new_params_list)
     backend.assert_circuitclose(fused_c, c)
 
 
+@pytest.mark.parametrize("trainable", [True, False])
+def test_set_parameters_with_light_cone(backend, trainable):
+    """Check updating parameters of light cone circuit."""
+    params = np.random.random(4)
+    c = Circuit(4)
+    c.add(gates.RX(0, theta=params[0], trainable=trainable))
+    c.add(gates.RY(1, theta=params[1]))
+    c.add(gates.CZ(0, 1))
+    c.add(gates.RX(2, theta=params[2]))
+    c.add(gates.RY(3, theta=params[3], trainable=trainable))
+    c.add(gates.CZ(2, 3))
+    if trainable:
+        c.set_parameters(np.random.random(4))
+    else:
+        c.set_parameters(np.random.random(2))
+    target_state = backend.execute_circuit(c)
+    lc, _ = c.light_cone(1, 2)
+    final_state = backend.execute_circuit(lc)
+    backend.assert_allclose(final_state, target_state)
+
+
 def test_variable_theta():
     """Check that parametrized gates accept `tf.Variable` parameters."""
     try:
         from qibo.backends import construct_backend
+
         backend = construct_backend("tensorflow")
-    except ModuleNotFoundError: # pragma: no cover
+    except ModuleNotFoundError:  # pragma: no cover
         pytest.skip("Skipping variable test because tensorflow is not available.")
 
     import tensorflow as tf
+
     theta1 = tf.Variable(0.1234, dtype="float64")
     theta2 = tf.Variable(0.4321, dtype="float64")
     cvar = Circuit(2)
     cvar.add(gates.RX(0, theta1))
     cvar.add(gates.RY(1, theta2))
     final_state = backend.execute_circuit(cvar)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_qasm.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_qasm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests creating abstract Qibo circuits from OpenQASM code."""
 import pytest
+
 import qibo
 from qibo import __version__, gates
 from qibo.models import Circuit
 
 
 def assert_strings_equal(a, b):
     """Asserts that two strings are identical character by character."""
@@ -29,14 +30,15 @@
 OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
 h q[0];
 h q[1];"""
     assert_strings_equal(c.to_qasm(), target)
 
+
 def test_singlequbit_gates():
     c = Circuit(2)
     c.add(gates.H(0))
     c.add(gates.X(1))
     c.add(gates.Y(0))
     c.add(gates.Z(1))
     c.add(gates.S(0))
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_circuit_qasm_cirq.py` & `qibo-0.1.9/src/qibo/tests/test_models_circuit_qasm_cirq.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Tests executing Qibo circuits created from OpenQASM code."""
-import pytest
-import numpy as np
 import cirq
-from qibo import gates
-from qibo.models import Circuit
+import numpy as np
+import pytest
 from cirq.contrib.qasm_import import circuit_from_qasm, exception
 
+from qibo import gates
+from qibo.models import Circuit
 
 # Absolute testing tolerance for cirq-qibo comparison
 _atol = 1e-7
 
 
 def test_from_qasm_simple(backend, accelerators):
     target = f"""OPENQASM 2.0;
@@ -17,14 +17,15 @@
 qreg q[5];
 h q[0];
 h q[1];
 h q[2];
 h q[3];
 h q[4];"""
     import qibo
+
     c = Circuit.from_qasm(target, accelerators)
     assert c.nqubits == 5
     assert c.depth == 1
     for i, gate in enumerate(c.queue):
         assert gate.__class__.__name__ == "H"
         assert gate.qubits == (i,)
     target_state = np.ones(32) / np.sqrt(32)
@@ -37,15 +38,17 @@
     c1.add(gates.H(0))
     c1.add(gates.H(1))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     assert c3.depth == c2depth
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
@@ -62,15 +65,17 @@
     c1.add(gates.TDG(1))
     c1.add(gates.I(0))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     assert c3.depth == c2depth
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
@@ -83,15 +88,17 @@
     c1.add(gates.SWAP(0, 1))
     c1.add(gates.X(0).controlled_by(1))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     assert c3.depth == c2depth
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
@@ -105,15 +112,17 @@
     c1.add(gates.Z(2))
     c1.add(gates.TOFFOLI(1, 2, 0))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     assert c3.depth == c2depth
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
@@ -123,15 +132,17 @@
     c1.add(gates.Y(0))
     c1.add(gates.RY(1, 0.1234))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
 
@@ -151,15 +162,17 @@
     c1.add(gates.RZ(1, 0.4))
     c1.add(gates.U2(2, 0.5, 0.6))
     final_state_c1 = backend.execute_circuit(c1)
 
     c2 = circuit_from_qasm(c1.to_qasm())
     c2depth = len(cirq.Circuit(c2.all_operations()))
     assert c1.depth == c2depth
-    final_state_c2 = cirq.Simulator().simulate(c2).final_state_vector # pylint: disable=no-member
+    final_state_c2 = (
+        cirq.Simulator().simulate(c2).final_state_vector
+    )  # pylint: disable=no-member
     backend.assert_allclose(final_state_c1, final_state_c2, atol=_atol)
 
     c3 = Circuit.from_qasm(c2.to_qasm())
     assert c3.depth == c2depth
     final_state_c3 = backend.execute_circuit(c3)
     backend.assert_allclose(final_state_c3, final_state_c2, atol=_atol)
 
@@ -182,14 +195,15 @@
     # catches unknown gate "crx"
     with pytest.raises(exception.QasmException):
         c2 = circuit_from_qasm(c1.to_qasm())
 
 
 def test_from_qasm_evaluation(backend):
     import numpy as np
+
     target = f"""OPENQASM 2.0;
 include "qelib1.inc";
 qreg q[2];
 h q[0];
 h q[1];"""
     c = Circuit.from_qasm(target)
     target_state = np.ones(4) / 2.0
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_distcircuit.py` & `qibo-0.1.9/src/qibo/tests/test_models_distcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test functions defined in `qibo/models/distcircuit.py`."""
-import pytest
 import numpy as np
+import pytest
+
 import qibo
 from qibo import gates
 from qibo.models import Circuit
 from qibo.models.distcircuit import DistributedQubits
 
 
 def check_device_queues(queues):
@@ -50,23 +51,23 @@
     # Attempt to access state before being set
     with pytest.raises(RuntimeError):
         final_state = c.final_state
 
 
 def test_distributed_circuit_fusion(accelerators):
     c = Circuit(4, accelerators)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     with pytest.raises(NotImplementedError):
         c.fuse()
 
 
 def test_distributed_circuit_set_gates():
     devices = {"/GPU:0": 2, "/GPU:1": 2}
     c = Circuit(6, devices)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     c.queues.set(c.queue)
 
     check_device_queues(c.queues)
     assert len(c.queues.queues) == 1
     assert len(c.queues.queues[0]) == 4
     for queues in c.queues.queues[0]:
         assert len(queues) == 4
@@ -93,23 +94,24 @@
 
 
 @pytest.mark.parametrize("nqubits", [28, 29, 30, 31, 32, 33, 34])
 @pytest.mark.parametrize("ndevices", [2, 4, 8, 16, 32, 64])
 def test_distributed_qft_global_qubits_validity(nqubits, ndevices):
     """Check that no gates are applied to global qubits for practical QFT cases."""
     from qibo.models import QFT
+
     c = QFT(nqubits, accelerators={"/GPU:0": ndevices})
-    c.queues.set(c.queue) # pylint: disable=E1101
-    check_device_queues(c.queues) # pylint: disable=E1101
+    c.queues.set(c.queue)  # pylint: disable=E1101
+    check_device_queues(c.queues)  # pylint: disable=E1101
 
 
 def test_transform_queue_simple():
     devices = {"/GPU:0": 1, "/GPU:1": 1}
     c = Circuit(4, devices)
-    c.add((gates.H(i) for i in range(4)))
+    c.add(gates.H(i) for i in range(4))
     c.queues.qubits = DistributedQubits([0], c.nqubits)
     tqueue = c.queues.transform(c.queue)
     assert len(tqueue) == 6
     for i in range(3):
         assert isinstance(tqueue[i], gates.H)
         assert tqueue[i].target_qubits == (i + 1,)
     assert isinstance(tqueue[3], gates.SWAP)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_distcircuit_execution.py` & `qibo-0.1.9/src/qibo/tests/test_models_distcircuit_execution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,99 +1,113 @@
 """Test :class:`qibo.models.distcircuit.DistributedCircuit` execution."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 from qibo.tests.utils import random_state
 
 
 @pytest.mark.parametrize("use_global_qubits", [False, True])
-def test_distributed_circuit_execution(backend, accelerators, use_global_qubits):  # pragma: no cover
+def test_distributed_circuit_execution(
+    backend, accelerators, use_global_qubits
+):  # pragma: no cover
     dist_c = Circuit(6, accelerators)
     c = Circuit(6)
     if use_global_qubits:
-        dist_c.add((gates.H(i) for i in range(dist_c.nqubits)))
-        c.add((gates.H(i) for i in range(dist_c.nqubits)))
+        dist_c.add(gates.H(i) for i in range(dist_c.nqubits))
+        c.add(gates.H(i) for i in range(dist_c.nqubits))
     else:
-        dist_c.add((gates.H(i) for i in range(dist_c.nlocal)))
-        c.add((gates.H(i) for i in range(dist_c.nlocal)))
+        dist_c.add(gates.H(i) for i in range(dist_c.nlocal))
+        c.add(gates.H(i) for i in range(dist_c.nlocal))
     dist_c.global_qubits = range(dist_c.nlocal, dist_c.nqubits)
 
     initial_state = random_state(c.nqubits)
     final_state = backend.execute_circuit(dist_c, np.copy(initial_state))
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(target_state, final_state)
 
 
-def test_distributed_circuit_execution_pretransformed(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_pretransformed(
+    backend, accelerators
+):  # pragma: no cover
     dist_c = Circuit(4, accelerators)
-    dist_c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    dist_c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
     dist_c.add(gates.SWAP(0, 2))
-    dist_c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    dist_c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
 
     c = Circuit(4)
-    c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
     c.add(gates.SWAP(0, 2))
-    c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
 
     initial_state = random_state(c.nqubits)
     final_state = backend.execute_circuit(dist_c, np.copy(initial_state))
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(target_state, final_state, atol=1e-7)
 
 
-def test_distributed_circuit_execution_with_swap(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_with_swap(
+    backend, accelerators
+):  # pragma: no cover
     dist_c = Circuit(6, accelerators)
-    dist_c.add((gates.H(i) for i in range(6)))
-    dist_c.add((gates.SWAP(i, i + 1) for i in range(5)))
+    dist_c.add(gates.H(i) for i in range(6))
+    dist_c.add(gates.SWAP(i, i + 1) for i in range(5))
     dist_c.global_qubits = [0, 1]
 
     c = Circuit(6)
-    c.add((gates.H(i) for i in range(6)))
-    c.add((gates.SWAP(i, i + 1) for i in range(5)))
+    c.add(gates.H(i) for i in range(6))
+    c.add(gates.SWAP(i, i + 1) for i in range(5))
 
     initial_state = random_state(c.nqubits)
     final_state = backend.execute_circuit(dist_c, np.copy(initial_state))
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(target_state, final_state, atol=1e-7)
 
 
-def test_distributed_circuit_execution_special_gate(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_special_gate(
+    backend, accelerators
+):  # pragma: no cover
     from qibo import callbacks
+
     dist_c = Circuit(6, accelerators)
     initial_state = random_state(dist_c.nqubits)
     entropy = callbacks.EntanglementEntropy([0])
     dist_c.add(gates.CallbackGate(entropy))
-    dist_c.add((gates.H(i) for i in range(dist_c.nlocal)))
+    dist_c.add(gates.H(i) for i in range(dist_c.nlocal))
     dist_c.add(gates.CallbackGate(entropy))
     dist_c.global_qubits = range(dist_c.nlocal, dist_c.nqubits)
     c = Circuit(6)
     c.add(gates.CallbackGate(entropy))
-    c.add((gates.H(i) for i in range(dist_c.nlocal)))
+    c.add(gates.H(i) for i in range(dist_c.nlocal))
     c.add(gates.CallbackGate(entropy))
     final_state = backend.execute_circuit(dist_c, initial_state=np.copy(initial_state))
     target_state = backend.execute_circuit(c, initial_state=np.copy(initial_state))
     backend.assert_allclose(final_state, target_state, atol=1e-7)
 
 
-def test_distributed_circuit_execution_controlled_gate(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_controlled_gate(
+    backend, accelerators
+):  # pragma: no cover
     dist_c = Circuit(4, accelerators)
-    dist_c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    dist_c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
     dist_c.add(gates.CNOT(0, 2))
     c = Circuit(4)
-    c.add((gates.H(i) for i in range(dist_c.nglobal, 4)))
+    c.add(gates.H(i) for i in range(dist_c.nglobal, 4))
     c.add(gates.CNOT(0, 2))
 
     initial_state = random_state(c.nqubits)
     final_state = backend.execute_circuit(dist_c, np.copy(initial_state))
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(target_state, final_state)
 
 
-def test_distributed_circuit_execution_controlled_by_gates(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_controlled_by_gates(
+    backend, accelerators
+):  # pragma: no cover
     dist_c = Circuit(6, accelerators)
     dist_c.add([gates.H(0), gates.H(2), gates.H(3)])
     dist_c.add(gates.CNOT(4, 5))
     dist_c.add(gates.Z(1).controlled_by(0))
     dist_c.add(gates.SWAP(2, 3))
     dist_c.add([gates.X(2), gates.X(3), gates.X(4)])
 
@@ -106,15 +120,17 @@
 
     initial_state = random_state(c.nqubits)
     final_state = backend.execute_circuit(dist_c, np.copy(initial_state))
     target_state = backend.execute_circuit(c, np.copy(initial_state))
     backend.assert_allclose(target_state, final_state, atol=1e-7)
 
 
-def test_distributed_circuit_execution_addition(backend, accelerators):  # pragma: no cover
+def test_distributed_circuit_execution_addition(
+    backend, accelerators
+):  # pragma: no cover
     # Attempt to add circuits with different devices
     c1 = Circuit(6, {"/GPU:0": 2, "/GPU:1": 2})
     c2 = Circuit(6, {"/GPU:0": 2})
     with pytest.raises(ValueError):
         c = c1 + c2
 
     c1 = Circuit(6, accelerators)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_evolution.py` & `qibo-0.1.9/src/qibo/tests/test_models_evolution.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-import pytest
 import numpy as np
+import pytest
+from scipy.linalg import expm
+
 from qibo import callbacks, hamiltonians, models
 from qibo.config import raise_error
-from scipy.linalg import expm
 
 
 def assert_states_equal(backend, state, target_state, atol=0):
     """Asserts that two state vectors are equal up to a phase."""
     state = backend.to_numpy(state)
     target_state = backend.to_numpy(target_state)
     phase = state[0] / target_state[0]
     backend.assert_allclose(state, phase * target_state, atol=atol)
 
 
 class TimeStepChecker(callbacks.Callback):
     """Callback that checks each evolution time step."""
 
     def __init__(self, target_states, atol=0):
-        super(TimeStepChecker, self).__init__()
+        super().__init__()
         self.target_states = iter(target_states)
         self.atol = atol
 
     def apply(self, backend, state):
         assert_states_equal(backend, state, next(self.target_states), atol=self.atol)
 
-    def apply_density_matrix(self, backend, state): # pragma: no cover
+    def apply_density_matrix(self, backend, state):  # pragma: no cover
         raise_error(NotImplementedError)
 
 
 def test_state_evolution_init(backend):
     ham = hamiltonians.Z(2, backend=backend)
     evolution = models.StateEvolution(ham, dt=1)
     assert evolution.nqubits == 2
@@ -47,16 +48,17 @@
     ham = hamiltonians.Z(2, backend=backend)
     evolution = models.StateEvolution(ham, dt=1)
     # execute without initial state
     with pytest.raises(ValueError):
         final_state = evolution(final_time=1)
 
 
-@pytest.mark.parametrize(("solver", "atol"),
-                         [("exp", 0), ("rk4", 1e-2), ("rk45", 1e-1)])
+@pytest.mark.parametrize(
+    ("solver", "atol"), [("exp", 0), ("rk4", 1e-2), ("rk45", 1e-1)]
+)
 def test_state_evolution_constant_hamiltonian(backend, solver, atol):
     nsteps = 200
     t = np.linspace(0, 1, nsteps + 1)
     phase = np.exp(2j * t)[:, np.newaxis]
     ones = np.ones((nsteps + 1, 2))
     target_psi = np.concatenate([phase, ones, phase.conj()], axis=1)
 
@@ -67,42 +69,46 @@
     final_psi = evolution(final_time=1, initial_state=target_psi[0])
 
 
 @pytest.mark.parametrize("nqubits,dt", [(2, 1e-2)])
 def test_state_evolution_time_dependent_hamiltonian(backend, nqubits, dt):
     ham = lambda t: np.cos(t) * hamiltonians.Z(nqubits, backend=backend)
     # Analytical solution
-    target_psi = [np.ones(2 ** nqubits) / np.sqrt(2 ** nqubits)]
+    target_psi = [np.ones(2**nqubits) / np.sqrt(2**nqubits)]
     for n in range(int(1 / dt)):
         prop = expm(-1j * dt * backend.to_numpy(ham(n * dt).matrix))
         target_psi.append(prop.dot(target_psi[-1]))
 
     checker = TimeStepChecker(target_psi, atol=1e-8)
     evolution = models.StateEvolution(ham, dt=dt, callbacks=[checker])
     final_psi = evolution(final_time=1, initial_state=np.copy(target_psi[0]))
 
 
 @pytest.mark.parametrize("nqubits", [5])
 @pytest.mark.parametrize("solver,dt,atol", [("exp", 1e-1, 1e-2), ("rk45", 1e-2, 1e-1)])
-def test_state_evolution_trotter_hamiltonian(backend, accelerators, nqubits, solver, dt, atol):
+def test_state_evolution_trotter_hamiltonian(
+    backend, accelerators, nqubits, solver, dt, atol
+):
     if accelerators is not None and solver != "exp":  # pragma: no cover
         pytest.skip("Distributed evolution is supported only with exp solver.")
     h = 1.0
 
-    target_psi = [np.ones(2 ** nqubits) / np.sqrt(2 ** nqubits)]
-    ham_matrix = backend.to_numpy(hamiltonians.TFIM(nqubits, h=h, backend=backend).matrix)
+    target_psi = [np.ones(2**nqubits) / np.sqrt(2**nqubits)]
+    ham_matrix = backend.to_numpy(
+        hamiltonians.TFIM(nqubits, h=h, backend=backend).matrix
+    )
     prop = expm(-1j * dt * ham_matrix)
     for n in range(int(1 / dt)):
         target_psi.append(prop.dot(target_psi[-1]))
 
     ham = hamiltonians.TFIM(nqubits, h=h, dense=False, backend=backend)
     checker = TimeStepChecker(target_psi, atol=atol)
-    evolution = models.StateEvolution(ham, dt, solver=solver,
-                                      callbacks=[checker],
-                                      accelerators=accelerators)
+    evolution = models.StateEvolution(
+        ham, dt, solver=solver, callbacks=[checker], accelerators=accelerators
+    )
     final_psi = evolution(final_time=1, initial_state=np.copy(target_psi[0]))
 
     # Change dt
     if solver == "exp":
         evolution = models.StateEvolution(ham, dt / 10, accelerators=accelerators)
         final_psi = evolution(final_time=1, initial_state=np.copy(target_psi[0]))
         assert_states_equal(backend, final_psi, target_psi[-1], atol=atol)
@@ -118,29 +124,30 @@
     with pytest.raises(TypeError):
         adev = models.AdiabaticEvolution(lambda t: h1, h1, s, dt=1e-2)
     # Hamiltonians with different number of qubits
     with pytest.raises(ValueError):
         adev = models.AdiabaticEvolution(h0, h1, s, dt=1e-2)
     # Adiabatic Hamiltonian with bad hamiltonian types
     from qibo.hamiltonians.adiabatic import AdiabaticHamiltonian
+
     with pytest.raises(TypeError):
-        h = AdiabaticHamiltonian("a", "b") # pylint: disable=E0110
+        h = AdiabaticHamiltonian("a", "b")  # pylint: disable=E0110
     # s with three arguments
     h0 = hamiltonians.X(2, backend=backend)
     s = lambda t, a, b: t + a + b
     with pytest.raises(ValueError):
         adev = models.AdiabaticEvolution(h0, h1, s, dt=1e-2)
 
 
 def test_adiabatic_evolution_schedule(backend):
     h0 = hamiltonians.X(3, backend=backend)
     h1 = hamiltonians.TFIM(3, backend=backend)
     adev = models.AdiabaticEvolution(h0, h1, lambda t: t, dt=1e-2)
-    assert adev.schedule(0.2) == 0.2 # pylint: disable=E1102
-    assert adev.schedule(0.8) == 0.8 # pylint: disable=E1102
+    assert adev.schedule(0.2) == 0.2  # pylint: disable=E1102
+    assert adev.schedule(0.8) == 0.8  # pylint: disable=E1102
     # s(0) != 0
     with pytest.raises(ValueError):
         adev = models.AdiabaticEvolution(h0, h1, lambda t: t + 1, dt=1e-2)
     # s(T) != 0
     with pytest.raises(ValueError):
         adev = models.AdiabaticEvolution(h0, h1, lambda t: t / 2, dt=1e-2)
 
@@ -155,41 +162,40 @@
     with pytest.raises(ValueError):
         s = adevp.schedule
 
     adevp.set_parameters([0.5, 1])
 
     target_s = lambda t: 0.5 * np.sqrt(t) + 0.5 * t
     for t in np.random.random(10):
-        assert adevp.schedule(t) == target_s(t) # pylint: disable=E1102
+        assert adevp.schedule(t) == target_s(t)  # pylint: disable=E1102
 
 
 @pytest.mark.parametrize("dense", [False, True])
 def test_adiabatic_evolution_hamiltonian(backend, dense):
     """Test adiabatic evolution hamiltonian as a function of time."""
     h0 = hamiltonians.X(2, dense=dense, backend=backend)
     h1 = hamiltonians.TFIM(2, dense=dense, backend=backend)
     adev = models.AdiabaticEvolution(h0, h1, lambda t: t, dt=1e-2)
     # try accessing hamiltonian before setting it
     with pytest.raises(RuntimeError):
         adev.hamiltonian(0.1)
 
-    m1 = np.array([[0, 1, 1, 0], [1, 0, 0, 1],
-                   [1, 0, 0, 1], [0, 1, 1, 0]])
+    m1 = np.array([[0, 1, 1, 0], [1, 0, 0, 1], [1, 0, 0, 1], [0, 1, 1, 0]])
     m2 = np.diag([2, -2, -2, 2])
-    ham = lambda t, T: - (1 - t / T) * m1 - (t / T) * m2
+    ham = lambda t, T: -(1 - t / T) * m1 - (t / T) * m2
 
     adev.hamiltonian.total_time = 1
     for t in [0, 0.3, 0.7, 1.0]:
         if dense:
             matrix = adev.hamiltonian(t).matrix
         else:
             matrix = adev.hamiltonian(t).dense.matrix
         backend.assert_allclose(matrix, ham(t, 1))
 
-    #try using a different total time
+    # try using a different total time
     adev.hamiltonian.total_time = 2
     for t in [0, 0.3, 0.7, 1.0]:
         if dense:
             matrix = adev.hamiltonian(t).matrix
         else:
             matrix = adev.hamiltonian(t).dense.matrix
         backend.assert_allclose(matrix, ham(t, 2))
@@ -198,18 +204,17 @@
 @pytest.mark.parametrize("dt", [1e-1])
 def test_adiabatic_evolution_execute_exp(backend, dt):
     """Test adiabatic evolution with exponential solver."""
     h0 = hamiltonians.X(2, backend=backend)
     h1 = hamiltonians.TFIM(2, backend=backend)
     adev = models.AdiabaticEvolution(h0, h1, lambda t: t, dt=dt)
 
-    m1 = np.array([[0, 1, 1, 0], [1, 0, 0, 1],
-                   [1, 0, 0, 1], [0, 1, 1, 0]])
+    m1 = np.array([[0, 1, 1, 0], [1, 0, 0, 1], [1, 0, 0, 1], [0, 1, 1, 0]])
     m2 = np.diag([2, -2, -2, 2])
-    ham = lambda t: - (1 - t) * m1 - t * m2
+    ham = lambda t: -(1 - t) * m1 - t * m2
 
     target_psi = np.ones(4) / 2
     nsteps = int(1 / dt)
     for n in range(nsteps):
         target_psi = expm(-1j * dt * ham(n * dt)).dot(target_psi)
     final_psi = adev(final_time=1)
     assert_states_equal(backend, final_psi, target_psi)
@@ -217,26 +222,31 @@
 
 @pytest.mark.parametrize("nqubits,dt", [(4, 1e-1)])
 def test_trotterized_adiabatic_evolution(backend, accelerators, nqubits, dt):
     """Test adiabatic evolution using Trotterization."""
     dense_h0 = hamiltonians.X(nqubits, backend=backend)
     dense_h1 = hamiltonians.TFIM(nqubits, backend=backend)
 
-    target_psi = [np.ones(2 ** nqubits) / np.sqrt(2 ** nqubits)]
+    target_psi = [np.ones(2**nqubits) / np.sqrt(2**nqubits)]
     ham = lambda t: dense_h0 * (1 - t) + dense_h1 * t
     for n in range(int(1 / dt)):
         prop = backend.to_numpy(ham(n * dt).exp(dt))
         target_psi.append(prop.dot(target_psi[-1]))
 
     local_h0 = hamiltonians.X(nqubits, dense=False, backend=backend)
     local_h1 = hamiltonians.TFIM(nqubits, dense=False, backend=backend)
     checker = TimeStepChecker(target_psi, atol=dt)
-    adev = models.AdiabaticEvolution(local_h0, local_h1, lambda t: t, dt,
-                                     callbacks=[checker],
-                                     accelerators=accelerators)
+    adev = models.AdiabaticEvolution(
+        local_h0,
+        local_h1,
+        lambda t: t,
+        dt,
+        callbacks=[checker],
+        accelerators=accelerators,
+    )
     final_psi = adev(final_time=1)
 
 
 @pytest.mark.parametrize("solver", ["rk4", "rk45"])
 @pytest.mark.parametrize("dense", [False, True])
 @pytest.mark.parametrize("dt", [0.1])
 def test_adiabatic_evolution_execute_rk(backend, solver, dense, dt):
@@ -247,16 +257,17 @@
     target_psi = [np.ones(8) / np.sqrt(8)]
     ham = lambda t: h0 * (1 - t) + h1 * t
     for n in range(int(1 / dt)):
         prop = backend.to_numpy(ham(n * dt).exp(dt))
         target_psi.append(prop.dot(target_psi[-1]))
 
     checker = TimeStepChecker(target_psi, atol=dt)
-    adev = models.AdiabaticEvolution(h0, h1, lambda t: t, dt, solver="rk4",
-                                     callbacks=[checker])
+    adev = models.AdiabaticEvolution(
+        h0, h1, lambda t: t, dt, solver="rk4", callbacks=[checker]
+    )
     final_psi = adev(final_time=1, initial_state=np.copy(target_psi[0]))
 
 
 def test_adiabatic_evolution_execute_errors(backend):
     h0 = hamiltonians.X(3, backend=backend)
     h1 = hamiltonians.TFIM(3, backend=backend)
     # Non-zero ``start_time``
@@ -266,23 +277,23 @@
     # execute without specifying variational parameters
     sp = lambda t, p: (1 - p) * np.sqrt(t) + p * t
     adevp = models.AdiabaticEvolution(h0, h1, sp, dt=1e-1)
     with pytest.raises(RuntimeError):
         final_state = adevp(final_time=1)
 
 
-@pytest.mark.parametrize("solver,dt,atol",
-                         [("exp", 1e-1, 1e-10), ("rk45", 1e-2, 1e-2)])
+@pytest.mark.parametrize("solver,dt,atol", [("exp", 1e-1, 1e-10), ("rk45", 1e-2, 1e-2)])
 def test_energy_callback(backend, solver, dt, atol):
     """Test using energy callback in adiabatic evolution."""
     h0 = hamiltonians.X(2, backend=backend)
     h1 = hamiltonians.TFIM(2, backend=backend)
     energy = callbacks.Energy(h1)
-    adev = models.AdiabaticEvolution(h0, h1, lambda t: t, dt=dt,
-                                     callbacks=[energy], solver=solver)
+    adev = models.AdiabaticEvolution(
+        h0, h1, lambda t: t, dt=dt, callbacks=[energy], solver=solver
+    )
     final_psi = adev(final_time=1)
 
     target_psi = np.ones(4) / 2
     calc_energy = lambda psi: psi.conj().dot(backend.to_numpy(h1.matrix).dot(psi))
     target_energies = [calc_energy(target_psi)]
     ham = lambda t: h0 * (1 - t) + h1 * t
     for n in range(int(1 / dt)):
@@ -294,31 +305,36 @@
     target_energies = backend.cast(target_energies)
     final_energies = np.array([backend.to_numpy(x) for x in energy[:]])
     backend.assert_allclose(final_energies, target_energies, atol=atol)
 
 
 test_names = "method,options,messages,dense,filename"
 test_values = [
-    ("BFGS", {'maxiter': 1}, True, True, "adiabatic_bfgs.out"),
-    ("BFGS", {'maxiter': 1}, True, False, "trotter_adiabatic_bfgs.out"),
-    ("sgd", {"nepochs": 5}, False, True, None)
-    ]
+    ("BFGS", {"maxiter": 1}, True, True, "adiabatic_bfgs.out"),
+    ("BFGS", {"maxiter": 1}, True, False, "trotter_adiabatic_bfgs.out"),
+    ("sgd", {"nepochs": 5}, False, True, None),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_scheduling_optimization(backend, method, options, messages, dense, filename):
     """Test optimization of s(t)."""
     from qibo.tests.test_models_variational import assert_regression_fixture
+
     h0 = hamiltonians.X(3, dense=dense, backend=backend)
     h1 = hamiltonians.TFIM(3, dense=dense, backend=backend)
     sp = lambda t, p: (1 - p) * np.sqrt(t) + p * t
     adevp = models.AdiabaticEvolution(h0, h1, sp, dt=1e-1)
 
     if method == "sgd":
         if backend.name != "tensorflow":
             with pytest.raises(RuntimeError):
-                best, params, _ = adevp.minimize([0.5, 1], method=method, options=options,
-                                messages=messages)
+                best, params, _ = adevp.minimize(
+                    [0.5, 1], method=method, options=options, messages=messages
+                )
     else:
-        best, params, _ = adevp.minimize([0.5, 1], method=method, options=options,
-                                        messages=messages)
+        best, params, _ = adevp.minimize(
+            [0.5, 1], method=method, options=options, messages=messages
+        )
 
     if filename is not None:
         assert_regression_fixture(backend, params, filename)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_grover.py` & `qibo-0.1.9/src/qibo/tests/test_models_grover.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Test Grover model defined in `qibo/models/grover.py`."""
 import pytest
+
 from qibo import gates
 from qibo.models import Circuit, Grover
 
 
 def test_grover_init(backend):
     oracle = Circuit(5 + 1)
     oracle.add(gates.X(5).controlled_by(*range(5)))
@@ -11,15 +12,17 @@
     superposition.add([gates.H(i) for i in range(5)])
     grover = Grover(oracle, superposition_circuit=superposition)
     assert grover.oracle == oracle
     assert grover.superposition == superposition
     assert grover.sup_qubits == 5
     assert grover.sup_size == 32
     assert not grover.iterative
-    grover = Grover(oracle, superposition_circuit=superposition, superposition_size=int(2**5))
+    grover = Grover(
+        oracle, superposition_circuit=superposition, superposition_size=int(2**5)
+    )
     assert grover.oracle == oracle
     assert grover.superposition == superposition
     assert grover.sup_qubits == 5
     assert grover.sup_size == 32
     assert not grover.iterative
 
 
@@ -39,27 +42,32 @@
 
 
 def test_grover_initial_state(backend):
     oracle = Circuit(5 + 1)
     oracle.add(gates.X(5).controlled_by(*range(5)))
     initial_state = Circuit(5)
     initial_state.add(gates.X(4))
-    grover = Grover(oracle, superposition_qubits=5, initial_state_circuit=initial_state, number_solutions=1)
+    grover = Grover(
+        oracle,
+        superposition_qubits=5,
+        initial_state_circuit=initial_state,
+        number_solutions=1,
+    )
     assert grover.initial_state_circuit == initial_state
     solution, iterations = grover(logs=True, backend=backend)
     assert solution == ["11111"]
 
 
 def test_grover_target_amplitude(backend):
     oracle = Circuit(5 + 1)
     oracle.add(gates.X(5).controlled_by(*range(5)))
-    grover = Grover(oracle, superposition_qubits=5, target_amplitude = 1/2**(5/2))
+    grover = Grover(oracle, superposition_qubits=5, target_amplitude=1 / 2 ** (5 / 2))
     solution, iterations = grover(logs=True, backend=backend)
     assert len(solution) == 1
-    assert solution == ['11111']
+    assert solution == ["11111"]
 
 
 def test_grover_wrong_solution(backend):
     def check(result):
         for i in result:
             if int(i) != 1:
                 return False
@@ -100,14 +108,16 @@
         for i in result:
             if int(i) != 1:
                 return False
         return True
 
     oracle = Circuit(5 + 1)
     oracle.add(gates.X(5).controlled_by(*range(5)))
-    grover = Grover(oracle, superposition_qubits=5, check=check, number_solutions=num_sol)
+    grover = Grover(
+        oracle, superposition_qubits=5, check=check, number_solutions=num_sol
+    )
     solution, iterations = grover(freq=True, logs=True, backend=backend)
     if num_sol:
         assert solution == ["11111"]
         assert iterations == 4
     else:
         assert solution == "11111"
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_hep.py` & `qibo-0.1.9/src/qibo/tests/test_models_hep.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,109 @@
 """Testing HEP models."""
 import numpy as np
 import pytest
-from qibo.models.hep import qPDF
 
+from qibo.models.hep import qPDF
 
 test_names = "ansatz,layers,nqubits,multi_output,output"
 test_values = [
-    ("Fourier", 3, 1, True,  np.array([[1.214777]])),
-    ("Weighted",5, 1, True,  np.array([[0.506931]])),
-    ("Fourier", 5, 1, True,  np.array([[0.475777]])),
-    ("Weighted",3, 8, True,  np.array([[0.102331, 0.196291, 0.250836, 0.246776, 2.63353, 0.658077, 0.421151, 0.025667]])),
-    ("Fourier", 3, 8, True,  np.array([[1.441044, 15.967666, 4.176307, 21.950216, 4.55334, 1.860604, 33.80421, 25.587542]])),
-    ("Weighted",5, 8, True,  np.array([[0.028491, 0.239515, 0.163759, 0.090604, 1.913209, 0.36426, 0.357044, 0.028548]])),
-    ("Fourier", 5, 8, True,  np.array([[2.473517, 5.402246, 1.073041, 84.60309, 2.271607, 2.877924, 27.200738, 1.657042]])),
-    ("Weighted",3, 1, False, np.array([[0.613767]])),
+    ("Fourier", 3, 1, True, np.array([[1.214777]])),
+    ("Weighted", 5, 1, True, np.array([[0.506931]])),
+    ("Fourier", 5, 1, True, np.array([[0.475777]])),
+    (
+        "Weighted",
+        3,
+        8,
+        True,
+        np.array(
+            [
+                [
+                    0.102331,
+                    0.196291,
+                    0.250836,
+                    0.246776,
+                    2.63353,
+                    0.658077,
+                    0.421151,
+                    0.025667,
+                ]
+            ]
+        ),
+    ),
+    (
+        "Fourier",
+        3,
+        8,
+        True,
+        np.array(
+            [
+                [
+                    1.441044,
+                    15.967666,
+                    4.176307,
+                    21.950216,
+                    4.55334,
+                    1.860604,
+                    33.80421,
+                    25.587542,
+                ]
+            ]
+        ),
+    ),
+    (
+        "Weighted",
+        5,
+        8,
+        True,
+        np.array(
+            [
+                [
+                    0.028491,
+                    0.239515,
+                    0.163759,
+                    0.090604,
+                    1.913209,
+                    0.36426,
+                    0.357044,
+                    0.028548,
+                ]
+            ]
+        ),
+    ),
+    (
+        "Fourier",
+        5,
+        8,
+        True,
+        np.array(
+            [
+                [
+                    2.473517,
+                    5.402246,
+                    1.073041,
+                    84.60309,
+                    2.271607,
+                    2.877924,
+                    27.200738,
+                    1.657042,
+                ]
+            ]
+        ),
+    ),
+    ("Weighted", 3, 1, False, np.array([[0.613767]])),
     ("Fourier", 3, 1, False, np.array([[1.214777]])),
-    ("Weighted",5, 1, False, np.array([[0.506931]])),
+    ("Weighted", 5, 1, False, np.array([[0.506931]])),
     ("Fourier", 5, 1, False, np.array([[0.475777]])),
-    ("Weighted",3, 8, False, np.array([[0.102331]])),
+    ("Weighted", 3, 8, False, np.array([[0.102331]])),
     ("Fourier", 3, 8, False, np.array([[1.441044]])),
-    ("Weighted",5, 8, False, np.array([[0.028491]])),
-    ("Fourier", 5, 8, False, np.array([[2.473517]]))]
+    ("Weighted", 5, 8, False, np.array([[0.028491]])),
+    ("Fourier", 5, 8, False, np.array([[2.473517]])),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_qpdf(backend, ansatz, layers, nqubits, multi_output, output):
     """Performs a qPDF circuit minimization test."""
     model = qPDF(ansatz, layers, nqubits, multi_output, backend=backend)
     np.random.seed(0)
     params = np.random.rand(model.nparams)
     result = model.predict(params, [0.1])
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_qft.py` & `qibo-0.1.9/src/qibo/tests/test_models_qft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Test methods defined in `qibo/models/circuit.py`."""
 import sys
+
 import numpy as np
 import pytest
+
 from qibo import gates, models
 from qibo.tests.utils import random_state
 
 
 def qft_matrix(dimension: int, inverse: bool = False) -> np.ndarray:
     """Creates exact QFT matrix.
 
@@ -28,21 +30,21 @@
 
 
 @pytest.mark.parametrize("nqubits", [4, 10, 100])
 def test_qft_circuit_size(backend, nqubits):
     c = models.QFT(nqubits)
     assert c.nqubits == nqubits
     assert c.depth == 2 * nqubits
-    assert c.ngates == nqubits ** 2 // 2 + nqubits
+    assert c.ngates == nqubits**2 // 2 + nqubits
 
 
 @pytest.mark.parametrize("nqubits", [4, 5])
 def test_qft_matrix(backend, nqubits):
     c = models.QFT(nqubits)
-    dim = 2 ** nqubits
+    dim = 2**nqubits
     target_matrix = qft_matrix(dim)
     backend.assert_allclose(c.unitary(backend), target_matrix)
     c = c.invert()
     target_matrix = qft_matrix(dim, inverse=True)
     backend.assert_allclose(c.unitary(backend), target_matrix)
 
 
@@ -58,11 +60,12 @@
     target_state = exact_qft(backend.to_numpy(initial_state))
     backend.assert_allclose(final_state, target_state)
 
 
 def test_qft_errors(backend):
     """Check that ``_DistributedQFT`` raises error if not sufficient qubits."""
     from qibo.models.qft import _DistributedQFT
+
     with pytest.raises(NotImplementedError):
         c = models.QFT(10, with_swaps=False, accelerators={"/GPU:0": 2})
     with pytest.raises(NotImplementedError):
         c = _DistributedQFT(2, accelerators={"/GPU:0": 4})
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_qgan.py` & `qibo-0.1.9/src/qibo/tests/test_models_qgan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Test style-qGAN model defined in `qibo/models/qgan.py`."""
-import pytest
 import numpy as np
+import pytest
+
 from qibo import gates, models
 
 
 def generate_distribution(samples):
     mean = [0, 0, 0]
     cov = [[0.5, 0.1, 0.25], [0.1, 0.5, 0.1], [0.25, 0.1, 0.5]]
     x, y, z = np.random.multivariate_normal(mean, cov, samples).T / 4.0
-    s1 = np.reshape(x, (samples,1))
-    s2 = np.reshape(y, (samples,1))
-    s3 = np.reshape(z, (samples,1))
+    s1 = np.reshape(x, (samples, 1))
+    s2 = np.reshape(y, (samples, 1))
+    s3 = np.reshape(z, (samples, 1))
     return np.hstack((s1, s2, s3))
 
 
 def test_default_qgan():
     reference_distribution = generate_distribution(10)
     qgan = models.StyleQGAN(latent_dim=2, layers=1)
     qgan.fit(reference_distribution, n_epochs=1, save=False)
@@ -29,24 +30,24 @@
     def set_params(circuit, params, x_input, i):
         """Set the parameters for the quantum generator circuit."""
         p = []
         index = 0
         noise = 0
         for l in range(1):
             for q in range(3):
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%2
-                p.append(params[index]*x_input[noise][i] + params[index+1])
-                index+=2
-                noise=(noise+1)%2
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % 2
+                p.append(params[index] * x_input[noise][i] + params[index + 1])
+                index += 2
+                noise = (noise + 1) % 2
         for q in range(3):
-            p.append(params[index]*x_input[noise][i] + params[index+1])
-            index+=2
-            noise=(noise+1)%2
+            p.append(params[index] * x_input[noise][i] + params[index + 1])
+            index += 2
+            noise = (noise + 1) % 2
         circuit.set_parameters(p)
 
     nqubits = 3
     nlayers = 1
     reference_distribution = generate_distribution(10)
     circuit = models.Circuit(nqubits)
     for l in range(nlayers):
@@ -56,20 +57,18 @@
         for i in range(0, nqubits - 1):
             circuit.add(gates.CZ(i, i + 1))
         circuit.add(gates.CZ(nqubits - 1, 0))
     for q in range(nqubits):
         circuit.add(gates.RY(q, 0))
 
     initial_params = np.random.uniform(-0.15, 0.15, 18)
-    qgan = models.StyleQGAN(
-            latent_dim=2,
-            circuit=circuit,
-            set_parameters=set_params
-        )
-    qgan.fit(reference_distribution, initial_params=initial_params, n_epochs=1, save=False)
+    qgan = models.StyleQGAN(latent_dim=2, circuit=circuit, set_parameters=set_params)
+    qgan.fit(
+        reference_distribution, initial_params=initial_params, n_epochs=1, save=False
+    )
     assert qgan.latent_dim == 2
     assert qgan.batch_samples == 128
     assert qgan.n_epochs == 1
     assert qgan.lr == 0.5
 
 
 def test_qgan_errors():
@@ -91,22 +90,23 @@
     initial_params = np.random.uniform(-0.15, 0.15, 18)
     qgan = models.StyleQGAN(latent_dim=2, layers=2)
     with pytest.raises(ValueError):
         qgan.fit(reference_distribution, initial_params=initial_params, save=False)
 
 
 def test_qgan_custom_discriminator():
-    from tensorflow.keras.models import Sequential  # pylint: disable=E0611,E0401
     from tensorflow.keras.layers import Dense  # pylint: disable=E0611,E0401
+    from tensorflow.keras.models import Sequential  # pylint: disable=E0611,E0401
+
     reference_distribution = generate_distribution(10)
     # use wrong number of qubits so that we capture the error
     nqubits = reference_distribution.shape[1] + 1
     discriminator = Sequential()
     discriminator.add(Dense(200, use_bias=False, input_dim=nqubits))
-    discriminator.add(Dense(1, activation='sigmoid'))
+    discriminator.add(Dense(1, activation="sigmoid"))
     qgan = models.StyleQGAN(latent_dim=2, layers=1, discriminator=discriminator)
     with pytest.raises(ValueError):
         qgan.fit(reference_distribution, n_epochs=1, save=False)
 
 
 def test_qgan_circuit_error():
     reference_distribution = generate_distribution(10)
@@ -121,14 +121,15 @@
         for i in range(0, nqubits - 1):
             circuit.add(gates.CZ(i, i + 1))
         circuit.add(gates.CZ(nqubits - 1, 0))
     for q in range(nqubits):
         circuit.add(gates.RY(q, 0))
 
     initial_params = np.random.uniform(-0.15, 0.15, 18)
-    qgan = models.StyleQGAN(
-            latent_dim=2,
-            circuit=circuit,
-            set_parameters=lambda x: x
-        )
+    qgan = models.StyleQGAN(latent_dim=2, circuit=circuit, set_parameters=lambda x: x)
     with pytest.raises(ValueError):
-        qgan.fit(reference_distribution, initial_params=initial_params, n_epochs=1, save=False)
+        qgan.fit(
+            reference_distribution,
+            initial_params=initial_params,
+            n_epochs=1,
+            save=False,
+        )
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_tsp.py` & `qibo-0.1.9/src/qibo/tests/test_models_tsp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-import pytest
-import numpy as np
 from collections import defaultdict
+
+import numpy as np
+import pytest
+
 from qibo import gates
 from qibo.models import QAOA, Circuit
 from qibo.models.tsp import TSP
 from qibo.tests.test_models_variational import assert_regression_fixture
 
 
 def qaoa_function_of_layer(backend, layer):
-    '''
+    """
     This is a function to study the impact of the number of layers on QAOA, it takes
     in the number of layers and compute the distance of the mode of the histogram obtained
     from QAOA
-    '''
+    """
     num_cities = 3
-    distance_matrix = np.array([[0, 0.9, 0.8],
-                                [0.4, 0, 0.1],
-                                [0, 0.7, 0]])
+    distance_matrix = np.array([[0, 0.9, 0.8], [0.4, 0, 0.1], [0, 0.7, 0]])
     # there are two possible cycles, one with distance 1, one with distance 1.9
     distance_matrix = distance_matrix.round(1)
 
     small_tsp = TSP(distance_matrix, backend=backend)
     initial_state = small_tsp.prepare_initial_state([i for i in range(num_cities)])
     obj_hamil, mixer = small_tsp.hamiltonians()
     qaoa = QAOA(obj_hamil, mixer=mixer)
     initial_state = backend.cast(initial_state, copy=True)
-    best_energy, final_parameters, extra = qaoa.minimize(initial_p=[0.1 for i in range(layer)],
-                                                         initial_state=initial_state, method='BFGS',
-                                                         options={"maxiter": 1})
+    best_energy, final_parameters, extra = qaoa.minimize(
+        initial_p=[0.1 for i in range(layer)],
+        initial_state=initial_state,
+        method="BFGS",
+        options={"maxiter": 1},
+    )
     qaoa.set_parameters(final_parameters)
     return qaoa.execute(initial_state)
 
 
 @pytest.mark.parametrize("nlayers", [4, 6, 8])
 def test_tsp(backend, nlayers):
     final_state = backend.to_numpy(qaoa_function_of_layer(backend, nlayers))
-    assert_regression_fixture(backend, final_state.real, f"tsp_layer{nlayers}_real.out", rtol=1e-3)
-    assert_regression_fixture(backend, final_state.imag, f"tsp_layer{nlayers}_imag.out", rtol=1e-3)
+    assert_regression_fixture(
+        backend, final_state.real, f"tsp_layer{nlayers}_real.out", rtol=1e-3, atol=1e-5
+    )
+    assert_regression_fixture(
+        backend, final_state.imag, f"tsp_layer{nlayers}_imag.out", rtol=1e-3, atol=1e-5
+    )
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_models_variational.py` & `qibo-0.1.9/src/qibo/tests/test_models_variational.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,152 @@
 """
 Testing Variational Quantum Circuits.
 """
-import numpy as np
 import pathlib
+
+import numpy as np
 import pytest
-from qibo import gates, models, hamiltonians
-from qibo.tests.utils import random_state
 from scipy.linalg import expm
 
+from qibo import gates, hamiltonians, models
+from qibo.tests.utils import random_state
+
 REGRESSION_FOLDER = pathlib.Path(__file__).with_name("regressions")
 
 
-def assert_regression_fixture(backend, array, filename, rtol=1e-5):
+def assert_regression_fixture(backend, array, filename, rtol=1e-5, atol=1e-12):
     """Check array matches data inside filename.
 
     Args:
         array: numpy array/
         filename: fixture filename
 
     If filename does not exists, this function
     creates the missing file otherwise it loads
     from file and compare.
     """
+
     def load(filename):
         return np.loadtxt(filename)
 
-    filename = REGRESSION_FOLDER/filename
+    filename = REGRESSION_FOLDER / filename
     try:
         array_fixture = load(filename)
-    except: # pragma: no cover
+    except:  # pragma: no cover
         # case not tested in GitHub workflows because files exist
         np.savetxt(filename, array)
         array_fixture = load(filename)
-    backend.assert_allclose(array, array_fixture, rtol=rtol)
+    backend.assert_allclose(array, array_fixture, rtol=rtol, atol=atol)
 
 
 test_names = "method,options,compile,filename"
-test_values = [("Powell", {'maxiter': 1}, True, 'vqc_powell.out'),
-               ("Powell", {'maxiter': 1}, False, 'vqc_powell.out'),
-               ("BFGS", {'maxiter': 1}, True, 'vqc_bfgs.out'),
-               ("BFGS", {'maxiter': 1}, False, 'vqc_bfgs.out')]
+test_values = [
+    ("Powell", {"maxiter": 1}, True, "vqc_powell.out"),
+    ("Powell", {"maxiter": 1}, False, "vqc_powell.out"),
+    ("BFGS", {"maxiter": 1}, True, "vqc_bfgs.out"),
+    ("BFGS", {"maxiter": 1}, False, "vqc_bfgs.out"),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_vqc(backend, method, options, compile, filename):
     """Performs a variational circuit minimization test."""
     from qibo.optimizers import optimize
+
     def myloss(parameters, circuit, target):
         circuit.set_parameters(parameters)
         state = backend.to_numpy(backend.execute_circuit(circuit).state())
         return 1 - np.abs(np.dot(np.conj(target), state))
 
     nqubits = 6
-    nlayers  = 4
+    nlayers = 4
 
     # Create variational circuit
     c = models.Circuit(nqubits)
     for _ in range(nlayers):
-        c.add((gates.RY(q, theta=0) for q in range(nqubits)))
-        c.add((gates.CZ(q, q+1) for q in range(0, nqubits-1, 2)))
-        c.add((gates.RY(q, theta=0) for q in range(nqubits)))
-        c.add((gates.CZ(q, q+1) for q in range(1, nqubits-2, 2)))
-        c.add(gates.CZ(0, nqubits-1))
-    c.add((gates.RY(q, theta=0) for q in range(nqubits)))
+        c.add(gates.RY(q, theta=0) for q in range(nqubits))
+        c.add(gates.CZ(q, q + 1) for q in range(0, nqubits - 1, 2))
+        c.add(gates.RY(q, theta=0) for q in range(nqubits))
+        c.add(gates.CZ(q, q + 1) for q in range(1, nqubits - 2, 2))
+        c.add(gates.CZ(0, nqubits - 1))
+    c.add(gates.RY(q, theta=0) for q in range(nqubits))
 
     # Optimize starting from a random guess for the variational parameters
     np.random.seed(0)
-    x0 = np.random.uniform(0, 2*np.pi, 2*nqubits*nlayers + nqubits)
+    x0 = np.random.uniform(0, 2 * np.pi, 2 * nqubits * nlayers + nqubits)
     data = np.random.normal(0, 1, size=2**nqubits)
 
     # perform optimization
-    best, params, _ = optimize(myloss, x0, args=(c, data), method=method,
-                            options=options, compile=compile)
+    best, params, _ = optimize(
+        myloss, x0, args=(c, data), method=method, options=options, compile=compile
+    )
     if filename is not None:
         assert_regression_fixture(backend, params, filename)
 
 
 test_names = "method,options,compile,filename"
-test_values = [("Powell", {'maxiter': 1}, True, 'vqe_powell.out'),
-               ("BFGS", {'maxiter': 1}, True, 'vqe_bfgs.out'),
-               ("BFGS", {'maxiter': 1}, False, 'vqe_bfgs.out'),
-               ("parallel_L-BFGS-B", {'maxiter': 1}, True, None),
-               ("parallel_L-BFGS-B", {'maxiter': 1}, False, None),
-               ("cma", {"maxfevals": 2}, False, None),
-               ("sgd", {"nepochs": 5}, False, None),
-               ("sgd", {"nepochs": 5}, True, None)]
+test_values = [
+    ("Powell", {"maxiter": 1}, True, "vqe_powell.out"),
+    ("BFGS", {"maxiter": 1}, True, "vqe_bfgs.out"),
+    ("BFGS", {"maxiter": 1}, False, "vqe_bfgs.out"),
+    ("parallel_L-BFGS-B", {"maxiter": 1}, True, None),
+    ("parallel_L-BFGS-B", {"maxiter": 1}, False, None),
+    ("cma", {"maxfevals": 2}, False, None),
+    ("sgd", {"nepochs": 5}, False, None),
+    ("sgd", {"nepochs": 5}, True, None),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_vqe(backend, method, options, compile, filename):
     """Performs a VQE circuit minimization test."""
     if (method == "sgd" or compile) and backend.name != "tensorflow":
         pytest.skip("Skipping SGD test for unsupported backend.")
     nqubits = 6
-    layers  = 4
+    layers = 4
     circuit = models.Circuit(nqubits)
     for l in range(layers):
         for q in range(nqubits):
             circuit.add(gates.RY(q, theta=1.0))
-        for q in range(0, nqubits-1, 2):
-            circuit.add(gates.CZ(q, q+1))
+        for q in range(0, nqubits - 1, 2):
+            circuit.add(gates.CZ(q, q + 1))
         for q in range(nqubits):
             circuit.add(gates.RY(q, theta=1.0))
-        for q in range(1, nqubits-2, 2):
-            circuit.add(gates.CZ(q, q+1))
-        circuit.add(gates.CZ(0, nqubits-1))
+        for q in range(1, nqubits - 2, 2):
+            circuit.add(gates.CZ(q, q + 1))
+        circuit.add(gates.CZ(0, nqubits - 1))
     for q in range(nqubits):
         circuit.add(gates.RY(q, theta=1.0))
     hamiltonian = hamiltonians.XXZ(nqubits=nqubits, backend=backend)
     np.random.seed(0)
-    initial_parameters = np.random.uniform(0, 2*np.pi, 2*nqubits*layers + nqubits)
+    initial_parameters = np.random.uniform(0, 2 * np.pi, 2 * nqubits * layers + nqubits)
     v = models.VQE(circuit, hamiltonian)
-    best, params, _ = v.minimize(initial_parameters, method=method,
-                                 options=options, compile=compile)
+    best, params, _ = v.minimize(
+        initial_parameters, method=method, options=options, compile=compile
+    )
     if method == "cma":
         # remove `outcmaes` folder
         import shutil
+
         shutil.rmtree("outcmaes")
     if filename is not None:
         assert_regression_fixture(backend, params, filename)
 
 
-@pytest.mark.parametrize("solver,dense",
-                         [("exp", False), ("exp", True),
-                          ("rk4", False),  ("rk4", True),
-                          ("rk45", False), ("rk45", True)])
+@pytest.mark.parametrize(
+    "solver,dense",
+    [
+        ("exp", False),
+        ("exp", True),
+        ("rk4", False),
+        ("rk4", True),
+        ("rk45", False),
+        ("rk45", True),
+    ],
+)
 def test_qaoa_execution(backend, solver, dense, accel=None):
     h = hamiltonians.TFIM(6, h=1.0, dense=dense, backend=backend)
     m = hamiltonians.X(6, dense=dense, backend=backend)
     # Trotter and RK require small p's!
     params = 0.01 * (1 - 2 * np.random.random(4))
     state = random_state(6)
     # set absolute test tolerance according to solver
@@ -153,14 +175,15 @@
 
 def test_qaoa_distributed_execution(backend, accelerators):
     test_qaoa_execution(backend, "exp", False, accelerators)
 
 
 def test_qaoa_callbacks(backend, accelerators):
     from qibo import callbacks
+
     # use ``Y`` Hamiltonian so that there are no errors
     # in the Trotter decomposition
     h = hamiltonians.Y(5, backend=backend)
     energy = callbacks.Energy(h)
     params = 0.1 * np.random.random(4)
     state = random_state(5)
 
@@ -206,19 +229,21 @@
     qaoa = models.QAOA(h)
     with pytest.raises(ValueError):
         qaoa.minimize(np.random.random(5))
 
 
 test_names = "method,options,dense,filename"
 test_values = [
-    ("BFGS", {'maxiter': 1}, True, "qaoa_bfgs.out"),
-    ("BFGS", {'maxiter': 1}, False, "trotter_qaoa_bfgs.out"),
-    ("Powell", {'maxiter': 1}, False, "trotter_qaoa_powell.out"),
-    ("sgd", {"nepochs": 5}, True, None)
-    ]
+    ("BFGS", {"maxiter": 1}, True, "qaoa_bfgs.out"),
+    ("BFGS", {"maxiter": 1}, False, "trotter_qaoa_bfgs.out"),
+    ("Powell", {"maxiter": 1}, False, "trotter_qaoa_powell.out"),
+    ("sgd", {"nepochs": 5}, True, None),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_qaoa_optimization(backend, method, options, dense, filename):
     if method == "sgd" and backend.name != "tensorflow":
         pytest.skip("Skipping SGD test for unsupported backend.")
     h = hamiltonians.XXZ(3, dense=dense, backend=backend)
     qaoa = models.QAOA(h)
     initial_p = [0.05, 0.06, 0.07, 0.08]
@@ -228,16 +253,18 @@
 
 
 test_names = "delta_t,max_layers,tolerance,filename"
 test_values = [
     (0.1, 5, None, "falqon1.out"),
     (0.01, 2, None, "falqon2.out"),
     (0.01, 2, 1e-5, "falqon3.out"),
-    (0.01, 5, 1, "falqon4.out")
-    ]
+    (0.01, 5, 1, "falqon4.out"),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_falqon_optimization(backend, delta_t, max_layers, tolerance, filename):
     h = hamiltonians.XXZ(3, backend=backend)
     falqon = models.FALQON(h)
     best, params, extra = falqon.minimize(delta_t, max_layers, tol=tolerance)
     if filename is not None:
         assert_regression_fixture(backend, params, filename)
@@ -252,45 +279,52 @@
     h = hamiltonians.XXZ(3, backend=backend)
     falqon = models.FALQON(h)
     best, params, extra = falqon.minimize(0.1, 5, callback=callback)
     assert len(extra["callbacks"]) == 5
 
 
 test_names = "method,options,compile,filename"
-test_values = [("BFGS", {'maxiter': 1}, False, 'aavqe_bfgs.out'),
-               ("cma", {"maxfevals": 2}, False, None),
-               ("parallel_L-BFGS-B", {'maxiter': 1}, False, None)]
+test_values = [
+    ("BFGS", {"maxiter": 1}, False, "aavqe_bfgs.out"),
+    ("cma", {"maxfevals": 2}, False, None),
+    ("parallel_L-BFGS-B", {"maxiter": 1}, False, None),
+]
+
+
 @pytest.mark.parametrize(test_names, test_values)
 def test_aavqe(backend, method, options, compile, filename):
     """Performs a AAVQE circuit minimization test."""
     nqubits = 4
-    layers  = 1
+    layers = 1
     circuit = models.Circuit(nqubits)
 
     for l in range(layers):
         for q in range(nqubits):
             circuit.add(gates.RY(q, theta=1.0))
-        for q in range(0, nqubits-1, 2):
-            circuit.add(gates.CZ(q, q+1))
+        for q in range(0, nqubits - 1, 2):
+            circuit.add(gates.CZ(q, q + 1))
         for q in range(nqubits):
             circuit.add(gates.RY(q, theta=1.0))
-        for q in range(1, nqubits-2, 2):
-            circuit.add(gates.CZ(q, q+1))
-        circuit.add(gates.CZ(0, nqubits-1))
+        for q in range(1, nqubits - 2, 2):
+            circuit.add(gates.CZ(q, q + 1))
+        circuit.add(gates.CZ(0, nqubits - 1))
     for q in range(nqubits):
         circuit.add(gates.RY(q, theta=1.0))
 
-    easy_hamiltonian=hamiltonians.X(nqubits, backend=backend)
-    problem_hamiltonian=hamiltonians.XXZ(nqubits, backend=backend)
+    easy_hamiltonian = hamiltonians.X(nqubits, backend=backend)
+    problem_hamiltonian = hamiltonians.XXZ(nqubits, backend=backend)
     s = lambda t: t
-    aavqe = models.AAVQE(circuit, easy_hamiltonian, problem_hamiltonian,
-                        s, nsteps=10, t_max=1)
+    aavqe = models.AAVQE(
+        circuit, easy_hamiltonian, problem_hamiltonian, s, nsteps=10, t_max=1
+    )
     np.random.seed(0)
-    initial_parameters = np.random.uniform(0, 2*np.pi, 2*nqubits*layers + nqubits)
-    best, params = aavqe.minimize(params=initial_parameters, method=method,
-                                 options=options, compile=compile)
+    initial_parameters = np.random.uniform(0, 2 * np.pi, 2 * nqubits * layers + nqubits)
+    best, params = aavqe.minimize(
+        params=initial_parameters, method=method, options=options, compile=compile
+    )
     if method == "cma":
         # remove `outcmaes` folder
         import shutil
+
         shutil.rmtree("outcmaes")
     if filename is not None:
         assert_regression_fixture(backend, params, filename, rtol=1e-2)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_noise.py` & `qibo-0.1.9/src/qibo/tests/test_noise.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,101 @@
 import numpy as np
 import pytest
+
 from qibo import gates
 from qibo.models import Circuit
 from qibo.noise import *
 from qibo.tests.utils import random_density_matrix, random_state
 
 
 @pytest.mark.parametrize("density_matrix", [False, True])
 @pytest.mark.parametrize("nshots", [None, 10, 100])
 def test_pauli_error(backend, density_matrix, nshots):
     pauli = PauliError(0, 0.2, 0.3)
     noise = NoiseModel()
     noise.add(pauli, gates.X, 1)
     noise.add(pauli, gates.CNOT)
-    noise.add(pauli, gates.Z, (0,1))
+    noise.add(pauli, gates.Z, (0, 1))
 
     circuit = Circuit(3, density_matrix=density_matrix)
-    circuit.add(gates.CNOT(0,1))
+    circuit.add(gates.CNOT(0, 1))
     circuit.add(gates.Z(1))
     circuit.add(gates.X(1))
     circuit.add(gates.X(2))
     circuit.add(gates.Z(2))
     circuit.add(gates.M(0, 1, 2))
 
     target_circuit = Circuit(3, density_matrix=density_matrix)
-    target_circuit.add(gates.CNOT(0,1))
+    target_circuit.add(gates.CNOT(0, 1))
     target_circuit.add(gates.PauliNoiseChannel(0, 0, 0.2, 0.3))
     target_circuit.add(gates.PauliNoiseChannel(1, 0, 0.2, 0.3))
     target_circuit.add(gates.Z(1))
     target_circuit.add(gates.PauliNoiseChannel(1, 0, 0.2, 0.3))
     target_circuit.add(gates.X(1))
     target_circuit.add(gates.PauliNoiseChannel(1, 0, 0.2, 0.3))
     target_circuit.add(gates.X(2))
     target_circuit.add(gates.Z(2))
     target_circuit.add(gates.M(0, 1, 2))
 
     initial_psi = random_density_matrix(3) if density_matrix else random_state(3)
     backend.set_seed(123)
-    final_state = backend.execute_circuit(noise.apply(circuit), initial_state=np.copy(initial_psi), nshots=nshots)
+    final_state = backend.execute_circuit(
+        noise.apply(circuit), initial_state=np.copy(initial_psi), nshots=nshots
+    )
+    final_state_samples = final_state.samples() if nshots else None
+    backend.set_seed(123)
+    target_final_state = backend.execute_circuit(
+        target_circuit, initial_state=np.copy(initial_psi), nshots=nshots
+    )
+    target_final_state_samples = target_final_state.samples() if nshots else None
+
+    if nshots is None:
+        backend.assert_allclose(final_state, target_final_state)
+    else:
+        backend.assert_allclose(final_state_samples, target_final_state_samples)
+
+
+@pytest.mark.parametrize("density_matrix", [False, True])
+@pytest.mark.parametrize("nshots", [None, 10, 100])
+def test_depolarizing_error(backend, density_matrix, nshots):
+    depol = DepolarizingError(0.3)
+    noise = NoiseModel()
+    noise.add(depol, gates.X, 1)
+    noise.add(depol, gates.CNOT)
+    noise.add(depol, gates.Z, (0, 1))
+
+    circuit = Circuit(3, density_matrix=density_matrix)
+    circuit.add(gates.CNOT(0, 1))
+    circuit.add(gates.Z(1))
+    circuit.add(gates.X(1))
+    circuit.add(gates.X(2))
+    circuit.add(gates.Z(2))
+    circuit.add(gates.M(0, 1, 2))
+
+    target_circuit = Circuit(3, density_matrix=density_matrix)
+    target_circuit.add(gates.CNOT(0, 1))
+    target_circuit.add(gates.DepolarizingChannel((0, 1), 0.3))
+    target_circuit.add(gates.Z(1))
+    target_circuit.add(gates.DepolarizingChannel((1,), 0.3))
+    target_circuit.add(gates.X(1))
+    target_circuit.add(gates.DepolarizingChannel((1,), 0.3))
+    target_circuit.add(gates.X(2))
+    target_circuit.add(gates.Z(2))
+    target_circuit.add(gates.M(0, 1, 2))
+
+    initial_psi = random_density_matrix(3) if density_matrix else random_state(3)
+    backend.set_seed(123)
+    final_state = backend.execute_circuit(
+        noise.apply(circuit), initial_state=np.copy(initial_psi), nshots=nshots
+    )
     final_state_samples = final_state.samples() if nshots else None
     backend.set_seed(123)
-    target_final_state = backend.execute_circuit(target_circuit, initial_state=np.copy(initial_psi), nshots=nshots)
+    target_final_state = backend.execute_circuit(
+        target_circuit, initial_state=np.copy(initial_psi), nshots=nshots
+    )
     target_final_state_samples = target_final_state.samples() if nshots else None
 
     if nshots is None:
         backend.assert_allclose(final_state, target_final_state)
     else:
         backend.assert_allclose(final_state_samples, target_final_state_samples)
 
@@ -53,25 +104,25 @@
 def test_thermal_error(backend, density_matrix):
     if not density_matrix:
         pytest.skip("Reset error is not implemented for state vectors.")
     thermal = ThermalRelaxationError(2, 1, 0.3)
     noise = NoiseModel()
     noise.add(thermal, gates.X, 1)
     noise.add(thermal, gates.CNOT)
-    noise.add(thermal, gates.Z, (0,1))
+    noise.add(thermal, gates.Z, (0, 1))
 
     circuit = Circuit(3, density_matrix=density_matrix)
-    circuit.add(gates.CNOT(0,1))
+    circuit.add(gates.CNOT(0, 1))
     circuit.add(gates.Z(1))
     circuit.add(gates.X(1))
     circuit.add(gates.X(2))
     circuit.add(gates.Z(2))
 
     target_circuit = Circuit(3, density_matrix=density_matrix)
-    target_circuit.add(gates.CNOT(0,1))
+    target_circuit.add(gates.CNOT(0, 1))
     target_circuit.add(gates.ThermalRelaxationChannel(0, 2, 1, 0.3))
     target_circuit.add(gates.ThermalRelaxationChannel(1, 2, 1, 0.3))
     target_circuit.add(gates.Z(1))
     target_circuit.add(gates.ThermalRelaxationChannel(1, 2, 1, 0.3))
     target_circuit.add(gates.X(1))
     target_circuit.add(gates.ThermalRelaxationChannel(1, 2, 1, 0.3))
     target_circuit.add(gates.X(2))
@@ -90,22 +141,22 @@
 def test_reset_error(backend, density_matrix):
     if not density_matrix:
         pytest.skip("Reset error is not implemented for state vectors.")
     reset = ResetError(0.8, 0.2)
     noise = NoiseModel()
     noise.add(reset, gates.X, 1)
     noise.add(reset, gates.CNOT)
-    noise.add(reset, gates.Z, (0,1))
+    noise.add(reset, gates.Z, (0, 1))
 
     circuit = Circuit(3, density_matrix=density_matrix)
-    circuit.add(gates.CNOT(0,1))
+    circuit.add(gates.CNOT(0, 1))
     circuit.add(gates.Z(1))
 
     target_circuit = Circuit(3, density_matrix=density_matrix)
-    target_circuit.add(gates.CNOT(0,1))
+    target_circuit.add(gates.CNOT(0, 1))
     target_circuit.add(gates.ResetChannel(0, 0.8, 0.2))
     target_circuit.add(gates.ResetChannel(1, 0.8, 0.2))
     target_circuit.add(gates.Z(1))
     target_circuit.add(gates.ResetChannel(1, 0.8, 0.2))
 
     initial_psi = random_density_matrix(3) if density_matrix else random_state(3)
     backend.set_seed(123)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_parallel.py` & `qibo-0.1.9/src/qibo/tests/test_parallel.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Testing parallel evaluations.
 """
 import sys
+
 import numpy as np
 import pytest
+
 import qibo
 from qibo import gates
-from qibo.models import Circuit, QFT
-from qibo.parallel import parallel_parametrized_execution, parallel_execution
+from qibo.models import QFT, Circuit
+from qibo.parallel import parallel_execution, parallel_parametrized_execution
 
 
+@pytest.mark.skipif(sys.platform == "darwin", reason="Mac tests")
 def test_parallel_circuit_evaluation(backend):
     """Evaluate circuit for multiple input states."""
     nqubits = 10
     np.random.seed(0)
     c = QFT(nqubits)
 
     states = [np.random.random(2**nqubits) for i in range(5)]
@@ -24,34 +27,37 @@
 
     r2 = parallel_execution(c, states=states, processes=2, backend=backend)
     r1 = [x.state(numpy=True) for x in r1]
     r2 = [x.state(numpy=True) for x in r2]
     backend.assert_allclose(r1, r2)
 
 
+@pytest.mark.skipif(sys.platform == "darwin", reason="Mac tests")
 def test_parallel_parametrized_circuit(backend):
     """Evaluate circuit for multiple parameters."""
     nqubits = 5
-    nlayers  = 10
+    nlayers = 10
     c = Circuit(nqubits)
     for l in range(nlayers):
-        c.add((gates.RY(q, theta=0) for q in range(nqubits)))
-        c.add((gates.CZ(q, q+1) for q in range(0, nqubits-1, 2)))
-        c.add((gates.RY(q, theta=0) for q in range(nqubits)))
-        c.add((gates.CZ(q, q+1) for q in range(1, nqubits-2, 2)))
-        c.add(gates.CZ(0, nqubits-1))
-    c.add((gates.RY(q, theta=0) for q in range(nqubits)))
+        c.add(gates.RY(q, theta=0) for q in range(nqubits))
+        c.add(gates.CZ(q, q + 1) for q in range(0, nqubits - 1, 2))
+        c.add(gates.RY(q, theta=0) for q in range(nqubits))
+        c.add(gates.CZ(q, q + 1) for q in range(1, nqubits - 2, 2))
+        c.add(gates.CZ(0, nqubits - 1))
+    c.add(gates.RY(q, theta=0) for q in range(nqubits))
 
     size = len(c.get_parameters())
     np.random.seed(0)
-    parameters = [np.random.uniform(0, 2*np.pi, size) for i in range(10)]
+    parameters = [np.random.uniform(0, 2 * np.pi, size) for i in range(10)]
     state = np.random.random(2**nqubits)
 
     r1 = []
     for params in parameters:
         c.set_parameters(params)
         r1.append(backend.execute_circuit(c, backend.cast(state)))
 
-    r2 = parallel_parametrized_execution(c, parameters=parameters, initial_state=state, processes=2, backend=backend)
+    r2 = parallel_parametrized_execution(
+        c, parameters=parameters, initial_state=state, processes=2, backend=backend
+    )
     r1 = [x.state(numpy=True) for x in r1]
     r2 = [x.state(numpy=True) for x in r2]
     backend.assert_allclose(r1, r2)
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/test_prints.py` & `qibo-0.1.9/src/qibo/tests/test_prints.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Test that the source contains no prints."""
 import os
-import pytest
 import pathlib
+
+import pytest
+
 from qibo.config import raise_error
 
+
 class CodeText:
     """Helper class to iterate through code text skipping the docstrings."""
 
     def __init__(self, code, filedir=None):
         self.code = code
         self.filedir = filedir
         self.line_counter = 0
         self.piece_counter = 0
         self.pieces = None
 
     @classmethod
     def from_file(cls, filedir):
         assert filedir[-3:] == ".py"
-        with open(filedir, "r", encoding="utf-8") as file:
+        with open(filedir, encoding="utf-8") as file:
             code = file.read()
         return cls(code, filedir)
 
     def __iter__(self):
         self.line_counter = 0
         self.piece_counter = -1
         self.pieces = self.code.split('"""')
@@ -52,48 +55,55 @@
         Args:
             target_word(str): word to be searched in the code text
         """
         for piece in self:
             for offset, line in enumerate(piece.split("\n")):
                 if ("print" in line) and ("CodeText:skip" not in line):
                     line_num = self.line_counter + offset + 1
-                    raise_error(ValueError, f"Found `{target_word}` in line {line_num} "
-                                            f"of {self.filedir}.")
+                    raise_error(
+                        ValueError,
+                        f"Found `{target_word}` in line {line_num} "
+                        f"of {self.filedir}.",
+                    )
 
 
 def python_files():
     """Iterator that yields all python files (`.py`) in `/src/qibo/`."""
     basedir = pathlib.Path(os.path.realpath(__file__)).parent.parent
     for subdir, _, files in os.walk(basedir):
         for file in files:
             pieces = file.split(".")
             # skip non-`.py` files
             # skip current file because it contains `print`
             if len(pieces) == 2 and pieces[1] == "py" and pieces[0] != "test_prints":
                 yield os.path.join(subdir, file)
 
+
 # Make sure the CodeText class works as intended
 text_examples = [
     ('print("Test")', True),
     ('print("Test")\n""" docstring """', True),
     ('""" docstring """\nprint("Test")\n""" docstring """', True),
-    ('pass', False),
+    ("pass", False),
     ('pass\n""" docstring with print """', False),
     ('""" docstring with print """\npass\n""" docstring with print """', False),
-    ('pass # CodeText:skip', False),
+    ("pass # CodeText:skip", False),
     ('print("Test") # CodeText:skip', False),
     ('print("Test")\nprint("Test) # CodeText:skip', True),
-    ('print("Test") # CodeText:skip\nprint("Test)', True)
+    ('print("Test") # CodeText:skip\nprint("Test)', True),
 ]
+
+
 @pytest.mark.parametrize(("text", "contains_print"), text_examples)
 def test_codetext_class(text, contains_print):
     """Check if the CodeText class is working properly"""
     if contains_print:
         with pytest.raises(ValueError):
             CodeText(text).check_exists("print")
     else:
         CodeText(text).check_exists("print")
 
+
 @pytest.mark.parametrize("filename", python_files())
 def test_qibo_code(filename):
     text = CodeText.from_file(filename)
     text.check_exists("print")
```

### Comparing `qibo-0.1.8rc0/src/qibo/tests/utils.py` & `qibo-0.1.9/src/qibo/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,30 +6,30 @@
     x = np.random.random(shape) + 1j * np.random.random(shape)
     if dtype is None:
         return x
     return x.astype(dtype)
 
 
 def random_hermitian(nqubits):
-    shape = 2 * (2 ** nqubits,)
+    shape = 2 * (2**nqubits,)
     m = random_complex(shape)
     return m + m.T.conj()
 
 
 def random_state(nqubits):
     """Generates a random normalized state vector as numpy array."""
-    initial_state = random_complex(2 ** nqubits)
+    initial_state = random_complex(2**nqubits)
     return initial_state / np.sqrt((np.abs(initial_state) ** 2).sum())
 
 
 def random_density_matrix(nqubits):
     """Generates a random normalized density matrix."""
     rho = random_hermitian(nqubits)
     # Normalize
-    ids = np.arange(2 ** nqubits)
+    ids = np.arange(2**nqubits)
     rho[ids, ids] = rho[ids, ids] / np.trace(rho)
     return rho
 
 
 def random_sparse_matrix(backend, n, sparse_type=None):
     if backend.name == "tensorflow":
         nonzero = int(0.1 * n * n)
```

### Comparing `qibo-0.1.8rc0/src/qibo.egg-info/PKG-INFO` & `qibo-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibo
-Version: 0.1.8rc0
+Version: 0.1.9
 Summary: A framework for quantum computing with hardware acceleration.
 Home-page: https://github.com/qiboteam/qibo
 Author: The Qibo team
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -71,8 +71,23 @@
 
 In both cases, the simulation will run in a single device CPU or GPU in double precision `complex128`.
 
 ## Citation policy
 
 If you use the package please refer to [the documentation](https://qibo.readthedocs.io/en/stable/appendix/citing-qibo.html) for citation instructions.
 
+## Supporters and collaborators
+
+- Quantum Research Center, Technology Innovation Institute (TII), United Arab Emirates
+- Università degli Studi di Milano (UNIMI), Italy.
+- Istituto Nazionale di Fisica Nucleare (INFN), Italy.
+- European Organization for Nuclear research (CERN), Switzerland.
+- Universitat de Barcelona (UB), Spain.
+- Barcelona Supercomputing Center (BSC), Spain.
+- Qilimanjaro Quantum Tech, Spain.
+- Centre for Quantum Technologies (CQT), Singapore.
+- Institute of High Performance Computing (IHPC), Singapore.
+- National Supercomputing Centre (NSCC), Singapore.
+- RIKEN Center for Computational Science (R-CCS), Japan.
+- NVIDIA (cuQuantum), USA.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qibo-0.1.8rc0/src/qibo.egg-info/SOURCES.txt` & `qibo-0.1.9/src/qibo.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 src/qibo.egg-info/dependency_links.txt
 src/qibo.egg-info/not-zip-safe
 src/qibo.egg-info/requires.txt
 src/qibo.egg-info/top_level.txt
 src/qibo/backends/__init__.py
 src/qibo/backends/abstract.py
 src/qibo/backends/einsum_utils.py
-src/qibo/backends/matrices.py
+src/qibo/backends/npmatrices.py
 src/qibo/backends/numpy.py
 src/qibo/backends/tensorflow.py
 src/qibo/gates/__init__.py
 src/qibo/gates/abstract.py
 src/qibo/gates/channels.py
 src/qibo/gates/gates.py
 src/qibo/gates/measurements.py
@@ -40,14 +40,17 @@
 src/qibo/models/evolution.py
 src/qibo/models/grover.py
 src/qibo/models/hep.py
 src/qibo/models/qft.py
 src/qibo/models/qgan.py
 src/qibo/models/tsp.py
 src/qibo/models/variational.py
+src/qibo/quantum_info/__init__.py
+src/qibo/quantum_info/metrics.py
+src/qibo/quantum_info/utils.py
 src/qibo/tests/__init__.py
 src/qibo/tests/conftest.py
 src/qibo/tests/test_backends.py
 src/qibo/tests/test_callbacks.py
 src/qibo/tests/test_cirq.py
 src/qibo/tests/test_dill.py
 src/qibo/tests/test_gates_abstract.py
@@ -82,10 +85,11 @@
 src/qibo/tests/test_models_qft.py
 src/qibo/tests/test_models_qgan.py
 src/qibo/tests/test_models_tsp.py
 src/qibo/tests/test_models_variational.py
 src/qibo/tests/test_noise.py
 src/qibo/tests/test_parallel.py
 src/qibo/tests/test_prints.py
+src/qibo/tests/test_quantum_info.py
 src/qibo/tests/test_states.py
 src/qibo/tests/utils.py
 src/qibo/tests/regressions/__init__.py
```

