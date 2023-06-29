# Comparing `tmp/UpyTest-3.1.6.tar.gz` & `tmp/UpyTest-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UpyTest-3.1.6.tar", last modified: Wed Jun 28 23:30:38 2023, max compression
+gzip compressed data, was "UpyTest-3.1.7.tar", last modified: Thu Jun 29 20:34:56 2023, max compression
```

## Comparing `UpyTest-3.1.6.tar` & `UpyTest-3.1.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.600284 UpyTest-3.1.6/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-28 23:30:38.596284 UpyTest-3.1.6/PKG-INFO
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.588284 UpyTest-3.1.6/UpyTest.egg-info/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-28 23:30:38.000000 UpyTest-3.1.6/UpyTest.egg-info/PKG-INFO
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2351 2023-06-28 23:30:38.000000 UpyTest-3.1.6/UpyTest.egg-info/SOURCES.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-28 23:30:38.000000 UpyTest-3.1.6/UpyTest.egg-info/dependency_links.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-28 23:30:38.000000 UpyTest-3.1.6/UpyTest.egg-info/requires.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-28 23:30:38.000000 UpyTest-3.1.6/UpyTest.egg-info/top_level.txt
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-28 23:30:38.600284 UpyTest-3.1.6/setup.cfg
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-28 23:30:28.000000 UpyTest-3.1.6/setup.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.588284 UpyTest-3.1.6/thonnycontrib/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.6/thonnycontrib/ThonnyLogsGenerator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.6/thonnycontrib/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.588284 UpyTest-3.1.6/thonnycontrib/backend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/backend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.6/thonnycontrib/backend/ast_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35404 2023-06-28 23:27:31.000000 UpyTest-3.1.6/thonnycontrib/backend/doctest_parser.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.6/thonnycontrib/backend/evaluator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4503 2023-06-25 22:01:28.000000 UpyTest-3.1.6/thonnycontrib/backend/l1test_backend.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.6/thonnycontrib/backend/test_finder.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.592284 UpyTest-3.1.6/thonnycontrib/backend/verdicts/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/ExampleVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/ExceptionVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/FailedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/PassedVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/SetupVerdict.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.6/thonnycontrib/backend/verdicts/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.592284 UpyTest-3.1.6/thonnycontrib/docs/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/__init__.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.592284 UpyTest-3.1.6/thonnycontrib/docs/res/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.6/thonnycontrib/docs/res/error_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/failed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1468 2023-06-25 02:50:15.000000 UpyTest-3.1.6/thonnycontrib/docs/res/l1test_debug.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/l1test_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/l1test_icon_old.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.6/thonnycontrib/docs/res/outline_class.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.6/thonnycontrib/docs/res/outline_method.gif
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/passed.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/pending_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.6/thonnycontrib/docs/res/restart_icon.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/test_only_btn.png
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docs/res/warning.png
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.596284 UpyTest-3.1.6/thonnycontrib/docstring_generator/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docstring_generator/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.6/thonnycontrib/docstring_generator/doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/docstring_generator/doc_template.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1315 2023-06-25 20:12:20.000000 UpyTest-3.1.6/thonnycontrib/environement_vars.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-06-28 23:02:20.000000 UpyTest-3.1.6/thonnycontrib/exceptions.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.596284 UpyTest-3.1.6/thonnycontrib/l1test_configuration/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.6/thonnycontrib/l1test_configuration/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.6/thonnycontrib/l1test_configuration/l1test_options.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.596284 UpyTest-3.1.6/thonnycontrib/l1test_frontend/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2507 2023-06-25 03:08:15.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_error_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2756 2023-06-25 13:23:15.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_reporter.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23240 2023-06-26 21:41:29.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_runner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36572 2023-06-28 00:14:02.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_treeview.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3523 2023-06-25 21:48:20.000000 UpyTest-3.1.6/thonnycontrib/l1test_frontend/outlines.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7311 2023-06-26 21:06:12.000000 UpyTest-3.1.6/thonnycontrib/plugin_loader.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2485 2023-06-26 23:21:42.000000 UpyTest-3.1.6/thonnycontrib/properties.py
-drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-28 23:30:38.596284 UpyTest-3.1.6/thonnycontrib/tests/
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.6/thonnycontrib/tests/__init__.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.6/thonnycontrib/tests/backend_mock.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.6/thonnycontrib/tests/test_doc_generator.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_example_no_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_example_with_exception.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_example_with_expected.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9799 2023-06-25 13:23:15.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_l1TestRunner.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_test_finder.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.6/thonnycontrib/tests/tests_view.py
--rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    19104 2023-06-28 23:23:13.000000 UpyTest-3.1.6/thonnycontrib/utils.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.831750 UpyTest-3.1.7/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-29 20:34:56.831750 UpyTest-3.1.7/PKG-INFO
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.823751 UpyTest-3.1.7/UpyTest.egg-info/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      694 2023-06-29 20:34:56.000000 UpyTest-3.1.7/UpyTest.egg-info/PKG-INFO
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2351 2023-06-29 20:34:56.000000 UpyTest-3.1.7/UpyTest.egg-info/SOURCES.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        1 2023-06-29 20:34:56.000000 UpyTest-3.1.7/UpyTest.egg-info/dependency_links.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-29 20:34:56.000000 UpyTest-3.1.7/UpyTest.egg-info/requires.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       14 2023-06-29 20:34:56.000000 UpyTest-3.1.7/UpyTest.egg-info/top_level.txt
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)       38 2023-06-29 20:34:56.831750 UpyTest-3.1.7/setup.cfg
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1985 2023-06-29 20:34:50.000000 UpyTest-3.1.7/setup.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.823751 UpyTest-3.1.7/thonnycontrib/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      947 2023-06-24 22:43:54.000000 UpyTest-3.1.7/thonnycontrib/ThonnyLogsGenerator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 22:52:20.000000 UpyTest-3.1.7/thonnycontrib/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.823751 UpyTest-3.1.7/thonnycontrib/backend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/backend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    16304 2023-06-24 19:59:14.000000 UpyTest-3.1.7/thonnycontrib/backend/ast_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    35404 2023-06-28 23:27:31.000000 UpyTest-3.1.7/thonnycontrib/backend/doctest_parser.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     5028 2023-06-24 15:10:56.000000 UpyTest-3.1.7/thonnycontrib/backend/evaluator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4503 2023-06-25 22:01:28.000000 UpyTest-3.1.7/thonnycontrib/backend/l1test_backend.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6541 2023-06-24 18:11:15.000000 UpyTest-3.1.7/thonnycontrib/backend/test_finder.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/backend/verdicts/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2057 2023-06-24 19:29:56.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/ExampleVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      496 2023-06-24 18:12:47.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/ExceptionVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      733 2023-06-24 18:13:06.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/FailedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      637 2023-06-24 19:25:27.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      450 2023-06-24 18:12:56.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/PassedVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      377 2023-06-24 18:13:00.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/SetupVerdict.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-24 02:35:02.000000 UpyTest-3.1.7/thonnycontrib/backend/verdicts/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/docs/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/__init__.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/docs/res/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      912 2023-06-21 22:17:10.000000 UpyTest-3.1.7/thonnycontrib/docs/res/error_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1275 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/failed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1468 2023-06-25 02:50:15.000000 UpyTest-3.1.7/thonnycontrib/docs/res/l1test_debug.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2130 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/l1test_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2086 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/l1test_icon_old.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      628 2023-04-23 12:41:34.000000 UpyTest-3.1.7/thonnycontrib/docs/res/outline_class.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      578 2023-04-23 12:41:32.000000 UpyTest-3.1.7/thonnycontrib/docs/res/outline_method.gif
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1213 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/passed.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1531 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/pending_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      997 2023-06-21 22:19:21.000000 UpyTest-3.1.7/thonnycontrib/docs/res/restart_icon.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2282 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/test_only_btn.png
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1073 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docs/res/warning.png
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/docstring_generator/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docstring_generator/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     8660 2023-06-24 13:42:03.000000 UpyTest-3.1.7/thonnycontrib/docstring_generator/doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7134 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/docstring_generator/doc_template.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1315 2023-06-25 20:12:20.000000 UpyTest-3.1.7/thonnycontrib/environement_vars.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3712 2023-06-28 23:02:20.000000 UpyTest-3.1.7/thonnycontrib/exceptions.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/l1test_configuration/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:40.000000 UpyTest-3.1.7/thonnycontrib/l1test_configuration/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2575 2023-04-02 02:23:42.000000 UpyTest-3.1.7/thonnycontrib/l1test_configuration/l1test_options.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.827751 UpyTest-3.1.7/thonnycontrib/l1test_frontend/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      708 2023-06-24 22:52:29.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2507 2023-06-25 03:08:15.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_error_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2756 2023-06-25 13:23:15.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_reporter.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    23240 2023-06-26 21:41:29.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_runner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    36844 2023-06-29 02:50:23.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_treeview.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     3523 2023-06-25 21:48:20.000000 UpyTest-3.1.7/thonnycontrib/l1test_frontend/outlines.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     7311 2023-06-26 21:06:12.000000 UpyTest-3.1.7/thonnycontrib/plugin_loader.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     2485 2023-06-26 23:21:42.000000 UpyTest-3.1.7/thonnycontrib/properties.py
+drwxrwxr-x   0 idtaleb   (1000) idtaleb   (1000)        0 2023-06-29 20:34:56.831750 UpyTest-3.1.7/thonnycontrib/tests/
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)        0 2023-03-15 10:38:42.000000 UpyTest-3.1.7/thonnycontrib/tests/__init__.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)      348 2023-03-15 10:38:42.000000 UpyTest-3.1.7/thonnycontrib/tests/backend_mock.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     1980 2023-03-15 10:38:42.000000 UpyTest-3.1.7/thonnycontrib/tests/test_doc_generator.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     4848 2023-06-24 02:33:48.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_example_no_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    14741 2023-06-24 02:34:31.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_example_with_exception.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    18496 2023-06-24 02:34:31.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_example_with_expected.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     9799 2023-06-25 13:23:15.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_l1TestRunner.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)     6392 2023-06-23 23:27:45.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_test_finder.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    12629 2023-06-24 02:34:31.000000 UpyTest-3.1.7/thonnycontrib/tests/tests_view.py
+-rw-rw-r--   0 idtaleb   (1000) idtaleb   (1000)    19128 2023-06-29 01:32:13.000000 UpyTest-3.1.7/thonnycontrib/utils.py
```

### Comparing `UpyTest-3.1.6/PKG-INFO` & `UpyTest-3.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.6
+Version: 3.1.7
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.6/UpyTest.egg-info/PKG-INFO` & `UpyTest-3.1.7/UpyTest.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UpyTest
-Version: 3.1.6
+Version: 3.1.7
 Summary: A plug-in which adds a test framework
 Home-page: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework
 Author: Réda Id-taleb
 Platform: Windows
 Platform: macOS
 Platform: Linux
 Classifier: Topic :: Education :: Testing
