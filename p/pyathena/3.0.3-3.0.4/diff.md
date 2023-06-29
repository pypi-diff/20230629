# Comparing `tmp/pyathena-3.0.3.tar.gz` & `tmp/pyathena-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyathena-3.0.3.tar", max compression
+gzip compressed data, was "pyathena-3.0.4.tar", max compression
```

## Comparing `pyathena-3.0.3.tar` & `pyathena-3.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1055 2023-05-29 14:36:52.101374 pyathena-3.0.3/LICENSE
--rw-r--r--   0        0        0    70055 2023-05-29 14:36:52.101374 pyathena-3.0.3/README.rst
--rw-r--r--   0        0        0     1959 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/__init__.py
--rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/__init__.py
--rw-r--r--   0        0        0     5193 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/async_cursor.py
--rw-r--r--   0        0        0     2590 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/converter.py
--rw-r--r--   0        0        0     7250 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/cursor.py
--rw-r--r--   0        0        0     9791 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/result_set.py
--rw-r--r--   0        0        0     2457 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/arrow/util.py
--rw-r--r--   0        0        0     5409 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/async_cursor.py
--rw-r--r--   0        0        0    21206 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/common.py
--rw-r--r--   0        0        0    10452 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/connection.py
--rw-r--r--   0        0        0     4245 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/converter.py
--rw-r--r--   0        0        0     5835 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/cursor.py
--rw-r--r--   0        0        0      660 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/error.py
--rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/fastparquet/__init__.py
--rw-r--r--   0        0        0     2475 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/fastparquet/util.py
--rw-r--r--   0        0        0       24 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/__init__.py
--rw-r--r--   0        0        0    20510 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/s3.py
--rw-r--r--   0        0        0     1252 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/filesystem/s3_object.py
--rw-r--r--   0        0        0     6571 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/formatter.py
--rw-r--r--   0        0        0    17121 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/model.py
--rw-r--r--   0        0        0      220 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/__init__.py
--rw-r--r--   0        0        0     5865 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/async_cursor.py
--rw-r--r--   0        0        0     1866 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/converter.py
--rw-r--r--   0        0        0     8327 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/cursor.py
--rw-r--r--   0        0        0    13625 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/result_set.py
--rw-r--r--   0        0        0     9858 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/pandas/util.py
--rw-r--r--   0        0        0        0 2023-05-29 14:36:52.101374 pyathena-3.0.3/pyathena/py.typed
--rw-r--r--   0        0        0    25140 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/result_set.py
--rw-r--r--   0        0        0       24 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/__init__.py
--rw-r--r--   0        0        0      661 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/arrow.py
--rw-r--r--   0        0        0    36928 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/base.py
--rw-r--r--   0        0        0      884 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/pandas.py
--rw-r--r--   0        0        0     2638 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/requirements.py
--rw-r--r--   0        0        0      173 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/rest.py
--rw-r--r--   0        0        0     1246 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/types.py
--rw-r--r--   0        0        0      142 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/sqlalchemy/util.py
--rw-r--r--   0        0        0     1984 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyathena/util.py
--rw-r--r--   0        0        0     3482 2023-05-29 14:36:52.105374 pyathena-3.0.3/pyproject.toml
--rw-r--r--   0        0        0    71294 1970-01-01 00:00:00.000000 pyathena-3.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-29 14:51:30.473008 pyathena-3.0.4/LICENSE
+-rw-r--r--   0        0        0    70055 2023-06-29 14:51:30.473008 pyathena-3.0.4/README.rst
+-rw-r--r--   0        0        0     1959 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/__init__.py
+-rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/__init__.py
+-rw-r--r--   0        0        0     5193 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/async_cursor.py
+-rw-r--r--   0        0        0     2590 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/converter.py
+-rw-r--r--   0        0        0     7250 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/cursor.py
+-rw-r--r--   0        0        0     9791 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/result_set.py
+-rw-r--r--   0        0        0     2457 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/arrow/util.py
+-rw-r--r--   0        0        0     5409 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/async_cursor.py
+-rw-r--r--   0        0        0    21206 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/common.py
+-rw-r--r--   0        0        0    10452 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/connection.py
+-rw-r--r--   0        0        0     4245 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/converter.py
+-rw-r--r--   0        0        0     5835 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/cursor.py
+-rw-r--r--   0        0        0      660 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/error.py
+-rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/fastparquet/__init__.py
+-rw-r--r--   0        0        0     2475 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/fastparquet/util.py
+-rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/__init__.py
+-rw-r--r--   0        0        0    20510 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/s3.py
+-rw-r--r--   0        0        0     1252 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/filesystem/s3_object.py
+-rw-r--r--   0        0        0     6571 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/formatter.py
+-rw-r--r--   0        0        0    17121 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/model.py
+-rw-r--r--   0        0        0      220 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/__init__.py
+-rw-r--r--   0        0        0     5865 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/async_cursor.py
+-rw-r--r--   0        0        0     1866 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/converter.py
+-rw-r--r--   0        0        0     8327 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/cursor.py
+-rw-r--r--   0        0        0    13625 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/result_set.py
+-rw-r--r--   0        0        0     9858 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/pandas/util.py
+-rw-r--r--   0        0        0        0 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/py.typed
+-rw-r--r--   0        0        0    25140 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/result_set.py
+-rw-r--r--   0        0        0       24 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0      661 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/arrow.py
+-rw-r--r--   0        0        0    37022 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/base.py
+-rw-r--r--   0        0        0      884 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/pandas.py
+-rw-r--r--   0        0        0     2638 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/requirements.py
+-rw-r--r--   0        0        0      173 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/rest.py
+-rw-r--r--   0        0        0     1246 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/types.py
+-rw-r--r--   0        0        0      142 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/sqlalchemy/util.py
+-rw-r--r--   0        0        0     1984 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyathena/util.py
+-rw-r--r--   0        0        0     3482 2023-06-29 14:51:30.477010 pyathena-3.0.4/pyproject.toml
+-rw-r--r--   0        0        0    71294 1970-01-01 00:00:00.000000 pyathena-3.0.4/PKG-INFO
```

### Comparing `pyathena-3.0.3/LICENSE` & `pyathena-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/README.rst` & `pyathena-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/__init__.py` & `pyathena-3.0.4/pyathena/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import TYPE_CHECKING, FrozenSet, Type
 
 from pyathena.error import *  # noqa
 
 if TYPE_CHECKING:
     from pyathena.connection import Connection
 
