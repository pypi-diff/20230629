# Comparing `tmp/kaiju_db-2.1.3-py3-none-any.whl.zip` & `tmp/kaiju_db-2.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 19605 bytes, number of entries: 12
--rw-r--r--  2.0 unx      183 b- defN 23-Jun-27 19:17 kaiju_db/__init__.py
--rw-r--r--  2.0 unx     3665 b- defN 23-Jun-27 19:17 kaiju_db/functions.py
--rw-r--r--  2.0 unx    57079 b- defN 23-Jun-27 19:17 kaiju_db/services.py
--rw-r--r--  2.0 unx      453 b- defN 23-Jun-27 19:17 kaiju_db/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 19:17 kaiju_db/tests/__init__.py
--rw-r--r--  2.0 unx     3240 b- defN 23-Jun-27 19:17 kaiju_db/tests/fixtures.py
--rw-r--r--  2.0 unx     4832 b- defN 23-Jun-27 19:17 kaiju_db/tests/test_db.py
--rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3090 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      939 b- defN 23-Jun-27 19:18 kaiju_db-2.1.3.dist-info/RECORD
-12 files, 74192 bytes uncompressed, 18033 bytes compressed:  75.7%
+Zip file size: 19823 bytes, number of entries: 12
+-rw-r--r--  2.0 unx      183 b- defN 23-Jun-29 12:17 kaiju_db/__init__.py
+-rw-r--r--  2.0 unx     3665 b- defN 23-Jun-29 12:17 kaiju_db/functions.py
+-rw-r--r--  2.0 unx    58012 b- defN 23-Jun-29 12:17 kaiju_db/services.py
+-rw-r--r--  2.0 unx      453 b- defN 23-Jun-29 12:17 kaiju_db/types.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 12:17 kaiju_db/tests/__init__.py
+-rw-r--r--  2.0 unx     3240 b- defN 23-Jun-29 12:17 kaiju_db/tests/fixtures.py
+-rw-r--r--  2.0 unx     4831 b- defN 23-Jun-29 12:17 kaiju_db/tests/test_db.py
+-rw-rw-rw-  2.0 unx      610 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3090 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      939 b- defN 23-Jun-29 12:17 kaiju_db-2.1.4.dist-info/RECORD
+12 files, 75124 bytes uncompressed, 18251 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: kaiju_db/tests/fixtures.py
 Comment: 
 
 Filename: kaiju_db/tests/test_db.py
 Comment: 
 
-Filename: kaiju_db-2.1.3.dist-info/LICENSE
+Filename: kaiju_db-2.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: kaiju_db-2.1.3.dist-info/METADATA
+Filename: kaiju_db-2.1.4.dist-info/METADATA
 Comment: 
 
-Filename: kaiju_db-2.1.3.dist-info/WHEEL
+Filename: kaiju_db-2.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: kaiju_db-2.1.3.dist-info/top_level.txt
+Filename: kaiju_db-2.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: kaiju_db-2.1.3.dist-info/RECORD
+Filename: kaiju_db-2.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kaiju_db/__init__.py

```diff
@@ -1,8 +1,8 @@
 from .types import *
 from .functions import *
 from .services import *
 
-__version__ = '2.1.3'
+__version__ = '2.1.4'
 __python_version__ = '3.8'
 __author__ = 'antonnidhoggr@me.com'
 __service_package__ = True
```

## kaiju_db/services.py

