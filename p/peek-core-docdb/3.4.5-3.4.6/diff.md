# Comparing `tmp/peek-core-docdb-3.4.5.tar.gz` & `tmp/peek-core-docdb-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-docdb-3.4.5.tar", last modified: Wed Jun 28 07:26:18 2023, max compression
+gzip compressed data, was "peek-core-docdb-3.4.6.tar", last modified: Thu Jun 29 10:20:08 2023, max compression
```

## Comparing `peek-core-docdb-3.4.5.tar` & `peek-core-docdb-3.4.6.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      368 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      217 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.790072 peek-core-docdb-3.4.5/peek_core_docdb/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     3281 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/docDb.component.html
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/docDb.component.ts
--rw-r--r--   0 root         (0) root         (0)     2675 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/docDb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-object-type-table/
--rw-r--r--   0 root         (0) root         (0)     1127 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     3114 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-property-table/
--rw-r--r--   0 root         (0) root         (0)     1999 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2314 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1459 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)      890 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      987 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/view-document/
--rw-r--r--   0 root         (0) root         (0)     1515 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/view-document/view-document.html
--rw-r--r--   0 root         (0) root         (0)     1899 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/view-document/view-document.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.791072 peek-core-docdb-3.4.5/peek_core_docdb/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      556 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     2969 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2625 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py
--rw-r--r--   0 root         (0) root         (0)     8149 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/
--rw-r--r--   0 root         (0) root         (0)       25 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/index.ts
--rw-r--r--   0 root         (0) root         (0)     3488 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.html
--rw-r--r--   0 root         (0) root         (0)      520 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.scss
--rw-r--r--   0 root         (0) root         (0)     6434 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html
--rw-r--r--   0 root         (0) root         (0)     2338 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts
--rw-r--r--   0 root         (0) root         (0)     1056 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts
--rw-r--r--   0 root         (0) root         (0)     1024 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/docdb-popup.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.792072 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12054 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.793072 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/
--rw-r--r--   0 root         (0) root         (0)     5938 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.793072 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)     1193 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/controller/DocumentCacheController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.793072 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.793072 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     3508 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.793072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/
--rw-r--r--   0 root         (0) root         (0)     9607 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2632 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.794072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1612 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1638 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py
--rw-r--r--   0 root         (0) root         (0)      811 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.794072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      660 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/api/DocDbApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.794072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     1823 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.794072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     3991 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/ImportController.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.794072 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      904 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1237 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1031 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)      991 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.795072 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      710 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1822 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbDocument.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py
--rw-r--r--   0 root         (0) root         (0)     2283 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbEncodedChunk.py
--rw-r--r--   0 root         (0) root         (0)      610 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbModelSet.py
--rw-r--r--   0 root         (0) root         (0)     1441 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbPropertyTuple.py
--rw-r--r--   0 root         (0) root         (0)     7642 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.795072 peek-core-docdb-3.4.5/peek_core_docdb/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      454 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.795072 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/
--rw-r--r--   0 root         (0) root         (0)      874 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.795072 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     6536 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)    11202 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/ImportTask.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.795072 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.796072 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    38648 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png
--rw-r--r--   0 root         (0) root         (0)    54690 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png
--rw-r--r--   0 root         (0) root         (0)     2340 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)   104337 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/view_document.png
--rw-r--r--   0 root         (0) root         (0)      341 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     1511 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.796072 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    37793 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      437 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/status/status.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.796072 peek-core-docdb-3.4.5/peek_core_docdb/both-doc/
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/both-doc/offline_support.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.796072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      574 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts
--rw-r--r--   0 root         (0) root         (0)      502 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbModelSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)     4381 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbPopupService.ts
--rw-r--r--   0 root         (0) root         (0)      871 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2851 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbService.ts
--rw-r--r--   0 root         (0) root         (0)      758 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocumentTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.796072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     2663 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/admin/AdminStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      567 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/
--rw-r--r--   0 root         (0) root         (0)      584 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/EncodedDocumentChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    21264 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      247 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/index.ts
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)    11450 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/constants/
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/constants/docdb.constants.ts
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/constants/index.ts
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     3852 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/server/
--rw-r--r--   0 root         (0) root         (0)      915 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/server/DocDbApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.797072 peek-core-docdb-3.4.5/peek_core_docdb/tuples/
--rw-r--r--   0 root         (0) root         (0)      797 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/tuples/DocumentTuple.py
--rw-r--r--   0 root         (0) root         (0)     1070 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/tuples/ImportDocumentTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-28 07:25:23.000000 peek-core-docdb-3.4.5/peek_core_docdb/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:18.790072 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      368 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7736 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/peek_core_docdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:18.798072 peek-core-docdb-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2481 2023-06-28 07:26:18.000000 peek-core-docdb-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.554378 peek-core-docdb-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      217 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.546378 peek-core-docdb-3.4.6/peek_core_docdb/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     3281 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/docDb.component.html
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/docDb.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/docDb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-object-type-table/
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     3114 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-property-table/
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2314 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)      890 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      987 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/view-document/
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/view-document/view-document.html
+-rw-r--r--   0 root         (0) root         (0)     1899 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/view-document/view-document.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.547378 peek-core-docdb-3.4.6/peek_core_docdb/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      556 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py
+-rw-r--r--   0 root         (0) root         (0)     8149 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3488 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.html
+-rw-r--r--   0 root         (0) root         (0)      520 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.scss
+-rw-r--r--   0 root         (0) root         (0)     6434 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1056 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/docdb-popup.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.548378 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12054 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.549378 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.549378 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)     1193 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/controller/DocumentCacheController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.549378 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.549378 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.549378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     9607 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.550378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py
+-rw-r--r--   0 root         (0) root         (0)      811 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.550378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/api/DocDbApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.550378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     1823 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.550378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     3991 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/ImportController.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.550378 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      904 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)      991 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.551378 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      710 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbDocument.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbEncodedChunk.py
+-rw-r--r--   0 root         (0) root         (0)      610 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbModelSet.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbPropertyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.551378 peek-core-docdb-3.4.6/peek_core_docdb/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.551378 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.551378 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     6536 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)    11202 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/ImportTask.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.551378 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.552378 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    38648 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png
+-rw-r--r--   0 root         (0) root         (0)    54690 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png
+-rw-r--r--   0 root         (0) root         (0)     2340 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)   104337 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/view_document.png
+-rw-r--r--   0 root         (0) root         (0)      341 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     1511 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.552378 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    37793 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      437 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/status/status.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.552378 peek-core-docdb-3.4.6/peek_core_docdb/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/both-doc/offline_support.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.552378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      574 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      502 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbModelSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbPopupService.ts
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbService.ts
+-rw-r--r--   0 root         (0) root         (0)      758 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocumentTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     2663 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/admin/AdminStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      567 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/
+-rw-r--r--   0 root         (0) root         (0)      584 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/EncodedDocumentChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    21264 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/index.ts
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)    11450 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/constants/
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/constants/docdb.constants.ts
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/constants/index.ts
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     3852 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/server/
+-rw-r--r--   0 root         (0) root         (0)      915 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/server/DocDbApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.553378 peek-core-docdb-3.4.6/peek_core_docdb/tuples/
+-rw-r--r--   0 root         (0) root         (0)      797 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/tuples/DocumentTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/tuples/ImportDocumentTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 10:19:14.000000 peek-core-docdb-3.4.6/peek_core_docdb/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:08.546378 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      368 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7736 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/peek_core_docdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:08.554378 peek-core-docdb-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2481 2023-06-29 10:20:08.000000 peek-core-docdb-3.4.6/setup.py
```

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/__init__.py` & `peek-core-docdb-3.4.6/peek_core_docdb/__init__.py`

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

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/docDb.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/docDb.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/docDb.module.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/docDb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-object-type-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-property-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/status/status.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/status/status.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/view-document/view-document.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/view-document/view-document.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/admin-app/view-document/view-document.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/admin-app/view-document/view-document.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/agent/AgentEntryHook.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/script.py.mako` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/0b20ccfb7a6a_change_to_biginteger.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/6c94c040e18c_added_showinheader.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/931b88db3117_added_showon_fields.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/a423a783700f_increased_chunk_size.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/alembic/versions/c1d2d5475c64_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.scss` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.scss`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/components/popup/popup.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/components/popup/popup.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/debug-page/debug-page.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-app/docdb-popup.module.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-app/docdb-popup.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/both-assets/icon.png` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/ClientEntryHook.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/TupleDataObservable.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/controller/DocumentCacheController.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/controller/DocumentCacheController.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/handlers/DocumentCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/ClientDocumentTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/client/tuple_providers/ClientDocumentUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/LogicEntryHook.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/TupleActionProcessor.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/TupleDataObservable.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/EditDocumentPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/EditDocumentTypeHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/ViewDocumentHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/admin_backend/__init__.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/api/DocDbApi.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/api/DocDbApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/ClientChunkLoadRpc.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/client_handlers/ClientChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/ChunkCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/controller/MainController.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/DocumentTypeTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/server/tuple_providers/ModelSetTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DeclarativeBase.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbCompilerQueue.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbDocument.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbDocument.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbDocumentTypeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbEncodedChunk.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbEncodedChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbModelSet.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbModelSet.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/DocDbPropertyTuple.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/DocDbPropertyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/storage/Setting.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/tuples/DocumentUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/WorkerEntryHook.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/ChunkCompilerTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/ImportTask.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/ImportTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py` & `peek-core-docdb-3.4.6/peek_core_docdb/_private/worker/tasks/_CalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_document_types.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_task_update_property_name.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/admin_tasks/view_document.png` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/admin_tasks/view_document.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/overview.rst` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/admin-doc/status/status.png` & `peek-core-docdb-3.4.6/peek_core_docdb/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbDocumentTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbPopupService.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbPopupService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocDbService.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocDbService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/DocumentTuple.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/DocumentTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/DocDbTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/DocumentUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/document-loader/PrivateDocumentLoaderService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/_private/services/PrivateDocDbPopupService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin-module/index.ts` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/plugin_package.json` & `peek-core-docdb-3.4.6/peek_core_docdb/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960317460317462%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -109,15 +109,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_docdb",
         "title": "Document DB",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "worker",
         "agent",
         "storage",
```

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/server/DocDbApiABC.py` & `peek-core-docdb-3.4.6/peek_core_docdb/server/DocDbApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/tuples/DocumentTuple.py` & `peek-core-docdb-3.4.6/peek_core_docdb/tuples/DocumentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb/tuples/ImportDocumentTuple.py` & `peek-core-docdb-3.4.6/peek_core_docdb/tuples/ImportDocumentTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/peek_core_docdb.egg-info/SOURCES.txt` & `peek-core-docdb-3.4.6/peek_core_docdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-docdb-3.4.5/setup.py` & `peek-core-docdb-3.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_docdb"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Core Plugin DocDB."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