```

### Comparing `UpyTest-3.1.6/UpyTest.egg-info/SOURCES.txt` & `UpyTest-3.1.7/UpyTest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/setup.py` & `UpyTest-3.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return py_packs | other_packs
 
 setupdir = os.path.dirname(__file__)
 
 
 setup(
     name="UpyTest",
-    version="3.1.6",
+    version="3.1.7",
     author="Réda Id-taleb",
     description="A plug-in which adds a test framework",
     long_description="""A plug-in for Thonny which allows you to test your doc examples
  
 More info: https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework""",
     url="https://gitlab.univ-lille.fr/reda.idtaleb.etu/thonny_test_framework",
 #    keywords="IDE education programming tests in documentation",
```

### Comparing `UpyTest-3.1.6/thonnycontrib/ThonnyLogsGenerator.py` & `UpyTest-3.1.7/thonnycontrib/ThonnyLogsGenerator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/ast_parser.py` & `UpyTest-3.1.7/thonnycontrib/backend/ast_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/doctest_parser.py` & `UpyTest-3.1.7/thonnycontrib/backend/doctest_parser.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/evaluator.py` & `UpyTest-3.1.7/thonnycontrib/backend/evaluator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/l1test_backend.py` & `UpyTest-3.1.7/thonnycontrib/backend/l1test_backend.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/test_finder.py` & `UpyTest-3.1.7/thonnycontrib/backend/test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/verdicts/ExampleVerdict.py` & `UpyTest-3.1.7/thonnycontrib/backend/verdicts/ExampleVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/verdicts/FailedVerdict.py` & `UpyTest-3.1.7/thonnycontrib/backend/verdicts/FailedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py` & `UpyTest-3.1.7/thonnycontrib/backend/verdicts/FailedWhenExceptionExpectedVerdict.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/error_icon.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/error_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/failed.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/failed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/l1test_debug.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/l1test_debug.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/l1test_icon.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/l1test_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/l1test_icon_old.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/l1test_icon_old.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/outline_class.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/outline_class.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/outline_method.gif` & `UpyTest-3.1.7/thonnycontrib/docs/res/outline_method.gif`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/passed.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/passed.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/pending_icon.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/pending_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/restart_icon.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/restart_icon.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/test_only_btn.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/test_only_btn.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docs/res/warning.png` & `UpyTest-3.1.7/thonnycontrib/docs/res/warning.png`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docstring_generator/doc_generator.py` & `UpyTest-3.1.7/thonnycontrib/docstring_generator/doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/docstring_generator/doc_template.py` & `UpyTest-3.1.7/thonnycontrib/docstring_generator/doc_template.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/environement_vars.py` & `UpyTest-3.1.7/thonnycontrib/environement_vars.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/exceptions.py` & `UpyTest-3.1.7/thonnycontrib/exceptions.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_configuration/l1test_options.py` & `UpyTest-3.1.7/thonnycontrib/l1test_configuration/l1test_options.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/__init__.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_error_view.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_error_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_reporter.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_reporter.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_runner.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_runner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/l1test_treeview.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/l1test_treeview.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from typing import Dict, List
 from copy import deepcopy
 
 # La hauteur, par défault, d'une ligne dans une Treeview
 ROW_HEIGHT = 40
 
 SMALL_MARGIN = 1.1
-NORMAL_MARGIN = 1.2
+NORMAL_MARGIN = 1.17
 
 clickable_tag = "clickable"
 
 # L'objet qui représente un summarize
 Summarize = namedtuple('Summarize', ["total", "success", "failures", "errors", "empty"])
 
 # Palette de couleurs utilisée par la treeview
@@ -34,24 +34,32 @@
                 'lightred': '#fcdbd9',
                 'darkred': '#f7140c',
                 'green': 'darkgreen',
                 'blue': '#0000cc',
                 'gray': 'gray'
             }
 
