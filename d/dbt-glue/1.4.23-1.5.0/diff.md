# Comparing `tmp/dbt-glue-1.4.23.tar.gz` & `tmp/dbt-glue-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-glue-1.4.23.tar", last modified: Mon Jun 19 12:14:15 2023, max compression
+gzip compressed data, was "dbt-glue-1.5.0.tar", last modified: Thu Jun 29 09:30:25 2023, max compression
```

## Comparing `dbt-glue-1.4.23.tar` & `dbt-glue-1.5.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.803721 dbt-glue-1.4.23/
--rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/LICENSE
--rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/NOTICE
--rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 12:14:15.803578 dbt-glue-1.4.23/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.4.23/README.md
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794809 dbt-glue-1.4.23/dbt/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794619 dbt-glue-1.4.23/dbt/adapters/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.798246 dbt-glue-1.4.23/dbt/adapters/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.4.23/dbt/adapters/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       18 2023-06-19 12:12:21.000000 dbt-glue-1.4.23/dbt/adapters/glue/__version__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     3431 2023-04-06 15:50:22.000000 dbt-glue-1.4.23/dbt/adapters/glue/connections.py
--rw-r--r--   0 menuetb    (504) staff       (20)     2590 2023-04-06 15:50:17.000000 dbt-glue-1.4.23/dbt/adapters/glue/credentials.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.799288 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/
--rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/commons.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8767 2023-04-06 14:25:36.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/connection.py
--rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/cursor.py
--rw-r--r--   0 menuetb    (504) staff       (20)    36485 2023-04-27 13:24:38.000000 dbt-glue-1.4.23/dbt/adapters/glue/impl.py
--rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.4.23/dbt/adapters/glue/relation.py
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.794867 dbt-glue-1.4.23/dbt/include/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800078 dbt-glue-1.4.23/dbt/include/glue/
--rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.4.23/dbt/include/glue/__init__.py
--rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/dbt_project.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800325 dbt-glue-1.4.23/dbt/include/glue/macros/
--rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.4.23/dbt/include/glue/macros/adapters.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.800864 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/
--rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/generic_test_sql/relationships.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.801539 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.801949 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/
--rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/seed.sql
--rw-r--r--   0 menuetb    (504) staff       (20)    10358 2023-01-18 17:12:34.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/snapshot.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.802186 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/
--rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/macros/materializations/view.sql
--rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.4.23/dbt/include/glue/sample_profiles.yml
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.795441 dbt-glue-1.4.23/dbt/include/glue/tests/
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.802322 dbt-glue-1.4.23/dbt/include/glue/tests/generic/
--rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.4.23/dbt/include/glue/tests/generic/builtin.sql
-drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-19 12:14:15.803348 dbt-glue-1.4.23/dbt_glue.egg-info/
--rw-r--r--   0 menuetb    (504) staff       (20)    45028 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/PKG-INFO
--rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/SOURCES.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/dependency_links.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.4.23/dbt_glue.egg-info/not-zip-safe
--rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/requires.txt
--rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-19 12:14:15.000000 dbt-glue-1.4.23/dbt_glue.egg-info/top_level.txt
--rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-19 12:14:15.803777 dbt-glue-1.4.23/setup.cfg
--rw-r--r--   0 menuetb    (504) staff       (20)     2872 2023-04-27 13:24:38.000000 dbt-glue-1.4.23/setup.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.782446 dbt-glue-1.5.0/
+-rw-r--r--   0 menuetb    (504) staff       (20)    10142 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/LICENSE
+-rw-r--r--   0 menuetb    (504) staff       (20)       67 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/NOTICE
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-06-29 09:30:25.782269 dbt-glue-1.5.0/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)    44126 2023-06-15 08:24:37.000000 dbt-glue-1.5.0/README.md
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774231 dbt-glue-1.5.0/dbt/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774051 dbt-glue-1.5.0/dbt/adapters/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.776975 dbt-glue-1.5.0/dbt/adapters/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)      394 2023-04-06 15:48:24.000000 dbt-glue-1.5.0/dbt/adapters/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       17 2023-06-29 08:43:24.000000 dbt-glue-1.5.0/dbt/adapters/glue/__version__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     3917 2023-06-29 08:34:49.000000 dbt-glue-1.5.0/dbt/adapters/glue/connections.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     2524 2023-06-29 08:38:08.000000 dbt-glue-1.5.0/dbt/adapters/glue/credentials.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.777791 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/
+-rw-r--r--   0 menuetb    (504) staff       (20)      140 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1216 2023-04-27 15:40:43.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/commons.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     9699 2023-06-29 08:34:49.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/connection.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     8229 2023-04-06 15:56:20.000000 dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/cursor.py
+-rw-r--r--   0 menuetb    (504) staff       (20)    36786 2023-06-29 09:26:37.000000 dbt-glue-1.5.0/dbt/adapters/glue/impl.py
+-rw-r--r--   0 menuetb    (504) staff       (20)     1264 2023-04-07 07:53:59.000000 dbt-glue-1.5.0/dbt/adapters/glue/relation.py
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774293 dbt-glue-1.5.0/dbt/include/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.778503 dbt-glue-1.5.0/dbt/include/glue/
+-rw-r--r--   0 menuetb    (504) staff       (20)       51 2022-04-05 16:42:41.000000 dbt-glue-1.5.0/dbt/include/glue/__init__.py
+-rw-r--r--   0 menuetb    (504) staff       (20)       72 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/dbt_project.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.778880 dbt-glue-1.5.0/dbt/include/glue/macros/
+-rw-r--r--   0 menuetb    (504) staff       (20)     5352 2023-01-17 10:30:07.000000 dbt-glue-1.5.0/dbt/include/glue/macros/adapters.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.779355 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/
+-rw-r--r--   0 menuetb    (504) staff       (20)      494 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      370 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/generic_test_sql/relationships.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.779960 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780469 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/
+-rw-r--r--   0 menuetb    (504) staff       (20)     4347 2023-06-19 12:11:48.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1689 2022-10-07 12:46:47.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)     1436 2023-01-06 16:44:08.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/seed.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)    10334 2023-06-29 09:23:22.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/snapshot.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780677 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/
+-rw-r--r--   0 menuetb    (504) staff       (20)     1159 2022-11-03 13:40:21.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      112 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/macros/materializations/view.sql
+-rw-r--r--   0 menuetb    (504) staff       (20)      584 2023-06-15 08:24:37.000000 dbt-glue-1.5.0/dbt/include/glue/sample_profiles.yml
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.774866 dbt-glue-1.5.0/dbt/include/glue/tests/
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.780863 dbt-glue-1.5.0/dbt/include/glue/tests/generic/
+-rw-r--r--   0 menuetb    (504) staff       (20)      290 2022-07-11 06:48:28.000000 dbt-glue-1.5.0/dbt/include/glue/tests/generic/builtin.sql
+drwxr-xr-x   0 menuetb    (504) staff       (20)        0 2023-06-29 09:30:25.781904 dbt-glue-1.5.0/dbt_glue.egg-info/
+-rw-r--r--   0 menuetb    (504) staff       (20)    44977 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/PKG-INFO
+-rw-r--r--   0 menuetb    (504) staff       (20)     1230 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        1 2022-05-12 16:43:26.000000 dbt-glue-1.5.0/dbt_glue.egg-info/not-zip-safe
+-rw-r--r--   0 menuetb    (504) staff       (20)       46 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/requires.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)        4 2023-06-29 09:30:25.000000 dbt-glue-1.5.0/dbt_glue.egg-info/top_level.txt
+-rw-r--r--   0 menuetb    (504) staff       (20)       38 2023-06-29 09:30:25.782505 dbt-glue-1.5.0/setup.cfg
+-rw-r--r--   0 menuetb    (504) staff       (20)     2857 2023-06-29 08:57:00.000000 dbt-glue-1.5.0/setup.py
```

### Comparing `dbt-glue-1.4.23/LICENSE` & `dbt-glue-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/PKG-INFO` & `dbt-glue-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.23
+Version: 1.5.0
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <p align="center">
   <img src="/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