-__version__: str = "3.0.3"
+__version__: str = "3.0.4"
 user_agent_extra: str = f"PyAthena/{__version__}"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 2
 paramstyle: str = "pyformat"
```

### Comparing `pyathena-3.0.3/pyathena/arrow/async_cursor.py` & `pyathena-3.0.4/pyathena/arrow/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/arrow/converter.py` & `pyathena-3.0.4/pyathena/arrow/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/arrow/cursor.py` & `pyathena-3.0.4/pyathena/arrow/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/arrow/result_set.py` & `pyathena-3.0.4/pyathena/arrow/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/arrow/util.py` & `pyathena-3.0.4/pyathena/arrow/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/async_cursor.py` & `pyathena-3.0.4/pyathena/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/common.py` & `pyathena-3.0.4/pyathena/common.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/connection.py` & `pyathena-3.0.4/pyathena/connection.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/converter.py` & `pyathena-3.0.4/pyathena/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/cursor.py` & `pyathena-3.0.4/pyathena/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/error.py` & `pyathena-3.0.4/pyathena/error.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/fastparquet/util.py` & `pyathena-3.0.4/pyathena/fastparquet/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/filesystem/s3.py` & `pyathena-3.0.4/pyathena/filesystem/s3.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/filesystem/s3_object.py` & `pyathena-3.0.4/pyathena/filesystem/s3_object.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/formatter.py` & `pyathena-3.0.4/pyathena/formatter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/model.py` & `pyathena-3.0.4/pyathena/model.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/pandas/async_cursor.py` & `pyathena-3.0.4/pyathena/pandas/async_cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/pandas/converter.py` & `pyathena-3.0.4/pyathena/pandas/converter.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/pandas/cursor.py` & `pyathena-3.0.4/pyathena/pandas/cursor.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/pandas/result_set.py` & `pyathena-3.0.4/pyathena/pandas/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/pandas/util.py` & `pyathena-3.0.4/pyathena/pandas/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/result_set.py` & `pyathena-3.0.4/pyathena/result_set.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/sqlalchemy/arrow.py` & `pyathena-3.0.4/pyathena/sqlalchemy/arrow.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/sqlalchemy/base.py` & `pyathena-3.0.4/pyathena/sqlalchemy/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,14 +916,18 @@
     _connect_options: Dict[str, Any] = dict()  # type: ignore
     _pattern_column_type: Pattern[str] = re.compile(r"^([a-zA-Z]+)(?:$|[\(|<](.+)[\)|>]$)")
 
     @classmethod
     def import_dbapi(cls) -> "ModuleType":
         return pyathena
 
+    @classmethod
+    def dbapi(cls) -> "ModuleType":  # type: ignore
+        return pyathena
+
     def _raw_connection(self, connection: Union[Engine, "Connection"]) -> "PoolProxiedConnection":
         if isinstance(connection, Engine):
             return connection.raw_connection()
         return connection.connection
 
     def create_connect_args(self, url: "URL") -> Tuple[Tuple[str], MutableMapping[str, Any]]:
         # Connection string format:
```

### Comparing `pyathena-3.0.3/pyathena/sqlalchemy/pandas.py` & `pyathena-3.0.4/pyathena/sqlalchemy/pandas.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/sqlalchemy/requirements.py` & `pyathena-3.0.4/pyathena/sqlalchemy/requirements.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/sqlalchemy/types.py` & `pyathena-3.0.4/pyathena/sqlalchemy/types.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyathena/util.py` & `pyathena-3.0.4/pyathena/util.py`

 * *Files identical despite different names*

### Comparing `pyathena-3.0.3/pyproject.toml` & `pyathena-3.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyAthena"
-version = "3.0.3"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
+version = "3.0.4"  # https://github.com/laughingman7743/PyAthena/blob/master/pyathena/__init__.py#L10
 description = "Python DB API 2.0 (PEP 249) client for Amazon Athena"
 license = "MIT"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `pyathena-3.0.3/PKG-INFO` & `pyathena-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyathena
-Version: 3.0.3
+Version: 3.0.4
 Summary: Python DB API 2.0 (PEP 249) client for Amazon Athena
 Home-page: https://github.com/laughingman7743/PyAthena/
 License: MIT
 Author: laughingman7743
 Author-email: laughingman7743@gmail.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
```

