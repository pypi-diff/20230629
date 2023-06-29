# Comparing `tmp/octoploy-1.2.2.tar.gz` & `tmp/octoploy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoploy-1.2.2.tar", last modified: Tue Jun 13 08:03:30 2023, max compression
+gzip compressed data, was "octoploy-1.2.3.tar", last modified: Thu Jun 29 10:15:08 2023, max compression
```

## Comparing `octoploy-1.2.2.tar` & `octoploy-1.2.3.tar`

### file list

```diff
@@ -1,81 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:03:17.000000 octoploy-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-13 08:03:30.419119 octoploy-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-13 08:03:17.000000 octoploy-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/Model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/Oc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/backup/BackupGenerator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/backup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/AppConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/BaseConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/DeploymentActionConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/DynamicConfigMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/YmlConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/AppDeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/DeploymentBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/K8sObjectDeployer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/BaseObj.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/SecretObj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/octoploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DataDiff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DataPreProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/DecryptionProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/K8sObjectMerge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/NamespaceProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/TreeWalker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/ValueLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/YmlTemplateProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.415118 octoploy-1.2.2/octoploy/state/
--rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/state/StateTracking.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/octoploy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Cert.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/DictUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Log.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/Yml.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/YmlWriter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/octoploy/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.411118 octoploy-1.2.2/octoploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 08:03:30.000000 octoploy-1.2.2/octoploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 08:03:30.419119 octoploy-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-13 08:03:17.000000 octoploy-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/AppDeploymentTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/DictUtilsTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/OcObjectMergeTest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/StateTrackingTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/TestUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/YmlTempalteProcessorTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/config/AppConfigTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/processing/ValueLoaderTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:30.419119 octoploy-1.2.2/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/EncryptionTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/YmlWriterTest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:03:17.000000 octoploy-1.2.2/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.711344 octoploy-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-29 10:14:54.000000 octoploy-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-29 10:15:08.711344 octoploy-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10011 2023-06-29 10:14:54.000000 octoploy-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.703343 octoploy-1.2.3/octoploy/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.703343 octoploy-1.2.3/octoploy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/api/Model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/api/Oc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.703343 octoploy-1.2.3/octoploy/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/backup/BackupGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/backup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/AppConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/BaseConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/DeploymentActionConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/DynamicConfigMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/YmlConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/deploy/AppDeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/deploy/DeploymentBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/deploy/K8sObjectDeployer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/k8s/BaseObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/k8s/SecretObj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9081 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/octoploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/DataDiff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/DataPreProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/DecryptionProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/K8sObjectMerge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/NamespaceProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/TreeWalker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/ValueLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7386 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/YmlTemplateProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/state/
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/state/StateMover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/state/StateTracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.707344 octoploy-1.2.3/octoploy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/DictUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/Yml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/YmlWriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/octoploy/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.703343 octoploy-1.2.3/octoploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-29 10:15:08.000000 octoploy-1.2.3/octoploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 10:15:08.711344 octoploy-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-29 10:14:54.000000 octoploy-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.711344 octoploy-1.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/AppDeploymentTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/DictUtilsTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/OcObjectMergeTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/StateTrackingTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/TestUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/YmlTempalteProcessorTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.711344 octoploy-1.2.3/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/config/AppConfigTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.711344 octoploy-1.2.3/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/processing/ValueLoaderTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:15:08.711344 octoploy-1.2.3/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/utils/EncryptionTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/utils/YmlWriterTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:14:54.000000 octoploy-1.2.3/tests/utils/__init__.py
```

### Comparing `octoploy-1.2.2/LICENSE` & `octoploy-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/PKG-INFO` & `octoploy-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.2/README.md` & `octoploy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/api/Model.py` & `octoploy-1.2.3/octoploy/api/Model.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/api/Oc.py` & `octoploy-1.2.3/octoploy/api/Oc.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/backup/BackupGenerator.py` & `octoploy-1.2.3/octoploy/backup/BackupGenerator.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/config/AppConfig.py` & `octoploy-1.2.3/octoploy/config/AppConfig.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import List, Optional, Dict
 
 from octoploy.config.BaseConfig import BaseConfig
-from octoploy.config.DynamicConfigMap import DynamicConfigMap
 from octoploy.config.DeploymentActionConfig import DeploymentActionConfig
