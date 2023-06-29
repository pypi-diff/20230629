# Comparing `tmp/peek-logic-service-3.4.5.tar.gz` & `tmp/peek-logic-service-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-logic-service-3.4.5.tar", last modified: Wed Jun 28 07:26:59 2023, max compression
+gzip compressed data, was "peek-logic-service-3.4.6.tar", last modified: Thu Jun 29 10:20:48 2023, max compression
```

## Comparing `peek-logic-service-3.4.5.tar` & `peek-logic-service-3.4.6.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.734085 peek-logic-service-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:59.734085 peek-logic-service-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.731085 peek-logic-service-3.4.5/peek_logic_service/
--rw-r--r--   0 root         (0) root         (0)     2532 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/PeekServerConfig.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.731085 peek-logic-service-3.4.5/peek_logic_service/alembic/
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.731085 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      572 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/05cf60a0fd22_initial_setup.py
--rw-r--r--   0 root         (0) root         (0)      764 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/3aa82a9abe67_enabled_postgis.py
--rw-r--r--   0 root         (0) root         (0)      587 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/5ad8b58df646_create.py
--rw-r--r--   0 root         (0) root         (0)     3123 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/7923ec94177a_added_peek_environent_tables.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/bc1622f6c16c_added_file_dir_name_to_peekappinfo.py
--rw-r--r--   0 root         (0) root         (0)     2513 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/c2a3b93e178d_added_mssql_csvtotable.py
--rw-r--r--   0 root         (0) root         (0)     2948 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic/versions/c5e78990adf6_added_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/
--rw-r--r--   0 root         (0) root         (0)     2179 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/AdminSiteResource.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/auth/
--rw-r--r--   0 root         (0) root         (0)      916 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthChecker.py
--rw-r--r--   0 root         (0) root         (0)     1022 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthElement.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthRealm.py
--rw-r--r--   0 root         (0) root         (0)     2033 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthResource.py
--rw-r--r--   0 root         (0) root         (0)    71689 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthTemplate.xml
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminUserAccess.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/auth/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/dashboard/
--rw-r--r--   0 root         (0) root         (0)     2776 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/dashboard/PeekAdmDashboardListHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/dashboard/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/environment/
--rw-r--r--   0 root         (0) root         (0)     2900 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/environment/PeekAdmEnvHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/environment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/navbar/
--rw-r--r--   0 root         (0) root         (0)     1370 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/navbar/PeekAdmNavbarHandler.py
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/navbar/PeekAdmNavbarUserTuple.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/navbar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.732085 peek-logic-service-3.4.5/peek_logic_service/backend/setting/
--rw-r--r--   0 root         (0) root         (0)      870 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/setting/PeekAdmSettingHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/setting/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/backend/update/
--rw-r--r--   0 root         (0) root         (0)     2622 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/update/PeekAdmCapabilitiesHandler.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/update/PeekAdmUpdatePappInfoHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/backend/update/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     2054 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/plugin/PeekServerPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/plugin/ServerFrontendLoadersMixin.py
--rw-r--r--   0 root         (0) root         (0)     4345 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/plugin/ServerPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1613 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/plugin/ServerPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/plugin/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    11994 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/run_peek_logic_service.py
--rwxr-xr-x   0 root         (0) root         (0)     2968 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/run_peek_logic_service_build_only.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/server/
--rw-r--r--   0 root         (0) root         (0)      969 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/PlatformSiteResource.py
--rw-r--r--   0 root         (0) root         (0)      242 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/server/sw_download/
--rw-r--r--   0 root         (0) root         (0)     1665 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_download/PeekSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)     2342 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_download/PluginSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_download/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/server/sw_install/
--rw-r--r--   0 root         (0) root         (0)      952 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.733085 peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/
--rw-r--r--   0 root         (0) root         (0)     4481 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PeekSwUploadManager.py
--rw-r--r--   0 root         (0) root         (0)     2847 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PeekSwUploadResource.py
--rw-r--r--   0 root         (0) root         (0)     8850 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PluginSwUploadManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.734085 peek-logic-service-3.4.5/peek_logic_service/server/sw_version/
--rw-r--r--   0 root         (0) root         (0)     1954 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_version/PeekSwVersionDataHandler.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_version/PluginSwVersionInfoUtil.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/server/sw_version/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.734085 peek-logic-service-3.4.5/peek_logic_service/storage/
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     2755 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/storage/PeekEnv.py
--rw-r--r--   0 root         (0) root         (0)     1396 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/storage/PeekPluginInfo.py
--rw-r--r--   0 root         (0) root         (0)     9178 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-28 07:25:24.000000 peek-logic-service-3.4.5/peek_logic_service/winsvc_peek_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:59.731085 peek-logic-service-3.4.5/peek_logic_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3652 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      263 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/peek_logic_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:59.734085 peek-logic-service-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3085 2023-06-28 07:26:59.000000 peek-logic-service-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.092454 peek-logic-service-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:20:48.092454 peek-logic-service-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.088454 peek-logic-service-3.4.6/peek_logic_service/
+-rw-r--r--   0 root         (0) root         (0)     2532 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/PeekServerConfig.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-29 10:20:47.000000 peek-logic-service-3.4.6/peek_logic_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.089454 peek-logic-service-3.4.6/peek_logic_service/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.089454 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/05cf60a0fd22_initial_setup.py
+-rw-r--r--   0 root         (0) root         (0)      764 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/3aa82a9abe67_enabled_postgis.py
+-rw-r--r--   0 root         (0) root         (0)      587 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/5ad8b58df646_create.py
+-rw-r--r--   0 root         (0) root         (0)     3123 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/7923ec94177a_added_peek_environent_tables.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/bc1622f6c16c_added_file_dir_name_to_peekappinfo.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/c2a3b93e178d_added_mssql_csvtotable.py
+-rw-r--r--   0 root         (0) root         (0)     2948 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic/versions/c5e78990adf6_added_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.089454 peek-logic-service-3.4.6/peek_logic_service/backend/
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/AdminSiteResource.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/auth/
+-rw-r--r--   0 root         (0) root         (0)      916 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthChecker.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthElement.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthRealm.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthResource.py
+-rw-r--r--   0 root         (0) root         (0)    71689 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthTemplate.xml
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminUserAccess.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/auth/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/dashboard/
+-rw-r--r--   0 root         (0) root         (0)     2776 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/dashboard/PeekAdmDashboardListHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/dashboard/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/environment/
+-rw-r--r--   0 root         (0) root         (0)     2900 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/environment/PeekAdmEnvHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/environment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/navbar/
+-rw-r--r--   0 root         (0) root         (0)     1370 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/navbar/PeekAdmNavbarHandler.py
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/navbar/PeekAdmNavbarUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/navbar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/setting/
+-rw-r--r--   0 root         (0) root         (0)      870 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/setting/PeekAdmSettingHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/setting/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.090454 peek-logic-service-3.4.6/peek_logic_service/backend/update/
+-rw-r--r--   0 root         (0) root         (0)     2622 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/update/PeekAdmCapabilitiesHandler.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/update/PeekAdmUpdatePappInfoHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/backend/update/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     2054 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/plugin/PeekServerPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/plugin/ServerFrontendLoadersMixin.py
+-rw-r--r--   0 root         (0) root         (0)     4345 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/plugin/ServerPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1613 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/plugin/ServerPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/plugin/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    11994 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/run_peek_logic_service.py
+-rwxr-xr-x   0 root         (0) root         (0)     2968 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/run_peek_logic_service_build_only.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/server/
+-rw-r--r--   0 root         (0) root         (0)      969 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/PlatformSiteResource.py
+-rw-r--r--   0 root         (0) root         (0)      242 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/server/sw_download/
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_download/PeekSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)     2342 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_download/PluginSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_download/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/server/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      952 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PeekSwUploadManager.py
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PeekSwUploadResource.py
+-rw-r--r--   0 root         (0) root         (0)     8850 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PluginSwUploadManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.091454 peek-logic-service-3.4.6/peek_logic_service/server/sw_version/
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_version/PeekSwVersionDataHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_version/PluginSwVersionInfoUtil.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/server/sw_version/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.092454 peek-logic-service-3.4.6/peek_logic_service/storage/
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/storage/PeekEnv.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/storage/PeekPluginInfo.py
+-rw-r--r--   0 root         (0) root         (0)     9178 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-29 10:19:15.000000 peek-logic-service-3.4.6/peek_logic_service/winsvc_peek_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:48.089454 peek-logic-service-3.4.6/peek_logic_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3652 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      263 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 10:20:48.000000 peek-logic-service-3.4.6/peek_logic_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:48.092454 peek-logic-service-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-06-29 10:20:47.000000 peek-logic-service-3.4.6/setup.py
```

### Comparing `peek-logic-service-3.4.5/peek_logic_service/PeekServerConfig.py` & `peek-logic-service-3.4.6/peek_logic_service/PeekServerConfig.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/env.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/env.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/05cf60a0fd22_initial_setup.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/05cf60a0fd22_initial_setup.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/3aa82a9abe67_enabled_postgis.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/3aa82a9abe67_enabled_postgis.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/5ad8b58df646_create.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/5ad8b58df646_create.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/7923ec94177a_added_peek_environent_tables.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/7923ec94177a_added_peek_environent_tables.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/bc1622f6c16c_added_file_dir_name_to_peekappinfo.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/bc1622f6c16c_added_file_dir_name_to_peekappinfo.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/c2a3b93e178d_added_mssql_csvtotable.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/c2a3b93e178d_added_mssql_csvtotable.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/alembic/versions/c5e78990adf6_added_initial_tables.py` & `peek-logic-service-3.4.6/peek_logic_service/alembic/versions/c5e78990adf6_added_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/AdminSiteResource.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/AdminSiteResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthChecker.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthChecker.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthElement.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthElement.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthRealm.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthRealm.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthResource.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/auth/AdminAuthTemplate.xml` & `peek-logic-service-3.4.6/peek_logic_service/backend/auth/AdminAuthTemplate.xml`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/dashboard/PeekAdmDashboardListHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/dashboard/PeekAdmDashboardListHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/environment/PeekAdmEnvHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/environment/PeekAdmEnvHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/navbar/PeekAdmNavbarHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/navbar/PeekAdmNavbarHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/setting/PeekAdmSettingHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/setting/PeekAdmSettingHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/update/PeekAdmCapabilitiesHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/update/PeekAdmCapabilitiesHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/backend/update/PeekAdmUpdatePappInfoHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/backend/update/PeekAdmUpdatePappInfoHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/plugin/PeekServerPlatformHook.py` & `peek-logic-service-3.4.6/peek_logic_service/plugin/PeekServerPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/plugin/ServerFrontendLoadersMixin.py` & `peek-logic-service-3.4.6/peek_logic_service/plugin/ServerFrontendLoadersMixin.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/plugin/ServerPluginLoader.py` & `peek-logic-service-3.4.6/peek_logic_service/plugin/ServerPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/plugin/ServerPluginLoaderTest.py` & `peek-logic-service-3.4.6/peek_logic_service/plugin/ServerPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/run_peek_logic_service.py` & `peek-logic-service-3.4.6/peek_logic_service/run_peek_logic_service.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/run_peek_logic_service_build_only.py` & `peek-logic-service-3.4.6/peek_logic_service/run_peek_logic_service_build_only.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/PlatformSiteResource.py` & `peek-logic-service-3.4.6/peek_logic_service/server/PlatformSiteResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_download/PeekSwDownloadResource.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_download/PeekSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_download/PluginSwDownloadResource.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_download/PluginSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_install/PeekSwInstallManager.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PeekSwUploadManager.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PeekSwUploadManager.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PeekSwUploadResource.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PeekSwUploadResource.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_upload/PluginSwUploadManager.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_upload/PluginSwUploadManager.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_version/PeekSwVersionDataHandler.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_version/PeekSwVersionDataHandler.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/server/sw_version/PluginSwVersionInfoUtil.py` & `peek-logic-service-3.4.6/peek_logic_service/server/sw_version/PluginSwVersionInfoUtil.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/storage/PeekEnv.py` & `peek-logic-service-3.4.6/peek_logic_service/storage/PeekEnv.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/storage/PeekPluginInfo.py` & `peek-logic-service-3.4.6/peek_logic_service/storage/PeekPluginInfo.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/storage/Setting.py` & `peek-logic-service-3.4.6/peek_logic_service/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/storage/__init__.py` & `peek-logic-service-3.4.6/peek_logic_service/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service/winsvc_peek_server.py` & `peek-logic-service-3.4.6/peek_logic_service/winsvc_peek_server.py`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/peek_logic_service.egg-info/SOURCES.txt` & `peek-logic-service-3.4.6/peek_logic_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-logic-service-3.4.5/setup.py` & `peek-logic-service-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_logic_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Logic Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

