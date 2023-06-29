# Comparing `tmp/syncqb-1.0.8.tar.gz` & `tmp/syncqb-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncqb-1.0.8.tar", last modified: Fri May  5 16:17:25 2023, max compression
+gzip compressed data, was "syncqb-1.0.9.tar", last modified: Fri Jun  2 15:01:38 2023, max compression
```

## Comparing `syncqb-1.0.8.tar` & `syncqb-1.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.8/LICENSE
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 16:17:25.613499 syncqb-1.0.8/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8642 2023-04-05 20:53:17.000000 syncqb-1.0.8/README.md
--rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-05-05 16:17:09.000000 syncqb-1.0.8/pyproject.toml
--rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-05-05 16:17:25.613499 syncqb-1.0.8/setup.cfg
--rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.8/setup.py
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.602666 syncqb-1.0.8/src/
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/src/syncqb/
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.8/src/syncqb/__init__.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.8/src/syncqb/__init__.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    17111 2023-05-05 16:16:45.000000 syncqb-1.0.8/src/syncqb/json_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)    13019 2023-05-05 15:40:29.000000 syncqb-1.0.8/src/syncqb/json_quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-05 15:50:43.000000 syncqb-1.0.8/src/syncqb/qb_client.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.8/src/syncqb/qb_client.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.8/src/syncqb/qb_errors.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.8/src/syncqb/qb_errors.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)     3274 2023-05-05 15:51:25.000000 syncqb-1.0.8/src/syncqb/quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.8/src/syncqb/quickbase.pyi
--rw-r--r--   0 jacob     (1000) jacob     (1000)    25524 2023-05-05 15:50:56.000000 syncqb-1.0.8/src/syncqb/xml_quickbase.py
--rw-r--r--   0 jacob     (1000) jacob     (1000)     8783 2023-04-07 14:18:50.000000 syncqb-1.0.8/src/syncqb/xml_quickbase.pyi
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/src/syncqb.egg-info/
--rw-r--r--   0 jacob     (1000) jacob     (1000)    10313 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/PKG-INFO
--rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/SOURCES.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/dependency_links.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/entry_points.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/requires.txt
--rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-05-05 16:17:25.000000 syncqb-1.0.8/src/syncqb.egg-info/top_level.txt
-drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-05-05 16:17:25.613499 syncqb-1.0.8/tests/
--rw-r--r--   0 jacob     (1000) jacob     (1000)     4225 2023-05-05 16:16:10.000000 syncqb-1.0.8/tests/test.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-06-02 15:01:38.065341 syncqb-1.0.9/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1073 2022-09-12 17:13:14.000000 syncqb-1.0.9/LICENSE
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10090 2023-06-02 15:01:38.065341 syncqb-1.0.9/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8419 2023-05-17 20:46:32.000000 syncqb-1.0.9/README.md
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      749 2023-06-02 14:50:44.000000 syncqb-1.0.9/pyproject.toml
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       38 2023-06-02 15:01:38.065341 syncqb-1.0.9/setup.cfg
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       82 2023-04-06 20:44:31.000000 syncqb-1.0.9/setup.py
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-06-02 15:01:38.025341 syncqb-1.0.9/src/
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-06-02 15:01:38.045341 syncqb-1.0.9/src/syncqb/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2022-09-12 14:58:01.000000 syncqb-1.0.9/src/syncqb/__init__.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        0 2023-03-29 20:36:22.000000 syncqb-1.0.9/src/syncqb/__init__.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    17111 2023-05-05 16:16:45.000000 syncqb-1.0.9/src/syncqb/json_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    13019 2023-05-05 15:40:29.000000 syncqb-1.0.9/src/syncqb/json_quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     2193 2023-05-05 15:50:43.000000 syncqb-1.0.9/src/syncqb/qb_client.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1665 2023-04-13 17:14:40.000000 syncqb-1.0.9/src/syncqb/qb_client.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1310 2023-04-07 16:31:57.000000 syncqb-1.0.9/src/syncqb/qb_errors.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     1046 2023-04-07 14:18:00.000000 syncqb-1.0.9/src/syncqb/qb_errors.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     3274 2023-05-05 15:51:25.000000 syncqb-1.0.9/src/syncqb/quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      588 2023-04-07 14:18:23.000000 syncqb-1.0.9/src/syncqb/quickbase.pyi
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    25624 2023-06-02 14:46:46.000000 syncqb-1.0.9/src/syncqb/xml_quickbase.py
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     8904 2023-06-02 14:46:02.000000 syncqb-1.0.9/src/syncqb/xml_quickbase.pyi
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-06-02 15:01:38.065341 syncqb-1.0.9/src/syncqb.egg-info/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)    10090 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/PKG-INFO
+-rw-r--r--   0 jacob     (1000) jacob     (1000)      571 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        1 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       59 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/entry_points.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)       44 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/requires.txt
+-rw-r--r--   0 jacob     (1000) jacob     (1000)        7 2023-06-02 15:01:37.000000 syncqb-1.0.9/src/syncqb.egg-info/top_level.txt
+drwxr-xr-x   0 jacob     (1000) jacob     (1000)        0 2023-06-02 15:01:38.065341 syncqb-1.0.9/tests/
+-rw-r--r--   0 jacob     (1000) jacob     (1000)     4225 2023-05-05 16:16:10.000000 syncqb-1.0.9/tests/test.py
```

### Comparing `syncqb-1.0.8/LICENSE` & `syncqb-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/PKG-INFO` & `syncqb-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -154,31 +154,22 @@
     print(e)
     #error handling code
 ```
 The `fields` parameter is a dictionary of values with their keys being the respective field IDs, the `database` parameter is the the table ID, and the `safemode` parameter determines whether the code will check for the primary key field in `fields` and return an error if it is present; this parameter is also optional for `add_multiple_records()`. There is also an `uploads` parameter that takes a file upload.
 
 Here is an example of `add_multiple_records()`*:
 ```python