+from octoploy.config.DynamicConfigMap import DynamicConfigMap
 from octoploy.utils.DictUtils import DictUtils
 from octoploy.utils.Errors import MissingVar
 
 
 class AppConfig(BaseConfig):
     """
     Contains the configuration for the deployment of a single app
```

### Comparing `octoploy-1.2.2/octoploy/config/BaseConfig.py` & `octoploy-1.2.3/octoploy/config/BaseConfig.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
 from typing import Dict, List, Optional
 
 from octoploy.config.YmlConfig import YmlConfig
-from octoploy.processing.DecryptionProcessor import DecryptionProcessor
-from octoploy.processing.TreeWalker import TreeProcessor
 from octoploy.processing.ValueLoader import ValueLoaderFactory
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 
 
 class BaseConfig(YmlConfig):
     def __init__(self, path: Optional[str], external_vars: Dict[str, str] = None):
         super().__init__(path)
@@ -45,15 +43,15 @@
             return self._replacements
 
         items = self.data.get('vars', {})
         new_items = {}
         for key, value in items.items():
             # Value can be a primitive or object
             if isinstance(value, dict):
-                # Is a object, use a loader to load the value
+                # Is an object, use a loader to load the value
                 loader_name = value.get('loader')
                 if loader_name is not None:
                     loader = ValueLoaderFactory.create(self, value['loader'])
                     new_values = loader.load(value)
                     new_items[key] = 'viaLoader'
                     for new_key, new_val in new_values.items():
                         new_items[key + new_key] = new_val
```

### Comparing `octoploy-1.2.2/octoploy/config/Config.py` & `octoploy-1.2.3/octoploy/config/Config.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import os
 from typing import Optional, Dict, List
 
 from octoploy.api.Oc import Oc, K8, K8sApi
 from octoploy.config.AppConfig import AppConfig
 from octoploy.config.BaseConfig import BaseConfig
+from octoploy.processing import Constants
 from octoploy.processing.DataPreProcessor import DataPreProcessor, OcToK8PreProcessor
 from octoploy.processing.DecryptionProcessor import DecryptionProcessor
 from octoploy.processing.NamespaceProcessor import NamespaceProcessor
 from octoploy.processing.TreeWalker import TreeProcessor
 from octoploy.processing.YmlTemplateProcessor import YmlTemplateProcessor
 from octoploy.state.StateTracking import StateTracking
 from octoploy.utils.Errors import ConfigError
@@ -28,25 +29,45 @@
         """
 
         self.plan = False
         """
         True if changes should be previewed
         """
 
+        self.var_override: Dict[str, str] = {}
+        """
+        Key/value pairs which should be passed to the templating engine.
+        These value have priority over already defined values
+        """
+
+    def set_override_env(self, env: List[str]):
+        """
+        Parses a key=value list
+        :param env: key=value strings
+        """
+        for entry in env:
+            parts = entry.split('=', 1)
+            if len(parts) < 2:
+                raise ValueError(f'Could not parse {entry}')
+            key = parts[0]
+            value = parts[1]
+            self.var_override[key] = value
+
 
 class RootConfig(BaseConfig):
     """
     Root configuration for a project (aka a collection of apps inside a single context/namespace)
     """
 
     def __init__(self, config_root: str, path: str):
         super().__init__(path)
         self._config_root = config_root
         self._oc = None
         self._library = None  # type: Optional[RootConfig]
+        self._global_var_overrides: Dict[str, str] = {}
 
         inherit = self.data.get('inherit')
         if inherit is not None:
             # Use a library
             parent_dir = os.path.abspath(os.path.join(path, os.pardir, os.pardir))
             lib_dir = os.path.join(parent_dir, inherit)
             if not os.path.isdir(lib_dir):
@@ -54,22 +75,26 @@
             self._library = RootConfig.load(lib_dir)
             if not self._library.is_library():
                 raise ConfigError('Project ' + inherit + ' referenced as library but is not a library')
 
         state_name = self.data.get('stateName', '')
         self._state = StateTracking(self.create_api(), state_name)
 
+    def get_var_overrides(self) -> Dict[str, str]:
+        return self._global_var_overrides
+
     @classmethod
     def load(cls, path: str) -> RootConfig:
         return RootConfig(path, os.path.join(path, '_root.yml'))
 
     def get_state(self) -> StateTracking:
         return self._state
 
     def initialize_state(self, run_mode: RunMode):
+        self._global_var_overrides = run_mode.var_override
         if run_mode.dry_run:
             return
         self._state.restore(self.get_namespace_name())
 
     def persist_state(self, run_mode: RunMode):
         if run_mode.dry_run or run_mode.plan:
             return
@@ -85,15 +110,15 @@
         return self.data.get('type', '') == 'library'
 
     def _get_mode(self) -> str:
         return self.data.get('mode', 'k8s')
 
     def create_api(self) -> K8sApi:
         """
-        Creates a new openshift / k8s client
+        Creates a new openshift / k8s client.
         :return: Client
         """
         if self._oc is not None:
             return self._oc
 
         mode = self._get_mode()
         if mode == 'oc':
@@ -107,26 +132,30 @@
 
     def get_namespace_name(self) -> Optional[str]:
         """
         Returns the namespace name of this project
 
         :return: Name or null for libraries or if the namespace should not be changed
         """
