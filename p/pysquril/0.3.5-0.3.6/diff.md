# Comparing `tmp/pysquril-0.3.5.tar.gz` & `tmp/pysquril-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysquril-0.3.5.tar", max compression
+gzip compressed data, was "pysquril-0.3.6.tar", max compression
```

## Comparing `pysquril-0.3.5.tar` & `pysquril-0.3.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      168 2023-06-28 09:44:50.951276 pysquril-0.3.5/README.md
--rw-r--r--   0        0        0      545 2023-06-28 09:44:50.951276 pysquril-0.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/__init__.py
--rw-r--r--   0        0        0    25536 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/backends.py
--rw-r--r--   0        0        0      326 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/exc.py
--rw-r--r--   0        0        0    21254 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/generator.py
--rw-r--r--   0        0        0     9570 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/parser.py
--rw-r--r--   0        0        0     1997 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/test_data.py
--rw-r--r--   0        0        0    21714 2023-06-28 09:44:50.951276 pysquril-0.3.5/pysquril/tests.py
--rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 pysquril-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      168 2023-06-29 11:34:48.653520 pysquril-0.3.6/README.md
+-rw-r--r--   0        0        0      545 2023-06-29 11:34:48.653520 pysquril-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/__init__.py
+-rw-r--r--   0        0        0    25761 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/backends.py
+-rw-r--r--   0        0        0      326 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/exc.py
+-rw-r--r--   0        0        0    21376 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/generator.py
+-rw-r--r--   0        0        0     9895 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/parser.py
+-rw-r--r--   0        0        0     1997 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/test_data.py
+-rw-r--r--   0        0        0    22448 2023-06-29 11:34:48.653520 pysquril-0.3.6/pysquril/tests.py
+-rw-r--r--   0        0        0      868 1970-01-01 00:00:00.000000 pysquril-0.3.6/PKG-INFO
```

### Comparing `pysquril-0.3.5/pyproject.toml` & `pysquril-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysquril"
-version = "0.3.5"
+version = "0.3.6"
 description = "Python implementation of structured URI query language"
 readme = "README.md"
 repository = "https://github.com/unioslo/pysquril"
 authors = [
     "Leon du Toit <l.c.d.toit@usit.uio.no>",
     "Eirik Haatveit <haatveit@uio.no>",
 ]
```

### Comparing `pysquril-0.3.5/pysquril/backends.py` & `pysquril-0.3.6/pysquril/backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import sqlite3
 
 from abc import ABC, abstractmethod
 from contextlib import contextmanager
 from typing import Union, ContextManager, Iterable, Optional, Any, Callable
+from urllib.parse import unquote
 from uuid import uuid4
 
 import psycopg2
 import psycopg2.extensions
 import psycopg2.pool
 
 from pysquril.exc import DataIntegrityError, ParseError
@@ -53,36 +54,39 @@
 
 
 class AuditTransaction(object):
 
     """
     Container for generating audit events.
     Keeps state for transaction IDs, generates
-    timestamps, and event IDs.
+    timestamps, and event IDs, propagates
+    audit messages.
 
     """
 
-    def __init__(self, identity: str) -> None:
+    def __init__(self, identity: str, message: Optional[str] = "") -> None:
         self.identity = identity
         self.timestamp = datetime.datetime.now().isoformat()
         self.transaction_id = self._id()
+        self.message = message
 
     def _id(self) -> str:
         return str(uuid4())
 
     def _event(self, diff: Any, previous: Any, event: str, query: str) -> dict:
         return {
             "diff": diff,
             "previous": previous,
             "event": event,
             "timestamp": self.timestamp,
             "identity": self.identity,
             "event_id": self._id(),
             "transaction_id": self.transaction_id,
             "query": query,
+            "message": self.message,
         }
 
     def event_update(self, *, diff: Any, previous: Any, query: str) -> dict:
         return self._event(diff, previous, "update", query)
 
     def event_delete(self, *, diff: Any, previous: Any, query: str) -> dict:
         return self._event(diff, previous, "delete", query)
