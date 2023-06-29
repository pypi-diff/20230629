# Comparing `tmp/peek-plugin-livedb-3.4.5.tar.gz` & `tmp/peek-plugin-livedb-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-livedb-3.4.5.tar", last modified: Wed Jun 28 07:28:29 2023, max compression
+gzip compressed data, was "peek-plugin-livedb-3.4.6.tar", last modified: Thu Jun 29 10:22:16 2023, max compression
```

## Comparing `peek-plugin-livedb-3.4.5.tar` & `peek-plugin-livedb-3.4.6.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.495115 peek-plugin-livedb-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-28 07:28:29.495115 peek-plugin-livedb-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      338 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.490115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/
--rw-r--r--   0 root         (0) root         (0)     1155 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.ts
--rw-r--r--   0 root         (0) root         (0)     1603 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/livedb.component.html
--rw-r--r--   0 root         (0) root         (0)      209 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/livedb.component.ts
--rw-r--r--   0 root         (0) root         (0)     2242 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/livedb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)      870 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      953 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/tuples/AdminStatusTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.491115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      323 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.492115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1264 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/19b2a8d326ad_removed_string_lengths.py
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/1f014c013f8b_fixed_nullable_queue_rawvalue.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/64309a77b48d_initial.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1403 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/ab9da4532175_fixed_key_modelset_index.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/b0b08aff8542_added_unique_constraing_to_model_set.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/d4ffb9c5cb27_added_queue_table.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.492115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/client/
--rw-r--r--   0 root         (0) root         (0)      636 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.492115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/
--rw-r--r--   0 root         (0) root         (0)     1886 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBApi.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBReadApi.py
--rw-r--r--   0 root         (0) root         (0)     2807 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBWriteApi.py
--rw-r--r--   0 root         (0) root         (0)     6335 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      536 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1306 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.492115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)      979 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1733 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/StringIntTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      374 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/AdminStatusController.py
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/LiveDbController.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/LiveDbImportController.py
--rw-r--r--   0 root         (0) root         (0)     5272 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/LiveDbValueUpdateQueueController.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      931 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1968 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbItem.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbModelSet.py
--rw-r--r--   0 root         (0) root         (0)     1276 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbRawValueQueue.py
--rw-r--r--   0 root         (0) root         (0)     7653 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      418 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.493115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     1435 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/BulkLoadChunkTask.py
--rw-r--r--   0 root         (0) root         (0)     3271 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/LiveDbItemImportTask.py
--rw-r--r--   0 root         (0) root         (0)     5682 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/LiveDbItemUpdateTask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.494115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/
--rw-r--r--   0 root         (0) root         (0)      638 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/index.rst
--rwxr-xr-x   0 root         (0) root         (0)    24208 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/live_db_edit_settings.png
--rwxr-xr-x   0 root         (0) root         (0)    22172 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/live_db_status.png
--rw-r--r--   0 root         (0) root         (0)     1563 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.490115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.494115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      367 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.494115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/AddIntValueActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/LiveDBTuple.ts
--rw-r--r--   0 root         (0) root         (0)      569 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/StringCapToggleActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/StringIntTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1018 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.494115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/
--rw-r--r--   0 root         (0) root         (0)      739 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBApiABC.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBReadApiABC.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBWriteApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.495115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/ImportLiveDbItemTuple.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbDisplayValueTuple.py
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbDisplayValueUpdateTuple.py
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbRawValueTuple.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbRawValueUpdateTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.495115 peek-plugin-livedb-3.4.5/peek_plugin_livedb/worker/
--rw-r--r--   0 root         (0) root         (0)     2119 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/worker/WorkerApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:29.490115 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      396 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4994 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:28:29.496115 peek-plugin-livedb-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2023-06-28 07:28:29.000000 peek-plugin-livedb-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.776626 peek-plugin-livedb-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-29 10:22:16.776626 peek-plugin-livedb-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      338 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.771626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.771626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.771626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.771626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/livedb.component.html
+-rw-r--r--   0 root         (0) root         (0)      209 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/livedb.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/livedb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)      870 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      953 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/tuples/AdminStatusTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      323 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/19b2a8d326ad_removed_string_lengths.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/1f014c013f8b_fixed_nullable_queue_rawvalue.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/64309a77b48d_initial.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/ab9da4532175_fixed_key_modelset_index.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/b0b08aff8542_added_unique_constraing_to_model_set.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/d4ffb9c5cb27_added_queue_table.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.772626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/client/
+-rw-r--r--   0 root         (0) root         (0)      636 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.773626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBApi.py
+-rw-r--r--   0 root         (0) root         (0)     3731 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBReadApi.py
+-rw-r--r--   0 root         (0) root         (0)     2807 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBWriteApi.py
+-rw-r--r--   0 root         (0) root         (0)     6335 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      536 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1306 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.773626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)      979 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1733 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/StringIntTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      374 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.773626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/AdminStatusController.py
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/LiveDbController.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/LiveDbImportController.py
+-rw-r--r--   0 root         (0) root         (0)     5272 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/LiveDbValueUpdateQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.773626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      931 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1968 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbItem.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbModelSet.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbRawValueQueue.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/BulkLoadChunkTask.py
+-rw-r--r--   0 root         (0) root         (0)     3271 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/LiveDbItemImportTask.py
+-rw-r--r--   0 root         (0) root         (0)     5682 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/LiveDbItemUpdateTask.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)      638 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/index.rst
+-rwxr-xr-x   0 root         (0) root         (0)    24208 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/live_db_edit_settings.png
+-rwxr-xr-x   0 root         (0) root         (0)    22172 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/live_db_status.png
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.770626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.774626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      367 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.775626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/AddIntValueActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/LiveDBTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      569 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/StringCapToggleActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      461 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/StringIntTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.775626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/
+-rw-r--r--   0 root         (0) root         (0)      739 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBReadApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBWriteApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.775626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/
+-rw-r--r--   0 root         (0) root         (0)      781 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/ImportLiveDbItemTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbDisplayValueTuple.py
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbDisplayValueUpdateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbRawValueTuple.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbRawValueUpdateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.775626 peek-plugin-livedb-3.4.6/peek_plugin_livedb/worker/
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/worker/WorkerApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:22:16.771626 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      396 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4994 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:22:16.776626 peek-plugin-livedb-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2023-06-29 10:22:16.000000 peek-plugin-livedb-3.4.6/setup.py
```

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/__init__.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/livedb.component.html` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/livedb.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/livedb.module.ts` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/livedb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/status/status.component.html` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/admin-app/status/status.component.ts` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/agent/AgentEntryHook.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/script.py.mako` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/19b2a8d326ad_removed_string_lengths.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/19b2a8d326ad_removed_string_lengths.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/1f014c013f8b_fixed_nullable_queue_rawvalue.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/1f014c013f8b_fixed_nullable_queue_rawvalue.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/64309a77b48d_initial.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/64309a77b48d_initial.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/ab9da4532175_fixed_key_modelset_index.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/ab9da4532175_fixed_key_modelset_index.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/b0b08aff8542_added_unique_constraing_to_model_set.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/b0b08aff8542_added_unique_constraing_to_model_set.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/alembic/versions/d4ffb9c5cb27_added_queue_table.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/alembic/versions/d4ffb9c5cb27_added_queue_table.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/client/ClientEntryHook.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBApi.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBReadApi.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBReadApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LiveDBWriteApi.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LiveDBWriteApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/LogicEntryHook.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/TupleActionProcessor.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/TupleDataObservable.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/admin_backend/StringIntTableHandler.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/admin_backend/StringIntTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/LiveDbImportController.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/LiveDbImportController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/LiveDbValueUpdateQueueController.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/LiveDbValueUpdateQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/controller/MainController.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/DeclarativeBase.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbItem.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbItem.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbModelSet.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbModelSet.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/LiveDbRawValueQueue.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/LiveDbRawValueQueue.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/storage/Setting.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/WorkerEntryHook.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/BulkLoadChunkTask.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/BulkLoadChunkTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/LiveDbItemImportTask.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/LiveDbItemImportTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/_private/worker/tasks/LiveDbItemUpdateTask.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/_private/worker/tasks/LiveDbItemUpdateTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/admin_tasks.rst` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/live_db_edit_settings.png` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/live_db_edit_settings.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/live_db_status.png` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/live_db_status.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/admin-doc/overview.rst` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/plugin_package.json` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/plugin_package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -20,15 +20,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_livedb",
         "title": "Live DB",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "field",
         "office",
         "logic",
         "storage",
```

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBApiABC.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBReadApiABC.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBReadApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/server/LiveDBWriteApiABC.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/server/LiveDBWriteApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/ImportLiveDbItemTuple.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/ImportLiveDbItemTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbDisplayValueTuple.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbDisplayValueTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/tuples/LiveDbRawValueTuple.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/tuples/LiveDbRawValueTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb/worker/WorkerApi.py` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb/worker/WorkerApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/peek_plugin_livedb.egg-info/SOURCES.txt` & `peek-plugin-livedb-3.4.6/peek_plugin_livedb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-livedb-3.4.5/setup.py` & `peek-plugin-livedb-3.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_livedb"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin LiveDB - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