```

### Comparing `dbt-glue-1.4.23/README.md` & `dbt-glue-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/connections.py` & `dbt-glue-1.5.0/dbt/adapters/glue/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import contextmanager
 import agate
-from typing import Any, List
+from typing import Any, List, Dict
 from dbt.adapters.sql import SQLConnectionManager
 from dbt.contracts.connection import AdapterResponse
 from dbt.exceptions import (
     FailedToConnectError,
     DbtRuntimeError
 )
 import dbt
@@ -19,27 +19,32 @@
     FAIL = "fail"
 
 class ReturnCode:
     OK = "OK"
 
 class GlueConnectionManager(SQLConnectionManager):
     TYPE = "glue"
+    GLUE_CONNECTIONS_BY_THREAD: Dict[str, GlueConnection] = {}
+
 
     @classmethod
     def open(cls, connection):
         if connection.state == "open":
             logger.debug("Connection is already open, skipping open.")
             return connection
 
         credentials = connection.credentials
         try:
-            cls._connection: GlueConnection = GlueConnection(credentials=credentials)
-            cls._connection.connect()
+            key = cls.get_thread_identifier()
+            if not cls.GLUE_CONNECTIONS_BY_THREAD.get(key):
+                logger.debug(f"opening a new glue connection for thread : {key}")
+                cls.GLUE_CONNECTIONS_BY_THREAD[key]: GlueConnection = GlueConnection(credentials=credentials)
+                cls.GLUE_CONNECTIONS_BY_THREAD[key].connect()
             connection.state = GlueSessionState.OPEN
