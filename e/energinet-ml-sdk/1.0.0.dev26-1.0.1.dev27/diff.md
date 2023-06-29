# Comparing `tmp/energinet-ml-sdk-1.0.0.dev26.tar.gz` & `tmp/energinet-ml-sdk-1.0.1.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energinet-ml-sdk-1.0.0.dev26.tar", last modified: Tue Jun 13 13:59:34 2023, max compression
+gzip compressed data, was "energinet-ml-sdk-1.0.1.dev27.tar", last modified: Thu Jun 29 12:41:36 2023, max compression
```

## Comparing `energinet-ml-sdk-1.0.0.dev26.tar` & `energinet-ml-sdk-1.0.1.dev27.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/
--rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-06-13 13:59:25.465278 energinet-ml-sdk-1.0.0.dev26/README
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/
--rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/__main__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/
--rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13203 2023-06-13 13:59:25.469278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/datasets.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/interactive.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7370 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/azure/training.py
--rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/backend.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2965 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/init.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/release.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/submit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5415 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/train.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.909187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/init.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/projects.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/verify.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/core/
--rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/backend.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/configurable.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/files.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4609 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/logger.py
--rw-r--r--   0 vsts      (1001) docker     (123)    27442 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/requirements.py
--rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/submitting.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/templates.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/core/training.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/
--rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/COMMAND_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PACKAGE_NAME
--rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-06-13 13:59:34.401189 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PACKAGE_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/meta/PYTHON_VERSION
--rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/settings.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/static/
--rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/Dockerfile
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4481 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/constants.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/deployment_smoke_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/datasets_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/training_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3739 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/init_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/release_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/submit_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/train_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/init_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/decorators_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/projects_test.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:34.913187 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/backend_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/configurable_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/files_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/logger_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-06-13 13:59:25.473278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/model_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/project_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/requirements_test.py
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-06-13 13:59:25.477278 energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/submitting_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/
+-rw-r--r--   0 vsts      (1001) docker     (123)      592 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     1733 2023-06-29 12:41:27.663968 energinet-ml-sdk-1.0.1.dev27/README
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/
+-rw-r--r--   0 vsts      (1001) docker     (123)      500 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/__main__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/
+-rw-r--r--   0 vsts      (1001) docker     (123)      210 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13203 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8140 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/datasets.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4352 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/interactive.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2130 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1245 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7370 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/azure/training.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      190 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/backend.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)      741 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      581 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2965 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/init.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3133 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/release.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5525 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/submit.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5415 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/train.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)      281 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2748 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/project/init.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)      393 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7294 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11202 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/projects.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2062 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/verify.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)       33 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4552 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/backend.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4381 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/configurable.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3006 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/files.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4609 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/logger.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    27364 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2555 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1871 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/requirements.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      595 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/submitting.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9048 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/templates.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3293 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/core/training.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/meta/
+-rw-r--r--   0 vsts      (1001) docker     (123)       12 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/meta/COMMAND_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       17 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/meta/PACKAGE_NAME
+-rw-r--r--   0 vsts      (1001) docker     (123)       11 2023-06-29 12:41:36.159871 energinet-ml-sdk-1.0.1.dev27/energinetml/meta/PACKAGE_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)        4 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/meta/PYTHON_VERSION
+-rw-r--r--   0 vsts      (1001) docker     (123)     2793 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/settings.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/static/
+-rw-r--r--   0 vsts      (1001) docker     (123)      492 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/static/Dockerfile
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/energinetml/static/model_template/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/static/model_template/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      147 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/static/model_template/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1728 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/energinetml/static/model_template/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4481 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5155 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      715 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/constants.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/ml_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/ml_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/ml_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/webapp_deployment/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/webapp_deployment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      515 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/smoketest/webapp_deployment/deployment_smoke_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8099 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4350 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/datasets_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      675 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/training_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      899 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2607 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/init_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       69 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/release_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9074 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/submit_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3566 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/train_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/project/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.671968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/project/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2310 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/project/init_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4922 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/decorators_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7759 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/projects_test.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:36.531868 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2197 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/backend_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1126 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/configurable_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1069 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/files_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2078 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/logger_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14679 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/model_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2874 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/project_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2378 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/requirements_test.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-06-29 12:41:27.675968 energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/submitting_test.py
```

### Comparing `energinet-ml-sdk-1.0.0.dev26/PKG-INFO` & `energinet-ml-sdk-1.0.1.dev27/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energinet-ml-sdk
-Version: 1.0.0.dev26
+Version: 1.0.1.dev27
 Summary: Energinet Machine Learning
 Home-page: UNKNOWN
 Author: Koncern Digitalisering Advanced Analytics Team
 Author-email: mny@energinet.dk, xjakk@energinet.dk
 License: Apache Software License 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `energinet-ml-sdk-1.0.0.dev26/README` & `energinet-ml-sdk-1.0.1.dev27/README`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/backend.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/backend.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/datasets.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/datasets.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/interactive.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/interactive.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/logger.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/submitting.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/azure/training.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/azure/training.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/__init__.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/__init__.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/__init__.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/init.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/init.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/release.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/release.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/submit.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/submit.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/model/train.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/model/train.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/project/init.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/project/init.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/decorators.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/projects.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/projects.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/cli/utils/verify.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/cli/utils/verify.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/backend.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/backend.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/configurable.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/configurable.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/files.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/files.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/logger.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/logger.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/model.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -602,15 +602,15 @@
 
         Example:
             The method can be used as a ContextManager:
 
             >>> with ModelArtifact.from_cloud(experiment_name, run_id)
             ... as model_artifact:
             >>>     # The downloaded files are downloaded to a temporary folder