@@ -231,23 +235,23 @@
         work_done = {"restores": [], "updates": []}
         # ensure we have enough information
         query_parts = uri_query.split("&")
         if not query_parts:
             raise ParseError("Missing query")
         if "restore" not in query_parts:
             raise ParseError("Missing restore directive")
+        has_pk = False
+        message = ""
         for part in query_parts:
-            has_pk = False
-            if part.startswith("primary_key"):
+            if part.startswith("primary_key="):
                 primary_key = part.split("=")[-1]
-                if primary_key == "":
-                    raise ParseError("Missing primary_key value")
-                else:
+                if primary_key != "":
                     has_pk = True
-                    break
+            if part.startswith("message="):
+                message = unquote(part.split("=")[-1])
         if not has_pk:
             raise ParseError("Missing primary_key")
         # fetch a copy of the current state, and all primay keys
         table_exists = False
         try:
             current_data = list(self.table_select(table_name, ""))
             current_pks = list(self.table_select(table_name, f"select={primary_key}"))
@@ -258,15 +262,15 @@
         # fetch the desired state
         if "order" in query_parts:
             uri_query = uri_query.split("&order")[0]
         uri_query = f"{uri_query}&order=timestamp.asc" # sorted from old to new
         target_data = list(self.table_select(f"{table_name}_audit", uri_query))
         if not target_data:
             return work_done # nothing to do
-        tsc = AuditTransaction(self.requestor)
+        tsc = AuditTransaction(self.requestor, message)
         session_func = self._session_func()
         try:
             # ensure the table exists, may have been deleted
             with session_func(self.engine) as session:
                 self.table_create(table_name, session)
         except psycopg2.errors.DuplicateObject as e:
             pass # already exists
@@ -447,33 +451,33 @@
         table_name: str,
         uri_query: str,
         data: dict,
         tsc: Optional[AuditTransaction] = None,
         session: Optional[sqlite3.Cursor] = None,
     ) -> bool:
         audit_data = []
-        tsc = AuditTransaction(self.requestor) if not tsc else tsc
+        sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query, data=data)
+        tsc = AuditTransaction(self.requestor, sql.message) if not tsc else tsc
         for val in self.table_select(table_name, uri_query, data=data):
             audit_data.append(tsc.event_update(diff=data, previous=val, query=uri_query))
-        sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query, data=data)
         if session:
             session.execute(sql.update_query)
             self.table_insert(f'{table_name}_audit', audit_data, session)
         else:
             with sqlite_session(self.engine) as session:
                 session.execute(sql.update_query)
             self.table_insert(f'{table_name}_audit', audit_data)
         return True
 
     def table_delete(self, table_name: str, uri_query: str) -> bool:
         audit_data = []
-        tsc = AuditTransaction(self.requestor)
+        sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query)
+        tsc = AuditTransaction(self.requestor, sql.message)
         for row in self.table_select(table_name, uri_query):
             audit_data.append(tsc.event_delete(diff=None, previous=row, query=uri_query))
-        sql = self.generator_class(f'"{self.schema}{self.sep}{table_name}"', uri_query)
         with sqlite_session(self.engine) as session:
             session.execute(sql.delete_query)
             if not table_name.endswith("_audit"):
                 self.table_create(f'{table_name}_audit', session)
                 self.table_insert(f'{table_name}_audit', audit_data, session)
         return True
 
@@ -635,33 +639,33 @@
         table_name: str,
         uri_query: str,
         data: dict,
         tsc: Optional[AuditTransaction] = None,
         session: Optional[psycopg2.extensions.cursor] = None,
     ) -> bool:
         audit_data = []
-        tsc = AuditTransaction(self.requestor) if not tsc else tsc
+        sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query, data=data)
+        tsc = AuditTransaction(self.requestor, sql.message) if not tsc else tsc
         for val in self.table_select(table_name, uri_query, data=data):
             audit_data.append(tsc.event_update(diff=data, previous=val, query=uri_query))
