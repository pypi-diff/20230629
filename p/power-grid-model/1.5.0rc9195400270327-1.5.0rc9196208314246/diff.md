# Comparing `tmp/power-grid-model-1.5.0rc9195400270327.tar.gz` & `tmp/power-grid-model-1.5.0rc9196208314246.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-grid-model-1.5.0rc9195400270327.tar", last modified: Wed Jun 28 13:36:31 2023, max compression
+gzip compressed data, was "power-grid-model-1.5.0rc9196208314246.tar", last modified: Wed Jun 28 15:29:38 2023, max compression
```

## Comparing `power-grid-model-1.5.0rc9195400270327.tar` & `power-grid-model-1.5.0rc9196208314246.tar`

### file list

```diff
@@ -1,620 +1,621 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.174387 power-grid-model-1.5.0rc9195400270327/
--rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-28 13:36:31.170387 power-grid-model-1.5.0rc9195400270327/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-28 13:35:44.000000 power-grid-model-1.5.0rc9195400270327/PYPI_VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.094386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.102386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.102386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.102386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/include/
--rw-r--r--   0 runner    (1001) docker     (123)    26155 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 13:36:31.174387 power-grid-model-1.5.0rc9195400270327/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.094386 power-grid-model-1.5.0rc9195400270327/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/index_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    17761 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.110386 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.106386 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-28 13:36:31.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    37053 2023-06-28 13:36:31.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 13:36:31.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 13:36:31.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 13:36:31.000000 power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.110386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.110386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.110386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.114386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.114386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.114386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.114386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.118386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.118386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.118386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.122387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/gaia_grid.gnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.122387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.094386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.094386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.122387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.126387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.126387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.126387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.130387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.130387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.130387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.130387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.134387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.134387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.134387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.134387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.138387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.138387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.138387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.138387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.142387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.142387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.142387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.142387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.146387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.146387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.146387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.146387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/
--rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.150387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/vision_grid.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/vision_grid.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.150387 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/
--rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/sym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.150387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.154387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60980 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.154387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.154387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.154387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.158387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58820 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.158387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.158387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60848 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.162387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60752 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.162387 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.098386 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.162387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.162387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.166387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/sym_output_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/update_batch.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/update_batch.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.166387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.166387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.166387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/residual-test/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.166387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.170387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.170387 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/asym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/asym_output.json.license
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/input.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/input.json.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/params.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/params.json.license
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/sym_output.json
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/sym_output.json.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.170387 power-grid-model-1.5.0rc9195400270327/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/test_0Z_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/test_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/test_power_grid_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 13:36:31.170387 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_batch_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_input_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-28 13:35:41.000000 power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_validation_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.166651 power-grid-model-1.5.0rc9196208314246/
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-28 15:29:38.166651 power-grid-model-1.5.0rc9196208314246/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-28 15:28:59.000000 power-grid-model-1.5.0rc9196208314246/PYPI_VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.078643 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.078643 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28563 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10354 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20067 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15128 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    67948 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41694 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16064 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11399 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    30818 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    26155 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 15:29:38.166651 power-grid-model-1.5.0rc9196208314246/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.086644 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/index_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17455 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21645 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.086644 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30704 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28618 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.082644 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-06-28 15:29:38.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    37096 2023-06-28 15:29:38.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 15:29:38.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-28 15:29:38.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-28 15:29:38.000000 power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.086644 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.086644 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.090644 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.090644 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.090644 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.094645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.094645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.098645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.098645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.098645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.098645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/gaia_grid.gnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/gaia_grid.gnf.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.102645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.102645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.102645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.102645 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.106646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.106646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.106646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.106646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.110646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.110646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17633 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.110646 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/basic-node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.114647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.114647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.114647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.114647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.118647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.118647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.118647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.122647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.070643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.122647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.122647 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10605 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/params.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.126648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     8702 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.126648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.126648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.126648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/asym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/asym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7374 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.130648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/vision_grid.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/vision_grid.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.130648 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/
+-rw-r--r--   0 runner    (1001) docker     (123)    20486 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/sym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    35119 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.130648 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60794 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.134648 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60980 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.134648 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60938 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.134648 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58916 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.138649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    59750 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.138649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58820 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.138649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    58892 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.142649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60848 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.142649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60752 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.142649 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    60554 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.074643 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.142649 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.146649 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.146649 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    19468 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/sym_output_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/sym_output_batch.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/update_batch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/update_batch.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.150650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.150650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.150650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/residual-test/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.150650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.154650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.154650 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29158 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/asym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/asym_output.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/input.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/input.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/params.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/params.json.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/sym_output.json
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/sym_output.json.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.158650 power-grid-model-1.5.0rc9196208314246/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/test_0Z_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/test_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/test_power_grid_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20807 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 15:29:38.158650 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_batch_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_input_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-28 15:28:56.000000 power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_validation_functions.py
```

### Comparing `power-grid-model-1.5.0rc9195400270327/LICENSE` & `power-grid-model-1.5.0rc9196208314246/LICENSE`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/PKG-INFO` & `power-grid-model-1.5.0rc9196208314246/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9195400270327
+Version: 1.5.0rc9196208314246
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9195400270327/README.md` & `power-grid-model-1.5.0rc9196208314246/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/CMakeLists.txt` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/all_components.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/dataset.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/input.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/meta_data_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/output.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/auxiliary/update.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/calculation_parameters.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/appliance.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/base.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/branch3.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/fault.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/line.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/link.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/load_gen.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/node.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/power_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/shunt.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/source.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/three_winding_transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/transformer_utils.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/component/voltage_sensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/container.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/enum.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/exception.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/main_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_current_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_linear_se_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/iterative_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/linear_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/math_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/newton_raphson_pf_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/sparse_lu_solver.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/math_solver/y_bus.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/power_grid_model.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/sparse_mapping.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/three_phase_tensor.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/timer.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model/include/power_grid_model/topology.hpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/CMakeLists.txt` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/include/power_grid_model_c.h`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp` & `power-grid-model-1.5.0rc9196208314246/power_grid_model_c/power_grid_model_c/power_grid_model_c.cpp`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/pyproject.toml` & `power-grid-model-1.5.0rc9196208314246/pyproject.toml`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/setup.py` & `power-grid-model-1.5.0rc9196208314246/setup.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/options.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     _opt: OptionsPtr
     # option setter
     calculation_type = OptionSetter(pgc.set_calculation_type)
     calculation_method = OptionSetter(pgc.set_calculation_method)
     symmetric = OptionSetter(pgc.set_symmetric)
     error_tolerance = OptionSetter(pgc.set_err_tol)
