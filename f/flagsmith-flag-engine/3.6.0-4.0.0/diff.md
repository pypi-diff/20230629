# Comparing `tmp/flagsmith-flag-engine-3.6.0.tar.gz` & `tmp/flagsmith-flag-engine-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-flag-engine-3.6.0.tar", last modified: Thu Jun 29 10:19:22 2023, max compression
+gzip compressed data, was "flagsmith-flag-engine-4.0.0.tar", last modified: Thu Jun 29 11:08:19 2023, max compression
```

## Comparing `flagsmith-flag-engine-3.6.0.tar` & `flagsmith-flag-engine-4.0.0.tar`

### file list

```diff
@@ -1,74 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.613602 flagsmith-flag-engine-3.6.0/flag_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/document_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/organisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.625603 flagsmith-flag-engine-3.6.0/flag_engine/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.625603 flagsmith-flag-engine-3.6.0/flag_engine/segments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/semver.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.735524 flagsmith-flag-engine-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-29 11:08:19.735524 flagsmith-flag-engine-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/environments/builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/environments/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/environments/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/environments/integrations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/environments/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/features/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/features/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/identities/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/traits/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/traits/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/identities/traits/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/organisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/organisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/organisations/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/projects/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/segments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/segments/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/segments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/segments/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.731524 flagsmith-flag-engine-4.0.0/flag_engine/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/json/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/flag_engine/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 11:08:19.735524 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-29 11:08:19.000000 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-29 11:08:19.000000 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 11:08:19.000000 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-29 11:08:19.000000 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 11:08:19.000000 flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 11:08:19.735524 flagsmith-flag-engine-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-29 11:08:18.000000 flagsmith-flag-engine-4.0.0/setup.py
```

### Comparing `flagsmith-flag-engine-3.6.0/LICENSE.txt` & `flagsmith-flag-engine-4.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/README.md` & `flagsmith-flag-engine-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/engine.py` & `flagsmith-flag-engine-4.0.0/flag_engine/engine.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/environments/models.py` & `flagsmith-flag-engine-4.0.0/flag_engine/environments/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 import typing
-from dataclasses import dataclass, field
 from datetime import datetime
 
+from pydantic import BaseModel, Field
+
 from flag_engine.environments.integrations.models import IntegrationModel
 from flag_engine.features.models import FeatureStateModel
 from flag_engine.projects.models import ProjectModel
 from flag_engine.utils.datetime import utcnow_with_tz
 
 
-@dataclass
-class EnvironmentAPIKeyModel:
+class EnvironmentAPIKeyModel(BaseModel):
     id: int
     key: str
     created_at: datetime
     name: str
     client_api_key: str
-    expires_at: datetime = None
+    expires_at: typing.Optional[datetime] = None
     active: bool = True
 
     @property
     def is_valid(self):
         return self.active and (
             not self.expires_at or self.expires_at > utcnow_with_tz()
         )
 
 
-@dataclass
-class WebhookModel:
+class WebhookModel(BaseModel):
     url: str
     secret: str
 
 
-@dataclass
-class EnvironmentModel:
+class EnvironmentModel(BaseModel):
     id: int
     api_key: str
     project: ProjectModel
-    feature_states: typing.List[FeatureStateModel] = field(default_factory=list)
+    feature_states: typing.List[FeatureStateModel] = Field(default_factory=list)
 
-    name: str = None
+    name: typing.Optional[str] = None
     allow_client_traits: bool = True
-    updated_at: datetime = field(default_factory=utcnow_with_tz)
+    updated_at: datetime = Field(default_factory=utcnow_with_tz)
     hide_sensitive_data: bool = False
+    hide_disabled_flags: typing.Optional[bool] = None
     use_identity_composite_key_for_hashing: bool = False
 
     amplitude_config: typing.Optional[IntegrationModel] = None
     dynatrace_config: typing.Optional[IntegrationModel] = None
     heap_config: typing.Optional[IntegrationModel] = None
     mixpanel_config: typing.Optional[IntegrationModel] = None
     rudderstack_config: typing.Optional[IntegrationModel] = None
     segment_config: typing.Optional[IntegrationModel] = None
 