-        sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query, data=data)
         if session:
             session.execute(sql.update_query)
             self.table_insert(f'{table_name}_audit', audit_data, session)
         else:
             with postgres_session(self.engine) as session:
                 session.execute(sql.update_query)
             self.table_insert(f'{table_name}_audit', audit_data)
         return True
 
     def table_delete(self, table_name: str, uri_query: str) -> bool:
         audit_data = []
-        tsc = AuditTransaction(self.requestor)
+        sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query)
+        tsc = AuditTransaction(self.requestor, sql.message)
         for row in self.table_select(table_name, uri_query):
             audit_data.append(tsc.event_delete(diff=None, previous=row, query=uri_query))
-        sql = self.generator_class(f'{self.schema}{self.sep}"{table_name}"', uri_query)
         with postgres_session(self.engine) as session:
             session.execute(sql.delete_query)
             if not table_name.endswith("_audit"):
                 self.table_create(f'{table_name}_audit', session)
                 self.table_insert(f'{table_name}_audit', audit_data, session)
         return True
```

### Comparing `pysquril-0.3.5/pysquril/generator.py` & `pysquril-0.3.6/pysquril/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,15 @@
         }
         if not self.json_array_sql:
             msg = 'Extending the SqlGenerator requires setting the class level property: json_array_sql'
             raise Exception(msg)
         self.select_query = self.sql_select()
         self.update_query = self.sql_update()
         self.delete_query = self.sql_delete()
+        self.message = self.uri_message()
 
     # Classes that extend the SqlGenerator must implement the following methods
     # they are called by functions that are mapped over terms in clauses
     # for each term, an appropriate piece of SQL needs to be returned.
     # What is appropriate, depends on the backend.
 
     def _gen_sql_key_selection(self, term: SelectTerm, parsed: Key) -> str:
@@ -317,14 +318,17 @@
         _where = self._gen_sql_where_clause()
         if not _where:
             query = f"drop table {self.table_name}"
         else:
             query = f"delete from {self.table_name} {_where}"
         return query
 
+    def uri_message(self) -> str:
+        return self.parsed_uri_query.message
+
 
 class SqliteQueryGenerator(SqlGenerator):
 
     """Generate SQL for SQLite json1 backed tables, from a given UriQuery."""
 
     db_init_sql = None
     json_array_sql = 'json_array'
```

### Comparing `pysquril-0.3.5/pysquril/parser.py` & `pysquril-0.3.6/pysquril/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 """SQURIL - Structured Query URI Language."""
 
 import json
 import re
 
 from abc import ABC, abstractmethod
 from typing import Optional, Union, Callable
+from urllib.parse import unquote
 
 from pysquril.exc import ParseError
 
 class SelectElement(ABC):
     @property
     @abstractmethod
     def name(self) -> str:
@@ -321,14 +322,23 @@
         self.original = uri_query
         self.data = data
         self.select = self.parse_clause(prefix='select=', Cls=SelectClause)
         self.where = self.parse_clause(prefix='where=', Cls=WhereClause)
         self.order = self.parse_clause(prefix='order=', Cls=OrderClause)
         self.range = self.parse_clause(prefix='range=', Cls=RangeClause)
         self.set = self.parse_clause(prefix='set=', Cls=SetClause)
+        self.message = self.parse_message()
+
+    def parse_message(self) -> str:
+        message = ""
+        parts = self.original.split("&")
+        for part in parts:
+            if part.startswith("message="):
+                message = unquote(part.split("=")[-1])
+        return message
 
     def parse_clause(self, *, prefix: str, Cls: Clause) -> Clause:
         if not prefix:
             raise Exception('prefix not specified')
         if not Cls:
             raise Exception('Cls not specified')
         parts = self.original.split('&')
```

### Comparing `pysquril-0.3.5/pysquril/test_data.py` & `pysquril-0.3.6/pysquril/test_data.py`

 * *Files identical despite different names*

### Comparing `pysquril-0.3.5/pysquril/tests.py` & `pysquril-0.3.6/pysquril/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import os
 import sqlite3
 import unittest
 import tempfile
 
 from typing import Callable, Union
