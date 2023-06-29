# Comparing `tmp/peek-plugin-diagram-trace-3.4.5.tar.gz` & `tmp/peek-plugin-diagram-trace-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-diagram-trace-3.4.5.tar", last modified: Wed Jun 28 07:27:55 2023, max compression
+gzip compressed data, was "peek-plugin-diagram-trace-3.4.6.tar", last modified: Thu Jun 29 10:21:41 2023, max compression
```

## Comparing `peek-plugin-diagram-trace-3.4.5.tar` & `peek-plugin-diagram-trace-3.4.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.208104 peek-plugin-diagram-trace-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/
--rw-r--r--   0 root         (0) root         (0)      679 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/
--rw-r--r--   0 root         (0) root         (0)      299 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)     1099 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.ts
--rw-r--r--   0 root         (0) root         (0)      772 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1490 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      337 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1952 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2043 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/
--rw-r--r--   0 root         (0) root         (0)     3065 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     1871 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      318 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)      720 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      716 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     7799 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.206103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)      606 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    45670 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/
--rw-r--r--   0 root         (0) root         (0)     8724 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/clear_trace_button.png
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)    10636 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/trace_button.png
--rw-r--r--   0 root         (0) root         (0)    16807 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/trace_popup.png
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/tracing.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      370 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/DiagramTraceService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/services/
--rw-r--r--   0 root         (0) root         (0)    11217 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts
--rw-r--r--   0 root         (0) root         (0)     2016 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.207104 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-28 07:25:25.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)     2101 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:55.205103 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3285 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:27:55.208104 peek-plugin-diagram-trace-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2507 2023-06-28 07:27:55.000000 peek-plugin-diagram-trace-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.634558 peek-plugin-diagram-trace-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.631558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/
+-rw-r--r--   0 root         (0) root         (0)      679 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.631558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/
+-rw-r--r--   0 root         (0) root         (0)      299 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.631558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.ts
+-rw-r--r--   0 root         (0) root         (0)      772 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.631558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1490 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      337 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1952 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2043 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     3065 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.632558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      716 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     7799 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)      606 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    45670 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png
+-rw-r--r--   0 root         (0) root         (0)      226 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/
+-rw-r--r--   0 root         (0) root         (0)     8724 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/clear_trace_button.png
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)    10636 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/trace_button.png
+-rw-r--r--   0 root         (0) root         (0)    16807 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/trace_popup.png
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/tracing.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/DiagramTraceService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/services/
+-rw-r--r--   0 root         (0) root         (0)    11217 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.633558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-29 10:19:16.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2101 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:41.631558 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:21:41.634558 peek-plugin-diagram-trace-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2507 2023-06-29 10:21:41.000000 peek-plugin-diagram-trace-3.4.6/setup.py
```

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/__init__.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
 from typing import Type
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/diagramTrace.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/script.py.mako` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/alembic/versions/007ac5377946_initial_tables.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/client/DeviceTupleProcessorActionProxy.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/controller/MainController.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/server/tuple_providers/SettingPropertyTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/_private/storage/Setting.py` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/admin-doc/admin_tasks/edit_layers.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/clear_trace_button.png` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/clear_trace_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/trace_button.png` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/trace_button.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/both-doc/trace_popup.png` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/both-doc/trace_popup.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/services/PrivateDiagramTraceTupleService.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin-module/_private/tuples/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace/plugin_package.json` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace/plugin_package.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9960317460317462%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -50,15 +50,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_diagram_trace",
         "title": "Diagram Trace",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "admin",
         "field",
```

### Comparing `peek-plugin-diagram-trace-3.4.5/peek_plugin_diagram_trace.egg-info/SOURCES.txt` & `peek-plugin-diagram-trace-3.4.6/peek_plugin_diagram_trace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-diagram-trace-3.4.5/setup.py` & `peek-plugin-diagram-trace-3.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_diagram_trace"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin DiagramTrace - My first enhancement."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

