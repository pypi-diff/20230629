# Comparing `tmp/greyhorse_sqla-0.3.tar.gz` & `tmp/greyhorse_sqla-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "greyhorse_sqla-0.3.tar", max compression
+gzip compressed data, was "greyhorse_sqla-0.3.1.tar", max compression
```

## Comparing `greyhorse_sqla-0.3.tar` & `greyhorse_sqla-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       96 2023-05-06 23:35:23.266980 greyhorse_sqla-0.3/greyhorse_sqla/__init__.py
--rw-r--r--   0        0        0     3254 2023-04-26 11:42:15.504046 greyhorse_sqla-0.3/greyhorse_sqla/config.py
--rw-r--r--   0        0        0     4767 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/containers.py
--rw-r--r--   0        0        0     3270 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/contexts.py
--rw-r--r--   0        0        0     5425 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/engine.py
--rw-r--r--   0        0        0     5138 2023-05-06 23:38:34.861859 greyhorse_sqla-0.3/greyhorse_sqla/factory.py
--rw-r--r--   0        0        0        0 2023-06-26 23:41:57.934035 greyhorse_sqla-0.3/greyhorse_sqla/migration/__init__.py
--rw-r--r--   0        0        0     2281 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/app.py
--rw-r--r--   0        0        0     2121 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/cmd.py
--rw-r--r--   0        0        0      440 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/containers.py
--rw-r--r--   0        0        0     4973 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/operator.py
--rw-r--r--   0        0        0     1559 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/migration/utils.py
--rw-r--r--   0        0        0     3161 2023-06-26 23:41:57.938035 greyhorse_sqla-0.3/greyhorse_sqla/model.py
--rw-r--r--   0        0        0     1422 2023-05-06 20:57:55.966776 greyhorse_sqla-0.3/greyhorse_sqla/query.py
--rw-r--r--   0        0        0    13404 2023-06-26 23:41:57.942035 greyhorse_sqla-0.3/greyhorse_sqla/repository.py
--rw-r--r--   0        0        0     5876 2023-06-26 23:41:57.942035 greyhorse_sqla-0.3/greyhorse_sqla/resources.py
--rw-r--r--   0        0        0      237 2023-05-06 23:37:41.048322 greyhorse_sqla-0.3/greyhorse_sqla/translations.toml
--rw-r--r--   0        0        0     1444 2023-06-26 23:41:57.958034 greyhorse_sqla-0.3/pyproject.toml
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 greyhorse_sqla-0.3/PKG-INFO
+-rw-r--r--   0        0        0       96 2023-05-30 11:55:28.473575 greyhorse_sqla-0.3.1/greyhorse_sqla/__init__.py
+-rw-r--r--   0        0        0     3234 2023-06-28 20:12:22.760341 greyhorse_sqla-0.3.1/greyhorse_sqla/config.py
+-rw-r--r--   0        0        0     4769 2023-06-28 20:12:22.596346 greyhorse_sqla-0.3.1/greyhorse_sqla/containers.py
+-rw-r--r--   0        0        0     3596 2023-06-28 20:12:22.712343 greyhorse_sqla-0.3.1/greyhorse_sqla/contexts.py
+-rw-r--r--   0        0        0     5425 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/engine.py
+-rw-r--r--   0        0        0     5138 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/factory.py
+-rw-r--r--   0        0        0        0 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/app.py
+-rw-r--r--   0        0        0     2121 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/cmd.py
+-rw-r--r--   0        0        0      440 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/containers.py
+-rw-r--r--   0        0        0     4973 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/operator.py
+-rw-r--r--   0        0        0     1559 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/migration/utils.py
+-rw-r--r--   0        0        0     3161 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/model.py
+-rw-r--r--   0        0        0     1422 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/query.py
+-rw-r--r--   0        0        0    13404 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/repository.py
+-rw-r--r--   0        0        0     5876 2023-06-28 15:45:30.033860 greyhorse_sqla-0.3.1/greyhorse_sqla/resources.py
+-rw-r--r--   0        0        0      237 2023-05-30 11:55:28.477575 greyhorse_sqla-0.3.1/greyhorse_sqla/translations.toml
+-rw-r--r--   0        0        0     1446 2023-06-28 20:11:23.522317 greyhorse_sqla-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 greyhorse_sqla-0.3.1/PKG-INFO
```

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/config.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 
-from pydantic import validator, BaseSettings, PostgresDsn
+from pydantic import BaseSettings, PostgresDsn, validator
 
 
 @dataclass
 class EngineConfig:
     dsn: str
     echo: bool = False
     pool_min_size: int = 1
@@ -50,15 +50,15 @@
     POSTGRES_PASSWORD_FILE: Path | None = None
     POSTGRES_DB: str
     POSTGRES_SCHEMA: str | None = None
 
     DATABASE_URI: PostgresDsn | None = None
 
     @validator('DATABASE_URI', pre=True)
-    def assemble_db_connection(cls, v: str | None, values: dict[str, Any]) -> str:
+    def assemble_dsn(cls, v: str | None, values: dict[str, Any]) -> str:
         if isinstance(v, str):
             return v
 
         if 'POSTGRES_PASSWORD_FILE' in values:
             password_file = values.get('POSTGRES_PASSWORD_FILE')
             if isinstance(password_file, Path) and password_file.exists():
                 with password_file.open() as f:
@@ -85,15 +85,15 @@
     MYSQL_PASSWORD: str = ''
     MYSQL_PASSWORD_FILE: Path | None = None
     MYSQL_DB: str
 
     DATABASE_URI: str | None = None
 
     @validator('DATABASE_URI', pre=True)
-    def assemble_db_connection(cls, v: str | None, values: dict[str, Any]) -> str:
+    def assemble_dsn(cls, v: str | None, values: dict[str, Any]) -> str:
         if isinstance(v, str):
             return v
 
         if 'MYSQL_PASSWORD_FILE' in values:
             password_file = values.get('MYSQL_PASSWORD_FILE')
             if isinstance(password_file, Path) and password_file.exists():
                 with password_file.open() as f:
```

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/containers.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from dependency_injector import containers, providers
 
 from greyhorse_core.utils.confs import default_value
 from greyhorse_sqla.config import EngineConfig, SqlEngineType