+from urllib.parse import quote
 
 import psycopg2
 import psycopg2.errors
 import psycopg2.extensions
 import psycopg2.pool
 import pytest
 
@@ -397,18 +398,19 @@
         more_data = {pkey: 2, key_to_update: original_value, "key3": {"moar": "things"}}
 
         self.backend.table_insert(table_name=test_table, data=data)
         self.backend.table_insert(table_name=test_table, data=more_data)
 
         # update the table with the new data
         new_data = {key_to_update: original_value+1}
+        message = "all the messages"
 
         self.backend.table_update(
             table_name=test_table,
-            uri_query=f"set={key_to_update}&where={key_to_update}=eq.{original_value}",
+            uri_query=f"set={key_to_update}&where={key_to_update}=eq.{original_value}&message={quote(message)}",
             data=new_data,
         )
         result = list(self.backend.table_select(table_name=test_table, uri_query=""))
         self.assertTrue(result)
         retrieved_data = result[0]
         self.assertEqual(retrieved_data, {**data, **new_data})
         self.assertNotEqual(retrieved_data[key_to_update], original_value)
@@ -423,37 +425,51 @@
         self.assertEqual(audit_event["previous"], data)
         self.assertEqual(audit_event["diff"], new_data)
         self.assertEqual(audit_event["event"], "update")
         self.assertTrue(audit_event["transaction_id"] is not None)
         self.assertTrue(audit_event["event_id"] is not None)
         self.assertTrue(audit_event["timestamp"] is not None)
         self.assertTrue(audit_event["query"] is not None)
+        self.assertEqual(audit_event["message"], message)
 
         # restore updates
         with self.assertRaises(ParseError): # missing restore directive
             self.backend.table_restore(table_name=test_table, uri_query="")
         with self.assertRaises(ParseError): # missing primary key
             self.backend.table_restore(table_name=test_table, uri_query="restore")
         with self.assertRaises(ParseError): # still missing primary key
             self.backend.table_restore(table_name=test_table, uri_query="restore&primary_key=")
 
         # restore to a specific state, for a specific row
+        message = "undoing mistakes"
         result = self.backend.table_restore(
             table_name=test_table,
-            uri_query=f"restore&primary_key={pkey}&where=event_id=eq.{audit_event.get('event_id')}"
+            uri_query=f"restore&primary_key={pkey}&where=event_id=eq.{audit_event.get('event_id')}&message={quote(message)}"
         )
         self.assertEqual(len(result.get("updates")), 1)
         self.assertEqual(len(result.get("restores")), 0)
         result = list(self.backend.table_select(table_name=test_table, uri_query="where=id=eq.1"))
         self.assertEqual(result[0].get(key_to_update), original_value)
+        result = list(self.backend.table_select(
+            table_name=f"{test_table}_audit", uri_query="order=timestamp.desc")
+        )
+        self.assertEqual(result[0].get("message"), message)
 
         # delete a specific entry
-        self.backend.table_delete(table_name=test_table, uri_query="where=key3=not.is.null")
+        message = "bad data: must delete, & never repeat (tm)"
+        self.backend.table_delete(
+            table_name=test_table,
+            uri_query=f"where=key3=not.is.null&message={quote(message)}"
+        )
         result = list(self.backend.table_select(table_name=f"{test_table}_audit", uri_query=""))
         self.assertEqual(len(result), 4)
+        result = list(self.backend.table_select(
+            table_name=f"{test_table}_audit", uri_query="order=timestamp.desc")
+        )
+        self.assertEqual(result[0].get("message"), message)
 
         # restore the deleted entry
         result = self.backend.table_restore(
             table_name=test_table,
             uri_query=f"restore&primary_key={pkey}&where=event=eq.delete"
         )
         self.assertEqual(len(result.get("updates")), 0)
```

### Comparing `pysquril-0.3.5/PKG-INFO` & `pysquril-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysquril
-Version: 0.3.5
+Version: 0.3.6
 Summary: Python implementation of structured URI query language
 Home-page: https://github.com/unioslo/pysquril
 Author: Leon du Toit
 Author-email: l.c.d.toit@usit.uio.no
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

