# Comparing `tmp/peek-core-search-3.4.5.tar.gz` & `tmp/peek-core-search-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-search-3.4.5.tar", last modified: Wed Jun 28 07:26:27 2023, max compression
+gzip compressed data, was "peek-core-search-3.4.6.tar", last modified: Thu Jun 29 10:20:17 2023, max compression
```

## Comparing `peek-core-search-3.4.5.tar` & `peek-core-search-3.4.6.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.973075 peek-core-search-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      216 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.963075 peek-core-search-3.4.5/peek_core_search/
--rw-r--r--   0 root         (0) root         (0)      555 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.963075 peek-core-search-3.4.5/peek_core_search/_private/
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.963075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.963075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-exclude-search-term-table/
--rw-r--r--   0 root         (0) root         (0)     2214 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     2248 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-object-type-table/
--rw-r--r--   0 root         (0) root         (0)     1259 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1503 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-property-table/
--rw-r--r--   0 root         (0) root         (0)     1572 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-property-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1458 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1462 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/search-component/
--rw-r--r--   0 root         (0) root         (0)     3816 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/search-component/search.component.html
--rw-r--r--   0 root         (0) root         (0)      164 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/search-component/search.component.ts
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/search.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/status-component/
--rw-r--r--   0 root         (0) root         (0)     1405 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/status-component/status.component.html
--rw-r--r--   0 root         (0) root         (0)      989 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/status-component/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      426 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/admin-app/tuples/ExcludeSearchStringTable.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.964075 peek-core-search-3.4.5/peek_core_search/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      319 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.965075 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3066 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py
--rw-r--r--   0 root         (0) root         (0)    10042 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py
--rw-r--r--   0 root         (0) root         (0)      819 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py
--rw-r--r--   0 root         (0) root         (0)      794 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py
--rw-r--r--   0 root         (0) root         (0)     1023 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3215 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py
--rw-r--r--   0 root         (0) root         (0)      756 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.965075 peek-core-search-3.4.5/peek_core_search/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.965075 peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/
--rw-r--r--   0 root         (0) root         (0)     2950 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.html
--rw-r--r--   0 root         (0) root         (0)      633 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.scss
--rw-r--r--   0 root         (0) root         (0)     8974 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.965075 peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/
--rw-r--r--   0 root         (0) root         (0)     1261 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/result.component.html
--rw-r--r--   0 root         (0) root         (0)      214 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/result.component.scss
--rw-r--r--   0 root         (0) root         (0)     3496 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/result.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.965075 peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/search.component.html
--rw-r--r--   0 root         (0) root         (0)      278 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/search.component.scss
--rw-r--r--   0 root         (0) root         (0)     1049 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/search.component.ts
--rw-r--r--   0 root         (0) root         (0)     1464 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-app/search.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.966075 peek-core-search-3.4.5/peek_core_search/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)    12730 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.966075 peek-core-search-3.4.5/peek_core_search/_private/client/
--rw-r--r--   0 root         (0) root         (0)     7303 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.966075 peek-core-search-3.4.5/peek_core_search/_private/client/controller/
--rw-r--r--   0 root         (0) root         (0)    15042 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/controller/FastKeywordController.py
--rw-r--r--   0 root         (0) root         (0)     3405 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/controller/FastKeywordControllerTest.py
--rw-r--r--   0 root         (0) root         (0)     1953 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/controller/SearchIndexCacheController.py
--rw-r--r--   0 root         (0) root         (0)     4720 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/controller/SearchObjectCacheController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.966075 peek-core-search-3.4.5/peek_core_search/_private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)     1115 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.966075 peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1019 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.967075 peek-core-search-3.4.5/peek_core_search/_private/server/
--rw-r--r--   0 root         (0) root         (0)    12183 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      532 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2435 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.967075 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1640 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)     1837 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      741 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.967075 peek-core-search-3.4.5/peek_core_search/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      774 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/api/SearchApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.967075 peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     3124 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.967075 peek-core-search-3.4.5/peek_core_search/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      821 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     4435 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)     4135 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchObjectImportController.py
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/StatusController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.968075 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      914 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1594 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1166 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1118 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.968075 peek-core-search-3.4.5/peek_core_search/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      711 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     2081 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/EncodedSearchIndexChunk.py
--rw-r--r--   0 root         (0) root         (0)     1947 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/EncodedSearchObjectChunk.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/ExcludeSearchStringTable.py
--rw-r--r--   0 root         (0) root         (0)     1169 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchIndex.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchIndexCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1207 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObject.py
--rw-r--r--   0 root         (0) root         (0)      971 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectCompilerQueue.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectRoute.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectTypeTuple.py
--rw-r--r--   0 root         (0) root         (0)      945 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/SearchPropertyTuple.py
--rw-r--r--   0 root         (0) root         (0)     7759 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.969075 peek-core-search-3.4.5/peek_core_search/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      711 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      414 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/ExcludeSearchStringsTuple.py
--rw-r--r--   0 root         (0) root         (0)      694 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      471 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/SearchResultDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      563 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/SearchResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.969075 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_index/
--rw-r--r--   0 root         (0) root         (0)     1273 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.969075 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/
--rw-r--r--   0 root         (0) root         (0)     1276 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py
--rw-r--r--   0 root         (0) root         (0)      539 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.969075 peek-core-search-3.4.5/peek_core_search/_private/worker/
--rw-r--r--   0 root         (0) root         (0)     1059 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/WorkerEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.970075 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     5006 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py
--rw-r--r--   0 root         (0) root         (0)    20585 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py
--rw-r--r--   0 root         (0) root         (0)     3088 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/KeywordSplitter.py
--rw-r--r--   0 root         (0) root         (0)     4748 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py
--rw-r--r--   0 root         (0) root         (0)     7063 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)     6236 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py
--rw-r--r--   0 root         (0) root         (0)      851 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/_CalcChunkKey.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.970075 peek-core-search-3.4.5/peek_core_search/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.970075 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    69265 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png
--rw-r--r--   0 root         (0) root         (0)    65374 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    59417 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/exclude_keyword.png
--rw-r--r--   0 root         (0) root         (0)    49895 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/general_settings.png
--rw-r--r--   0 root         (0) root         (0)    45973 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/remove_exclude.png
--rw-r--r--   0 root         (0) root         (0)   167257 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/search_object_order.png
--rw-r--r--   0 root         (0) root         (0)      528 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.970075 peek-core-search-3.4.5/peek_core_search/admin-doc/status/
--rw-r--r--   0 root         (0) root         (0)    37092 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/status/status.png
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/admin-doc/status/status.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.971075 peek-core-search-3.4.5/peek_core_search/both-doc/
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      966 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/both-doc/search_button.png
--rw-r--r--   0 root         (0) root         (0)    31589 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/both-doc/search_filtered.png
--rw-r--r--   0 root         (0) root         (0)    28759 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/both-doc/search_popup.png
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/both-doc/searching.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.971075 peek-core-search-3.4.5/peek_core_search/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      559 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/SearchObjectTypeTuple.ts
--rw-r--r--   0 root         (0) root         (0)      988 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts
--rw-r--r--   0 root         (0) root         (0)      981 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/SearchResultObjectTuple.ts
--rw-r--r--   0 root         (0) root         (0)     7550 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/SearchService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.971075 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     3291 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/KeywordSplitter.ts
--rw-r--r--   0 root         (0) root         (0)      534 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)     2697 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/SearchTupleService.ts
--rw-r--r--   0 root         (0) root         (0)    11554 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/fast-keyword-controller.ts
--rw-r--r--   0 root         (0) root         (0)      381 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/
--rw-r--r--   0 root         (0) root         (0)      437 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/EncodedSearchIndexChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    17206 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      595 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/
--rw-r--r--   0 root         (0) root         (0)      440 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/EncodedSearchObjectChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    19221 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      598 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      448 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/ExcludeSearchStringsTuple.ts
--rw-r--r--   0 root         (0) root         (0)      652 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/admin/
--rw-r--r--   0 root         (0) root         (0)      702 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      572 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      310 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     2989 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/server/
--rw-r--r--   0 root         (0) root         (0)     1235 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/server/SearchApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.972075 peek-core-search-3.4.5/peek_core_search/tuples/
--rw-r--r--   0 root         (0) root         (0)      695 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/tuples/ImportSearchObjectRouteTuple.py
--rw-r--r--   0 root         (0) root         (0)     1851 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/tuples/ImportSearchObjectTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-28 07:25:23.000000 peek-core-search-3.4.5/peek_core_search/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:27.963075 peek-core-search-3.4.5/peek_core_search.egg-info/
--rw-r--r--   0 root         (0) root         (0)      390 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11138 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/peek_core_search.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:27.973075 peek-core-search-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2727 2023-06-28 07:26:27.000000 peek-core-search-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.027394 peek-core-search-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search/_private/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-exclude-search-term-table/
+-rw-r--r--   0 root         (0) root         (0)     2214 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-object-type-table/
+-rw-r--r--   0 root         (0) root         (0)     1259 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1503 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-property-table/
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-property-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/search-component/
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/search-component/search.component.html
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/search-component/search.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/search.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/status-component/
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/status-component/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      989 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/status-component/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/admin-app/tuples/ExcludeSearchStringTable.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.018394 peek-core-search-3.4.6/peek_core_search/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      319 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3066 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py
+-rw-r--r--   0 root         (0) root         (0)    10042 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py
+-rw-r--r--   0 root         (0) root         (0)      794 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py
+-rw-r--r--   0 root         (0) root         (0)      756 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.html
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.scss
+-rw-r--r--   0 root         (0) root         (0)     8974 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/
+-rw-r--r--   0 root         (0) root         (0)     1261 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/result.component.html
+-rw-r--r--   0 root         (0) root         (0)      214 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/result.component.scss
+-rw-r--r--   0 root         (0) root         (0)     3496 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/result.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/
+-rw-r--r--   0 root         (0) root         (0)      550 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/search.component.html
+-rw-r--r--   0 root         (0) root         (0)      278 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/search.component.scss
+-rw-r--r--   0 root         (0) root         (0)     1049 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/search.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1464 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-app/search.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.019394 peek-core-search-3.4.6/peek_core_search/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)    12730 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.020394 peek-core-search-3.4.6/peek_core_search/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     7303 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.020394 peek-core-search-3.4.6/peek_core_search/_private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)    16350 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/controller/FastKeywordController.py
+-rw-r--r--   0 root         (0) root         (0)     3405 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/controller/FastKeywordControllerTest.py
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/controller/SearchIndexCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     4736 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/controller/SearchObjectCacheController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.020394 peek-core-search-3.4.6/peek_core_search/_private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.020394 peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.020394 peek-core-search-3.4.6/peek_core_search/_private/server/
+-rw-r--r--   0 root         (0) root         (0)    12183 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2435 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.021394 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      741 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.021394 peek-core-search-3.4.6/peek_core_search/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      774 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/api/SearchApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.021394 peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     3124 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.021394 peek-core-search-3.4.6/peek_core_search/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      821 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     4435 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchObjectImportController.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/StatusController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.022394 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1594 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1166 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.022394 peek-core-search-3.4.6/peek_core_search/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/EncodedSearchIndexChunk.py
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/EncodedSearchObjectChunk.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/ExcludeSearchStringTable.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchIndex.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchIndexCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObject.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectCompilerQueue.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectRoute.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectTypeTuple.py
+-rw-r--r--   0 root         (0) root         (0)      945 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/SearchPropertyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7759 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.023394 peek-core-search-3.4.6/peek_core_search/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/ExcludeSearchStringsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      694 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/SearchResultDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      563 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/SearchResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.023394 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_index/
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.023394 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/
+-rw-r--r--   0 root         (0) root         (0)     1276 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py
+-rw-r--r--   0 root         (0) root         (0)      539 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.023394 peek-core-search-3.4.6/peek_core_search/_private/worker/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/WorkerEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.024394 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     5006 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py
+-rw-r--r--   0 root         (0) root         (0)    20585 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/KeywordSplitter.py
+-rw-r--r--   0 root         (0) root         (0)     4748 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py
+-rw-r--r--   0 root         (0) root         (0)     7063 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)     6236 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py
+-rw-r--r--   0 root         (0) root         (0)      851 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/_CalcChunkKey.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.024394 peek-core-search-3.4.6/peek_core_search/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.024394 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    69265 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png
+-rw-r--r--   0 root         (0) root         (0)    65374 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    59417 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/exclude_keyword.png
+-rw-r--r--   0 root         (0) root         (0)    49895 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/general_settings.png
+-rw-r--r--   0 root         (0) root         (0)    45973 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/remove_exclude.png
+-rw-r--r--   0 root         (0) root         (0)   167257 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/search_object_order.png
+-rw-r--r--   0 root         (0) root         (0)      528 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.024394 peek-core-search-3.4.6/peek_core_search/admin-doc/status/
+-rw-r--r--   0 root         (0) root         (0)    37092 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/status/status.png
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/admin-doc/status/status.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.025394 peek-core-search-3.4.6/peek_core_search/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      966 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/both-doc/search_button.png
+-rw-r--r--   0 root         (0) root         (0)    31589 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/both-doc/search_filtered.png
+-rw-r--r--   0 root         (0) root         (0)    28759 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/both-doc/search_popup.png
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/both-doc/searching.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.025394 peek-core-search-3.4.6/peek_core_search/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/SearchObjectTypeTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      988 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      981 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/SearchResultObjectTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     7550 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/SearchService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.025394 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/KeywordSplitter.ts
+-rw-r--r--   0 root         (0) root         (0)      534 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/SearchTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)    12494 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/fast-keyword-controller.ts
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/EncodedSearchIndexChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    17206 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      595 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/
+-rw-r--r--   0 root         (0) root         (0)      440 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/EncodedSearchObjectChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    19550 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      598 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/ExcludeSearchStringsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      652 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/admin/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      310 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/server/
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/server/SearchApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.026394 peek-core-search-3.4.6/peek_core_search/tuples/
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/tuples/ImportSearchObjectRouteTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/tuples/ImportSearchObjectTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 10:19:14.000000 peek-core-search-3.4.6/peek_core_search/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:17.017394 peek-core-search-3.4.6/peek_core_search.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11138 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/peek_core_search.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:17.027394 peek-core-search-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-06-29 10:20:16.000000 peek-core-search-3.4.6/setup.py
```

### Comparing `peek-core-search-3.4.5/peek_core_search/PlatformDependencyTest.py` & `peek-core-search-3.4.6/peek_core_search/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/__init__.py` & `peek-core-search-3.4.6/peek_core_search/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.worker.PluginWorkerEntryHookABC import PluginWorkerEntryHookABC
 from typing import Type
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-exclude-search-term-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-object-type-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-property-table/edit.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-property-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-property-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/search-component/search.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/search-component/search.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/search.module.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/search.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/status-component/status.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/status-component/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/admin-app/status-component/status.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/admin-app/status-component/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/agent/AgentEntryHook.py` & `peek-core-search-3.4.6/peek_core_search/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/script.py.mako` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/0736e757d1ec_change_to_biginteger.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/2c6cad1f280e_added_si_objectid_index.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/30f0d0f925ca_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/36aeb6eaea5c_added_show_to_prop.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/3dba609610b6_fix_exclude_comment.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/5e2b9afbb499_added_object_order.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/62059f03f89f_change_chunkkey_to_str.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/758f26706069_add_partial_kw.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/79609b0e25a5_add_full_exclude_terms.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/c18d0a2ab678_increased_chunk_size.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py` & `peek-core-search-3.4.6/peek_core_search/_private/alembic/versions/e51cdf9b7d4c_add_exclude_terms.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.scss` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.scss`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/find-component/find.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/find-component/find.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/result.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/result.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/result-component/result.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/result-component/result.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/search.component.html` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/search.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/search-component/search.component.ts` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/search-component/search.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-app/search.module.ts` & `peek-core-search-3.4.6/peek_core_search/_private/both-app/search.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/both-assets/icon.png` & `peek-core-search-3.4.6/peek_core_search/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/ClientEntryHook.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/TupleDataObservable.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/controller/FastKeywordController.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/controller/FastKeywordController.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 This module stores a memory resident model of a graph network.
 
 """
 import logging
 from collections import defaultdict
 from datetime import datetime
+from functools import cmp_to_key
 from typing import Optional, List, Dict, Iterable, Set
 
 import pytz
 import json
 from twisted.internet.defer import inlineCallbacks, Deferred
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
@@ -23,14 +24,17 @@
 )
 from peek_core_search._private.client.controller.SearchObjectCacheController import (
     SearchObjectCacheController,
 )
 from peek_core_search._private.storage.EncodedSearchIndexChunk import (
     EncodedSearchIndexChunk,
 )
+from peek_core_search._private.storage.SearchObjectTypeTuple import (
+    SearchObjectTypeTuple,
+)
 from peek_core_search._private.tuples.ExcludeSearchStringsTuple import (
     ExcludeSearchStringsTuple,
 )
 from peek_core_search._private.tuples.KeywordAutoCompleteTupleAction import (
     KeywordAutoCompleteTupleAction,
 )
 from peek_core_search._private.tuples.search_object.SearchResultObjectTuple import (
@@ -73,14 +77,16 @@
         self.excludedPartialSearchTerms: list[str] = []
         self.excludedFullSearchTerms: set[str] = set()
 
         excludeStringsTs = TupleSelector(
             ExcludeSearchStringsTuple.tupleName(), {}
         )
 
+        # excludeCallback
+
         def excludeCallback(tuples):
             if tuples:
                 self.excludedPartialSearchTerms = (
                     prepareExcludedPartialTermsForFind(
                         tuples[0].excludedPartialSearchTerms
                     )
                 )
@@ -91,14 +97,34 @@
 
         self._excludedSubscription = (
             serverTupleObserver.subscribeToTupleSelector(
                 excludeStringsTs
             ).subscribe(excludeCallback)
         )
 
+        # _objectTypeSubscription
+
+        self._objectTypeOrdersById: Dict[int, int] = {}
+
+        def objectTypeCallback(tuples: list[SearchObjectTypeTuple]):
+            if not tuples:
+                return
+
+            self._objectTypeOrdersById = {}
+            for objectType in tuples:
+                self._objectTypeOrdersById[objectType.id] = objectType.order
+
+        objectTypeTs = TupleSelector(SearchObjectTypeTuple.tupleName(), {})
+
+        self._objectTypeSubscription = (
+            serverTupleObserver.subscribeToTupleSelector(
+                objectTypeTs
+            ).subscribe(objectTypeCallback)
+        )
+
     def shutdown(self):
         self._objectCacheController = None
         self._indexCacheController = None
         self._objectIdsByKeywordByPropertyKeyByChunkKey = {}
         self.excludedPartialSearchTerms = []
         self.excludedFullSearchTerms = set()
 
@@ -194,18 +220,37 @@
 
             result.rank = 0
             for p in allPropVals.split():
                 for w in splitWords:
                     if p.startswith(w):
                         result.rank += len(p) - len(w)
 
+            # 10,000 should be a good differentiator
+            # Order by the results by object type order
+            result.rank *= (
+                self._objectTypeOrdersById.get(result.objectType.id, 0) * 10000
+            )
+
             return True
 
+        def sortComp(a, b):
+            if a.rank != b.rank:
+                return a.rank - b.rank
+
+            if a.key < b.key:
+                return -1
+            elif a.key > b.key:
+                return 1
+            else:
+                return 0
+
         # Filter and set the rank
-        return list(sorted(filter(rankResult, results), key=lambda r: r.rank))
+        return list(
+            sorted(filter(rankResult, results), key=cmp_to_key(sortComp))
+        )
 
     @deferToThreadWrapWithLogger(logger)
     def _getObjectIdsForSearchString(
         self, searchString: str, propertyName: Optional[str]
     ) -> Deferred:
         """Get ObjectIds For Search String
```

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/controller/FastKeywordControllerTest.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/controller/FastKeywordControllerTest.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/controller/SearchIndexCacheController.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/controller/SearchIndexCacheController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/controller/SearchObjectCacheController.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/controller/SearchObjectCacheController.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import json
 import logging
 from collections import defaultdict