-            connection.handle = cls._connection
+            connection.handle = cls.GLUE_CONNECTIONS_BY_THREAD[key]
             return connection
         except Exception as e:
             logger.error(
                 f"Got an error when attempting to open a GlueSession : {e}"
             )
             connection.handle = None
             connection.state = GlueSessionState.FAIL
@@ -99,11 +104,13 @@
         logger.debug("NotImplemented: commit")
 
     def rollback(self, *args, **kwargs):
         logger.debug("NotImplemented: rollback")
 
     def cleanup_all(self):
         logger.debug("cleanup called")
-        try:
-            self._connection.close_session()
-        except:
-            logger.debug("connection not yet initialized")
+        for connection in self.GLUE_CONNECTIONS_BY_THREAD.values():
+            try:
+                connection.close_session()
+            except Exception as e:
+                logger.exception(f"failed to close session : {e}")
+                logger.debug("connection not yet initialized")
```

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/credentials.py` & `dbt-glue-1.5.0/dbt/adapters/glue/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 class GlueCredentials(Credentials):
     """ Required connections for a Glue connection"""
     role_arn: str
     region: str
     workers: int
     worker_type: str
     session_provisioning_timeout_in_seconds: int = 120
-    session_id: Optional[str] = None
     location: Optional[str] = None
     extra_jars: Optional[str] = None
     idle_timeout: int = 10
     query_timeout_in_seconds: int = 300
     glue_version: Optional[str] = "3.0"
     security_configuration: Optional[str] = None
     connections: Optional[str] = None
@@ -31,15 +30,15 @@
 
     @property
     def type(self):
         return "glue"
 
     @property
     def unique_field(self):
-        return self.host
+        return "glue"
 
     @classmethod
     def __pre_deserialize__(cls, data):
         data = super().__pre_deserialize__(data)
         if "database" not in data:
             data["database"] = None
         return data
@@ -56,15 +55,14 @@
         self.database = None
 
     def _connection_keys(self):
         """ Keys to show when debugging """
         return [
             'role_arn',
             'region',
-            'session_id',
             'workers',
             'worker_type',
             'session_provisioning_timeout_in_seconds',
             'schema',
             'location',
             'extra_jars',
             'idle_timeout',
```

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/commons.py` & `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/commons.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/connection.py` & `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dbt import exceptions as dbterrors
 import boto3
 from botocore.config import Config
 from waiter import wait
 from dbt.adapters.glue.gluedbapi.cursor import GlueCursor, GlueDictCursor
 from dbt.adapters.glue.credentials import GlueCredentials
 from dbt.adapters.glue.gluedbapi.commons import GlueStatement
+import time
 import uuid
 from dbt.events import AdapterLogger
 
 logger = AdapterLogger("Glue")
 
 
 class GlueSessionState:
@@ -19,35 +20,34 @@
     RUNNING = "RUNNING"
     CLOSED = "CLOSED"
 
 
 @dataclass
 class GlueConnection:
 
-    def __init__(self, credentials: GlueCredentials):
+    def __init__(self, credentials: GlueCredentials, session_id: str = None):
         self.credentials = credentials
+        self._session_id = session_id
         self._client = None
         self._session = None
         self._state = None
 
     def connect(self):
         logger.debug("GlueConnection connect called")
-        if not self.credentials.session_id:
+        if not self._session_id:
             logger.debug("No session present, starting one")
             self._start_session()
         else:
             self._session = {
-                "Session": {"Id": self.credentials.session_id}
+                "Session": {"Id": self._session_id}
             }
             logger.debug("Existing session with status : " + self.state)
             if self.state == GlueSessionState.CLOSED:
                 self._session = self._start_session()
 
-        self._init_session()
-        self.credentials.session_id = self.session_id
         return self.session_id
 
     def _start_session(self):
         logger.debug("GlueConnection _start_session called")
 
         args = {
             "--enable-glue-datacatalog": "true"
@@ -100,20 +100,16 @@
                 },
                 **additional_args)
         except Exception as e:
             logger.error(
                 f"Got an error when attempting to open a GlueSession : {e}"
             )
             raise dbterrors.FailedToConnectError(str(e))
