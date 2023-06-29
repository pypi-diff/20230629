# Comparing `tmp/peek-plugin-chat-3.4.5.tar.gz` & `tmp/peek-plugin-chat-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-plugin-chat-3.4.5.tar", last modified: Wed Jun 28 07:27:41 2023, max compression
+gzip compressed data, was "peek-plugin-chat-3.4.6.tar", last modified: Thu Jun 29 10:21:29 2023, max compression
```

## Comparing `peek-plugin-chat-3.4.5.tar` & `peek-plugin-chat-3.4.6.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.276099 peek-plugin-chat-3.4.5/peek_plugin_chat/
--rw-r--r--   0 root         (0) root         (0)      680 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.276099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/
--rw-r--r--   0 root         (0) root         (0)      202 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.276099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/
--rw-r--r--   0 root         (0) root         (0)      577 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/chat.component.html
--rw-r--r--   0 root         (0) root         (0)      203 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/chat.component.ts
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/chat.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.276099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      543 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     5669 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/5288d02e94e4_initial_schema.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/52f3163b45de_added_read_payload_constraint.py
--rw-r--r--   0 root         (0) root         (0)      464 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/9b0976dcfd53_truncate_chats.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/a4d6b26d39b7_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      487 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/
--rw-r--r--   0 root         (0) root         (0)     1658 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     3601 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     3360 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.ts
--rw-r--r--   0 root         (0) root         (0)     2536 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat.module.ts
--rw-r--r--   0 root         (0) root         (0)      766 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat.routes.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/msg-list/
--rw-r--r--   0 root         (0) root         (0)     2317 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.mweb.html
--rw-r--r--   0 root         (0) root         (0)     7377 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-assets/
--rw-r--r--   0 root         (0) root         (0)     3961 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-assets/icon.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/
--rw-r--r--   0 root         (0) root         (0)     2437 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/ChatApi.py
--rw-r--r--   0 root         (0) root         (0)     4509 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.277099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.278099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)    16376 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     5518 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/TaskController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.278099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     2331 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/tuple_providers/ChatTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.278099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/ChatTuple.py
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/ChatUserTuple.py
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     1134 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/MessageReadPayloadTuple.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/MessageTuple.py
--rw-r--r--   0 root         (0) root         (0)     7698 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)      456 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.278099 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      416 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/tuples/ChatUserReadActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/tuples/CreateChatActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/tuples/SendMessageActionTuple.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.278099 peek-plugin-chat-3.4.5/peek_plugin_chat/admin-doc/
--rw-r--r--   0 root         (0) root         (0)    40599 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/admin-doc/flow_diagram.png
--rw-r--r--   0 root         (0) root         (0)      735 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/admin-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/both-doc/
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)      411 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      579 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/ChatTuple.ts
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/ChatUserReadActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      551 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/ChatUserTuple.ts
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/CreateChatActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/MessageTuple.ts
--rw-r--r--   0 root         (0) root         (0)      434 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/SendMessageActionTuple.ts
--rw-r--r--   0 root         (0) root         (0)       59 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/package.json
--rw-r--r--   0 root         (0) root         (0)     1319 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/server/
--rw-r--r--   0 root         (0) root         (0)     4823 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/server/ChatApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.279099 peek-plugin-chat-3.4.5/peek_plugin_chat/tuples/
--rw-r--r--   0 root         (0) root         (0)      194 2023-06-28 07:25:25.000000 peek-plugin-chat-3.4.5/peek_plugin_chat/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:27:41.276099 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3881 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:27:41.280099 peek-plugin-chat-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2510 2023-06-28 07:27:41.000000 peek-plugin-chat-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.102534 peek-plugin-chat-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 10:21:29.102534 peek-plugin-chat-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.098534 peek-plugin-chat-3.4.6/peek_plugin_chat/
+-rw-r--r--   0 root         (0) root         (0)      680 2023-06-29 10:21:28.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.098534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.098534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/chat.component.html
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/chat.component.ts
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/chat.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      543 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     5669 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/5288d02e94e4_initial_schema.py
+-rw-r--r--   0 root         (0) root         (0)     1339 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/52f3163b45de_added_read_payload_constraint.py
+-rw-r--r--   0 root         (0) root         (0)      464 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/9b0976dcfd53_truncate_chats.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/a4d6b26d39b7_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      487 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/
+-rw-r--r--   0 root         (0) root         (0)     1658 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     3601 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     3360 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2536 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat.module.ts
+-rw-r--r--   0 root         (0) root         (0)      766 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat.routes.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.099534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/msg-list/
+-rw-r--r--   0 root         (0) root         (0)     2317 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.mweb.html
+-rw-r--r--   0 root         (0) root         (0)     7377 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-assets/
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-assets/icon.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     2437 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/ChatApi.py
+-rw-r--r--   0 root         (0) root         (0)     4509 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)    16376 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     5518 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/TaskController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     2331 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/tuple_providers/ChatTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.100534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/ChatTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1455 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/ChatUserTuple.py
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     1134 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/MessageReadPayloadTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/MessageTuple.py
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)      456 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      416 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/tuples/ChatUserReadActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/tuples/CreateChatActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/tuples/SendMessageActionTuple.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/admin-doc/
+-rw-r--r--   0 root         (0) root         (0)    40599 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/admin-doc/flow_diagram.png
+-rw-r--r--   0 root         (0) root         (0)      735 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/admin-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)      411 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/ChatTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/ChatUserReadActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/ChatUserTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/CreateChatActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/MessageTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      434 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/SendMessageActionTuple.ts
+-rw-r--r--   0 root         (0) root         (0)       59 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/package.json
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-06-29 10:21:28.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/server/
+-rw-r--r--   0 root         (0) root         (0)     4823 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/server/ChatApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.101534 peek-plugin-chat-3.4.6/peek_plugin_chat/tuples/
+-rw-r--r--   0 root         (0) root         (0)      194 2023-06-29 10:19:16.000000 peek-plugin-chat-3.4.6/peek_plugin_chat/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:21:29.098534 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 10:21:29.000000 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3881 2023-06-29 10:21:29.000000 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:21:29.000000 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:21:29.000000 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 10:21:29.000000 peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:21:29.102534 peek-plugin-chat-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2510 2023-06-29 10:21:28.000000 peek-plugin-chat-3.4.6/setup.py
```

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/__init__.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.4.5'
+__version__ = '3.4.6'
 
 from peek_plugin_base.server.PluginLogicEntryHookABC import PluginLogicEntryHookABC
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import PluginClientEntryHookABC
```

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/chat.component.html` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/chat.component.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/admin-app/chat.module.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/admin-app/chat.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/script.py.mako` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/5288d02e94e4_initial_schema.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/5288d02e94e4_initial_schema.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/52f3163b45de_added_read_payload_constraint.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/52f3163b45de_added_read_payload_constraint.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/alembic/versions/a4d6b26d39b7_timezone_aware.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/alembic/versions/a4d6b26d39b7_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/client/ClientEntryHook.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.mweb.html` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/chat-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.mweb.html` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat-list/new-chat/new-chat.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat.module.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat.module.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/chat.routes.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/chat.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.mweb.html` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.mweb.html`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-app/msg-list/msg-list.component.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/mobile-assets/icon.png` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/mobile-assets/icon.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/ChatApi.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/ChatApi.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/LogicEntryHook.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/TupleActionProcessor.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/TupleDataObservable.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/TupleDataObservable.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/MainController.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/controller/TaskController.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/controller/TaskController.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/server/tuple_providers/ChatTupleProvider.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/server/tuple_providers/ChatTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/ChatTuple.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/ChatTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/ChatUserTuple.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/ChatUserTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/MessageReadPayloadTuple.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/MessageReadPayloadTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/MessageTuple.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/MessageTuple.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/_private/storage/Setting.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/_private/storage/Setting.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/admin-doc/flow_diagram.png` & `peek-plugin-chat-3.4.6/peek_plugin_chat/admin-doc/flow_diagram.png`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/admin-doc/index.rst` & `peek-plugin-chat-3.4.6/peek_plugin_chat/admin-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/ChatTuple.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/ChatTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/ChatUserTuple.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/ChatUserTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/plugin-module/_private/tuples/MessageTuple.ts` & `peek-plugin-chat-3.4.6/peek_plugin_chat/plugin-module/_private/tuples/MessageTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/plugin_package.json` & `peek-plugin-chat-3.4.6/peek_plugin_chat/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'plugin'": "{'version': '3.4.6'}"}*

```diff
@@ -32,15 +32,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_plugin_chat",
         "title": "Chat",
-        "version": "3.4.5",
+        "version": "3.4.6",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "field",
         "storage",
         "admin",
```

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat/server/ChatApiABC.py` & `peek-plugin-chat-3.4.6/peek_plugin_chat/server/ChatApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/peek_plugin_chat.egg-info/SOURCES.txt` & `peek-plugin-chat-3.4.6/peek_plugin_chat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-plugin-chat-3.4.5/setup.py` & `peek-plugin-chat-3.4.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_plugin_chat"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Plugin - Chat - Chat between users in the Peek platform"
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

