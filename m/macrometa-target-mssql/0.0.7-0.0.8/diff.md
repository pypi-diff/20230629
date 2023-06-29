# Comparing `tmp/macrometa-target-mssql-0.0.7.tar.gz` & `tmp/macrometa-target-mssql-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.7.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.8.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.7.tar` & `macrometa-target-mssql-0.0.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    33842 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 17:24:49.785449 macrometa-target-mssql-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.7/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 18:13:48.824964 macrometa-target-mssql-0.0.8/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 18:13:48.824964 macrometa-target-mssql-0.0.8/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    34142 2023-06-29 18:13:48.828964 macrometa-target-mssql-0.0.8/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 18:13:49.076965 macrometa-target-mssql-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.8/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.8/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.7/LICENSE` & `macrometa-target-mssql-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.7/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.8/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.7/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.8/macrometa_target_mssql/db_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,29 +252,30 @@
                 self.grantees = config_schema_mapping[stream_schema_name].get('target_schema_select_permissions',
                                                                               self.grantees)
 
             self.data_flattening_max_level = self.connection_config.get('data_flattening_max_level', 0)
             self.flatten_schema = flatten_schema(stream_schema_message['schema'],
                                                  max_level=self.data_flattening_max_level)
 
-    def open_connection(self):
+    def open_connection(self, require_database=True):
         args = {
             "user": self.connection_config.get("user"),
             "password": self.connection_config.get("password"),
             "server": self.connection_config["host"],
-            "database": self.connection_config.get("database", "master"),
             "charset": self.connection_config.get("characterset", "utf8"),
             "port": self.connection_config.get("port", "1433"),
             "tds_version": self.connection_config.get("tds_version", "7.3")
         }
+        if require_database:
+            args["database"] = self.connection_config["database"]
         return pymssql.connect(**args)
 
-    def query(self, query, params=None):
+    def query(self, query, params=None, require_database=True):
         self.logger.info("Running query: %s , params: %s", query, params)
-        with self.open_connection() as connection:
+        with self.open_connection(require_database=require_database) as connection:
             with connection.cursor(as_dict=True) as cur:
                 cur.execute(
                     query,
                     params
                 )
 
                 if cur.rowcount > 0:
@@ -696,15 +697,15 @@
                     AND name = '{index_name}'
             )
             BEGIN
                 CREATE INDEX {index_name} ON {table} ({column});
             END"""
         self.logger.info("Creating index on '%s' table on '%s' column(s)... %s", table, column, query)
         try:
-            self.query(query)
+            self.query(query, require_database=False)
         except Exception as e:
             self.logger.warn(f"Failed to create index, error: {e}")
 
     def create_indices(self, stream):
         if isinstance(self.indices, list):
             for index in self.indices:
                 self.create_index(stream, index)
@@ -723,35 +724,38 @@
         # table_columns_cache is an optional pre-collected list of available objects in mssql
         if table_columns_cache:
             schema_rows = list(filter(lambda x: x['TABLE_SCHEMA'] == schema_name, table_columns_cache))
         # Query realtime if not pre-collected
         else:
             self.logger.info("reached here..")
             schema_rows = self.query(
-                f"SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = '{schema_name.lower()}'"
+                f"SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = '{schema_name.lower()}'",
+                require_database=False
             )
             self.logger.info(f"schema rows: {schema_rows}")
 
         if len(schema_rows) == 0:
             query = "CREATE SCHEMA {}".format(schema_name)
             self.logger.info("Schema '%s' does not exist. Creating... %s", schema_name, query)
             self.query(query)
 
             self.grant_privilege(schema_name, self.grantees, self.grant_usage_on_schema)
 
     def get_tables(self):
         return self.query(
-            f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.schema_name}'"
+            f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.schema_name}'",
+            require_database=False
         )
 
     def get_table_columns(self, table_name):
         return self.query("""SELECT column_name, data_type
       FROM information_schema.columns
-      WHERE lower(table_name) = %s AND lower(table_schema) = %s""", (table_name.replace("\"", "").lower(),
-                                                                     self.schema_name.lower()))
+      WHERE lower(table_name) = %s AND lower(table_schema) = %s""", params=(table_name.replace("\"", "").lower(),
+                                                                     self.schema_name.lower()),
+                                                                     require_database=False)
 
     def update_columns(self):
         stream_schema_message = self.stream_schema_message
         stream = stream_schema_message['stream']
         table_name = self.table_name(stream, without_schema=True)
         columns = self.get_table_columns(table_name)
         columns_dict = {column['column_name'].lower(): column for column in columns}
```

### Comparing `macrometa-target-mssql-0.0.7/pyproject.toml` & `macrometa-target-mssql-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.7'
+version='0.0.8'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.7/setup.py` & `macrometa-target-mssql-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.7',
+    'version': '0.0.8',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.7/PKG-INFO` & `macrometa-target-mssql-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.7
+Version: 0.0.8
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