-
-        for elapsed in wait(1):
-            if self.state == GlueSessionState.READY:
-                return self._session
-            if elapsed > self.credentials.session_provisioning_timeout_in_seconds:
-                raise TimeoutError(f"GlueSession took more than {self.credentials.session_provisioning_timeout_in_seconds} seconds to start")
+        
+        self._session_create_time = time.time()
 
     def _init_session(self):
         logger.debug("GlueConnection _init_session called")
         logger.debug("GlueConnection session_id : " + self.session_id)
         statement = GlueStatement(client=self.client, session_id=self.session_id, code=SQLPROXY)
         try:
             statement.execute()
@@ -166,23 +162,48 @@
 
     @staticmethod
     def rollback():
         logger.debug("NotImplemented: rollback")
 
     def cursor(self, as_dict=False) -> GlueCursor:
         logger.debug("GlueConnection cursor called")
-        return GlueDictCursor(connection=self) if as_dict else GlueCursor(connection=self)
+        if self.state == GlueSessionState.READY:
+            self._init_session()
+            return GlueDictCursor(connection=self) if as_dict else GlueCursor(connection=self)
+        else:
+            for elapsed in wait(1):
+                if self.state == GlueSessionState.READY:
+                    self._init_session()
+                    return GlueDictCursor(connection=self) if as_dict else GlueCursor(connection=self)
+                if ((time.time() - self._session_create_time) if self._session_create_time else elapsed) > self.credentials.session_provisioning_timeout_in_seconds:
+                    raise TimeoutError(f"GlueSession took more than {self.credentials.session_provisioning_timeout_in_seconds} seconds to start")
+        
 
     def close_session(self):
-        if self.credentials.session_id:
-            self.client.delete_session(Id=self.credentials.session_id)
+        logger.debug("GlueConnection close_session called")
+        if not self._session:
+            return
+
+        for elapsed in wait(1):
+            if self.state not in [GlueSessionState.PROVISIONING, GlueSessionState.READY, GlueSessionState.RUNNING]:
+                return
+            
+            logger.debug(f"[elapsed {elapsed}s - calling delete_session for {self.session_id} in {self.state} state")
+            try:
+                self.client.delete_session(Id=self.session_id)
+            except Exception as e:
+                if "Session is in PROVISIONING status" in str(e):
+                    logger.debug(f"session is not yet initialised - retrying to close")
+                else:
+                    raise e
+
 
     @property
     def state(self):
-        if self._state in [GlueSessionState.FAILED, GlueSessionState.READY]:
+        if self._state in [GlueSessionState.FAILED]:
             return self._state
         try:
             response = self.client.get_session(Id=self.session_id)
             session = response.get("Session", {})
             self._state = session.get("Status")
         except:
             self._state = GlueSessionState.CLOSED
