# Comparing `tmp/apidevtools-3.3.6.tar.gz` & `tmp/apidevtools-3.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apidevtools-3.3.6.tar", last modified: Wed Jun 28 23:12:59 2023, max compression
+gzip compressed data, was "apidevtools-3.3.7.tar", last modified: Thu Jun 29 16:30:41 2023, max compression
```

## Comparing `apidevtools-3.3.6.tar` & `apidevtools-3.3.7.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.596740 apidevtools-3.3.6/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3546 2023-06-28 23:12:59.596740 apidevtools-3.3.6/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.6/README.md
--rw-rw-rw-   0        0        0     2185 2023-06-28 23:12:30.000000 apidevtools-3.3.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 23:12:59.596740 apidevtools-3.3.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.528743 apidevtools-3.3.6/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.531741 apidevtools-3.3.6/src/apidevtools/
--rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.6/src/apidevtools/__init__.py
--rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-3.3.6/src/apidevtools/logman.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.557742 apidevtools-3.3.6/src/apidevtools/media/
--rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.6/src/apidevtools/media/ARIALNB.TTF
--rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.6/src/apidevtools/media/__init__.py
--rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.6/src/apidevtools/media/imgproc.py
--rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.6/src/apidevtools/media/telegraph.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.563742 apidevtools-3.3.6/src/apidevtools/orm/
--rw-rw-rw-   0        0        0        0 2023-06-28 21:59:08.000000 apidevtools-3.3.6/src/apidevtools/orm/__init__.py
--rw-rw-rw-   0        0        0     4387 2023-06-28 21:01:25.000000 apidevtools-3.3.6/src/apidevtools/orm/mysql.py
--rw-rw-rw-   0        0        0     4384 2023-06-28 18:25:50.000000 apidevtools-3.3.6/src/apidevtools/orm/postgresql.py
--rw-rw-rw-   0        0        0     3545 2023-06-28 18:26:07.000000 apidevtools-3.3.6/src/apidevtools/orm/sqlite.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.567742 apidevtools-3.3.6/src/apidevtools/orm/types/
--rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-3.3.6/src/apidevtools/orm/types/__init__.py
--rw-rw-rw-   0        0        0     2049 2023-06-28 21:40:46.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_connector.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.575744 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/
--rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/__init__.py
--rw-rw-rw-   0        0        0     2269 2023-06-28 13:56:49.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/_operation.py
--rw-rw-rw-   0        0        0      239 2023-06-27 19:42:54.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/delete.py
--rw-rw-rw-   0        0        0      803 2023-06-27 22:44:17.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/insert.py
--rw-rw-rw-   0        0        0      377 2023-06-27 22:03:36.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/select.py
--rw-rw-rw-   0        0        0      474 2023-06-27 19:52:56.000000 apidevtools-3.3.6/src/apidevtools/orm/types/_operations/update.py
--rw-rw-rw-   0        0        0      446 2023-06-28 10:03:39.000000 apidevtools-3.3.6/src/apidevtools/orm/types/types.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.579741 apidevtools-3.3.6/src/apidevtools/security/
--rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.6/src/apidevtools/security/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.6/src/apidevtools/security/encryptor.py
--rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.6/src/apidevtools/security/hasher.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.584745 apidevtools-3.3.6/src/apidevtools/simpleorm/
--rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.590740 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/
--rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/__init__.py
--rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/_connector.py
--rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/mysql.py
--rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/postgresql.py
--rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/sqlite.py
--rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/orm.py
--rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/redis.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.594740 apidevtools-3.3.6/src/apidevtools/simpleorm/types/
--rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/types/__init__.py
--rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/types/records.py
--rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.6/src/apidevtools/simpleorm/types/schema.py
--rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.6/src/apidevtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-28 23:12:59.551742 apidevtools-3.3.6/src/apidevtools.egg-info/
--rw-rw-rw-   0        0        0     3546 2023-06-28 23:12:59.000000 apidevtools-3.3.6/src/apidevtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1582 2023-06-28 23:12:59.000000 apidevtools-3.3.6/src/apidevtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 23:12:59.000000 apidevtools-3.3.6/src/apidevtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      266 2023-06-28 23:12:59.000000 apidevtools-3.3.6/src/apidevtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-28 23:12:59.000000 apidevtools-3.3.6/src/apidevtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.630603 apidevtools-3.3.7/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 apidevtools-3.3.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3546 2023-06-29 16:30:41.629604 apidevtools-3.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2023-05-15 08:19:30.000000 apidevtools-3.3.7/README.md
+-rw-rw-rw-   0        0        0     2185 2023-06-29 15:56:44.000000 apidevtools-3.3.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-29 16:30:41.630603 apidevtools-3.3.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.590603 apidevtools-3.3.7/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 apidevtools-3.3.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.593603 apidevtools-3.3.7/src/apidevtools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 21:00:17.000000 apidevtools-3.3.7/src/apidevtools/__init__.py
+-rw-rw-rw-   0        0        0      790 2023-06-28 22:51:51.000000 apidevtools-3.3.7/src/apidevtools/logman.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.602604 apidevtools-3.3.7/src/apidevtools/media/
+-rw-rw-rw-   0        0        0   180740 2022-09-11 19:36:12.000000 apidevtools-3.3.7/src/apidevtools/media/ARIALNB.TTF
+-rw-rw-rw-   0        0        0        0 2023-02-27 14:43:20.000000 apidevtools-3.3.7/src/apidevtools/media/__init__.py
+-rw-rw-rw-   0        0        0     2857 2023-05-12 16:00:39.000000 apidevtools-3.3.7/src/apidevtools/media/imgproc.py
+-rw-rw-rw-   0        0        0     1194 2023-05-26 17:06:14.000000 apidevtools-3.3.7/src/apidevtools/media/telegraph.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.606604 apidevtools-3.3.7/src/apidevtools/orm/
+-rw-rw-rw-   0        0        0       65 2023-06-29 15:17:56.000000 apidevtools-3.3.7/src/apidevtools/orm/__init__.py
+-rw-rw-rw-   0        0        0     4353 2023-06-28 23:14:07.000000 apidevtools-3.3.7/src/apidevtools/orm/mysql.py
+-rw-rw-rw-   0        0        0     4350 2023-06-28 23:14:07.000000 apidevtools-3.3.7/src/apidevtools/orm/postgresql.py
+-rw-rw-rw-   0        0        0     3511 2023-06-28 23:14:07.000000 apidevtools-3.3.7/src/apidevtools/orm/sqlite.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.609604 apidevtools-3.3.7/src/apidevtools/orm/types/
+-rw-rw-rw-   0        0        0      157 2023-06-28 10:05:16.000000 apidevtools-3.3.7/src/apidevtools/orm/types/__init__.py
+-rw-rw-rw-   0        0        0     2049 2023-06-28 21:40:46.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_connector.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.615604 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/
+-rw-rw-rw-   0        0        0      154 2023-06-28 10:05:05.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/__init__.py
+-rw-rw-rw-   0        0        0     2269 2023-06-28 13:56:49.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/_operation.py
+-rw-rw-rw-   0        0        0      491 2023-06-29 16:30:07.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/delete.py
+-rw-rw-rw-   0        0        0     1567 2023-06-29 16:20:57.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/insert.py
+-rw-rw-rw-   0        0        0      377 2023-06-27 22:03:36.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/select.py
+-rw-rw-rw-   0        0        0      784 2023-06-29 16:30:07.000000 apidevtools-3.3.7/src/apidevtools/orm/types/_operations/update.py
+-rw-rw-rw-   0        0        0      516 2023-06-29 16:28:13.000000 apidevtools-3.3.7/src/apidevtools/orm/types/types.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.617604 apidevtools-3.3.7/src/apidevtools/security/
+-rw-rw-rw-   0        0        0        0 2023-02-26 16:41:50.000000 apidevtools-3.3.7/src/apidevtools/security/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-05-26 17:50:26.000000 apidevtools-3.3.7/src/apidevtools/security/encryptor.py
+-rw-rw-rw-   0        0        0      778 2023-03-21 01:22:16.000000 apidevtools-3.3.7/src/apidevtools/security/hasher.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.621603 apidevtools-3.3.7/src/apidevtools/simpleorm/
+-rw-rw-rw-   0        0        0       86 2023-03-28 00:28:15.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.625603 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/
+-rw-rw-rw-   0        0        0        0 2023-03-19 23:37:31.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/__init__.py
+-rw-rw-rw-   0        0        0     3317 2023-06-19 22:40:38.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/_connector.py
+-rw-rw-rw-   0        0        0     4781 2023-06-27 19:37:44.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/mysql.py
+-rw-rw-rw-   0        0        0     4434 2023-06-27 19:37:44.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/postgresql.py
+-rw-rw-rw-   0        0        0     3384 2023-06-27 19:38:53.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/sqlite.py
+-rw-rw-rw-   0        0        0     6732 2023-06-21 20:37:26.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/orm.py
+-rw-rw-rw-   0        0        0     2090 2023-05-12 15:05:27.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/redis.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.628603 apidevtools-3.3.7/src/apidevtools/simpleorm/types/
+-rw-rw-rw-   0        0        0       98 2023-03-28 00:37:03.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/types/__init__.py
+-rw-rw-rw-   0        0        0     2656 2023-03-28 01:04:24.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/types/records.py
+-rw-rw-rw-   0        0        0      797 2023-04-16 14:00:00.000000 apidevtools-3.3.7/src/apidevtools/simpleorm/types/schema.py
+-rw-rw-rw-   0        0        0     1120 2023-05-12 15:00:29.000000 apidevtools-3.3.7/src/apidevtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-29 16:30:41.598603 apidevtools-3.3.7/src/apidevtools.egg-info/
+-rw-rw-rw-   0        0        0     3546 2023-06-29 16:30:41.000000 apidevtools-3.3.7/src/apidevtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1582 2023-06-29 16:30:41.000000 apidevtools-3.3.7/src/apidevtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-29 16:30:41.000000 apidevtools-3.3.7/src/apidevtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      266 2023-06-29 16:30:41.000000 apidevtools-3.3.7/src/apidevtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-29 16:30:41.000000 apidevtools-3.3.7/src/apidevtools.egg-info/top_level.txt
```

### Comparing `apidevtools-3.3.6/LICENSE.txt` & `apidevtools-3.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/PKG-INFO` & `apidevtools-3.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.6
+Version: 3.3.7
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.6/README.md` & `apidevtools-3.3.7/README.md`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/pyproject.toml` & `apidevtools-3.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apidevtools"
-version = "3.3.6"
+version = "3.3.7"
 authors = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 maintainers = [{ name="cxllmerichie", email="cxllmerichie@gmail.com" }, ]
 description = "All in one tools for API development."
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `apidevtools-3.3.6/src/apidevtools/logman.py` & `apidevtools-3.3.7/src/apidevtools/logman.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/media/ARIALNB.TTF` & `apidevtools-3.3.7/src/apidevtools/media/ARIALNB.TTF`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/media/imgproc.py` & `apidevtools-3.3.7/src/apidevtools/media/imgproc.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/media/telegraph.py` & `apidevtools-3.3.7/src/apidevtools/media/telegraph.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/orm/mysql.py` & `apidevtools-3.3.7/src/apidevtools/orm/mysql.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,24 @@
         self.pool: aiomysql.Pool | None = None
 
     async def create_pool(self) -> bool:
         try:
             self.pool = await aiomysql.create_pool(
                 db=self.database, host=self.host, port=self.port, user=self.user, password=self.password
             )
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool created')
+            self.logger.info(f'{self.__class__.__name__} pool created')
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def close_pool(self) -> bool:
         try:
             self.pool.close()
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool closed')
+            self.logger.info(f'{self.__class__.__name__} pool closed')
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     # @cache
     # async def columns(self, tablename: str) -> list[str]:
```