-    max_iteration = OptionSetter(pgc.set_max_iter)
+    max_iterations = OptionSetter(pgc.set_max_iter)
     threading = OptionSetter(pgc.set_threading)
 
     @property
     def opt(self) -> OptionsPtr:
         """
 
         Returns: Pointer to the option object
```

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_core.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_core.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_meta.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_meta.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/core/power_grid_model.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/core/power_grid_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,33 @@
 #
 # SPDX-License-Identifier: MPL-2.0
 
 
 """
 Main power grid model class
 """
+from enum import IntEnum
 from typing import Dict, List, Optional, Set, Union
 
 import numpy as np
 
-from power_grid_model.core.error_handling import PowerGridBatchError, assert_no_error, find_error
+from power_grid_model.core.data_handling import (
+    create_output_data,
+    get_output_type,
+    is_batch_calculation,
+    prepare_input_view,
+    prepare_output_view,
+    prepare_update_view,
+    reduce_output_data,
+)
+from power_grid_model.core.error_handling import PowerGridBatchError, assert_no_error, handle_errors
 from power_grid_model.core.index_integer import IdNp, IdxNp
 from power_grid_model.core.options import Options
 from power_grid_model.core.power_grid_core import IDPtr, IdxPtr, ModelPtr
 from power_grid_model.core.power_grid_core import power_grid_core as pgc
-from power_grid_model.core.power_grid_meta import CDataset, initialize_array, power_grid_meta_data, prepare_cpp_array
 from power_grid_model.enum import CalculationMethod, CalculationType
 
 
 class PowerGridModel:
     """
     Main class for Power Grid Model
     """
@@ -91,15 +100,15 @@
                 value: 1D numpy structured array for this component input
             system_frequency: frequency of the power system, default 50 Hz
         """
         # destroy old instance
         pgc.destroy_model(self._model_ptr)
         self._all_component_count = None
         # create new
-        prepared_input: CDataset = prepare_cpp_array("input", input_data)
+        prepared_input = prepare_input_view(input_data)
         self._model_ptr = pgc.create_model(
             system_frequency,
             components=prepared_input.components,
             n_components=prepared_input.n_components,
             component_sizes=prepared_input.n_component_elements_per_scenario,
             input_data=prepared_input.data_ptrs_per_component,
         )