```

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/gluedbapi/cursor.py` & `dbt-glue-1.5.0/dbt/adapters/glue/gluedbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/impl.py` & `dbt-glue-1.5.0/dbt/adapters/glue/impl.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,30 +69,29 @@
     def convert_datetime_type(cls, agate_table, col_idx):
         return "timestamp"
 
     def get_connection(self):
         connection: GlueConnectionManager = self.connections.get_thread_connection()
         session: GlueConnection = connection.handle
         client = boto3.client("glue", region_name=session.credentials.region)
-        cursor = session.cursor()
 
-        return session, client, cursor
+        return session, client
 
     def list_schemas(self, database: str) -> List[str]:
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         responseGetDatabases = client.get_databases()
         databaseList = responseGetDatabases['DatabaseList']
         schemas = []
         for databaseDict in databaseList:
             databaseName = databaseDict['Name']
             schemas.append(databaseName)
         return schemas
 
     def list_relations_without_caching(self, schema_relation: SparkRelation):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         relations = []
         try:
             response = client.get_tables(
                 DatabaseName=schema_relation.schema,
             )
             for table in response.get("TableList", []):
                 relations.append(self.Relation.create(
@@ -128,15 +127,15 @@
                 return True
         except Exception as e:
             logger.error(e)
 
     @available
     def glue_rename_relation(self, from_relation, to_relation):
         logger.debug("rename " + from_relation.schema + " to " + to_relation.identifier)
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         code = f'''
         custom_glue_code_for_dbt_adapter
         df = spark.sql("""select * from {from_relation.schema}.{from_relation.name}""")
         df.registerTempTable("df")
         table_name = '{to_relation.schema}.{to_relation.name}'
         writer = (
                         df.write.mode("append")
@@ -144,23 +143,23 @@
                         .option("path", "{session.credentials.location}/{to_relation.schema}/{to_relation.name}/")
                     )
         writer.saveAsTable(table_name, mode="append")
         spark.sql("""drop table {from_relation.schema}.{from_relation.name}""")
         SqlWrapper2.execute("""select * from {to_relation.schema}.{to_relation.name} limit 1""")
         '''
         try:
-            cursor.execute(code)
+            session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueRenameRelationFailed") from e
         except Exception as e:
             logger.error(e)
             logger.error("rename_relation exception")
 
     def get_relation(self, database, schema, identifier):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         try:
             response = client.get_table(
                 DatabaseName=schema,
                 Name=identifier
             )
             relations = self.Relation.create(
                 database=schema,
@@ -175,15 +174,15 @@
             return relations
         except client.exceptions.EntityNotFoundException as e:
             logger.debug(e)
         except Exception as e:
             logger.error(e)
 
     def get_columns_in_relation(self, relation: BaseRelation):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         # https://spark.apache.org/docs/3.0.0/sql-ref-syntax-aux-describe-table.html
         response = client.get_table(
                 DatabaseName=relation.schema,
                 Name=relation.name
             )
         _specific_type = response.get("Table", {}).get('Parameters', {}).get('table_type', '')
 
@@ -204,16 +203,16 @@
                 .config("spark.sql.extensions", "org.apache.iceberg.spark.extensions.IcebergSparkSessionExtensions") \
                 .getOrCreate()
             SqlWrapper2.execute("""describe glue_catalog.{relation.schema}.{relation.name}""")'''
         else : 
             code = f'''describe {relation.schema}.{relation.identifier}'''
         columns = []
         try:
-            cursor.execute(code)
-            for record in cursor.fetchall():
+            session.cursor().execute(code)
+            for record in session.cursor().fetchall():
                 column = Column(column=record[0], dtype=record[1])
                 if record[0][:1] != "#":
                     if column not in columns:
                         columns.append(column)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueGetColumnsInRelationFailed") from e
         except Exception as e:
@@ -241,59 +240,59 @@
     def set_iceberg_merge_key(self, merge_key):
         if not isinstance(merge_key, list):
             merge_key = [merge_key]
         return ' AND '.join(['t.{} = s.{}'.format(field, field) for field in merge_key])
             
     @available
     def duplicate_view(self, from_relation: BaseRelation, to_relation: BaseRelation, ):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         code = f'''SHOW CREATE TABLE {from_relation.schema}.{from_relation.identifier}'''
         try:
-            cursor.execute(code)
-            for record in cursor.fetchall():
+            session.cursor().execute(code)
+            for record in session.cursor().fetchall():
                 create_view_statement = record[0]
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueDuplicateViewFailed") from e
         except Exception as e:
             logger.error(e)
         target_query = create_view_statement.replace(from_relation.schema, to_relation.schema)
         target_query = target_query.replace(from_relation.identifier, to_relation.identifier)
         return target_query
 
     @available
     def get_location(self, relation: BaseRelation):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         return f"LOCATION '{session.credentials.location}/{relation.schema}/{relation.name}/'"
 
     @available
     def get_iceberg_location(self, relation: BaseRelation):
         """
         Helper method to deal with issues due to trailing / in Iceberg location.
         The method ensure that no final slash is in the location.
         """
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         s3_path = os.path.join(session.credentials.location, relation.schema, relation.name)
         return f"LOCATION '{s3_path}'"
 
     def drop_schema(self, relation: BaseRelation) -> None:
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         if self.check_schema_exists(relation.database, relation.schema):
             try:
                 client.delete_database(Name=relation.schema)
                 logger.debug("Successfull deleted schema ", relation.schema)
                 self.connections.cleanup_all()
                 return True
             except Exception as e:
                 self.connections.cleanup_all()
                 logger.error(e)
         else:
             logger.debug("No schema to delete")
 
     def create_schema(self, relation: BaseRelation):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         lf = boto3.client("lakeformation", region_name=session.credentials.region)
         sts = boto3.client("sts")
         identity = sts.get_caller_identity()
         account = identity.get("Account")
         if self.check_schema_exists(relation.database, relation.schema):
             logger.debug(f"Schema {relation.database} exists - nothing to do")
         else:
@@ -433,15 +432,15 @@
         ]
         table = agate.Table(rows, column_names)
 
         return table
 
     @available
     def create_csv_table(self, model, agate_table):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         logger.debug(model)
         f = io.StringIO("")
         agate_table.to_json(f)
         if session.credentials.seed_mode == "overwrite":
             mode = "True"
         else:
             mode = "False"
@@ -460,23 +459,23 @@
     df.write\
         .option("path", "{session.credentials.location}/{model["schema"]}/{model["name"]}")\
         .format("{session.credentials.seed_format}")\
         .saveAsTable(table_name)
 SqlWrapper2.execute("""select * from {model["schema"]}.{model["name"]} limit 1""")
 '''
         try:
-            cursor.execute(code)
+            session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueCreateCsvFailed") from e
         except Exception as e:
             logger.error(e)
 
     @available
     def delta_update_manifest(self, target_relation, custom_location):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         if custom_location == "empty":
             location = f"{session.credentials.location}/{target_relation.schema}/{target_relation.name}"
         else:
             location = custom_location
 
         if {session.credentials.delta_athena_prefix} is not None:
             update_manifest_code = f'''
@@ -485,22 +484,22 @@
             deltaTable = DeltaTable.forPath(spark, "{location}")
             deltaTable.generate("symlink_format_manifest")
             spark.sql("MSCK REPAIR TABLE {target_relation.schema}.headertoberepalced_{target_relation.name}") 
             SqlWrapper2.execute("""select 1""")
             '''
 
             try:
-                cursor.execute(re.sub("headertoberepalced", session.credentials.delta_athena_prefix, update_manifest_code))
+                session.cursor().execute(re.sub("headertoberepalced", session.credentials.delta_athena_prefix, update_manifest_code))
             except DbtDatabaseError as e:
                 raise DbtDatabaseError(msg="GlueDeltaUpdateManifestFailed") from e
             except Exception as e:
                 logger.error(e)
     @available
     def delta_create_table(self, target_relation, request, primary_key, partition_key, custom_location):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         logger.debug(request)
 
         table_name = f'{target_relation.schema}.{target_relation.name}'
         if custom_location == "empty":
             location = f"{session.credentials.location}/{target_relation.schema}/{target_relation.name}"
         else:
             location = custom_location
@@ -552,38 +551,38 @@
         else:
             write_data_code = write_data_header + write_data_footer
             create_athena_table = create_athena_table_header + create_athena_table_footer
 
 
 
         try:
-            cursor.execute(write_data_code)
+            session.cursor().execute(write_data_code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueDeltaWriteTableFailed") from e
         except Exception as e:
             logger.error(e)
 
         try:
-            cursor.execute(create_table_query)
+            session.cursor().execute(create_table_query)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueDeltaWriteTableFailed") from e
         except Exception as e:
             logger.error(e)
 
         if {session.credentials.delta_athena_prefix} is not None:
             try:
-                cursor.execute(re.sub("headertoberepalced", session.credentials.delta_athena_prefix, create_athena_table))
+                session.cursor().execute(re.sub("headertoberepalced", session.credentials.delta_athena_prefix, create_athena_table))
             except DbtDatabaseError as e:
                 raise DbtDatabaseError(msg="GlueDeltaCreateTableFailed") from e
             except Exception as e:
                 logger.error(e)
 
     @available
     def get_table_type(self, relation):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         try:
             response = client.get_table(
                 DatabaseName=relation.schema,
                 Name=relation.name
             )
         except client.exceptions.EntityNotFoundException as e:
             logger.debug(e)
@@ -603,22 +602,26 @@
     def hudi_write(self, write_mode, session, target_relation, custom_location):
         if custom_location == "empty":
             return f'''outputDf.write.format('org.apache.hudi').options(**combinedConf).mode('{write_mode}').save("{session.credentials.location}/{target_relation.schema}/{target_relation.name}/")'''
         else:
             return f'''outputDf.write.format('org.apache.hudi').options(**combinedConf).mode('{write_mode}').save("{custom_location}/")'''
 
     @available
-    def hudi_merge_table(self, target_relation, request, primary_key, partition_key, custom_location, hudi_config = {}):
-        session, client, cursor = self.get_connection()
+    def hudi_merge_table(self, target_relation, request, primary_key, partition_key, custom_location, hudi_config):
+        session, client = self.get_connection()
         isTableExists = False
         if self.check_relation_exists(target_relation):
             isTableExists = True
         else:
             isTableExists = False
 
+        # Test if variable hudi_config is NoneType
+        if hudi_config is None:
+            hudi_config = {}
+
         base_config = {
             'className' : 'org.apache.hudi',
             'hoodie.datasource.hive_sync.use_jdbc':'false',
             'hoodie.datasource.write.precombine.field': 'update_hudi_ts',
             'hoodie.consistency.check.enabled': 'true',
             'hoodie.datasource.write.recordkey.field': primary_key,
             'hoodie.table.name': target_relation.name,
@@ -644,23 +647,21 @@
                 'hoodie.index.type': 'GLOBAL_BLOOM',
                 'hoodie.bloom.index.update.partition.path': 'true',
             }
 
         if isTableExists:
             write_mode = 'Append'
             write_operation_config = {
-                'hoodie.upsert.shuffle.parallelism': 20,
                 'hoodie.datasource.write.operation': 'upsert',
                 'hoodie.cleaner.policy': 'KEEP_LATEST_COMMITS',
                 'hoodie.cleaner.commits.retained': 10,
             }
         else :
             write_mode = 'Overwrite'
             write_operation_config = {
-                'hoodie.bulkinsert.shuffle.parallelism': 20,
                 'hoodie.datasource.write.operation': 'bulk_insert',
             }
 
         combined_config = {**base_config, **partition_config, **write_operation_config, **hudi_config}
 
         code = f'''
 custom_glue_code_for_dbt_adapter
@@ -668,27 +669,33 @@
 from pyspark.sql.functions import *
 spark = SparkSession.builder \
 .config("spark.serializer", "org.apache.spark.serializer.KryoSerializer") \
 .getOrCreate()
 inputDf = spark.sql("""{request}""")
 outputDf = inputDf.drop("dbt_unique_key").withColumn("update_hudi_ts",current_timestamp())
 if outputDf.count() > 0:
-        combinedConf = {str(combined_config)}
+        parallelism = spark.conf.get("spark.default.parallelism")
+        print("spark.default.parallelism: %s", parallelism)
+        hudi_parallelism_options = {{
+            "hoodie.upsert.shuffle.parallelism": parallelism,
+            "hoodie.bulkinsert.shuffle.parallelism": parallelism,
+        }}
+        combinedConf = {{**{str(combined_config)}, **hudi_parallelism_options, **{str(hudi_config)}}}
         {self.hudi_write(write_mode, session, target_relation, custom_location)}
 
 spark.sql("""REFRESH TABLE {target_relation.schema}.{target_relation.name}""")
 SqlWrapper2.execute("""SELECT * FROM {target_relation.schema}.{target_relation.name} LIMIT 1""")
         '''
 
         logger.debug(f"""hudi code :
         {code}
         """)
 
         try:
-            cursor.execute(code)
+            session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueHudiMergeTableFailed") from e
         except Exception as e:
             logger.error(e)
     
     def iceberg_create_or_replace_table(self, target_relation, partition_by, table_properties):
         table_properties = self.set_table_properties(table_properties)
@@ -753,15 +760,15 @@
         WHEN MATCHED THEN UPDATE SET *
         WHEN NOT MATCHED THEN INSERT *
         """
         return query
     
     @available
     def iceberg_write(self, target_relation, request, primary_key, partition_key, custom_location, write_mode, table_properties):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         if partition_key is not None:
             partition_key  = '(' + ','.join(partition_key) + ')'
         if custom_location == "empty":
             location = f"{session.credentials.location}/{target_relation.schema}/{target_relation.name}"
         else:
             location = custom_location
         isTableExists = False
@@ -808,28 +815,28 @@
         '''
         code = head_code + core_code + footer_code
         logger.debug(f"""iceberg code :
         {code}
         """)
 
         try:
-            cursor.execute(code)
+            session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueIcebergWriteTableFailed") from e
         except Exception as e:
             logger.error(e)
 
     @available
     def iceberg_expire_snapshots(self, table):
         """
         Helper function to call snapshot expiration.
         The function check for the latest snapshot and it expire all versions before it.
         If the table has only one snapshot it is retained.
         """
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
         logger.debug(f'expiring snapshots for table {str(table)}')
 
         expire_sql = f"CALL glue_catalog.system.expire_snapshots('{str(table)}', timestamp 'to_replace')"
 
         code = f'''
         custom_glue_code_for_dbt_adapter
         history_df = spark.sql("select committed_at from glue_catalog.{table}.snapshots order by committed_at desc")
@@ -838,32 +845,32 @@
         result_df = spark.sql(expire_sql_procedure)
         SqlWrapper2.execute("""SELECT 1""")
         '''
         logger.debug(f"""expire procedure code:
             {code}
             """)
         try:
-            cursor.execute(code)
+            session.cursor().execute(code)
         except DbtDatabaseError as e:
             raise DbtDatabaseError(msg="GlueIcebergExpireSnapshotsFailed") from e
         except Exception as e:
             logger.error(e)
 
     @available
     def execute_pyspark(self, codeblock):
-        session, client, cursor = self.get_connection()
+        session, client = self.get_connection()
 
         code = f"""
 custom_glue_code_for_dbt_adapter
 {codeblock}
         """
 
         logger.debug(f"""pyspark code :
         {code}
         """)
 
         try:
-            cursor.execute(code)
-        except DatabaseException as e:
-            raise DatabaseException(msg="GlueExecutePySparkFailed") from e
+            session.cursor().execute(code)
+        except DbtDatabaseError as e:
+            raise DbtDatabaseError(msg="GlueExecutePySparkFailed") from e
         except Exception as e:
             logger.error(e)
```