-    hide_disabled_flags: typing.Optional[bool] = None
-
     webhook_config: typing.Optional[WebhookModel] = None
 
     _INTEGRATION_ATTS = [
         "amplitude_config",
         "dynatrace_config",
         "heap_config",
         "mixpanel_config",
         "rudderstack_config",
         "segment_config",
     ]
 
     @property
-    def integrations_data(self) -> dict:
+    def integrations_data(self) -> typing.Dict[str, typing.Dict[str, str]]:
         """
         Return a dictionary representation of all integration config objects.
 
             e.g.
             {
                 "mixpanel_config": {"base_url": None, "api_key": "some-key"},
                 "segment_config": {
```

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/features/models.py` & `flagsmith-flag-engine-4.0.0/flag_engine/features/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,105 @@
 import math
 import typing
 import uuid
-from dataclasses import dataclass, field
 
+from pydantic import UUID4, BaseModel, Field, confloat
+from pydantic_collections import BaseCollectionModel
+
+from flag_engine.utils.exceptions import InvalidPercentageAllocation
 from flag_engine.utils.hashing import get_hashed_percentage_for_object_ids
 
 
-@dataclass
-class FeatureModel:
+class FeatureModel(BaseModel):
     id: int
     name: str
     type: str
 
     def __eq__(self, other):
         return self.id == other.id
 
     def __hash__(self):
         return hash(self.id)
 
 
-@dataclass
-class MultivariateFeatureOptionModel:
+class MultivariateFeatureOptionModel(BaseModel):
     value: typing.Any
     id: int = None
 
 
-@dataclass
-class MultivariateFeatureStateValueModel:
+class MultivariateFeatureStateValueModel(BaseModel):
     multivariate_feature_option: MultivariateFeatureOptionModel
-    percentage_allocation: float
+    percentage_allocation: confloat(ge=0, le=100)
     id: int = None
-    mv_fs_value_uuid: str = field(default_factory=uuid.uuid4)
+    mv_fs_value_uuid: UUID4 = Field(default_factory=uuid.uuid4)
 
 
-@dataclass
-class FeatureSegmentModel:
+class FeatureSegmentModel(BaseModel):
     priority: int = None
 
 
-@dataclass
-class FeatureStateModel:
+class MultivariateFeatureStateValueList(
+    BaseCollectionModel[MultivariateFeatureStateValueModel]
+):
+    # TODO @khvn26 Consider dropping pydantic_collections in favour of a `list`/`set`
+    #      subclass after upgrading to Pydantic V2
+    #      or not use custom collections at all and move their validation/interfaces
+    #      to the parent model
+    #      https://github.com/Flagsmith/flagsmith-engine/issues/172
+    @classmethod
+    def __get_validators__(
+        cls,
+    ) -> typing.Generator[typing.Callable[..., typing.Any], None, None]:
+        yield cls.validate
+        yield cls._ensure_correct_percentage_allocations
+
+    @staticmethod
+    def _ensure_correct_percentage_allocations(
+        value: typing.List[MultivariateFeatureStateValueModel],
+    ) -> typing.List[MultivariateFeatureStateValueModel]:
+        if (
+            sum(
+                multivariate_feature_state.percentage_allocation
+                for multivariate_feature_state in value
+            )
+            > 100
+        ):
+            raise InvalidPercentageAllocation(
+                "Total percentage allocation for feature must be less or equal to 100 percent"
+            )
+        return value
+
+    def append(
+        self,
+        multivariate_feature_state_value: MultivariateFeatureStateValueModel,
+    ) -> None:
+        self._ensure_correct_percentage_allocations(
+            [*self, multivariate_feature_state_value],
+        )
+        super().append(multivariate_feature_state_value)
+
+
+class FeatureStateModel(BaseModel):
+    class Config:
+        validate_assignment: bool = True
+
     feature: FeatureModel
     enabled: bool
     django_id: int = None
     feature_segment: FeatureSegmentModel = None
-    featurestate_uuid: str = field(default_factory=uuid.uuid4)
-    feature_state_value: typing.Any = field(default=None, init=False)
-    multivariate_feature_state_values: typing.List[
-        MultivariateFeatureStateValueModel
-    ] = field(default_factory=list)
+    featurestate_uuid: UUID4 = Field(default_factory=uuid.uuid4)
+    feature_state_value: typing.Any = None
+    multivariate_feature_state_values: MultivariateFeatureStateValueList = Field(
+        default_factory=MultivariateFeatureStateValueList
+    )
 
     def set_value(self, value: typing.Any):
         self.feature_state_value = value
 
-    def get_value(self, identity_id: typing.Union[int, str] = None) -> typing.Any:
+    def get_value(self, identity_id: typing.Union[None, int, str] = None) -> typing.Any:
         """
         Get the value of the feature state.
 
         :param identity_id: a unique identifier for the identity, can be either a
             numeric id or a string but must be unique for the identity.
         :return: the value of the feature state.
         """
```

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/segments/constants.py` & `flagsmith-flag-engine-4.0.0/flag_engine/segments/constants.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/segments/evaluator.py` & `flagsmith-flag-engine-4.0.0/flag_engine/segments/evaluator.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/segments/models.py` & `flagsmith-flag-engine-4.0.0/flag_engine/segments/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import re
 import typing
 from contextlib import suppress
-from dataclasses import dataclass, field
 
 import semver
+from pydantic import BaseModel, Field
 
 from flag_engine.features.models import FeatureStateModel
 from flag_engine.segments import constants
+from flag_engine.segments.types import ConditionOperator, RuleType
 from flag_engine.utils.semver import is_semver
 from flag_engine.utils.types import get_casting_function
 
 
-@dataclass
-class SegmentConditionModel:
-    EXCEPTION_OPERATOR_METHODS = {
+class SegmentConditionModel(BaseModel):
+    _EXCEPTION_OPERATOR_METHODS = {
         constants.NOT_CONTAINS: "evaluate_not_contains",
         constants.REGEX: "evaluate_regex",
         constants.MODULO: "evaluate_modulo",
         constants.IN: "evaluate_in",
     }
 
-    operator: str
-    value: str = None
-    property_: str = None
+    operator: ConditionOperator
+    value: typing.Optional[str] = None
+    property_: typing.Optional[str] = None
 
     def matches_trait_value(self, trait_value: typing.Any) -> bool:
         # TODO: move this logic to the evaluator module
         with suppress(ValueError):
             if type(self.value) is str and is_semver(self.value):
                 trait_value = semver.VersionInfo.parse(trait_value)
-            if self.operator in self.EXCEPTION_OPERATOR_METHODS:
+            if self.operator in self._EXCEPTION_OPERATOR_METHODS:
                 evaluator_function = getattr(
-                    self, self.EXCEPTION_OPERATOR_METHODS.get(self.operator)
+                    self, self._EXCEPTION_OPERATOR_METHODS.get(self.operator)
                 )
                 return evaluator_function(trait_value)
 
             matching_function_name = {
                 constants.EQUAL: "__eq__",
                 constants.GREATER_THAN: "__gt__",
                 constants.GREATER_THAN_INCLUSIVE: "__ge__",
@@ -75,32 +75,30 @@
     def evaluate_in(self, trait_value) -> bool:
         try:
             return str(trait_value) in self.value.split(",")
         except AttributeError:
             return False
 
 
-@dataclass
-class SegmentRuleModel:
-    type: str
-    rules: typing.List["SegmentRuleModel"] = field(default_factory=list)
-    conditions: typing.List[SegmentConditionModel] = field(default_factory=list)
+class SegmentRuleModel(BaseModel):
+    type: RuleType
+    rules: typing.List["SegmentRuleModel"] = Field(default_factory=list)
+    conditions: typing.List[SegmentConditionModel] = Field(default_factory=list)
 
     @staticmethod
     def none(iterable: typing.Iterable) -> bool:
         return not any(iterable)
 
     @property
     def matching_function(self) -> callable:
         return {
             constants.ANY_RULE: any,
             constants.ALL_RULE: all,
             constants.NONE_RULE: SegmentRuleModel.none,
         }.get(self.type)
 
 
-@dataclass
-class SegmentModel:
+class SegmentModel(BaseModel):
     id: int
     name: str
-    rules: typing.List[SegmentRuleModel] = field(default_factory=list)
-    feature_states: typing.List[FeatureStateModel] = field(default_factory=list)
+    rules: typing.List[SegmentRuleModel] = Field(default_factory=list)
+    feature_states: typing.List[FeatureStateModel] = Field(default_factory=list)
```

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/utils/hashing.py` & `flagsmith-flag-engine-4.0.0/flag_engine/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/utils/semver.py` & `flagsmith-flag-engine-4.0.0/flag_engine/utils/semver.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flag_engine/utils/types.py` & `flagsmith-flag-engine-4.0.0/flag_engine/utils/types.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/SOURCES.txt` & `flagsmith-flag-engine-4.0.0/flagsmith_flag_engine.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,58 +1,43 @@
 LICENSE.txt
 README.md
 setup.cfg
 setup.py
 flag_engine/__init__.py
 flag_engine/engine.py
-flag_engine/api/__init__.py
-flag_engine/api/constants.py
-flag_engine/api/document_builders.py
-flag_engine/api/fields.py
-flag_engine/api/filters.py
-flag_engine/api/schemas.py
 flag_engine/environments/__init__.py
 flag_engine/environments/builders.py
 flag_engine/environments/models.py
-flag_engine/environments/schemas.py
 flag_engine/environments/integrations/__init__.py
 flag_engine/environments/integrations/models.py
-flag_engine/environments/integrations/schemas.py
 flag_engine/features/__init__.py
 flag_engine/features/constants.py
 flag_engine/features/models.py
-flag_engine/features/schemas.py
 flag_engine/identities/__init__.py
 flag_engine/identities/builders.py
 flag_engine/identities/models.py
-flag_engine/identities/schemas.py
 flag_engine/identities/traits/__init__.py
+flag_engine/identities/traits/constants.py
 flag_engine/identities/traits/models.py
-flag_engine/identities/traits/schemas.py
+flag_engine/identities/traits/types.py
 flag_engine/organisations/__init__.py
 flag_engine/organisations/models.py
-flag_engine/organisations/schemas.py
 flag_engine/projects/__init__.py
 flag_engine/projects/models.py
-flag_engine/projects/schemas.py
 flag_engine/segments/__init__.py
 flag_engine/segments/constants.py
 flag_engine/segments/evaluator.py
 flag_engine/segments/models.py
-flag_engine/segments/schemas.py
+flag_engine/segments/types.py
 flag_engine/utils/__init__.py
-flag_engine/utils/collections.py
 flag_engine/utils/datetime.py
 flag_engine/utils/exceptions.py
 flag_engine/utils/hashing.py
 flag_engine/utils/semver.py
 flag_engine/utils/types.py
 flag_engine/utils/json/__init__.py
 flag_engine/utils/json/encoders.py
-flag_engine/utils/marshmallow/__init__.py
-flag_engine/utils/marshmallow/fields.py
-flag_engine/utils/marshmallow/schemas.py
 flagsmith_flag_engine.egg-info/PKG-INFO
 flagsmith_flag_engine.egg-info/SOURCES.txt
 flagsmith_flag_engine.egg-info/dependency_links.txt
 flagsmith_flag_engine.egg-info/requires.txt
 flagsmith_flag_engine.egg-info/top_level.txt
```

