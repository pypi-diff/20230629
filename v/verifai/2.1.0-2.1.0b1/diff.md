# Comparing `tmp/verifai-2.1.0.tar.gz` & `tmp/verifai-2.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verifai-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "verifai-2.1.0b1.tar", max compression
```

## Comparing `verifai-2.1.0.tar` & `verifai-2.1.0b1.tar`

### file list

```diff
@@ -1,82 +1,76 @@
--rw-r--r--   0        0        0     1519 2019-12-13 14:56:32.000000 verifai-2.1.0/LICENSE
--rw-r--r--   0        0        0     2148 2020-10-22 16:03:16.042484 verifai-2.1.0/README.md
--rw-r--r--   0        0        0     2123 2023-06-29 13:57:43.775128 verifai-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     8196 2020-11-22 15:38:10.797797 verifai-2.1.0/src/verifai/.DS_Store
--rw-r--r--   0        0        0       62 2020-10-22 16:03:16.043841 verifai-2.1.0/src/verifai/__init__.py
--rw-r--r--   0        0        0     1962 2022-09-01 17:19:52.694839 verifai-2.1.0/src/verifai/client.py
--rw-r--r--   0        0        0    13455 2022-07-22 03:24:44.828267 verifai-2.1.0/src/verifai/error_table.py
--rw-r--r--   0        0        0    12281 2022-09-01 17:44:41.775734 verifai-2.1.0/src/verifai/falsifier.py
--rw-r--r--   0        0        0       24 2020-10-22 16:03:16.044661 verifai-2.1.0/src/verifai/features/__init__.py
--rw-r--r--   0        0        0    41696 2022-07-22 03:24:44.829830 verifai-2.1.0/src/verifai/features/features.py
--rw-r--r--   0        0        0     1861 2022-07-22 03:24:44.830209 verifai-2.1.0/src/verifai/monitor.py
--rw-r--r--   0        0        0     6148 2020-05-20 05:08:56.000000 verifai-2.1.0/src/verifai/samplers/.DS_Store
--rw-r--r--   0        0        0      621 2020-10-22 16:03:16.045406 verifai-2.1.0/src/verifai/samplers/__init__.py
--rw-r--r--   0        0        0     1604 2022-07-22 03:24:44.830982 verifai-2.1.0/src/verifai/samplers/bayesian_optimization.py
--rw-r--r--   0        0        0     7075 2022-07-26 20:25:41.417490 verifai-2.1.0/src/verifai/samplers/cross_entropy.py
--rw-r--r--   0        0        0     2229 2022-07-22 03:24:44.832588 verifai-2.1.0/src/verifai/samplers/dist_BO.py
--rw-r--r--   0        0        0     8263 2022-07-22 03:24:44.833474 verifai-2.1.0/src/verifai/samplers/domain_sampler.py
--rw-r--r--   0        0        0     4754 2022-07-26 20:08:34.726736 verifai-2.1.0/src/verifai/samplers/eg_sampler.py
--rw-r--r--   0        0        0    10417 2022-07-22 03:24:44.834926 verifai-2.1.0/src/verifai/samplers/feature_sampler.py
--rw-r--r--   0        0        0     3218 2022-07-22 03:24:44.836712 verifai-2.1.0/src/verifai/samplers/grid_sampler.py
--rw-r--r--   0        0        0     1192 2022-07-22 03:24:44.837582 verifai-2.1.0/src/verifai/samplers/halton.py
--rw-r--r--   0        0        0     8050 2022-07-26 20:08:05.231862 verifai-2.1.0/src/verifai/samplers/multi_armed_bandit.py
--rw-r--r--   0        0        0      568 2022-07-22 03:24:44.838281 verifai-2.1.0/src/verifai/samplers/multi_objective.py
--rw-r--r--   0        0        0      687 2022-07-22 03:24:44.839073 verifai-2.1.0/src/verifai/samplers/random_sampler.py
--rw-r--r--   0        0        0     1572 2022-07-22 03:24:44.839751 verifai-2.1.0/src/verifai/samplers/rejection.py
--rw-r--r--   0        0        0    12473 2023-06-29 05:24:45.194754 verifai-2.1.0/src/verifai/samplers/scenic_sampler.py
--rw-r--r--   0        0        0     4009 2022-07-22 03:24:44.840919 verifai-2.1.0/src/verifai/samplers/simulated_annealing.py
--rw-r--r--   0        0        0     9797 2022-09-01 16:17:26.729070 verifai-2.1.0/src/verifai/scenic_server.py
--rw-r--r--   0        0        0     8399 2022-09-01 17:05:12.693708 verifai-2.1.0/src/verifai/server.py
--rw-r--r--   0        0        0    10244 2020-05-20 04:54:18.000000 verifai-2.1.0/src/verifai/simulators/.DS_Store
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.047860 verifai-2.1.0/src/verifai/simulators/__init__.py
--rw-r--r--   0        0        0     6148 2020-03-19 00:38:19.000000 verifai-2.1.0/src/verifai/simulators/car_simulator/.DS_Store
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.047970 verifai-2.1.0/src/verifai/simulators/car_simulator/__init__.py
--rw-r--r--   0        0        0      648 2020-10-22 16:03:16.048147 verifai-2.1.0/src/verifai/simulators/car_simulator/car_dynamics.py
--rw-r--r--   0        0        0     1525 2020-10-22 16:03:16.048308 verifai-2.1.0/src/verifai/simulators/car_simulator/car_object.py
--rw-r--r--   0        0        0      348 2020-10-22 16:03:16.048458 verifai-2.1.0/src/verifai/simulators/car_simulator/client_car_sim.py
--rw-r--r--   0        0        0     6148 2020-03-19 00:38:34.000000 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/.DS_Store
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.048547 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/__init__.py
--rw-r--r--   0        0        0     1521 2020-10-22 16:03:16.048738 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/control_utils/LQR_computation.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.048838 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/control_utils/__init__.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.049069 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/__init__.py
--rw-r--r--   0        0        0     1446 2022-09-01 17:40:28.318125 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_falsifier.py
--rw-r--r--   0        0        0     3557 2020-10-22 16:03:16.049640 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_simulation.py
--rw-r--r--   0        0        0     1769 2020-10-22 16:03:16.049853 verifai-2.1.0/src/verifai/simulators/car_simulator/examples/simple_control.py
--rw-r--r--   0        0        0    34703 2020-10-22 16:03:16.050306 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-blue.png
--rw-r--r--   0        0        0    35818 2020-10-22 16:03:16.050883 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-gray.png
--rw-r--r--   0        0        0    46045 2020-10-22 16:03:16.051467 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-orange.png
--rw-r--r--   0        0        0    47932 2020-10-22 16:03:16.051991 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-purple.png
--rw-r--r--   0        0        0    29755 2020-10-22 16:03:16.052429 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-red.png
--rw-r--r--   0        0        0    43944 2020-10-22 16:03:16.052807 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-white.png
--rw-r--r--   0        0        0    32237 2020-10-22 16:03:16.053154 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-yellow.png
--rw-r--r--   0        0        0    80687 2020-10-22 16:03:16.053851 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/cone.png
--rw-r--r--   0        0        0    63722 2020-10-22 16:03:16.054381 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/firetruck.png
--rw-r--r--   0        0        0   161331 2020-10-22 16:03:16.055001 verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/grass.png
--rw-r--r--   0        0        0      567 2020-10-22 16:03:16.055224 verifai-2.1.0/src/verifai/simulators/car_simulator/lane.py
--rw-r--r--   0        0        0     5876 2020-10-22 16:03:16.055499 verifai-2.1.0/src/verifai/simulators/car_simulator/simulator.py
--rw-r--r--   0        0        0     6148 2020-05-20 04:49:07.000000 verifai-2.1.0/src/verifai/simulators/carla/.DS_Store
--rw-r--r--   0        0        0      546 2020-10-22 16:03:16.055826 verifai-2.1.0/src/verifai/simulators/carla/agents/brake_agent.py
--rw-r--r--   0        0        0     5612 2020-10-22 16:03:16.056074 verifai-2.1.0/src/verifai/simulators/carla/agents/overtake_agent.py
--rw-r--r--   0        0        0     3907 2020-10-22 16:03:16.056317 verifai-2.1.0/src/verifai/simulators/carla/agents/pid_agent.py
--rw-r--r--   0        0        0     2405 2020-10-22 16:03:16.056564 verifai-2.1.0/src/verifai/simulators/carla/agents/pid_follow_controller.py
--rw-r--r--   0        0        0     3363 2020-10-22 16:03:16.056887 verifai-2.1.0/src/verifai/simulators/carla/carla_scenic_task.py
--rw-r--r--   0        0        0     2608 2020-10-22 16:03:16.057127 verifai-2.1.0/src/verifai/simulators/carla/carla_task.py
--rw-r--r--   0        0        0    26303 2020-10-22 16:03:16.057471 verifai-2.1.0/src/verifai/simulators/carla/carla_world.py
--rw-r--r--   0        0        0      352 2020-10-22 16:03:16.057727 verifai-2.1.0/src/verifai/simulators/carla/client_carla.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.057814 verifai-2.1.0/src/verifai/simulators/openai_gym/__init__.py
--rw-r--r--   0        0        0     3846 2020-10-22 16:03:16.058073 verifai-2.1.0/src/verifai/simulators/openai_gym/baselines_task.py
--rw-r--r--   0        0        0      337 2020-10-22 16:03:16.058236 verifai-2.1.0/src/verifai/simulators/openai_gym/client_gym.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.058314 verifai-2.1.0/src/verifai/simulators/webots/__init__.py
--rw-r--r--   0        0        0      455 2020-10-22 16:03:16.058551 verifai-2.1.0/src/verifai/simulators/webots/client_webots.py
--rw-r--r--   0        0        0      396 2020-10-22 16:03:16.058780 verifai-2.1.0/src/verifai/simulators/webots/webots_task.py
--rw-r--r--   0        0        0     6148 2020-03-19 15:41:25.000000 verifai-2.1.0/src/verifai/simulators/xplane/.DS_Store
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.058940 verifai-2.1.0/src/verifai/simulators/xplane/__init__.py
--rw-r--r--   0        0        0    14443 2020-10-22 16:03:16.059260 verifai-2.1.0/src/verifai/simulators/xplane/server.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.059351 verifai-2.1.0/src/verifai/simulators/xplane/utils/__init__.py
--rw-r--r--   0        0        0      490 2020-10-22 16:03:16.059600 verifai-2.1.0/src/verifai/simulators/xplane/utils/controller.py
--rw-r--r--   0        0        0     2544 2020-10-22 16:03:16.059833 verifai-2.1.0/src/verifai/simulators/xplane/utils/geometry.py
--rw-r--r--   0        0        0      800 2020-10-22 16:03:16.060080 verifai-2.1.0/src/verifai/simulators/xplane/utils/images.py
--rw-r--r--   0        0        0        0 2020-10-22 16:03:16.060166 verifai-2.1.0/src/verifai/utils/__init__.py
--rw-r--r--   0        0        0      566 2022-06-06 18:59:52.008123 verifai-2.1.0/src/verifai/utils/frozendict.py
--rw-r--r--   0        0        0      671 2020-10-22 16:03:16.060691 verifai-2.1.0/src/verifai/utils/utils.py
--rw-r--r--   0        0        0     4672 1970-01-01 00:00:00.000000 verifai-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1519 2019-12-13 14:56:32.000000 verifai-2.1.0b1/LICENSE
+-rw-r--r--   0        0        0     2148 2020-10-22 16:03:16.042484 verifai-2.1.0b1/README.md
+-rw-r--r--   0        0        0     2449 2022-07-21 21:17:17.150207 verifai-2.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0       62 2020-10-22 16:03:16.043841 verifai-2.1.0b1/src/verifai/__init__.py
+-rw-r--r--   0        0        0     1747 2022-07-21 17:21:19.246979 verifai-2.1.0b1/src/verifai/client.py
+-rw-r--r--   0        0        0    13455 2022-07-21 17:21:19.247632 verifai-2.1.0b1/src/verifai/error_table.py
+-rw-r--r--   0        0        0    11865 2022-07-21 21:53:50.434049 verifai-2.1.0b1/src/verifai/falsifier.py
+-rw-r--r--   0        0        0       24 2020-10-22 16:03:16.044661 verifai-2.1.0b1/src/verifai/features/__init__.py
+-rw-r--r--   0        0        0    41696 2022-07-21 17:21:19.249081 verifai-2.1.0b1/src/verifai/features/features.py
+-rw-r--r--   0        0        0     1861 2022-03-27 20:28:26.112997 verifai-2.1.0b1/src/verifai/monitor.py
+-rw-r--r--   0        0        0      621 2020-10-22 16:03:16.045406 verifai-2.1.0b1/src/verifai/samplers/__init__.py
+-rw-r--r--   0        0        0     1604 2022-03-27 20:28:26.113296 verifai-2.1.0b1/src/verifai/samplers/bayesian_optimization.py
+-rw-r--r--   0        0        0     7079 2022-07-21 17:21:19.250033 verifai-2.1.0b1/src/verifai/samplers/cross_entropy.py
+-rw-r--r--   0        0        0     2229 2022-03-27 20:28:26.114158 verifai-2.1.0b1/src/verifai/samplers/dist_BO.py
+-rw-r--r--   0        0        0     8263 2022-03-27 20:28:26.114770 verifai-2.1.0b1/src/verifai/samplers/domain_sampler.py
+-rw-r--r--   0        0        0     4754 2022-03-27 20:28:26.115302 verifai-2.1.0b1/src/verifai/samplers/eg_sampler.py
+-rw-r--r--   0        0        0    10417 2022-07-21 17:21:19.250801 verifai-2.1.0b1/src/verifai/samplers/feature_sampler.py
+-rw-r--r--   0        0        0     3218 2022-03-27 20:28:26.116638 verifai-2.1.0b1/src/verifai/samplers/grid_sampler.py
+-rw-r--r--   0        0        0     1192 2022-03-27 20:28:26.117365 verifai-2.1.0b1/src/verifai/samplers/halton.py
+-rw-r--r--   0        0        0     8042 2022-03-27 20:28:26.118410 verifai-2.1.0b1/src/verifai/samplers/multi_armed_bandit.py
+-rw-r--r--   0        0        0      568 2022-03-27 20:28:26.119256 verifai-2.1.0b1/src/verifai/samplers/multi_objective.py
+-rw-r--r--   0        0        0      687 2022-03-27 20:28:26.120823 verifai-2.1.0b1/src/verifai/samplers/random_sampler.py
+-rw-r--r--   0        0        0     1572 2022-03-27 20:28:26.123358 verifai-2.1.0b1/src/verifai/samplers/rejection.py
+-rw-r--r--   0        0        0    11512 2022-07-21 21:25:32.799454 verifai-2.1.0b1/src/verifai/samplers/scenic_sampler.py
+-rw-r--r--   0        0        0     4009 2022-07-21 17:21:19.251371 verifai-2.1.0b1/src/verifai/samplers/simulated_annealing.py
+-rw-r--r--   0        0        0    10058 2022-07-21 21:53:07.559602 verifai-2.1.0b1/src/verifai/scenic_server.py
+-rw-r--r--   0        0        0     7993 2022-07-21 17:21:19.252812 verifai-2.1.0b1/src/verifai/server.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.047860 verifai-2.1.0b1/src/verifai/simulators/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.047970 verifai-2.1.0b1/src/verifai/simulators/car_simulator/__init__.py
+-rw-r--r--   0        0        0      648 2020-10-22 16:03:16.048147 verifai-2.1.0b1/src/verifai/simulators/car_simulator/car_dynamics.py
+-rw-r--r--   0        0        0     1525 2020-10-22 16:03:16.048308 verifai-2.1.0b1/src/verifai/simulators/car_simulator/car_object.py
+-rw-r--r--   0        0        0      348 2020-10-22 16:03:16.048458 verifai-2.1.0b1/src/verifai/simulators/car_simulator/client_car_sim.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.048547 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/__init__.py
+-rw-r--r--   0        0        0     1521 2020-10-22 16:03:16.048738 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/control_utils/LQR_computation.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.048838 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/control_utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.049069 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/__init__.py
+-rw-r--r--   0        0        0     1415 2020-10-22 16:03:16.049366 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_falsifier.py
+-rw-r--r--   0        0        0     3557 2020-10-22 16:03:16.049640 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_simulation.py
+-rw-r--r--   0        0        0     1769 2020-10-22 16:03:16.049853 verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/simple_control.py
+-rw-r--r--   0        0        0    34703 2020-10-22 16:03:16.050306 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-blue.png
+-rw-r--r--   0        0        0    35818 2020-10-22 16:03:16.050883 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-gray.png
+-rw-r--r--   0        0        0    46045 2020-10-22 16:03:16.051467 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-orange.png
+-rw-r--r--   0        0        0    47932 2020-10-22 16:03:16.051991 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-purple.png
+-rw-r--r--   0        0        0    29755 2020-10-22 16:03:16.052429 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-red.png
+-rw-r--r--   0        0        0    43944 2020-10-22 16:03:16.052807 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-white.png
+-rw-r--r--   0        0        0    32237 2020-10-22 16:03:16.053154 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-yellow.png
+-rw-r--r--   0        0        0    80687 2020-10-22 16:03:16.053851 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/cone.png
+-rw-r--r--   0        0        0    63722 2020-10-22 16:03:16.054381 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/firetruck.png
+-rw-r--r--   0        0        0   161331 2020-10-22 16:03:16.055001 verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/grass.png
+-rw-r--r--   0        0        0      567 2020-10-22 16:03:16.055224 verifai-2.1.0b1/src/verifai/simulators/car_simulator/lane.py
+-rw-r--r--   0        0        0     5876 2020-10-22 16:03:16.055499 verifai-2.1.0b1/src/verifai/simulators/car_simulator/simulator.py
+-rw-r--r--   0        0        0      546 2020-10-22 16:03:16.055826 verifai-2.1.0b1/src/verifai/simulators/carla/agents/brake_agent.py
+-rw-r--r--   0        0        0     5612 2020-10-22 16:03:16.056074 verifai-2.1.0b1/src/verifai/simulators/carla/agents/overtake_agent.py
+-rw-r--r--   0        0        0     3907 2020-10-22 16:03:16.056317 verifai-2.1.0b1/src/verifai/simulators/carla/agents/pid_agent.py
+-rw-r--r--   0        0        0     2405 2020-10-22 16:03:16.056564 verifai-2.1.0b1/src/verifai/simulators/carla/agents/pid_follow_controller.py
+-rw-r--r--   0        0        0     3363 2020-10-22 16:03:16.056887 verifai-2.1.0b1/src/verifai/simulators/carla/carla_scenic_task.py
+-rw-r--r--   0        0        0     2608 2020-10-22 16:03:16.057127 verifai-2.1.0b1/src/verifai/simulators/carla/carla_task.py
+-rw-r--r--   0        0        0    26303 2020-10-22 16:03:16.057471 verifai-2.1.0b1/src/verifai/simulators/carla/carla_world.py
+-rw-r--r--   0        0        0      352 2020-10-22 16:03:16.057727 verifai-2.1.0b1/src/verifai/simulators/carla/client_carla.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.057814 verifai-2.1.0b1/src/verifai/simulators/openai_gym/__init__.py
+-rw-r--r--   0        0        0     3846 2020-10-22 16:03:16.058073 verifai-2.1.0b1/src/verifai/simulators/openai_gym/baselines_task.py
+-rw-r--r--   0        0        0      337 2020-10-22 16:03:16.058236 verifai-2.1.0b1/src/verifai/simulators/openai_gym/client_gym.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.058314 verifai-2.1.0b1/src/verifai/simulators/webots/__init__.py
+-rw-r--r--   0        0        0      455 2020-10-22 16:03:16.058551 verifai-2.1.0b1/src/verifai/simulators/webots/client_webots.py
+-rw-r--r--   0        0        0      396 2020-10-22 16:03:16.058780 verifai-2.1.0b1/src/verifai/simulators/webots/webots_task.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.058940 verifai-2.1.0b1/src/verifai/simulators/xplane/__init__.py
+-rw-r--r--   0        0        0    14443 2020-10-22 16:03:16.059260 verifai-2.1.0b1/src/verifai/simulators/xplane/server.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.059351 verifai-2.1.0b1/src/verifai/simulators/xplane/utils/__init__.py
+-rw-r--r--   0        0        0      490 2020-10-22 16:03:16.059600 verifai-2.1.0b1/src/verifai/simulators/xplane/utils/controller.py
+-rw-r--r--   0        0        0     2544 2020-10-22 16:03:16.059833 verifai-2.1.0b1/src/verifai/simulators/xplane/utils/geometry.py
+-rw-r--r--   0        0        0      800 2020-10-22 16:03:16.060080 verifai-2.1.0b1/src/verifai/simulators/xplane/utils/images.py
+-rw-r--r--   0        0        0        0 2020-10-22 16:03:16.060166 verifai-2.1.0b1/src/verifai/utils/__init__.py
+-rw-r--r--   0        0        0      566 2022-06-06 18:59:52.008123 verifai-2.1.0b1/src/verifai/utils/frozendict.py
+-rw-r--r--   0        0        0      671 2020-10-22 16:03:16.060691 verifai-2.1.0b1/src/verifai/utils/utils.py
+-rw-r--r--   0        0        0     4752 2022-07-22 03:21:34.174443 verifai-2.1.0b1/setup.py
+-rw-r--r--   0        0        0     4915 2022-07-22 03:21:34.174886 verifai-2.1.0b1/PKG-INFO
```

### Comparing `verifai-2.1.0/LICENSE` & `verifai-2.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/README.md` & `verifai-2.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/client.py` & `verifai-2.1.0b1/src/verifai/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,21 +14,16 @@
         self.bufsize = bufsize
 
     def initialize(self):
         self.socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.host = '127.0.0.1'
         try:
             self.socket.connect((self.host, self.port))