### Comparing `dbt-glue-1.4.23/dbt/adapters/glue/relation.py` & `dbt-glue-1.5.0/dbt/adapters/glue/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/adapters.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/incremental.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/incremental/strategies.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/seed.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/snapshot.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/snapshot.sql`

 * *Files 1% similar despite different names*

```diff
@@ -182,15 +182,15 @@
   {% if not target_relation_exists %}
 
     {%- if file_format == 'hudi' -%}
       {%- set partition_by = None -%}
       {%- set custom_location = 'empty' -%}
       {%- set unique_key = 'dbt_scd_id' -%}
       {% set build_sql = build_snapshot_table(strategy, sql) %}
-      {%- set hudi_options = config.get('hudi_options', default={}) -%}
+      {%- set hudi_options = config.get('hudi_options') -%}
       {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options) }}
       {% set final_sql = "select * from " + target_relation.schema + "." + target_relation.identifier %}
     {% elif file_format == 'iceberg'%}
       {%- set partition_by = None -%}
       {%- set custom_location = 'empty' -%}
       {%- set unique_key = 'dbt_scd_id' -%}
       {% set build_sql = build_snapshot_table(strategy, sql | replace("from ", "from glue_catalog.")) %}
@@ -231,15 +231,15 @@
       {% endfor %}
 
     {%- if file_format == 'hudi' -%}
         {%- set partition_by = None -%}
         {%- set custom_location = 'empty' -%}
         {%- set build_sql = "select * from " + staging_table.schema + "." + staging_table.identifier -%}
         {%- set unique_key = 'dbt_scd_id' -%}
-        {%- set hudi_options = config.get('hudi_options', default={}) -%}
+        {%- set hudi_options = config.get('hudi_options') -%}
         {{ adapter.hudi_merge_table(target_relation, build_sql, unique_key, partition_by, custom_location, hudi_options) }}
         {% set final_sql = "select * from " + target_relation.schema + "." + target_relation.identifier %}
       {% elif file_format == 'iceberg' %}
         {%- set partition_by = None -%}
         {%- set custom_location = 'empty' -%}
         {%- set build_sql = "select * from " + staging_table.schema + "." + staging_table.identifier -%}
         {%- set unique_key = 'dbt_scd_id' -%}
```