-        return self.data.get('namespace', self.data.get('project'))
+        namespace = self.data.get('namespace', self.data.get('project'))
+        if namespace is None:
+            # Maybe passed via commandline?
+            return self._global_var_overrides.get(Constants.VAR_NAMESPACE)
+        return namespace
 
     def get_kubectl_context(self) -> Optional[str]:
         """
-        Returns the configuration context name
+        Returns the configuration context name.
         :return: Name or null if the current context should be used
         """
         return self.data.get('context')
 
     def get_pre_processor(self) -> DataPreProcessor:
         """
-        Returns the pre processor for the current config
+        Returns the pre-processor for the current config
         """
         mode = self._get_mode()
         if mode == 'k8s' or mode == 'k8s':
             return OcToK8PreProcessor()
         return DataPreProcessor()
 
     def get_template_processor(self) -> YmlTemplateProcessor:
@@ -142,16 +171,18 @@
         :return: Key, value map
         """
         items = super().get_replacements()
         name = self.get_namespace_name()
         if name is not None:
             items.update({
                 'OC_PROJECT': name,
-                'NAMESPACE': name
+                Constants.VAR_NAMESPACE: name
             })
+
+        items.update(self._global_var_overrides)
         return items
 
     def get_yml_processors(self) -> List[TreeProcessor]:
         """
         Returns all yml processors which should be applied
         :return: Processors
         """
```

### Comparing `octoploy-1.2.2/octoploy/config/DeploymentActionConfig.py` & `octoploy-1.2.3/octoploy/config/DeploymentActionConfig.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/config/DynamicConfigMap.py` & `octoploy-1.2.3/octoploy/config/DynamicConfigMap.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/deploy/AppDeploy.py` & `octoploy-1.2.3/octoploy/deploy/AppDeploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
                     processor.process(k8s_object)
                 except SkipObject as e:
                     self.log.warning(f'Skipping object: {e}')
                     skipped_objects.append(k8s_object)
 
         for k8s_object in skipped_objects:
             # Mark in state as "visited" so the object doesn't get deleted on k8s side
-            self._root_config.get_state().visit(self._app_config.get_name(), k8s_object, k8s_object.get_hash())
+            self._root_config.get_state().visit(self._app_config.get_name(), k8s_object, k8s_object.get_hash(),
+                                                only_update=True)
             self._bundle.objects.remove(k8s_object)
 
         api = self._root_config.create_api()
         if self._mode.out_file is not None:
             self._bundle.dump_objects(self._mode.out_file)
 
         if self._mode.dry_run:
```

### Comparing `octoploy-1.2.2/octoploy/deploy/DeploymentBundle.py` & `octoploy-1.2.3/octoploy/deploy/DeploymentBundle.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,17 +62,17 @@
         def sorting(x: BaseObj):
             if x.is_kind('DeploymentConfig') or x.is_kind('Deployment'):
                 return 1
             return 0
 
         self.objects.sort(key=sorting)
         for item in self.objects:
-            deploy_runner.deploy_object(item)
+            deploy_runner.add_object(item)
 
-        deploy_runner.delete_abandoned_objects()
+        deploy_runner.execute()
 
     def dump_objects(self, path: str):
         """
         Very crude method for dumping the objects to a yml file.
         If the file does already exist the content will be appended
         :param path: Path to a file
         """
```

### Comparing `octoploy-1.2.2/octoploy/deploy/K8sObjectDeployer.py` & `octoploy-1.2.3/octoploy/deploy/K8sObjectDeployer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from octoploy.api.Oc import K8sApi
 from octoploy.config.Config import RootConfig, AppConfig, RunMode
 from octoploy.k8s.BaseObj import BaseObj
 from octoploy.state.StateTracking import StateTracking
 from octoploy.utils.Log import Log
 
 
@@ -23,23 +25,47 @@
         super().__init__()
         self._root_config = root_config
         self._app_config = app_config
         self._api = k8sapi
         self._mode = mode
         self._state = root_config.get_state()
 
+        self._to_be_deployed: List[BaseObj] = []
+
     def select_context(self):
         """
         Selects the cluster context
         """
         context = self._root_config.get_kubectl_context()
         if context is not None:
             self._api.switch_context(context)
 
-    def deploy_object(self, k8s_object: BaseObj):
+    def add_object(self, k8s_object: BaseObj):
+        """
+        Adds the given object to the deployment list
+        :param k8s_object: Object which should be deployed
+        """
+        self._to_be_deployed.append(k8s_object)
+        self._state.visit_only(self._app_config.get_name(), k8s_object)
+
+    def execute(self):
+        """
+        Executes the deployment
+        """
+        self._delete_abandoned_objects()
+        self._deploy_objects()
+
+    def _deploy_objects(self):
+        """
+        Deploys the pending objects
+        """
+        for k8s_object in self._to_be_deployed:
+            self._deploy_object(k8s_object)
+
+    def _deploy_object(self, k8s_object: BaseObj):
         """
         Deploy the given object (if a deployment required, otherwise does nothing)
         :param k8s_object: Object which should be deployed
         """
         hash_val = k8s_object.get_hash()
         item_path = k8s_object.get_fqn()
         namespace = k8s_object.namespace
@@ -56,40 +82,41 @@
             if obj_state is not None and obj_state.hash != '':
                 state_hash = obj_state.hash
             else:  # Fallback to old hash location
                 state_hash = old_state_hash
 
         if current_object is not None and state_hash is None:
             # Item has not been deployed with octoploy, but it does already exist
-            self.log.warning(f'{item_path} has no state annotation, assuming no change required')
+            self.log.warning(f'{item_path} has no state, assuming no change required')
             self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             return
 
         if state_hash == hash_val:
-            self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             self.log.debug(f"{item_path} hasn't changed")
             return
 
         if current_object is not None:
             self._log_update(item_path)
 
         if self._mode.plan:
-            self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
             return
 
         if old_state_hash is not None:
             # Migrate to new state format by removing the old one
             self._api.annotate(k8s_object.get_fqn(), self.HASH_ANNOTATION, None, namespace=k8s_object.namespace)
+
         self._api.apply(k8s_object.as_string(), namespace=namespace)
+
+        # Update hash
         self._state.visit(self._app_config.get_name(), k8s_object, hash_val)
 
         if k8s_object.is_kind('ConfigMap'):
             self._reload_config()
 
-    def delete_abandoned_objects(self):
+    def _delete_abandoned_objects(self):
         """
         Deletes all objects which are not anymore included in the
         current app config
         """
         abandoned = self._state.get_not_visited(self._app_config.get_name())
         for item in abandoned:
             namespace = item.namespace
```

### Comparing `octoploy-1.2.2/octoploy/k8s/BaseObj.py` & `octoploy-1.2.3/octoploy/k8s/BaseObj.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/octoploy.py` & `octoploy-1.2.3/octoploy/octoploy.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import argparse
 
 from octoploy.backup.BackupGenerator import BackupGenerator
 from octoploy.config.Config import RootConfig, RunMode
 from octoploy.deploy.AppDeploy import AppDeployment
 from octoploy.processing.DecryptionProcessor import DecryptionProcessor
+from octoploy.state.StateMover import StateMover
 from octoploy.utils.Encryption import YmlEncrypter
 from octoploy.utils.Log import Log
 
 log_instance = Log('octoploy')
 
 
 def load_project(config_dir: str) -> RootConfig:
@@ -42,85 +43,94 @@
     for action in reload_actions:
         action.run(oc)
     log_instance.log.info('Done')
 
 
 def _run_app_deploy(config_dir: str, app_name: str, mode: RunMode):
     root_config = load_project(config_dir)
-    app_config = root_config.load_app_config(app_name)
     root_config.initialize_state(mode)
+    app_config = root_config.load_app_config(app_name)
     try:
         deployment = AppDeployment(root_config, app_config, mode)
         deployment.deploy()
     finally:
         root_config.persist_state(mode)
     log_instance.log.info('Done')
 
 
 def _run_apps_deploy(config_dir: str, mode: RunMode):
     root_config = load_project(config_dir)
-    configs = root_config.load_app_configs()
     root_config.initialize_state(mode)
+    configs = root_config.load_app_configs()
     log_instance.log.debug(f'Found {len(configs)} apps to deploy')
     try:
         for app_config in configs:
             AppDeployment(root_config, app_config, mode).deploy()
     finally:
         root_config.persist_state(mode)
     log_instance.log.info('Done')
 
 
 def plan_app(args):
     mode = RunMode()
     mode.plan = True
+    mode.set_override_env(args.env)
     _run_app_deploy(args.config_dir, args.name[0], mode)
 
 
 def deploy_app(args):
     mode = RunMode()
     mode.out_file = args.out_file
     mode.dry_run = args.dry_run
+    mode.set_override_env(args.env)
     _run_app_deploy(args.config_dir, args.name[0], mode)
 
 
 def plan_all(args):
     mode = RunMode()
     mode.plan = True
+    mode.set_override_env(args.env)
     _run_apps_deploy(args.config_dir, mode)
 
 
 def deploy_all(args):
     mode = RunMode()
     mode.out_file = args.out_file
     mode.dry_run = args.dry_run
+    mode.set_override_env(args.env)
     _run_apps_deploy(args.config_dir, mode)
 
 
 def create_backup(args):
     root_config = load_project(args.config_dir)
     BackupGenerator(root_config).create_backup(args.name[0])
 
 
 def encrypt_secrets(args):
     files = args.file
     for file in files:
         YmlEncrypter(file).encrypt()
 
 
+def list_state(args):
+    root_config = load_project(args.config_dir)
+    root_config.initialize_state(RunMode())
+
+    state = root_config.get_state()
+    state.print()
+
+
 def move_state(args):
-    run_mode = RunMode()
     source = args.items[0]
     dest = args.items[1]
+    target_cm = args.to
 
     root_config = load_project(args.config_dir)
-    root_config.initialize_state(run_mode)
-
-    state = root_config.get_state()
-    state.move(source, dest)
-    root_config.persist_state(run_mode)
+    mover = StateMover(root_config)
+    mover.move(source, dest, dest_configmap=target_cm)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--version', dest='version', action='store_true',
                         help='Prints the current version')
     parser.add_argument('--debug', dest='debug', action='store_true',
@@ -128,22 +138,35 @@
     parser.add_argument('--skip-secrets', dest='skip_secrets', action='store_true',
                         help="Skips all secret objects and therefore doesn't require a key to be set")
     parser.add_argument('--deploy-plain-secrets', dest='deploy_plain_text', action='store_true',
                         help="Deploys plain text secret objects")
     parser.add_argument('-c', '--config-dir', dest='config_dir',
                         help='Path to the folder containing all configurations',
                         default='')
+    parser.add_argument('-e', '--env', dest='env', action='append',
+                        help='key=value pairs of parameters to set/override during for the templating engine',
+                        default=[])
 
     subparsers = parser.add_subparsers(help='Commands')
-    state_parser = subparsers.add_parser('move-state', help='Moves objects from the state to other places')
-    state_parser.add_argument('items', help='Source and destination.\n'
-                                            'The format for an object is: octoployName/Namespace/Kind/K8sObjectName\n'
-                                            'For example: "my-old-app/Namespace2/Deployment/app" '
-                                            '"my-new-app/Namespace2/Deployment/app"', nargs=2)
-    state_parser.set_defaults(func=move_state)
+    state_parser = subparsers.add_parser('state', help='State interactions')
+
+    state_subparsers = state_parser.add_subparsers(help='State commands')
+    state_list_parser = state_subparsers.add_parser('list')
+    state_list_parser.set_defaults(func=list_state)
+
+    state_mv_parser = state_subparsers.add_parser('mv')
+    state_mv_parser.set_defaults(func=move_state)
+
+    state_mv_parser.add_argument('items', help='Source and destination.\n'
+                                               'The format for an object is: octoployName/Namespace/k8sFqn\n'
+                                               'For example: "my-old-app/Namespace2/k8sFqn" '
+                                               '"my-new-app/Namespace2/k8sFqn"', nargs=2)
+    state_mv_parser.add_argument('--to', dest='to', help='Configmap where the state should be moved to (optional).'
+                                                         'Format: configmapSuffix|namespace/configmapSuffix')
+    state_mv_parser.set_defaults(func=move_state)
 
     encrypt_parser = subparsers.add_parser('encrypt', help='Encrypts k8s secrets objects')
     encrypt_parser.add_argument('file', help='Yml file to be encrypted', nargs=1)
     encrypt_parser.set_defaults(func=encrypt_secrets)
 
     backup_parser = subparsers.add_parser('backup', help='Creates a backup of all resources in the cluster')
     backup_parser.add_argument('name', help='Name of the backup folder', nargs=1)
```

### Comparing `octoploy-1.2.2/octoploy/processing/DataPreProcessor.py` & `octoploy-1.2.3/octoploy/processing/DataPreProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/DecryptionProcessor.py` & `octoploy-1.2.3/octoploy/processing/DecryptionProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/K8sObjectMerge.py` & `octoploy-1.2.3/octoploy/processing/K8sObjectMerge.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/NamespaceProcessor.py` & `octoploy-1.2.3/octoploy/processing/NamespaceProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/TreeWalker.py` & `octoploy-1.2.3/octoploy/processing/TreeWalker.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/ValueLoader.py` & `octoploy-1.2.3/octoploy/processing/ValueLoader.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/processing/YmlTemplateProcessor.py` & `octoploy-1.2.3/octoploy/processing/YmlTemplateProcessor.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/state/StateTracking.py` & `octoploy-1.2.3/octoploy/state/StateTracking.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,29 +107,36 @@
             'data': {
                 'state': YmlWriter.dump(states)
             }
         }
         yml = YmlWriter.dump(data)
         self._k8s_api.apply(yml, namespace=namespace)
 
-    def move(self, source: str, dest: str):
-        if source.count('/') != dest.count('/'):
-            raise ValueError('Source and destination point to different path depths')
+    def add(self, object_state: ObjectState):
+        self._state[object_state.get_key()] = object_state
 
+    def remove(self, object_state: ObjectState):
+        del self._state[object_state.get_key()]
+
+    def remove_key(self, key: str):
+        del self._state[key]
+
+    def get_items(self, prefix: str) -> List[ObjectState]:
+        """
+        Returns all state items which start with the given prefix
+        :param prefix: Prefix
+        :return: Items
+        """
+        items = []
         for value in list(self._state.values()):
             key = value.get_key()
-            if not key.startswith(source):
+            if not key.startswith(prefix):
                 continue
-            target = key.replace(source, dest)
-            self.log.info(f'Moving {key} to {target}')
-            value.update_from_key(target)
-
-            if key in self._state:
-                del self._state[key]
-            self._state[target] = value
+            items.append(value)
+        return items
 
     def get_not_visited(self, context: str) -> List[ObjectState]:
         """
         Returns all objects which have not been visited
         :param context: Context
         :return: Objects
         """
@@ -139,33 +146,47 @@
                 items.append(object_state)
         return items
 
     def get_state(self, context_name: str, k8s_object: BaseObj) -> Optional[ObjectState]:
         state = self._k8s_to_state(context_name, k8s_object)
         return self._state.get(state.get_key())
 
-    def visit(self, context_name: str, k8s_object: BaseObj, hash_val: str):
+    def visit(self, context_name: str, k8s_object: BaseObj, hash_val: str, only_update: bool = False):
         """
         Marks the given object as "visited".
         If the object is not yet in the state it will be added
         :param context_name: Name of the state context
         :param k8s_object: Kubernetes object
         :param hash_val: The new hash value of the object.