@@ -114,15 +123,15 @@
         Args:
             update_data: update data dictionary
                 key: component type name
                 value: 1D numpy structured array for this component update
         Returns:
             None
         """
-        prepared_update: CDataset = prepare_cpp_array("update", update_data)
+        prepared_update = prepare_update_view(update_data)
         pgc.update_model(
             self._model,
             prepared_update.n_components,
             prepared_update.components,
             prepared_update.n_component_elements_per_scenario,
             prepared_update.data_ptrs_per_component,
         )
@@ -145,132 +154,114 @@
         indexer_c = indexer.ctypes.data_as(IdxPtr)
         size = ids.size
         # call c function
         pgc.get_indexer(self._model, component_type, size, ids_c, indexer_c)
         assert_no_error()
         return indexer
 
-    # pylint: disable=too-many-locals
-    # pylint: disable=too-many-branches
+    def _construct_output(
+        self,
+        output_component_types: Optional[Union[Set[str], List[str]]],
+        calculation_type: CalculationType,
+        symmetric: bool,
+        batch_size: int,
+    ) -> Dict[str, np.ndarray]:
+        # prepare result dataset
+        all_component_count = self.all_component_count
+
+        # for power flow, there is no need for sensor output
+        if calculation_type == CalculationType.power_flow:
+            all_component_count = {k: v for k, v in all_component_count.items() if "sensor" not in k}
+
+        # limit all component count to user specified component types in output
+        if output_component_types is None:
+            output_component_types = set(all_component_count.keys())
+
+        return create_output_data(
+            output_component_types=output_component_types,
+            output_type=get_output_type(calculation_type=calculation_type, symmetric=symmetric),
+            all_component_count=all_component_count,
+            batch_size=batch_size,
+        )
+
+    @staticmethod
+    def _options(**kwargs) -> Options:
+        if "calculation_method" in kwargs:
+            calculation_method = kwargs["calculation_method"]
+            if isinstance(calculation_method, str):
+                kwargs["calculation_method"] = CalculationMethod[calculation_method]
+
+        opt = Options()
+        for key, value in kwargs.items():
+            setattr(opt, key, value.value if isinstance(value, IntEnum) else value)
+        return opt
+
+    def _handle_errors(self, continue_on_batch_error: bool, batch_size: int):
+        self._batch_error = handle_errors(continue_on_batch_error=continue_on_batch_error, batch_size=batch_size)
+
     # pylint: disable=too-many-arguments
-    def _calculate(
+    def _calculate_impl(
         self,
         calculation_type: CalculationType,
         symmetric: bool,
-        error_tolerance: float,
-        max_iterations: int,
-        calculation_method: Union[CalculationMethod, str],
         update_data: Optional[Dict[str, Union[np.ndarray, Dict[str, np.ndarray]]]],
-        threading: int,
         output_component_types: Optional[Union[Set[str], List[str]]],
+        options: Options,
         continue_on_batch_error: bool,
     ):
         """
         Core calculation routine
 
         Args:
-            calculation_type:
-            symmetric:
-            error_tolerance:
-            max_iterations:
-            calculation_method:
+            options:
             update_data:
