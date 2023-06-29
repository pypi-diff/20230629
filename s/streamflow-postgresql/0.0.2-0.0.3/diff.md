# Comparing `tmp/streamflow-postgresql-0.0.2.tar.gz` & `tmp/streamflow-postgresql-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamflow-postgresql-0.0.2.tar", last modified: Sat May 20 18:13:26 2023, max compression
+gzip compressed data, was "streamflow-postgresql-0.0.3.tar", last modified: Thu Jun 29 08:03:39 2023, max compression
```

## Comparing `streamflow-postgresql-0.0.2.tar` & `streamflow-postgresql-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/bandit-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/lint-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.687495 streamflow-postgresql-0.0.2/postgresql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.687495 streamflow-postgresql-0.0.2/postgresql/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.json
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.sql
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/postgresql/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 18:13:26.000000 streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 18:13:26.691495 streamflow-postgresql-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-20 18:13:09.000000 streamflow-postgresql-0.0.2/tests/test_persistence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:39.334771 streamflow-postgresql-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-29 08:03:39.334771 streamflow-postgresql-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/bandit-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/lint-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:39.330771 streamflow-postgresql-0.0.3/postgresql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24413 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:39.330771 streamflow-postgresql-0.0.3/postgresql/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/schemas/postgresql.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/schemas/postgresql.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/postgresql/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 08:03:39.334771 streamflow-postgresql-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:39.334771 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-29 08:03:39.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:03:38.000000 streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:03:39.334771 streamflow-postgresql-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-29 08:03:26.000000 streamflow-postgresql-0.0.3/tests/test_persistence.py
```

### Comparing `streamflow-postgresql-0.0.2/LICENSE` & `streamflow-postgresql-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/PKG-INFO` & `streamflow-postgresql-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.2
+Version: 0.0.3
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `streamflow-postgresql-0.0.2/README.md` & `streamflow-postgresql-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/postgresql/database.py` & `streamflow-postgresql-0.0.3/postgresql/database.py`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.json` & `streamflow-postgresql-0.0.3/postgresql/schemas/postgresql.json`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/postgresql/schemas/postgresql.sql` & `streamflow-postgresql-0.0.3/postgresql/schemas/postgresql.sql`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/pyproject.toml` & `streamflow-postgresql-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/PKG-INFO` & `streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamflow-postgresql
-Version: 0.0.2
+Version: 0.0.3
 Summary: StreamFlow PostgreSQL plugin
 Author-email: Iacopo Colonnelli <iacopo.colonnelli@unito.it>
 License: LGPL-3.0-or-later
 Project-URL: Package, https://pypi.org/project/streamflow-postgresql
 Project-URL: Repository, https://github.com/alpha-unito/streamflow-postgresql
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `streamflow-postgresql-0.0.2/streamflow_postgresql.egg-info/SOURCES.txt` & `streamflow-postgresql-0.0.3/streamflow_postgresql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `streamflow-postgresql-0.0.2/tests/test_persistence.py` & `streamflow-postgresql-0.0.3/tests/test_persistence.py`

 * *Files identical despite different names*