-        except ConnectionResetError:
-            self.close()
-            return False
         except OSError as e:
-            self.close()
             raise RuntimeError('unable to connect to server') from e
-        return True
 
     def receive(self):
         data = []
         try:
             while True:
                 msg = self.socket.recv(self.bufsize)
                 if not msg:
@@ -38,24 +33,22 @@
             return False, None
         data = dill.loads(b"".join(data))
         return True, data
 
     def send(self, data):
         msg = dill.dumps(data)
         self.socket.send(msg)
-        self.socket.shutdown(socket.SHUT_WR)
 
     def close(self):
         self.socket.close()
 
     def run_client(self):
-        success = self.initialize()
+        self.initialize()
         try:
-            if success:
-                success, sample = self.receive()
+            success, sample = self.receive()
             if not success:
                 print("No new sample received from server.")
                 return False
             sim = self.simulate(sample)
             self.send(sim)
             return True
         finally:
```

### Comparing `verifai-2.1.0/src/verifai/error_table.py` & `verifai-2.1.0b1/src/verifai/error_table.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/falsifier.py` & `verifai-2.1.0b1/src/verifai/falsifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,14 @@
         self.samples = {}
         self.monitor = monitor
 
         params = DotMap(
             save_error_table=True, save_safe_table=True,
             error_table_path=None, safe_table_path=None,
             n_iters=1000, ce_num_max=np.inf, fal_thres=0,
-            max_time=None,
             sampler_params=None, verbosity=0,
         )
         if falsifier_params is not None:
             params.update(falsifier_params)
         if params.sampler_params is None:
             params.sampler_params = DotMap(thres=params.fal_thres)
         self.multi = isinstance(self.monitor, multi_objective_monitor)
