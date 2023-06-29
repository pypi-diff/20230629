# Comparing `tmp/peek-platform-3.4.5.tar.gz` & `tmp/peek-platform-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-platform-3.4.5.tar", last modified: Wed Jun 28 07:27:22 2023, max compression
+gzip compressed data, was "peek-platform-3.4.6.tar", last modified: Thu Jun 29 10:21:10 2023, max compression
```

## Comparing `peek-platform-3.4.5.tar` & `peek-platform-3.4.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.579093 peek-platform-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      353 2023-06-28 07:27:22.579093 peek-platform-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       96 2023-06-28 07:25:24.000000 peek-platform-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.576093 peek-platform-3.4.5/peek_platform/
--rw-r--r--   0 root         (0) root         (0)     4386 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/CeleryPatchToPlPython.py
--rw-r--r--   0 root         (0) root         (0)     7177 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/ConfigCeleryApp.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/WindowsPatch.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.577093 peek-platform-3.4.5/peek_platform/file_config/
--rw-r--r--   0 root         (0) root         (0)     3628 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigABC.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py
--rw-r--r--   0 root         (0) root         (0)     2527 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDocBuildMixin.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigHttpServerMixin.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigOsMixin.py
--rw-r--r--   0 root         (0) root         (0)     8032 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigPlatformMixin.py
--rw-r--r--   0 root         (0) root         (0)     1388 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigTest.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigWorkerMixin.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/file_config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.577093 peek-platform-3.4.5/peek_platform/platform_init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/platform_init/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11125 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/platform_init/init_platform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.577093 peek-platform-3.4.5/peek_platform/plugin/
--rw-r--r--   0 root         (0) root         (0)    17891 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/plugin/PluginLoaderABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.578093 peek-platform-3.4.5/peek_platform/subproc_plugin_init/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.578093 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4004 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py
--rw-r--r--   0 root         (0) root         (0)     2999 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py
--rw-r--r--   0 root         (0) root         (0)     3270 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_constants.py
--rw-r--r--   0 root         (0) root         (0)     7744 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py
--rw-r--r--   0 root         (0) root         (0)      353 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_platform_config_tuple.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py
--rw-r--r--   0 root         (0) root         (0)     5294 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py
--rw-r--r--   0 root         (0) root         (0)     4401 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.578093 peek-platform-3.4.5/peek_platform/sw_install/
--rw-r--r--   0 root         (0) root         (0)     9495 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_install/PeekSwInstallManagerABC.py
--rw-r--r--   0 root         (0) root         (0)     8235 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_install/PluginSwInstallManagerABC.py
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.579093 peek-platform-3.4.5/peek_platform/sw_version/
--rw-r--r--   0 root         (0) root         (0)     3875 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_version/PeekSwVersionPollHandler.py
--rw-r--r--   0 root         (0) root         (0)      332 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_version/PeekSwVersionTuple.py
--rw-r--r--   0 root         (0) root         (0)      162 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/sw_version/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.579093 peek-platform-3.4.5/peek_platform/util/
--rw-r--r--   0 root         (0) root         (0)     2505 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/util/LogUtil.py
--rw-r--r--   0 root         (0) root         (0)     1719 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/util/ManHoleUtil.py
--rw-r--r--   0 root         (0) root         (0)     8893 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/util/MemUtil.py
--rw-r--r--   0 root         (0) root         (0)     7221 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/util/PtyUtil.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2676 2023-06-28 07:25:24.000000 peek-platform-3.4.5/peek_platform/winsvc_peek_restarter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:22.577093 peek-platform-3.4.5/peek_platform.egg-info/
--rw-r--r--   0 root         (0) root         (0)      353 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2857 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      530 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-28 07:27:22.000000 peek-platform-3.4.5/peek_platform.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-28 07:27:22.588093 peek-platform-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     4754 2023-06-28 07:27:22.000000 peek-platform-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.740498 peek-platform-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-29 10:21:10.740498 peek-platform-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       96 2023-06-29 10:19:15.000000 peek-platform-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.738498 peek-platform-3.4.6/peek_platform/
+-rw-r--r--   0 root         (0) root         (0)     4386 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/CeleryPatchToPlPython.py
+-rw-r--r--   0 root         (0) root         (0)     7177 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/ConfigCeleryApp.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/WindowsPatch.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.739498 peek-platform-3.4.6/peek_platform/file_config/
+-rw-r--r--   0 root         (0) root         (0)     3628 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigABC.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2527 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDocBuildMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py
+-rw-r--r--   0 root         (0) root         (0)     1676 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigHttpServerMixin.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigOsMixin.py
+-rw-r--r--   0 root         (0) root         (0)     8032 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigPlatformMixin.py
+-rw-r--r--   0 root         (0) root         (0)     1388 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py
+-rw-r--r--   0 root         (0) root         (0)     3428 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigWorkerMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/file_config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.739498 peek-platform-3.4.6/peek_platform/platform_init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/platform_init/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11125 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/platform_init/init_platform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.739498 peek-platform-3.4.6/peek_platform/plugin/
+-rw-r--r--   0 root         (0) root         (0)    17891 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/plugin/PluginLoaderABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.739498 peek-platform-3.4.6/peek_platform/subproc_plugin_init/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.740498 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_constants.py
+-rw-r--r--   0 root         (0) root         (0)     7744 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_platform_config_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     5294 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py
+-rw-r--r--   0 root         (0) root         (0)     4401 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.740498 peek-platform-3.4.6/peek_platform/sw_install/
+-rw-r--r--   0 root         (0) root         (0)     9495 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_install/PeekSwInstallManagerABC.py
+-rw-r--r--   0 root         (0) root         (0)     8235 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_install/PluginSwInstallManagerABC.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.740498 peek-platform-3.4.6/peek_platform/sw_version/
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_version/PeekSwVersionPollHandler.py
+-rw-r--r--   0 root         (0) root         (0)      332 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_version/PeekSwVersionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      162 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/sw_version/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.740498 peek-platform-3.4.6/peek_platform/util/
+-rw-r--r--   0 root         (0) root         (0)     2505 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/util/LogUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/util/ManHoleUtil.py
+-rw-r--r--   0 root         (0) root         (0)     8893 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/util/MemUtil.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/util/PtyUtil.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2676 2023-06-29 10:19:15.000000 peek-platform-3.4.6/peek_platform/winsvc_peek_restarter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:10.738498 peek-platform-3.4.6/peek_platform.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2857 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      530 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 10:21:10.000000 peek-platform-3.4.6/peek_platform.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 10:21:10.741498 peek-platform-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4754 2023-06-29 10:21:10.000000 peek-platform-3.4.6/setup.py
```

### Comparing `peek-platform-3.4.5/peek_platform/CeleryPatchToPlPython.py` & `peek-platform-3.4.6/peek_platform/CeleryPatchToPlPython.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/ConfigCeleryApp.py` & `peek-platform-3.4.6/peek_platform/ConfigCeleryApp.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/WindowsPatch.py` & `peek-platform-3.4.6/peek_platform/WindowsPatch.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/__init__.py` & `peek-platform-3.4.6/peek_platform/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from . import WindowsPatch
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 class PeekPlatformConfig:
     """Peek Platform Config
 
     This is really a GLOBAL pettern, It should be replaced at some stage.
     (Maybe named as a factory?)
```

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigABC.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDataExchangeClientMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDataExchangeServerMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigDocBuildMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigDocBuildMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigFrontendDirMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigHttpServerMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigHttpServerMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigOsMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigOsMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigPlatformMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigPlatformMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigSqlAlchemyMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigTest.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/file_config/PeekFileConfigWorkerMixin.py` & `peek-platform-3.4.6/peek_platform/file_config/PeekFileConfigWorkerMixin.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/platform_init/init_platform.py` & `peek-platform-3.4.6/peek_platform/platform_init/init_platform.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/plugin/PluginLoaderABC.py` & `peek-platform-3.4.6/peek_platform/plugin/PluginLoaderABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_main.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_state_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_child_vortex_uuid_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_parent_protocol.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_msg_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc/plugin_subproc_vortex_payload_envelope_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc_parent_main.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py` & `peek-platform-3.4.6/peek_platform/subproc_plugin_init/plugin_subproc_parent_main_delegate.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/sw_install/PeekSwInstallManagerABC.py` & `peek-platform-3.4.6/peek_platform/sw_install/PeekSwInstallManagerABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/sw_install/PluginSwInstallManagerABC.py` & `peek-platform-3.4.6/peek_platform/sw_install/PluginSwInstallManagerABC.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/sw_version/PeekSwVersionPollHandler.py` & `peek-platform-3.4.6/peek_platform/sw_version/PeekSwVersionPollHandler.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/util/LogUtil.py` & `peek-platform-3.4.6/peek_platform/util/LogUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/util/ManHoleUtil.py` & `peek-platform-3.4.6/peek_platform/util/ManHoleUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/util/MemUtil.py` & `peek-platform-3.4.6/peek_platform/util/MemUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/util/PtyUtil.py` & `peek-platform-3.4.6/peek_platform/util/PtyUtil.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform/winsvc_peek_restarter.py` & `peek-platform-3.4.6/peek_platform/winsvc_peek_restarter.py`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform.egg-info/SOURCES.txt` & `peek-platform-3.4.6/peek_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-platform-3.4.5/peek_platform.egg-info/requires.txt` & `peek-platform-3.4.6/peek_platform.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 alembic>=0.8.7
 python-dateutil>=2.6.0
 Pygments>=2.0.1
 watchdog>=0.8.3
 pycryptodome
 cryptography<38.0.0
 flower<1.0.0
-peek-plugin-base==3.4.*,>=3.4.5
-peek-core-device==3.4.*,>=3.4.5
-peek-core-email==3.4.*,>=3.4.5
+peek-plugin-base==3.4.*,>=3.4.6
+peek-core-device==3.4.*,>=3.4.6
+peek-core-email==3.4.*,>=3.4.6
 psutil
 pexpect<5.0,>=4.8.0
 Shapely>=1.5.16
 pymssql
 future
 celery[auth,redis]<5.0.0
 coverage>=4.2
```

### Comparing `peek-platform-3.4.5/setup.py` & `peek-platform-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_platform"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Platform."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
@@ -89,15 +89,15 @@
 
 win_dependencies = [
     # "pymssql >= 2.1.3",  # DB-API interface to Microsoft SQL Server, requires FreeTDS
     "pycparser >= 2.17",
     "cffi >= 1.9.1",
     "cryptography <= 3.1.1",  # PEEK-1136
     "pytest >= 3.0.5",
-    "wheel >= 0.33.4.5",
+    "wheel >= 0.33.4.6",
     "virtualenv >= 15.1.0",
     # Celery 4 is not supported on windows
     "celery[redis,auth]<4.0.0",
     # Service support for windows
     "pypiwin32",
 ]
```