+## Binding sequence for the treeview dictionary
+ALT_I = "<Alt-i>"
+ALT_D = "<Alt-d>"
+ALT_F = "<Alt-f>"
+ALT_U = "<Alt-u>"
+ALT_O = "<Alt-o>"
+BINDS = {ALT_I: "Alt+i", ALT_D: "Alt+d", ALT_F: "Alt+f", ALT_U: "Alt+u", ALT_O: "Alt+o"}
+
+
 class L1TestTreeView(ttk.Frame):    
     def __init__(self, master=None):
         ttk.Frame.__init__(self, master, borderwidth=0, relief="flat")
         self.workbench = thonny.get_workbench()
-        
-        self._init_treeview()
-        
         self._origin_l1doctests: List[L1DocTest] = dict()
         self._copy_l1doctests = self._origin_l1doctests.copy()
         
+        self._init_treeview()
+        
         # Le binding est censé augmenter/diminuer automatiquement la taille de la treeview
         self.workbench.bind("<Control-plus>", self.__observe_font_changing, True)
         self.workbench.bind("<Control-minus>", self.__observe_font_changing, True)
             
     def _init_treeview(self):
         """
         Creates the treeview widget.
@@ -100,21 +108,23 @@
 
         self.image_references["pending_icon.png"] = get_photoImage("pending_icon.png")
         self.image_references["error_icon.png"] = get_photoImage("error_icon.png")
         self.image_references["restart_icon.png"] = get_photoImage("restart_icon.png")
         
         # add a menu to the treeview
         self.menu = tk.Menu(self.treeview, name="menu", tearoff=False)
-        
+          
         # Here we handle the motion event of the treeview 
         self.treeview.bind("<Configure>", partial(self.__wrap_tree_content, self.treeview))
-        self.treeview.bind("<Shift-I>", self.increase_row_height, True)
-        self.treeview.bind("<Shift-D>", self.decrease_row_height, True)
-        self.workbench.bind("<Shift-F>", self.update_font, True)
-
+        self.workbench.bind(ALT_I, self.increase_row_height, True)
+        self.workbench.bind(ALT_D, self.decrease_row_height, True)
+        self.workbench.bind(ALT_F, self.update_font, True)
+        self.workbench.bind(ALT_U, self.unfold_rows, True) 
+        self.workbench.bind(ALT_O, self.fold_rows, True)
+        
     # ------------------------------------
     # Fonctions pour le Header du treeview
     # ------------------------------------
     
     def init_header(self, row=0, column=0):
         """
         Initialize the header of the treeview. Initially, the header contains 