-            threading:
             output_component_types:
             continue_on_batch_error:
 
         Returns:
 
         """
-        if isinstance(calculation_method, str):
-            calculation_method = CalculationMethod[calculation_method]
-        if symmetric:
-            output_type = "sym_output"
-        else:
-            output_type = "asym_output"
         self._batch_error = None
+        batch_calculation = is_batch_calculation(update_data=update_data)
 
-        # prepare update dataset
-        # update data exist for batch calculation
-        if update_data is not None:
-            batch_calculation = True
-        # no update dataset, create one batch with empty set
-        else:
-            batch_calculation = False
-            update_data = {}
-        prepared_update: CDataset = prepare_cpp_array(data_type="update", array_dict=update_data)
+        prepared_update = prepare_update_view(update_data)
         batch_size = prepared_update.batch_size
 
-        # prepare result dataset
-        all_component_count = self.all_component_count
-        # for power flow, there is no need for sensor output
-        if calculation_type == CalculationType.power_flow:
-            all_component_count = {k: v for k, v in all_component_count.items() if "sensor" not in k}
-        # limit all component count to user specified component types in output
-        if output_component_types is None:
-            output_component_types = set(all_component_count.keys())
-        # raise error is some specified components are unknown
-        unknown_components = [x for x in output_component_types if x not in power_grid_meta_data[output_type]]
-        if unknown_components:
-            raise KeyError(f"You have specified some unknown component types: {unknown_components}")
-        all_component_count = {k: v for k, v in all_component_count.items() if k in output_component_types}
-        # create result dataset
-        result_dict = {}
-        for name, count in all_component_count.items():
-            # intialize array
-            arr = initialize_array(output_type, name, (batch_size, count), empty=True)
-            result_dict[name] = arr
-        prepared_result: CDataset = prepare_cpp_array(data_type=output_type, array_dict=result_dict)
-
-        # prepare options
-        opt: Options = Options()
-        opt.calculation_type = calculation_type.value
-        opt.calculation_method = calculation_method.value
-        opt.symmetric = symmetric
-        opt.error_tolerance = error_tolerance
-        opt.max_iteration = max_iterations
-        opt.threading = threading
+        output_data = self._construct_output(
+            output_component_types=output_component_types,
+            calculation_type=calculation_type,
+            symmetric=symmetric,
+            batch_size=batch_size,
+        )
+        prepared_result = prepare_output_view(
+            output_data=output_data,
+            output_type=get_output_type(calculation_type=calculation_type, symmetric=symmetric),
+        )
 
         # run calculation
         pgc.calculate(
             # model and options
             self._model,
-            opt.opt,
+            options.opt,
             # result dataset
             prepared_result.n_components,
             prepared_result.components,
             prepared_result.data_ptrs_per_component,
             # update dataset
             batch_size,
             prepared_update.n_components,
             prepared_update.components,
             prepared_update.n_component_elements_per_scenario,
             prepared_update.indptrs_per_component,
             prepared_update.data_ptrs_per_component,
         )
 
-        # error handling
-        if not continue_on_batch_error:
-            assert_no_error(batch_size=batch_size)
-        else:
-            # continue on batch error
-            error: Optional[RuntimeError] = find_error(batch_size=batch_size)
-            if error is not None:
-                if isinstance(error, PowerGridBatchError):
-                    # continue on batch error
-                    self._batch_error = error
-                else:
-                    # raise normal error
-                    raise error
-
-        # flatten array for normal calculation
-        if not batch_calculation:
-            result_dict = {k: v.ravel() for k, v in result_dict.items()}
+        self._handle_errors(continue_on_batch_error=continue_on_batch_error, batch_size=batch_size)
 
-        return result_dict
+        return reduce_output_data(output_data=output_data, batch_calculation=batch_calculation)
 
     def calculate_power_flow(
         self,
         *,
         symmetric: bool = True,
         error_tolerance: float = 1e-8,
         max_iterations: int = 20,
@@ -327,23 +318,29 @@
                     for single calculation: 1D numpy structured array for the results of this component type
                     for batch calculation: 2D numpy structured array for the results of this component type
                         Dimension 0: each batch
                         Dimension 1: the result of each element for this component type
             Error handling:
                 in case an error in the core occurs, an exception will be thrown
         """