### Comparing `apidevtools-3.3.6/src/apidevtools/orm/postgresql.py` & `apidevtools-3.3.7/src/apidevtools/orm/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,25 +23,25 @@
         self.pool: asyncpg.pool.Pool | None = None
 
     async def create_pool(self):
         try:
             self.pool = await asyncpg.pool.create_pool(
                 database=self.database, host=self.host, port=self.port, user=self.user, password=self.password
             )
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool created')
+            self.logger.info(f'{self.__class__.__name__} pool created')
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def close_pool(self) -> bool:
         try:
             await self.pool.expire_connections()
             await self.pool.close()
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool created')
+            self.logger.info(f'{self.__class__.__name__} pool created')
             return True
         except AttributeError:
             self.logger.error(f'Attempting to close not acquired pool')
             return False
 
     # @cache
     # async def columns(self, tablename: str) -> list[str]:
```

### Comparing `apidevtools-3.3.6/src/apidevtools/orm/sqlite.py` & `apidevtools-3.3.7/src/apidevtools/orm/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,24 @@
         self.logger: logman.Logger = logger
         self.pool: aiosqlite.Connection | None = None
 
     async def create_pool(self) -> bool:
         try:
             self.pool = await aiosqlite.connect(database=self.database)
             self.pool.row_factory = aiosqlite.Row
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool created')
+            self.logger.info(f'{self.__class__.__name__} pool created')
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     async def close_pool(self) -> bool:
         try:
             await self.pool.close()