@@ -42,15 +41,18 @@
         self.save_error_table = params.save_error_table
         self.save_safe_table = params.save_safe_table
         self.error_table_path = params.error_table_path
         self.safe_table_path = params.safe_table_path
         if not hasattr(self, 'num_workers'):
             self.num_workers = 1
         self.n_iters, self.ce_num_max = params.n_iters, params.ce_num_max
-        self.max_time = params.max_time
+        if self.n_iters is None:
+            self.max_time = params.max_time
+        else:
+            self.max_time = None
         self.fal_thres = params.fal_thres
         self.sampler_params = params.sampler_params
         self.verbosity = params.verbosity
 
         server_params = DotMap(init=True)
         if server_options is not None:
             server_params.update(server_options)
@@ -66,16 +68,14 @@
             self.sampler_type = 'random'
         sampling_data.sampler_type = self.sampler_type
         sampling_data.sample_space = self.sample_space
         sampling_data.sampler_params = self.sampler_params
         sampling_data.sampler = self.sampler
 
         self.server = server_class(sampling_data, self.monitor, options=server_options)
-        if self.verbosity >= 1:
-            print("Server ready")
 
     def init_error_table(self):
         # Initializing error table
         if self.save_error_table:
             self.error_table = error_table(space = self.server.sample_space)
         if self.save_safe_table:
             self.safe_table = error_table(space = self.server.sample_space)
