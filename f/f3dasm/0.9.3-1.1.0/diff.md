# Comparing `tmp/f3dasm-0.9.3.tar.gz` & `tmp/f3dasm-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f3dasm-0.9.3.tar", last modified: Mon Apr  3 09:22:07 2023, max compression
+gzip compressed data, was "f3dasm-1.1.0.tar", last modified: Thu Jun 29 14:38:01 2023, max compression
```

## Comparing `f3dasm-0.9.3.tar` & `f3dasm-1.1.0.tar`

### file list

```diff
@@ -1,125 +1,124 @@
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.605119 f3dasm-0.9.3/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-0.9.3/LICENSE
--rw-rw-r--   0 martin    (1000) martin    (1000)      164 2023-03-31 07:42:30.000000 f3dasm-0.9.3/MANIFEST.in
--rw-rw-r--   0 martin    (1000) martin    (1000)     3584 2023-04-03 09:22:07.605119 f3dasm-0.9.3/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     2203 2023-04-03 08:58:00.000000 f3dasm-0.9.3/README.md
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/docs/
--rw-rw-r--   0 martin    (1000) martin    (1000)       69 2023-03-31 08:16:15.000000 f3dasm-0.9.3/docs/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-03-31 07:42:30.000000 f3dasm-0.9.3/pyproject.toml
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/requirements/
--rw-rw-r--   0 martin    (1000) martin    (1000)       18 2023-03-31 07:42:30.000000 f3dasm-0.9.3/requirements/machinelearning.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-03-31 11:13:42.000000 f3dasm-0.9.3/requirements/optimization.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-03-31 07:42:30.000000 f3dasm-0.9.3/requirements/sampling.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       64 2023-03-31 13:03:34.000000 f3dasm-0.9.3/requirements.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-04-03 09:22:07.605119 f3dasm-0.9.3/setup.cfg
--rw-rw-r--   0 martin    (1000) martin    (1000)     3053 2023-04-03 09:21:59.000000 f3dasm-0.9.3/setup.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.589119 f3dasm-0.9.3/src/
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/src/f3dasm/
--rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-04-03 08:58:46.000000 f3dasm-0.9.3/src/f3dasm/VERSION
--rw-rw-r--   0 martin    (1000) martin    (1000)     1774 2023-03-31 08:06:53.000000 f3dasm-0.9.3/src/f3dasm/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5469 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/_imports.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1027 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/_logging.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3982 2023-04-03 09:00:16.000000 f3dasm-0.9.3/src/f3dasm/_show_versions.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/src/f3dasm/data/
--rw-rw-r--   0 martin    (1000) martin    (1000)      153 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/data/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2693 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/data/benchmarkfunction_data.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      923 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/data/learningdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1790 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/data/linearregression_data.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/src/f3dasm/design/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1129 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/design/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      856 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/design/all_parameters.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      678 2023-03-10 12:07:18.000000 f3dasm-0.9.3/src/f3dasm/design/constraint.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     9680 2023-03-31 08:04:34.000000 f3dasm-0.9.3/src/f3dasm/design/design.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7672 2023-03-31 08:59:31.000000 f3dasm-0.9.3/src/f3dasm/design/experimentdata.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5006 2023-03-31 08:05:48.000000 f3dasm-0.9.3/src/f3dasm/design/parameter.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4747 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/design/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.597119 f3dasm-0.9.3/src/f3dasm/experiment/
--rw-rw-r--   0 martin    (1000) martin    (1000)      746 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/experiment/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4244 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/experiment/filehandler.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7775 2023-03-31 11:47:00.000000 f3dasm-0.9.3/src/f3dasm/experiment/jobs.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2898 2023-03-31 09:01:59.000000 f3dasm-0.9.3/src/f3dasm/experiment/logging.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      730 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/experiment/quickstart.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.597119 f3dasm-0.9.3/src/f3dasm/functions/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3507 2023-03-31 08:39:55.000000 f3dasm-0.9.3/src/f3dasm/functions/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.597119 f3dasm-0.9.3/src/f3dasm/functions/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-0.9.3/src/f3dasm/functions/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7314 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/functions/adapters/augmentor.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4493 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/functions/adapters/pybenchfunction.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    10185 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/functions/function.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    81361 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/functions/pybenchfunction.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.597119 f3dasm-0.9.3/src/f3dasm/machinelearning/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1628 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.597119 f3dasm-0.9.3/src/f3dasm/machinelearning/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-10 12:07:18.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2595 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1036 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/all_models.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4946 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/evaluator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1523 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/linear_regression.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1039 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/loss_functions.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1183 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2475 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/passthrough_model.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1924 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/machinelearning/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.601119 f3dasm-0.9.3/src/f3dasm/optimization/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3704 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1210 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/_protocol.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1756 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/adam.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1675 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/adamax.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.601119 f3dasm-0.9.3/src/f3dasm/optimization/adapters/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-0.9.3/src/f3dasm/optimization/adapters/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4705 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/adapters/pygmo_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3404 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/adapters/scipy_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4111 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/adapters/tensorflow_implementations.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2442 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/all_optimizers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     3605 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/bayesianoptimization.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1131 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/cg.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1588 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/cmaes.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1273 2023-03-31 07:42:17.000000 f3dasm-0.9.3/src/f3dasm/optimization/cmaesadam.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1377 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/cobyla.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2219 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/differentialevolution.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2108 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/ftrl.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1204 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/lbfgsb.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1664 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/nadam.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1267 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/neldermead.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     8240 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/optimizer.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1679 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/pso.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1666 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/randomsearch.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1707 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/rmsprop.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1832 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/sade.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1488 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/sea.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2035 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/sga.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1570 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/sgd.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1973 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/simulatedannealing.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     2180 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/utils.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1968 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/optimization/xnes.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     7481 2023-03-31 07:58:08.000000 f3dasm-0.9.3/src/f3dasm/run_optimization.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.601119 f3dasm-0.9.3/src/f3dasm/sampling/
--rw-rw-r--   0 martin    (1000) martin    (1000)     1685 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1086 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/all_samplers.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1748 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/latinhypercube.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1307 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/randomuniform.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5887 2023-03-31 07:51:55.000000 f3dasm-0.9.3/src/f3dasm/sampling/sampler.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1668 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/sobolsequence.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1840 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/sampling/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.605119 f3dasm-0.9.3/src/f3dasm/simulation/
--rw-rw-r--   0 martin    (1000) martin    (1000)      107 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/__init__.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.605119 f3dasm-0.9.3/src/f3dasm/simulation/abaqus_script/
--rw-rw-r--   0 martin    (1000) martin    (1000)       63 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/abaqus_script/__init__.py
--rwxrwxr-x   0 martin    (1000) martin    (1000)    32487 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/abaqus_script/flower_rve_script.py
--rw-rw-r--   0 martin    (1000) martin    (1000)    11667 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/abaqus_simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     4520 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/abaqus_utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.605119 f3dasm-0.9.3/src/f3dasm/simulation/cases/
--rw-rw-r--   0 martin    (1000) martin    (1000)       34 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/cases/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     5736 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/cases/flower_rve.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1422 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/simulation/simulator.py
--rw-rw-r--   0 martin    (1000) martin    (1000)     1266 2023-03-31 07:42:30.000000 f3dasm-0.9.3/src/f3dasm/utils.py
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.593119 f3dasm-0.9.3/src/f3dasm.egg-info/
--rw-rw-r--   0 martin    (1000) martin    (1000)     3584 2023-04-03 09:22:07.000000 f3dasm-0.9.3/src/f3dasm.egg-info/PKG-INFO
--rw-rw-r--   0 martin    (1000) martin    (1000)     3544 2023-04-03 09:22:07.000000 f3dasm-0.9.3/src/f3dasm.egg-info/SOURCES.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-04-03 09:22:07.000000 f3dasm-0.9.3/src/f3dasm.egg-info/dependency_links.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)      532 2023-04-03 09:22:07.000000 f3dasm-0.9.3/src/f3dasm.egg-info/requires.txt
--rw-rw-r--   0 martin    (1000) martin    (1000)        7 2023-04-03 09:22:07.000000 f3dasm-0.9.3/src/f3dasm.egg-info/top_level.txt
-drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-04-03 09:22:07.605119 f3dasm-0.9.3/tests/
--rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-0.9.3/tests/__init__.py
--rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-0.9.3/tests/__init__.pyc
--rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-03-31 07:42:30.000000 f3dasm-0.9.3/tests/conftest.py
--rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-0.9.3/tests/requirements.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.818372 f3dasm-1.1.0/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1531 2023-03-30 12:29:51.000000 f3dasm-1.1.0/LICENSE
+-rw-rw-r--   0 martin    (1000) martin    (1000)      164 2023-03-31 07:42:30.000000 f3dasm-1.1.0/MANIFEST.in
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3573 2023-06-29 14:38:01.818372 f3dasm-1.1.0/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2193 2023-04-17 07:39:19.000000 f3dasm-1.1.0/README.md
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/docs/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       69 2023-03-31 08:16:15.000000 f3dasm-1.1.0/docs/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      457 2023-03-31 07:42:30.000000 f3dasm-1.1.0/pyproject.toml
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/requirements/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       18 2023-03-31 07:42:30.000000 f3dasm-1.1.0/requirements/machinelearning.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       78 2023-03-31 11:13:42.000000 f3dasm-1.1.0/requirements/optimization.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-03-31 07:42:30.000000 f3dasm-1.1.0/requirements/sampling.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       64 2023-03-31 13:03:34.000000 f3dasm-1.1.0/requirements.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)       38 2023-06-29 14:38:01.818372 f3dasm-1.1.0/setup.cfg
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3053 2023-06-29 14:36:32.000000 f3dasm-1.1.0/setup.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.802372 f3dasm-1.1.0/src/
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        5 2023-04-03 08:58:46.000000 f3dasm-1.1.0/src/f3dasm/VERSION
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1723 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5469 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/_imports.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4886 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/_logging.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3982 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/_show_versions.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/data/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      153 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2693 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/benchmarkfunction_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      923 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/learningdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1790 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/data/linearregression_data.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/design/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      885 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6902 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/_data.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4863 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/_jobqueue.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    15181 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/design.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    17309 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/experimentdata.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5609 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/design/parameter.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/experiment/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      760 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/experiment/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4244 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/experiment/filehandler.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2900 2023-06-05 12:02:43.000000 f3dasm-1.1.0/src/f3dasm/experiment/logging.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6117 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/experiment/parallelization.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      730 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/experiment/quickstart.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm/functions/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3507 2023-03-31 08:39:55.000000 f3dasm-1.1.0/src/f3dasm/functions/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/functions/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7314 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/augmentor.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4503 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/adapters/pybenchfunction.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    10469 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/function.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    81430 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/functions/pybenchfunction.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/machinelearning/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1760 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.810372 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2023-03-10 12:07:18.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3073 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/tensorflow_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1036 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/all_models.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4946 2023-05-26 13:48:37.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/evaluator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1523 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/linear_regression.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1039 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/loss_functions.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1593 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/mnist_classifier.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1280 2023-04-12 15:38:50.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2475 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/passthrough_model.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1924 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/machinelearning/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/optimization/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3704 2023-04-19 11:31:27.000000 f3dasm-1.1.0/src/f3dasm/optimization/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1296 2023-04-12 07:58:51.000000 f3dasm-1.1.0/src/f3dasm/optimization/_protocol.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1756 2023-04-04 11:19:13.000000 f3dasm-1.1.0/src/f3dasm/optimization/adam.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1675 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adamax.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/optimization/adapters/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-11-03 14:34:52.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4745 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/pygmo_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3404 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/scipy_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4111 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/adapters/tensorflow_implementations.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2736 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/all_optimizers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3605 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/bayesianoptimization.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1131 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cg.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1588 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cmaes.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1377 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/cobyla.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2219 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/differentialevolution.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2108 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/ftrl.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1204 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/lbfgsb.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1664 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/nadam.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1267 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/neldermead.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     8420 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/optimization/optimizer.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1679 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/pso.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1666 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/randomsearch.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1707 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/rmsprop.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1832 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sade.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1488 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sea.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2035 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sga.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1570 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/sgd.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1973 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/simulatedannealing.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     2170 2023-04-14 09:00:21.000000 f3dasm-1.1.0/src/f3dasm/optimization/utils.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1968 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/optimization/xnes.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     7356 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/run_optimization.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/sampling/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1685 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1086 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/all_samplers.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1752 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/sampling/latinhypercube.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1307 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/sampling/randomuniform.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     6529 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/sampling/sampler.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1668 2023-06-23 13:36:28.000000 f3dasm-1.1.0/src/f3dasm/sampling/sobolsequence.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1826 2023-04-14 08:29:08.000000 f3dasm-1.1.0/src/f3dasm/sampling/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/
+-rw-rw-r--   0 martin    (1000) martin    (1000)      142 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/simulation/__init__.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       63 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/__init__.py
+-rwxrwxr-x   0 martin    (1000) martin    (1000)    32487 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/flower_rve_script.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)    11667 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_simulator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     4520 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/abaqus_utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/src/f3dasm/simulation/cases/
+-rw-rw-r--   0 martin    (1000) martin    (1000)       34 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/cases/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     5736 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/simulation/cases/flower_rve.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1306 2023-06-29 14:36:32.000000 f3dasm-1.1.0/src/f3dasm/simulation/simulator.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)     1266 2023-03-31 07:42:30.000000 f3dasm-1.1.0/src/f3dasm/utils.py
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.806372 f3dasm-1.1.0/src/f3dasm.egg-info/
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3573 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/PKG-INFO
+-rw-rw-r--   0 martin    (1000) martin    (1000)     3528 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/SOURCES.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        1 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/dependency_links.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)      532 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/requires.txt
+-rw-rw-r--   0 martin    (1000) martin    (1000)        7 2023-06-29 14:38:01.000000 f3dasm-1.1.0/src/f3dasm.egg-info/top_level.txt
+drwxrwxr-x   0 martin    (1000) martin    (1000)        0 2023-06-29 14:38:01.814372 f3dasm-1.1.0/tests/
+-rw-rw-r--   0 martin    (1000) martin    (1000)        0 2022-08-17 09:47:40.000000 f3dasm-1.1.0/tests/__init__.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)      141 2022-08-31 10:13:29.000000 f3dasm-1.1.0/tests/__init__.pyc
+-rw-rw-r--   0 martin    (1000) martin    (1000)      855 2023-03-31 07:42:30.000000 f3dasm-1.1.0/tests/conftest.py
+-rw-rw-r--   0 martin    (1000) martin    (1000)       29 2023-03-10 12:07:18.000000 f3dasm-1.1.0/tests/requirements.txt
```

### Comparing `f3dasm-0.9.3/LICENSE` & `f3dasm-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/PKG-INFO` & `f3dasm-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 0.9.3
+Version: 1.1.0
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
-Home-page: https://github.com/bessagroup/F3DASM
+Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
-Project-URL: Documentation, https://bessagroup.github.io/F3DASM/
-Project-URL: Wiki, https://github.com/bessagroup/F3DASM/wiki
+Project-URL: Documentation, https://bessagroup.github.io/f3dasm/
+Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
 Keywords: data-driven materials framework,machine learning
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -37,17 +37,17 @@
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
-[**Docs**](https://bessagroup.github.io/F3DASM/)
-| [**Installation**](https://bessagroup.github.io/F3DASM/gettingstarted.html)
-| [**GitHub**](https://github.com/bessagroup/F3DASM/tree/versionmartin)
+[**Docs**](https://bessagroup.github.io/f3dasm/)
+| [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
+| [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 | [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
```

### Comparing `f3dasm-0.9.3/README.md` & `f3dasm-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
-[**Docs**](https://bessagroup.github.io/F3DASM/)
-| [**Installation**](https://bessagroup.github.io/F3DASM/gettingstarted.html)
-| [**GitHub**](https://github.com/bessagroup/F3DASM/tree/versionmartin)
+[**Docs**](https://bessagroup.github.io/f3dasm/)
+| [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
+| [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 | [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
@@ -27,8 +27,8 @@
 
 [1] Bessa, M. A., Bostanabad, R., Liu, Z., Hu, A., Apley, D. W., Brinson, C., Chen, W., & Liu, W. K. (2017). A framework for data-driven analysis of materials under uncertainty: Countering the curse of dimensionality. Computer Methods in Applied Mechanics and Engineering, 320, 633-667.
 
 [2] Bessa, M. A., & Pellegrino, S. (2018). Design of ultra-thin shell structures in the stochastic post-buckling range using Bayesian machine learning and optimization. International Journal of Solids and Structures, 139, 174-188.
 
 [3] Bessa, M. A., Glowacki, P., & Houlder, M. (2019). Bayesian machine learning in metamaterial design: fragile becomes super-compressible. Advanced Materials, 31(48), 1904845.
 
-[4] Mojtaba, M., Bostanabad, R., Chen, W., Ehmann, K., Cao, J., & Bessa, M. A. (2019). Deep learning predicts path-dependent plasticity. Proceedings of the National Academy of Sciences, 116(52), 26414-26420.
+[4] Mojtaba, M., Bostanabad, R., Chen, W., Ehmann, K., Cao, J., & Bessa, M. A. (2019). Deep learning predicts path-dependent plasticity. Proceedings of the National Academy of Sciences, 116(52), 26414-26420.
```

### Comparing `f3dasm-0.9.3/setup.py` & `f3dasm-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from setuptools import find_packages, setup
 
 here = Path(__file__).absolute().parent
 
 # version
 # version = here.joinpath("src", "f3dasm", "VERSION").read_text().strip()
-version = '0.9.3'
+version = '1.1.0'
 
 # Get the long description from the README file
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 # Get requirements
 
@@ -43,18 +43,18 @@
                                    ["flake8"]))
 setup(
     name="f3dasm",
     version=version,
     description="f3dasm - Framework for Data-driven development and Analysis of Structures and Materials",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    url="https://github.com/bessagroup/F3DASM",
+    url="https://github.com/bessagroup/f3dasm",
     project_urls={
-        "Documentation": "https://bessagroup.github.io/F3DASM/",
-        "Wiki": "https://github.com/bessagroup/F3DASM/wiki",
+        "Documentation": "https://bessagroup.github.io/f3dasm/",
+        "Wiki": "https://github.com/bessagroup/f3dasm/wiki",
     },
     author="Martin van der Schelling",
     author_email="M.P.vanderSchelling@tudelft.nl",
     license="BSD",
     classifiers=[
 
         "License :: OSI Approved :: BSD License",
```

### Comparing `f3dasm-0.9.3/src/f3dasm/__init__.py` & `f3dasm-1.1.0/src/f3dasm/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-F3DASM - A package for data-driven design and analysis of structures and materials
+f3dasm - A package for data-driven design and analysis of structures and materials
 
 This package provides tools for designing and optimizing materials, including
 functions for data analysis, design of experiments, machine learning, optimization,
 sampling, and simulation.
 
 Usage:
   import f3dasm
@@ -18,23 +18,22 @@
                     machinelearning, optimization, sampling, simulation)
 
 from ._show_versions import __version__, show_versions
 # Design classes
 from .design.design import DesignSpace, make_nd_continuous_design
 from .design.experimentdata import ExperimentData
 from .design.parameter import (CategoricalParameter, ConstantParameter,
-                               ConstraintInterface, ContinuousParameter,
-                               DiscreteParameter)
+                               ContinuousParameter, DiscreteParameter)
+from .experiment.parallelization import run_operation_on_experiments
 # Base classes
 from .functions.function import Function
 from .machinelearning.model import Model
 from .optimization.optimizer import Optimizer
-from .run_optimization import (OptimizationResult,
-                               create_optimizationresult_from_json,
-                               run_multiple_realizations, run_optimization)
+from .run_optimization import (OptimizationResult, run_multiple_realizations,
+                               run_optimization)
 from .sampling.sampler import Sampler
 from .utils import find_class, write_json
 
 #                                                        Authorship and Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
```

### Comparing `f3dasm-0.9.3/src/f3dasm/_imports.py` & `f3dasm-1.1.0/src/f3dasm/_imports.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/_show_versions.py` & `f3dasm-1.1.0/src/f3dasm/_show_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # =============================================================================
 #
 # =============================================================================
 
 # version
 # here = Path(__file__).absolute().parent
 # __version__ = here.joinpath("VERSION").read_text().strip()
-__version__ = '0.9.3'
+__version__ = '1.1.0'
 
 # List of the dependencies per extension:
 CORE_DEPS = [
     'numpy',
     'scipy',
     'pandas',
     'matplotlib',
```

### Comparing `f3dasm-0.9.3/src/f3dasm/data/benchmarkfunction_data.py` & `f3dasm-1.1.0/src/f3dasm/data/benchmarkfunction_data.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/data/learningdata.py` & `f3dasm-1.1.0/src/f3dasm/data/learningdata.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/data/linearregression_data.py` & `f3dasm-1.1.0/src/f3dasm/data/linearregression_data.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/design/__init__.py` & `f3dasm-1.1.0/src/f3dasm/design/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 #                                                                       Modules
 # =============================================================================
 
 # Local
-from .all_parameters import PARAMETERS
-from .constraint import Constraint
 from .design import DesignSpace, make_nd_continuous_design
 from .experimentdata import ExperimentData
 from .parameter import (CategoricalParameter, ConstantParameter,
-                        ContinuousParameter, DiscreteParameter, Parameter)
-from .utils import (create_design_from_json, create_experimentdata_from_json,
-                    create_parameter_from_json, find_parameter,
-                    load_experimentdata)
+                        ContinuousParameter, DiscreteParameter, Parameter, PARAMETERS)
+
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
```

### Comparing `f3dasm-0.9.3/src/f3dasm/design/parameter.py` & `f3dasm-1.1.0/src/f3dasm/design/parameter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 import json
 from dataclasses import dataclass, field
-from typing import Any, List
+from typing import Any, ClassVar, List, Type
 
 # Third-party core
 import numpy as np
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
@@ -21,65 +21,85 @@
 
 @dataclass
 class Parameter:
     """Interface class of a search space parameter
 
     Parameters
     ----------
-    name
-        name of the parameter
     """
-
-    name: str
-    _type: str = field(init=False, default="object")
+    _type: ClassVar[str] = field(init=False, default="object")
 
     @classmethod
     def get_name(self) -> str:
+        """Return the name of the parameter class"""
         return self.__name__
 
-    def to_json(self) -> str:  # Tuple[dict, str]:
-        args = self.__dict__
-        name = self.get_name()
-        return json.dumps((args, name))
-        # return self.__dict__, self.get_name()
-
 
 @dataclass
 class ConstantParameter(Parameter):
-    """Create a search space parameter that is constant
+    """Create a search space parameter that is constant.
 
     Parameters
     ----------
-    name
-        name of the parameter
-    value
-        value of the parameters
+    value : Any
+        The constant value of the parameter.
+
+    Attributes
+    ----------
+    _type : str
+        The type of the parameter, which is always 'object'.
+
+    Raises
+    ------
+    TypeError
+        If the value is not hashable.
+
     """
 
     value: Any
-    _type: str = field(init=False, default="category")
+    _type: ClassVar[str] = field(init=False, default="object")
+
+    def __post_init__(self):
+        self._check_hashable()
+
+    def _check_hashable(self):
+        """Check if the value is hashable."""
+        try:
+            hash(self.value)
+        except TypeError:
+            raise TypeError("The value must be hashable.")
 
 
 @dataclass
 class ContinuousParameter(Parameter):
-    """Create a search space parameter that is continuous
+    """
+    A search space parameter that is continuous.
 
-    Parameters
+    Attributes
     ----------
-    name
-        name of the parameter
-    lower_bound
-        lower bound of continuous search space
-    upper_bound
-        upper bound of continuous search space (exclusive)
+    lower_bound : float, optional
+        The lower bound of the continuous search space. Defaults to negative infinity.
+    upper_bound : float, optional
+        The upper bound of the continuous search space (exclusive). Defaults to infinity.
+
+    Raises
+    ------
+    TypeError
+        If the boundaries are not floats.
+    ValueError
+        If the upper bound is less than the lower bound, or if the lower bound is equal to the upper bound.
+
+    Notes
+    -----
+    This class inherits from the `Parameter` class and adds the ability to specify a continuous search space.
     """
 
     lower_bound: float = field(default=-np.inf)
     upper_bound: float = field(default=np.inf)
-    _type: str = field(init=False, default="float")
+    _type: ClassVar[str] = field(init=False, default="float")
 
     def __post_init__(self):
         self._check_types()
         self._check_range()
 
     def _check_types(self):
         """Check if the boundaries are actually floats"""
@@ -98,25 +118,23 @@
 
 @dataclass
 class DiscreteParameter(Parameter):
     """Create a search space parameter that is discrete
 
     Parameters
     ----------
-    name
-        name of the parameter
     lower_bound
         lower bound of discrete search space
     upper_bound
         upper bound of discrete search space (exclusive)
     """
 
     lower_bound: int = field(default=0)
     upper_bound: int = field(default=1)
-    _type: str = field(init=False, default="int")
+    _type: ClassVar[str] = field(init=False, default="int")
 
     def __post_init__(self):
         self._check_types()
         self._check_range()
 
     def _check_types(self):
         """Check if the boundaries are actually ints"""
@@ -135,16 +153,14 @@
 
 @dataclass
 class CategoricalParameter(Parameter):
     """Create a search space parameter that is categorical
 
     Parameters
     ----------
-    name
-        name of the parameter
     categories
         list of strings that represent available categories
     """
 
     categories: List[str]
     _type: str = field(init=False, default="category")
 
@@ -156,20 +172,15 @@
         """Check if there are duplicates in the categories list"""
         if len(self.categories) != len(set(self.categories)):
             raise ValueError("Categories contain duplicates!")
 
     def _check_types(self):
         """Check if the entries of the lists are all strings"""
 
-        if not isinstance(self.categories, list):
-            raise TypeError(f"Expect list, got {type(self.categories)}")
+        self.categories = list(self.categories)  # Convert to list because hydra parses omegaconf.ListConfig
 
         for category in self.categories:
             if not isinstance(category, str):
                 raise TypeError(f"Expect string, got {type(category)}")
 
 
-@dataclass
-class ConstraintInterface:
-    """Interface for constraints"""
-
-    pass
+PARAMETERS = [CategoricalParameter, ConstantParameter, ContinuousParameter, DiscreteParameter]
```

### Comparing `f3dasm-0.9.3/src/f3dasm/experiment/filehandler.py` & `f3dasm-1.1.0/src/f3dasm/experiment/filehandler.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/experiment/logging.py` & `f3dasm-1.1.0/src/f3dasm/experiment/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 if self.stream is None:
                     self.stream = self._open()
 
                 _lock_file(self.stream)
                 StreamHandler.emit(self, record)
 
                 _unlock_file(self.stream)
-                print("Succesfully logged!")
+                # print("Succesfully logged!")
 
                 break
             except IOError as e:
                 # the file is locked by another process
                 if e.errno == errno.EAGAIN:
                     print("The log file is currently locked by another process. Retrying in 1 second...")
                     sleep(1)
```

### Comparing `f3dasm-0.9.3/src/f3dasm/experiment/quickstart.py` & `f3dasm-1.1.0/src/f3dasm/experiment/quickstart.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/functions/__init__.py` & `f3dasm-1.1.0/src/f3dasm/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/functions/adapters/augmentor.py` & `f3dasm-1.1.0/src/f3dasm/functions/adapters/augmentor.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/functions/adapters/pybenchfunction.py` & `f3dasm-1.1.0/src/f3dasm/functions/adapters/pybenchfunction.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,16 +96,16 @@
             [
                 np.random.uniform(
                     low=-abs(g[d] - self.scale_bounds[d, 0]), high=abs(g[d] - self.scale_bounds[d, 1]))
                 for d in range(self.dimensionality)
             ]
         )
 
-        o = Offset(offset=unscaled_offset)
-        self.augmentor.insert_input_augmentor(position=0, augmentor=o)
+        self.o = Offset(offset=unscaled_offset)
+        self.augmentor.insert_input_augmentor(position=0, augmentor=self.o)
 
     def _get_global_minimum_for_offset_calculation(self):
         """Get the global minimum used for offset calculations
 
         Returns
         -------
             Returns a numpy array containing the global
```

### Comparing `f3dasm-0.9.3/src/f3dasm/functions/function.py` & `f3dasm-1.1.0/src/f3dasm/functions/function.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,15 +199,17 @@
 
     def plot(
         self,
         orientation: str = "3D",
         px: int = 300,
         domain: np.ndarray = np.array([[0.0, 1.0], [0.0, 1.0]]),
         show: bool = True,
+        ax: plt.Axes = None,
     ) -> Tuple[plt.Figure, plt.Axes]:  # pragma: no cover
+        # TODO: orientation string is case sensitive!
         """Generate a surface plot, either 2D or 3D, of the function
 
         Parameters
         ----------
         orientation, optional
             Either 2D or 3D orientation
         px, optional
@@ -224,28 +226,33 @@
         if not show:
             plt.ioff()
         else:
             plt.ion()
 
         xv, yv, Y = self._create_mesh(px=px, domain=domain)
 
+        # Shift Y values to avoid log(0)
+        Y_shifted = Y - np.min(Y) + 1e-6  # Add a small constant to avoid log(0)
+
         fig = plt.figure(figsize=(7, 7), constrained_layout=True)
         if orientation == "2D":
-            ax = plt.axes()
-            ax.pcolormesh(xv, yv, Y, cmap="viridis",
+            if ax is None:
+                ax = plt.axes()
+            ax.pcolormesh(xv, yv, Y_shifted, cmap="viridis",
                           norm=mcol.LogNorm())  # mcol.LogNorm()
             # fig.colorbar(cm.ScalarMappable(norm=mcol.LogNorm(), cmap="viridis"), ax=ax)
 
         if orientation == "3D":
-            ax = plt.axes(projection="3d", elev=50, azim=-50)
+            if ax is None:
+                ax = plt.axes(projection="3d", elev=50, azim=-50)
 
             ax.plot_surface(
                 xv,
                 yv,
-                Y,
+                Y_shifted,
                 rstride=1,
                 cstride=1,
                 edgecolor="none",
                 alpha=0.8,
                 cmap="viridis",
                 norm=mcol.LogNorm(),  # mcol.LogNorm()
                 zorder=1,
```

### Comparing `f3dasm-0.9.3/src/f3dasm/functions/pybenchfunction.py` & `f3dasm-1.1.0/src/f3dasm/functions/pybenchfunction.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,16 @@
         self.input_domain = np.array([[-32, 32], [-32, 32]])
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
         X = np.array([0.682584587365898, -0.36075325513719])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+        Y = np.array([[-195.629028238419]])
+        return (self._retrieve_original_input(X), Y)
 
     def evaluate(self, X):
         x, y = X
         res = -200 * np.exp(-0.2 * np.sqrt(x**2 + y**2))
         res += 5 * np.exp(np.cos(3 * x) + np.sin(3 * y))
         return res
 
@@ -198,15 +199,15 @@
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
 
         if d != 2:  # WARNING ! Is only is available for d=2
-            return (None, None)
+            return (None, np.array([[-4.5901016]]))  # This is the global minimum for d=2
 
         X = np.array([-1.51, -0.755])
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         X, Xp1 = X[:-1], X[1]
         res = np.sum(np.exp(-0.2) * np.sqrt(
@@ -239,15 +240,16 @@
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
         X = np.array([1 / (i + 1) for i in range(d)])
         X = np.array([0, 0])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+        Y = np.array([[-2.02180678]])
+        return (self._retrieve_original_input(X), Y)
 
     def evaluate(self, X):
         d = X.shape[0]
         x, y = X
         res = np.cos(x) * np.sin(y) - x / (y**2 + 1)
         return res
 
@@ -317,15 +319,15 @@
 
     def get_global_minimum(self, d):
         X = np.array([3, 0.5])
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         x, y = X
-        res = (1.5 - x + x * y) ** 2 + (2.25 - x + x * y**2) ** 2 + (2.625 - x + x * y**3) * 2
+        res = (1.5 - x + x * y) ** 2 + (2.25 - x + x * y**2) ** 2 + (2.625 - x + x * y**3) ** 2
         return res
 
 
 class Bird(PyBenchFunction):
     """.. image:: ../img/functions/Bird.png"""
 
     name = "Bird"
@@ -671,50 +673,51 @@
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         x, y = X
         res = 100 * np.sqrt(np.abs(y - 0.01 * x**2)) + 0.01 * np.abs(x + 10)
         return res
 
-        # class Colville(PyBenchFunction):
-        #     """.. image:: ../img/functions/Colville.png"""
 
-        #     name = "Colville"
-        #     continuous = True
-        #     convex = False
-        #     separable = False
-        #     differentiable = True
-        #     multimodal = True
-        #     randomized_term = False
-        #     parametric = False
-
-        #     @classmethod
-        #     def is_dim_compatible(cls, d):
-        #         assert (d is None) or (
-        #             isinstance(d, int) and (not d < 0)
-        #         ), "The dimension d must be None or a positive integer"
-        #         return d == 4
-
-        #     def _set_parameters(self):
-        #         d = self.dimensionality
-        #         self.input_domain = np.array([[-10, 10], [-10, 10], [-10, 10], [-10, 10]])
-
-        #     def get_param(self):
-        #         return {}
-
-        #     def get_global_minimum(self, d):
-        #         X = np.array([1, 1, 1, 1])
-        #         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
-
-        #     def evaluate(self, X):
-        # x1, x2, x3, x4 = X
-        # res = 100 * (x1**2 - x2) ** 2 + (x1 - 1) ** 2 + (x3 - 1) ** 2
-        # res = res + 90 * (x3**2 - x4) ** 2 + 10.1 * ((x2 - 1)
-        #                                             ** 2 + (x4 - 1) ** 2) + 19.8 * (x2 - 1) * (x4 - 1)
-        # return res
+class Colville(PyBenchFunction):
+    """.. image:: ../img/functions/Colville.png"""
+
+    name = "Colville"
+    continuous = True
+    convex = False
+    separable = False
+    differentiable = True
+    multimodal = True
+    randomized_term = False
+    parametric = False
+
+    @classmethod
+    def is_dim_compatible(cls, d):
+        assert (d is None) or (
+            isinstance(d, int) and (not d < 0)
+        ), "The dimension d must be None or a positive integer"
+        return d == 4
+
+    def _set_parameters(self):
+        d = self.dimensionality
+        self.input_domain = np.array([[-10, 10], [-10, 10], [-10, 10], [-10, 10]])
+
+    def get_param(self):
+        return {}
+
+    def get_global_minimum(self, d):
+        X = np.array([1, 1, 1, 1])
+        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+
+    def evaluate(self, X):
+        x1, x2, x3, x4 = X
+        res = 100 * (x1**2 - x2) ** 2 + (x1 - 1) ** 2 + (x3 - 1) ** 2
+        res = res + 90 * (x3**2 - x4) ** 2 + 10.1 * ((x2 - 1)
+                                                     ** 2 + (x4 - 1) ** 2) + 19.8 * (x2 - 1) * (x4 - 1)
+        return res
 
 
 class CrossInTray(PyBenchFunction):
     """.. image:: ../img/functions/CrossInTray.png"""
 
     name = "Cross-in-Tray"
     continuous = True
@@ -832,15 +835,15 @@
 
     def get_global_minimum(self, d):
         X = np.array([[0, -15], [0, 15]])
         return (self._retrieve_original_input(X), [self(x) for x in self._retrieve_original_input(X)])
 
     def evaluate(self, X):
         x, y = X
-        res = 1e5 * x**2 + y**2 - (x**2 + y**2) + 1e-5 * (x**2 + y**2) ** 4
+        res = 1e5 * x**2 + y**2 - (x**2 + y**2) ** 2 + 1e-5 * (x**2 + y**2) ** 4
         return res
 
 
 class DixonPrice(PyBenchFunction):
     """.. image:: ../img/functions/DixonPrice.png"""
 
     name = "Dixon Price"
@@ -863,15 +866,15 @@
         d = self.dimensionality
         self.input_domain = np.array([[-10, 10] for _ in range(d)])
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
-        X = np.array([2 ** ((-(2 ** (i)) - 2) / 2**i)
+        X = np.array([2 ** -(((2 ** (i)) - 2) / 2**i)
                      for i in range(1, d + 1)])
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         d = X.shape[0]
         res = (X[0] - 1) ** 2 + np.sum(
             [(i + 1) * (2 * X[i] ** 2 - X[i - 1]) ** 2 for i in range(1, d)])
@@ -1016,53 +1019,53 @@
 
     def get_global_minimum(self, d):
         X = np.array([512, 404.2319])
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         x, y = X
-        res = -(y + 47) * np.sin(np.sqrt(np.abs(y + x / 2 + 47))) - \
-            x * np.sin(np.sqrt(np.abs(x - y - 47)))
+        res = -(y + 47) * np.sin(np.sqrt(np.abs(y + 0.5 * x + 47))) - \
+            x * np.sin(np.sqrt(np.abs(x - (y + 47))))
         return res
 
 
-# class Exponential(PyBenchFunction):
-#     """.. image:: ../img/functions/Exponential.png"""
+class Exponential(PyBenchFunction):
+    """.. image:: ../img/functions/Exponential.png"""
 
-#     name = "Exponential"
-#     continuous = True
-#     convex = True
-#     separable = True
-#     differentiable = True
-#     multimodal = False
-#     randomized_term = False
-#     parametric = False
+    name = "Exponential"
+    continuous = True
+    convex = True
+    separable = True
+    differentiable = True
+    multimodal = False
+    randomized_term = False
+    parametric = False
 
-#     @classmethod
-#     def is_dim_compatible(cls, d):
-#         assert (d is None) or (
-#             isinstance(d, int) and (not d < 0)
-#         ), "The dimension d must be None or a positive integer"
-#         return (d is None) or (d > 0)
+    @classmethod
+    def is_dim_compatible(cls, d):
+        assert (d is None) or (
+            isinstance(d, int) and (not d < 0)
+        ), "The dimension d must be None or a positive integer"
+        return (d is None) or (d > 0)
 
-#     def _set_parameters(self):
-#         d = self.dimensionality
-#         self.input_domain = np.array([[-1, 1] for _ in range(d)])
+    def _set_parameters(self):
+        d = self.dimensionality
+        self.input_domain = np.array([[-1, 1] for _ in range(d)])
 
-#     def get_param(self):
-#         return {}
+    def get_param(self):
+        return {}
 
-#     def get_global_minimum(self, d):
-#         X = np.array([0 for _ in range(d)])
-#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+    def get_global_minimum(self, d):
+        X = np.array([0 for _ in range(d)])
+        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-#     def evaluate(self, X):
-#         d = X.shape[0]
-#         res = -np.exp(-0.5 * np.sum(X**2))
-#         return res
+    def evaluate(self, X):
+        d = X.shape[0]
+        res = -np.exp(-0.5 * np.sum(X**2))
+        return res
 
 
 class GoldsteinPrice(PyBenchFunction):
     """.. image:: ../img/functions/GoldsteinPrice.png"""
 
     name = "Goldstein-Price"
     continuous = True
@@ -1326,15 +1329,17 @@
             [[3, 5], [5, 2], [2, 1], [1, 4], [7, 9]])
 
     def get_param(self):
         return {"m": self.m, "c": self.c, "A": self.A}
 
     def get_global_minimum(self, d):
         X = np.array([0 for _ in range(d)])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+        # Global minimum is not known but the following is definitely smaller than the global minimum
+        Y = np.array([[-4.5]])
+        return (self._retrieve_original_input(X), Y)
 
     def evaluate(self, X):
         d = X.shape[0]
         res = np.sum(
             [
                 self.c[i] * np.exp(-1 / np.pi * np.sum(
                     (X - self.A[i]) ** 2)) * np.cos(
@@ -1559,16 +1564,18 @@
         self.m = m
 
     def get_param(self):
         return {"m": self.m}
 
     def get_global_minimum(self, d):
         if d != 2:  # Michalewicz minimum is only given for d=2
-            return (None, None)
+            Y = np.array([[4.49903414e-04*(d**2) - 2.15704771e-01*d - 4.85292809e+00]])  # Calculated with polyfit
+            return (None, Y)  # Substituted minimum for d=2
         X = np.array([2.20, 1.57])
+        Y = np.array([[-1.8013]])
         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
     def evaluate(self, X):
         d = X.shape[0]
         i = np.arange(1, d + 1)
         res = -np.sum(np.sin(X) * np.sin(i * X**2 / np.pi) ** (2 * self.m))
         return res
@@ -1606,94 +1613,94 @@
 
     def evaluate(self, X):
         d = X.shape[0]
         res = 1 + np.sum(np.sin(X) ** 2) - 0.1 * np.exp(-np.sum(X**2))
         return res
 
 
-class PermZeroDBeta(PyBenchFunction):
-    """.. image:: ../img/functions/PermZeroDBeta.png"""
+# class PermZeroDBeta(PyBenchFunction):
+#     """.. image:: ../img/functions/PermZeroDBeta.png"""
 
-    name = "Perm 0, d, beta"
-    continuous = True
-    convex = True
-    separable = False
-    differentiable = True
-    multimodal = False
-    randomized_term = False
-    parametric = True
+#     name = "Perm 0, d, beta"
+#     continuous = True
+#     convex = True
+#     separable = False
+#     differentiable = True
+#     multimodal = False
+#     randomized_term = False
+#     parametric = True
 
-    @classmethod
-    def is_dim_compatible(cls, d):
-        assert (d is None) or (
-            isinstance(d, int) and (not d < 0)
-        ), "The dimension d must be None or a positive integer"
-        return (d is None) or (d > 0)
+#     @classmethod
+#     def is_dim_compatible(cls, d):
+#         assert (d is None) or (
+#             isinstance(d, int) and (not d < 0)
+#         ), "The dimension d must be None or a positive integer"
+#         return (d is None) or (d > 0)
 
-    def _set_parameters(self, beta=10):
-        d = self.dimensionality
-        self.input_domain = np.array([[-d, d] for _ in range(d)])
-        self.beta = beta
+#     def _set_parameters(self, beta=10):
+#         d = self.dimensionality
+#         self.input_domain = np.array([[-d, d] for _ in range(d)])
+#         self.beta = beta
 
-    def get_param(self):
-        return {"beta": self.beta}
+#     def get_param(self):
+#         return {"beta": self.beta}
 
-    def get_global_minimum(self, d):
-        X = np.array([1 / (i + 1) for i in range(d)])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+#     def get_global_minimum(self, d):
+#         X = np.array([1 / (i + 1) for i in range(d)])
+#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-    def evaluate(self, X):
-        d = X.shape[0]
-        res = np.sum(
-            [
-                (np.sum([((j + 1) + self.beta * (X[j] ** (i + 1) - j ** (i + 1)))
-                 for j in range(d)])) ** 2
-                for i in range(d)
-            ]
-        )
-        return res
+#     def evaluate(self, X):
+#         d = X.shape[0]
+#         res = np.sum(
+#             [
+#                 (np.sum([((j + 1) + self.beta * (X[j] ** (i + 1) - j ** (i + 1)))
+#                  for j in range(d)])) ** 2
+#                 for i in range(d)
+#             ]
+#         )
+#         return res
 
 
-class PermDBeta(PyBenchFunction):
-    """.. image:: ../img/functions/PermDBeta.png"""
+# class PermDBeta(PyBenchFunction):
+#     """.. image:: ../img/functions/PermDBeta.png"""
 
-    name = "Perm d, beta"
-    continuous = True
-    convex = False
-    separable = False
-    differentiable = True
-    multimodal = True
-    randomized_term = False
-    parametric = True
+#     name = "Perm d, beta"
+#     continuous = True
+#     convex = False
+#     separable = False
+#     differentiable = True
+#     multimodal = True
+#     randomized_term = False
+#     parametric = True
 
-    @classmethod
-    def is_dim_compatible(cls, d):
-        assert (d is None) or (
-            isinstance(d, int) and (not d < 0)
-        ), "The dimension d must be None or a positive integer"
-        return (d is None) or (d > 0)
+#     @classmethod
+#     def is_dim_compatible(cls, d):
+#         assert (d is None) or (
+#             isinstance(d, int) and (not d < 0)
+#         ), "The dimension d must be None or a positive integer"
+#         return (d is None) or (d > 0)
 
-    def _set_parameters(self, beta=0.5):
-        d = self.dimensionality
-        self.input_domain = np.array([[-d, d] for _ in range(d)])
-        self.beta = beta
+#     def _set_parameters(self, beta=0.5):
+#         d = self.dimensionality
+#         self.input_domain = np.array([[-d, d] for _ in range(d)])
+#         self.beta = beta
 
-    def get_param(self):
-        return {"beta": self.beta}
+#     def get_param(self):
+#         return {"beta": self.beta}
 
-    def get_global_minimum(self, d):
-        X = np.array([1 / (i + 1) for i in range(d)])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+#     def get_global_minimum(self, d):
+#         X = np.array([1 / (i + 1) for i in range(d)])
+#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-    def evaluate(self, X):
-        d = X.shape[0]
-        j = np.arange(1, d + 1)
-        res = np.sum([np.sum((j**i + self.beta) * (
-            (X / j) ** i - 1)) ** 2 for i in range(1, d + 1)])
-        return res
+#     def evaluate(self, X):
+#         d = X.shape[0]
+#         j = np.arange(1, d + 1)
+#         res = np.sum([np.sum((j**i + self.beta) * (
+#             (X / j) ** i - 1)) ** 2 for i in range(1, d + 1)])
+#         return res
 
 
 class Powell(PyBenchFunction):
     """.. image:: ../img/functions/Powell.png"""
 
     name = "Powell"
     continuous = True
@@ -1797,15 +1804,16 @@
         self.input_domain = np.array([[-1.28, 1.28] for _ in range(d)])
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
         X = np.array([0 for _ in range(d)])
-        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+        Y = np.array([[0.0]])  # Global minimum value without the randomized term
+        return (self._retrieve_original_input(X), Y)
 
     def evaluate(self, X):
         d = X.shape[0]
         res = np.sum(np.arange(1, d + 1) * X**4) + np.random.random()
         return res
 
 
@@ -2260,50 +2268,50 @@
 
     def evaluate(self, X):
         d = X.shape[0]
         res = np.max(np.abs(X))
         return res
 
 
-# class Schwefel2_22(PyBenchFunction):
-#     """.. image:: ../img/functions/Schwefel2_22.png"""
+class Schwefel2_22(PyBenchFunction):
+    """.. image:: ../img/functions/Schwefel2_22.png"""
 
-#     name = "Schwefel 2.22"
-#     continuous = True
-#     convex = True
-#     separable = True
-#     differentiable = False
-#     multimodal = False
-#     randomized_term = False
-#     parametric = False
+    name = "Schwefel 2.22"
+    continuous = True
+    convex = True
+    separable = True
+    differentiable = False
+    multimodal = False
+    randomized_term = False
+    parametric = False
 
-#     @classmethod
-#     def is_dim_compatible(cls, d):
-#         assert (d is None) or (
-#             isinstance(d, int) and (not d < 0)
-#         ), "The dimension d must be None or a positive integer"
-#         return (d is None) or (d > 0)
+    @classmethod
+    def is_dim_compatible(cls, d):
+        assert (d is None) or (
+            isinstance(d, int) and (not d < 0)
+        ), "The dimension d must be None or a positive integer"
+        return (d is None) or (d > 0)
 
-#     def _set_parameters(
-#         self,
-#     ):
-#         d = self.dimensionality
-#         self.input_domain = np.array([[-100, 100] for _ in range(d)])
+    def _set_parameters(
+        self,
+    ):
+        d = self.dimensionality
+        self.input_domain = np.array([[-100, 100] for _ in range(d)])
 
-#     def get_param(self):
-#         return {}
+    def get_param(self):
+        return {}
 
-#     def get_global_minimum(self, d):
-#         X = np.array([0 for _ in range(d)])
-#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+    def get_global_minimum(self, d):
+        X = np.array([0 for _ in range(d)])
+        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-#     def evaluate(self, X):
-#         d = X.shape[0]
-#         res = np.sum(np.abs(X)) + np.prod(np.abs(X))
-#         return res
+    def evaluate(self, X):
+        d = X.shape[0]
+        res = np.sum(np.abs(X)) + np.prod(np.abs(X))
+        return res
 
 
 class Schwefel2_23(PyBenchFunction):
     """.. image:: ../img/functions/Schwefel2_23.png"""
 
     name = "Schwefel 2.23"
     continuous = True
@@ -2336,68 +2344,68 @@
 
     def evaluate(self, X):
         d = X.shape[0]
         res = np.sum(X**10)
         return res
 
 
-# class Shekel(PyBenchFunction):
-#     """.. image:: ../img/functions/Shekel.png"""
+class Shekel(PyBenchFunction):
+    """.. image:: ../img/functions/Shekel.png"""
 
-#     name = "Shekel"
-#     continuous = True
-#     convex = False
-#     separable = False
-#     differentiable = True
-#     multimodal = True
-#     randomized_term = False
-#     parametric = True
+    name = "Shekel"
+    continuous = True
+    convex = False
+    separable = False
+    differentiable = True
+    multimodal = True
+    randomized_term = False
+    parametric = True
 
-#     @classmethod
-#     def is_dim_compatible(cls, d):
-#         assert (d is None) or (
-#             isinstance(d, int) and (not d < 0)
-#         ), "The dimension d must be None or a positive integer"
-#         return d == 4
+    @classmethod
+    def is_dim_compatible(cls, d):
+        assert (d is None) or (
+            isinstance(d, int) and (not d < 0)
+        ), "The dimension d must be None or a positive integer"
+        return d == 4
 
-#     def _set_parameters(self, m=None, C=None, beta=None):
-#         d = self.dimensionality
-#         self.input_domain = np.array([[-10, 10], [-10, 10], [-10, 10], [-10, 10]])
-#         self.m = m if m is not None else 10
-#         self.beta = beta if beta is not None else 1 / 10 * np.array([1, 2, 2, 4, 4, 6, 3, 7, 5, 5])
-#         self.C = (
-#             C
-#             if C is not None
-#             else np.array(
-#                 [
-#                     [4, 4, 4, 4],
-#                     [1, 1, 1, 1],
-#                     [8, 8, 8, 8],
-#                     [6, 6, 6, 6],
-#                     [3, 7, 3, 7],
-#                     [2, 9, 2, 9],
-#                     [5, 3, 5, 3],
-#                     [8, 1, 8, 1],
-#                     [6, 2, 6, 2],
-#                     [7, 3.6, 7, 3.6],
-#                 ]
-#             )
-#         )
+    def _set_parameters(self, m=None, C=None, beta=None):
+        d = self.dimensionality
+        self.input_domain = np.array([[-10, 10], [-10, 10], [-10, 10], [-10, 10]])
+        self.m = m if m is not None else 10
+        self.beta = beta if beta is not None else 1 / 10 * np.array([1, 2, 2, 4, 4, 6, 3, 7, 5, 5])
+        self.C = (
+            C
+            if C is not None
+            else np.array(
+                [
+                    [4, 4, 4, 4],
+                    [1, 1, 1, 1],
+                    [8, 8, 8, 8],
+                    [6, 6, 6, 6],
+                    [3, 7, 3, 7],
+                    [2, 9, 2, 9],
+                    [5, 3, 5, 3],
+                    [8, 1, 8, 1],
+                    [6, 2, 6, 2],
+                    [7, 3.6, 7, 3.6],
+                ]
+            )
+        )
 
-#     def get_param(self):
-#         return {"m": self.m, "C": self.C, "beta": self.beta}
+    def get_param(self):
+        return {"m": self.m, "C": self.C, "beta": self.beta}
 
-#     def get_global_minimum(self, d):
-#         X = self.C[0]
-#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+    def get_global_minimum(self, d):
+        X = self.C[0]
+        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-#     def evaluate(self, X):
-#         x1, x2, x3, x4 = X
-#         res = -np.sum([[np.sum((X - self.C[i]) ** 2 + self.beta[i]) ** -1] for i in range(self.m)])
-#         return res
+    def evaluate(self, X):
+        x1, x2, x3, x4 = X
+        res = -np.sum([[np.sum((X - self.C[i]) ** 2 + self.beta[i]) ** -1] for i in range(self.m)])
+        return res
 
 
 class Shubert(PyBenchFunction):
     """.. image:: ../img/functions/Shubert.png"""
 
     name = "Shubert"
     continuous = True
@@ -2423,15 +2431,16 @@
 
     def get_param(self):
         return {}
 
     def get_global_minimum(self, d):
         # Global minimum from https://documentation.sas.com/doc/en/orcdc/14.2/orlsoug/orlsoug_ga_gettingstarted09.htm"
         # X = np.array([-7.708309818, -0.800371886])
-        return (None, None)
+        # Has 18 global minima around -186.7309
+        return (None, np.array([[-186.7309]]))
 
     def evaluate(self, X):
         d = X.shape[0]
         for i in range(0, d):
             res = np.prod(np.sum([i * np.cos((j + 1) * X[i] + j)
                           for j in range(1, 5 + 1)]))
         return res
@@ -2698,48 +2707,48 @@
     def evaluate(self, X):
         d = X.shape[0]
         i = np.arange(1, d + 1)
         res = np.sum((X - 1) ** 2) - np.sum(X[1:] * X[:-1])
         return res
 
 
-# class Wolfe(PyBenchFunction):
-#     """.. image:: ../img/functions/Wolfe.png"""
+class Wolfe(PyBenchFunction):
+    """.. image:: ../img/functions/Wolfe.png"""
 
-#     name = "Wolfe"
-#     continuous = True
-#     convex = False
-#     separable = False
-#     differentiable = True
-#     multimodal = True
-#     randomized_term = False
-#     parametric = False
+    name = "Wolfe"
+    continuous = True
+    convex = False
+    separable = False
+    differentiable = True
+    multimodal = True
+    randomized_term = False
+    parametric = False
 
-#     @classmethod
-#     def is_dim_compatible(cls, d):
-#         assert (d is None) or (
-#             isinstance(d, int) and (not d < 0)
-#         ), "The dimension d must be None or a positive integer"
-#         return d == 3
+    @classmethod
+    def is_dim_compatible(cls, d):
+        assert (d is None) or (
+            isinstance(d, int) and (not d < 0)
+        ), "The dimension d must be None or a positive integer"
+        return d == 3
 
-#     def _set_parameters(self):
-#         d = self.dimensionality
-#         self.input_domain = np.array([[0, 2], [0, 2], [0, 2]])
+    def _set_parameters(self):
+        d = self.dimensionality
+        self.input_domain = np.array([[0, 2], [0, 2], [0, 2]])
 
-#     def get_param(self):
-#         return {}
+    def get_param(self):
+        return {}
 
-#     def get_global_minimum(self, d):
-#         X = np.array([0, 0, 0])
-#         return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
+    def get_global_minimum(self, d):
+        X = np.array([0, 0, 0])
+        return (self._retrieve_original_input(X), self(self._retrieve_original_input(X)))
 
-#     def evaluate(self, X):
-#         x, y, z = X
-#         res = 4 / 3 * (x**2 + y**2 - x * y) ** 0.75 + z
-#         return res
+    def evaluate(self, X):
+        x, y, z = X
+        res = (4 / 3) * (x**2 + y**2 - x * y) ** 0.75 + z
+        return res
 
 
 class XinSheYang(PyBenchFunction):
     """.. image:: ../img/functions/XinSheYang.png"""
 
     name = "Xin She Yang"
     continuous = True
```

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/__init__.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 from os import path
 from typing import TYPE_CHECKING
 
 # Local
 from .._imports import _IntegrationModule
 
 if TYPE_CHECKING:
+    from .evaluator import Evaluator
     from .linear_regression import LinearRegression
+    from .mnist_classifier import MNISTClassifier
     from .model import Model
     from .passthrough_model import PassthroughModel
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
@@ -25,14 +27,15 @@
 # =============================================================================
 
 _import_structure: dict = {
     "utils": ["find_model", "create_model_from_json", "create_model_from_dict", "MeanSquaredError"],
     "model": ["Model"],
     "linear_regression": ["LinearRegression"],
     "passthrough_model": ["PassthroughModel"],
+    "mnist_classifier": ["MNISTClassifier"],
     "evaluator": ["Evaluator"],
     "all_models": ["MODELS"],
     "loss_functions": ["MeanSquaredError"],
 }
 
 if not TYPE_CHECKING:
     class _LocalIntegrationModule(_IntegrationModule):
```

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/adapters/tensorflow_implementations.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/adapters/tensorflow_implementations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-from typing import List
+from typing import List, Tuple
 from unittest import mock
 
 # Third-party core
 import numpy as np
 
 # Local
 from ..._imports import try_import
@@ -46,32 +46,46 @@
 
     def get_model_weights(self) -> List[np.ndarray]:
         return get_flat_array_from_list_of_arrays(self.model.get_weights())
         # return self.model.get_weights()
 
     def set_model_weights(self, weights: np.ndarray):
         reshaped_weights = get_reshaped_array_from_list_of_arrays(
-            flat_array=weights.ravel(), list_of_arrays=self.model.get_weights())
+            flat_array=weights.ravel(), shapes=[w.shape for w in self.model.get_weights()])
         self.model.set_weights(reshaped_weights)
 
 
-
-def get_reshaped_array_from_list_of_arrays(flat_array: np.ndarray,
-                                           list_of_arrays: List[np.ndarray]) -> List[np.ndarray]:
-    total_array = []
+def get_reshaped_array_from_list_of_arrays(flat_array: np.ndarray, shapes: List[Tuple[int, int]]):
+    # Initialize list of unflattened arrays
+    unflattened_arrays = []
     index = 0
-    for mimic_array in list_of_arrays:
-        number_of_values = np.product(mimic_array.shape)
-        current_array = np.array(flat_array[index:index+number_of_values])
 
-        if number_of_values > 1:
-            current_array = current_array.reshape(-1, 1)  # Make 2D array
+    # Iterate over shapes and reconstruct arrays
+    for shape in shapes:
+        size = np.prod(shape)
+        arr = flat_array[index:index+size].reshape(shape)
+        unflattened_arrays.append(arr)
+        index += size
+
+    return unflattened_arrays
+
+
+# def get_reshaped_array_from_list_of_arrays(flat_array: np.ndarray,
+#                                            list_of_arrays: List[np.ndarray]) -> List[np.ndarray]:
+#     total_array = []
+#     index = 0
+#     for mimic_array in list_of_arrays:
+#         number_of_values = np.product(mimic_array.shape)
+#         current_array = np.array(flat_array[index:index+number_of_values])
+
+#         if number_of_values > 1:
+#             current_array = current_array.reshape(-1, 1)  # Make 2D array
 
-        total_array.append(current_array)
-        index += number_of_values
+#         total_array.append(current_array)
+#         index += number_of_values
 
-    return total_array
+#     return total_array
 
 
 # technically not a np array input!
 def get_flat_array_from_list_of_arrays(list_of_arrays: List[np.ndarray]) -> np.ndarray:
-    return np.concatenate([np.atleast_2d(array) for array in list_of_arrays])
+    return np.concatenate([array.flatten() for array in list_of_arrays])
```

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/all_models.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/all_models.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/evaluator.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/evaluator.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/linear_regression.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/linear_regression.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/loss_functions.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/loss_functions.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/model.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-from typing import Protocol
+# Standard
+try:
+    from typing import Protocol
+except ImportError:  # Python 3.7
+    from typing_extensions import Protocol
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling', 'https://d2l.ai/']
 __status__ = 'Alpha'
 # =============================================================================
```

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/passthrough_model.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/passthrough_model.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/machinelearning/utils.py` & `f3dasm-1.1.0/src/f3dasm/machinelearning/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/__init__.py` & `f3dasm-1.1.0/src/f3dasm/optimization/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/_protocol.py` & `f3dasm-1.1.0/src/f3dasm/optimization/_protocol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """
 Protocol classes from types outside the optimization submodule
 """
 #                                                                       Modules
 # =============================================================================
 
 # Standard
-from typing import Protocol
+try:
+    from typing import Protocol
+except ImportError:  # Python 3.7
+    from typing_extensions import Protocol
 
 # Third-party core
 import numpy as np
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
```

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/adam.py` & `f3dasm-1.1.0/src/f3dasm/optimization/adam.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/adamax.py` & `f3dasm-1.1.0/src/f3dasm/optimization/adamax.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/adapters/pygmo_implementations.py` & `f3dasm-1.1.0/src/f3dasm/optimization/adapters/pygmo_implementations.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from typing import Any, List, Tuple
 
 # Third-party core
 import autograd.numpy as np
 
 # Locals
 from ..._imports import try_import
-from .._protocol import DesignSpace, Function
+from ...design import DesignSpace
+from ...functions import Function
 from ..optimizer import Optimizer
 
 # Third-party extension
 with try_import('optimization') as _imports:
     import pygmo as pg
 
 #                                                          Authorship & Credits
@@ -82,16 +83,16 @@
         """Box-constrained boundaries of the problem. Necessary for pygmo library
 
         Returns
         -------
             box constraints
         """
         return (
-            [parameter.lower_bound for parameter in self.design.get_continuous_input_parameters()],
-            [parameter.upper_bound for parameter in self.design.get_continuous_input_parameters()],
+            [parameter.lower_bound for parameter in self.design.get_continuous_input_parameters().values()],
+            [parameter.upper_bound for parameter in self.design.get_continuous_input_parameters().values()],
         )
 
     def gradient(self, x: np.ndarray):
         """Gradient in pygmo accepted format
 
         Parameters
         ----------
```

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/adapters/scipy_implementations.py` & `f3dasm-1.1.0/src/f3dasm/optimization/adapters/scipy_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/adapters/tensorflow_implementations.py` & `f3dasm-1.1.0/src/f3dasm/optimization/adapters/tensorflow_implementations.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/all_optimizers.py` & `f3dasm-1.1.0/src/f3dasm/optimization/all_optimizers.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 from typing import List
 
+from .._imports import try_import
 from . import (adam, adamax, bayesianoptimization, cg, cmaes,
                differentialevolution, ftrl, lbfgsb, nadam, neldermead,
                optimizer, pso, randomsearch, rmsprop, sade, sea, sga, sgd,
                simulatedannealing, xnes)
 # Locals
 from .optimizer import Optimizer
 
@@ -25,53 +26,61 @@
 
 # Core models
 OPTIMIZERS.append(randomsearch.RandomSearch)
 OPTIMIZERS.append(cg.CG)
 OPTIMIZERS.append(lbfgsb.LBFGSB)
 OPTIMIZERS.append(neldermead.NelderMead)
 
-# Extension samplers
-if adam._imports.is_successful():
-    OPTIMIZERS.append(adam.Adam)
 
-if adamax._imports.is_successful():
-    OPTIMIZERS.append(adamax.Adamax)
+# WIP: Import from f3dasm_optimize package
+with try_import('f3dasm_optimize') as _imports:
+    import f3dasm_optimize
 
-# COMMENT THIS BECAUSE BAYESIAN OPTIMIZATION IS TOO SLOW TO TEST PROPERLY NOW
-# if bayesianoptimization._imports.is_successful():
-#     OPTIMIZERS.append(bayesianoptimization.BayesianOptimization)
+if _imports.is_successful():
+    OPTIMIZERS.extend(f3dasm_optimize.OPTIMIZERS)
 
-if cmaes._imports.is_successful():
-    OPTIMIZERS.append(cmaes.CMAES)
+# # Extension samplers
+# if adam._imports.is_successful():
+#     OPTIMIZERS.append(adam.Adam)
 
-if differentialevolution._imports.is_successful():
-    OPTIMIZERS.append(differentialevolution.DifferentialEvolution)
+# if adamax._imports.is_successful():
+#     OPTIMIZERS.append(adamax.Adamax)
 
-if ftrl._imports.is_successful():
-    OPTIMIZERS.append(ftrl.Ftrl)
+# # COMMENT THIS BECAUSE BAYESIAN OPTIMIZATION IS TOO SLOW TO TEST PROPERLY NOW
+# # if bayesianoptimization._imports.is_successful():
+# #     OPTIMIZERS.append(bayesianoptimization.BayesianOptimization)
 
-if nadam._imports.is_successful():
-    OPTIMIZERS.append(nadam.Nadam)
+# if cmaes._imports.is_successful():
+#     OPTIMIZERS.append(cmaes.CMAES)
 
-if pso._imports.is_successful():
-    OPTIMIZERS.append(pso.PSO)
+# if differentialevolution._imports.is_successful():
+#     OPTIMIZERS.append(differentialevolution.DifferentialEvolution)
 
-if rmsprop._imports.is_successful():
-    OPTIMIZERS.append(rmsprop.RMSprop)
+# if ftrl._imports.is_successful():
+#     OPTIMIZERS.append(ftrl.Ftrl)
 
-if sade._imports.is_successful():
-    OPTIMIZERS.append(sade.SADE)
+# if nadam._imports.is_successful():
+#     OPTIMIZERS.append(nadam.Nadam)
 
-if sea._imports.is_successful():
-    OPTIMIZERS.append(sea.SEA)
+# if pso._imports.is_successful():
+#     OPTIMIZERS.append(pso.PSO)
 
-if sga._imports.is_successful():
-    OPTIMIZERS.append(sga.SGA)
+# if rmsprop._imports.is_successful():
+#     OPTIMIZERS.append(rmsprop.RMSprop)
 
-if sgd._imports.is_successful():
-    OPTIMIZERS.append(sgd.SGD)
+# if sade._imports.is_successful():
+#     OPTIMIZERS.append(sade.SADE)
 
-if simulatedannealing._imports.is_successful():
-    OPTIMIZERS.append(simulatedannealing.SimulatedAnnealing)
+# if sea._imports.is_successful():
+#     OPTIMIZERS.append(sea.SEA)
+
+# if sga._imports.is_successful():
+#     OPTIMIZERS.append(sga.SGA)
+
+# if sgd._imports.is_successful():
+#     OPTIMIZERS.append(sgd.SGD)
+
+# if simulatedannealing._imports.is_successful():
+#     OPTIMIZERS.append(simulatedannealing.SimulatedAnnealing)
 
 if xnes._imports.is_successful():
     OPTIMIZERS.append(xnes.XNES)
```

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/bayesianoptimization.py` & `f3dasm-1.1.0/src/f3dasm/optimization/bayesianoptimization.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/cg.py` & `f3dasm-1.1.0/src/f3dasm/optimization/cg.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/cmaes.py` & `f3dasm-1.1.0/src/f3dasm/optimization/cmaes.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/cobyla.py` & `f3dasm-1.1.0/src/f3dasm/optimization/cobyla.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/differentialevolution.py` & `f3dasm-1.1.0/src/f3dasm/optimization/differentialevolution.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/ftrl.py` & `f3dasm-1.1.0/src/f3dasm/optimization/ftrl.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/lbfgsb.py` & `f3dasm-1.1.0/src/f3dasm/optimization/lbfgsb.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/nadam.py` & `f3dasm-1.1.0/src/f3dasm/optimization/nadam.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/neldermead.py` & `f3dasm-1.1.0/src/f3dasm/optimization/neldermead.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/optimizer.py` & `f3dasm-1.1.0/src/f3dasm/optimization/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 import json
-from copy import copy
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Any, List, Mapping, Optional, Tuple
 
 # Third-party core
 import numpy as np
 
 # Locals
@@ -50,31 +50,38 @@
         Data-object
     hyperparameters : dict
         Dictionary with hyperparameteres
     seed : int
         seed to set the optimizer
     defaults : OptimizerParameters
         Default hyperparameter arguments
+    name : str
+        Name of the optimizer object. Default to classname. Optional.
 
     Raises
     ------
     NotImplementedError
         When no update step is implemented
     ValueError
         When number of datapoints is lower than the population
     """
 
     data: ExperimentData
     hyperparameters: Optional[Mapping[str, Any]] = field(default_factory=dict)
     seed: int = np.random.randint(low=0, high=1e5)
     algorithm: Any = field(init=False)
     parameter: OptimizerParameters = field(init=False)
+    name: str = None
 
     def __post_init__(self):
         self._check_imports()
+
+        if self.name is None:
+            self.name = self.__class__.__name__
+
         if self.seed:
             self.set_seed(self.seed)
 
         self.init_parameters()
         self._set_hyperparameters()
         self.set_algorithm()
 
@@ -228,24 +235,24 @@
     def extract_data(self) -> ExperimentData:
         """Returns a copy of the data
 
         Returns
         -------
             copy of the data
         """
-        return copy(self.data)
+        return deepcopy(self.data)
 
     def get_name(self) -> str:
         """Retrieve the name of the optimizers
 
         Returns
         -------
             name of the optimizer
         """
-        return self.__class__.__name__
+        return self.name
 
     def get_info(self) -> List[str]:
         """Give a list of characteristic features of this optimizer
 
         Returns
         -------
             List of strings denoting the characteristics of this optimizer
```

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/pso.py` & `f3dasm-1.1.0/src/f3dasm/optimization/pso.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/randomsearch.py` & `f3dasm-1.1.0/src/f3dasm/optimization/randomsearch.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/rmsprop.py` & `f3dasm-1.1.0/src/f3dasm/optimization/rmsprop.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/sade.py` & `f3dasm-1.1.0/src/f3dasm/optimization/sade.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/sea.py` & `f3dasm-1.1.0/src/f3dasm/optimization/sea.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/sga.py` & `f3dasm-1.1.0/src/f3dasm/optimization/sga.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/sgd.py` & `f3dasm-1.1.0/src/f3dasm/optimization/sgd.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/simulatedannealing.py` & `f3dasm-1.1.0/src/f3dasm/optimization/simulatedannealing.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/utils.py` & `f3dasm-1.1.0/src/f3dasm/optimization/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 import json
 
 # Local
+from ..design.experimentdata import ExperimentData
 from ..optimization.all_optimizers import OPTIMIZERS
 from ..optimization.optimizer import Optimizer
-from ..design import create_experimentdata_from_json
-
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
 __status__ = 'Stable'
 # =============================================================================
@@ -64,9 +63,9 @@
     name
         name of the class
 
     Returns
     -------
         Requested Optimizer object
     """
-    optimizer_dict['data'] = create_experimentdata_from_json(optimizer_dict['data'])
+    optimizer_dict['data'] = ExperimentData.from_json(optimizer_dict['data'])
     return find_optimizer(name)(**optimizer_dict)
```

### Comparing `f3dasm-0.9.3/src/f3dasm/optimization/xnes.py` & `f3dasm-1.1.0/src/f3dasm/optimization/xnes.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/run_optimization.py` & `f3dasm-1.1.0/src/f3dasm/run_optimization.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 Module to optimize benchmark optimization functions
 """
 #                                                                       Modules
 # =============================================================================
 
 # Standard
 import json
-import logging
 import time
-from typing import Any, List
+from typing import Any, List, Type
 
 # Third-party
 import numpy as np
 import pandas as pd
 from pathos.helpers import mp
 
-from f3dasm.optimization import Optimizer, create_optimizer_from_json
+from f3dasm.optimization import Optimizer, find_optimizer
 from f3dasm.sampling import Sampler, create_sampler_from_json
 
+from ._logging import logger, time_and_log
 # Locals
-from .design import ExperimentData, create_experimentdata_from_json
+from .design import ExperimentData
 from .functions import create_function_from_json
 from .functions.function import Function
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
@@ -57,52 +57,52 @@
         self.optimizer = optimizer
         self.function = function
         self.sampler = sampler
         self.number_of_samples = number_of_samples
         self.seeds = seeds
         self._log()
 
+    @classmethod
+    def from_json(cls: Type['OptimizationResult'], json_string: str) -> 'OptimizationResult':
+        optimizationresult_dict = json.loads(json_string)
+        return cls.from_dict(optimizationresult_dict)
+
+    @classmethod
+    def from_dict(cls: Type['OptimizationResult'], optimizationresult_dict: dict) -> 'OptimizationResult':
+        args = {
+            'data': [ExperimentData.from_json(json_data) for json_data in optimizationresult_dict['data']],
+            # 'optimizer': create_optimizer_from_json(optimizationresult_dict['optimizer']),
+            'function': create_function_from_json(optimizationresult_dict['function']),
+            'sampler': create_sampler_from_json(optimizationresult_dict['sampler']),
+            'number_of_samples': optimizationresult_dict['number_of_samples'],
+            'seeds': optimizationresult_dict['seeds'],
+        }
+        return cls(**args)
+
     def to_json(self):
         args = {'data': [d.to_json() for d in self.data],
                 'optimizer': self.optimizer.to_json(),
                 'function': self.function.to_json(),
                 'sampler': self.sampler.to_json(),
                 'number_of_samples': self.number_of_samples,
                 'seeds': self.seeds
                 }
 
         return json.dumps(args)
 
     def _log(self):
         # Log
-        logging.info(
+        logger.info(
             (f"Optimized {self.function.get_name()} function (seed={self.function.seed}, "
              f"dim={self.function.dimensionality}, "
              f"with {self.optimizer.get_name()} optimizer for "
              f"{len(self.data)} realizations!")
         )
 
 
-def create_optimizationresult_from_json(json_string: str) -> OptimizationResult:
-    optimizationresult_dict = json.loads(json_string)
-    return _create_optimizationresult_from_dict(optimizationresult_dict)
-
-
-def _create_optimizationresult_from_dict(optimizationresult_dict: dict) -> OptimizationResult:
-    args = {
-        'data': [create_experimentdata_from_json(json_data) for json_data in optimizationresult_dict['data']],
-        'optimizer': create_optimizer_from_json(optimizationresult_dict['optimizer']),
-        'function': create_function_from_json(optimizationresult_dict['function']),
-        'sampler': create_sampler_from_json(optimizationresult_dict['sampler']),
-        'number_of_samples': optimizationresult_dict['number_of_samples'],
-        'seeds': optimizationresult_dict['seeds'],
-    }
-    return OptimizationResult(**args)
-
-
 def run_optimization(
     optimizer: Optimizer,
     function: Function,
     sampler: Sampler,
     iterations: int,
     seed: int,
     number_of_samples: int = 30,
@@ -150,14 +150,15 @@
 
     # Reset data
     optimizer.data.reset_data()
 
     return res
 
 
+@time_and_log
 def run_multiple_realizations(
     optimizer: Optimizer,
     function: Function,
     sampler: Sampler,
     iterations: int,
     realizations: int,
     number_of_samples: int = 30,
@@ -188,16 +189,14 @@
     seed, optional
         seed for the random number generator
 
     Returns
     -------
         Object with the optimization data results
     """
-    start_t = time.perf_counter()
-
     if seed is None:
         seed = np.random.randint(low=0, high=1e5)
 
     if parallelization:
         args = [
             (optimizer, function, sampler, iterations,
              seed + index, number_of_samples)
@@ -217,20 +216,14 @@
                 "sampler": sampler,
                 "iterations": iterations,
                 "number_of_samples": number_of_samples,
                 "seed": seed + index,
             }
             results.append(run_optimization(**args))
 
-    end_t = time.perf_counter()
-
-    total_duration = end_t - start_t
-    if verbal:
-        print(f"Optimization took {total_duration:.2f}s total")
-
     return OptimizationResult(
         data=results,
         optimizer=optimizer,
         function=function,
         sampler=sampler,
         number_of_samples=number_of_samples,
         seeds=[seed + i for i in range(realizations)],
```

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/__init__.py` & `f3dasm-1.1.0/src/f3dasm/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/all_samplers.py` & `f3dasm-1.1.0/src/f3dasm/sampling/all_samplers.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/latinhypercube.py` & `f3dasm-1.1.0/src/f3dasm/sampling/latinhypercube.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,13 +45,13 @@
         Returns
         -------
             samples
         """
         continuous = self.design.get_continuous_input_parameters()
         problem = {
             "num_vars": len(continuous),
-            "names": [s.name for s in continuous],
-            "bounds": [[s.lower_bound, s.upper_bound] for s in continuous],
+            "names": list(continuous.keys()),
+            "bounds": [[s.lower_bound, s.upper_bound] for s in continuous.values()],
         }
 
         samples = latin.sample(problem, N=numsamples, seed=self.seed)
         return samples
```

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/randomuniform.py` & `f3dasm-1.1.0/src/f3dasm/sampling/randomuniform.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/sampler.py` & `f3dasm-1.1.0/src/f3dasm/sampling/sampler.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 # Standard
 import json
 from typing import Any, List, Union
 
 # Third-party core
 import numpy as np
 import pandas as pd
+from hydra.utils import instantiate
+from omegaconf import DictConfig, OmegaConf
 
 # Locals
 from ..design.design import DesignSpace
 from ..design.experimentdata import ExperimentData
 
 #                                                          Authorship & Credits
 # =============================================================================
@@ -30,26 +32,36 @@
     ----------
     design
         design of experiments object
     seed
         seed for sampling
     """
 
-    def __init__(self, design: DesignSpace, seed: Union[Any, int] = None):
+    def __init__(self, design: DesignSpace, seed: Union[Any, int] = None, number_of_samples: int = None):
         self.design = design
         self.seed = seed
+        self.number_of_samples = number_of_samples
         self.__post_init__()
 
     def __post_init__(self):
         if self.seed:
             np.random.seed(self.seed)
 
     def __eq__(self, __o: object) -> bool:
         return all((self.design == __o.design, self.seed == __o.seed))
 
+    @classmethod
+    def from_yaml(cls, config: DictConfig) -> 'Sampler':
+        """Create a sampler from a yaml configuration"""
+
+        args = {**config.sampler, 'design': None}
+        sampler: Sampler = instantiate(args)
+        sampler.design = DesignSpace.from_yaml(config.design)
+        return sampler
+
     def to_json(self):
         args = {'design': self.design.to_json(),
                 'seed': self.seed}
         name = self.__class__.__name__
         return json.dumps((args, name))
 
     def set_seed(self, seed: int):
@@ -73,26 +85,30 @@
 
         Returns
         -------
             samples
         """
         raise NotImplementedError("Subclasses should implement this method.")
 
-    def get_samples(self, numsamples: int) -> ExperimentData:
+    def get_samples(self, numsamples: Union[int, None] = None) -> ExperimentData:
         """Receive samples of the search space
 
         Parameters
         ----------
         numsamples
             number of samples
 
         Returns
         -------
             Data objects with the samples
         """
+        # If numsamples is None, take the object attribute number_of_samples
+        if numsamples is None:
+            numsamples = self.number_of_samples
+
         # First sample the continuous parameters
         samples_continuous = self.sample_continuous(numsamples=numsamples)
 
         # Sample discrete parameters
         samples_discrete = self._sample_discrete(numsamples=numsamples)
 
         # Sample categorical parameters
@@ -120,60 +136,60 @@
         return data
 
     def _cast_to_data_object(self, samples: np.ndarray, columnnames: List[str]) -> ExperimentData:
         """Cast the samples to a Data object"""
         data = ExperimentData(design=self.design)
 
         # First get an empty reference frame from the DoE
-        empty_frame = self.design.get_empty_dataframe()
+        empty_frame = self.design.create_empty_dataframe()
 
         # Then, create a new frame from the samples and columnnames
         samples_frame = pd.DataFrame(data=samples, columns=columnnames)
         df = pd.concat([empty_frame, samples_frame], sort=True)
 
         # Add the samples to the Data object
         data.add(data=df)
 
         return data
 
     def _sample_constant(self, numsamples: int):
         constant = self.design.get_constant_input_parameters()
         samples = np.empty(shape=(numsamples, len(constant)))
-        for dim, _ in enumerate(constant):
-            samples[:, dim] = constant[dim].value
+        for dim, param in enumerate(constant.values()):
+            samples[:, dim] = param.value
 
         return samples
 
     def _sample_discrete(self, numsamples: int):
         """Sample the descrete parameters, default randomly uniform"""
         discrete = self.design.get_discrete_input_parameters()
         samples = np.empty(shape=(numsamples, len(discrete)))
-        for dim, _ in enumerate(discrete):
+        for dim, param in enumerate(discrete.values()):
             samples[:, dim] = np.random.choice(
-                range(discrete[dim].lower_bound,
-                      discrete[dim].upper_bound + 1),
+                range(param.lower_bound,
+                      param.upper_bound + 1),
                 size=numsamples,
             )
 
         return samples
 
     def _sample_categorical(self, numsamples: int):
         """Sample the categorical parameters, default randomly uniform"""
         categorical = self.design.get_categorical_input_parameters()
         samples = np.empty(shape=(numsamples, len(categorical)), dtype=object)
-        for dim, _ in enumerate(categorical):
+        for dim, param in enumerate(categorical.values()):
             samples[:, dim] = np.random.choice(
-                categorical[dim].categories, size=numsamples)
+                param.categories, size=numsamples)
 
         return samples
 
     def _stretch_samples(self, samples: np.ndarray) -> np.ndarray:
         """Stretch samples to their boundaries"""
         continuous = self.design.get_continuous_input_parameters()
-        for dim, _ in enumerate(continuous):
+        for dim, param in enumerate(continuous.values()):
             samples[:, dim] = (
                 samples[:, dim] * (
-                    continuous[dim].upper_bound - continuous[dim].lower_bound
-                ) + continuous[dim].lower_bound
+                    param.upper_bound - param.lower_bound
+                ) + param.lower_bound
             )
 
         return samples
```

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/sobolsequence.py` & `f3dasm-1.1.0/src/f3dasm/sampling/sobolsequence.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/sampling/utils.py` & `f3dasm-1.1.0/src/f3dasm/sampling/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # =============================================================================
 
 # Standard
 import json
 from typing import List
 
 # Locals
-from ..design import create_design_from_json
+from ..design import DesignSpace
 from .all_samplers import SAMPLERS
 from .sampler import Sampler
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = 'Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)'
 __credits__ = ['Martin van der Schelling']
@@ -51,9 +51,9 @@
         Requested Sampler object
     """
     sampler_dict, name = json.loads(json_string)
     return _create_sampler_from_dict(sampler_dict, name)
 
 
 def _create_sampler_from_dict(sampler_dict: dict, name: str) -> Sampler:
-    sampler_dict['design'] = create_design_from_json(sampler_dict['design'])
+    sampler_dict['design'] = DesignSpace.from_json(sampler_dict['design'])
     return find_sampler(name)(**sampler_dict)
```

### Comparing `f3dasm-0.9.3/src/f3dasm/simulation/abaqus_script/flower_rve_script.py` & `f3dasm-1.1.0/src/f3dasm/simulation/abaqus_script/flower_rve_script.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/simulation/abaqus_simulator.py` & `f3dasm-1.1.0/src/f3dasm/simulation/abaqus_simulator.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/simulation/abaqus_utils.py` & `f3dasm-1.1.0/src/f3dasm/simulation/abaqus_utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/simulation/cases/flower_rve.py` & `f3dasm-1.1.0/src/f3dasm/simulation/cases/flower_rve.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm/simulation/simulator.py` & `f3dasm-1.1.0/src/f3dasm/simulation/simulator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 #                                                                       Modules
 # =============================================================================
 
-# Third-party
-import numpy as np
+from .._logging import logger, time_and_log
 
 #                                                          Authorship & Credits
 # =============================================================================
 __author__ = "Martin van der Schelling (M.P.vanderSchelling@tudelft.nl)"
 __credits__ = ["Martin van der Schelling"]
 __status__ = "Alpha"
 # =============================================================================
 #
 # =============================================================================
 
 
 class Simulator:
     """Base class for a FEM simulator"""
 
-    # def __init__(self, data: Data):
-    #     self.data = data
-
     def pre_process(self) -> None:
         """Function that handles the pre-processing"""
-        pass
+        ...
         # raise NotImplementedError("No pre-process function implemented!")
 
     def execute(self) -> None:
         """Function that calls the FEM simulator the pre-processing"""
         raise NotImplementedError("No execute function implemented!")
 
     def post_process(self) -> None:
         """Function that handles the post-processing"""
-        pass
-        # raise NotImplementedError("No post-process function implemented!")
+        ...
 
+    @time_and_log
     def run(self) -> None:
         self.pre_process()
         self.execute()
         self.post_process()
```

### Comparing `f3dasm-0.9.3/src/f3dasm/utils.py` & `f3dasm-1.1.0/src/f3dasm/utils.py`

 * *Files identical despite different names*

### Comparing `f3dasm-0.9.3/src/f3dasm.egg-info/PKG-INFO` & `f3dasm-1.1.0/src/f3dasm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: f3dasm
-Version: 0.9.3
+Version: 1.1.0
 Summary: f3dasm - Framework for Data-driven development and Analysis of Structures and Materials
-Home-page: https://github.com/bessagroup/F3DASM
+Home-page: https://github.com/bessagroup/f3dasm
 Author: Martin van der Schelling
 Author-email: M.P.vanderSchelling@tudelft.nl
 License: BSD
-Project-URL: Documentation, https://bessagroup.github.io/F3DASM/
-Project-URL: Wiki, https://github.com/bessagroup/F3DASM/wiki
+Project-URL: Documentation, https://bessagroup.github.io/f3dasm/
+Project-URL: Wiki, https://github.com/bessagroup/f3dasm/wiki
 Keywords: data-driven materials framework,machine learning
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -37,17 +37,17 @@
 
 ***
 
 [![Python](https://img.shields.io/pypi/pyversions/f3dasm)](https://www.python.org)
 [![pypi](https://img.shields.io/pypi/v/f3dasm.svg)](https://pypi.org/project/f3dasm/)
 [![GitHub license](https://img.shields.io/badge/license-BSD-blue)](https://github.com/bessagroup/f3dasm)
 
-[**Docs**](https://bessagroup.github.io/F3DASM/)
-| [**Installation**](https://bessagroup.github.io/F3DASM/gettingstarted.html)
-| [**GitHub**](https://github.com/bessagroup/F3DASM/tree/versionmartin)
+[**Docs**](https://bessagroup.github.io/f3dasm/)
+| [**Installation**](https://bessagroup.github.io/f3dasm/general/gettingstarted.html)
+| [**GitHub**](https://github.com/bessagroup/f3dasm)
 | [**PyPI**](https://pypi.org/project/f3dasm/)
 | [**Practical sessions**](https://github.com/mpvanderschelling/F3DASM_practical)
 
 Welcome to `f3dasm`, a Python package for data-driven design and analysis of structures and materials.
 
 * Created by M.A. Bessa (M.A.Bessa@tudelft.nl) in September 2016
 * Current developer and maintainer: [M.P. van der Schelling](https://github.com/mpvanderschelling/) (M.P.vanderSchelling@tudelft.nl)
```

### Comparing `f3dasm-0.9.3/src/f3dasm.egg-info/SOURCES.txt` & `f3dasm-1.1.0/src/f3dasm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,50 +21,49 @@
 src/f3dasm.egg-info/requires.txt
 src/f3dasm.egg-info/top_level.txt
 src/f3dasm/data/__init__.py
 src/f3dasm/data/benchmarkfunction_data.py
 src/f3dasm/data/learningdata.py
 src/f3dasm/data/linearregression_data.py
 src/f3dasm/design/__init__.py
-src/f3dasm/design/all_parameters.py
-src/f3dasm/design/constraint.py
+src/f3dasm/design/_data.py
+src/f3dasm/design/_jobqueue.py
 src/f3dasm/design/design.py
 src/f3dasm/design/experimentdata.py
 src/f3dasm/design/parameter.py
-src/f3dasm/design/utils.py
 src/f3dasm/experiment/__init__.py
 src/f3dasm/experiment/filehandler.py
-src/f3dasm/experiment/jobs.py
 src/f3dasm/experiment/logging.py
+src/f3dasm/experiment/parallelization.py
 src/f3dasm/experiment/quickstart.py
 src/f3dasm/functions/__init__.py
 src/f3dasm/functions/function.py
 src/f3dasm/functions/pybenchfunction.py
 src/f3dasm/functions/adapters/__init__.py
 src/f3dasm/functions/adapters/augmentor.py
 src/f3dasm/functions/adapters/pybenchfunction.py
 src/f3dasm/machinelearning/__init__.py
 src/f3dasm/machinelearning/all_models.py
 src/f3dasm/machinelearning/evaluator.py
 src/f3dasm/machinelearning/linear_regression.py
 src/f3dasm/machinelearning/loss_functions.py
+src/f3dasm/machinelearning/mnist_classifier.py
 src/f3dasm/machinelearning/model.py
 src/f3dasm/machinelearning/passthrough_model.py
 src/f3dasm/machinelearning/utils.py
 src/f3dasm/machinelearning/adapters/__init__.py
 src/f3dasm/machinelearning/adapters/tensorflow_implementations.py
 src/f3dasm/optimization/__init__.py
 src/f3dasm/optimization/_protocol.py
 src/f3dasm/optimization/adam.py
 src/f3dasm/optimization/adamax.py
 src/f3dasm/optimization/all_optimizers.py
 src/f3dasm/optimization/bayesianoptimization.py
 src/f3dasm/optimization/cg.py
 src/f3dasm/optimization/cmaes.py
-src/f3dasm/optimization/cmaesadam.py
 src/f3dasm/optimization/cobyla.py
 src/f3dasm/optimization/differentialevolution.py
 src/f3dasm/optimization/ftrl.py
 src/f3dasm/optimization/lbfgsb.py
 src/f3dasm/optimization/nadam.py
 src/f3dasm/optimization/neldermead.py
 src/f3dasm/optimization/optimizer.py
```

### Comparing `f3dasm-0.9.3/src/f3dasm.egg-info/requires.txt` & `f3dasm-1.1.0/src/f3dasm.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 pandas
 matplotlib
 hydra-core
 pathos>=0.3.0
 autograd
 
 [all]
-tensorflow>=2.11.0
-GPy>=1.10.0
 GPyOpt>=1.2.6
 SALib
+GPy>=1.10.0
+tensorflow>=2.11.0
 
 [all:platform_system == "Linux"]
 pygmo
 
 [dev]
-tensorflow>=2.11.0
-GPy>=1.10.0
 GPyOpt>=1.2.6
 SALib
+GPy>=1.10.0
+tensorflow>=2.11.0
 sphinx
 sphinx_rtd_theme
 sphinxcontrib-bibtex
 sphinx_autodoc_typehints
 pytest
 pytest-cov
 hypothesis
```

### Comparing `f3dasm-0.9.3/tests/conftest.py` & `f3dasm-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