-        return self._calculate(
-            CalculationType.power_flow,
+        calculation_type = CalculationType.power_flow
+        options = self._options(
+            calculation_type=calculation_type,
             symmetric=symmetric,
             error_tolerance=error_tolerance,
             max_iterations=max_iterations,
             calculation_method=calculation_method,
-            update_data=update_data,
             threading=threading,
+        )
+        return self._calculate_impl(
+            calculation_type=calculation_type,
+            symmetric=symmetric,
+            update_data=update_data,
             output_component_types=output_component_types,
+            options=options,
             continue_on_batch_error=continue_on_batch_error,
         )
 
     def calculate_state_estimation(
         self,
         *,
         symmetric: bool = True,
@@ -402,21 +399,27 @@
                     for single calculation: 1D numpy structured array for the results of this component type
                     for batch calculation: 2D numpy structured array for the results of this component type
                         Dimension 0: each batch
                         Dimension 1: the result of each element for this component type
             Error handling:
                 in case an error in the core occurs, an exception will be thrown
         """
-        return self._calculate(
-            CalculationType.state_estimation,
+        calculation_type = CalculationType.state_estimation
+        options = self._options(
+            calculation_type=calculation_type,
             symmetric=symmetric,
             error_tolerance=error_tolerance,
             max_iterations=max_iterations,
             calculation_method=calculation_method,
-            update_data=update_data,
             threading=threading,
+        )
+        return self._calculate_impl(
+            calculation_type=calculation_type,
+            symmetric=symmetric,
+            update_data=update_data,
             output_component_types=output_component_types,
+            options=options,
             continue_on_batch_error=continue_on_batch_error,
         )
 
     def __del__(self):
         pgc.destroy_model(self._model_ptr)
```

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/data_types.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/data_types.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/enum.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/enum.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/utils.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/__init__.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/assertions.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/errors.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/rules.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/utils.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model/validation/validation.py` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model/validation/validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/PKG-INFO` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-grid-model
-Version: 1.5.0rc9195400270327
+Version: 1.5.0rc9196208314246
 Summary: Python/C++ library for distribution power system analysis
 Author-email: Alliander Dynamic Grid Calculation <dynamic.grid.calculation@alliander.com>
 License: MPL-2.0
 Project-URL: Home-page, https://lfenergy.org/projects/power-grid-model/
 Project-URL: GitHub, https://github.com/PowerGridModel/power-grid-model
 Project-URL: Documentation, https://power-grid-model.readthedocs.io/en/stable/
 Project-URL: Mailing-list, https://lists.lfenergy.org/g/powergridmodel
```

### Comparing `power-grid-model-1.5.0rc9195400270327/src/power_grid_model.egg-info/SOURCES.txt` & `power-grid-model-1.5.0rc9196208314246/src/power_grid_model.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 src/power_grid_model/utils.py
 src/power_grid_model.egg-info/PKG-INFO
 src/power_grid_model.egg-info/SOURCES.txt
 src/power_grid_model.egg-info/dependency_links.txt
 src/power_grid_model.egg-info/requires.txt
 src/power_grid_model.egg-info/top_level.txt
 src/power_grid_model/core/__init__.py
+src/power_grid_model/core/data_handling.py
 src/power_grid_model/core/error_handling.py
 src/power_grid_model/core/index_integer.py
 src/power_grid_model/core/options.py
 src/power_grid_model/core/power_grid_core.py
 src/power_grid_model/core/power_grid_meta.py
 src/power_grid_model/core/power_grid_model.py
 src/power_grid_model/validation/__init__.py
```

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-dependent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-incomplete-input/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-independent-not-cacheable/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-batch-newton/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-batch-newton/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/dummy-test-i-n-optional/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/gaia_grid.gnf` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/gaia_grid.gnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/gaia-example/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/gaia-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/multi-source-with-angle/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/multi-source-with-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/asym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/line/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/node/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/source/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/asymmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/line/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/node/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/shunt/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/source/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_gen/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/sym_load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/three_winding_transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/components/symmetric/transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/asymmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/pandapower/networks/symmetric/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/r-state-estimation/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/r-state-estimation/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/asym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/asym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/sym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/three-winding-transformer/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/three-winding-transformer/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-example/vision_grid.vnf` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-example/vision_grid.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf` & `power-grid-model-1.5.0rc9196208314246/tests/data/power_flow/vision-validation-network/vision_validation_network.vnf`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_a/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_b/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/single_phase_to_ground_c/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/three_phase_abc/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/three_phase_abc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ab/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_ac/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_bc/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ab/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_ac/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/sc_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/short_circuit/two_phase_to_ground_bc/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/1os2msr-no-angle/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/1os2msr-no-angle/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/sym_output_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/sym_output_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/distribution-case/update_batch.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/distribution-case/update_batch.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/dummy-test-sym/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/dummy-test-sym/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/node-injection-sensor-and-zero-injection/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/single-line-load/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/single-line-load/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/three_winding_transformer/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/three_winding_transformer/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/README.md` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/README.md`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/asym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/asym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/input.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/input.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/data/state_estimation/transmission-case/sym_output.json` & `power-grid-model-1.5.0rc9196208314246/tests/data/state_estimation/transmission-case/sym_output.json`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/test_0Z_model_validation.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/test_0Z_model_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/test_error_handling.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/test_meta_data.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/test_meta_data.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/test_power_grid_model.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/test_power_grid_model.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/test_utils.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/utils.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_assertions.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_assertions.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_batch_validation.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_batch_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_errors.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_errors.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_input_validation.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_input_validation.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_rules.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_utils.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_utils.py`

 * *Files identical despite different names*

### Comparing `power-grid-model-1.5.0rc9195400270327/tests/unit/validation/test_validation_functions.py` & `power-grid-model-1.5.0rc9196208314246/tests/unit/validation/test_validation_functions.py`

 * *Files identical despite different names*