@@ -125,38 +125,31 @@
     def run_falsifier(self):
         i = 0
         ce_num = 0
         server_samples = []
         rhos = []
         self.total_sample_time = 0
         self.total_simulate_time = 0
-        if self.verbosity >= 1:
-            suffix = ''
-            if self.n_iters:
-                suffix = f' for {self.n_iters} iterations'
-            if self.max_time:
-                suffix += f' for {self.max_time:.0f} seconds'
-            print('Running falsification' + suffix)
         if self.verbosity >= 2:
-            print(f'Server class is {type(self.server)}')
+            print(f'Running falsifier; server class is {type(self.server)}')
 
         if self.verbosity >= 1:
             if self.n_iters is not None:
                 bar = progressbar.ProgressBar(max_value=self.n_iters)
             else:
-                widgets = ['Samples generated: ', progressbar.Counter('%(value)d'),
+                widgets = ['Scenes generated: ', progressbar.Counter('%(value)d'),
                 ' (', progressbar.Timer(), ')']
                 bar = progressbar.ProgressBar(widgets=widgets)
 
         try:
             while True:
                 try:
-                    sample, rho, timings = self.server.run_server()
-                    self.total_sample_time += timings.sample_time
-                    self.total_simulate_time += timings.simulate_time
+                    sample, rho, (sample_time, simulate_time) = self.server.run_server()
+                    self.total_sample_time += sample_time
+                    self.total_simulate_time += simulate_time
                 except TerminationException:
                     if self.verbosity >= 1:
                         print("Sampler has generated all possible samples")
                     break
                 if self.verbosity >= 2:
                     print("Sample no: ", i, "\nSample: ", sample, "\nRho: ", rho)
                 self.samples[i] = sample
@@ -168,29 +161,25 @@
                 if i == 1:
                     t0 = time.time()
                 if self.n_iters is not None and i == self.n_iters:
                     break
                 if self.max_time is not None and time.time() - t0 >= self.max_time:
                     break
         finally:
-            if self.verbosity >= 1:
-                bar.finish()
             self.server.terminate()
         for sample, rho in zip(server_samples, rhos):
             ce = any([r <= self.fal_thres for r in rho]) if self.multi else rho <= self.fal_thres
             if ce:
                 if self.save_error_table:
                     self.populate_error_table(sample, rho)
                 ce_num = ce_num + 1
                 if ce_num >= self.ce_num_max:
                     break
             elif self.save_safe_table:
                 self.populate_error_table(sample, rho, error=False)
-        if self.verbosity >= 1:
-            print('Falsification complete.')
 
 class generic_falsifier(falsifier):
     def __init__(self,  monitor=None, sampler_type= None, sample_space=None, sampler=None,
                  falsifier_params=None, server_options={}, server_class=Server):
         if monitor is None:
             class monitor(specification_monitor):
                 def __init__(self):
```

### Comparing `verifai-2.1.0/src/verifai/features/features.py` & `verifai-2.1.0b1/src/verifai/features/features.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/monitor.py` & `verifai-2.1.0b1/src/verifai/monitor.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/__init__.py` & `verifai-2.1.0b1/src/verifai/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/bayesian_optimization.py` & `verifai-2.1.0b1/src/verifai/samplers/bayesian_optimization.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/cross_entropy.py` & `verifai-2.1.0b1/src/verifai/samplers/cross_entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     def getVector(self):
         bucket_samples = np.array([np.random.choice(int(b), p=self.dist[i])
                                    for i, b in enumerate(self.buckets)])
         self.current_sample = bucket_samples
         ret = tuple(np.random.uniform(bs, bs+1.)/b for b, bs
               in zip(self.buckets, bucket_samples))
         return ret, bucket_samples
-
+    
     def updateVector(self, vector, info, rho):
         if rho is None or rho >= self.thres:
             return
         for row, b in zip(self.dist, info):
             row *= self.alpha
             row[b] += 1 - self.alpha
```

### Comparing `verifai-2.1.0/src/verifai/samplers/dist_BO.py` & `verifai-2.1.0b1/src/verifai/samplers/dist_BO.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/domain_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/domain_sampler.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/eg_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/eg_sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import numpy as np
 from verifai.samplers.domain_sampler import BoxSampler, DiscreteBoxSampler, \
     DomainSampler, SplitSampler
 from verifai.samplers.random_sampler import RandomSampler
 from verifai.samplers.cross_entropy import DiscreteCrossEntropySampler
 
 class EpsilonGreedySampler(DomainSampler):
-    def __init__(self, domain, eg_params):
+    def __init__(self, domain, ce_params):
         super().__init__(domain)
-        self.alpha = eg_params.alpha
-        self.thres = eg_params.thres
-        self.cont_buckets = eg_params.cont.buckets
-        self.cont_dist = eg_params.cont.dist
-        self.disc_dist = eg_params.disc.dist
+        self.alpha = ce_params.alpha
+        self.thres = ce_params.thres
+        self.cont_buckets = ce_params.cont.buckets
+        self.cont_dist = ce_params.cont.dist
+        self.disc_dist = ce_params.disc.dist
         self.cont_ce = lambda domain: ContinuousEpsilonGreedySampler(domain=domain,
                                                      buckets=self.cont_buckets,
                                                      dist=self.cont_dist,
                                                      alpha=self.alpha,
                                                      thres=self.thres)
         self.disc_ce = lambda domain: DiscreteEpsilonGreedySampler(domain=domain,
                                                    dist=self.disc_dist,
```

### Comparing `verifai-2.1.0/src/verifai/samplers/feature_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/feature_sampler.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/grid_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/grid_sampler.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/halton.py` & `verifai-2.1.0b1/src/verifai/samplers/halton.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/multi_armed_bandit.py` & `verifai-2.1.0b1/src/verifai/samplers/multi_armed_bandit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 from verifai.samplers.domain_sampler import BoxSampler, DiscreteBoxSampler, \
     DomainSampler, SplitSampler
 from verifai.samplers.random_sampler import RandomSampler
 from verifai.samplers.cross_entropy import DiscreteCrossEntropySampler
 from verifai.samplers.multi_objective import MultiObjectiveSampler
 
 class MultiArmedBanditSampler(DomainSampler):
-    def __init__(self, domain, mab_params):
+    def __init__(self, domain, ce_params):
         super().__init__(domain)
-        self.alpha = mab_params.alpha
-        self.thres = mab_params.thres
-        self.cont_buckets = mab_params.cont.buckets
-        self.cont_dist = mab_params.cont.dist
-        self.disc_dist = mab_params.disc.dist
+        self.alpha = ce_params.alpha
+        self.thres = ce_params.thres
+        self.cont_buckets = ce_params.cont.buckets
+        self.cont_dist = ce_params.cont.dist
+        self.disc_dist = ce_params.disc.dist
         self.cont_ce = lambda domain: ContinuousMultiArmedBanditSampler(domain=domain,
                                                      buckets=self.cont_buckets,
                                                      dist=self.cont_dist,
                                                      alpha=self.alpha,
                                                      thres=self.thres)
         self.disc_ce = lambda domain: DiscreteMultiArmedBanditSampler(domain=domain,
                                                    dist=self.disc_dist,
@@ -32,16 +32,16 @@
                                                         partition,
                                                         RandomSampler)
         self.cont_sampler, self.disc_sampler = None, None
         self.rand_sampler = None
         for subsampler in self.split_sampler.samplers:
             if isinstance(subsampler, ContinuousMultiArmedBanditSampler):
                 assert self.cont_sampler is None
-                if 'priority_graph' in mab_params:
-                    subsampler.set_graph(mab_params.priority_graph)
+                if 'priority_graph' in ce_params:
+                    subsampler.set_graph(ce_params.priority_graph)
                 self.cont_sampler = subsampler
             elif isinstance(subsampler, DiscreteMultiArmedBanditSampler):
                 assert self.disc_sampler is None
                 self.disc_sampler = subsampler
             else:
                 assert isinstance(subsampler, RandomSampler)
                 assert self.rand_sampler is None
```

### Comparing `verifai-2.1.0/src/verifai/samplers/multi_objective.py` & `verifai-2.1.0b1/src/verifai/samplers/multi_objective.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/random_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/random_sampler.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/rejection.py` & `verifai-2.1.0b1/src/verifai/samplers/rejection.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/samplers/scenic_sampler.py` & `verifai-2.1.0b1/src/verifai/samplers/scenic_sampler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 
 """Interface to Scenic."""
 
-import importlib.metadata
-
 import scenic
 from scenic.core.distributions import needsSampling, Options
 from scenic.core.vectors import Vector
 from scenic.core.type_support import canCoerceType, coerce, underlyingType
 
 # TODO unify handling of these custom types!
 from scenic.simulators.utils.colors import Color
@@ -15,24 +13,16 @@
     CarModel as WebotsCarModel, carModels as webotsCarModels)
 
 from verifai.features import (Constant, Categorical, Real, Box, Array, Struct,
                               Feature, FeatureSpace)
 from verifai.samplers.feature_sampler import FeatureSampler
 from verifai.utils.frozendict import frozendict
 
-scenicMajorVersion = int(importlib.metadata.version('scenic').split('.')[0])
-if scenicMajorVersion >= 3:
-    from scenic.core.vectors import Orientation
-else:
-    Orientation = None
-
 scalarDomain = Real()
-vectorDim = 2 if scenicMajorVersion < 3 else 3
-vectorDomain = Array(scalarDomain, (vectorDim,))
-orientationDomain = Array(scalarDomain, (4,))  # as quaternions
+vectorDomain = Array(scalarDomain, (2,))
 gtaModelDomain = Categorical(*GTACarModel.models.values())
 webotsModelDomain = Categorical(*webotsCarModels)
 colorDomain = Box((0, 1), (0, 1), (0, 1))
 
 def convertToVerifaiType(value, strict=True):
     """Attempt to convert a Scenic value to a type known to VerifAI"""
     ty = underlyingType(value)
@@ -46,16 +36,14 @@
         return value
     elif ty is WebotsCarModel:
         return value
     elif ty is Color:
         return value
     elif canCoerceType(ty, Vector):
         return tuple(coerce(value, Vector))
-    elif Orientation and isinstance(value, Orientation):
-        return tuple(value.getRotation().as_quat())
     elif strict:    # Unknown type, so give up if we're being strict
         raise RuntimeError(
             f'attempted to convert Scenic value {value} of unknown type {ty}')
     else:
         return value
 
 def domainForValue(value):
@@ -67,16 +55,14 @@
         domain = gtaModelDomain
     elif ty is WebotsCarModel:
         domain = webotsModelDomain
     elif ty is Color:
         domain = colorDomain
     elif canCoerceType(ty, Vector):
         domain = vectorDomain
-    elif ty is Orientation:
-        domain = orientationDomain
     elif ty is str:
         # We can only handle strings when they come from a finite set of
         # possibilities; we heuristically detect that here.
         if isinstance(value, Options):
             domain = Categorical(*value.options)
         else:
             domain = None   # we can't ensure the domain is finite
@@ -102,16 +88,14 @@
     elif dom == scalarDomain:
         if not isinstance(scenicValue, (float, int)):
             raise RuntimeError(
                 f'could not coerce Scenic value {scenicValue} to scalar')
         return coerce(scenicValue, float)
     elif dom == vectorDomain:
         return tuple(coerce(scenicValue, Vector))
-    elif dom == orientationDomain:
-        return tuple(scenicValue.getRotation().as_quat())
     elif dom == colorDomain:
         assert isinstance(scenicValue, (tuple, list))
         assert len(scenicValue) == 3
         return scenicValue
     else:
         raise RuntimeError(
             f'Scenic value {scenicValue} has unexpected domain {dom}')
@@ -120,40 +104,35 @@
 ignoredParameters = {
     'externalSampler', 'externalSamplerRejectionFeedback',
     'verifaiSamplerType', 'verifaiSamplerParams',
     'behavior',
 }
 #: Scenic object properties not included in generated samples
 defaultIgnoredProperties = {
-    'shape',
-    'viewAngle', 'viewAngles', 'visibleDistance', 'cameraOffset',
-    'viewRayDensity', 'viewRayCount', 'viewRayDistanceScaling',
-    'baseOffset', 'contactTolerance', 'onDirection', 'sideComponentThresholds',
-    'allowCollisions', 'requireVisible', 'regionContainedIn', 'occluding',
-    'showVisibleRegion',
-    'mutator', 'mutationEnabled', 'mutationScale',
-    'positionStdDev', 'headingStdDev', 'orientationStdDev',
-    'behavior', 'lastActions',
+    'viewAngle', 'visibleDistance', 'cameraOffset',
+    'allowCollisions', 'requireVisible', 'regionContainedIn',
+    'mutator', 'mutationEnabled', 'positionStdDev', 'headingStdDev',
+    'behavior',
 }
-# certain built-in properties requiring type normalization before Scenic 3
+# certain built-in properties requiring type normalization
 normalizedProperties = {
     'position': Vector,
     'heading': float
-} if scenicMajorVersion < 3 else {}
+}
 # hard-coded Domains for certain properties
 specialDomainProperties = {
     'webotsType': Categorical(*(model.name for model in webotsCarModels)),
     'color': colorDomain,   # to allow Colors, tuples, or lists
 }
 
 def domainForObject(obj, ignoredProperties):
     """Construct a Domain for the given Scenic Object"""
     domains = {}
     for prop in obj.properties:
