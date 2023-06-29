# Comparing `tmp/macrometa-target-mssql-0.0.3.tar.gz` & `tmp/macrometa-target-mssql-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.3.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.4.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.3.tar` & `macrometa-target-mssql-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    34913 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 11:43:01.926731 macrometa-target-mssql-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.3/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    33682 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 15:19:21.111929 macrometa-target-mssql-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.4/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.4/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.3/LICENSE` & `macrometa-target-mssql-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.3/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.4/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.3/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.4/macrometa_target_mssql/db_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,60 +38,18 @@
     config_schema_mapping = config.get('schema_mapping', None)
     if not config_default_target_schema and not config_schema_mapping:
         errors.append("Neither 'default_target_schema' (string) nor 'schema_mapping' (object) keys set in config.")
 
     return errors
 
 
-# pylint: disable=fixme
-def column_type(schema_property):
-    property_type = schema_property['type']
-    property_format = schema_property['format'] if 'format' in schema_property else None
-    col_type = 'character varying'
-    if 'object' in property_type or 'array' in property_type:
-        col_type = 'jsonb'
-
-    # Every date-time JSON value is currently mapped to TIMESTAMP WITHOUT TIME ZONE
-    #
-    # TODO: Detect if timezone postfix exists in the JSON and find if TIMESTAMP WITHOUT TIME ZONE or
-    # TIMESTAMP WITH TIME ZONE is the better column type
-    elif property_format == 'date-time':
-        col_type = 'timestamp without time zone'
-    elif property_format == 'time':
-        col_type = 'time without time zone'
-    elif 'number' in property_type:
-        col_type = 'double precision'
-    elif 'integer' in property_type and 'string' in property_type:
-        col_type = 'character varying'
-    elif 'integer' in property_type:
-        if 'maximum' in schema_property:
-            if schema_property['maximum'] <= 32767:
-                col_type = 'smallint'
-            elif schema_property['maximum'] <= 2147483647:
-                col_type = 'integer'
-            elif schema_property['maximum'] <= 9223372036854775807:
-                col_type = 'bigint'
-        else:
-            col_type = 'numeric'
-    elif 'boolean' in property_type:
-        col_type = 'boolean'
-
-    get_logger('macrometa_target_mssql').debug("schema_property: %s -> col_type: %s", schema_property, col_type)
-
-    return col_type
-
-
 def safe_column_name(name):
     return '"{}"'.format(name).lower()
 
 
-def column_clause(name, schema_property):
-    return '{} {}'.format(safe_column_name(name), column_type(schema_property))
-
-
 def flatten_key(k, parent_key, sep):
     full_key = parent_key + [k]
     inflected_key = full_key.copy()
     reducer_index = 0
     while len(sep.join(inflected_key)) >= 63 and reducer_index < len(inflected_key):
         reduced_key = re.sub(r'[a-z]', '', inflection.camelize(inflected_key[reducer_index]))
         inflected_key[reducer_index] = \
@@ -465,15 +423,14 @@
         if "string" in type_dict.get("type", []) and type_dict.get("format") in {
             "date-time",
             "time",
             "date",
         }:
             return True
 
-
     def get_datelike_property_type(self, property_schema: Dict) -> Optional[str]:
         """Return one of 'date-time', 'time', or 'date' if property is date-like.
 
         Otherwise return None.
         """
         if self._is_string_with_format(property_schema):
             return cast(str, property_schema["format"])
@@ -526,14 +483,17 @@
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR())
 
         if self._jsonschema_type_check(jsonschema_type, ("array",)):
             return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.JSON())
 
         return cast(sqlalchemy.types.TypeEngine, sqlalchemy.types.VARCHAR())
 
+    def column_clause(self, name, schema_property):
+        return '{} {}'.format(safe_column_name(name), self.to_sql_type(schema_property))
+
     def create_temp_table_from_table(self, from_table_name):
         """Temp table from another table."""
 
         db_name, schema_name, table_name = self.parse_full_table_name(from_table_name)
         full_table_name = (
             f"{schema_name}.{table_name}" if schema_name else f"{table_name}"
         )
