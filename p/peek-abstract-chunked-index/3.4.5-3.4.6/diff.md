# Comparing `tmp/peek-abstract-chunked-index-3.4.5.tar.gz` & `tmp/peek-abstract-chunked-index-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-abstract-chunked-index-3.4.5.tar", last modified: Wed Jun 28 07:25:56 2023, max compression
+gzip compressed data, was "peek-abstract-chunked-index-3.4.6.tar", last modified: Thu Jun 29 10:19:46 2023, max compression
```

## Comparing `peek-abstract-chunked-index-3.4.5.tar` & `peek-abstract-chunked-index-3.4.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.516065 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/
--rw-r--r--   0 root         (0) root         (0)      614 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      530 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts
--rw-r--r--   0 root         (0) root         (0)      920 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts
--rw-r--r--   0 root         (0) root         (0)      963 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts
--rw-r--r--   0 root         (0) root         (0)      565 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/PluginNames.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/admin/
--rw-r--r--   0 root         (0) root         (0)      513 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/
--rw-r--r--   0 root         (0) root         (0)      394 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexEncodedChunkTuple.ts
--rw-r--r--   0 root         (0) root         (0)    20958 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts
--rw-r--r--   0 root         (0) root         (0)      610 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      342 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/index.ts
--rw-r--r--   0 root         (0) root         (0)     2838 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)      253 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      334 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/tuples/OfflineConfigTuple.ts
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.517064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/
--rw-r--r--   0 root         (0) root         (0)    12460 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py
--rw-r--r--   0 root         (0) root         (0)     8543 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py
--rw-r--r--   0 root         (0) root         (0)     3069 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py
--rw-r--r--   0 root         (0) root         (0)     4347 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py
--rw-r--r--   0 root         (0) root         (0)     6349 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/handlers/
--rw-r--r--   0 root         (0) root         (0)     9390 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     1223 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo
--rw-r--r--   0 root         (0) root         (0)     2330 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/
--rw-r--r--   0 root         (0) root         (0)     6534 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py
--rw-r--r--   0 root         (0) root         (0)     3222 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.518064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/
--rw-r--r--   0 root         (0) root         (0)    18313 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py
--rw-r--r--   0 root         (0) root         (0)     1552 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py
--rw-r--r--   0 root         (0) root         (0)     1710 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py
--rw-r--r--   0 root         (0) root         (0)      254 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ChunkedIndexQueueStatusTupleABC.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/
--rw-r--r--   0 root         (0) root         (0)     6206 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo
--rw-r--r--   0 root         (0) root         (0)     9317 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexRemover.py_abctodo
--rw-r--r--   0 root         (0) root         (0)      631 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-28 07:25:22.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 07:25:56.516065 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4023 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 07:25:56.519064 peek-abstract-chunked-index-3.4.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2488 2023-06-28 07:25:56.000000 peek-abstract-chunked-index-3.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.965336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/
+-rw-r--r--   0 root         (0) root         (0)      614 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      530 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      920 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts
+-rw-r--r--   0 root         (0) root         (0)      963 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/PluginNames.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/admin/
+-rw-r--r--   0 root         (0) root         (0)      513 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/
+-rw-r--r--   0 root         (0) root         (0)      394 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexEncodedChunkTuple.ts
+-rw-r--r--   0 root         (0) root         (0)    20958 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts
+-rw-r--r--   0 root         (0) root         (0)      610 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      342 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/index.ts
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)      253 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/tuples/OfflineConfigTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.966336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.967336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/
+-rw-r--r--   0 root         (0) root         (0)    12460 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     8543 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py
+-rw-r--r--   0 root         (0) root         (0)     3069 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py
+-rw-r--r--   0 root         (0) root         (0)     6349 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.967336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/handlers/
+-rw-r--r--   0 root         (0) root         (0)     9390 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.967336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)     2330 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.967336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.967336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/
+-rw-r--r--   0 root         (0) root         (0)     6534 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py
+-rw-r--r--   0 root         (0) root         (0)     3222 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)    18313 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py
+-rw-r--r--   0 root         (0) root         (0)     1921 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)     1710 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py
+-rw-r--r--   0 root         (0) root         (0)      254 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ChunkedIndexQueueStatusTupleABC.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.968336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/
+-rw-r--r--   0 root         (0) root         (0)     6206 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)     9317 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexRemover.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)      631 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-29 10:19:13.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 10:19:46.965336 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4023 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-29 10:19:46.969336 peek-abstract-chunked-index-3.4.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2488 2023-06-29 10:19:46.000000 peek-abstract-chunked-index-3.4.6/setup.py
```

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/PlatformDependencyTest.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/PlatformDependencyTest.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedIndexModelSetTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedIndexService.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/ChunkedTypeTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/admin/ChunkedIndexServerStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexLoaderService.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/chunked-index-loader/ChunkedIndexUpdateDateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/plugin-module/_private/index-blueprint-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerLoadFromLogicMixin.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerNotifyMixin.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerOfflineIndexMixin.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteAppDbMixin.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/controller/ACICacheControllerSqliteCacheMixin.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/handlers/ACICacheHandlerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedIndexUpdateDateTupleProvider.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/client/tuple_providers/ChunkedTupleProvider.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkLoadRpcABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/client_handlers/ACIChunkUpdateHandlerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorQueueControllerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusControllerABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/server/controller/ACIProcessorStatusNotifierABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIEncodedChunkTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIProcessorQueueTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/tuples/ACIUpdateDateTupleABC.py`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexCompiler.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/ChunkedIndexImporter.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index/private/worker/tasks/_ChunkedIndexCalcChunkKey.py_abctodo`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/peek_abstract_chunked_index.egg-info/SOURCES.txt` & `peek-abstract-chunked-index-3.4.6/peek_abstract_chunked_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-abstract-chunked-index-3.4.5/setup.py` & `peek-abstract-chunked-index-3.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_abstract_chunked_index"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.5"
+package_version = "3.4.6"
 description = "Peek Abstract Chunked Index"
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

