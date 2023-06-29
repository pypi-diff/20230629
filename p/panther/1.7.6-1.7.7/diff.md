# Comparing `tmp/panther-1.7.6.tar.gz` & `tmp/panther-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.6.tar", last modified: Fri May 26 10:27:58 2023, max compression
+gzip compressed data, was "panther-1.7.7.tar", last modified: Thu Jun 29 14:20:19 2023, max compression
```

## Comparing `panther-1.7.6.tar` & `panther-1.7.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 10:27:43.000000 panther-1.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 10:27:58.124644 panther-1.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 10:27:43.000000 panther-1.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 10:27:43.000000 panther-1.7.6/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 10:27:43.000000 panther-1.7.6/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-26 10:27:43.000000 panther-1.7.6/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 10:27:43.000000 panther-1.7.6/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 10:27:43.000000 panther-1.7.6/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-26 10:27:43.000000 panther-1.7.6/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-26 10:27:43.000000 panther-1.7.6/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-26 10:27:43.000000 panther-1.7.6/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-26 10:27:43.000000 panther-1.7.6/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 10:27:43.000000 panther-1.7.6/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:27:43.000000 panther-1.7.6/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-26 10:27:43.000000 panther-1.7.6/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-26 10:27:43.000000 panther-1.7.6/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 10:27:43.000000 panther-1.7.6/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-26 10:27:43.000000 panther-1.7.6/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 10:27:43.000000 panther-1.7.6/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 10:27:43.000000 panther-1.7.6/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 10:27:43.000000 panther-1.7.6/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 10:27:43.000000 panther-1.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:27:58.124644 panther-1.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 10:27:43.000000 panther-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-29 14:19:56.000000 panther-1.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-29 14:20:19.780356 panther-1.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-29 14:19:56.000000 panther-1.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.772356 panther-1.7.7/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-29 14:19:56.000000 panther-1.7.7/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-29 14:19:56.000000 panther-1.7.7/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-06-29 14:19:56.000000 panther-1.7.7/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-29 14:19:56.000000 panther-1.7.7/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-29 14:19:56.000000 panther-1.7.7/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-29 14:19:56.000000 panther-1.7.7/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-29 14:19:56.000000 panther-1.7.7/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 14:19:56.000000 panther-1.7.7/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-29 14:19:56.000000 panther-1.7.7/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-29 14:19:56.000000 panther-1.7.7/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-06-29 14:19:56.000000 panther-1.7.7/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-29 14:19:56.000000 panther-1.7.7/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.780356 panther-1.7.7/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-29 14:19:56.000000 panther-1.7.7/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-29 14:19:56.000000 panther-1.7.7/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-29 14:19:56.000000 panther-1.7.7/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-06-29 14:19:56.000000 panther-1.7.7/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-29 14:19:56.000000 panther-1.7.7/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-29 14:19:56.000000 panther-1.7.7/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-29 14:19:56.000000 panther-1.7.7/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-29 14:19:56.000000 panther-1.7.7/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-29 14:19:56.000000 panther-1.7.7/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 14:20:19.776356 panther-1.7.7/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-29 14:20:19.000000 panther-1.7.7/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-29 14:19:56.000000 panther-1.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 14:20:19.780356 panther-1.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-29 14:19:56.000000 panther-1.7.7/setup.py
```

### Comparing `panther-1.7.6/LICENSE` & `panther-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/PKG-INFO` & `panther-1.7.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.6
+Version: 1.7.7
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.6/README.md` & `panther-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/_utils.py` & `panther-1.7.7/panther/_utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/app.py` & `panther-1.7.7/panther/app.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/authentications.py` & `panther-1.7.7/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/caching.py` & `panther-1.7.7/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/create_command.py` & `panther-1.7.7/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/main.py` & `panther-1.7.7/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/monitor_command.py` & `panther-1.7.7/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/run_command.py` & `panther-1.7.7/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/template.py` & `panther-1.7.7/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/cli/utils.py` & `panther-1.7.7/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/configs.py` & `panther-1.7.7/panther/configs.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/connection.py` & `panther-1.7.7/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/models.py` & `panther-1.7.7/panther/db/models.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/queries/mongodb_queries.py` & `panther-1.7.7/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/queries/pantherdb_queries.py` & `panther-1.7.7/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/queries/queries.py` & `panther-1.7.7/panther/db/queries/queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/db/utils.py` & `panther-1.7.7/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/exceptions.py` & `panther-1.7.7/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/logger.py` & `panther-1.7.7/panther/logger.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/main.py` & `panther-1.7.7/panther/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             middlewares.append(Middleware(**data))  # NOQA: Py Argument List
         return middlewares
 
     def _get_authentication_class(self) -> ModelMetaclass | None:
         return self.settings.get('AUTHENTICATION') and import_class(self.settings['AUTHENTICATION'])
 
     def _get_user_model(self) -> ModelMetaclass:
-        return import_class(self.settings.get('USER_MODEL', 'panther.db.models.User'))
+        return import_class(self.settings.get('USER_MODEL', 'panther.db.models.BaseUser'))
 
     def _get_jwt_config(self) -> JWTConfig:
         """Only Collect JWT Config If Authentication Is JWTAuthentication"""
         if getattr(config['authentication'], '__name__', None) == 'JWTAuthentication':
             user_config = self.settings.get('JWTConfig')
             return JWTConfig(**user_config) if user_config else JWTConfig(key=config['secret_key'].decode())
```

### Comparing `panther-1.7.6/panther/middlewares/monitoring.py` & `panther-1.7.7/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/middlewares/redis.py` & `panther-1.7.7/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/panel/apis.py` & `panther-1.7.7/panther/panel/apis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/request.py` & `panther-1.7.7/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/response.py` & `panther-1.7.7/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/routings.py` & `panther-1.7.7/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/status.py` & `panther-1.7.7/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther/utils.py` & `panther-1.7.7/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/panther.egg-info/PKG-INFO` & `panther-1.7.7/panther.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.6
+Version: 1.7.7
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.6/panther.egg-info/SOURCES.txt` & `panther-1.7.7/panther.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panther-1.7.6/setup.py` & `panther-1.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 VERSION = panther_version()
 DESCRIPTION = open('README.md').read()
 
 EXTRAS_REQUIRE = {
     'full': [
-        'python-jose>=3.3.0',
         'pymongo>=4.3.3',
     ]
 }
 
 setup(
     name='panther',
     version=VERSION,
@@ -49,10 +48,11 @@
         'pantherdb>=1.2.2',
         'pydantic>=1.10.7',
         'redis>=4.5.3',
         'rich>=13.3.2',
         'uvicorn>=0.21.1',
         'uvloop>=0.17.0',
         'watchfiles>=0.18.1',
+        'python-jose==3.3.0',
     ],
     extras_require=EXTRAS_REQUIRE,
 )
```

