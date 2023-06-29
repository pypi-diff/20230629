# Comparing `tmp/django-clickhouse-backend-1.0.2.tar.gz` & `tmp/django-clickhouse-backend-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-clickhouse-backend-1.0.2.tar", last modified: Tue Feb 28 15:15:14 2023, max compression
+gzip compressed data, was "django-clickhouse-backend-1.0.3.tar", last modified: Thu Jun 29 15:05:02 2023, max compression
```

## Comparing `django-clickhouse-backend-1.0.2.tar` & `django-clickhouse-backend-1.0.3.tar`

### file list

```diff
@@ -1,58 +1,64 @@
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.609219 django-clickhouse-backend-1.0.2/
--rw-rw-r--   0 wen       (1000) wen       (1000)     1067 2022-10-18 14:44:39.000000 django-clickhouse-backend-1.0.2/LICENSE
--rw-rw-r--   0 wen       (1000) wen       (1000)       34 2022-10-28 13:33:01.000000 django-clickhouse-backend-1.0.2/MANIFEST.in
--rw-rw-r--   0 wen       (1000) wen       (1000)    13849 2023-02-28 15:15:14.609219 django-clickhouse-backend-1.0.2/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)    12722 2023-02-28 14:25:09.000000 django-clickhouse-backend-1.0.2/README.md
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.577219 django-clickhouse-backend-1.0.2/clickhouse_backend/
--rw-rw-r--   0 wen       (1000) wen       (1000)        5 2023-02-28 15:13:34.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/VERSION
--rw-rw-r--   0 wen       (1000) wen       (1000)      102 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/__init__.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.589219 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/
--rw-rw-r--   0 wen       (1000) wen       (1000)        0 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     8377 2023-02-28 13:18:27.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1365 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/client.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1980 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/creation.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4692 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/features.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4285 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/introspection.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    13799 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/operations.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    24233 2023-02-28 15:05:58.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/backend/schema.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      161 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/compat.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.593219 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/
--rw-rw-r--   0 wen       (1000) wen       (1000)      988 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1975 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/client.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     2117 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/connection.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     2495 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/escape.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      734 2022-10-15 03:05:40.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/pool.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       15 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/driver/types.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.597219 django-clickhouse-backend-1.0.2/clickhouse_backend/idworker/
--rw-rw-r--   0 wen       (1000) wen       (1000)      495 2022-10-16 09:51:45.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/idworker/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       78 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/idworker/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4120 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/idworker/snowflake.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.597219 django-clickhouse-backend-1.0.2/clickhouse_backend/models/
--rw-rw-r--   0 wen       (1000) wen       (1000)      341 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     2634 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     3618 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/engines.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.605219 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/
--rw-rw-r--   0 wen       (1000) wen       (1000)    16445 2023-02-28 13:01:36.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    11632 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/array.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     2691 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/base.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     4212 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/integer.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    12929 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/map.py
--rw-rw-r--   0 wen       (1000) wen       (1000)    13155 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/tuple.py
--rw-rw-r--   0 wen       (1000) wen       (1000)       95 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/utils.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     6459 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/indexes.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      623 2022-10-26 15:41:29.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/query.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.605219 django-clickhouse-backend-1.0.2/clickhouse_backend/models/sql/
--rw-rw-r--   0 wen       (1000) wen       (1000)       46 2022-10-15 12:11:54.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/sql/__init__.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     6929 2023-02-28 12:51:43.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/sql/compiler.py
--rw-rw-r--   0 wen       (1000) wen       (1000)     1219 2023-02-28 12:52:36.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/models/sql/query.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      712 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/utils.py
--rw-rw-r--   0 wen       (1000) wen       (1000)      625 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/clickhouse_backend/validators.py
-drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-02-28 15:15:14.609219 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/
--rw-rw-r--   0 wen       (1000) wen       (1000)    13849 2023-02-28 15:15:14.000000 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/PKG-INFO
--rw-rw-r--   0 wen       (1000) wen       (1000)     1692 2023-02-28 15:15:14.000000 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/SOURCES.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-02-28 15:15:14.000000 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/dependency_links.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       60 2023-02-28 15:15:14.000000 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/requires.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       19 2023-02-28 15:15:14.000000 django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/top_level.txt
--rw-rw-r--   0 wen       (1000) wen       (1000)       81 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.2/pyproject.toml
--rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-02-28 15:15:14.609219 django-clickhouse-backend-1.0.2/setup.cfg
--rw-rw-r--   0 wen       (1000) wen       (1000)     1593 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.2/setup.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1067 2022-10-18 14:44:39.000000 django-clickhouse-backend-1.0.3/LICENSE
+-rw-rw-r--   0 wen       (1000) wen       (1000)       34 2022-10-28 13:33:01.000000 django-clickhouse-backend-1.0.3/MANIFEST.in
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13838 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12722 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/README.md
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.668181 django-clickhouse-backend-1.0.3/clickhouse_backend/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        5 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/VERSION
+-rw-rw-r--   0 wen       (1000) wen       (1000)      102 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/__init__.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/
+-rw-rw-r--   0 wen       (1000) wen       (1000)        0 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     8557 2023-06-24 12:24:00.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1365 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/client.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1980 2023-01-04 14:13:06.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/creation.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     5449 2023-06-24 14:50:47.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/features.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4360 2023-06-24 12:21:48.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/introspection.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13424 2023-06-28 14:43:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/operations.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    24709 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/backend/schema.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      196 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/compat.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      986 2023-06-28 13:03:21.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1975 2023-06-22 07:01:32.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/client.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4934 2023-06-22 14:45:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/connection.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3367 2023-06-28 14:52:51.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/escape.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      734 2022-10-15 03:05:40.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/pool.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       87 2023-06-28 14:43:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/driver/types.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      495 2022-10-16 09:51:45.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       78 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4120 2022-10-16 09:50:31.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/snowflake.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.672181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      507 2023-06-27 13:26:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1671 2023-06-27 12:46:23.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     3618 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/engines.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.676181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/
+-rw-rw-r--   0 wen       (1000) wen       (1000)    15813 2023-06-26 14:58:38.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    11632 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/array.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     2613 2023-06-24 13:02:34.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/base.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     4212 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/integer.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1278 2023-06-29 14:56:49.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/json.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    12991 2023-06-24 12:37:01.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/map.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13318 2023-06-27 14:52:42.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/tuple.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)       95 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/utils.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      981 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/functions.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     6459 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/indexes.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      623 2022-10-26 15:41:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/query.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.676181 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/
+-rw-rw-r--   0 wen       (1000) wen       (1000)       46 2022-10-15 12:11:54.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     7803 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/compiler.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1418 2023-06-21 11:54:13.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/query.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/
+-rw-rw-r--   0 wen       (1000) wen       (1000)      138 2023-06-27 12:48:43.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/__init__.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      559 2023-06-28 14:56:30.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/fields.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      308 2023-06-27 12:46:23.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/patch/functions.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      712 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/utils.py
+-rw-rw-r--   0 wen       (1000) wen       (1000)      625 2023-02-28 12:35:52.000000 django-clickhouse-backend-1.0.3/clickhouse_backend/validators.py
+drwxrwxr-x   0 wen       (1000) wen       (1000)        0 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/
+-rw-rw-r--   0 wen       (1000) wen       (1000)    13838 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/PKG-INFO
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1882 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/SOURCES.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)        1 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/dependency_links.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       60 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/requires.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       19 2023-06-29 15:05:02.000000 django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/top_level.txt
+-rw-rw-r--   0 wen       (1000) wen       (1000)       81 2022-08-30 00:45:24.000000 django-clickhouse-backend-1.0.3/pyproject.toml
+-rw-rw-r--   0 wen       (1000) wen       (1000)       38 2023-06-29 15:05:02.680181 django-clickhouse-backend-1.0.3/setup.cfg
+-rw-rw-r--   0 wen       (1000) wen       (1000)     1582 2023-06-24 07:04:29.000000 django-clickhouse-backend-1.0.3/setup.py
```

### Comparing `django-clickhouse-backend-1.0.2/LICENSE` & `django-clickhouse-backend-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/PKG-INFO` & `django-clickhouse-backend-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-clickhouse-backend
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django clickHouse database backend.
 Home-page: https://github.com/jayvynl/django-clickhouse-backend
 Author: Lin Zhiwen
 Author-email: zhiwenlin1116@gmail.com
 License: MIT
 Keywords: Django ClickHouse database backend engine driver
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django ClickHouse Database Backend
 ===
 
 Django clickhouse backend is a [django database backend](https://docs.djangoproject.com/en/4.1/ref/databases/) for 
@@ -56,15 +56,15 @@
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
 
 **Requirements:**
 
-- [Python](https://www.python.org/) >= 3.6
+- [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
 
 
 Get started
 ---
```

### Comparing `django-clickhouse-backend-1.0.2/README.md` & `django-clickhouse-backend-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
 
 **Requirements:**
 
-- [Python](https://www.python.org/) >= 3.6
+- [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
 
 
 Get started
 ---
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/base.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     data_types = {
         # Django fields.
         "SmallAutoField": "Int16",
         "AutoField": "Int32",
         "BigAutoField": "Int64",
         "IPAddressField": "IPv4",
         "GenericIPAddressField": "IPv6",
+        "JSONField": "JSON",
         "BinaryField": "String",
         "CharField": "FixedString(%(max_length)s)",
         "DateField": "Date32",
         "DateTimeField": "DateTime64(6, 'UTC')" if settings.USE_TZ else "DateTime64(6)",
         "DecimalField": "Decimal(%(max_digits)s, %(decimal_places)s)",
         "FileField": "String",
         "FilePathField": "String",
@@ -199,14 +200,23 @@
     def init_connection_state(self):
         pass
 
     @async_unsafe
     def create_cursor(self, name=None):
         return self.connection.cursor()
 
+    def _savepoint(self, sid):
+        pass
+
+    def _savepoint_rollback(self, sid):
+        pass
+
+    def _savepoint_commit(self, sid):
+        pass
+
     def _set_autocommit(self, autocommit):
         pass
 
     def is_usable(self):
         try:
             # Use a clickhouse_driver cursor directly, bypassing Django's utilities.
             with self.connection.cursor() as cursor:
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/client.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/client.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/creation.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/creation.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/features.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/features.py`

 * *Files 8% similar despite different names*

```diff
@@ -96,15 +96,31 @@
     # https://clickhouse.com/docs/en/sql-reference/statements/insert-into/#constraints
     supports_ignore_conflicts = False
 
     # Does the backend support partial indexes (CREATE INDEX ... WHERE ...)?
     supports_partial_indexes = False
 
     # Does the backend support JSONField?
-    supports_json_field = False
+    supports_json_field = True
+    # Can the backend introspect a JSONField?
+    can_introspect_json_field = True
+    # Does the backend support primitives in JSONField?
+    supports_primitives_in_json_field = False
+    # Is there a true datatype for JSON?
+    has_native_json_field = True
+    # Does the backend use PostgreSQL-style JSON operators like '->'?
+    has_json_operators = False
+    # Does the backend support __contains and __contained_by lookups for
+    # a JSONField?
+    supports_json_field_contains = False
+    # Does value__d__contains={'f': 'g'} (without a list around the dict) match
+    # {'d': [{'f': 'g'}]}?
+    json_key_contains_list_matching_requires_list = False
+    # Does the backend support JSONObject() database function?
+    has_json_object_function = False
 
     # Does the backend support column collations?
     supports_collation_on_charfield = False
     supports_collation_on_textfield = False
     # Does the backend support non-deterministic collations?
     supports_non_deterministic_collations = False
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/introspection.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/introspection.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             return "EnumField"
         elif data_type.startswith("Array"):
             return "ArrayField"
         elif data_type.startswith("Tuple"):
             return "TupleField"
         elif data_type.startswith("Map"):
             return "MapField"
+        elif data_type == "Object('json')":
+            return "JSONField"
 
         return f"{data_type}Field"  # Int8
 
     def get_table_list(self, cursor):
         """Return a list of table and view names in the current database."""
         cursor.execute("""
             SELECT table_name,
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/operations.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from django.conf import settings
 from django.db.backends.base.operations import BaseDatabaseOperations
 
 from clickhouse_backend import compat
-from clickhouse_backend.utils import get_timezone
+from clickhouse_backend.driver import JSON
 from clickhouse_backend.driver.client import insert_pattern
+from clickhouse_backend.utils import get_timezone
 
 
 class DatabaseOperations(BaseDatabaseOperations):
     # Use this class attribute control whether using fake transaction.
     # Fake transaction is used in test, prevent other database such as postgresql
     # from flush at the end of each testcase. Only use this feature when you are
     # aware of the effect in TransactionTestCase.
@@ -290,25 +290,28 @@
 
     def adapt_datetimefield_value(self, value):
         return value
 
     def adapt_decimalfield_value(self, value, max_digits=None, decimal_places=None):
         return value
 
+    def adapt_json_value(self, value, encoder):
+        return JSON(value)
+
     def explain_query_prefix(self, format=None, **options):
         # bypass normal explain prefix insert in compiler.as_sql
         return ""
 
     def explain_query(self, format=None, type=None, **settings):
         # https://clickhouse.com/docs/en/sql-reference/statements/explain/
         prefix = self.explain_prefix
         suffix = ""
         options = {}
         unknown_settings = []
-        for setting, value in settings:
+        for setting, value in settings.items():
             if setting in self.explain_settings:
                 options[setting] = int(bool(value))
             else:
                 unknown_settings.append(setting)
 
         if format:
             supported_formats = self.supported_output_formats
@@ -340,29 +343,14 @@
 
     def last_insert_id(self, cursor, table_name, pk_name):
         query = "SELECT %s FROM %s ORDER BY %s DESC LIMIT 1"
         params = (self.quote_name(pk_name), self.quote_name(table_name), self.quote_name(pk_name))
         cursor.execute(query % params)
         return cursor.fetchone()[0]
 
-    def savepoint_create_sql(self, sid):
-        if self.fake_transaction:
-            return "SELECT 1"
-        return super().savepoint_create_sql(sid)
-
-    def savepoint_commit_sql(self, sid):
-        if self.fake_transaction:
-            return "SELECT 1"
-        return super().savepoint_commit_sql(sid)
-
-    def savepoint_rollback_sql(self, sid):
-        if self.fake_transaction:
-            return "SELECT 1"
-        return super().savepoint_rollback_sql(sid)
-
     def last_executed_query(self, cursor, sql, params):
         if params:
             if insert_pattern.match(sql):
                 return "%s %s" % (sql, ", ".join(map(str, params)))
             else:
                 return sql % tuple(params)
         return sql
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/backend/schema.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/backend/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 )
 from django.db.backends.ddl_references import (
     Expressions, IndexName, Statement, Table, Columns
 )
 from django.db.models.expressions import ExpressionList
 from django.db.models.indexes import IndexExpression
 
+from clickhouse_backend import compat
 from clickhouse_backend.driver.escape import escape_param
 
 
 class ChColumns(Columns):
     def __str__(self):
         def col_str(column, idx):
             col = self.quote_name(column)
@@ -360,14 +361,23 @@
             old_kwargs.pop(attr, None)
             new_kwargs.pop(attr, None)
         return (
             self.quote_name(old_field.column) != self.quote_name(new_field.column) or
             (old_path, old_args, old_kwargs) != (new_path, new_args, new_kwargs)
         )
 
+    def _alter_column_type_sql(
+        self, model, old_field, new_field, new_type, old_collation=None, new_collation=None
+    ):
+        """Django4.2 add old_collation, new_collation"""
+        if compat.dj_ge42:
+            return super()._alter_column_type_sql(model, old_field, new_field, new_type, old_collation, new_collation)
+        else:
+            return super()._alter_column_type_sql(model, old_field, new_field, new_type)
+
     def _alter_field(self, model, old_field, new_field, old_type, new_type,
                      old_db_params, new_db_params, strict=False):
         # Change check constraints?
         if (old_db_params["check"] and (old_db_params["check"] != new_db_params["check"]
                                         or old_field.column != new_field.column)):
             constraint_name = self._column_check_name(old_field)
             self.execute(self._delete_check_sql(model, constraint_name))
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/driver/__init__.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,15 @@
 from clickhouse_driver.dbapi.errors import (  # NOQA
     Warning, Error, DataError, DatabaseError, ProgrammingError, IntegrityError,
     InterfaceError, InternalError, NotSupportedError, OperationalError
 )
 
 from .connection import Connection
 # Binary is compatible for django's BinaryField.
-from .types import (  # NOQA
-    Binary
-)
+from .types import Binary, JSON  # NOQA
 
 
 def connect(dsn=None, host=None,
             user=defines.DEFAULT_USER, password=defines.DEFAULT_PASSWORD,
             port=defines.DEFAULT_PORT, database=defines.DEFAULT_DATABASE,
             **kwargs):
     """
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/driver/client.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import time
 
 from clickhouse_driver import client
 
 from .escape import escape_params
 
-insert_pattern = re.compile(r'\s*insert\s*into', flags=re.IGNORECASE)
+insert_pattern = re.compile(r'\s*insert\s+into', flags=re.IGNORECASE)
 
 
 class Client(client.Client):
     def __init__(self, *args, **kwargs):
         # https://clickhouse.com/docs/en/sql-reference/data-types/datetime/#usage-remarks
         # The clickhouse-client applies the server time zone by default
         # if a time zone isn’t explicitly set when initializing the data type.
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/driver/escape.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/escape.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, datetime, timezone
+from datetime import date, datetime, time, timezone
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from typing import Sequence, Dict, Union
 from uuid import UUID
 
 from clickhouse_driver.util import escape
 
@@ -33,56 +33,72 @@
     # b"\x00F '\xfe" ->   '\x00F \'\xfe'
     b2s = str(item)
     if b2s[1] == '"':
         return "'%s'" % b2s[2:-1].replace("'", "\\'")
     return b2s[1:]
 
 
-def escape_param(item, context):
+@escape.maybe_enquote_for_server
+def escape_param(item, context, for_server=False):
     if item is None:
         return 'NULL'
 
     elif isinstance(item, datetime):
         return escape_datetime(item, context)
 
     elif isinstance(item, date):
         return "'%s'" % item.strftime('%Y-%m-%d')
 
+    elif isinstance(item, time):
+        return "'%s'" % item.strftime('%H:%M:%S')
+
     elif isinstance(item, str):
+        # We need double escaping for server-side parameters.
+        if for_server:
+            item = ''.join(escape.escape_chars_map.get(c, c) for c in item)
         return "'%s'" % ''.join(escape.escape_chars_map.get(c, c) for c in item)
 
     elif isinstance(item, list):
-        return "[%s]" % ', '.join(str(escape_param(x, context)) for x in item)
+        return "[%s]" % ', '.join(str(escape_param(x, context, for_server=for_server)) for x in item)
 
     elif isinstance(item, tuple):
-        return "(%s)" % ', '.join(str(escape_param(x, context)) for x in item)
+        return "tuple(%s)" % ', '.join(str(escape_param(x, context, for_server=for_server)) for x in item)
 
     elif isinstance(item, Enum):
-        return escape_param(item.value, context)
+        return escape_param(item.value, context, for_server=for_server)
 
     elif isinstance(item, (UUID, IPv4Address, IPv6Address)):
         return "'%s'" % str(item)
 
     elif isinstance(item, types.Binary):
         return escape_binary(item, context)
 
+    elif isinstance(item, types.JSON):
+        value = item.value
+        if isinstance(value, list):
+            return escape_param([types.JSON(v) for v in value], context, for_server=for_server)
+        elif isinstance(value, dict):
+            return escape_param(tuple(types.JSON(v) for v in value.values()), context, for_server=for_server)
+        else:
+            return escape_param(value, context, for_server=for_server)
+
     else:
         return item
 
 
-def escape_params(params: Params, context: Dict) -> Params:
+def escape_params(params: Params, context: Dict, for_server=False) -> Params:
     """Escape param to qualified string representation.
 
     This function is not used in INSERT INTO queries.
     """
     if isinstance(params, Dict):
         escaped = {
-            key: escape_param(value, context)
+            key: escape_param(value, context, for_server=for_server)
             for key, value in params.items()
         }
     else:
         escaped = tuple(
-            escape_param(value, context)
+            escape_param(value, context, for_server=for_server)
             for value in params
         )
 
     return escaped
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/driver/pool.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/driver/pool.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/idworker/snowflake.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/idworker/snowflake.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/base.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 from django.db import models
 from django.db.migrations import state
-from django.db.models import functions
 from django.db.models import options
-from django.db.models.manager import BaseManager
 
 from .query import QuerySet
 from .sql import Query
 
 options.DEFAULT_NAMES = (
     *options.DEFAULT_NAMES,
     # Clickhouse features
     'engine',
 )
 # Also monkey patch state.DEFAULT_NAMES, this makes new option names contained in migrations.
 state.DEFAULT_NAMES = options.DEFAULT_NAMES
 
 
-def as_clickhouse(self, compiler, connection, **extra_context):
-    return functions.Random.as_sql(
-        self, compiler, connection, function="rand64", **extra_context
-    )
+class ClickhouseManager(models.Manager):
+    _queryset_class = QuerySet
 
-
-functions.Random.as_clickhouse = as_clickhouse
-
-
-class ClickhouseManager(BaseManager.from_queryset(QuerySet)):
     def get_queryset(self):
         """
         User defined Query and QuerySet class that support clickhouse particular query.
         """
         return self._queryset_class(
             model=self.model,
             query=Query(self.model),
@@ -42,30 +33,19 @@
     objects = ClickhouseManager()
 
     class Meta:
         abstract = True
 
     def _do_update(self, base_qs, using, pk_val, values, update_fields, forced_update):
         """
-         Try to update the model. Return True if the model was updated (if an
-         update query was done and a matching row was found in the DB).
-         """
+        Try to update the model. Return True if the model was updated (if an
+        update query was done and a matching row was found in the DB).
+        """
         filtered = base_qs.filter(pk=pk_val)
         if not values:
             # We can end up here when saving a model in inheritance chain where
             # update_fields doesn't target any field in current model. In that
             # case we just say the update succeeded. Another case ending up here
             # is a model with just PK - in that case check that the PK still
             # exists.
             return update_fields is not None or filtered.exists()
-        return (
-                filtered.exists()
-                and
-                # It may happen that the object is deleted from the DB right after
-                # this check, causing the subsequent UPDATE to return zero matching
-                # rows. The same result can occur in some rare cases when the
-                # database returns zero despite the UPDATE being executed
-                # successfully (a row is matched and updated). In order to
-                # distinguish these two cases, the object's existence in the
-                # database is again checked for if the UPDATE query returns 0.
-                (filtered._update(values) > 0 or filtered.exists())
-        )
+        return filtered._update(values) > 0
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/engines.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/engines.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/__init__.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from django.utils.itercompat import is_iterable
 from django.utils.translation import gettext_lazy as _
 
 from clickhouse_backend.validators import MaxBytesValidator
 from .array import *
 from .base import FieldMixin
 from .integer import *
+from .json import *
 from .map import *
 from .tuple import *
 
 __all__ = [
     "Int8Field", "UInt8Field",
     "Int16Field", "UInt16Field",
     "Int32Field", "UInt32Field",
@@ -26,15 +27,15 @@
     "Float32Field", "Float64Field",
     "DecimalField", "BoolField",
     "StringField", "FixedStringField",
     "UUIDField",
     "DateField", "Date32Field", "DateTimeField", "DateTime64Field",
     "Enum8Field", "Enum16Field", "EnumField",
     "IPv4Field", "IPv6Field", "GenericIPAddressField",
-    "ArrayField", "TupleField", "MapField",
+    "ArrayField", "TupleField", "MapField", "JSONField",
 ]
 
 
 class Float32Field(FieldMixin, fields.FloatField):
     description = _("Single precision floating point number")
 
     def __init__(self, *args, low_cardinality=False, **kwargs):
@@ -145,30 +146,14 @@
 #         return super().get_db_prep_save(value, connection)
 
 
 class DateField(FieldMixin, fields.DateField):
     """Support integer or float may cause strange behavior,
     as integer and float are always treated as UTC timestamps,
     clickhouse store them as date in utc, which may not be what you want.
-
-    Due to a bug of clickhouse-driver 0.2.5,
-    when set null and low_cardinality the same time to DateField or Date32Field,
-    an exception will be raised when create a row.
-    The same bug is also in UUIDField.
-    Below is the minimum reproducing code:
-
-    from clickhouse_driver import Client
-    from datetime import date
-
-    client = Client('localhost', settings={'allow_suspicious_low_cardinality_types': 1})
-    client.execute('create table test (lnd LowCardinality(Nullable(Date))) engine MergeTree order by ()')
-    client.execute('insert into test values', [{'lnd': date.today()}])
-
-    ...
-    AttributeError: 'int' object has no attribute 'year'
     """
     def __init__(self, *args, low_cardinality=False, **kwargs):
         self.low_cardinality = low_cardinality
         super().__init__(*args, **kwargs)
 
     def get_internal_type(self):
         return "ClickhouseDateField"
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/array.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/array.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/base.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 from django.core.exceptions import ImproperlyConfigured
 
 
 class FieldMixin:
     """All clickhouse field should inherit this mixin.
 
     1. Remove unsupported arguments: unique, db_index, unique_for_date,
-       unique_for_month, unique_for_year, db_tablespace.
+       unique_for_month, unique_for_year, db_tablespace, db_collation.
     2. Return shortened name in deconstruct method.
-    3. Add low_cardinality attribute, corresponding to clickhouse LowCardinality Data Type.
 
     low_cardinality argument is added separately in every specific field that support LowCardinality.
     If added in this mixin, then PyCharm will not supply argument hints.
     """
     nullable_allowed = True
 
     def check(self, **kwargs):
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/integer.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/integer.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/map.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/map.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,16 @@
                 self.key_field.get_db_prep_value(k, connection, prepared=prepared):
                 self.value_field.get_db_prep_value(v, connection, prepared=prepared)
                 for k, v in value.items()
             }
         return value
 
     def get_db_prep_save(self, value, connection):
+        if hasattr(value, "as_sql"):
+            return value
         if isinstance(value, collections.abc.Mapping):
             return {
                 self.key_field.get_db_prep_save(k, connection):
                 self.value_field.get_db_prep_save(v, connection)
                 for k, v in value.items()
             }
         return value
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/fields/tuple.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/fields/tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,17 @@
         return self._convert_type(value)
 
     def _from_db_value(self, value, expression, connection):
         if value is None:
             return value
         self._validate_length(value)
         values = []
+        # when set allow_experimental_object_type=1 at session level, value will be a dict.
+        if isinstance(value, dict):
+            value = value.values()
         for i, field in zip(value, self._base_fields):
             if hasattr(field, "from_db_value"):
                 values.append(field.from_db_value(i, expression, connection))
             else:
                 values.append(i)
         return self._convert_type(values)
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/indexes.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/indexes.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/query.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/query.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/models/sql/query.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/models/sql/query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import namedtuple
 
+from django.db import router
 from django.db.models.sql import query
 from django.db.models.sql import subqueries
 
 from clickhouse_backend import compat
 
 ExplainInfo = namedtuple("ExplainInfo", ("format", "type", "options"))
 
@@ -12,14 +13,18 @@
     def __init__(self, model, where=query.WhereNode, alias_cols=True):
         if compat.dj_ge4:
             super().__init__(model, alias_cols)
         else:
             super().__init__(model, where, alias_cols)
         self.setting_info = {}
 
+    def sql_with_params(self):
+        """Choose the right db when database router is used."""
+        return self.get_compiler(router.db_for_read(self.model)).as_sql()
+
     def clone(self):
         obj = super().clone()
         obj.setting_info = self.setting_info.copy()
         return obj
 
     def explain(self, using, format=None, type=None, **settings):
         q = self.clone()
```

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/utils.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/utils.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/clickhouse_backend/validators.py` & `django-clickhouse-backend-1.0.3/clickhouse_backend/validators.py`

 * *Files identical despite different names*

### Comparing `django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/PKG-INFO` & `django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: django-clickhouse-backend
-Version: 1.0.2
+Version: 1.0.3
 Summary: Django clickHouse database backend.
 Home-page: https://github.com/jayvynl/django-clickhouse-backend
 Author: Lin Zhiwen
 Author-email: zhiwenlin1116@gmail.com
 License: MIT
 Keywords: Django ClickHouse database backend engine driver
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Django ClickHouse Database Backend
 ===
 
 Django clickhouse backend is a [django database backend](https://docs.djangoproject.com/en/4.1/ref/databases/) for 
@@ -56,15 +56,15 @@
 - Aggregation functions result in 0 or nan (Not NULL) when data set is empty. max/min/sum/count is 0, avg/STDDEV_POP/VAR_POP is nan.
 - In outer join, clickhouse will set missing columns to empty values (0 for number, empty string for text, unix epoch for date/datatime) instead of NULL. 
   So Count("book") resolve to 1 in a missing LEFT OUTER JOIN match, not 0.
   In aggregation expression Avg("book__rating", default=2.5), default=2.5 have no effect in a missing match.
 
 **Requirements:**
 
-- [Python](https://www.python.org/) >= 3.6
+- [Python](https://www.python.org/) >= 3.7
 - [Django](https://docs.djangoproject.com/) >= 3.2
 - [clickhouse driver](https://github.com/mymarilyn/clickhouse-driver)
 - [clickhouse pool](https://github.com/ericmccarthy7/clickhouse-pool)
 
 
 Get started
 ---
```

### Comparing `django-clickhouse-backend-1.0.2/django_clickhouse_backend.egg-info/SOURCES.txt` & `django-clickhouse-backend-1.0.3/django_clickhouse_backend.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,29 @@
 clickhouse_backend/driver/types.py
 clickhouse_backend/idworker/__init__.py
 clickhouse_backend/idworker/base.py
 clickhouse_backend/idworker/snowflake.py
 clickhouse_backend/models/__init__.py
 clickhouse_backend/models/base.py
 clickhouse_backend/models/engines.py
+clickhouse_backend/models/functions.py
 clickhouse_backend/models/indexes.py
 clickhouse_backend/models/query.py
 clickhouse_backend/models/fields/__init__.py
 clickhouse_backend/models/fields/array.py
 clickhouse_backend/models/fields/base.py
 clickhouse_backend/models/fields/integer.py
+clickhouse_backend/models/fields/json.py
 clickhouse_backend/models/fields/map.py
 clickhouse_backend/models/fields/tuple.py
 clickhouse_backend/models/fields/utils.py
 clickhouse_backend/models/sql/__init__.py
 clickhouse_backend/models/sql/compiler.py
 clickhouse_backend/models/sql/query.py
+clickhouse_backend/patch/__init__.py
+clickhouse_backend/patch/fields.py
+clickhouse_backend/patch/functions.py
 django_clickhouse_backend.egg-info/PKG-INFO
 django_clickhouse_backend.egg-info/SOURCES.txt
 django_clickhouse_backend.egg-info/dependency_links.txt
 django_clickhouse_backend.egg-info/requires.txt
 django_clickhouse_backend.egg-info/top_level.txt
```

### Comparing `django-clickhouse-backend-1.0.2/setup.py` & `django-clickhouse-backend-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,32 +17,32 @@
     url="https://github.com/jayvynl/django-clickhouse-backend",
     author="Lin Zhiwen",
     author_email="zhiwenlin1116@gmail.com",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     license="MIT",
     keywords='Django ClickHouse database backend engine driver',
-    python_requires='>=3.6, <4',
+    python_requires='>=3.7, <4',
     install_requires=[
         "django>=3.2",
-        "clickhouse-driver==0.2.5",
+        "clickhouse-driver==0.2.6",
         "clickhouse-pool==0.5.3",
     ],
     classifiers=[
         "Framework :: Django",
         "Framework :: Django :: 3.2",
         "Framework :: Django :: 4",
         "Framework :: Django :: 4.0",
         "Framework :: Django :: 4.1",
+        "Framework :: Django :: 4.2",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ]
 )
```