-        if prop in ignoredProperties or prop.startswith('_'):
+        if prop in ignoredProperties:
             continue
         value = getattr(obj, prop)
         if prop in normalizedProperties:
             value = coerce(value, normalizedProperties[prop])
         # TODO improve this system... (need to get better type info in Scenic)
         if prop in specialDomainProperties and needsSampling(value):
             dom = specialDomainProperties[prop]
@@ -174,19 +153,14 @@
 
 def pointForObject(dom, obj):
     """Convert a sampled Scenic Object to a point in its Domain"""
     values = []
     for prop, subdom in dom.domainNamed.items():
         if prop == 'type':      # special case for 'type' pseudo-property
             scenicValue = type(obj).__name__
-        elif (prop == 'speed'
-              and isinstance(subdom, Constant)
-              and scenicMajorVersion < 3):
-            # work around bug in Scenic 2.1
-            scenicValue = subdom.value
         else:
             scenicValue = getattr(obj, prop)
         values.append(pointForValue(subdom, scenicValue))
     return dom.makePoint(*values)
 
 def spaceForScenario(scenario, ignoredProperties):
     """Construct a FeatureSpace for the given Scenic Scenario."""
@@ -237,48 +211,50 @@
         if ignoredProperties is None:
             ignoredProperties = defaultIgnoredProperties
         space, self.quotedParams = spaceForScenario(scenario, ignoredProperties)
         super().__init__(space)
 
     @classmethod
     def fromScenario(cls, path, maxIterations=None,
-                     ignoredProperties=None, **kwargs):
+                     params={}, model=None, scenario=None,
+                     ignoredProperties=None):
         """Create a sampler corresponding to a Scenic program.
 
         The only required argument is ``path``, and ``maxIterations`` may be useful if
         your scenario requires a very large number of rejection sampling iterations.
-        See `scenic.scenarioFromFile` for details on optional keyword arguments used to
+        See `scenic.scenarioFromFile` for details on the optional arguments used to
         customize compilation of the Scenic file.
 
         Args:
             path (str): path to a Scenic file.
             maxIterations (int): maximum number of rejection sampling iterations
               (default 2000).
+            params (dict): global parameters to override; see `scenic.scenarioFromFile`.
+            model (str): :term:`world model` to use; see `scenic.scenarioFromFile`.
+            scenario (str): :term:`modular scenario` to use; see `scenic.scenarioFromFile`.
             ignoredProperties: properties of Scenic objects to not include in
               generated samples (see ``defaultIgnoredProperties`` for the default).
-            kwargs: additional keyword arguments passed to `scenic.scenarioFromFile`;
-              e.g. ``params`` to override global parameters or ``model`` to set the
-              :term:`world model`.
         """