-from greyhorse_sqla.contexts import SqlaSyncContext, SqlaAsyncContext
-from greyhorse_sqla.factory import SqlaSyncEngineFactory, SqlaAsyncEngineFactory
-from greyhorse_sqla.resources import SqlaSyncResource, SqlaAsyncResource
+from greyhorse_sqla.contexts import SqlaAsyncContext, SqlaSyncContext
+from greyhorse_sqla.factory import SqlaAsyncEngineFactory, SqlaSyncEngineFactory
+from greyhorse_sqla.resources import SqlaAsyncResource, SqlaSyncResource
 
 
 def _prepare_single_engine_config(config, factory):
     if isinstance(config.engine_config(), EngineConfig):
         engine_config = config.engine_config()
     else:
         engine_config = EngineConfig(
@@ -17,15 +17,15 @@
             pool_min_size=config.engine_config.
                 pool_min_size.as_(default_value(int))(default=1),
             pool_max_size=config.engine_config.
                 pool_max_size.as_(default_value(int))(default=8),
             pool_expire_seconds=config.engine_config.
                 pool_expire_seconds.as_(default_value(int))(default=60),
             pool_timeout_seconds=config.engine_config.
-                pool_timeout_seconds.as_(default_value(int))(default=15)
+                pool_timeout_seconds.as_(default_value(int))(default=15),
         )
     return factory(name=config.name(), config=engine_config, db_type=config.db_type())
 
 
 def _prepare_multiple_engine_config(name: str, config, factory):
     if conf := config.get(name):
         if isinstance(conf['engine_config'], EngineConfig):
