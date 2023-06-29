# Comparing `tmp/macrometa-target-mssql-0.0.1.tar.gz` & `tmp/macrometa-target-mssql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.1.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.2.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.1.tar` & `macrometa-target-mssql-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 09:30:53.529438 macrometa-target-mssql-0.0.1/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 09:30:53.529438 macrometa-target-mssql-0.0.1/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    34970 2023-06-29 09:30:53.529438 macrometa-target-mssql-0.0.1/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 09:30:53.829461 macrometa-target-mssql-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.1/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 10:33:40.147972 macrometa-target-mssql-0.0.2/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 10:33:40.147972 macrometa-target-mssql-0.0.2/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    34908 2023-06-29 10:33:40.151972 macrometa-target-mssql-0.0.2/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 10:33:40.399974 macrometa-target-mssql-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.2/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.2/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.1/LICENSE` & `macrometa-target-mssql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.1/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.2/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.1/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.2/macrometa_target_mssql/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -646,31 +646,31 @@
                 VALUES ({", ".join([f"temp.{key}" for key in schema["properties"].keys()])});
         """  # nosec
 
         self.query(merge_sql)
 
     def parse_full_table_name(
         self, full_table_name: str
-    ) -> tuple[str | None, str | None, str]:
+    ):
         """Parse a fully qualified table name into its parts.
         Developers may override this method if their platform does not support the
         traditional 3-part convention: `db_name.schema_name.table_name`
         Args:
             full_table_name: A table name or a fully qualified table name. Depending on
                 SQL the platform, this could take the following forms:
                 - `<db>.<schema>.<table>` (three part names)
                 - `<db>.<table>` (platforms which do not use schema groupings)
                 - `<schema>.<name>` (if DB name is already in context)
                 - `<table>` (if DB name and schema name are already in context)
         Returns:
             A three part tuple (db_name, schema_name, table_name) with any unspecified
             or unused parts returned as None.
         """
-        db_name: str | None = None
-        schema_name: str | None = None
+        db_name = None
+        schema_name = None
 
         parts = full_table_name.split(".")
         if len(parts) == 1:
             table_name = full_table_name
         if len(parts) == 2:
             schema_name, table_name = parts
         if len(parts) == 3:
```

### Comparing `macrometa-target-mssql-0.0.1/pyproject.toml` & `macrometa-target-mssql-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.1'
+version='0.0.2'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.1/setup.py` & `macrometa-target-mssql-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.1/PKG-INFO` & `macrometa-target-mssql-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.1
+Version: 0.0.2
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