-        scenario = scenic.scenarioFromFile(path, **kwargs)
+        scenario = scenic.scenarioFromFile(path, params=params, model=model)
         return cls(scenario, maxIterations=maxIterations,
                    ignoredProperties=ignoredProperties)
 
     @classmethod
     def fromScenicCode(cls, code, maxIterations=None,
-                       ignoredProperties=None, **kwargs):
+                       params={}, model=None, scenario=None,
+                       ignoredProperties=None):
         """As above, but given a Scenic program as a string."""
-        scenario = scenic.scenarioFromString(code, **kwargs)
+        scenario = scenic.scenarioFromString(code)
         return cls(scenario, maxIterations=maxIterations,
                    ignoredProperties=ignoredProperties)
 
     def nextSample(self, feedback=None):
         ret = self.scenario.generate(
-            maxIterations=self.maxIterations, feedback=feedback, verbosity=0
-        )
+            maxIterations=self.maxIterations, feedback=feedback, verbosity=0)
+        # print(ret)
         self.lastScene, _ = ret
         return self.pointForScene(self.lastScene)
 
     def pointForScene(self, scene):
         """Convert a sampled Scenic :obj:`Scene` to a point in our feature space."""
         lengths, dom = self.space.domains
         assert lengths is None
```

### Comparing `verifai-2.1.0/src/verifai/samplers/simulated_annealing.py` & `verifai-2.1.0b1/src/verifai/samplers/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/scenic_server.py` & `verifai-2.1.0b1/src/verifai/scenic_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import progressbar
 
 try:
     import ray
 except ModuleNotFoundError:
     ray = None   # ignore for now; we'll raise an error below if ray is actually needed
 
-from verifai.server import Server, ServerTimings
+from verifai.server import Server
 from verifai.samplers.scenic_sampler import ScenicSampler
 from verifai.monitor import multi_objective_monitor
 from scenic.core.simulators import SimulationCreationError
 from scenic.core.external_params import VerifaiSampler
 from scenic.core.distributions import RejectionException
 
 class ScenicServer(Server):