-from typing import List, Optional
+from typing import List
+from typing import Optional
 
-import json
 from vortex.DeferUtil import deferToThreadWrapWithLogger
 from vortex.Payload import Payload
 
 from peek_abstract_chunked_index.private.client.controller.ACICacheControllerABC import (
     ACICacheControllerABC,
 )
 from peek_core_search._private.PluginNames import searchFilt
@@ -60,15 +61,14 @@
         self, objectTypeId: Optional[int], objectIds: List[int]
     ) -> List[SearchResultObjectTuple]:
         return self.getObjectsBlocking(objectTypeId, objectIds)
 
     def getObjectsBlocking(
         self, objectTypeId: Optional[int], objectIds: List[int]
     ) -> List[SearchResultObjectTuple]:
-
         objectIdsByChunkKey = defaultdict(list)
         for objectId in objectIds:
             objectIdsByChunkKey[makeSearchObjectChunkKey(objectId)].append(
                 objectId
             )
 
         foundObjects: List[SearchResultObjectTuple] = []
@@ -78,15 +78,14 @@
             )
 
         return foundObjects
 
     def _getObjectsForChunkBlocking(
         self, chunkKey: str, objectTypeId: Optional[int], objectIds: List[int]
     ) -> List[SearchResultObjectTuple]:
