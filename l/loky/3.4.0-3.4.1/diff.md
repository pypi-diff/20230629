# Comparing `tmp/loky-3.4.0.tar.gz` & `tmp/loky-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loky-3.4.0.tar", last modified: Fri Apr 14 16:50:41 2023, max compression
+gzip compressed data, was "loky-3.4.1.tar", last modified: Thu Jun 29 13:04:07 2023, max compression
```

## Comparing `loky-3.4.0.tar` & `loky-3.4.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.976706 loky-3.4.0/
--rw-r--r--   0 tom       (1000) users      (984)      272 2023-03-26 21:55:20.000000 loky-3.4.0/.coveragerc
--rw-r--r--   0 tom       (1000) users      (984)    11324 2023-04-14 16:50:38.000000 loky-3.4.0/CHANGES.md
--rw-r--r--   0 tom       (1000) users      (984)     1531 2023-03-26 21:55:20.000000 loky-3.4.0/LICENSE.txt
--rw-r--r--   0 tom       (1000) users      (984)      190 2023-03-26 21:55:20.000000 loky-3.4.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) users      (984)     6377 2023-04-14 16:50:41.976706 loky-3.4.0/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)     5367 2023-04-09 14:26:50.000000 loky-3.4.0/README.md
--rw-r--r--   0 tom       (1000) users      (984)     5507 2023-04-09 14:26:50.000000 loky-3.4.0/README.rst
--rw-r--r--   0 tom       (1000) users      (984)      106 2023-04-14 14:46:27.000000 loky-3.4.0/RELEASE.md
--rw-r--r--   0 tom       (1000) users      (984)     1681 2023-03-26 21:55:20.000000 loky-3.4.0/TODO.md
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.973373 loky-3.4.0/continuous_integration/
--rw-r--r--   0 tom       (1000) users      (984)      101 2023-03-26 21:55:20.000000 loky-3.4.0/continuous_integration/build_test_ext.sh
--rw-r--r--   0 tom       (1000) users      (984)      985 2023-03-26 21:55:20.000000 loky-3.4.0/continuous_integration/copy_loky.sh
--rw-r--r--   0 tom       (1000) users      (984)      483 2023-04-09 14:26:50.000000 loky-3.4.0/continuous_integration/install_coverage_subprocess_pth.py
--rwxr-xr-x   0 tom       (1000) users      (984)     1379 2023-04-14 12:50:20.000000 loky-3.4.0/continuous_integration/runtests.sh
--rw-rw-r--   0 tom       (1000) users      (984)      250 2023-03-01 07:00:12.000000 loky-3.4.0/frozen_loky.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.973373 loky-3.4.0/loky/
--rw-r--r--   0 tom       (1000) users      (984)     1104 2023-04-14 16:50:38.000000 loky-3.4.0/loky/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1057 2023-04-09 14:26:50.000000 loky-3.4.0/loky/_base.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.973373 loky-3.4.0/loky/backend/
--rw-r--r--   0 tom       (1000) users      (984)      312 2023-04-09 14:26:50.000000 loky-3.4.0/loky/backend/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)     1776 2023-04-09 14:26:50.000000 loky-3.4.0/loky/backend/_posix_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)      683 2023-04-14 10:41:06.000000 loky-3.4.0/loky/backend/_win_reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    13510 2023-04-14 10:41:06.000000 loky-3.4.0/loky/backend/context.py
--rw-r--r--   0 tom       (1000) users      (984)     1186 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/fork_exec.py
--rw-r--r--   0 tom       (1000) users      (984)     5580 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/popen_loky_posix.py
--rw-r--r--   0 tom       (1000) users      (984)     5308 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/popen_loky_win32.py
--rw-r--r--   0 tom       (1000) users      (984)     2018 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/process.py
--rw-r--r--   0 tom       (1000) users      (984)     7322 2023-04-09 14:26:50.000000 loky-3.4.0/loky/backend/queues.py
--rw-r--r--   0 tom       (1000) users      (984)     7024 2023-04-09 14:26:50.000000 loky-3.4.0/loky/backend/reduction.py
--rw-r--r--   0 tom       (1000) users      (984)    14498 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/resource_tracker.py
--rw-r--r--   0 tom       (1000) users      (984)     8962 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/spawn.py
--rw-r--r--   0 tom       (1000) users      (984)    11768 2023-04-14 12:50:20.000000 loky-3.4.0/loky/backend/synchronize.py
--rw-r--r--   0 tom       (1000) users      (984)     5757 2023-04-14 10:41:06.000000 loky-3.4.0/loky/backend/utils.py
--rw-r--r--   0 tom       (1000) users      (984)     3591 2023-04-09 14:26:50.000000 loky-3.4.0/loky/cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     2567 2023-04-09 14:26:50.000000 loky-3.4.0/loky/initializers.py
--rw-r--r--   0 tom       (1000) users      (984)    51050 2023-04-14 13:42:51.000000 loky-3.4.0/loky/process_executor.py
--rw-r--r--   0 tom       (1000) users      (984)    10310 2023-04-14 10:41:06.000000 loky-3.4.0/loky/reusable_executor.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.973373 loky-3.4.0/loky.egg-info/
--rw-r--r--   0 tom       (1000) users      (984)     6377 2023-04-14 16:50:41.000000 loky-3.4.0/loky.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) users      (984)     1577 2023-04-14 16:50:41.000000 loky-3.4.0/loky.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) users      (984)        1 2023-04-14 16:50:41.000000 loky-3.4.0/loky.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) users      (984)        1 2023-04-14 06:52:03.000000 loky-3.4.0/loky.egg-info/not-zip-safe
--rw-r--r--   0 tom       (1000) users      (984)       12 2023-04-14 16:50:41.000000 loky-3.4.0/loky.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) users      (984)        5 2023-04-14 16:50:41.000000 loky-3.4.0/loky.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) users      (984)      174 2023-04-09 14:26:50.000000 loky-3.4.0/pyproject.toml
--rw-rw-rw-   0 tom       (1000) users      (984)      156 2023-02-28 06:15:37.000000 loky-3.4.0/runtest.py
--rw-r--r--   0 tom       (1000) users      (984)       77 2023-04-14 16:50:41.976706 loky-3.4.0/setup.cfg
--rw-r--r--   0 tom       (1000) users      (984)     3310 2023-04-09 14:26:50.000000 loky-3.4.0/setup.py
--rw-rw-r--   0 tom       (1000) users      (984)      613 2023-02-27 16:31:39.000000 loky-3.4.0/test_freeze.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.976706 loky-3.4.0/tests/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:20.000000 loky-3.4.0/tests/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)    10562 2023-04-09 14:26:50.000000 loky-3.4.0/tests/_executor_mixin.py
-drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-04-14 16:50:41.976706 loky-3.4.0/tests/_openmp/
--rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:20.000000 loky-3.4.0/tests/_openmp/__init__.py
--rw-r--r--   0 tom       (1000) users      (984)      741 2023-04-09 14:26:50.000000 loky-3.4.0/tests/_openmp/_fail_fork.py
--rw-r--r--   0 tom       (1000) users      (984)      287 2023-03-26 21:55:20.000000 loky-3.4.0/tests/_openmp/parallel_sum.pyx
--rw-r--r--   0 tom       (1000) users      (984)      668 2023-04-09 14:26:50.000000 loky-3.4.0/tests/_openmp/setup.py
--rw-r--r--   0 tom       (1000) users      (984)    42704 2023-04-14 12:50:20.000000 loky-3.4.0/tests/_test_process_executor.py
--rw-r--r--   0 tom       (1000) users      (984)     1506 2023-04-09 14:26:50.000000 loky-3.4.0/tests/conftest.py
--rw-r--r--   0 tom       (1000) users      (984)     9839 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_cloudpickle_wrapper.py
--rw-r--r--   0 tom       (1000) users      (984)     8955 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_futures.py
--rw-r--r--   0 tom       (1000) users      (984)    24858 2023-04-14 12:50:20.000000 loky-3.4.0/tests/test_loky_backend.py
--rw-r--r--   0 tom       (1000) users      (984)     6512 2023-04-14 12:50:20.000000 loky-3.4.0/tests/test_loky_module.py
--rw-r--r--   0 tom       (1000) users      (984)     1070 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_process_executor_forkserver.py
--rw-r--r--   0 tom       (1000) users      (984)      792 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_process_executor_loky.py
--rw-r--r--   0 tom       (1000) users      (984)      908 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_process_executor_spawn.py
--rw-r--r--   0 tom       (1000) users      (984)    11769 2023-04-09 14:26:50.000000 loky-3.4.0/tests/test_resource_tracker.py
--rw-r--r--   0 tom       (1000) users      (984)    39116 2023-04-14 13:42:51.000000 loky-3.4.0/tests/test_reusable_executor.py
--rw-r--r--   0 tom       (1000) users      (984)    10391 2023-04-14 12:50:20.000000 loky-3.4.0/tests/test_synchronize.py
--rw-r--r--   0 tom       (1000) users      (984)     4443 2023-04-14 12:50:20.000000 loky-3.4.0/tests/test_worker_timeout.py
--rw-r--r--   0 tom       (1000) users      (984)     5883 2023-04-09 14:26:50.000000 loky-3.4.0/tests/utils.py
--rw-r--r--   0 tom       (1000) users      (984)     1251 2023-04-14 10:41:06.000000 loky-3.4.0/tox.ini
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.010032 loky-3.4.1/
+-rw-r--r--   0 tom       (1000) users      (984)      272 2023-03-26 21:55:20.000000 loky-3.4.1/.coveragerc
+-rw-r--r--   0 tom       (1000) users      (984)    11451 2023-06-29 13:03:41.000000 loky-3.4.1/CHANGES.md
+-rw-r--r--   0 tom       (1000) users      (984)     1531 2023-03-26 21:55:20.000000 loky-3.4.1/LICENSE.txt
+-rw-r--r--   0 tom       (1000) users      (984)      190 2023-03-26 21:55:20.000000 loky-3.4.1/MANIFEST.in
+-rw-r--r--   0 tom       (1000) users      (984)     6377 2023-06-29 13:04:07.010032 loky-3.4.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)     5367 2023-04-09 14:26:50.000000 loky-3.4.1/README.md
+-rw-r--r--   0 tom       (1000) users      (984)     5507 2023-04-09 14:26:50.000000 loky-3.4.1/README.rst
+-rw-r--r--   0 tom       (1000) users      (984)      106 2023-04-14 14:46:27.000000 loky-3.4.1/RELEASE.md
+-rw-r--r--   0 tom       (1000) users      (984)     1681 2023-03-26 21:55:20.000000 loky-3.4.1/TODO.md
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.006698 loky-3.4.1/continuous_integration/
+-rw-r--r--   0 tom       (1000) users      (984)      101 2023-03-26 21:55:20.000000 loky-3.4.1/continuous_integration/build_test_ext.sh
+-rw-r--r--   0 tom       (1000) users      (984)      985 2023-03-26 21:55:20.000000 loky-3.4.1/continuous_integration/copy_loky.sh
+-rw-r--r--   0 tom       (1000) users      (984)      483 2023-04-09 14:26:50.000000 loky-3.4.1/continuous_integration/install_coverage_subprocess_pth.py
+-rwxr-xr-x   0 tom       (1000) users      (984)     1379 2023-04-14 12:50:20.000000 loky-3.4.1/continuous_integration/runtests.sh
+-rw-rw-r--   0 tom       (1000) users      (984)      250 2023-03-01 07:00:12.000000 loky-3.4.1/frozen_loky.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.006698 loky-3.4.1/loky/
+-rw-r--r--   0 tom       (1000) users      (984)     1104 2023-06-29 13:03:41.000000 loky-3.4.1/loky/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1057 2023-04-09 14:26:50.000000 loky-3.4.1/loky/_base.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.010032 loky-3.4.1/loky/backend/
+-rw-r--r--   0 tom       (1000) users      (984)      312 2023-04-09 14:26:50.000000 loky-3.4.1/loky/backend/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)     1776 2023-04-09 14:26:50.000000 loky-3.4.1/loky/backend/_posix_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)      683 2023-04-14 10:41:06.000000 loky-3.4.1/loky/backend/_win_reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    13654 2023-06-29 13:03:41.000000 loky-3.4.1/loky/backend/context.py
+-rw-r--r--   0 tom       (1000) users      (984)     1186 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/fork_exec.py
+-rw-r--r--   0 tom       (1000) users      (984)     5580 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/popen_loky_posix.py
+-rw-r--r--   0 tom       (1000) users      (984)     5308 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/popen_loky_win32.py
+-rw-r--r--   0 tom       (1000) users      (984)     2018 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/process.py
+-rw-r--r--   0 tom       (1000) users      (984)     7322 2023-04-09 14:26:50.000000 loky-3.4.1/loky/backend/queues.py
+-rw-r--r--   0 tom       (1000) users      (984)     7024 2023-04-09 14:26:50.000000 loky-3.4.1/loky/backend/reduction.py
+-rw-r--r--   0 tom       (1000) users      (984)    14498 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/resource_tracker.py
+-rw-r--r--   0 tom       (1000) users      (984)     8962 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/spawn.py
+-rw-r--r--   0 tom       (1000) users      (984)    11768 2023-04-14 12:50:20.000000 loky-3.4.1/loky/backend/synchronize.py
+-rw-r--r--   0 tom       (1000) users      (984)     5757 2023-04-14 10:41:06.000000 loky-3.4.1/loky/backend/utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     3591 2023-04-09 14:26:50.000000 loky-3.4.1/loky/cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     2567 2023-04-09 14:26:50.000000 loky-3.4.1/loky/initializers.py
+-rw-r--r--   0 tom       (1000) users      (984)    51050 2023-04-14 13:42:51.000000 loky-3.4.1/loky/process_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)    10310 2023-04-14 10:41:06.000000 loky-3.4.1/loky/reusable_executor.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.006698 loky-3.4.1/loky.egg-info/
+-rw-r--r--   0 tom       (1000) users      (984)     6377 2023-06-29 13:04:06.000000 loky-3.4.1/loky.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) users      (984)     1577 2023-06-29 13:04:06.000000 loky-3.4.1/loky.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) users      (984)        1 2023-06-29 13:04:06.000000 loky-3.4.1/loky.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) users      (984)        1 2023-04-14 06:52:03.000000 loky-3.4.1/loky.egg-info/not-zip-safe
+-rw-r--r--   0 tom       (1000) users      (984)       12 2023-06-29 13:04:06.000000 loky-3.4.1/loky.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) users      (984)        5 2023-06-29 13:04:06.000000 loky-3.4.1/loky.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) users      (984)      174 2023-04-09 14:26:50.000000 loky-3.4.1/pyproject.toml
+-rw-rw-rw-   0 tom       (1000) users      (984)      156 2023-02-28 06:15:37.000000 loky-3.4.1/runtest.py
+-rw-r--r--   0 tom       (1000) users      (984)       77 2023-06-29 13:04:07.010032 loky-3.4.1/setup.cfg
+-rw-r--r--   0 tom       (1000) users      (984)     3307 2023-06-29 13:03:41.000000 loky-3.4.1/setup.py
+-rw-rw-r--   0 tom       (1000) users      (984)      613 2023-02-27 16:31:39.000000 loky-3.4.1/test_freeze.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.010032 loky-3.4.1/tests/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:20.000000 loky-3.4.1/tests/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)    10562 2023-04-09 14:26:50.000000 loky-3.4.1/tests/_executor_mixin.py
+drwxr-xr-x   0 tom       (1000) users      (984)        0 2023-06-29 13:04:07.010032 loky-3.4.1/tests/_openmp/
+-rw-r--r--   0 tom       (1000) users      (984)        0 2023-03-26 21:55:20.000000 loky-3.4.1/tests/_openmp/__init__.py
+-rw-r--r--   0 tom       (1000) users      (984)      741 2023-04-09 14:26:50.000000 loky-3.4.1/tests/_openmp/_fail_fork.py
+-rw-r--r--   0 tom       (1000) users      (984)      287 2023-03-26 21:55:20.000000 loky-3.4.1/tests/_openmp/parallel_sum.pyx
+-rw-r--r--   0 tom       (1000) users      (984)      668 2023-04-09 14:26:50.000000 loky-3.4.1/tests/_openmp/setup.py
+-rw-r--r--   0 tom       (1000) users      (984)    42704 2023-04-14 12:50:20.000000 loky-3.4.1/tests/_test_process_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)     1506 2023-04-09 14:26:50.000000 loky-3.4.1/tests/conftest.py
+-rw-r--r--   0 tom       (1000) users      (984)     9839 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_cloudpickle_wrapper.py
+-rw-r--r--   0 tom       (1000) users      (984)     8955 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_futures.py
+-rw-r--r--   0 tom       (1000) users      (984)    24858 2023-04-14 12:50:20.000000 loky-3.4.1/tests/test_loky_backend.py
+-rw-r--r--   0 tom       (1000) users      (984)     6512 2023-04-14 12:50:20.000000 loky-3.4.1/tests/test_loky_module.py
+-rw-r--r--   0 tom       (1000) users      (984)     1070 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_process_executor_forkserver.py
+-rw-r--r--   0 tom       (1000) users      (984)      792 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_process_executor_loky.py
+-rw-r--r--   0 tom       (1000) users      (984)      908 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_process_executor_spawn.py
+-rw-r--r--   0 tom       (1000) users      (984)    11769 2023-04-09 14:26:50.000000 loky-3.4.1/tests/test_resource_tracker.py
+-rw-r--r--   0 tom       (1000) users      (984)    39116 2023-04-14 13:42:51.000000 loky-3.4.1/tests/test_reusable_executor.py
+-rw-r--r--   0 tom       (1000) users      (984)    10391 2023-04-14 12:50:20.000000 loky-3.4.1/tests/test_synchronize.py
+-rw-r--r--   0 tom       (1000) users      (984)     4443 2023-04-14 12:50:20.000000 loky-3.4.1/tests/test_worker_timeout.py
+-rw-r--r--   0 tom       (1000) users      (984)     5883 2023-04-09 14:26:50.000000 loky-3.4.1/tests/utils.py
+-rw-r--r--   0 tom       (1000) users      (984)     1251 2023-04-14 10:41:06.000000 loky-3.4.1/tox.ini
```

### Comparing `loky-3.4.0/CHANGES.md` & `loky-3.4.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+### 3.4.1 - 2023-06-29
+
+- Fix compatibility with python3.7, which does not define
+  a `_MAX_WINDOWS_WORKERS` constant. (#408)
+
 ### 3.4.0 - 2023-04-14
 
 - Fix exception `__cause__` not being propagated with
   `tblib.pickling_support.install()`. (#255).
 
 - Fix handling of CPU affinity  by using `psutil`'s `cpu_affinity` on platforms
   that do not implement `os.sched_getaffinity`, such as PyPy. (#381).
```

### Comparing `loky-3.4.0/LICENSE.txt` & `loky-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/PKG-INFO` & `loky-3.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loky
-Version: 3.4.0
+Version: 3.4.1
 Summary: A robust implementation of concurrent.futures.ProcessPoolExecutor
 Home-page: https://github.com/joblib/loky/
 Author: Thomas Moreau
 Author-email: thomas.moreau.2010@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `loky-3.4.0/README.md` & `loky-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/README.rst` & `loky-3.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/TODO.md` & `loky-3.4.1/TODO.md`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/continuous_integration/copy_loky.sh` & `loky-3.4.1/continuous_integration/copy_loky.sh`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/continuous_integration/runtests.sh` & `loky-3.4.1/continuous_integration/runtests.sh`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/__init__.py` & `loky-3.4.1/loky/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,8 +37,8 @@
     "FIRST_EXCEPTION",
     "ALL_COMPLETED",
     "wrap_non_picklable_objects",
     "set_loky_pickler",
 ]
 
 
-__version__ = "3.4.0"
+__version__ = "3.4.1"
```

### Comparing `loky-3.4.0/loky/_base.py` & `loky-3.4.1/loky/_base.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/_posix_reduction.py` & `loky-3.4.1/loky/backend/_posix_reduction.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/_win_reduction.py` & `loky-3.4.1/loky/backend/_win_reduction.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/context.py` & `loky-3.4.1/loky/backend/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,22 +14,28 @@
 import math
 import subprocess
 import traceback
 import warnings
 import multiprocessing as mp
 from multiprocessing import get_context as mp_get_context
 from multiprocessing.context import BaseContext
-from concurrent.futures.process import _MAX_WINDOWS_WORKERS
+
 
 from .process import LokyProcess, LokyInitMainProcess
 
 # Apparently, on older Python versions, loky cannot work 61 workers on Windows
 # but instead 60: ¯\_(ツ)_/¯
-if sys.version_info < (3, 10):
-    _MAX_WINDOWS_WORKERS = _MAX_WINDOWS_WORKERS - 1
+if sys.version_info >= (3, 8):
+    from concurrent.futures.process import _MAX_WINDOWS_WORKERS
+
+    if sys.version_info < (3, 10):
+        _MAX_WINDOWS_WORKERS = _MAX_WINDOWS_WORKERS - 1
+else:
+    # compat for versions before 3.8 which do not define this.
+    _MAX_WINDOWS_WORKERS = 60
 
 START_METHODS = ["loky", "loky_init_main", "spawn"]
 if sys.platform != "win32":
     START_METHODS += ["fork", "forkserver"]
 
 _DEFAULT_START_METHOD = None
```

### Comparing `loky-3.4.0/loky/backend/fork_exec.py` & `loky-3.4.1/loky/backend/fork_exec.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/popen_loky_posix.py` & `loky-3.4.1/loky/backend/popen_loky_posix.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/popen_loky_win32.py` & `loky-3.4.1/loky/backend/popen_loky_win32.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/process.py` & `loky-3.4.1/loky/backend/process.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/queues.py` & `loky-3.4.1/loky/backend/queues.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/reduction.py` & `loky-3.4.1/loky/backend/reduction.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/resource_tracker.py` & `loky-3.4.1/loky/backend/resource_tracker.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/spawn.py` & `loky-3.4.1/loky/backend/spawn.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/synchronize.py` & `loky-3.4.1/loky/backend/synchronize.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/backend/utils.py` & `loky-3.4.1/loky/backend/utils.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/cloudpickle_wrapper.py` & `loky-3.4.1/loky/cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/initializers.py` & `loky-3.4.1/loky/initializers.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/process_executor.py` & `loky-3.4.1/loky/process_executor.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky/reusable_executor.py` & `loky-3.4.1/loky/reusable_executor.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/loky.egg-info/PKG-INFO` & `loky-3.4.1/loky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loky
-Version: 3.4.0
+Version: 3.4.1
 Summary: A robust implementation of concurrent.futures.ProcessPoolExecutor
 Home-page: https://github.com/joblib/loky/
 Author: Thomas Moreau
 Author-email: thomas.moreau.2010@gmail.com
 License: BSD
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `loky-3.4.0/loky.egg-info/SOURCES.txt` & `loky-3.4.1/loky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/setup.py` & `loky-3.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 cmdclass = {"clean": CleanCommand}
 
 setup(
     name="loky",
     version=find_version(),
     description=(
-        "A robust implementation of " "concurrent.futures.ProcessPoolExecutor"
+        "A robust implementation of concurrent.futures.ProcessPoolExecutor"
     ),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/joblib/loky/",
     author="Thomas Moreau",
     author_email="thomas.moreau.2010@gmail.com",
     packages=packages,
```

### Comparing `loky-3.4.0/test_freeze.py` & `loky-3.4.1/test_freeze.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/_executor_mixin.py` & `loky-3.4.1/tests/_executor_mixin.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/_openmp/_fail_fork.py` & `loky-3.4.1/tests/_openmp/_fail_fork.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/_openmp/setup.py` & `loky-3.4.1/tests/_openmp/setup.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/_test_process_executor.py` & `loky-3.4.1/tests/_test_process_executor.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/conftest.py` & `loky-3.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_cloudpickle_wrapper.py` & `loky-3.4.1/tests/test_cloudpickle_wrapper.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_futures.py` & `loky-3.4.1/tests/test_futures.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_loky_backend.py` & `loky-3.4.1/tests/test_loky_backend.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_loky_module.py` & `loky-3.4.1/tests/test_loky_module.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_process_executor_forkserver.py` & `loky-3.4.1/tests/test_process_executor_forkserver.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_process_executor_loky.py` & `loky-3.4.1/tests/test_process_executor_loky.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_process_executor_spawn.py` & `loky-3.4.1/tests/test_process_executor_spawn.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_resource_tracker.py` & `loky-3.4.1/tests/test_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_reusable_executor.py` & `loky-3.4.1/tests/test_reusable_executor.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_synchronize.py` & `loky-3.4.1/tests/test_synchronize.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/test_worker_timeout.py` & `loky-3.4.1/tests/test_worker_timeout.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tests/utils.py` & `loky-3.4.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `loky-3.4.0/tox.ini` & `loky-3.4.1/tox.ini`

 * *Files identical despite different names*

