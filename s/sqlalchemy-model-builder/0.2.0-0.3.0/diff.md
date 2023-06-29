# Comparing `tmp/sqlalchemy_model_builder-0.2.0.tar.gz` & `tmp/sqlalchemy_model_builder-0.3.0.tar.gz`

## Comparing `sqlalchemy_model_builder-0.2.0.tar` & `sqlalchemy_model_builder-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/__init__.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/_models.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/exceptions.py
--rw-r--r--   0        0        0     5633 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/model_builder.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/random_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_model_builder_relationships.py
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_model_builder_types.py
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/tests/test_random_builder.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/LICENSE
--rw-r--r--   0        0        0     2130 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/README.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/__init__.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/_models.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/exceptions.py
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/model_builder.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/random_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/tests/test_model_builder_relationships.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/tests/test_model_builder_types.py
+-rw-r--r--   0        0        0     2223 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/tests/test_random_builder.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/README.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 sqlalchemy_model_builder-0.3.0/PKG-INFO
```

### Comparing `sqlalchemy_model_builder-0.2.0/.github/workflows/publish.yml` & `sqlalchemy_model_builder-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/.github/workflows/test.yml` & `sqlalchemy_model_builder-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/model_builder.py` & `sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/model_builder.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from datetime import date, datetime, time, timedelta
-from typing import Any, Generic, Optional, Type, TypeVar
-from uuid import UUID
+from typing import Any, Callable, Dict, Generic, Optional, Type, TypeVar
 
 from sqlalchemy import inspect
 from sqlalchemy.exc import NoInspectionAvailable
 from sqlalchemy.orm import Mapper, Session
 
 from sqlalchemy_model_builder._models import ColumnValuePair, ColumnValuePairList
 from sqlalchemy_model_builder.exceptions import ModelBuilderException
 from sqlalchemy_model_builder.random_builder import RandomBuilder
 
 T = TypeVar("T")
 
-_TYPE_MAPPING = {
-    bool: RandomBuilder.next_bool,
-    bytes: RandomBuilder.next_bytes,
-    date: RandomBuilder.next_date,
-    datetime: RandomBuilder.next_datetime,
-    float: RandomBuilder.next_float,
-    int: RandomBuilder.next_int,
-    str: RandomBuilder.next_str,
-    time: RandomBuilder.next_time,
-    timedelta: RandomBuilder.next_timedelta,
-    UUID: RandomBuilder.next_uuid,
+_TYPE_MAPPING: Dict[str, Callable[[], Any]] = {
+    "BigInteger": RandomBuilder.next_int,
+    "Boolean": RandomBuilder.next_bool,
+    "Date": RandomBuilder.next_date,
+    "DateTime": RandomBuilder.next_datetime,
+    "Float": RandomBuilder.next_float,
+    "Integer": RandomBuilder.next_int,
+    "Interval": RandomBuilder.next_timedelta,
+    "LargeBinary": RandomBuilder.next_bytes,
+    "Numeric": RandomBuilder.next_float,
+    "SmallInteger": RandomBuilder.next_int,
+    "String": RandomBuilder.next_str,
+    "Text": RandomBuilder.next_str,
+    "Time": RandomBuilder.next_time,
+    "Unicode": RandomBuilder.next_str,
+    "UnicodeText": RandomBuilder.next_str,
+    "Uuid": RandomBuilder.next_uuid,
 }
 
 
 class ModelBuilder(Generic[T]):
     def __init__(self, db_model: Type[T], minimal: bool = False):
         self.db: Optional[Session] = None
         self.db_model = db_model
@@ -116,46 +120,31 @@
             primary_key = inspect(relationship.value).mapper.primary_key[0]
             column_value = ColumnValuePair(
                 relationship.column, getattr(relationship.value, primary_key.key)
             )
             column_values.append(column_value)
 
         for column in mapper.columns:  # type: ignore
-            python_type: Optional[type] = None
-
-            if hasattr(column.type, "impl"):
-                if hasattr(column.type.impl, "python_type"):
-                    python_type = column.type.python_type
-            elif hasattr(column.type, "python_type"):
-                python_type = column.type.python_type
-            assert python_type, f"Could not infer python_type for {column}"
+            type_ = column.type.__class__.__name__
 
             if self.minimal and column.nullable:
                 continue
 
             if column.foreign_keys:
                 continue
 
-            if column.type.__class__.__name__ == "Enum":
+            if type_ == "Enum":
                 random_value = RandomBuilder.next_from_list(column.type.enums)
             else:
-                random_value = self.__map_field_to_random_builder_method(python_type)()
+                builder = _TYPE_MAPPING.get(type_, RandomBuilder.next_str)
+                random_value = builder()
 
             column_value = ColumnValuePair(column.key, random_value)
             column_values.append(column_value)
 
         return ColumnValuePairList(column_values)
 
-    def __map_field_to_random_builder_method(self, field_type: type) -> Any:
-        """Mapping between field type and RandomBuilder methods
-
-        :returns: a RandomBuilder method for the provided type
-        :rtype: function
-        """
-
-        return _TYPE_MAPPING.get(field_type, RandomBuilder.next_str)
-
     def __save(self, instance: T) -> None:
         assert self.db is not None
 
         self.db.add(instance)
         self.db.commit()
```

### Comparing `sqlalchemy_model_builder-0.2.0/sqlalchemy_model_builder/random_builder.py` & `sqlalchemy_model_builder-0.3.0/sqlalchemy_model_builder/random_builder.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/.gitignore` & `sqlalchemy_model_builder-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/LICENSE` & `sqlalchemy_model_builder-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/README.md` & `sqlalchemy_model_builder-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,25 +9,25 @@
 - Build minimal (with required fields) only
 
 ---
 
 ## Installation
 
 ```shell
-$ pip install sqladmin
+$ pip install sqlalchemy-model-builder
 ```
 
 ---
 
 ## How to use
 Deinfe the SQLAlchemy models:
 
 ```python
+from sqlalchemy import Integer, String, Text
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql.sqltypes import Integer, String, Text
 
 Base = declarative_base()
 
 
 class Address(Base):
     __tablename__ = "addresses"
```

### Comparing `sqlalchemy_model_builder-0.2.0/pyproject.toml` & `sqlalchemy_model_builder-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sqlalchemy_model_builder-0.2.0/PKG-INFO` & `sqlalchemy_model_builder-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-model-builder
-Version: 0.2.0
+Version: 0.3.0
 Summary: SQLAlchemy Model Builder
 Project-URL: Documentation, https://github.com/aminalaee/sqlalchemy-model-builder
 Project-URL: Issues, https://github.com/aminalaee/sqlalchemy-model-builder/issues
 Project-URL: Source, https://github.com/aminalaee/sqlalchemy-model-builder
 Author-email: Amin Alaee <me@aminalaee.dev>
 License-Expression: MIT
 License-File: LICENSE
@@ -34,25 +34,25 @@
 - Build minimal (with required fields) only
 
 ---
 
 ## Installation
 
 ```shell
-$ pip install sqladmin
+$ pip install sqlalchemy-model-builder
 ```
 
 ---
 
 ## How to use
 Deinfe the SQLAlchemy models:
 
 ```python
+from sqlalchemy import Integer, String, Text
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql.sqltypes import Integer, String, Text
 
 Base = declarative_base()
 
 
 class Address(Base):
     __tablename__ = "addresses"
```