-
         chunk = self.encodedChunk(chunkKey)
         if not chunk:
             return []
 
         objectPropsByIdStr = (
             Payload().fromEncodedPayload(chunk.encodedData).tuples[0]
         )
```

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/handlers/SearchIndexCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/handlers/SearchObjectCacheHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/ClientSearchIndexUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/client/tuple_providers/ClientSearchObjectUpdateDateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/LogicEntryHook.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/TupleActionProcessor.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/TupleDataObservable.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/EditSearchObjectTypeHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/EditSearchPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/ExcludeSearchStringTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/admin_backend/__init__.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/admin_backend/__init__.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/api/SearchApi.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/api/SearchApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientChunkLoadRpc.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientSearchIndexChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/client_handlers/ClientSearchObjectChunkUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/controller/MainController.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchIndexChunkCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchObjectChunkCompilerQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/controller/SearchObjectImportController.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/controller/SearchObjectImportController.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/ExcludeSearchStringsTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/SearchObjectTypeTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py` & `peek-core-search-3.4.6/peek_core_search/_private/server/tuple_providers/SearchPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/DeclarativeBase.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/EncodedSearchIndexChunk.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/EncodedSearchIndexChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/EncodedSearchObjectChunk.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/EncodedSearchObjectChunk.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/ExcludeSearchStringTable.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/ExcludeSearchStringTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchIndex.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchIndex.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchIndexCompilerQueue.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchIndexCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObject.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObject.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectCompilerQueue.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectCompilerQueue.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectRoute.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectRoute.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchObjectTypeTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchObjectTypeTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/SearchPropertyTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/SearchPropertyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/storage/Setting.py` & `peek-core-search-3.4.6/peek_core_search/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/AdminStatusTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/AdminStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/KeywordAutoCompleteTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/SearchResultOpenHandlerTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/SearchResultTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/SearchResultTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/search_index/SearchIndexUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchObjectUpdateDateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchResultObjectRouteTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py` & `peek-core-search-3.4.6/peek_core_search/_private/tuples/search_object/SearchResultObjectTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/WorkerEntryHook.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/WorkerEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/ImportSearchIndexTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/ImportSearchObjectTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/KeywordSplitter.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/KeywordSplitter.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/KeywordSplitterTest.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/SearchIndexChunkCompilerTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/SearchObjectChunkCompilerTask.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/_private/worker/tasks/_CalcChunkKey.py` & `peek-core-search-3.4.6/peek_core_search/_private/worker/tasks/_CalcChunkKey.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_properties.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_task_update_object_type_name.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/exclude_keyword.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/exclude_keyword.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/general_settings.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/general_settings.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/remove_exclude.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/remove_exclude.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/admin_tasks/search_object_order.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/admin_tasks/search_object_order.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/index.rst` & `peek-core-search-3.4.6/peek_core_search/admin-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/overview.rst` & `peek-core-search-3.4.6/peek_core_search/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/status/status.png` & `peek-core-search-3.4.6/peek_core_search/admin-doc/status/status.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/admin-doc/status/status.rst` & `peek-core-search-3.4.6/peek_core_search/admin-doc/status/status.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/both-doc/search_button.png` & `peek-core-search-3.4.6/peek_core_search/both-doc/search_button.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/both-doc/search_filtered.png` & `peek-core-search-3.4.6/peek_core_search/both-doc/search_filtered.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/both-doc/search_popup.png` & `peek-core-search-3.4.6/peek_core_search/both-doc/search_popup.png`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/both-doc/searching.rst` & `peek-core-search-3.4.6/peek_core_search/both-doc/searching.rst`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/SearchObjectTypeTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/SearchObjectTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/SearchResultObjectRouteTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/SearchResultObjectTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/SearchResultObjectTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/SearchService.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/SearchService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/KeywordSplitter.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/KeywordSplitter.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/PluginNames.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/PluginNames.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/SearchTupleService.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/SearchTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/fast-keyword-controller.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/fast-keyword-controller.ts`

 * *Files 12% similar despite different names*

