# Comparing `tmp/macrometa-target-mssql-0.0.2.tar.gz` & `tmp/macrometa-target-mssql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-mssql-0.0.2.tar", max compression
+gzip compressed data, was "macrometa-target-mssql-0.0.3.tar", max compression
```

## Comparing `macrometa-target-mssql-0.0.2.tar` & `macrometa-target-mssql-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-29 10:33:40.147972 macrometa-target-mssql-0.0.2/LICENSE
--rw-r--r--   0        0        0    24115 2023-06-29 10:33:40.147972 macrometa-target-mssql-0.0.2/macrometa_target_mssql/__init__.py
--rw-r--r--   0        0        0    34908 2023-06-29 10:33:40.151972 macrometa-target-mssql-0.0.2/macrometa_target_mssql/db_sync.py
--rw-r--r--   0        0        0     1554 2023-06-29 10:33:40.399974 macrometa-target-mssql-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.2/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/LICENSE
+-rw-r--r--   0        0        0    24115 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/macrometa_target_mssql/__init__.py
+-rw-r--r--   0        0        0    34913 2023-06-29 11:43:01.678732 macrometa-target-mssql-0.0.3/macrometa_target_mssql/db_sync.py
+-rw-r--r--   0        0        0     1554 2023-06-29 11:43:01.926731 macrometa-target-mssql-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.3/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 macrometa-target-mssql-0.0.3/PKG-INFO
```

### Comparing `macrometa-target-mssql-0.0.2/LICENSE` & `macrometa-target-mssql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.2/macrometa_target_mssql/__init__.py` & `macrometa-target-mssql-0.0.3/macrometa_target_mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-mssql-0.0.2/macrometa_target_mssql/db_sync.py` & `macrometa-target-mssql-0.0.3/macrometa_target_mssql/db_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,20 +304,20 @@
             "password": self.connection_config.get("password"),
             "server": self.connection_config["host"],
             "database": self.connection_config.get("database", "master"),
             "charset": self.connection_config.get("characterset", "utf8"),
             "port": self.connection_config.get("port", "1433"),
             "tds_version": self.connection_config.get("tds_version", "7.3")
         }
-        return pymssql._mssql.connect(**args)
+        return pymssql.connect(**args)
 
     def query(self, query, params=None):
         self.logger.debug("Running query: %s", query)
         with self.open_connection() as connection:
-            with connection.cursor() as cur:
+            with connection.cursor(as_dict=True) as cur:
                 cur.execute(
                     query,
                     params
                 )
 
                 if cur.rowcount > 0:
                     return cur.fetchall()
```

### Comparing `macrometa-target-mssql-0.0.2/pyproject.toml` & `macrometa-target-mssql-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-target-mssql"
-version='0.0.2'
+version='0.0.3'
 description = "Macrometa target connector for writing data into Microsoft SQL Server."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-target-mssql-0.0.2/setup.py` & `macrometa-target-mssql-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'sqlalchemy>=1.4,<2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-target-mssql = macrometa_target_mssql:main']}
 
 setup_kwargs = {
     'name': 'macrometa-target-mssql',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Macrometa target connector for writing data into Microsoft SQL Server.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-target-mssql-0.0.2/PKG-INFO` & `macrometa-target-mssql-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-mssql
-Version: 0.0.2
+Version: 0.0.3
 Summary: Macrometa target connector for writing data into Microsoft SQL Server.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,Target,MicrosoftSQLServer
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