-# data can either be nested like '6':{'value':value} or like '6':value
 data = [
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
 ]
 response = qb_client.add_multiple_records(data=data, database='dbid', return_fields=[3,6,7])
 # do stuff with response
 ```
 `data` is a list of dicts as shown above, `database` is the table ID, and `return_fields` is an optional list of field id's that you want returned.
 
@@ -218,17 +209,17 @@
     'value': 'b64_string',
     'field':7
 }
 qb_client.upload_file(rid=100, upload=upload, database=dbid)
 ```
 The `add_record()` method also takes an optional `uploads` parameter which takes a list set up like this: 
 ```python
-uploads = [fid: {"value" : { "fileName": filename, "data": base64encoded_file_content }}]
+uploads = [{'field': fid, 'filename': filename, 'value': b64_data}]
 ```
 
 ## Other features
 
 The `nest()` and `denest()` methods will convert data from `{fid:value}` to `{fid: {'value':value}}` and vice versa.
 The `import_from_csv()` method will take a csv string and upload the records contained in the string.
 The `round_ints()` method will take any returned data and change any unneeded floating-points to numbers. This method can be automatically called with an optional parameter `round_ints` in methods that return field data.
 
-For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.py or src/xml_quickbase.py.
+For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.pyi or src/xml_quickbase.pyi.
```

### Comparing `syncqb-1.0.8/README.md` & `syncqb-1.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,31 +122,22 @@
     print(e)
     #error handling code
 ```
 The `fields` parameter is a dictionary of values with their keys being the respective field IDs, the `database` parameter is the the table ID, and the `safemode` parameter determines whether the code will check for the primary key field in `fields` and return an error if it is present; this parameter is also optional for `add_multiple_records()`. There is also an `uploads` parameter that takes a file upload.
 
 Here is an example of `add_multiple_records()`*:
 ```python
-# data can either be nested like '6':{'value':value} or like '6':value
 data = [
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
 ]
 response = qb_client.add_multiple_records(data=data, database='dbid', return_fields=[3,6,7])
 # do stuff with response
 ```
 `data` is a list of dicts as shown above, `database` is the table ID, and `return_fields` is an optional list of field id's that you want returned.
 
@@ -186,17 +177,17 @@
     'value': 'b64_string',
     'field':7
 }
 qb_client.upload_file(rid=100, upload=upload, database=dbid)
 ```
 The `add_record()` method also takes an optional `uploads` parameter which takes a list set up like this: 
 ```python
-uploads = [fid: {"value" : { "fileName": filename, "data": base64encoded_file_content }}]
+uploads = [{'field': fid, 'filename': filename, 'value': b64_data}]
 ```
 
 ## Other features
 
 The `nest()` and `denest()` methods will convert data from `{fid:value}` to `{fid: {'value':value}}` and vice versa.
 The `import_from_csv()` method will take a csv string and upload the records contained in the string.
 The `round_ints()` method will take any returned data and change any unneeded floating-points to numbers. This method can be automatically called with an optional parameter `round_ints` in methods that return field data.
 
-For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.py or src/xml_quickbase.py.
+For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.pyi or src/xml_quickbase.pyi.
```

### Comparing `syncqb-1.0.8/pyproject.toml` & `syncqb-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0",'requests>=2.25.1','lxml>=4.6.3','chardet>=3.0.4']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "syncqb"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Jacob Gearhardt", email="jacob@synctivate.com" },
 ]
 description = "A Python SDK for quickbase"
 readme = "README.md"
 license = { file="LICENSE" }
 dependencies = [
```

### Comparing `syncqb-1.0.8/src/syncqb/json_quickbase.py` & `syncqb-1.0.9/src/syncqb/json_quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/json_quickbase.pyi` & `syncqb-1.0.9/src/syncqb/json_quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/qb_client.py` & `syncqb-1.0.9/src/syncqb/qb_client.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/qb_client.pyi` & `syncqb-1.0.9/src/syncqb/qb_client.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/qb_errors.py` & `syncqb-1.0.9/src/syncqb/qb_errors.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/qb_errors.pyi` & `syncqb-1.0.9/src/syncqb/qb_errors.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/quickbase.py` & `syncqb-1.0.9/src/syncqb/quickbase.py`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/quickbase.pyi` & `syncqb-1.0.9/src/syncqb/quickbase.pyi`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/src/syncqb/xml_quickbase.py` & `syncqb-1.0.9/src/syncqb/xml_quickbase.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,22 +407,24 @@
             self._build_xml(request),
             'UploadFile',
             'POST'
         )
 
         return self._parse_xml(response)
 