```diff
@@ -9,41 +9,56 @@
 import { PrivateSearchIndexLoaderService } from "./search-index-loader";
 import { PrivateSearchObjectLoaderService } from "./search-object-loader";
 import { SearchResultObjectTuple } from "../SearchResultObjectTuple";
 import { SearchTupleService } from "./SearchTupleService";
 import { NgLifeCycleEvents, TupleSelector } from "@synerty/vortexjs";
 import { ExcludeSearchStringsTuple } from "./tuples/ExcludeSearchStringsTuple";
 import { filter, takeUntil } from "rxjs/operators";
+import { SearchObjectTypeTuple } from "@peek/peek_core_search";
 
 export class FastKeywordController {
     private excludedPartialSearchTerms: string[] = [];
     private excludedFullSearchTerms: Set<string> = new Set<string>();
+
+    private objectTypeOrdersById = {};
+
     constructor(
         private searchIndexLoader: PrivateSearchIndexLoaderService,
         private searchObjectLoader: PrivateSearchObjectLoaderService,
         tupleService: SearchTupleService,
         ngLifeCycleEvents: NgLifeCycleEvents
     ) {
-        const excludeStringsTs = new TupleSelector(
-            ExcludeSearchStringsTuple.tupleName,
-            {}
-        );
         tupleService.offlineObserver
-            .subscribeToTupleSelector(excludeStringsTs)
+            .subscribeToTupleSelector(
+                new TupleSelector(ExcludeSearchStringsTuple.tupleName, {})
+            )
             .pipe(takeUntil(ngLifeCycleEvents.onDestroyEvent))
             .pipe(filter((t) => t.length !== 0))
             .subscribe((tuples: any[]) => {
                 this.excludedPartialSearchTerms =
                     prepareExcludedPartialTermsForFind(
                         tuples[0].excludedPartialSearchTerms
                     );
                 this.excludedFullSearchTerms = new Set<string>(
                     tuples[0].excludedFullSearchTerms
                 );
             });
+
+        tupleService.offlineObserver
+            .subscribeToTupleSelector(
+                new TupleSelector(SearchObjectTypeTuple.tupleName, {})
+            )
+            .pipe(takeUntil(ngLifeCycleEvents.onDestroyEvent))
+            .pipe(filter((t) => t.length !== 0))
+            .subscribe((tuples: any[]) => {
+                this.objectTypeOrdersById = {};
+                for (let tuple of tuples) {
+                    this.objectTypeOrdersById[tuple.id] = tuple.order;
+                }
+            });
     }
 
     haveEnoughSearchKeywords(keywordsString: string): boolean {
         keywordsString = filterExcludedFullTerms(
             this.excludedFullSearchTerms,
             keywordsString
         );
@@ -191,19 +206,19 @@
         const objectIdsList = this._setIntersectFilterIndexResults(resultsByKw);
 
         // Limit to 50 and return
         return objectIdsList;
     }
 
     /** Rank and Filter Objects For Search String
-     
+
      STAGE 2 of the search.
-     
+
      This method filters the loaded objects to ensure we have full matches.
-     
+
      :param results:
      :param searchString:
      :param propertyName:
      :return:
      */
     private filterAndRankObjectsForSearchString(
         results: SearchResultObjectTuple[],
@@ -234,21 +249,34 @@
             result.rank = 0;
             for (const p of allPropVals.split(" ")) {
                 for (const w of splitWords) {
                     if (p.indexOf(w) === 0) result.rank += p.length - w.length;
                 }
             }
 
+            // 10,000 should be a good differentiator
+            // Order by the results by object type order
+            result.rank *=
+                (this.objectTypeOrdersById[result.objectType.id] || 0) * 10000;
+
             return true;
         };
 
+        const sortComp = (a, b) => {
+            if (a.rank !== b.rank) {
+                return a.rank - b.rank;
+            }
+
+            return a.key.localeCompare(b.key);
+        };
+
         // Filter and set the rank
         return results //
             .filter(rankResult)
-            .sort((a, b) => a.rank - b.rank);
+            .sort(sortComp);
     }
 
     /** Merge Partial
      */
     private _mergePartialAndFullMatches(
         searchString: string,
         resultsByFullKw: { [key: string]: number[] },
```

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/PrivateSearchIndexLoaderService.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-index-loader/SearchIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/PrivateSearchObjectLoaderService.ts`

 * *Files 2% similar despite different names*

```diff
@@ -71,24 +71,24 @@
 // ----------------------------------------------------------------------------
 /** hash method
  */
 let OBJECT_BUCKET_COUNT = 8192;
 
 function objectIdChunk(objectId: number): string {
     /** Object ID Chunk
-     
+
      This method creates an int from 0 to MAX, representing the hash bucket for this
      object Id.
-     
+
      This is simple, and provides a reasonable distribution
-     
+
      @param objectId: The ID if the object to get the chunk key for
-     
+
      @return: The bucket / chunkKey where you'll find the object with this ID
-     
+
      */
     if (objectId == null) throw new Error("objectId None or zero length");
 
     return (objectId & (OBJECT_BUCKET_COUNT - 1)).toString();
 }
 
 // ----------------------------------------------------------------------------
