# Comparing `tmp/peek-plugin-base-3.4.5.tar.gz` & `tmp/peek-plugin-base-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-base-3.4.5.tar", last modified: Wed Jun 28 07:27:18 2023, max compression
+gzip compressed data, was "peek-plugin-base-3.4.6.tar", last modified: Thu Jun 29 10:21:06 2023, max compression
```

## Comparing `peek-plugin-base-3.4.5.tar` & `peek-plugin-base-3.4.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.645091 peek-plugin-base-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-28 07:27:18.645091 peek-plugin-base-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.642091 peek-plugin-base-3.4.5/peek_plugin_base/
--rw-r--r--   0 root         (0) root         (0)      871 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/LoopingCallUtil.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformCommonHookABC.py
--rw-r--r--   0 root         (0) root         (0)      830 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformFileStorageHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformServerInfoHookABC.py
--rw-r--r--   0 root         (0) root         (0)      976 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PeekVortexUtil.py
--rw-r--r--   0 root         (0) root         (0)     1765 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PluginCommonEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2094 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/PluginPackageFileConfig.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.642091 peek-plugin-base-3.4.5/peek_plugin_base/agent/
--rw-r--r--   0 root         (0) root         (0)      462 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/agent/PeekAgentPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1200 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1481 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/agent/PluginAgentEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.643092 peek-plugin-base-3.4.5/peek_plugin_base/client/
--rw-r--r--   0 root         (0) root         (0)      705 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/client/PeekClientPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/client/PluginClientEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.643092 peek-plugin-base-3.4.5/peek_plugin_base/server/
--rw-r--r--   0 root         (0) root         (0)     1660 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1060 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PeekServerPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PluginLogicEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PluginServerStorageEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/PluginServerWorkerEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.643092 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2610 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py
--rw-r--r--   0 root         (0) root         (0)     3063 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_task_call_tuple.py
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_task_constructor_tuple.py
--rw-r--r--   0 root         (0) root         (0)      483 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_task_result_tuple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.644091 peek-plugin-base-3.4.5/peek_plugin_base/storage/
--rw-r--r--   0 root         (0) root         (0)     2613 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/AlembicEnvBase.py
--rw-r--r--   0 root         (0) root         (0)    11090 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/DbConnection.py
--rw-r--r--   0 root         (0) root         (0)     1253 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/LoadPayloadPgUtil.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/RunPyInPg.py
--rw-r--r--   0 root         (0) root         (0)     1863 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/StorageUtil.py
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/TypeDecorators.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.644091 peek-plugin-base-3.4.5/peek_plugin_base/util/
--rw-r--r--   0 root         (0) root         (0)     4770 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/PeekPsUtil.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.644091 peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/
--rw-r--r--   0 root         (0) root         (0)     3744 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/BuilderABC.py
--rw-r--r--   0 root         (0) root         (0)     2023 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/BuilderOsCmd.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.644091 peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/
--rw-r--r--   0 root         (0) root         (0)     3656 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/DocBuilder.py
--rw-r--r--   0 root         (0) root         (0)     7496 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/DocBuilderABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.644091 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/
--rw-r--r--   0 root         (0) root         (0)     5184 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py
--rw-r--r--   0 root         (0) root         (0)    22377 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py
--rw-r--r--   0 root         (0) root         (0)    14140 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/FrontendFileSync.py
--rw-r--r--   0 root         (0) root         (0)     9870 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/WebBuilder.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.645091 peek-plugin-base-3.4.5/peek_plugin_base/worker/
--rw-r--r--   0 root         (0) root         (0)       57 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryApp.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryDbConn.py
--rw-r--r--   0 root         (0) root         (0)     1781 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryDbConnInit.py
--rw-r--r--   0 root         (0) root         (0)      308 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryFileStorageConfig.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryLogicServerInfoConfig.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/PeekWorkerPlatformHookABC.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/PluginWorkerEntryHookABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-plugin-base-3.4.5/peek_plugin_base/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:18.642091 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/
--rw-r--r--   0 root         (0) root         (0)      365 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3180 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      264 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/peek_plugin_base.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:27:18.645091 peek-plugin-base-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2665 2023-06-28 07:27:18.000000 peek-plugin-base-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.926491 peek-plugin-base-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-29 10:21:06.926491 peek-plugin-base-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.923491 peek-plugin-base-3.4.6/peek_plugin_base/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/LoopingCallUtil.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformCommonHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      830 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformFileStorageHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformServerInfoHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      976 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PeekVortexUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1765 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PluginCommonEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2094 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/PluginPackageFileConfig.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.923491 peek-plugin-base-3.4.6/peek_plugin_base/agent/
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/agent/PeekAgentPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1200 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/agent/PluginAgentEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.923491 peek-plugin-base-3.4.6/peek_plugin_base/client/
+-rw-r--r--   0 root         (0) root         (0)      705 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/client/PeekClientPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/client/PluginClientEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.924491 peek-plugin-base-3.4.6/peek_plugin_base/server/
+-rw-r--r--   0 root         (0) root         (0)     1660 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PeekServerPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PluginLogicEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PluginServerStorageEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/PluginServerWorkerEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.924491 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2610 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_task_call_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_task_constructor_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      483 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_task_result_tuple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.925491 peek-plugin-base-3.4.6/peek_plugin_base/storage/
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/AlembicEnvBase.py
+-rw-r--r--   0 root         (0) root         (0)    11090 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/DbConnection.py
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/LoadPayloadPgUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/RunPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/StorageUtil.py
+-rw-r--r--   0 root         (0) root         (0)      292 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/TypeDecorators.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.925491 peek-plugin-base-3.4.6/peek_plugin_base/util/
+-rw-r--r--   0 root         (0) root         (0)     4770 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/PeekPsUtil.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.925491 peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/
+-rw-r--r--   0 root         (0) root         (0)     3744 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/BuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/BuilderOsCmd.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.925491 peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/
+-rw-r--r--   0 root         (0) root         (0)     3656 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/DocBuilder.py
+-rw-r--r--   0 root         (0) root         (0)     7496 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/DocBuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.925491 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/
+-rw-r--r--   0 root         (0) root         (0)     5184 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py
+-rw-r--r--   0 root         (0) root         (0)    22377 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py
+-rw-r--r--   0 root         (0) root         (0)    14140 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/FrontendFileSync.py
+-rw-r--r--   0 root         (0) root         (0)     9870 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/WebBuilder.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.926491 peek-plugin-base-3.4.6/peek_plugin_base/worker/
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryApp.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryDbConn.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryDbConnInit.py
+-rw-r--r--   0 root         (0) root         (0)      308 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryFileStorageConfig.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryLogicServerInfoConfig.py
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/PeekWorkerPlatformHookABC.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/PluginWorkerEntryHookABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-plugin-base-3.4.6/peek_plugin_base/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:06.923491 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      365 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3180 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      264 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/peek_plugin_base.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:21:06.926491 peek-plugin-base-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2665 2023-06-29 10:21:06.000000 peek-plugin-base-3.4.6/setup.py
```

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/LoopingCallUtil.py` & `peek-plugin-base-3.4.6/peek_plugin_base/LoopingCallUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformCommonHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformCommonHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformFileStorageHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformFileStorageHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PeekPlatformServerInfoHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PeekPlatformServerInfoHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PeekVortexUtil.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PeekVortexUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PlatformDependencyTest.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PluginCommonEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PluginCommonEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/PluginPackageFileConfig.py` & `peek-plugin-base-3.4.6/peek_plugin_base/PluginPackageFileConfig.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/agent/PeekPlatformAgentHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/agent/PluginAgentEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/agent/PluginAgentEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/client/PeekClientPlatformHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/client/PeekClientPlatformHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/client/PeekPlatformFieldHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/client/PeekPlatformOfficeHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/client/PluginClientEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/client/PluginClientEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PeekPlatformAdminHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PeekPlatformServerHttpHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PeekServerPlatformHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PeekServerPlatformHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PluginLogicEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PluginLogicEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PluginLogicEntryHookInheritenceTest.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/server/PluginServerStorageEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/server/PluginServerStorageEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py` & `peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_child_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py` & `peek-plugin-base-3.4.6/peek_plugin_base/simple_subproc/simple_subproc_parent_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/storage/AlembicEnvBase.py` & `peek-plugin-base-3.4.6/peek_plugin_base/storage/AlembicEnvBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/storage/DbConnection.py` & `peek-plugin-base-3.4.6/peek_plugin_base/storage/DbConnection.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/storage/LoadPayloadPgUtil.py` & `peek-plugin-base-3.4.6/peek_plugin_base/storage/LoadPayloadPgUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/storage/RunPyInPg.py` & `peek-plugin-base-3.4.6/peek_plugin_base/storage/RunPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/storage/StorageUtil.py` & `peek-plugin-base-3.4.6/peek_plugin_base/storage/StorageUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/PeekPsUtil.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/PeekPsUtil.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/BuilderABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/BuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_common/BuilderOsCmd.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_common/BuilderOsCmd.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/DocBuilder.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/DocBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_doc/DocBuilderABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_doc/DocBuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/EdnarWebBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/FrontendBuilderABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/FrontendFileSync.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/FrontendFileSync.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/util/build_frontend/WebBuilder.py` & `peek-plugin-base-3.4.6/peek_plugin_base/util/build_frontend/WebBuilder.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryDbConn.py` & `peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryDbConn.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/worker/CeleryDbConnInit.py` & `peek-plugin-base-3.4.6/peek_plugin_base/worker/CeleryDbConnInit.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base/worker/PluginWorkerEntryHookABC.py` & `peek-plugin-base-3.4.6/peek_plugin_base/worker/PluginWorkerEntryHookABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/peek_plugin_base.egg-info/SOURCES.txt` & `peek-plugin-base-3.4.6/peek_plugin_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-base-3.4.5/setup.py` & `peek-plugin-base-3.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_base"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin Base."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

