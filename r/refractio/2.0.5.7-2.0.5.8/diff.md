# Comparing `tmp/refractio-2.0.5.7.tar.gz` & `tmp/refractio-2.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.5.7.tar", last modified: Tue Jun 27 10:35:40 2023, max compression
+gzip compressed data, was "refractio-2.0.5.8.tar", last modified: Thu Jun 29 13:12:55 2023, max compression
```

## Comparing `refractio-2.0.5.7.tar` & `refractio-2.0.5.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.766329 refractio-2.0.5.7/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-27 10:35:40.766329 refractio-2.0.5.7/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-27 10:34:00.000000 refractio-2.0.5.7/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.764329 refractio-2.0.5.7/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/postgres.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16508 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/snowflake.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6223 2023-06-27 10:34:00.000000 refractio-2.0.5.7/refractio/sqlserver.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-27 10:35:40.765329 refractio-2.0.5.7/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-27 10:35:40.000000 refractio-2.0.5.7/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-27 10:35:40.766329 refractio-2.0.5.7/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-27 10:34:00.000000 refractio-2.0.5.7/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.758445 refractio-2.0.5.8/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:12:55.758445 refractio-2.0.5.8/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     9330 2023-06-27 10:34:00.000000 refractio-2.0.5.8/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.756445 refractio-2.0.5.8/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      429 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     8058 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4151 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4488 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4795 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/postgres.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    16508 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5416 2023-06-27 10:34:00.000000 refractio-2.0.5.8/refractio/snowflake.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6332 2023-06-29 13:12:02.000000 refractio-2.0.5.8/refractio/sqlserver.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-06-29 13:12:55.757445 refractio-2.0.5.8/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    10052 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      412 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      584 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-06-29 13:12:55.000000 refractio-2.0.5.8/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-06-29 13:12:55.758445 refractio-2.0.5.8/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1978 2023-06-29 13:12:02.000000 refractio-2.0.5.8/setup.py
```

### Comparing `refractio-2.0.5.7/PKG-INFO` & `refractio-2.0.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.7
+Version: 2.0.5.8
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.7/README.md` & `refractio-2.0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/amazons3.py` & `refractio-2.0.5.8/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/azure.py` & `refractio-2.0.5.8/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/hive.py` & `refractio-2.0.5.8/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/manager.py` & `refractio-2.0.5.8/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/mysql.py` & `refractio-2.0.5.8/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/postgres.py` & `refractio-2.0.5.8/refractio/postgres.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/refractio.py` & `refractio-2.0.5.8/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/sftp.py` & `refractio-2.0.5.8/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/snowflake.py` & `refractio-2.0.5.8/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/refractio/sqlserver.py` & `refractio-2.0.5.8/refractio/sqlserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     def _get_connection(self):
         try:
             # Connect to Sqlserver
             import pyodbc
             # This need the OS should have sql server driver installed. Like,
             # sudo curl -o /etc/yum.repos.d/mssql-release.repo https://packages.microsoft.com/config/rhel/9.0/prod.repo
             # sudo ACCEPT_EULA=Y yum install -y msodbcsql18
-            driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+            # driver_lib = "/opt/microsoft/msodbcsql18/lib64/libmsodbcsql-18.2.so.1.1"    # sqlserver driver lib path
+            driver_lib = "{ODBC Driver 18 for SQL Server}"  # sqlserver driver version instead of lib path
             # todo: To update the keys here, once we have the connection manager API created for refractio.
             if self.__connection_details["params"]["READER"].get("database"):
                 connection_string = f'''DRIVER={driver_lib};
                 SERVER={self.__connection_details["params"]["READER"]["host"] if self.__connection_details["params"]["READER"].get("host") else self.__connection_details["params"]["READER"].get("ipAddress")};
                 UID={self.__connection_details["params"]["READER"].get("user") if self.__connection_details["params"]["READER"].get("user") else self.__connection_details["params"]["READER"].get("dbUserName")};
                 PWD={self.__connection_details["params"]["READER"].get("password") if self.__connection_details["params"]["READER"].get("password") else self.__connection_details["params"]["READER"].get("dbPassword")};
                 DATABASE={self.__connection_details["params"]["READER"].get("database")};
```

### Comparing `refractio-2.0.5.7/refractio.egg-info/PKG-INFO` & `refractio-2.0.5.8/refractio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.5.7
+Version: 2.0.5.8
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
```

### Comparing `refractio-2.0.5.7/refractio.egg-info/requires.txt` & `refractio-2.0.5.8/refractio.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `refractio-2.0.5.7/setup.py` & `refractio-2.0.5.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.5.7'
+VERSION = '2.0.5.8'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