@@ -476,28 +476,34 @@
         for (let chunkKey of chunkKeys) {
             let objectIds = objectIdsByChunkKey[chunkKey];
             promises.push(
                 this.getObjectsForObjectIds(objectTypeId, objectIds, chunkKey)
             );
         }
 
+        const objectIdsAdded = new Set<number>();
         return Promise.all(promises).then(
-            (results: SearchResultObjectTuple[][]) => {
-                let objects: SearchResultObjectTuple[] = [];
-                for (let result of results) {
-                    objects.add(result);
+            (listOfObjectLists: SearchResultObjectTuple[][]) => {
+                let objectsToReturn: SearchResultObjectTuple[] = [];
+                for (let listOfObjects of listOfObjectLists) {
+                    for (let objectTuple of listOfObjects) {
+                        if (!objectIdsAdded.has(objectTuple.id)) {
+                            objectIdsAdded.add(objectTuple.id);
+                            objectsToReturn.push(objectTuple);
+                        }
+                    }
                 }
-                return objects;
+                return objectsToReturn;
             }
         );
     }
 
     /** Get Objects for Object ID
      *
-     * Get the objects with matching keywords from the index..
+     * Get the objects with matching keywords from the index.
      *
      */
     private getObjectsForObjectIds(
         objectTypeId: number | null,
         objectIds: number[],
         chunkKey: string
     ): Promise<SearchResultObjectTuple[]> {
```

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/search-object-loader/SearchObjectUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/KeywordAutoCompleteTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/SearchPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/admin/AdminStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts` & `peek-core-search-3.4.6/peek_core_search/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/plugin_package.json` & `peek-core-search-3.4.6/peek_core_search/plugin_package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -76,15 +76,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_search",
         "title": "Search",
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

### Comparing `peek-core-search-3.4.5/peek_core_search/server/SearchApiABC.py` & `peek-core-search-3.4.6/peek_core_search/server/SearchApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/tuples/ImportSearchObjectRouteTuple.py` & `peek-core-search-3.4.6/peek_core_search/tuples/ImportSearchObjectRouteTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search/tuples/ImportSearchObjectTuple.py` & `peek-core-search-3.4.6/peek_core_search/tuples/ImportSearchObjectTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/peek_core_search.egg-info/SOURCES.txt` & `peek-core-search-3.4.6/peek_core_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-search-3.4.5/setup.py` & `peek-core-search-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_search"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin Search - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