@@ -33,15 +33,15 @@
         else:
             engine_config = EngineConfig(
                 dsn=conf['engine_config']['dsn'],
                 echo=bool(conf['engine_config'].get('echo')),
                 pool_min_size=int(conf['engine_config'].get('pool_min_size', 1)),
                 pool_max_size=int(conf['engine_config'].get('pool_max_size', 8)),
                 pool_expire_seconds=int(conf['engine_config'].get('pool_expire_seconds', 60)),
-                pool_timeout_seconds=int(conf['engine_config'].get('pool_timeout_seconds', 15))
+                pool_timeout_seconds=int(conf['engine_config'].get('pool_timeout_seconds', 15)),
             )
         return factory(name=name, config=engine_config, db_type=conf['db_type'])
 
     return None
 
 
 class SqlaSyncContainer(containers.DeclarativeContainer):
```

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/contexts.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/contexts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,128 +1,136 @@
 import asyncio
 import threading
-from contextlib import contextmanager, asynccontextmanager
+from contextlib import asynccontextmanager, contextmanager
 from typing import Callable
 
 from sqlalchemy import exc
+from sqlalchemy.ext.asyncio import AsyncSession as SqlaAsyncSession
+from sqlalchemy.orm import Session as SqlaSyncSession
 
-from greyhorse_sqla.engine import SqlaSyncEngine, SqlaAsyncEngine
+from greyhorse_sqla.engine import SqlaAsyncEngine, SqlaSyncEngine
 
 
 class SqlaSyncContext:
-    def __init__(
-        self, sqla_engine: SqlaSyncEngine, force_rollback: bool = True,
-    ):
-        self._sqla_engine = sqla_engine
+    def __init__(self, engine: SqlaSyncEngine, force_rollback: bool = True):
+        self._engine = engine
         self._force_rollback = force_rollback
         self._counter = 0
         self._lock = threading.Lock()
+        self._session: SqlaSyncSession | None = None
 
     @property
     def name(self) -> str:
-        return self._sqla_engine.name
+        return self._engine.name
+
+    @property
+    def engine(self) -> SqlaSyncEngine:
+        return self._engine
 
     @contextmanager
     def session_factory(self):
-        yield self.session
+        yield self._session
 
     def commit(self):
-        self.session.commit()
+        self._session.commit()
 
     def rollback(self):
-        self.session.rollback()
+        self._session.rollback()
 
-    def setup(self):
+    def _setup(self):
         pass
 
-    def teardown(self):
+    def _teardown(self):
         pass
 
     def __enter__(self):
         with self._lock:
             self._counter += 1
             if 1 != self._counter:
                 return self
 
-            self._cm = self._sqla_engine.session(force_rollback=self._force_rollback)
-            self.session = self._cm.__enter__()
-            self.setup()
+            self._cm = self._engine.session(force_rollback=self._force_rollback)
+            self._session = self._cm.__enter__()
+            self._setup()
             return self
 
     def __exit__(self, *args):
         with self._lock:
             self._counter = max(self._counter - 1, 0)
             if 0 != self._counter:
-                self.session.flush()
+                self._session.flush()
                 return
 
-            self.teardown()
+            self._teardown()
 
             try:
                 self._cm.__exit__(*args)
             except exc.ResourceClosedError:
                 pass
 
-            self._cm = self.session = None
-            self._sqla_engine.teardown_session()
+            self._cm = self._session = None
+            self._engine.teardown_session()
 
 
 class SqlaAsyncContext:
-    def __init__(
-        self, sqla_engine: SqlaAsyncEngine, force_rollback: bool = True,
-    ):
-        self._sqla_engine = sqla_engine
+    def __init__(self, engine: SqlaAsyncEngine, force_rollback: bool = True):
+        self._engine = engine
         self._force_rollback = force_rollback
         self._counter = 0
         self._lock = asyncio.Lock()
+        self._session: SqlaAsyncSession | None = None
 
     @property
     def name(self) -> str:
-        return self._sqla_engine.name
+        return self._engine.name
+
+    @property
+    def engine(self) -> SqlaAsyncEngine:
+        return self._engine
 
     @asynccontextmanager
     async def session_factory(self):
-        yield self.session
+        yield self._session
 
     async def commit(self):
-        await self.session.commit()
+        await self._session.commit()
 
     async def rollback(self):
-        await self.session.rollback()
+        await self._session.rollback()
 
-    async def setup(self):
+    async def _setup(self):
         pass
 
-    async def teardown(self):
+    async def _teardown(self):
         pass
 
     async def __aenter__(self):
         async with self._lock:
             self._counter += 1
             if 1 != self._counter:
                 return self
 
-            self._cm = self._sqla_engine.session(force_rollback=self._force_rollback)
-            self.session = await self._cm.__aenter__()
-            await self.setup()
+            self._cm = self._engine.session(force_rollback=self._force_rollback)
+            self._session = await self._cm.__aenter__()
+            await self._setup()
             return self
 
     async def __aexit__(self, *args):
         async with self._lock:
             self._counter = max(self._counter - 1, 0)
             if 0 != self._counter:
-                await self.session.flush()
+                await self._session.flush()
                 return
 
-            await self.teardown()
+            await self._teardown()
 
             try:
                 await self._cm.__aexit__(*args)
             except exc.ResourceClosedError:
                 pass
 
-            self._cm = self.session = None
-            await self._sqla_engine.teardown_session()
+            self._cm = self._session = None
+            await self._engine.teardown_session()
 
 
 SqlaSyncContextFactory = Callable[[SqlaSyncEngine, bool], SqlaSyncContext]
 SqlaAsyncContextFactory = Callable[[SqlaAsyncEngine, bool], SqlaAsyncContext]
```

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/engine.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/engine.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/factory.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/factory.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/migration/app.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/migration/app.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/migration/cmd.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/migration/cmd.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/migration/operator.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/migration/operator.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/migration/utils.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/migration/utils.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/model.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/model.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/query.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/query.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/repository.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/repository.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/greyhorse_sqla/resources.py` & `greyhorse_sqla-0.3.1/greyhorse_sqla/resources.py`

 * *Files identical despite different names*

### Comparing `greyhorse_sqla-0.3/pyproject.toml` & `greyhorse_sqla-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "greyhorse-sqla"
-version = "0.3"
+version = "0.3.1"
 description = "Greyhorse SqlAlchemy library"
 license = "MIT"
 repository = "https://gitlab.com/max-plutonium/greyhorse"
 authors = ["Max Plutonium <plutonium.max@gmail.com>"]
 maintainers = ["Max Plutonium <plutonium.max@gmail.com>"]
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `greyhorse_sqla-0.3/PKG-INFO` & `greyhorse_sqla-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: greyhorse-sqla
-Version: 0.3
+Version: 0.3.1
 Summary: Greyhorse SqlAlchemy library
 Home-page: https://gitlab.com/max-plutonium/greyhorse
 License: MIT
 Author: Max Plutonium
 Author-email: plutonium.max@gmail.com
 Maintainer: Max Plutonium
 Maintainer-email: plutonium.max@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mysql
 Provides-Extra: pg
 Provides-Extra: sqlite
 Requires-Dist: aiomysql (>=0.1,<0.2) ; extra == "mysql"
 Requires-Dist: aiosqlite (>=0.18,<0.19) ; extra == "sqlite"
 Requires-Dist: alembic (>=1.10,<2.0)
 Requires-Dist: asyncpg (>=0.27,<0.28) ; extra == "pg"
-Requires-Dist: greyhorse-core (==0.3)
+Requires-Dist: greyhorse_core @ file:///home/plutonium/Projects/greyhorse/core
 Requires-Dist: psycopg2 (>=2.9,<3.0) ; extra == "pg"
 Requires-Dist: pymysql[rsa] (>=1.0,<2.0) ; extra == "mysql"
 Requires-Dist: sqlalchemy-utils (>=0.41,<0.42)
 Requires-Dist: sqlalchemy[asyncio,mypy] (>=2.0,<3.0)
 Project-URL: Repository, https://gitlab.com/max-plutonium/greyhorse
```

