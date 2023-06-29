# Comparing `tmp/macrometa-target-mssql-0.0.4.tar.gz` & `tmp/macrometa-target-mssql-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.4.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.5.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.4.tar` & `macrometa-target-mssql-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    33682 2023-06-29 15:19:20.871932 macrometa-target-mssql-0.0.4/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 15:19:21.111929 macrometa-target-mssql-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.4/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 15:49:19.326507 macrometa-target-mssql-0.0.5/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 15:49:19.330507 macrometa-target-mssql-0.0.5/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    33874 2023-06-29 15:49:19.330507 macrometa-target-mssql-0.0.5/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 15:49:19.582477 macrometa-target-mssql-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.5/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.5/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.4/LICENSE` & `macrometa-target-mssql-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.4/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.5/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.4/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.5/macrometa_target_mssql/db_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,23 +265,24 @@
             "charset": self.connection_config.get("characterset", "utf8"),
             "port": self.connection_config.get("port", "1433"),
             "tds_version": self.connection_config.get("tds_version", "7.3")
         }
         return pymssql.connect(**args)
 
     def query(self, query, params=None):
-        self.logger.debug("Running query: %s", query)
+        self.logger.info("Running query: %s , params: %s", query, params)
         with self.open_connection() as connection:
             with connection.cursor(as_dict=True) as cur:
                 cur.execute(
                     query,
                     params
                 )
 
                 if cur.rowcount > 0:
+                    self.logger.info(f"rowcount:{cur.rowcount}")
                     return cur.fetchall()
 
                 return []
 
     def table_name(self, stream_name, is_temporary=False, without_schema=False):
         config_target_table = self.connection_config.get('target_table', '').strip()
         stream_dict = stream_name_to_dict(stream_name, table_name=config_target_table)
@@ -720,18 +721,20 @@
         schema_rows = 0
 
         # table_columns_cache is an optional pre-collected list of available objects in mssql
         if table_columns_cache:
             schema_rows = list(filter(lambda x: x['TABLE_SCHEMA'] == schema_name, table_columns_cache))
         # Query realtime if not pre-collected
         else:
+            self.logger.info("reached here..")
             schema_rows = self.query(
                 'SELECT LOWER(schema_name) schema_name FROM information_schema.schemata WHERE LOWER(schema_name) = %s',
                 (schema_name.lower(),)
             )
+            self.logger.info(f"schema rows: {schema_rows}")
 
         if len(schema_rows) == 0:
             query = "CREATE SCHEMA {}".format(schema_name)
             self.logger.info("Schema '%s' does not exist. Creating... %s", schema_name, query)
             self.query(query)
 
             self.grant_privilege(schema_name, self.grantees, self.grant_usage_on_schema)
```

### Comparing `macrometa-target-mssql-0.0.4/pyproject.toml` & `macrometa-target-mssql-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.4'
+version='0.0.5'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.4/setup.py` & `macrometa-target-mssql-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.4',
+    'version': '0.0.5',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.4/PKG-INFO` & `macrometa-target-mssql-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.4
+Version: 0.0.5
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

