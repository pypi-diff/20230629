# Comparing `tmp/flagsmith-flag-engine-3.5.1.tar.gz` & `tmp/flagsmith-flag-engine-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flagsmith-flag-engine-3.5.1.tar", last modified: Mon Jun 26 15:19:04 2023, max compression
+gzip compressed data, was "flagsmith-flag-engine-3.6.0.tar", last modified: Thu Jun 29 10:19:22 2023, max compression
```

## Comparing `flagsmith-flag-engine-3.5.1.tar` & `flagsmith-flag-engine-3.6.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.127701 flagsmith-flag-engine-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 15:19:04.127701 flagsmith-flag-engine-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.103701 flagsmith-flag-engine-3.5.1/flag_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.107701 flagsmith-flag-engine-3.5.1/flag_engine/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/document_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/api/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.111701 flagsmith-flag-engine-3.5.1/flag_engine/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/builders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.111701 flagsmith-flag-engine-3.5.1/flag_engine/environments/integrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/integrations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/integrations/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/environments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.111701 flagsmith-flag-engine-3.5.1/flag_engine/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/features/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/features/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/features/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.115701 flagsmith-flag-engine-3.5.1/flag_engine/identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.115701 flagsmith-flag-engine-3.5.1/flag_engine/identities/traits/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/traits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/traits/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/identities/traits/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.115701 flagsmith-flag-engine-3.5.1/flag_engine/organisations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/organisations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/organisations/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/organisations/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.115701 flagsmith-flag-engine-3.5.1/flag_engine/projects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/projects/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/projects/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.119701 flagsmith-flag-engine-3.5.1/flag_engine/segments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/segments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/segments/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/segments/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/segments/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/segments/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.123701 flagsmith-flag-engine-3.5.1/flag_engine/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.123701 flagsmith-flag-engine-3.5.1/flag_engine/utils/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/json/encoders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.123701 flagsmith-flag-engine-3.5.1/flag_engine/utils/marshmallow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/marshmallow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/marshmallow/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/marshmallow/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/semver.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/flag_engine/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 15:19:04.123701 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-26 15:19:04.000000 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-26 15:19:04.000000 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 15:19:04.000000 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 15:19:04.000000 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 15:19:04.000000 flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-26 15:19:04.127701 flagsmith-flag-engine-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-26 15:19:03.000000 flagsmith-flag-engine-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.613602 flagsmith-flag-engine-3.6.0/flag_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/document_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/api/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/builders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.617603 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/integrations/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/environments/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/features/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/identities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.621603 flagsmith-flag-engine-3.6.0/flag_engine/organisations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/organisations/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.625603 flagsmith-flag-engine-3.6.0/flag_engine/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/projects/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.625603 flagsmith-flag-engine-3.6.0/flag_engine/segments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/segments/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/json/encoders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flag_engine/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-29 10:19:22.629603 flagsmith-flag-engine-3.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-06-29 10:19:22.000000 flagsmith-flag-engine-3.6.0/setup.py
```

### Comparing `flagsmith-flag-engine-3.5.1/LICENSE.txt` & `flagsmith-flag-engine-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/PKG-INFO` & `flagsmith-flag-engine-3.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 3.5.1
+Version: 3.6.0
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-3.5.1/README.md` & `flagsmith-flag-engine-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/api/document_builders.py` & `flagsmith-flag-engine-3.6.0/flag_engine/api/document_builders.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/api/fields.py` & `flagsmith-flag-engine-3.6.0/flag_engine/api/fields.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/api/filters.py` & `flagsmith-flag-engine-3.6.0/flag_engine/api/filters.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/api/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/api/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/engine.py` & `flagsmith-flag-engine-3.6.0/flag_engine/engine.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/environments/builders.py` & `flagsmith-flag-engine-3.6.0/flag_engine/environments/builders.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/environments/models.py` & `flagsmith-flag-engine-3.6.0/flag_engine/environments/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,16 +37,16 @@
     api_key: str
     project: ProjectModel
     feature_states: typing.List[FeatureStateModel] = field(default_factory=list)
 
     name: str = None
     allow_client_traits: bool = True
     updated_at: datetime = field(default_factory=utcnow_with_tz)
-    use_mv_v2_evaluation: bool = False
     hide_sensitive_data: bool = False