@@ -48,23 +48,28 @@
         self.verbosity = defaults.verbosity
         self.maxIterations = defaults.maxIterations
         if defaults.simulator is None:
             self.simulator = self.sampler.scenario.getSimulator()
         else:
             self.simulator = defaults.simulator
 
-    def evaluate_sample(self, sample):
+    def run_server(self):
+        start = time.time()
+        sample = self.sampler.nextSample(self.lastValue)
         scene = self.sampler.lastScene
         assert scene
+        after_sampling = time.time()
         result = self._simulate(scene)
         if result is None:
-            return self.rejectionFeedback
-        value = (0 if self.monitor is None
-                 else self.monitor.evaluate(result))
-        return value
+            self.lastValue = self.rejectionFeedback
+        else:
+            self.lastValue = (0 if self.monitor is None
+                              else self.monitor.evaluate(result))
+        after_simulation = time.time()
+        return sample, self.lastValue, (after_sampling - start, after_simulation - after_sampling)
 
     def _simulate(self, scene):
         startTime = time.time()
         if self.verbosity >= 1:
             print('  Beginning simulation...')
         try:
             result = self.simulator.simulate(scene,
```

### Comparing `verifai-2.1.0/src/verifai/server.py` & `verifai-2.1.0b1/src/verifai/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from dataclasses import dataclass
 import socket
-import time
-
 import dill
 from dotmap import DotMap
 
 from verifai.features.features import *
 from verifai.samplers.feature_sampler import *
 
 def choose_sampler(sample_space, sampler_type,
@@ -43,51 +40,51 @@
             if 'thres' in sampler_params:
                 ce_params.thres = sampler_params.thres
         sampler = FeatureSampler.crossEntropySamplerFor(
             sample_space, ce_params=ce_params)
         return 'ce', sampler
     if sampler_type == 'mab':
         if sampler_params is None:
-            mab_params = default_sampler_params('mab')
+            ce_params = default_sampler_params('ce')
         else:
-            mab_params = default_sampler_params('mab')
+            ce_params = default_sampler_params('ce')
             if 'cont' in sampler_params:
                 if 'buckets' in sampler_params.cont:
-                    mab_params.cont.buckets = sampler_params.cont.buckets
+                    ce_params.cont.buckets = sampler_params.cont.buckets
                 if 'dist' in sampler_params.cont:
-                    mab_params.cont.dist = sampler_params.cont.dist
+                    ce_params.cont.dist = sampler_params.cont.dist
             if 'dist' in sampler_params.disc:
-                mab_params.disc.dist = sampler_params.disc.dist
+                ce_params.disc.dist = sampler_params.disc.dist
             if 'alpha' in sampler_params:
-                mab_params.alpha = sampler_params.alpha
+                ce_params.alpha = sampler_params.alpha
             if 'thres' in sampler_params:
-                mab_params.thres = sampler_params.thres
+                ce_params.thres = sampler_params.thres
             if 'priority_graph' in sampler_params:
-                mab_params.priority_graph = sampler_params.priority_graph
+                ce_params.priority_graph = sampler_params.priority_graph
         sampler = FeatureSampler.multiArmedBanditSamplerFor(
-            sample_space, mab_params=mab_params)
+            sample_space, ce_params=ce_params)
         return 'mab', sampler
     if sampler_type == 'eg':
         if sampler_params is None:
-            eg_params = default_sampler_params('eg')
+            ce_params = default_sampler_params('ce')
         else:
-            eg_params = default_sampler_params('eg')
+            ce_params = default_sampler_params('ce')
             if 'cont' in sampler_params:
                 if 'buckets' in sampler_params.cont:
-                    eg_params.cont.buckets = sampler_params.cont.buckets
+                    ce_params.cont.buckets = sampler_params.cont.buckets
                 if 'dist' in sampler_params.cont:
-                    eg_params.cont.dist = sampler_params.cont.dist
+                    ce_params.cont.dist = sampler_params.cont.dist
             if 'dist' in sampler_params.disc:
-                eg_params.disc.dist = sampler_params.disc.dist
+                ce_params.disc.dist = sampler_params.disc.dist
             if 'alpha' in sampler_params:
-                eg_params.alpha = sampler_params.alpha
+                ce_params.alpha = sampler_params.alpha
             if 'thres' in sampler_params:
-                eg_params.thres = sampler_params.thres
+                ce_params.thres = sampler_params.thres
         sampler = FeatureSampler.epsilonGreedySamplerFor(
-            sample_space, eg_params=eg_params)
+            sample_space, ce_params=ce_params)
         return 'eg', sampler
 
     if sampler_type == 'bo':
         if sampler_params is None:
             bo_params = default_sampler_params('bo')
         else:
             bo_params = default_sampler_params('bo')
@@ -188,30 +185,20 @@
         simulation_data = self.receive()
         self.close_connection()
         value = (0 if self.monitor is None
                  else self.monitor.evaluate(simulation_data))
         return value
 
     def run_server(self):
-        start = time.time()
         sample = self.get_sample(self.lastValue)
-        after_sampling = time.time()
         self.lastValue = self.evaluate_sample(sample)
-        after_simulation = time.time()
-        timings = ServerTimings(sample_time=(after_sampling - start),
-                                simulate_time=(after_simulation - after_sampling))
-        return sample, self.lastValue, timings
+        return sample, self.lastValue
 
 try:
     import ray
     @ray.remote
     class ParallelServer(Server):
         pass
 except ModuleNotFoundError:
     class ParallelServer(Server):
         def __init__(*args, **kwargs):
             raise RuntimeError('ParallelServer requires ray to be installed')
-
-@dataclass
-class ServerTimings:
-    sample_time: float
-    simulate_time: float
```

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/car_dynamics.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/car_dynamics.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/car_object.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/car_object.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/examples/control_utils/LQR_computation.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/control_utils/LQR_computation.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_falsifier.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_falsifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 MAXREQS = 5
 BUFSIZE = 4096
 
 specification = ["G(xdeviation)"]
 
 falsifier_params = DotMap()
 falsifier_params.n_iters = MAX_ITERS
-falsifier_params.verbosity = 1
 falsifier_params.compute_error_table = True
 falsifier_params.fal_thres = 0.0
 
 server_options = DotMap(port=PORT, bufsize=BUFSIZE, maxreqs=MAXREQS)
 
 
 sampler_params = DotMap()
```

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_simulation.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/lanekeeping_LQR/lanekeeping_simulation.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/examples/simple_control.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/examples/simple_control.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-blue.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-blue.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-gray.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-gray.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-orange.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-orange.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-purple.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-purple.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-red.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-red.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-white.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-white.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/car-yellow.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/car-yellow.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/cone.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/cone.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/firetruck.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/firetruck.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/imgs/grass.png` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/imgs/grass.png`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/lane.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/lane.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/car_simulator/simulator.py` & `verifai-2.1.0b1/src/verifai/simulators/car_simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/agents/brake_agent.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/agents/brake_agent.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/agents/overtake_agent.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/agents/overtake_agent.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/agents/pid_agent.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/agents/pid_agent.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/agents/pid_follow_controller.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/agents/pid_follow_controller.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/carla_scenic_task.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/carla_scenic_task.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/carla_task.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/carla_task.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/carla/carla_world.py` & `verifai-2.1.0b1/src/verifai/simulators/carla/carla_world.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/openai_gym/baselines_task.py` & `verifai-2.1.0b1/src/verifai/simulators/openai_gym/baselines_task.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/xplane/server.py` & `verifai-2.1.0b1/src/verifai/simulators/xplane/server.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/xplane/utils/geometry.py` & `verifai-2.1.0b1/src/verifai/simulators/xplane/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/simulators/xplane/utils/images.py` & `verifai-2.1.0b1/src/verifai/simulators/xplane/utils/images.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/utils/frozendict.py` & `verifai-2.1.0b1/src/verifai/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/src/verifai/utils/utils.py` & `verifai-2.1.0b1/src/verifai/utils/utils.py`

 * *Files identical despite different names*

### Comparing `verifai-2.1.0/PKG-INFO` & `verifai-2.1.0b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 Metadata-Version: 2.1
 Name: verifai
