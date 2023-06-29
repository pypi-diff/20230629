# Comparing `tmp/macrometa-target-mssql-0.0.6.tar.gz` & `tmp/macrometa-target-mssql-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.6.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.7.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.6.tar` & `macrometa-target-mssql-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 17:14:09.721344 macrometa-target-mssql-0.0.6/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 17:14:09.721344 macrometa-target-mssql-0.0.6/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    33868 2023-06-29 17:14:09.721344 macrometa-target-mssql-0.0.6/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 17:14:09.965344 macrometa-target-mssql-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.6/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    33842 2023-06-29 17:24:49.429447 macrometa-target-mssql-0.0.7/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 17:24:49.785449 macrometa-target-mssql-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.7/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.7/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.6/LICENSE` & `macrometa-target-mssql-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.6/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.7/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.6/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.7/macrometa_target_mssql/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -723,30 +723,28 @@
         # table_columns_cache is an optional pre-collected list of available objects in mssql
         if table_columns_cache:
             schema_rows = list(filter(lambda x: x['TABLE_SCHEMA'] == schema_name, table_columns_cache))
         # Query realtime if not pre-collected
         else:
             self.logger.info("reached here..")
             schema_rows = self.query(
-                'SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = %s',
-                schema_name.lower()
+                f"SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = '{schema_name.lower()}'"
             )
             self.logger.info(f"schema rows: {schema_rows}")
 
         if len(schema_rows) == 0:
             query = "CREATE SCHEMA {}".format(schema_name)
             self.logger.info("Schema '%s' does not exist. Creating... %s", schema_name, query)
             self.query(query)
 
             self.grant_privilege(schema_name, self.grantees, self.grant_usage_on_schema)
 
     def get_tables(self):
         return self.query(
-            'SELECT table_name FROM information_schema.tables WHERE table_schema = %s',
-            self.schema_name
+            f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.schema_name}'"
         )
 
     def get_table_columns(self, table_name):
         return self.query("""SELECT column_name, data_type
       FROM information_schema.columns
       WHERE lower(table_name) = %s AND lower(table_schema) = %s""", (table_name.replace("\"", "").lower(),
                                                                      self.schema_name.lower()))
```

### Comparing `macrometa-target-mssql-0.0.6/pyproject.toml` & `macrometa-target-mssql-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.6'
+version='0.0.7'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.6/setup.py` & `macrometa-target-mssql-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.6',
+    'version': '0.0.7',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.6/PKG-INFO` & `macrometa-target-mssql-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.6
+Version: 0.0.7
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

