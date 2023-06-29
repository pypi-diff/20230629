# Comparing `tmp/apidevtools-3.3.8.tar.gz` & `tmp/apidevtools-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.3.8.tar", last modified: Thu Jun 29 19:24:54 2023, max compression
+gzip compressed data, was "apidevtools-3.3.9.tar", last modified: Thu Jun 29 21:14:40 2023, max compression
```

## Comparing `apidevtools-3.3.8.tar` & `apidevtools-3.3.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.581557 apidevtools-3.3.8/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.8/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-06-29 19:24:54.580582 apidevtools-3.3.8/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.8/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-29 19:24:38.000000 apidevtools-3.3.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 19:24:54.581557 apidevtools-3.3.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.542558 apidevtools-3.3.8/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.8/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.545557 apidevtools-3.3.8/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.8/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-3.3.8/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.555559 apidevtools-3.3.8/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.8/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.8/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.8/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.8/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.558558 apidevtools-3.3.8/src/apidevtools/orm/
--rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-3.3.8/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4353 2023-06-28 23:14:07.000000 apidevtools-3.3.8/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-3.3.8/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-3.3.8/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.561558 apidevtools-3.3.8/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-3.3.8/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2049 2023-06-28 21:40:46.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.566567 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2297 2023-06-29 18:55:11.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      491 2023-06-29 16:30:07.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0     1581 2023-06-29 18:55:35.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      385 2023-06-29 18:55:37.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      894 2023-06-29 18:54:29.000000 apidevtools-3.3.8/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-3.3.8/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.569558 apidevtools-3.3.8/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.8/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.8/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.8/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.571558 apidevtools-3.3.8/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.576572 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.579571 apidevtools-3.3.8/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.8/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.8/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-29 19:24:54.550558 apidevtools-3.3.8/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-06-29 19:24:54.000000 apidevtools-3.3.8/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-06-29 19:24:54.000000 apidevtools-3.3.8/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 19:24:54.000000 apidevtools-3.3.8/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-06-29 19:24:54.000000 apidevtools-3.3.8/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-29 19:24:54.000000 apidevtools-3.3.8/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.932526 apidevtools-3.3.9/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-06-29 21:14:40.931527 apidevtools-3.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.9/README.md
+-rw-rw-rw-   0        0        0     2185 2023-06-29 21:14:26.000000 apidevtools-3.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 21:14:40.932526 apidevtools-3.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.899552 apidevtools-3.3.9/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.9/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.902551 apidevtools-3.3.9/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.9/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-3.3.9/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.909527 apidevtools-3.3.9/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.9/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.9/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.9/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.9/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.912527 apidevtools-3.3.9/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-3.3.9/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4353 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-3.3.9/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.915528 apidevtools-3.3.9/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-3.3.9/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2049 2023-06-28 21:40:46.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.919527 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2297 2023-06-29 18:55:11.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      491 2023-06-29 16:30:07.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1581 2023-06-29 18:55:35.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      385 2023-06-29 18:55:37.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      885 2023-06-29 20:52:22.000000 apidevtools-3.3.9/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-3.3.9/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.922527 apidevtools-3.3.9/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.9/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.9/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.9/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.924527 apidevtools-3.3.9/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.928527 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.930527 apidevtools-3.3.9/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.9/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.9/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 21:14:40.906527 apidevtools-3.3.9/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-29 21:14:40.000000 apidevtools-3.3.9/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.3.8/LICENSE.txt` & `apidevtools-3.3.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/PKG-INFO` & `apidevtools-3.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.8
+Version: 3.3.9
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.8/README.md` & `apidevtools-3.3.9/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/pyproject.toml` & `apidevtools-3.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.3.8"
+version = "3.3.9"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-3.3.8/src/apidevtools/logman.py` & `apidevtools-3.3.9/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.3.9/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/media/imgproc.py` & `apidevtools-3.3.9/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/media/telegraph.py` & `apidevtools-3.3.9/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/mysql.py` & `apidevtools-3.3.9/src/apidevtools/orm/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/postgresql.py` & `apidevtools-3.3.9/src/apidevtools/orm/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/sqlite.py` & `apidevtools-3.3.9/src/apidevtools/orm/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/types/_connector.py` & `apidevtools-3.3.9/src/apidevtools/orm/types/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-3.3.9/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/types/_operations/insert.py` & `apidevtools-3.3.9/src/apidevtools/orm/types/_operations/insert.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/types/_operations/update.py` & `apidevtools-3.3.9/src/apidevtools/orm/types/_operations/update.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from typing import Any
 
 from ._operation import Operation
 from ..types import Schema, Record
 
 
 class Update(Operation):
-    def update(self, table: str, instance: Record = None) -> 'Update':
+    def update(self, what: Record | str) -> 'Update':
         self._refresh()
-        if instance:
-            if isinstance(instance, Schema):
-                self.update(instance.__tablename__)
-                self.set(**dict(instance))
-                key = instance.__primary__
-                self.where(**{key: instance.__getattribute__(key)})
-            return self
-        self._query = f"UPDATE {table} "
+        if isinstance(what, Schema):
+            self.update(what.__tablename__)
+            self.set(**dict(what))
+            key = what.__primary__
+            self.where(**{key: what.__getattribute__(key)})
+        elif isinstance(what, dict):
+            ...
+        elif isinstance(what, str):
+            self._query = f"UPDATE {what} "
         return self
 
     def set(self, **values: Any) -> 'Update':
         self._qargs += values.values()
         p, c = self._placeholder, self._constraint_wrapper  # noqa
         values = ', '.join([f'{c}{key}{c} = {p}' for key, value in values.items()])
         self._query += f"SET {values} "
```

### Comparing `apidevtools-3.3.8/src/apidevtools/orm/types/types.py` & `apidevtools-3.3.9/src/apidevtools/orm/types/types.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/security/encryptor.py` & `apidevtools-3.3.9/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/security/hasher.py` & `apidevtools-3.3.9/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.3.9/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools/utils.py` & `apidevtools-3.3.9/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.8/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.3.9/src/apidevtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.8
+Version: 3.3.9
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.8/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.3.9/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