```diff
@@ -1,12 +1,26 @@
 """Database services."""
 
 import abc
 from pathlib import Path
-from typing import cast, List, Collection, TypedDict, AsyncGenerator, Union, Optional
+from typing import (
+    cast,
+    List,
+    Collection,
+    TypedDict,
+    AsyncGenerator,
+    Union,
+    Optional,
+    Generic,
+    TypeVar,
+    Hashable,
+    Dict,
+    FrozenSet,
+    Literal,
+)
 
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as sa_pg
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.sql.expression import nullslast
 from sqlalchemy import MetaData, text, Table  # noqa pycharm
 from sqlalchemy.ext.asyncio import create_async_engine  # noqa pycharm
@@ -238,15 +252,42 @@
         for _function_key in self._functions_registry:
             _function = self._functions_registry[_function_key]
             if issubclass(_function, UserFunction):
                 _function = _function.sql()
             await conn.execute(text(f'CREATE OR REPLACE {_function}'))
 
 
-class SQLService(Service, DataStore, abc.ABC):
+class _SortAsc(TypedDict):
+    asc: str
+
+
+class _SortDesc(TypedDict):
+    desc: str
+
+
+_Id = TypeVar('_Id', bound=Hashable)
+_Row = TypeVar('_Row', bound=dict)
+_Columns = Union[Collection[str], Literal['*'], None]
+_SortField = Union[_SortDesc, _SortAsc, str]
+_Sort = Optional[List[_SortField]]
+_Condition = Union[dict, List[dict], None]
+
+
+class _List(TypedDict):
+    """Type hinting for a list query."""
+
+    count: Optional[int]  #: total rows matching the query, None if count hasn't been requested
+    offset: int  #: row offset for this selection
+    page: Optional[int]  #: current page number, None if count hasn't been requested
+    pages: Optional[int]  #: total pages, None if count hasn't been requested
+    on_page: int  #: number of rows on this page
+    data: Optional[List[_Row]]  #: returned rows, None if limit was set to 0
+
+
+class SQLService(Service, DataStore, Generic[_Id, _Row], abc.ABC):
     """Base SQL service interface with common commands and errors.
 
     Optimized for a single primary key only with a name "id"
 
     Example of use:
 
     You need to set your own table and, if needed, define column whitelists
@@ -279,24 +320,14 @@
                 ... # custom query
 
     :param app: web app instance
     :param database_service: database service instance or instance name
     :param logger: optional logger instance
     """
 
-    class _List(TypedDict):
-        """Type hinting for a list query."""
-
-        count: Optional[int]  #: total rows matching the query, None if count hasn't been requested
-        offset: int  #: row offset for this selection
-        page: Optional[int]  #: current page number, None if count hasn't been requested
-        pages: Optional[int]  #: total pages, None if count hasn't been requested
-        on_page: int  #: number of rows on this page
-        data: Optional[List[dict]]  #: returned rows, None if limit was set to 0
-
     class ErrorCode:
         """These error codes should be commonly used for SQL related errors."""
 
         EXISTS = 'query.exists'
         REFERENCE_NOT_FOUND = 'query.reference_not_found'
         NOT_FOUND = 'query.not_found'
         INTERNAL_ERROR = 'query.internal_error'
@@ -386,43 +417,43 @@
         return sql
 
     @staticmethod
     def delete_condition_hook(sql):
         """Set up specific delete conditions."""
         return sql
 
-    def _create_primary_key_condition_for_single_key(self, sql, _id):
+    def _create_primary_key_condition_for_single_key(self, sql, _id: _Id):
         return sql.where(self._primary_key == _id)
 
-    def _create_list_primary_key_condition_for_single_key(self, sql, _id):
+    def _create_list_primary_key_condition_for_single_key(self, sql, _id: Union[_Id, Collection[_Id]]):
         if not isinstance(_id, (list, tuple, set)):
             _id = [_id]
         return sql.where(self._primary_key.in_(_id))
 
-    def _parse_composite_id(self, _id):
+    def _parse_composite_id(self, _id: Union[Dict[str, _Id], Collection[_Id], _Id]):
         conditions = []
         try:
             if isinstance(_id, dict):
                 for col in self._primary_key:
                     conditions.append(col == _id[col.name])
             else:
                 for value, col in zip(_id, self._primary_key):
                     conditions.append(col == value)
         except KeyError:
             raise ValidationError('Primary key field is not present.')
         else:
             return sa.and_(*conditions)
 
-    def _create_list_primary_key_condition_for_composite_key(self, sql, _id):
+    def _create_list_primary_key_condition_for_composite_key(self, sql, _id: Union[_Id, Collection[_Id]]):
         if not isinstance(_id, (list, tuple, set)):
             _id = [_id]
         condition = sa.or_(*(self._parse_composite_id(n) for n in _id))
         return sql.where(condition)
 
-    def _create_primary_key_condition_for_composite_key(self, sql, _id: dict):
+    def _create_primary_key_condition_for_composite_key(self, sql, _id):
         condition = self._parse_composite_id(_id)
         return sql.where(condition)
 
     def _raise_primary_key_condition_for_no_keys(self, *_, **__):
         raise MethodNotAllowed(
             message='Direct referencing objects in the table is forbidden'
             ' because there are no primary keys in this table.'
@@ -477,38 +508,38 @@
             table = self.table
         sql = table.select().with_only_columns(sa.text('1'))
         sql = self._primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         sql = sql.limit(1)
         return sql
 
-    async def exists(self, id, _connection=None) -> bool:
+    async def exists(self, id: _Id, _connection=None) -> bool:
         """Return True if object exists. False otherwise.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
             await service.exists({'id': 1, 'key': 'abc'})
 
         """
         sql = self._create_exists_query(id)
         result = await self._wrap_get(_connection, sql)
         return bool(result.first())
 
-    def _create_m_exists_query(self, _id: list, table=None):
+    def _create_m_exists_query(self, _id: Collection[_Id], table=None):
         if table is None:
             table = self.table
         sql = table.select().with_only_columns(*self._primary_key_list)
         sql = self._list_primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         return sql
 
-    async def m_exists(self, id: list, _connection=None):
+    async def m_exists(self, id: Collection[_Id], _connection=None) -> FrozenSet[_Id]:
         """Return a set of existing IDs for a list of IDs.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -598,25 +629,25 @@
     @staticmethod
     def _filter_columns(columns: List[sa.Column], whitelist: Optional[frozenset]):
         if whitelist is None:
             return columns
         else:
             return [col for col in columns if col.name in whitelist]
 
-    def _create_get_query(self, _id, columns, table=None):
+    def _create_get_query(self, _id: _Id, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         sql = table.select().with_only_columns(*columns)
         sql = self._primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         sql = sql.limit(1)
         return sql
 
-    async def get(self, id, columns='*', _connection=None):
+    async def get(self, id: _Id, columns: _Columns = '*', _connection=None) -> _Row:
         """Return information about an object.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -636,24 +667,24 @@
                 service=self.service_name,
                 object_id=str(id),
                 code=SQLService.ErrorCode.NOT_FOUND,
             )
         if columns:
             return result._asdict()
 
-    def _create_m_get_query(self, _id: list, columns, table=None):
+    def _create_m_get_query(self, _id: Collection[_Id], columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         sql = table.select().with_only_columns(*columns)
         sql = self._list_primary_key_condition(sql, _id)
         sql = self.get_condition_hook(sql)
         return sql
 
-    async def m_get(self, id: list, columns='*', _connection=None):
+    async def m_get(self, id: Collection[_Id], columns: _Columns = '*', _connection=None) -> List[_Row]:
         """Return multiple objects.
 
         Objects that don't exist will be skipped.
         Returns all data at once without pagination. Use `SQLService.list` if
         you want pagination or sorting.
 
         If you have composite primary keys you should pass dictionary objects
@@ -664,28 +695,28 @@
             await service.m_get([{'id': 1, 'key': 'abc'}, ...], ...)
 
         """
         sql = self._create_m_get_query(id, columns)
         result = await self._wrap_get(_connection, sql)
         return [row._asdict() for row in result.all()]
 
-    def _create_delete_query(self, _id, columns, table=None):
+    def _create_delete_query(self, _id: _Id, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         sql = table.delete()
         sql = self._primary_key_condition(sql, _id)
         sql = self.delete_condition_hook(sql)
         if columns:
             sql = sql.returning(*columns)
         else:
             sql = sql.returning(sa.literal_column('1'))
         return sql
 
-    async def delete(self, id, columns=None, _connection=None):
+    async def delete(self, id: _Id, columns: _Columns = None, _connection=None) -> _Row:
         """Remove a single object from a table.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -702,28 +733,30 @@
                 service=self.service_name,
                 object_id=str(id),
                 code=SQLService.ErrorCode.NOT_FOUND,
             )
         if columns:
             return result._asdict()
 
-    def _create_m_delete_query(self, _id, conditions, columns, table=None):
+    def _create_m_delete_query(self, _id: Collection[_Id], conditions, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         sql = table.delete()
         if _id:
             sql = self._list_primary_key_condition(sql, _id)
         if conditions:
             sql = self._create_conditions(sql, conditions, table)
         sql = self.delete_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
-    async def m_delete(self, id: list = None, conditions=None, columns=None, _connection=None):
+    async def m_delete(
+        self, id: Collection[_Id] = None, conditions: _Condition = None, columns: _Columns = None, _connection=None
+    ) -> List[_Row]:
         """Remove multiple objects from a table. Non-existing objects will be skipped.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -758,15 +791,15 @@
                     'There are not consumed columns in the update statement.',
                     data=data,
                     service=self.service_name,
                     allowed_columns=self.insert_columns,
                     code=SQLService.ErrorCode.INVALID_COLUMN,
                 )
 
-    def _create_insert_query(self, data, columns, table=None, **on_conflict_clause):
+    def _create_insert_query(self, data: dict, columns, table=None, **on_conflict_clause):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         self._validate_row(data, whitelist=self.insert_columns)
         data = self.prepare_insert_data(data)
         sql = sa_pg.insert(table).values(data)
         sql = self._on_conflict_clause(sql, **on_conflict_clause)
@@ -782,20 +815,20 @@
                 on_conflict_values = self.prepare_update_data(on_conflict_values)
             sql = sql.on_conflict_do_update(index_elements=on_conflict_keys, set_=on_conflict_values)
         return sql
 
     async def create(
         self,
         data: dict,
-        columns='*',
+        columns: _Columns = '*',
         _connection=None,
         on_conflict=None,
         on_conflict_keys=None,
         on_conflict_values=None,
-    ):
+    ) -> _Row:
         """Create a single object.
 
         :param data: objects data
         :param columns: columns to return, None for no return
         :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
         :param on_conflict_keys: list of on conflict constraints
         :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
@@ -809,15 +842,15 @@
             on_conflict_keys=on_conflict_keys,
             on_conflict_values=on_conflict_values,
         )
         result = await self._wrap_insert(_connection, sql)
         if columns:
             return result.first()._asdict()
 
-    def _create_m_insert_query(self, data: List[dict], columns, table=None, **on_conflict_clause):
+    def _create_m_insert_query(self, data: Collection[dict], columns, table=None, **on_conflict_clause):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         _data = []
         for row in data:
             self._validate_row(row, whitelist=self.insert_columns)
             _data.append(self.prepare_insert_data(row))
@@ -825,21 +858,21 @@
         sql = self._on_conflict_clause(sql, **on_conflict_clause)
         sql = self.insert_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
     async def m_create(
         self,
-        data: List[dict],
-        columns='*',
+        data: Collection[dict],
+        columns: _Columns = '*',
         _connection=None,
         on_conflict: str = None,
         on_conflict_keys: list = None,
         on_conflict_values: dict = None,
-    ):
+    ) -> List[_Row]:
         """Create multiple objects.
 
         :param data: list of objects data
         :param columns: columns to return, None for no return
         :param on_conflict: on conflict clause if required ('do_nothing', 'do_update')
         :param on_conflict_keys: list of on conflict constraints
         :param on_conflict_values: an object with on conflict values, used only by `do_update` clause
@@ -858,27 +891,27 @@
             return [row._asdict() for row in result.all()]
 
     @staticmethod
     def prepare_update_data(data: dict):
         """You may define your custom row update logic here."""
         return data
 
-    def _create_update_query(self, _id, data: dict, columns, table=None):
+    def _create_update_query(self, _id: _Id, data: dict, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         self._validate_row(data, whitelist=self.update_columns)
         data = self.prepare_update_data(data)
         sql = table.update().values(data)
         sql = self._primary_key_condition(sql, _id)
         sql = self.update_condition_hook(sql)
         sql = sql.returning(*columns) if columns else sql.returning(sa.literal_column('1'))
         return sql
 
-    async def update(self, id, data: dict, columns='*', _connection=None) -> dict:
+    async def update(self, id: _Id, data: dict, columns: _Columns = '*', _connection=None) -> _Row:
         """Update a single object. Raises error if object doesn't exist.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -894,30 +927,32 @@
                 service=self.service_name,
                 object_id=str(id),
                 code=SQLService.ErrorCode.NOT_FOUND,
             )
         if columns:
             return result._asdict()
 
-    def _create_m_update_query(self, _id, data: dict, conditions, columns, table=None):
+    def _create_m_update_query(self, _id: Collection[_Id], data: dict, conditions, columns, table=None):
         if table is None:
             table = self.table
         columns = self._sql_get_columns(columns, table=table)
         self._validate_row(data, whitelist=self.update_columns)
         data = self.prepare_update_data(data)
         sql = table.update().values(data)
         if _id:
             sql = self._list_primary_key_condition(sql, _id)
         if conditions:
             sql = self._create_conditions(sql, conditions, table)
         sql = self.update_condition_hook(sql)
         sql = sql.returning(*columns)
         return sql
 
-    async def m_update(self, id: list, data: dict, conditions=None, columns='*', _connection=None):
+    async def m_update(
+        self, id: Collection[_Id], data: dict, conditions: _Condition = None, columns: _Columns = '*', _connection=None
+    ) -> List[_Row]:
         """Update multiple objects with the same data. Non-existing objects will be skipped.
 
         If you have composite primary keys you should pass dictionary objects
         in id field, like this:
 
         .. code-block:: python
 
@@ -926,15 +961,15 @@
         """
         sql = self._create_m_update_query(id, data, conditions, columns)
         result = await self._wrap_update(_connection, sql)
         if columns:
             return [row._asdict() for row in result.all()]
 
     def _create_conditions(self, sql, conditions, table=None):
-        """Add SQL conditions to an sql query.
+        """Add SQL conditions to sql query.
 
         Allows some simple queries to be constructed.
 
         .. code-block:: python
 
             [ ... ]  # OR
             { ... }  # AND
@@ -1121,32 +1156,29 @@
             page = max(1, offset // page_size + bool(n % page_size))
             return page, pages
         else:
             return None, None
 
     async def list(
         self,
-        conditions=None,
-        sort=None,
-        offset=0,
-        limit=DEFAULT_ROW_LIMIT,
-        count=True,
-        precision=None,
-        columns='*',
+        conditions: _Condition = None,
+        sort: _Sort = None,
+        offset: int = 0,
+        limit: int = DEFAULT_ROW_LIMIT,
+        count: bool = True,
+        columns: _Columns = '*',
         _connection=None,
     ) -> _List:
         """List rows with pagination and conditions.
 
         :param conditions: optional query conditions
         :param sort: optional row ordering
         :param offset: optional row offset
         :param limit: optional row limit
         :param count: calculate page count
-        :param precision: count precision, if None then table sampling won't be used
-            must be from 0 to 100
         :param columns: columns to return
         :param _connection: optional connection object (when using inside a transactional block)
         :returns: This method may return different data depending on the provided params
 
         Condition example:
 
         .. code-block:: python
@@ -1221,36 +1253,41 @@
         """
         if columns and limit:
             sql = self._create_list_query(conditions, sort, offset, limit, columns)
             result = await self._wrap_get(_connection, sql)
             result = result.all()
             result = [row._asdict() for row in result]
             if count:
-                sql_count = self._create_count_query(conditions, precision)
+                sql_count = self._create_count_query(conditions, None)
                 count = await self._wrap_get(_connection, sql_count)
                 count = count.scalar()
                 page, pages = self._get_page_count(count, offset, limit)
             else:
                 count, page, pages = None, None, None
             on_page = len(result)
         else:
             on_page, result = 0, None
             if count:
-                sql_count = self._create_count_query(conditions, precision)
+                sql_count = self._create_count_query(conditions, None)
                 count = await self._wrap_get(_connection, sql_count)
                 count = count.scalar()
                 page, pages = self._get_page_count(count, offset, limit)
             else:
                 count, page, pages, on_page = None, None, None, 0
 
         return {'count': count, 'offset': offset, 'page': page, 'pages': pages, 'on_page': on_page, 'data': result}
 
     async def iter(
-        self, conditions=None, sort=None, offset=0, limit=DEFAULT_ROW_LIMIT, columns='*'
-    ) -> AsyncGenerator[List[dict], None]:
+        self,
+        conditions: _Condition = None,
+        sort: _Sort = None,
+        offset: int = 0,
+        limit: int = DEFAULT_ROW_LIMIT,
+        columns: _Columns = '*',
+    ) -> AsyncGenerator[List[_Row], None]:
         """Iterate over listed data.
 
         Almost the same as `SQLService.list` but returns a generator which iterates
         over the query content. It's not intended to be used by a client
         but inside the app or the service itself.
 
         See `SQLService.list` for info about params.
```

## kaiju_db/tests/test_db.py

```diff
@@ -96,15 +96,14 @@
 
     async def _remove_tables(self, database_service):
         for t in self.table_names:
             await database_service.execute(f'DROP TABLE IF EXISTS {t};')
 
     @pytest.fixture
     def _service(self, app, database_service, test_table):
-
         test_table.append_column(sa.Column('uuid', sa_pg.UUID))
 
         class TestService(SQLService):
             table = test_table
 
         return TestService(app=app, database_service=database_service)
```

## Comparing `kaiju_db-2.1.3.dist-info/LICENSE` & `kaiju_db-2.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kaiju_db-2.1.3.dist-info/METADATA` & `kaiju_db-2.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaiju-db
-Version: 2.1.3
+Version: 2.1.4
 Summary: Postgresql db services and tools
 Home-page: https://gitlab.com/kaiju-python/kaiju-db
 Author: antonnidhoggr@me.com
 Author-email: antonnidhoggr@me.com
 License: Apache Software License 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