### Comparing `dbt-glue-1.4.23/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql` & `dbt-glue-1.5.0/dbt/include/glue/macros/materializations/table/iceberg_table_replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt/include/glue/sample_profiles.yml` & `dbt-glue-1.5.0/dbt/include/glue/sample_profiles.yml`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/dbt_glue.egg-info/PKG-INFO` & `dbt-glue-1.5.0/dbt_glue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dbt-glue
-Version: 1.4.23
+Version: 1.5.0
 Summary: dbt (data build tool) adapter for Aws Glue
 Home-page: https://github.com/aws-samples/dbt-glue
 Author: moshirm,menuetb,mamallem,segnina
 Author-email: moshirm@amazon.fr, menuetb@amazon.fr, mamallem@amazon.fr, segnina@amazon.fr 
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 <p align="center">
   <img src="/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
```

### Comparing `dbt-glue-1.4.23/dbt_glue.egg-info/SOURCES.txt` & `dbt-glue-1.5.0/dbt_glue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-glue-1.4.23/setup.py` & `dbt-glue-1.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 import os
 import sys
 
 # require python 3.7 or newer
-if sys.version_info < (3, 7):
+if sys.version_info < (3, 8):
     print('Error: dbt does not support this version of Python.')
-    print('Please upgrade to Python 3.7 or higher.')
+    print('Please upgrade to Python 3.8 or higher.')
     sys.exit(1)
 
 # require version of setuptools that supports find_namespace_packages
 from setuptools import setup
 
 try:
     from setuptools import find_namespace_packages
@@ -34,15 +34,16 @@
             return line.split(delim)[1]
     else:
         raise RuntimeError("Unable to find version string.")
 
 
 package_name = "dbt-glue"
 package_version = get_version("dbt/adapters/glue/__version__.py")
-dbt_version = "1.4.1"
+dbt_version = "1.5.2"
+dbt_spark_version = "1.5.0"
 description = """dbt (data build tool) adapter for Aws Glue"""
 long_description = read('README.md')
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
@@ -61,29 +62,28 @@
             'include/glue/tests/*/*.sql',
             'adapters/glue/*.py',
             'adapters/gluedbapi/*.py',
         ]
     },
     install_requires=[
         "dbt-core~={}".format(dbt_version),
-        "dbt-spark~={}".format(dbt_version),
+        "dbt-spark~={}".format(dbt_spark_version),
         "waiter",
         "boto3"
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 4 - Beta",
 
         'License :: OSI Approved :: Apache Software License',
 
         'Operating System :: Microsoft :: Windows',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX :: Linux',
 
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

