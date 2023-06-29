# Comparing `tmp/refractio-2.0.5.8.tar.gz` & `tmp/refractio-2.0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.8.tar", last modified: Thu Jun 29 13:12:55 2023, max compression
+gzip compressed data, was "refractio-2.0.5.9.tar", last modified: Thu Jun 29 13:30:27 2023, max compression
```

## Comparing `refractio-2.0.5.8.tar` & `refractio-2.0.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.758445 refractio-2.0.5.8/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:12:55.758445 refractio-2.0.5.8/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-27 10:34:00.000000 refractio-2.0.5.8/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.756445 refractio-2.0.5.8/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16508 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6332 2023-06-29 13:12:02.000000 refractio-2.0.5.8/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.757445 refractio-2.0.5.8/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-29 13:12:55.758445 refractio-2.0.5.8/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-29 13:12:02.000000 refractio-2.0.5.8/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:30:27.796481 refractio-2.0.5.9/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:30:27.796481 refractio-2.0.5.9/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-29 13:29:32.000000 refractio-2.0.5.9/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:30:27.795482 refractio-2.0.5.9/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4163 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16609 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6332 2023-06-29 13:29:32.000000 refractio-2.0.5.9/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:30:27.796481 refractio-2.0.5.9/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:30:27.000000 refractio-2.0.5.9/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-29 13:30:27.000000 refractio-2.0.5.9/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-29 13:30:27.000000 refractio-2.0.5.9/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-29 13:30:27.000000 refractio-2.0.5.9/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-29 13:30:27.000000 refractio-2.0.5.9/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-29 13:30:27.796481 refractio-2.0.5.9/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-29 13:29:32.000000 refractio-2.0.5.9/setup.py
```

### Comparing `refractio-2.0.5.8/PKG-INFO` & `refractio-2.0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.8
+Version: 2.0.5.9
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.8/README.md` & `refractio-2.0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/amazons3.py` & `refractio-2.0.5.9/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/azure.py` & `refractio-2.0.5.9/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/hive.py` & `refractio-2.0.5.9/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/manager.py` & `refractio-2.0.5.9/refractio/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,14 +98,14 @@
     :param filter_condition:
     :param top:
     :return: query
     """
     query = f"SELECT * FROM {table_name}"
     if top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
-        query = f"SELECT TOP * FROM {table_name}"
+        query = f"SELECT TOP {row_count} * FROM {table_name}"
     if filter_condition:
         query = query + " " + filter_condition
     if not top and int(row_count) > 0:
         print(f"fetching {row_count} records!")
         query = f"{query} LIMIT {row_count}"
     return query
```

### Comparing `refractio-2.0.5.8/refractio/mysql.py` & `refractio-2.0.5.9/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/postgres.py` & `refractio-2.0.5.9/refractio/postgres.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/refractio.py` & `refractio-2.0.5.9/refractio/refractio.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,16 @@
     """
     print("Reading dataframe from sqlserver native connector")
     import pyodbc
 
     # This need the OS should have sql server driver installed. Like,
     # curl https://packages.microsoft.com/config/rhel/9.0/prod.repo > /etc/yum.repos.d/mssql-release.repo
     # ACCEPT_EULA=Y yum install -y msodbcsql18
-    driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+    # driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+    driver_lib = "{ODBC Driver 18 for SQL Server}"  # sqlserver driver version instead of lib path
     conn = pyodbc.connect(f'DRIVER={driver_lib};'
                           f'SERVER={connection_details["params"]["READER"]["host"]};'
                           f'DATABASE={connection_details["params"]["READER"]["database"]};'
                           f'UID={connection_details["params"]["READER"]["user"]};'
                           f'PWD={connection_details["params"]["READER"]["password"]};'
                           f'TrustServerCertificate=yes;')
```

### Comparing `refractio-2.0.5.8/refractio/sftp.py` & `refractio-2.0.5.9/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/snowflake.py` & `refractio-2.0.5.9/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio/sqlserver.py` & `refractio-2.0.5.9/refractio/sqlserver.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.9/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.8
+Version: 2.0.5.9
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.8/refractio.egg-info/requires.txt` & `refractio-2.0.5.9/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.8/setup.py` & `refractio-2.0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.8'
+VERSION = '2.0.5.9'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