+        :param only_update: True if the state should only be updated and not added if not existing
         """
         state = self._k8s_to_state(context_name, k8s_object)
         existing_state = self._state.get(state.get_key())
         if existing_state is None:
+            if only_update:
+                return
             state.hash = hash_val
             self._state[state.get_key()] = state
             return
         existing_state.hash = hash_val
         existing_state.visited = True
 
-    def remove(self, object_state: ObjectState):
-        del self._state[object_state.get_key()]
+    def visit_only(self, context_name: str, k8s_object):
+        """
+        Marks the given object as "visited" if already in the state
+        """
+        state = self._k8s_to_state(context_name, k8s_object)
+        existing_state = self._state.get(state.get_key())
+        if existing_state is not None:
+            existing_state.visited = True
+
+    def print(self):
+        self.log.info(f'State content of ConfigMap {self._cm_name}')
+        for key, value in self._state.items():
+            self.log.info('|- ' + value.get_key())
 
     @staticmethod
     def _k8s_to_state(context_name: str, k8s_object: BaseObj) -> ObjectState:
         # At this point we always have a namespace set for the object
         state = ObjectState()
         state.context = context_name
         state.namespace = k8s_object.namespace
```

### Comparing `octoploy-1.2.2/octoploy/utils/Cert.py` & `octoploy-1.2.3/octoploy/utils/Cert.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/utils/DictUtils.py` & `octoploy-1.2.3/octoploy/utils/DictUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/utils/Encryption.py` & `octoploy-1.2.3/octoploy/utils/Encryption.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/utils/Log.py` & `octoploy-1.2.3/octoploy/utils/Log.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy/utils/YmlWriter.py` & `octoploy-1.2.3/octoploy/utils/YmlWriter.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/octoploy.egg-info/PKG-INFO` & `octoploy-1.2.3/octoploy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoploy
-Version: 1.2.2
+Version: 1.2.3
 Summary: Simple kubernetes / openshift templating engine with templating, libraries, state tracking
 Home-page: https://github.com/davidgiga1993/octoploy
 Author: davidgiga1993
 Author-email: david@dev-core.org
 License: UNKNOWN
 Description: # Kubernetes / openshift templating and deployment engine
```

### Comparing `octoploy-1.2.2/octoploy.egg-info/SOURCES.txt` & `octoploy-1.2.3/octoploy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,23 +25,25 @@
 octoploy/deploy/AppDeploy.py
 octoploy/deploy/DeploymentBundle.py
 octoploy/deploy/K8sObjectDeployer.py
 octoploy/deploy/__init__.py
 octoploy/k8s/BaseObj.py
 octoploy/k8s/SecretObj.py
 octoploy/k8s/__init__.py
+octoploy/processing/Constants.py
 octoploy/processing/DataDiff.py
 octoploy/processing/DataPreProcessor.py
 octoploy/processing/DecryptionProcessor.py
 octoploy/processing/K8sObjectMerge.py
 octoploy/processing/NamespaceProcessor.py
 octoploy/processing/TreeWalker.py
 octoploy/processing/ValueLoader.py
 octoploy/processing/YmlTemplateProcessor.py
 octoploy/processing/__init__.py
+octoploy/state/StateMover.py
 octoploy/state/StateTracking.py
 octoploy/state/__init__.py
 octoploy/utils/Cert.py
 octoploy/utils/DictUtils.py
 octoploy/utils/Encryption.py
 octoploy/utils/Errors.py
 octoploy/utils/Log.py
```

### Comparing `octoploy-1.2.2/setup.py` & `octoploy-1.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/tests/AppDeploymentTest.py` & `octoploy-1.2.3/tests/AppDeploymentTest.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from time import sleep
 from unittest import TestCase
 
 import yaml
 
 from octoploy.config.Config import RootConfig, RunMode
 from octoploy.deploy.AppDeploy import AppDeployment
 from octoploy.utils.Errors import MissingParam
@@ -23,28 +22,35 @@
     def tearDown(self) -> None:
         if os.path.isfile(self._tmp_file):
             os.remove(self._tmp_file)
 
     def test_inherit_vars(self):
         """
         Makes sure variables from the app are passed to the library