@@ -181,20 +191,20 @@
         self.menu.add_command(label=RESUME_ORIGINAL_ORDER, command=self.remove_sort_filter)
         self.menu.add_separator() 
         self.menu.add_command(label=SHOW_ONLY_RED_TESTS, command=self.show_only_red_tests)
         self.menu.add_command(label=SHOW_ALL_TESTS, command=self.show_all_tests)
         self.menu.add_separator()
         self.menu.add_command(label=GROUP_BY_VERDICTS, command=self.group_by_verdicts)
         self.menu.add_separator()    
-        self.menu.add_command(label=EXPAND_TEST_RESULTS, command=self.expand_rows) 
-        self.menu.add_command(label=FOLD_TEST_RESULTS, command=self.fold_rows)
+        self.menu.add_command(label=EXPAND_TEST_RESULTS, command=self.unfold_rows, accelerator=BINDS[ALT_U]) 
+        self.menu.add_command(label=FOLD_TEST_RESULTS, command=self.fold_rows, accelerator=BINDS[ALT_O])
         self.menu.add_separator() 
-        self.menu.add_command(label=UPDATE_FONT_LABEL, command=self.update_font, accelerator="Shift+f")
-        self.menu.add_command(label=INCREASE_SPACE_BETWEEN_ROWS, command=self.increase_row_height, accelerator="Shift+i")
-        self.menu.add_command(label=DECREASE_SPACE_BETWEEN_ROWS, command=self.decrease_row_height, accelerator="Shift+d")
+        self.menu.add_command(label=UPDATE_FONT_LABEL, command=self.update_font, accelerator=BINDS[ALT_F])
+        self.menu.add_command(label=INCREASE_SPACE_BETWEEN_ROWS, command=self.increase_row_height, accelerator=BINDS[ALT_I])
+        self.menu.add_command(label=DECREASE_SPACE_BETWEEN_ROWS, command=self.decrease_row_height, accelerator=BINDS[ALT_D])
         self.menu.add_command(label=REMOVE_ERROR_DETAILS if not get_option(EXCEPTION_DETAIL) else INCLUDE_ERROR_DETAILS, 
                               command=self.remove_error_details)
         self.menu.add_separator()
         self.menu.add_command(label=CLEAR_LABEL, command=self.clear_tree) 
          
     def resize_header_bar(self, event=None):
         """
@@ -210,26 +220,19 @@
             time when the treeview was refreshed. 
             
             It also update the font size of the treeview if and 
             only if the font is changed in thonny.
             
             Note : if a row of the treeview is selected so the effect of the selection will 
             be removed after refresh.
-        """
-        all_childs = get_all_tree_childrens(self.treeview)
-        rowheight = ROW_HEIGHT
-        if all_childs:
-            # on calcule le meilleure height à appliquer pour la treeview.
-            # Cela est fait quand la taille de la police a changé dans thonny.
-            rowheight = self.get_optimal_row_height(all_childs)
-                     
+        """          
         self.resize_header_bar()
         # on applique la nouvelle police pour la treeview
-        self.__observe_font_changing(rowheight=rowheight)
-    
+        self.__observe_font_changing()
+     
     def sort_by_red_tests(self):
         
         # On filtre que les l1doctest qui ont un flag rouge.
         sorted_failed_nodes = [l1doctest for l1doctest in self._copy_l1doctests if l1doctest.get_flag() == L1DocTestFlag.FAILED_FLAG ]
         
         # On met les tests rouges en haut et cela pour tous les l1doctest qui ont au moins un test rouge.
         sorted_failed_tests = []
@@ -320,19 +323,19 @@
         if self.treeview.get_children(): # on met à jour que si la treeview possède des éléments
             self.clear_tree(clear_all=False) 
             for status, l1doctests in grouped.items():
                 row_id = self.insert_row(text=status.short_name(), open=status.should_expand(), 
                                          tags=(status.get_color()))
                 self.__add_verdicts_to_treeview(l1doctests, row_id)
      
-    def expand_rows(self): 
+    def unfold_rows(self, event): 
         """Spreads only the node rows"""
         self.__apply_row_change(True)
     
-    def fold_rows(self):
+    def fold_rows(self, event):
         """Folds only the node rows"""
         self.__apply_row_change(False)
     
     def __apply_row_change(self, to_expand:bool):
         """Depending on the `to_fold` it folds or spreads the rows that
         correspond to the ast nodes.
          