@@ -558,15 +518,15 @@
         in order to provide a more efficient upload/upsert process.
         Args:
             records: List of records to load into database.
         """
 
         key_properties = self.stream_schema_message['key_properties']
         join_keys = list(key_properties)
-        schema = self.flatten_schema
+        schema = self.stream_schema_message['schema']
 
         stream_schema_message = self.stream_schema_message
         full_table_name = self.table_name(stream_schema_message['stream'], is_temporary=False)
         if key_properties:
             # Create a temp table (Creates from the table above)
             db_name, schema_name, table_name = self.parse_full_table_name(
                 full_table_name
@@ -680,29 +640,28 @@
 
     def column_names(self):
         return [safe_column_name(name) for name in self.flatten_schema]
 
     def create_table_query(self, table_name=None, is_temporary=False):
         stream_schema_message = self.stream_schema_message
         columns = [
-            column_clause(
+            self.column_clause(
                 name,
                 schema
             )
             for (name, schema) in self.flatten_schema.items()
         ]
 
         primary_key = ["PRIMARY KEY ({})".format(', '.join(primary_column_names(stream_schema_message)))] \
             if len(stream_schema_message['key_properties']) > 0 else []
 
         if not table_name:
             gen_table_name = self.table_name(stream_schema_message['stream'], is_temporary=is_temporary)
 
-        return 'CREATE {}TABLE IF NOT EXISTS {} ({})'.format(
-            'TEMP ' if is_temporary else '',
+        return 'CREATE TABLE {} ({})'.format(
             table_name if table_name else gen_table_name,
             ', '.join(columns + primary_key)
         )
 
     def grant_usage_on_schema(self, schema_name, grantee):
         query = "GRANT USAGE ON SCHEMA {} TO GROUP {}".format(schema_name, grantee)
         self.logger.info("Granting USAGE privilege on '%s' schema to '%s'... %s", schema_name, grantee, query)
@@ -725,28 +684,40 @@
             grant_method(schema, grantees)
 
     def create_index(self, stream, column):
         table = self.table_name(stream)
         table_without_schema = self.table_name(stream, without_schema=True)
         index_name = 'i_{}_{}'.format(table_without_schema[:30].replace(' ', '').replace('"', ''),
                                       column.replace(',', '_'))
-        query = "CREATE INDEX IF NOT EXISTS {} ON {} ({})".format(index_name, table, column)
+        query = f"""IF NOT EXISTS (
+                SELECT 1
+                FROM sys.indexes
+                WHERE object_id = OBJECT_ID('{table}')
+                    AND name = '{index_name}'
+            )
+            BEGIN
+                CREATE INDEX {index_name} ON {table} ({column});
+            END"""
         self.logger.info("Creating index on '%s' table on '%s' column(s)... %s", table, column, query)
-        self.query(query)
+        try:
+            self.query(query)
+        except Exception as e:
+            self.logger.warn(f"Failed to create index, error: {e}")
 
     def create_indices(self, stream):
         if isinstance(self.indices, list):
             for index in self.indices:
                 self.create_index(stream, index)
 
     def delete_rows(self, stream):
         table = self.table_name(stream)
-        query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL RETURNING _sdc_deleted_at".format(table)
+        query = "DELETE FROM {} WHERE _sdc_deleted_at IS NOT NULL".format(table)
         self.logger.info("Deleting rows from '%s' table... %s", table, query)
-        self.logger.info("DELETE %s", len(self.query(query)))
+        self.query(query)
+        self.logger.info("Delete query completed.")
 
     def create_schema_if_not_exists(self, table_columns_cache=None):
         schema_name = self.schema_name
         schema_rows = 0
 
         # table_columns_cache is an optional pre-collected list of available objects in mssql
         if table_columns_cache:
@@ -755,15 +726,15 @@
         else:
             schema_rows = self.query(
                 'SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = %s',
                 (schema_name.lower(),)
             )
 
         if len(schema_rows) == 0:
-            query = "CREATE SCHEMA IF NOT EXISTS {}".format(schema_name)
+            query = "CREATE SCHEMA {}".format(schema_name)
             self.logger.info("Schema '%s' does not exist. Creating... %s", schema_name, query)
             self.query(query)
 
             self.grant_privilege(schema_name, self.grantees, self.grant_usage_on_schema)
 
     def get_tables(self):
         return self.query(
@@ -781,46 +752,46 @@
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
         table_name = self.table_name(stream, without_schema=True)
         columns = self.get_table_columns(table_name)
         columns_dict = {column['column_name'].lower(): column for column in columns}
 
         columns_to_add = [
-            column_clause(
+            self.column_clause(
                 name,
                 properties_schema
             )
             for (name, properties_schema) in self.flatten_schema.items()
             if name.lower() not in columns_dict
         ]
 
         for column in columns_to_add:
             self.add_column(column, stream)
 
         columns_to_replace = [
-            (safe_column_name(name), column_clause(
+            (safe_column_name(name), self.column_clause(
                 name,
                 properties_schema
             ))
             for (name, properties_schema) in self.flatten_schema.items()
             if name.lower() in columns_dict and
-            columns_dict[name.lower()]['data_type'].lower() != column_type(properties_schema).lower()
+            columns_dict[name.lower()]['data_type'].lower() != self.to_sql_type(properties_schema).lower()
         ]
 
         for (column_name, column) in columns_to_replace:
             self.version_column(column_name, stream)
             self.add_column(column, stream)
 
     def drop_column(self, column_name, stream):
         drop_column = "ALTER TABLE {} DROP COLUMN {}".format(self.table_name(stream), column_name)
         self.logger.info('Dropping column: %s', drop_column)
         self.query(drop_column)
 
     def version_column(self, column_name, stream):
-        version_column = "ALTER TABLE {} RENAME COLUMN {} TO \"{}_{}\"".format(self.table_name(stream, False),
+        version_column = "EXEC sp_rename '{}.{}', '{}_{}', 'COLUMN';".format(self.table_name(stream, False),
                                                                                column_name,
                                                                                column_name.replace("\"", ""),
                                                                                time.strftime("%Y%m%d_%H%M"))
         self.logger.info('Versioning column: %s', version_column)
         self.query(version_column)
 
     def add_column(self, column, stream):
```

### Comparing `macrometa-target-mssql-0.0.3/pyproject.toml` & `macrometa-target-mssql-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.3'
+version='0.0.4'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.3/setup.py` & `macrometa-target-mssql-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.3',
+    'version': '0.0.4',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.3/PKG-INFO` & `macrometa-target-mssql-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.3
+Version: 0.0.4
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