-        and overrides and conflicts with values from the app
+        and overrides conflicts with values from the app
         """
         self._deploy('app')
         with open(self._tmp_file) as f:
             data = yaml.load(f, Loader=yaml.FullLoader)
         self.assertEqual('ABC', data['metadata']['name'])
         self.assertEqual('ABC-1', data['metadata']['REMAPPED'])
         self.assertEqual('ABC', data['metadata']['REMAPPED2'])
         self.assertEqual('DEF', data['metadata']['name2'])
         self.assertEqual('3', data['metadata']['base'])
         # Global variable should be passed down and should not be
         # overwritten by apps
         self.assertEqual('global', data['metadata']['GLOBAL_TEST'])
 
+    def test_var_override(self):
+        self._mode.var_override['globalVar'] = 'ext-override'
+        self._deploy('app')
+        with open(self._tmp_file) as f:
+            data = yaml.load(f, Loader=yaml.FullLoader)
+        self.assertEqual('ext-override', data['metadata']['GLOBAL_TEST'])
+
     def test_cm_types(self):
         self._deploy('cm-types')
 
         with open(self._tmp_file) as f:
             content = f.read()
         # Make sure the "y" is quoted
         self.assertIn('"y"', content)
@@ -113,10 +119,11 @@
         with open(self._tmp_file) as f:
             data = yaml.load(f, Loader=yaml.FullLoader)
         self.assertEqual('hello world', data['stringData']['ref'])
         self.assertEqual('hello world', data['stringData']['field'])
 
     def _deploy(self, app: str, project: str = 'app_deploy_test'):
         prj_config = RootConfig.load(os.path.join(self._base_path, project))
+        prj_config.initialize_state(self._mode)
         app_config = prj_config.load_app_config(app)
         runner = AppDeployment(prj_config, app_config, self._mode)
         runner.deploy()
```

### Comparing `octoploy-1.2.2/tests/DictUtilsTest.py` & `octoploy-1.2.3/tests/DictUtilsTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/tests/OcObjectMergeTest.py` & `octoploy-1.2.3/tests/OcObjectMergeTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/tests/StateTrackingTest.py` & `octoploy-1.2.3/tests/StateTrackingTest.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import List
 from unittest import TestCase
 
 import yaml
 
 import octoploy.octoploy
 from octoploy.config.Config import RunMode, RootConfig
+from octoploy.state.StateMover import StateMover
 from octoploy.state.StateTracking import StateTracking, ObjectState
 from tests import TestUtils
 from tests.TestUtils import DummyK8sApi
 
 
 class StateTrackingTest(TestCase):
 
@@ -33,63 +34,71 @@
         prj_config.create_api = get_dummy_api
         return prj_config
 
     def _create_state_data(self):
         data = {}
         obj = ObjectState()
         obj.update_from_key('a/b/c.d/12')
-        data['a'] = obj
+        data[obj.get_key()] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
         self.assertEqual('c.d/12', obj.fqn)
 
         obj = ObjectState()
         obj.update_from_key('a/b/c')
-        data['b'] = obj
+        data[obj.get_key()] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
         self.assertEqual('c', obj.fqn)
 
         obj = ObjectState()
         obj.update_from_key('a/b/Deployment/name')
-        data['c'] = obj
+        data[obj.get_key()] = obj
         self.assertEqual('a', obj.context)
         self.assertEqual('b', obj.namespace)
         return data
 
     def test_move(self):
-        state = StateTracking(None)
+        root = self._load_project('app_deploy_test')
+        mover = StateMover(root)
+        state = StateTracking(root.create_api())
         data = state._state
+        root._state = state
+
+        def void(ignore):
+            pass
+
+        root.initialize_state = void
         data.update(self._create_state_data())
 
-        self.assertEqual('a', data['a'].context)
-        self.assertEqual('b', data['a'].namespace)
-        self.assertEqual('c.d/12', data['a'].fqn)
-
-        self.assertEqual('a', data['b'].context)
-        self.assertEqual('b', data['b'].namespace)
-        self.assertEqual('c', data['b'].fqn)
-
-        self.assertEqual('a', data['c'].context)
-        self.assertEqual('b', data['c'].namespace)
-
-        state.move('a/b/c.d/12', '1/2/3/4')
-        self.assertEqual('1', data['a'].context)
-        self.assertEqual('2', data['a'].namespace)
-        self.assertEqual('3/4', data['a'].fqn)
+        self.assertEqual('a', data['a/b/c.d/12'].context)
+        self.assertEqual('b', data['a/b/c.d/12'].namespace)
+        self.assertEqual('c.d/12', data['a/b/c.d/12'].fqn)
+
+        self.assertEqual('a', data['a/b/c'].context)
+        self.assertEqual('b', data['a/b/c'].namespace)
+        self.assertEqual('c', data['a/b/c'].fqn)
+
+        self.assertEqual('a', data['a/b/Deployment/name'].context)
+        self.assertEqual('b', data['a/b/Deployment/name'].namespace)
+
+        mover.move('a/b/c.d/12', '1/2/3/4', None)
+        self.assertEqual('1', data['1/2/3/4'].context)
+        self.assertEqual('2', data['1/2/3/4'].namespace)
+        self.assertEqual('3/4', data['1/2/3/4'].fqn)
         data = state._state = self._create_state_data()
 
-        state.move('a/b', '1/2')
-        self.assertEqual('1', data['a'].context)
-        self.assertEqual('2', data['a'].namespace)
-        self.assertEqual('c.d/12', data['a'].fqn)
-
-        self.assertEqual('1', data['b'].context)
-        self.assertEqual('2', data['b'].namespace)
-        self.assertEqual('c', data['b'].fqn)
+        mover.move('a/b', '1/2', None)
+        self.assertEqual('1', data['1/2/Deployment/name'].context)
+        self.assertEqual('2', data['1/2/Deployment/name'].namespace)
+        self.assertEqual('Deployment/name', data['1/2/Deployment/name'].fqn)
+
+        self.assertEqual('1', data['1/2/c'].context)
+        self.assertEqual('2', data['1/2/c'].namespace)
+        self.assertEqual('c', data['1/2/c'].fqn)
         data = state._state = self._create_state_data()
 
     def test_create_new(self):
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '', error=Exception('NotFound'))
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], '{}')
 
         octoploy.octoploy._run_app_deploy('app_deploy_test', 'app', self._mode)
@@ -157,18 +166,14 @@
              "hash": "1f4d778af0ea594402e656fd6139c584",
              "fqn": "ConfigMap/config",
              "namespace": "oc-project"},
             {"context": "ABC2",
              "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
              "fqn": "Secret/secret",
              "namespace": "oc-project"},
-            {"context": "ABC2",
-             "hash": "178859f1aa21598384610f352d314ae6",
-             "fqn": "Secret/plain-secret",
-             "namespace": "oc-project"},
             {"context": "var-append",
              "hash": "24d921e38f585e26cdc247d8fddc260e",
              "fqn": "ConfigMap/config",
              "namespace": "oc-project"},
         ], state_update.stdin)
 
         # Now deploy a single app
@@ -217,18 +222,14 @@
                                 "hash": "d6e8e8f4b59b77117ec4ad267be8dcae",
                                 "fqn": "Secret/secret",
                                 "namespace": "oc-project"},
                                {"context": "var-append",
                                 "hash": "24d921e38f585e26cdc247d8fddc260e",
                                 "fqn": "ConfigMap/config",
                                 "namespace": "oc-project"},
-                               {"context": "ABC2",
-                                "hash": "178859f1aa21598384610f352d314ae6",
-                                "fqn": "Secret/plain-secret",
-                                "namespace": "oc-project"},
                                ], state_update.stdin)
         # Now deploy a single app
         current_state = yaml.safe_load(state_update.stdin)
         self._dummy_api.respond(['get', 'ConfigMap/octoploy-state', '-o', 'json'], json.dumps(current_state))
         self._dummy_api.respond(['get', 'Deployment/ABC', '-o', 'json'], '{}')
         self._dummy_api.respond(['get', 'Deployment/8080', '-o', 'json'], '{}')
         self._dummy_api.respond(['get', 'Deployment/8081', '-o', 'json'], '{}')
```

### Comparing `octoploy-1.2.2/tests/TestUtils.py` & `octoploy-1.2.3/tests/TestUtils.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/tests/YmlTempalteProcessorTest.py` & `octoploy-1.2.3/tests/YmlTempalteProcessorTest.py`

 * *Files identical despite different names*

### Comparing `octoploy-1.2.2/tests/processing/ValueLoaderTest.py` & `octoploy-1.2.3/tests/processing/ValueLoaderTest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,32 @@
+import os
 from unittest import TestCase
 
 from octoploy.config.BaseConfig import BaseConfig
 from octoploy.processing.ValueLoader import ValueLoaderFactory
 
 
 class ValueLoaderTest(TestCase):
 
     def test_env(self):
         factory = ValueLoaderFactory()
         loader = factory.create(BaseConfig(None), 'env')
         items = loader.load({})
         self.assertTrue(len(items) > 0)
 
-    def test_file(self):
+    def test_file_abspath(self):
         factory = ValueLoaderFactory()
         loader = factory.create(BaseConfig(None), 'file')
         items = loader.load({'file': __file__})
         self.assertIsNotNone(items.get(''))
         self.assertIn('class', items.get(''))
 
         items = loader.load({'file': __file__, 'conversion': 'base64'})
         self.assertNotIn('class', items.get(''))
+
+    def test_file_relpath(self):
+        factory = ValueLoaderFactory()
+        parent = os.path.abspath(os.path.join(os.path.dirname(__file__), '..', '..'))
+        loader = factory.create(BaseConfig(os.path.join(parent, 'tests', 'lib', '_root.yml')), 'file')
+        items = loader.load({'file': 'var-loader-app/dummy.pem'})
+        self.assertIsNotNone(items.get(''))
+        self.assertIn('BEGIN', items.get(''))
```

### Comparing `octoploy-1.2.2/tests/utils/EncryptionTest.py` & `octoploy-1.2.3/tests/utils/EncryptionTest.py`

 * *Files identical despite different names*