@@ -371,46 +374,48 @@
             self.treeview.update()
     
     def decrease_row_height(self, event):
         if not self.is_empty():
             current_height = self.get_rowheight()
             max_lines = self.__get_longest_wrapped_line()
             opt = self.__compute_optimal_height(max_lines, SMALL_MARGIN)
-            print("opt=", opt)
-            print("current_height=", current_height)
             if current_height > opt:
                 self.style.configure("Treeview", rowheight=current_height-1) 
                 self.treeview.update()
         
     def get_rowheight(self):
         return self.style.lookup("Treeview", 'rowheight')
     # -------------------------------------------
     # Fin des fonction pour le Header du treeview
     # ------------------------------------------
     
-    def __observe_font_changing(self, event=None, rowheight=ROW_HEIGHT):
+    def __observe_font_changing(self, event=None):
         """
             Changes the font of the treeview.
         """
         self.__update_tree_font(get_font_family_option(), 
                                 get_font_size_option(), 
-                                rowheight=rowheight)
-        self.header_bar.config(font=(get_font_family_option(), 
-                                     get_font_size_option()))
-        return "break"
+                                rowheight=self.get_optimal_row_height())
+        self.change_header_font()
+        self.update_tree_contents(self._copy_l1doctests, clear_header=False, update_header=False)
+    
+    def change_header_font(self, header_font_size=11):
+        self.header_bar.config(font=(get_font_family_option(), header_font_size))
+        self.resize_header_bar()
     
     def __update_tree_font(self, font_family, font_size, rowheight=ROW_HEIGHT):
         """
             Applies the new font to the treeview.
         """
         self.style.configure("Treeview", 
                              justify="left", 
                              rowheight=rowheight, 
                              font=(font_family, font_size), 
                              wrap=tk.WORD)  
