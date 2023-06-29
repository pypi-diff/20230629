# Comparing `tmp/peek-core-api-3.4.5.tar.gz` & `tmp/peek-core-api-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-api-3.4.5.tar", last modified: Wed Jun 28 07:26:39 2023, max compression
+gzip compressed data, was "peek-core-api-3.4.6.tar", last modified: Thu Jun 29 10:20:29 2023, max compression
```

## Comparing `peek-core-api-3.4.5.tar` & `peek-core-api-3.4.6.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      138 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api/
--rw-r--r--   0 root         (0) root         (0)      533 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api/_private/
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api/_private/agent/
--rw-r--r--   0 root         (0) root         (0)     1471 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/AgentEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      779 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/AgentTupleDataObserver.py
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/RpcForServer.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api/_private/agent/controller/
--rw-r--r--   0 root         (0) root         (0)     6475 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/controller/OutboundMessageController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/agent/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic/versions/b6ab5ef39719_added_lastpublisheddate.py
--rw-r--r--   0 root         (0) root         (0)     3922 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic/versions/c31aaab9c30e_add_core_api_tables.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/logic/
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/AgentTupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)     3396 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/logic/agent_handlers/
--rw-r--r--   0 root         (0) root         (0)     5190 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/agent_handlers/RpcForAgent.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/agent_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/logic/api/
--rw-r--r--   0 root         (0) root         (0)     1055 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/api/CoreApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/
--rw-r--r--   0 root         (0) root         (0)     2981 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/ApiManagementController.py
--rw-r--r--   0 root         (0) root         (0)     4096 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/ApiPublishingController.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/HashController.py
--rw-r--r--   0 root         (0) root         (0)     1661 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     5019 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/MessageQueueController.py
--rw-r--r--   0 root         (0) root         (0)     5153 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/SqlController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.891079 peek-core-api-3.4.5/peek_core_api/_private/logic/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)      840 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/tuple_providers/MessageBatchAvailableTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/logic/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.892079 peek-core-api-3.4.5/peek_core_api/_private/server/
--rw-r--r--   0 root         (0) root         (0)     2975 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.892079 peek-core-api-3.4.5/peek_core_api/_private/server/api/
--rw-r--r--   0 root         (0) root         (0)      856 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/api/CoreApi.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.892079 peek-core-api-3.4.5/peek_core_api/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     1739 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/controller/ApiManagementController.py
--rw-r--r--   0 root         (0) root         (0)     2374 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/controller/MessageQueueController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.892079 peek-core-api-3.4.5/peek_core_api/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      708 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     4185 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/MessageQueueTable.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/PublishedApiTable.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/WebhookMapTable.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/WebhookTable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/peek_core_api/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      666 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/GzippedDataHttpResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)      291 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageBatchAvailableTuple.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageHttpRequestTuple.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageHttpResponseTuple.py
--rw-r--r--   0 root         (0) root         (0)     1582 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageQueueTuple.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/WebhookTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/peek_core_api/admin_doc/
--rw-r--r--   0 root         (0) root         (0)      101 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/admin_doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/peek_core_api/server/
--rw-r--r--   0 root         (0) root         (0)     1208 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/server/CoreApiABC.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/server/CoreApiProvider.py
--rw-r--r--   0 root         (0) root         (0)     2294 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/server/CoreApiProviderABC.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/server/JsonDataTupleProviderABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:23.000000 peek-core-api-3.4.5/peek_core_api/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:26:39.890079 peek-core-api-3.4.5/peek_core_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      392 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3202 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/peek_core_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:26:39.893079 peek-core-api-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2572 2023-06-28 07:26:39.000000 peek-core-api-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.241418 peek-core-api-3.4.6/peek_core_api/
+-rw-r--r--   0 root         (0) root         (0)      533 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.241418 peek-core-api-3.4.6/peek_core_api/_private/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.241418 peek-core-api-3.4.6/peek_core_api/_private/agent/
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/AgentEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      779 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/AgentTupleDataObserver.py
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/RpcForServer.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.241418 peek-core-api-3.4.6/peek_core_api/_private/agent/controller/
+-rw-r--r--   0 root         (0) root         (0)     6475 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/controller/OutboundMessageController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/agent/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic/versions/b6ab5ef39719_added_lastpublisheddate.py
+-rw-r--r--   0 root         (0) root         (0)     3922 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic/versions/c31aaab9c30e_add_core_api_tables.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/logic/
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/AgentTupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/logic/agent_handlers/
+-rw-r--r--   0 root         (0) root         (0)     5190 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/agent_handlers/RpcForAgent.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/agent_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/logic/api/
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/api/CoreApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.242418 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/
+-rw-r--r--   0 root         (0) root         (0)     2981 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/ApiManagementController.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/ApiPublishingController.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/HashController.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     5019 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/MessageQueueController.py
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/SqlController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.243418 peek-core-api-3.4.6/peek_core_api/_private/logic/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)      840 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/tuple_providers/MessageBatchAvailableTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/logic/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.243418 peek-core-api-3.4.6/peek_core_api/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     2975 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.243418 peek-core-api-3.4.6/peek_core_api/_private/server/api/
+-rw-r--r--   0 root         (0) root         (0)      856 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/api/CoreApi.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.243418 peek-core-api-3.4.6/peek_core_api/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     1739 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/controller/ApiManagementController.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/controller/MessageQueueController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.243418 peek-core-api-3.4.6/peek_core_api/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      708 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/MessageQueueTable.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/PublishedApiTable.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/WebhookMapTable.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/WebhookTable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/peek_core_api/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/GzippedDataHttpResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)      291 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageBatchAvailableTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageHttpRequestTuple.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageHttpResponseTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageQueueTuple.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/WebhookTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/peek_core_api/admin_doc/
+-rw-r--r--   0 root         (0) root         (0)      101 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/admin_doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/peek_core_api/server/
+-rw-r--r--   0 root         (0) root         (0)     1208 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/server/CoreApiABC.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/server/CoreApiProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/server/CoreApiProviderABC.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/server/JsonDataTupleProviderABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:14.000000 peek-core-api-3.4.6/peek_core_api/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:20:29.241418 peek-core-api-3.4.6/peek_core_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      392 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/peek_core_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:20:29.244418 peek-core-api-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2572 2023-06-29 10:20:29.000000 peek-core-api-3.4.6/setup.py
```

### Comparing `peek-core-api-3.4.5/peek_core_api/__init__.py` & `peek-core-api-3.4.6/peek_core_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from peek_plugin_base.agent.PluginAgentEntryHookABC import (
     PluginAgentEntryHookABC,
 )
 from peek_plugin_base.server.PluginLogicEntryHookABC import (
     PluginLogicEntryHookABC,
 )
 
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.logic.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/agent/AgentEntryHook.py` & `peek-core-api-3.4.6/peek_core_api/_private/agent/AgentEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/agent/AgentTupleDataObserver.py` & `peek-core-api-3.4.6/peek_core_api/_private/agent/AgentTupleDataObserver.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/agent/RpcForServer.py` & `peek-core-api-3.4.6/peek_core_api/_private/agent/RpcForServer.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/agent/controller/OutboundMessageController.py` & `peek-core-api-3.4.6/peek_core_api/_private/agent/controller/OutboundMessageController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/alembic/script.py.mako` & `peek-core-api-3.4.6/peek_core_api/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/alembic/versions/b6ab5ef39719_added_lastpublisheddate.py` & `peek-core-api-3.4.6/peek_core_api/_private/alembic/versions/b6ab5ef39719_added_lastpublisheddate.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/alembic/versions/c31aaab9c30e_add_core_api_tables.py` & `peek-core-api-3.4.6/peek_core_api/_private/alembic/versions/c31aaab9c30e_add_core_api_tables.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/AgentTupleDataObservable.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/AgentTupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/LogicEntryHook.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/TupleDataObservable.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/agent_handlers/RpcForAgent.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/agent_handlers/RpcForAgent.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/api/CoreApi.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/api/CoreApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/controller/ApiManagementController.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/controller/ApiManagementController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/controller/ApiPublishingController.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/controller/ApiPublishingController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/controller/MainController.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/controller/MessageQueueController.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/controller/MessageQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/controller/SqlController.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/controller/SqlController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/logic/tuple_providers/MessageBatchAvailableTupleProvider.py` & `peek-core-api-3.4.6/peek_core_api/_private/logic/tuple_providers/MessageBatchAvailableTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/server/LogicEntryHook.py` & `peek-core-api-3.4.6/peek_core_api/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/server/api/CoreApi.py` & `peek-core-api-3.4.6/peek_core_api/_private/server/api/CoreApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/server/controller/ApiManagementController.py` & `peek-core-api-3.4.6/peek_core_api/_private/server/controller/ApiManagementController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/server/controller/MessageQueueController.py` & `peek-core-api-3.4.6/peek_core_api/_private/server/controller/MessageQueueController.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/storage/DeclarativeBase.py` & `peek-core-api-3.4.6/peek_core_api/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/storage/MessageQueueTable.py` & `peek-core-api-3.4.6/peek_core_api/_private/storage/MessageQueueTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/storage/PublishedApiTable.py` & `peek-core-api-3.4.6/peek_core_api/_private/storage/PublishedApiTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/storage/WebhookMapTable.py` & `peek-core-api-3.4.6/peek_core_api/_private/storage/WebhookMapTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/storage/WebhookTable.py` & `peek-core-api-3.4.6/peek_core_api/_private/storage/WebhookTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/tuples/GzippedDataHttpResponseTuple.py` & `peek-core-api-3.4.6/peek_core_api/_private/tuples/GzippedDataHttpResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageHttpRequestTuple.py` & `peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageHttpRequestTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageHttpResponseTuple.py` & `peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageHttpResponseTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/_private/tuples/MessageQueueTuple.py` & `peek-core-api-3.4.6/peek_core_api/_private/tuples/MessageQueueTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/plugin_package.json` & `peek-core-api-3.4.6/peek_core_api/plugin_package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948979591836735%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -14,15 +14,15 @@
     "logic": {},
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_api",
         "title": "API",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "agent",
         "admin",
```

### Comparing `peek-core-api-3.4.5/peek_core_api/server/CoreApiABC.py` & `peek-core-api-3.4.6/peek_core_api/server/CoreApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/server/CoreApiProvider.py` & `peek-core-api-3.4.6/peek_core_api/server/CoreApiProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/server/CoreApiProviderABC.py` & `peek-core-api-3.4.6/peek_core_api/server/CoreApiProviderABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api/server/JsonDataTupleProviderABC.py` & `peek-core-api-3.4.6/peek_core_api/server/JsonDataTupleProviderABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/peek_core_api.egg-info/SOURCES.txt` & `peek-core-api-3.4.6/peek_core_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-api-3.4.5/setup.py` & `peek-core-api-3.4.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_api"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Core API - Outbound API with guaranteed delivery"
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