-            ...     # and they are accesible from the model_artifact-instance
+            ...     # and they are accessible from the model_artifact-instance
             >>>     print(model_artifact.portal_url)
 
         It can also be used as an object, but then you have to clean up in the
         temporary folder afterwards:
 
             >>> model_artifact = ModelArtifact.from_cloud(experiment_name, run_id)
             >>> model_artifact.clean_up() # Clean up in the temporary directory
@@ -659,14 +659,27 @@
         )
 
         if tempdir:
             artifact._tempdir = tempdir
 
         return artifact
 
+    @classmethod
+    def from_path(cls, path) -> "ModelArtifact":
+        with open(f"{path}/outputs/meta.json") as fp:
+            project_meta = json.load(fp)
+
+        ma = cls(
+            path=path,
+            run_id=project_meta["run_id"],
+            experiment_name="",  # This is not used and we do not have it here
+            project_meta=project_meta,
+        )
+        return ma
+
     def clean_up(self):
         """Clean up in temporary directory when using
         :func:`~energinetml.ModelArtifact.from_cloud`
         as a standard function (ie. not a context manager).
 
         Example:
             >>> model_artifact = ModelArtifact.from_cloud(experiment_name, run_id)
@@ -882,25 +895,7 @@
 
     if not inspect.isclass(model_class):
         raise ModelNotClassError()
     if not issubclass(model_class, Model):
         raise ModelNotInheritModel()
 
     return model_class
-
-
-def df_to_pydantic_json(df: pd.DataFrame) -> Dict[str, List[Any]]:
-    """Convert a pd.DataFrame object to a dictionary in expected format.
-
-    Args:
-        df (pd.DataFrame): _description_
-
-    Returns:
-        Dict[str, List[Any]]: _description_
-    """
-    json_dict = df.to_dict(orient="records")
-    features_list = []
-    for record in json_dict:
-        features_list.append({"features": record})
-
-    json_data = {"inputs": features_list}
-    return json_data
```

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/project.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/project.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/requirements.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/requirements.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/submitting.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/submitting.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/templates.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/templates.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/core/training.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/core/training.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/settings.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/settings.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/energinetml/static/model_template/model.py` & `energinet-ml-sdk-1.0.1.dev27/energinetml/static/model_template/model.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/setup.py` & `energinet-ml-sdk-1.0.1.dev27/setup.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/conftest.py` & `energinet-ml-sdk-1.0.1.dev27/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/constants.py` & `energinet-ml-sdk-1.0.1.dev27/tests/constants.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/smoketest/ml_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/smoketest/ml_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/smoketest/webapp_deployment/deployment_smoke_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/smoketest/webapp_deployment/deployment_smoke_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/backend_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/datasets_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/datasets_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/azure_/training_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/azure_/training_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/files_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/init_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/init_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -62,17 +62,16 @@
         )
 
         # Assert
         assert result.exit_code == 1
 
 
 @patch("energinetml.cli.model.init.click.confirm")
-@patch("energinetml.cli.model.init.create_cluster")
-def test__init_model__no_name_provided__should_prompt_for_name_and_create_model_and_new_cluster(  # noqa: E501
-    create_cluster_mock, confirm_mock
+def test__init_model__no_name_provided__should_prompt_for_name_and_create_model(  # noqa: E501
+    confirm_mock
 ):
     """
     :param Mock create_cluster_mock:
     :param Mock confirm_mock:
     """
     confirm_mock.return_value = True
 
@@ -92,44 +91,7 @@
         # Act
         result = runner.invoke(
             cli=init_model, args=["--path", path], input="MODEL-NAME\nnew\n"
         )
 
         # Assert
         assert result.exit_code == 0
-
-        create_cluster_mock.assert_called_once()
-
-
-@patch("energinetml.cli.model.init.click.confirm")
-@patch("energinetml.cli.model.init.change_cluster")
-def test__init_model__no_name_provided__should_prompt_for_name_and_create_model_and_change_cluster(  # noqa: E501
-    change_cluster_mock, confirm_mock
-):
-    """
-    :param Mock change_cluster_mock:
-    :param Mock confirm_mock:
-    """
-    confirm_mock.return_value = True
-
-    runner = CliRunner()
-
-    with tempfile.TemporaryDirectory() as path:
-        MachineLearningProject.create(
-            path=path,
-            name=PROJECT_NAME,
-            subscription_id=SUBSCRIPTION_ID,
-            resource_group=RESOURCE_GROUP,
-            workspace_name=WORKSPACE_NAME,
-            vnet_name=VNET,
-            subnet_name=SUBNET,
-        )
-
-        # Act
-        result = runner.invoke(
-            cli=init_model, args=["--path", path], input="MODEL-NAME\nexisting\n"
-        )
-
-        # Assert
-        assert result.exit_code == 0
-
-        change_cluster_mock.assert_called_once()
```

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/submit_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/submit_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/model/train_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/model/train_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/project/init_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/project/init_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/decorators_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/decorators_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/cli/utils/projects_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/cli/utils/projects_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/backend_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/backend_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/configurable_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/configurable_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/files_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/files_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/logger_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/logger_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/model_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/model_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/project_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/project_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/requirements_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/requirements_test.py`

 * *Files identical despite different names*

### Comparing `energinet-ml-sdk-1.0.0.dev26/tests/unittests/core/submitting_test.py` & `energinet-ml-sdk-1.0.1.dev27/tests/unittests/core/submitting_test.py`

 * *Files identical despite different names*