+        
     
     def __wrap_tree_content(self, tree: ttk.Treeview, event):
         """
             This function wraps the text of treeview to follow its width.
         """
         widget = event.widget if event else tree
         
@@ -424,38 +429,39 @@
                     
                     childs = get_all_tree_childrens(self.treeview)
                     for iid in childs:
                         text = widget.item(iid)["text"]
                         wrapped = wrap(text, chars_per_100_pixels)   
                         tree.item(iid, text=wrapped)
                     self.reduce_row_spaces(childs, NORMAL_MARGIN) 
-        
+        return "break"
+    
     def reduce_row_spaces(self, childs, margin=NORMAL_MARGIN):
-        all_texts = self.__extract_wrapped_texts(childs)
-        max_lines = self.__get_longest_wrapped_line(all_texts)
-        opt_height = self.__compute_optimal_height(max_lines, margin)
-        self.style.configure("Treeview", rowheight=opt_height)
+        height = self.get_optimal_row_height(childs, margin)
+        self.style.configure("Treeview", rowheight=height)
         self.treeview.update()                
     
     def __extract_wrapped_texts(self, childs:list):
         """
             Returns a list containing all the wrapped texts of all nodes of the treeview.
         """
         return [self.treeview.item(iid)["text"] for iid in childs]
     
-    def get_optimal_row_height(self, childs:list):
+    def get_optimal_row_height(self, childs:list=None, margin=NORMAL_MARGIN):
         """
             Returns the new optimal height.
         """
+        if not childs:
+            childs = get_all_tree_childrens(self.treeview)
         all_texts = self.__extract_wrapped_texts(childs)
         
         # Quand le contenu est wrappé, on ajuste la hauteur des lignes, 
         # pour s'assurer que tout le contenu d'une ligne est affichée
         max_lines = self.__get_longest_wrapped_line(all_texts)
-        return self.__compute_optimal_height(max_lines)        
+        return self.__compute_optimal_height(max_lines, margin)        
         
     def __get_longest_wrapped_line(self, all_texts:list[str]=None):
         """
             Returns the size of the longest wrapped text in the treeview.
         """ 
         if not all_texts:
             childs = get_all_tree_childrens(self.treeview)
