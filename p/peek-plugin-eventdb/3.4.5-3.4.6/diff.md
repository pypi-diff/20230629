# Comparing `tmp/peek-plugin-eventdb-3.4.5.tar.gz` & `tmp/peek-plugin-eventdb-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-eventdb-3.4.5.tar", last modified: Wed Jun 28 07:28:07 2023, max compression
+gzip compressed data, was "peek-plugin-eventdb-3.4.6.tar", last modified: Thu Jun 29 10:21:53 2023, max compression
```

## Comparing `peek-plugin-eventdb-3.4.5.tar` & `peek-plugin-eventdb-3.4.6.tar`

### file list

```diff
@@ -1,162 +1,162 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.606108 peek-plugin-eventdb-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      400 2023-06-28 07:28:07.606108 peek-plugin-eventdb-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.599108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/
--rw-r--r--   0 root         (0) root         (0)      913 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)      246 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/PluginNamesTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)      357 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-property-table/
--rw-r--r--   0 root         (0) root         (0)    11203 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     3857 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2476 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1488 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.ts
--rw-r--r--   0 root         (0) root         (0)     1171 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/eventdb.component.html
--rw-r--r--   0 root         (0) root         (0)      212 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/eventdb.component.ts
--rw-r--r--   0 root         (0) root         (0)     3096 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/eventdb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/status/
--rw-r--r--   0 root         (0) root         (0)      869 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/status/status.component.html
--rw-r--r--   0 root         (0) root         (0)      954 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/status/status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/AdminStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      449 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/EventDBModelSetTableTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1317 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyTableTuple.ts
--rw-r--r--   0 root         (0) root         (0)      699 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyValueTableTuple.ts
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/SettingPropertyTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.600108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/agent/
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      325 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/0338181f05cf_add_color.py
--rw-r--r--   0 root         (0) root         (0)     6613 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/4ea424ad3883_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      880 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/a63487e16375_fix_useforpopup.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/af33359d5854_add_useforprop.py
--rw-r--r--   0 root         (0) root         (0)      484 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/e24b71e8ebb5_add_isalarm.py
--rw-r--r--   0 root         (0) root         (0)      133 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-column-component/
--rw-r--r--   0 root         (0) root         (0)     4020 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.ts
--rw-r--r--   0 root         (0) root         (0)      985 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.web.html
--rw-r--r--   0 root         (0) root         (0)      372 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-common.component.web.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/
--rw-r--r--   0 root         (0) root         (0)     9576 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.ts
--rw-r--r--   0 root         (0) root         (0)     3743 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.html
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/
--rw-r--r--   0 root         (0) root         (0)     5025 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.ts
--rw-r--r--   0 root         (0) root         (0)     1310 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.html
--rw-r--r--   0 root         (0) root         (0)      472 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.scss
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-page-component/
--rw-r--r--   0 root         (0) root         (0)     4291 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.ts
--rw-r--r--   0 root         (0) root         (0)     2501 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/eventdb.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.601108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-assets/
--rw-r--r--   0 root         (0) root         (0)     8407 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.602108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-doc/
--rw-r--r--   0 root         (0) root         (0)      146 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.602108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2544 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.602108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/
--rw-r--r--   0 root         (0) root         (0)     1686 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBApi.py
--rw-r--r--   0 root         (0) root         (0)     1371 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBReadApi.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBWriteApi.py
--rw-r--r--   0 root         (0) root         (0)     5867 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      542 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.602108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     2400 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/EventDBPropertyTableHandler.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      399 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/AdminStatusController.py
--rw-r--r--   0 root         (0) root         (0)      218 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBController.py
--rw-r--r--   0 root         (0) root         (0)     5808 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportController.py
--rw-r--r--   0 root         (0) root         (0)     4794 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportEventsInPgTask.py
--rw-r--r--   0 root         (0) root         (0)     4244 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportPropertiesInPgTask.py
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/download_resources/
--rw-r--r--   0 root         (0) root         (0)     4989 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/download_resources/DownloadEventsResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/download_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      932 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     6427 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBEventTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBModelSetTableTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_selector_mappers/
--rw-r--r--   0 root         (0) root         (0)     2108 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_selector_mappers/NewEventTSUpdateMapper.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_selector_mappers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      711 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBEventTable.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBModelSetTable.py
--rw-r--r--   0 root         (0) root         (0)     2181 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBPropertyTable.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBPropertyValueTable.py
--rw-r--r--   0 root         (0) root         (0)     7693 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.603108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      430 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/tuples/AdminStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.604108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    75931 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/edit_properties.png
--rw-r--r--   0 root         (0) root         (0)      188 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      958 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.604108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/
--rwxr-xr-x   0 root         (0) root         (0)     1591 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_button.png
--rw-r--r--   0 root         (0) root         (0)     2067 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_events.rst
--rw-r--r--   0 root         (0) root         (0)   184762 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_events_screen.png
--rw-r--r--   0 root         (0) root         (0)    34157 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/columns.png
--rw-r--r--   0 root         (0) root         (0)    34204 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/download_button.png
--rw-r--r--   0 root         (0) root         (0)    57607 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/events_column.png
--rw-r--r--   0 root         (0) root         (0)    33519 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/filter_button.png
--rw-r--r--   0 root         (0) root         (0)    58897 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/filter_popup.png
--rw-r--r--   0 root         (0) root         (0)      110 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)     4312 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/options_toggle.png
--rw-r--r--   0 root         (0) root         (0)    15794 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/save.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.605108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/
--rw-r--r--   0 root         (0) root         (0)     2125 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/EventDBService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.605108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)     2729 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/EventDBTupleService.ts
--rw-r--r--   0 root         (0) root         (0)      412 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)     5608 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/PrivateEventDBService.ts
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/index.ts
--rw-r--r--   0 root         (0) root         (0)      289 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.605108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)      591 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBEventTuple.ts
--rw-r--r--   0 root         (0) root         (0)      617 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyCriteriaTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3626 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)     1072 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyValueTuple.ts
--rw-r--r--   0 root         (0) root         (0)      346 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/index.ts
--rw-r--r--   0 root         (0) root         (0)     2705 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.605108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/
--rw-r--r--   0 root         (0) root         (0)      754 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBApiABC.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBReadApiABC.py
--rw-r--r--   0 root         (0) root         (0)     2105 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBWriteApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.605108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/
--rw-r--r--   0 root         (0) root         (0)      702 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBEventTuple.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyCriteriaTuple.py
--rw-r--r--   0 root         (0) root         (0)     2553 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyTuple.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyValueTuple.py
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-28 07:25:26.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:28:07.599108 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)      400 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7492 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:28:07.606108 peek-plugin-eventdb-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2496 2023-06-28 07:28:07.000000 peek-plugin-eventdb-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.235580 peek-plugin-eventdb-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-29 10:21:53.235580 peek-plugin-eventdb-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.228580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/
+-rw-r--r--   0 root         (0) root         (0)      913 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)      246 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/PluginNamesTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)      357 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-property-table/
+-rw-r--r--   0 root         (0) root         (0)    11203 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     3857 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2476 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1488 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1171 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/eventdb.component.html
+-rw-r--r--   0 root         (0) root         (0)      212 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/eventdb.component.ts
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/eventdb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/status/
+-rw-r--r--   0 root         (0) root         (0)      869 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/status/status.component.html
+-rw-r--r--   0 root         (0) root         (0)      954 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/status/status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/AdminStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      449 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/EventDBModelSetTableTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1317 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyTableTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      699 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyValueTableTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/SettingPropertyTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/0338181f05cf_add_color.py
+-rw-r--r--   0 root         (0) root         (0)     6613 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/4ea424ad3883_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      880 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/a63487e16375_fix_useforpopup.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/af33359d5854_add_useforprop.py
+-rw-r--r--   0 root         (0) root         (0)      484 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/e24b71e8ebb5_add_isalarm.py
+-rw-r--r--   0 root         (0) root         (0)      133 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.230580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-column-component/
+-rw-r--r--   0 root         (0) root         (0)     4020 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.ts
+-rw-r--r--   0 root         (0) root         (0)      985 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      372 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-common.component.web.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.ts
+-rw-r--r--   0 root         (0) root         (0)     3743 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.html
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/
+-rw-r--r--   0 root         (0) root         (0)     5025 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1310 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      472 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.scss
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-page-component/
+-rw-r--r--   0 root         (0) root         (0)     4291 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2501 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/eventdb.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-assets/
+-rw-r--r--   0 root         (0) root         (0)     8407 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      146 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2544 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.231580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     1686 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBApi.py
+-rw-r--r--   0 root         (0) root         (0)     1371 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBReadApi.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBWriteApi.py
+-rw-r--r--   0 root         (0) root         (0)     5867 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.232580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     2400 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/EventDBPropertyTableHandler.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.232580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/AdminStatusController.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBController.py
+-rw-r--r--   0 root         (0) root         (0)     5808 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportController.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportEventsInPgTask.py
+-rw-r--r--   0 root         (0) root         (0)     4244 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportPropertiesInPgTask.py
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.232580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/download_resources/
+-rw-r--r--   0 root         (0) root         (0)     4989 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/download_resources/DownloadEventsResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/download_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.232580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      932 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/AdminStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     6427 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBEventTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBModelSetTableTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.232580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_selector_mappers/
+-rw-r--r--   0 root         (0) root         (0)     2108 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_selector_mappers/NewEventTSUpdateMapper.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_selector_mappers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.233580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBEventTable.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBModelSetTable.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBPropertyTable.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBPropertyValueTable.py
+-rw-r--r--   0 root         (0) root         (0)     7693 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.233580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      430 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/tuples/AdminStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.233580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    75931 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/edit_properties.png
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      958 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.234580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/
+-rwxr-xr-x   0 root         (0) root         (0)     1591 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_button.png
+-rw-r--r--   0 root         (0) root         (0)     2067 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_events.rst
+-rw-r--r--   0 root         (0) root         (0)   184762 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_events_screen.png
+-rw-r--r--   0 root         (0) root         (0)    34157 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/columns.png
+-rw-r--r--   0 root         (0) root         (0)    34204 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/download_button.png
+-rw-r--r--   0 root         (0) root         (0)    57607 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/events_column.png
+-rw-r--r--   0 root         (0) root         (0)    33519 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/filter_button.png
+-rw-r--r--   0 root         (0) root         (0)    58897 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/filter_popup.png
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/options_toggle.png
+-rw-r--r--   0 root         (0) root         (0)    15794 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/save.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.234580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)     2125 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/EventDBService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.234580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/EventDBTupleService.ts
+-rw-r--r--   0 root         (0) root         (0)      412 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/PrivateEventDBService.ts
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/index.ts
+-rw-r--r--   0 root         (0) root         (0)      289 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.234580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)      591 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBEventTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      617 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyCriteriaTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3626 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyValueTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.235580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBApiABC.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBReadApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBWriteApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.235580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/
+-rw-r--r--   0 root         (0) root         (0)      702 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBEventTuple.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyCriteriaTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyValueTuple.py
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-29 10:19:17.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:53.229580 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      400 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7492 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:21:53.236580 peek-plugin-eventdb-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2496 2023-06-29 10:21:53.000000 peek-plugin-eventdb-3.4.6/setup.py
```

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/__init__.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Type
 
 from peek_plugin_base.agent.PluginAgentEntryHookABC import PluginAgentEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-property-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/eventdb.component.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/eventdb.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/eventdb.module.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/eventdb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/status/status.component.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/status/status.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/status/status.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/status/status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyTableTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyTableTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyValueTableTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/EventDBPropertyValueTableTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/admin-app/tuples/SettingPropertyTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/admin-app/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/agent/AgentEntryHook.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/script.py.mako` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/0338181f05cf_add_color.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/0338181f05cf_add_color.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/4ea424ad3883_initial_tables.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/4ea424ad3883_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/a63487e16375_fix_useforpopup.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/a63487e16375_fix_useforpopup.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/alembic/versions/af33359d5854_add_useforprop.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/alembic/versions/af33359d5854_add_useforprop.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.web.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-column-component/event-column.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-filter-component/event-filter.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-list-component/event-list.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.web.html` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/event-page-component/event-page.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-app/eventdb.module.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-app/eventdb.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/both-assets/icon.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/both-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/client/ClientEntryHook.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBApi.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBReadApi.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBReadApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/EventDBWriteApi.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/EventDBWriteApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/LogicEntryHook.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/TupleActionProcessor.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/TupleDataObservable.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/EventDBPropertyTableHandler.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/EventDBPropertyTableHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportController.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportEventsInPgTask.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportEventsInPgTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/EventDBImportPropertiesInPgTask.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/EventDBImportPropertiesInPgTask.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/controller/MainController.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/download_resources/DownloadEventsResource.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/download_resources/DownloadEventsResource.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/AdminStatusTupleProvider.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/AdminStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBEventTupleProvider.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBEventTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBModelSetTableTupleProvider.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBModelSetTableTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_providers/EventDBPropertyTupleProvider.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_providers/EventDBPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/server/tuple_selector_mappers/NewEventTSUpdateMapper.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/server/tuple_selector_mappers/NewEventTSUpdateMapper.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/DeclarativeBase.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBEventTable.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBEventTable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBModelSetTable.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBModelSetTable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBPropertyTable.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBPropertyTable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/EventDBPropertyValueTable.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/EventDBPropertyValueTable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/_private/storage/Setting.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/admin_tasks.rst` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/edit_properties.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/edit_properties.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/admin-doc/overview.rst` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_button.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_events.rst` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_events.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/alarms_events_screen.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/alarms_events_screen.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/columns.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/columns.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/download_button.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/download_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/events_column.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/events_column.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/filter_button.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/filter_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/filter_popup.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/filter_popup.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/options_toggle.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/options_toggle.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/both-doc/save.png` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/both-doc/save.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/EventDBService.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/EventDBService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/EventDBTupleService.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/EventDBTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/_private/PrivateEventDBService.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/_private/PrivateEventDBService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBEventTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBEventTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyCriteriaTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyCriteriaTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyValueTuple.ts` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin-module/tuples/EventDBPropertyValueTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/plugin_package.json` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/plugin_package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967532467532468%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -71,15 +71,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_eventdb",
         "title": "Event DB",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "admin",
         "agent",
```

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBApiABC.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBReadApiABC.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBReadApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/server/EventDBWriteApiABC.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/server/EventDBWriteApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBEventTuple.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBEventTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyCriteriaTuple.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyCriteriaTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyTuple.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb/tuples/EventDBPropertyValueTuple.py` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb/tuples/EventDBPropertyValueTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/peek_plugin_eventdb.egg-info/SOURCES.txt` & `peek-plugin-eventdb-3.4.6/peek_plugin_eventdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-eventdb-3.4.5/setup.py` & `peek-plugin-eventdb-3.4.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_eventdb"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin EventDB - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

