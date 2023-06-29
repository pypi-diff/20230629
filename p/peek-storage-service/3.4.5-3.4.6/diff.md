# Comparing `tmp/peek-storage-service-3.4.5.tar.gz` & `tmp/peek-storage-service-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-storage-service-3.4.5.tar", last modified: Wed Jun 28 07:27:26 2023, max compression
+gzip compressed data, was "peek-storage-service-3.4.6.tar", last modified: Thu Jun 29 10:21:14 2023, max compression
```

## Comparing `peek-storage-service-3.4.5.tar` & `peek-storage-service-3.4.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.274094 peek-storage-service-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 07:27:26.275094 peek-storage-service-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.271094 peek-storage-service-3.4.5/peek_storage_service/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.271094 peek-storage-service-3.4.5/peek_storage_service/_private/
--rw-r--r--   0 root         (0) root         (0)     2560 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/StorageInit.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.271094 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)     2516 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/env.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.272094 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2162 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_run_generic_python.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.272094 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      406 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/34490abd765c_add_pg_load_payload_tuples.py
--rw-r--r--   0 root         (0) root         (0)      402 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/bab14faf0cd7_add_timescale.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.273094 peek-storage-service-3.4.5/peek_storage_service/_private/plugin/
--rw-r--r--   0 root         (0) root         (0)     1791 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/plugin/StoragePluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/plugin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.273094 peek-storage-service-3.4.5/peek_storage_service/_private/service/
--rw-r--r--   0 root         (0) root         (0)      988 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/PeekStorageConfig.py
--rw-r--r--   0 root         (0) root         (0)      675 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/StorageSiteResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.273094 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/
--rw-r--r--   0 root         (0) root         (0)     1616 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.274094 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_install/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.274094 peek-storage-service-3.4.5/peek_storage_service/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     8581 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.274094 peek-storage-service-3.4.5/peek_storage_service/_private/test/
--rw-r--r--   0 root         (0) root         (0)     1276 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/test/StorageTestMixin.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/_private/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.274094 peek-storage-service-3.4.5/peek_storage_service/plpython/
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/plpython/LoadPayloadPgUtil.py
--rw-r--r--   0 root         (0) root         (0)     1952 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/plpython/RunPyInPg.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/plpython/RunPyInPgTest.py
--rw-r--r--   0 root         (0) root         (0)     1353 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/plpython/RunWorkerTaskPyInPg.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/plpython/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6313 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/run_peek_storage_service.py
--rw-r--r--   0 root         (0) root         (0)     1460 2023-06-28 07:25:24.000000 peek-storage-service-3.4.5/peek_storage_service/winsvc_peek_storage_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:26.271094 peek-storage-service-3.4.5/peek_storage_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2915 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/peek_storage_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-06-28 07:27:26.277094 peek-storage-service-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-28 07:27:26.000000 peek-storage-service-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.474505 peek-storage-service-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-29 10:21:14.474505 peek-storage-service-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.471505 peek-storage-service-3.4.6/peek_storage_service/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.472505 peek-storage-service-3.4.6/peek_storage_service/_private/
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/StorageInit.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.472505 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/env.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.472505 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py
+-rw-r--r--   0 root         (0) root         (0)     2906 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_run_generic_python.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.472505 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      406 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/12a0ab3826f3_add_run_generic_python.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/34490abd765c_add_pg_load_payload_tuples.py
+-rw-r--r--   0 root         (0) root         (0)      402 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/51e48a6594d5_up1_run_generic_py.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/72518909970f_add_run_worker_plpy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/bab14faf0cd7_add_timescale.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/plugin/StoragePluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/plugin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/service/
+-rw-r--r--   0 root         (0) root         (0)      988 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/PeekStorageConfig.py
+-rw-r--r--   0 root         (0) root         (0)      675 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/StorageSiteResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/
+-rw-r--r--   0 root         (0) root         (0)     1616 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_install/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      453 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     8581 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.473505 peek-storage-service-3.4.6/peek_storage_service/_private/test/
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/test/StorageTestMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/_private/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.474505 peek-storage-service-3.4.6/peek_storage_service/plpython/
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/plpython/LoadPayloadPgUtil.py
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/plpython/RunPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/plpython/RunPyInPgTest.py
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/plpython/RunWorkerTaskPyInPg.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/plpython/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6313 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/run_peek_storage_service.py
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-06-29 10:19:15.000000 peek-storage-service-3.4.6/peek_storage_service/winsvc_peek_storage_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:14.472505 peek-storage-service-3.4.6/peek_storage_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2915 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/peek_storage_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-06-29 10:21:14.474505 peek-storage-service-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-29 10:21:14.000000 peek-storage-service-3.4.6/setup.py
```

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/StorageInit.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/StorageInit.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/alembic/env.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/alembic/env.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_load_paylaod_tuples.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_run_generic_python.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_run_generic_python.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/alembic/objects/object_run_worker_task_python.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/alembic/versions/2efc91c0f0f6_add_plpython3u.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/plugin/PeekStoragePlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/plugin/StoragePluginLoader.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/plugin/StoragePluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/plugin/StoragePluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/service/PeekStorageConfig.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/service/PeekStorageConfig.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/service/StorageSiteResource.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/service/StorageSiteResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/PeekSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_download/PluginSwDownloadResource.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/storage/Setting.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/storage/__init__.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/_private/test/StorageTestMixin.py` & `peek-storage-service-3.4.6/peek_storage_service/_private/test/StorageTestMixin.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/plpython/LoadPayloadPgUtil.py` & `peek-storage-service-3.4.6/peek_storage_service/plpython/LoadPayloadPgUtil.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/plpython/RunPyInPg.py` & `peek-storage-service-3.4.6/peek_storage_service/plpython/RunPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/plpython/RunPyInPgTest.py` & `peek-storage-service-3.4.6/peek_storage_service/plpython/RunPyInPgTest.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/plpython/RunWorkerTaskPyInPg.py` & `peek-storage-service-3.4.6/peek_storage_service/plpython/RunWorkerTaskPyInPg.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/run_peek_storage_service.py` & `peek-storage-service-3.4.6/peek_storage_service/run_peek_storage_service.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service/winsvc_peek_storage_service.py` & `peek-storage-service-3.4.6/peek_storage_service/winsvc_peek_storage_service.py`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/peek_storage_service.egg-info/SOURCES.txt` & `peek-storage-service-3.4.6/peek_storage_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-storage-service-3.4.5/setup.py` & `peek-storage-service-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_storage_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Storage Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