@@ -476,35 +482,37 @@
             Return:
                 (int): The new height.
         """
         row_height = get_font_size_option() * 2     # multiply by 2 to handle the line spacing
         opt_height = max_lines * (row_height * margin) if max_lines else row_height
         return round(opt_height)
     
-    def update_tree_contents(self, l1doctests:List[L1DocTest], parent="", full_clear=True):
+    def update_tree_contents(self, l1doctests:List[L1DocTest], parent="", clear_header=True, update_header=True):
         """
             This function contructs and inserts the rows into the treeview.
         """
         def __update_tree_header__():            
             # We build the summarize object 
             summarize: Summarize = self.build_summarize_object(self._origin_l1doctests)
             # We insert the summarize infos into the header bar of the treeview
             self.insert_summarize_in_header_bar(summarize, self.header_bar)
-            self.resize_header_bar()
+            self.change_header_font() 
         
-        self._restore_row_selection_effect()  
-        self.clear_tree(clear_all=full_clear)
+        self._restore_row_selection_effect() 
+        clear_header = True if update_header and not clear_header else clear_header 
+        self.clear_tree(clear_all=clear_header)
    
         if not self.__check_if_editor_is_open():
             return
 
         self.__add_verdicts_to_treeview(l1doctests, parent)
         
         if self.treeview.get_children():
-            __update_tree_header__()
+            if update_header:
+                __update_tree_header__()
     
     def __add_verdicts_to_treeview(self, l1doctests:List[L1DocTest], parent=""):
         o_names = [c_l1doctest.get_name() for c_l1doctest in self._origin_l1doctests]
         for l1doctest in l1doctests:
             o_index = o_names.index(l1doctest.get_name())
             current_node = self._add_node_to_tree(self._origin_l1doctests[o_index], parent)
             if l1doctest.get_flag() == L1DocTestFlag.EMPTY_FLAG:
```

### Comparing `UpyTest-3.1.6/thonnycontrib/l1test_frontend/outlines.py` & `UpyTest-3.1.7/thonnycontrib/l1test_frontend/outlines.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/plugin_loader.py` & `UpyTest-3.1.7/thonnycontrib/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/properties.py` & `UpyTest-3.1.7/thonnycontrib/properties.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/test_doc_generator.py` & `UpyTest-3.1.7/thonnycontrib/tests/test_doc_generator.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_example_no_expected.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_example_no_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_example_with_exception.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_example_with_exception.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_example_with_expected.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_example_with_expected.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_l1TestRunner.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_l1TestRunner.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_test_finder.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_test_finder.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/tests/tests_view.py` & `UpyTest-3.1.7/thonnycontrib/tests/tests_view.py`

 * *Files identical despite different names*

### Comparing `UpyTest-3.1.6/thonnycontrib/utils.py` & `UpyTest-3.1.7/thonnycontrib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from thonny import rst_utils, get_workbench
 from setuptools import find_packages
 from thonnycontrib.exceptions import CannotImportModuleException, CannotSelectSeveralLines, CompilationError
 from .properties import BACKEND_COMMAND 
 from .environement_vars import *
 import os, re, ast, traceback, textwrap, tkinter as tk
 import thonny
-    
+import platform
+
 def wrap(string:str, length=8, break_long_words=False):   
     """Wrap a text using the `wraptext` module.
 
     Args:
         string (str): the string to wrap.
         length (int, optional): the min length from which the string will be wrapped. Defaults to 8.
         break_long_words (bool, optional): if False the entire words will not be wrapped
@@ -126,27 +127,27 @@
     if extracted:
         if os.path.exists(extracted["filename"]):
             filename, lineno, comp = extracted["filename"], extracted["lineno"], extracted["complement"]
             url = "thonny-editor://" + escape(filename).replace(" ", "%20")
             if lineno is not None:
                 url += "#" + str(lineno)
             # return the hyperlink format following the rst specification
-            return "`File \"%s\", line %s%s <%s>`__\n" % (filename, lineno, comp, url)
+            return "`File \"%s\", line %s%s <%s>`__\n" % (escape(filename), lineno, comp, url)
         else: 
             return ""
     else:
         return ""
 
 def escape(s:str):
     return (
         s.replace("\\", "\\\\")
-        .replace("*", "\\*")
-        .replace("`", "\\`")
-        .replace("_", "\\_")
-        .replace("..", "\\..")
+         .replace("*", "\\*")
+         .replace("`", "\\`")
+         .replace("_", "\\_")
+         .replace("..", "\\..")
     )
 
 def get_last_exception(exc_info:tuple):
     """
     Formats exception information provided by ~exc_info~.
     Extracts the last exception located in the last frame.
```