-Version: 2.1.0
+Version: 2.1.0b1
 Summary: A toolkit for the formal design and analysis of systems that include artificial intelligence (AI) and machine learning (ML) components.
-Author: Tommaso Dreossi, Shromona Ghosh, Hadi Ravanbakhsh, Marcell Vazquez-Chanlatte, Sanjit A. Seshia
-Author-email: Daniel Fremont <dfremont@ucsc.edu>, Edward Kim <ek65@berkeley.edu>
-Maintainer-email: Daniel Fremont <dfremont@ucsc.edu>, Edward Kim <ek65@berkeley.edu>
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
+Home-page: https://github.com/BerkeleyLearnVerify/VerifAI
+License: BSD-3-Clause
+Author: Tommaso Dreossi
+Maintainer: Daniel Fremont
+Maintainer-email: dfremont@ucsc.edu
+Requires-Python: >=3.8,<3.11
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: numpy ~= 1.21
-Requires-Dist: scipy ~= 1.7
-Requires-Dist: dotmap ~= 1.3
-Requires-Dist: metric-temporal-logic >= 0.1.5
-Requires-Dist: matplotlib ~= 3.2
-Requires-Dist: easydict ~= 1.9
-Requires-Dist: joblib ~= 1.2
-Requires-Dist: dill >= 0.3.1
-Requires-Dist: future >= 0.18.3
-Requires-Dist: pandas ~= 1.3
-Requires-Dist: scikit-learn ~= 1.0
-Requires-Dist: pygame ~= 2.1
-Requires-Dist: kmodes <= 0.10.2
-Requires-Dist: scenic >= 2.1.0b1, <4
-Requires-Dist: progressbar2 ~= 3.53
-Requires-Dist: networkx >= 2.6
-Requires-Dist: statsmodels >= 0.13.2
-Requires-Dist: GPy ~= 1.9 ; extra == "bayesopt"
-Requires-Dist: GPyOpt ~= 1.2 ; extra == "bayesopt"
-Requires-Dist: verifai[test] ; extra == "dev"
-Requires-Dist: tox ~= 3.14 ; extra == "dev"
-Requires-Dist: sphinx >= 4.1.0, <6 ; extra == "dev"
-Requires-Dist: sphinx-rtd-theme >= 0.5.2 ; extra == "dev"
-Requires-Dist: sphinx-tabs ~= 3.4.1 ; extra == "dev"
-Requires-Dist: recommonmark >= 0.6.0 ; extra == "dev"
-Requires-Dist: tensorflow ~= 2.8 ; extra == "examples"
-Requires-Dist: gym >= 0.22 ; extra == "examples"
-Requires-Dist: pyglet ~= 1.5 ; extra == "examples"
-Requires-Dist: opencv-python ~= 4.5 ; extra == "examples"
-Requires-Dist: pillow ~= 9.3 ; extra == "examples"
-Requires-Dist: pyproj ~= 3.0 ; extra == "examples" and ( python_version < "3.10")
-Requires-Dist: pyproj ~= 3.3 ; extra == "examples" and ( python_version >= "3.10")
-Requires-Dist: ray ~= 1.10 ; extra == "parallel"
-Requires-Dist: pytest >= 6.2.5, <8 ; extra == "test"
-Requires-Dist: pytest-randomly >= 3.2 ; extra == "test"
-Project-URL: Documentation, https://verifai.readthedocs.io
-Project-URL: Repository, https://github.com/BerkeleyLearnVerify/VerifAI
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: bayesopt
 Provides-Extra: dev
 Provides-Extra: examples
 Provides-Extra: parallel
 Provides-Extra: test
+Requires-Dist: GPy (>=1.9.9,<2.0.0); extra == "bayesopt"
+Requires-Dist: GPyOpt (>=1.2.6,<2.0.0); extra == "bayesopt"
+Requires-Dist: dill (>=0.3.1,<0.4.0)
+Requires-Dist: dotmap (>=1.3.13,<2.0.0)
+Requires-Dist: easydict (>=1.9,<2.0)
+Requires-Dist: future (>=0.18.2,<0.19.0)
+Requires-Dist: gym (>=0.22,<0.23); extra == "examples"
+Requires-Dist: joblib (>=0.14.1,<0.15.0)
+Requires-Dist: kmodes (>=0.10.2,<0.11.0)
+Requires-Dist: matplotlib (>=3.2.1,<4.0.0)
+Requires-Dist: metric-temporal-logic (>=0.1.5,<0.2.0)
+Requires-Dist: networkx (>=2.6.3,<3.0.0)
+Requires-Dist: numpy (>=1.21.5,<2.0.0)
+Requires-Dist: opencv-python (>=4.5.3,<5.0.0); extra == "examples"
+Requires-Dist: pandas (>=1.3.5,<2.0.0)
+Requires-Dist: pillow (>=9.0.1,<10.0.0); extra == "examples"
+Requires-Dist: progressbar2 (>=3.53.1,<4.0.0)
+Requires-Dist: pygame (>=2.1.0,<3.0.0)
+Requires-Dist: pyglet (>=1.5.11,<2.0.0); extra == "examples"
+Requires-Dist: pyproj (>=3.0.0,<4.0.0); (python_version < "3.10") and (extra == "examples")
+Requires-Dist: pyproj (>=3.3.0,<4.0.0); python_version >= "3.10" and python_version < "4.0"
+Requires-Dist: pytest (>=6.2.5); extra == "dev" or extra == "test"
+Requires-Dist: pytest-randomly (>=3.2.1); extra == "dev" or extra == "test"
+Requires-Dist: ray (>=1.10.0,<2.0.0); extra == "parallel"
+Requires-Dist: recommonmark (>=0.6.0,<0.7.0); extra == "dev"
+Requires-Dist: scenic (>=2.1.0b4,<3.0.0)
+Requires-Dist: scikit-learn (>=1.0,<2.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Requires-Dist: sphinx (>=4.1.0,<6); extra == "dev"
+Requires-Dist: sphinx-rtd-theme (>=0.5.2,<0.6.0); extra == "dev"
+Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
+Requires-Dist: tensorflow (>=2.8.0,<3.0.0); extra == "examples"
+Requires-Dist: tox (>=3.14.0,<4.0.0); extra == "dev"
+Project-URL: Documentation, https://verifai.readthedocs.io
+Project-URL: Repository, https://github.com/BerkeleyLearnVerify/VerifAI
+Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/verifai/badge/?version=latest)](https://verifai.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
 
 
 # VerifAI
```