+    use_identity_composite_key_for_hashing: bool = False
 
     amplitude_config: typing.Optional[IntegrationModel] = None
     dynatrace_config: typing.Optional[IntegrationModel] = None
     heap_config: typing.Optional[IntegrationModel] = None
     mixpanel_config: typing.Optional[IntegrationModel] = None
     rudderstack_config: typing.Optional[IntegrationModel] = None
     segment_config: typing.Optional[IntegrationModel] = None
```

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/environments/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/environments/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     id = fields.Int()
     api_key = fields.Str()
     updated_at = fields.DateTime()
 
     name = fields.Str(required=False)
     allow_client_traits = fields.Bool(required=False, default=True)
     hide_disabled_flags = fields.Bool(required=False, allow_none=True)
-    use_mv_v2_evaluation = fields.Bool(required=False, default=False)
+    use_identity_composite_key_for_hashing = fields.Bool(required=False, default=False)
     hide_sensitive_data = fields.Bool(required=False, default=False)
 
     amplitude_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     dynatrace_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     heap_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     mixpanel_config = fields.Nested(IntegrationSchema, required=False, allow_none=True)
     rudderstack_config = fields.Nested(
```

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/features/models.py` & `flagsmith-flag-engine-3.6.0/flag_engine/features/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/features/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/features/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/identities/models.py` & `flagsmith-flag-engine-3.6.0/flag_engine/identities/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,20 @@
     def composite_key(self) -> str:
         return self.generate_composite_key(self.environment_api_key, self.identifier)
 
     @staticmethod
     def generate_composite_key(env_key: str, identifier: str) -> str:
         return f"{env_key}_{identifier}"
 
-    def get_hash_key(self, use_mv_v2_evaluation: bool) -> str:
-        return self.composite_key if use_mv_v2_evaluation else self.identifier
+    def get_hash_key(self, use_identity_composite_key_for_hashing: bool) -> str:
+        return (
+            self.composite_key
+            if use_identity_composite_key_for_hashing
+            else self.identifier
+        )
 
     def update_traits(
         self, traits: typing.List[TraitModel]
     ) -> typing.Tuple[typing.List[TraitModel], bool]:
         existing_traits = {trait.trait_key: trait for trait in self.identity_traits}
         traits_changed = False
```

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/identities/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/identities/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/identities/traits/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/identities/traits/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/projects/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/projects/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/segments/constants.py` & `flagsmith-flag-engine-3.6.0/flag_engine/segments/constants.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/segments/evaluator.py` & `flagsmith-flag-engine-3.6.0/flag_engine/segments/evaluator.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/segments/models.py` & `flagsmith-flag-engine-3.6.0/flag_engine/segments/models.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/segments/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/segments/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/utils/hashing.py` & `flagsmith-flag-engine-3.6.0/flag_engine/utils/hashing.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/utils/marshmallow/schemas.py` & `flagsmith-flag-engine-3.6.0/flag_engine/utils/marshmallow/schemas.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/utils/semver.py` & `flagsmith-flag-engine-3.6.0/flag_engine/utils/semver.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flag_engine/utils/types.py` & `flagsmith-flag-engine-3.6.0/flag_engine/utils/types.py`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/PKG-INFO` & `flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flagsmith-flag-engine
-Version: 3.5.1
+Version: 3.6.0
 Summary: Flag engine for the Flagsmith API.
 Home-page: https://github.com/Flagsmith/flagsmith-engine
 Author: Flagsmith
 Author-email: support@flagsmith.com
 License: BSD3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `flagsmith-flag-engine-3.5.1/flagsmith_flag_engine.egg-info/SOURCES.txt` & `flagsmith-flag-engine-3.6.0/flagsmith_flag_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flagsmith-flag-engine-3.5.1/setup.py` & `flagsmith-flag-engine-3.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="flagsmith-flag-engine",
-    version="3.5.1",
+    version="3.6.0",
     author="Flagsmith",
     author_email="support@flagsmith.com",
     packages=find_packages(include=["flag_engine", "flag_engine.*"]),
     url="https://github.com/Flagsmith/flagsmith-engine",
     license="BSD3",
     description="Flag engine for the Flagsmith API.",
     long_description=open("README.md").read(),
```