-            self.logger.info(f'`ORM.connector: {self.__class__.__name__}` pool closed')
+            self.logger.info(f'{self.__class__.__name__} pool closed')
             return True
         except Exception as error:
             self.logger.error(error)
             return False
 
     # @cache
     # async def columns(self, tablename: str) -> list[str]:
```

### Comparing `apidevtools-3.3.6/src/apidevtools/orm/types/_connector.py` & `apidevtools-3.3.7/src/apidevtools/orm/types/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/orm/types/_operations/_operation.py` & `apidevtools-3.3.7/src/apidevtools/orm/types/_operations/_operation.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/security/encryptor.py` & `apidevtools-3.3.7/src/apidevtools/security/encryptor.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/security/hasher.py` & `apidevtools-3.3.7/src/apidevtools/security/hasher.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/_connector.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/_connector.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/mysql.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/postgresql.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/postgresql.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/connectors/sqlite.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/connectors/sqlite.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/orm.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/orm.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/redis.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/redis.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/types/records.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/types/records.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/simpleorm/types/schema.py` & `apidevtools-3.3.7/src/apidevtools/simpleorm/types/schema.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools/utils.py` & `apidevtools-3.3.7/src/apidevtools/utils.py`

 * *Files identical despite different names*

### Comparing `apidevtools-3.3.6/src/apidevtools.egg-info/PKG-INFO` & `apidevtools-3.3.7/src/apidevtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apidevtools
-Version: 3.3.6
+Version: 3.3.7
 Summary: All in one tools for API development.
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
```

### Comparing `apidevtools-3.3.6/src/apidevtools.egg-info/SOURCES.txt` & `apidevtools-3.3.7/src/apidevtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

