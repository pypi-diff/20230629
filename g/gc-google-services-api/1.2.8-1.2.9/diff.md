# Comparing `tmp/gc_google_services_api-1.2.8.tar.gz` & `tmp/gc_google_services_api-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gc_google_services_api-1.2.8.tar", max compression
+gzip compressed data, was "gc_google_services_api-1.2.9.tar", max compression
```

## Comparing `gc_google_services_api-1.2.8.tar` & `gc_google_services_api-1.2.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/LICENSE
--rw-r--r--   0        0        0     4789 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/README.md
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/__init__.py
--rw-r--r--   0        0        0      796 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/auth/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/auth/__tests__/__init__.py
--rw-r--r--   0        0        0     2168 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/auth/__tests__/test_auth.py
--rw-r--r--   0        0        0     1995 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/bigquery/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/bigquery/__tests__/__init__.py
--rw-r--r--   0        0        0      988 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/bigquery/__tests__/test_bigquery.py
--rw-r--r--   0        0        0     4192 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/calendar_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/calendar_api/__tests__/__init__.py
--rw-r--r--   0        0        0     7927 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/calendar_api/__tests__/test_calendar.py
--rw-r--r--   0        0        0     1711 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gmail/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gmail/__tests__/__init__.py
--rw-r--r--   0        0        0     2827 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gmail/__tests__/test_gmail.py
--rw-r--r--   0        0        0     2085 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gsheet/__init__.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gsheet/__tests__/__init__.py
--rw-r--r--   0        0        0     3635 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/gsheet/__tests__/test_gsheet.py
--rw-r--r--   0        0        0        0 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/permissions/__init__.py
--rw-r--r--   0        0        0     3281 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/permissions/drive.py
--rw-r--r--   0        0        0     3506 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/gc_google_services_api/permissions/workspace.py
--rw-r--r--   0        0        0      656 2023-06-29 08:38:21.012877 gc_google_services_api-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/LICENSE
+-rw-r--r--   0        0        0     4789 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/__init__.py
+-rw-r--r--   0        0        0      796 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/__init__.py
+-rw-r--r--   0        0        0     2168 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/test_auth.py
+-rw-r--r--   0        0        0     2106 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/__init__.py
+-rw-r--r--   0        0        0      988 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/test_bigquery.py
+-rw-r--r--   0        0        0     4192 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/__init__.py
+-rw-r--r--   0        0        0     7927 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/test_calendar.py
+-rw-r--r--   0        0        0     1711 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/__init__.py
+-rw-r--r--   0        0        0     2827 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/test_gmail.py
+-rw-r--r--   0        0        0     2085 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/__init__.py
+-rw-r--r--   0        0        0     3635 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/test_gsheet.py
+-rw-r--r--   0        0        0        0 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/__init__.py
+-rw-r--r--   0        0        0     3281 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/drive.py
+-rw-r--r--   0        0        0     3506 2023-06-29 08:51:32.348630 gc_google_services_api-1.2.9/gc_google_services_api/permissions/workspace.py
+-rw-r--r--   0        0        0      656 2023-06-29 08:51:32.352630 gc_google_services_api-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     5447 1970-01-01 00:00:00.000000 gc_google_services_api-1.2.9/PKG-INFO
```

### Comparing `gc_google_services_api-1.2.8/LICENSE` & `gc_google_services_api-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/README.md` & `gc_google_services_api-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/auth/__init__.py` & `gc_google_services_api-1.2.9/gc_google_services_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/auth/__tests__/test_auth.py` & `gc_google_services_api-1.2.9/gc_google_services_api/auth/__tests__/test_auth.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/bigquery/__init__.py` & `gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,22 +5,28 @@
 from google.cloud import bigquery
 
 logging.basicConfig(
     level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
 )
 
 
+def wait_for_job(query_job):
+    retry = Retry()
+    retry(query_job.result)
+
+
 def execute_query(query="", error_value=[]):
     """
     DEPRECATED: Now use BigQueryManager class instead this method.
     """
     client = bigquery.Client()
     query_job = client.query(query)
 
     try:
+        wait_for_job(query_job)
         return query_job.result()
     except Exception as e:
         print("[ERROR]: ", e)
         return error_value
 
 
 class BigQueryManager:
```

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/bigquery/__tests__/test_bigquery.py` & `gc_google_services_api-1.2.9/gc_google_services_api/bigquery/__tests__/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/calendar_api/__init__.py` & `gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/calendar_api/__tests__/test_calendar.py` & `gc_google_services_api-1.2.9/gc_google_services_api/calendar_api/__tests__/test_calendar.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/gmail/__init__.py` & `gc_google_services_api-1.2.9/gc_google_services_api/gmail/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/gmail/__tests__/test_gmail.py` & `gc_google_services_api-1.2.9/gc_google_services_api/gmail/__tests__/test_gmail.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/gsheet/__init__.py` & `gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__init__.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/gsheet/__tests__/test_gsheet.py` & `gc_google_services_api-1.2.9/gc_google_services_api/gsheet/__tests__/test_gsheet.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/permissions/drive.py` & `gc_google_services_api-1.2.9/gc_google_services_api/permissions/drive.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/gc_google_services_api/permissions/workspace.py` & `gc_google_services_api-1.2.9/gc_google_services_api/permissions/workspace.py`

 * *Files identical despite different names*

### Comparing `gc_google_services_api-1.2.8/pyproject.toml` & `gc_google_services_api-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gc-google-services-api"
-version = "1.2.8"
+version = "1.2.9"
 description = ""
 authors = ["Jonathan Rodríguez Alejos <jrodriguez.5716@gmail.com>"]
 readme = "README.md"
 packages = [{include = "gc_google_services_api"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `gc_google_services_api-1.2.8/PKG-INFO` & `gc_google_services_api-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gc-google-services-api
-Version: 1.2.8
+Version: 1.2.9
 Summary: 
 Author: Jonathan Rodríguez Alejos
 Author-email: jrodriguez.5716@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