-    def import_from_csv(self, records_csv, clist, clist_output=None, skipfirst=False, database=None, required=None,
+    def import_from_csv(self, records_csv, clist, merge_field=None, clist_output=None, skipfirst=False, database=None, required=None,
                         chunk=None):
         # support function to generate import request and return response
         def _run_import(records_csv, clist, clist_output, skipfirst, database, required):
             request = {
                 'clist': '.'.join(str(c) for c in clist),
                 'records_csv': records_csv,
             }
+            if merge_field:
+                request['mergeFieldId'] = merge_field
             if clist_output:
                 request['clist_output'] = '.'.join(str(c) for c in clist_output)
 
             if skipfirst:
                 request['skipfirst'] = 1
 
             response = self._request(
```

### Comparing `syncqb-1.0.8/src/syncqb/xml_quickbase.pyi` & `syncqb-1.0.9/src/syncqb/xml_quickbase.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -120,19 +120,20 @@
         Upload a file to a Quickbase database
         :param rid: (str or int) The record ID
         :param upload: (dict) A dictionary of the file name and file contents and field ID
         :param database: (str or None) The Quickbase database ID (default None, will use self.database)
         :return: (dict) The response
         """
         ...
-    def import_from_csv(self, records_csv: str, clist: list[str | int], clist_output: list[str | int] | None = None, skipfirst: bool = False, 
+    def import_from_csv(self, records_csv: str, clist: list[str | int], merge_field: int | None = None, clist_output: list[str | int] | None = None, skipfirst: bool = False, 
                         database: str | None = None, required: list[str | int] | None = None, chunk: int | None = None) -> dict[str, Any]:
         """
         :param records_csv: (str) The records CSV string, comma separated with rows separated by newlines
         :param clist: (list of str) The column list
+        :param merge_field: (int or None) Field ID to merge existing data (default None)
         :param clist_output: (list of str) The column list output (default None)
         :param skipfirst: (bool) Whether to skip the first row (default False)
         :param database: (str or None) The Quickbase database ID (default None, will use self.database)
         :param required: (list of str or None) The required fields to return (default None)
         :param chunk: (int or None) Amount to chunk the records (default None, will split into chunks of given number of records if not none or 0 - USES MULTPLE API CALLS)
         :return: (dict) The response
         """
```

### Comparing `syncqb-1.0.8/src/syncqb.egg-info/PKG-INFO` & `syncqb-1.0.9/src/syncqb.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncqb
-Version: 1.0.8
+Version: 1.0.9
 Summary: A Python SDK for quickbase
 Author-email: Jacob Gearhardt <jacob@synctivate.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -154,31 +154,22 @@
     print(e)
     #error handling code
 ```
 The `fields` parameter is a dictionary of values with their keys being the respective field IDs, the `database` parameter is the the table ID, and the `safemode` parameter determines whether the code will check for the primary key field in `fields` and return an error if it is present; this parameter is also optional for `add_multiple_records()`. There is also an `uploads` parameter that takes a file upload.
 
 Here is an example of `add_multiple_records()`*:
 ```python
-# data can either be nested like '6':{'value':value} or like '6':value
 data = [
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
     {
-        '6': {
-            'value':value
-        },
-        '7': {
-            'value':value
-        },
+        '6': value
+        '7': value
     },
 ]
 response = qb_client.add_multiple_records(data=data, database='dbid', return_fields=[3,6,7])
 # do stuff with response
 ```
 `data` is a list of dicts as shown above, `database` is the table ID, and `return_fields` is an optional list of field id's that you want returned.
 
@@ -218,17 +209,17 @@
     'value': 'b64_string',
     'field':7
 }
 qb_client.upload_file(rid=100, upload=upload, database=dbid)
 ```
 The `add_record()` method also takes an optional `uploads` parameter which takes a list set up like this: 
 ```python
-uploads = [fid: {"value" : { "fileName": filename, "data": base64encoded_file_content }}]
+uploads = [{'field': fid, 'filename': filename, 'value': b64_data}]
 ```
 
 ## Other features
 
 The `nest()` and `denest()` methods will convert data from `{fid:value}` to `{fid: {'value':value}}` and vice versa.
 The `import_from_csv()` method will take a csv string and upload the records contained in the string.
 The `round_ints()` method will take any returned data and change any unneeded floating-points to numbers. This method can be automatically called with an optional parameter `round_ints` in methods that return field data.
 
-For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.py or src/xml_quickbase.py.
+For more information on these additional features and other features, you can look at their individual documentation in src/json_quickbase.pyi or src/xml_quickbase.pyi.
```

### Comparing `syncqb-1.0.8/src/syncqb.egg-info/SOURCES.txt` & `syncqb-1.0.9/src/syncqb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syncqb-1.0.8/tests/test.py` & `syncqb-1.0.9/tests/test.py`

 * *Files identical despite different names*

