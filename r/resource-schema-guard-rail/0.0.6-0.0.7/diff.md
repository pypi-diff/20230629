# Comparing `tmp/resource-schema-guard-rail-0.0.6.tar.gz` & `tmp/resource-schema-guard-rail-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resource-schema-guard-rail-0.0.6.tar", last modified: Thu Jun  1 21:05:53 2023, max compression
+gzip compressed data, was "resource-schema-guard-rail-0.0.7.tar", last modified: Thu Jun 29 06:14:27 2023, max compression
```

## Comparing `resource-schema-guard-rail-0.0.6.tar` & `resource-schema-guard-rail-0.0.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.640442 resource-schema-guard-rail-0.0.6/
--rw-r--r--   0 sgathili   (504) staff       (20)    10142 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/LICENSE
--rw-r--r--   0 sgathili   (504) staff       (20)       63 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/MANIFEST.in
--rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-06-01 21:05:53.640549 resource-schema-guard-rail-0.0.6/PKG-INFO
--rw-r--r--   0 sgathili   (504) staff       (20)     3349 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/README.md
--rw-r--r--   0 sgathili   (504) staff       (20)      593 2023-06-01 21:05:53.641114 resource-schema-guard-rail-0.0.6/setup.cfg
--rw-r--r--   0 sgathili   (504) staff       (20)     2010 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/setup.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.634453 resource-schema-guard-rail-0.0.6/src/
--rw-r--r--   0 sgathili   (504) staff       (20)     2538 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/cli.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635517 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/
--rw-r--r--   0 sgathili   (504) staff       (20)     4023 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/PKG-INFO
--rw-r--r--   0 sgathili   (504) staff       (20)     1661 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/SOURCES.txt
--rw-r--r--   0 sgathili   (504) staff       (20)        1 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/dependency_links.txt
--rw-r--r--   0 sgathili   (504) staff       (20)       67 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/entry_points.txt
--rw-r--r--   0 sgathili   (504) staff       (20)      258 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/requires.txt
--rw-r--r--   0 sgathili   (504) staff       (20)        9 2023-06-01 21:05:53.000000 resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/top_level.txt
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635673 resource-schema-guard-rail-0.0.6/src/rpdk/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/__init__.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.635813 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/__init__.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636465 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)     3870 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/data_types.py
--rw-r--r--   0 sgathili   (504) staff       (20)     6239 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/runner.py
--rw-r--r--   0 sgathili   (504) staff       (20)    11087 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/stateful.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636669 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/templates/
--rw-r--r--   0 sgathili   (504) staff       (20)      590 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/templates/guard-result-pojo.output
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.636858 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/__init__.py
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.637138 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)     1579 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.637751 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)      555 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard
--rw-r--r--   0 sgathili   (504) staff       (20)     2855 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638190 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)     2699 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638589 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)    12380 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.638942 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)     2711 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard
-drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-01 21:05:53.640147 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/
--rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/__init__.py
--rw-r--r--   0 sgathili   (504) staff       (20)     4997 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/arg_handler.py
--rw-r--r--   0 sgathili   (504) staff       (20)      858 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/common.py
--rw-r--r--   0 sgathili   (504) staff       (20)      928 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/logger.py
--rw-r--r--   0 sgathili   (504) staff       (20)      893 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/miscellaneous.py
--rw-r--r--   0 sgathili   (504) staff       (20)     2510 2023-06-01 20:58:52.000000 resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/schema_utils.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.341894 resource-schema-guard-rail-0.0.7/
+-rw-r--r--   0 sgathili   (504) staff       (20)    10142 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/LICENSE
+-rw-r--r--   0 sgathili   (504) staff       (20)       63 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/MANIFEST.in
+-rw-r--r--   0 sgathili   (504) staff       (20)     4422 2023-06-29 06:14:27.341961 resource-schema-guard-rail-0.0.7/PKG-INFO
+-rw-r--r--   0 sgathili   (504) staff       (20)     3748 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/README.md
+-rw-r--r--   0 sgathili   (504) staff       (20)      593 2023-06-29 06:14:27.342345 resource-schema-guard-rail-0.0.7/setup.cfg
+-rw-r--r--   0 sgathili   (504) staff       (20)     2010 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/setup.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.336517 resource-schema-guard-rail-0.0.7/src/
+-rw-r--r--   0 sgathili   (504) staff       (20)     2538 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/cli.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.337896 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/
+-rw-r--r--   0 sgathili   (504) staff       (20)     4422 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/PKG-INFO
+-rw-r--r--   0 sgathili   (504) staff       (20)     1661 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/SOURCES.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)        1 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/dependency_links.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)       67 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/entry_points.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)      258 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/requires.txt
+-rw-r--r--   0 sgathili   (504) staff       (20)        9 2023-06-29 06:14:27.000000 resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/top_level.txt
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.338058 resource-schema-guard-rail-0.0.7/src/rpdk/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.338193 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.338780 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     3870 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/data_types.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     6239 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/runner.py
+-rw-r--r--   0 sgathili   (504) staff       (20)    11111 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/stateful.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.338966 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/templates/
+-rw-r--r--   0 sgathili   (504) staff       (20)      590 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/templates/guard-result-pojo.output
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.339121 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/__init__.py
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.339369 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/combiners/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/combiners/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     1579 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.339827 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      555 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard
+-rw-r--r--   0 sgathili   (504) staff       (20)     2855 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.340222 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/permissions/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/permissions/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2699 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.340534 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/stateful/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/stateful/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)    12380 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.340834 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/tags/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/tags/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2711 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard
+drwxr-xr-x   0 sgathili   (504) staff       (20)        0 2023-06-29 06:14:27.341749 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/
+-rw-r--r--   0 sgathili   (504) staff       (20)        0 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/__init__.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     4997 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/arg_handler.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      858 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/common.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      928 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/logger.py
+-rw-r--r--   0 sgathili   (504) staff       (20)      893 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/miscellaneous.py
+-rw-r--r--   0 sgathili   (504) staff       (20)     2510 2023-06-29 06:13:56.000000 resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/schema_utils.py
```

### Comparing `resource-schema-guard-rail-0.0.6/LICENSE` & `resource-schema-guard-rail-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/PKG-INFO` & `resource-schema-guard-rail-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.6
+Version: 0.0.7
 Summary: Schema Guard Rail
 Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,18 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CloudFormation - Resource Schema Guard Rail
+![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
 [![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
-
+[![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
 
 ### Notes
 This is not a stable version (Beta), it's still under development
 
 ## Overview
 AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
```

### Comparing `resource-schema-guard-rail-0.0.6/README.md` & `resource-schema-guard-rail-0.0.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # CloudFormation - Resource Schema Guard Rail
+![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
 [![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
-
+[![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
 
 ### Notes
 This is not a stable version (Beta), it's still under development
 
 ## Overview
 AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
```

### Comparing `resource-schema-guard-rail-0.0.6/setup.cfg` & `resource-schema-guard-rail-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/setup.py` & `resource-schema-guard-rail-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         else:
             requirements.append(line)
     return requirements
 
 
 setuptools.setup(
     name="resource-schema-guard-rail",
-    version="0.0.6",
+    version="0.0.7",
     description="Schema Guard Rail",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Amazon Web Services",
     author_email="aws-cloudformation-developers@amazon.com",
     packages=setuptools.find_packages(where="src"),
     package_dir={"": "src"},
```

### Comparing `resource-schema-guard-rail-0.0.6/src/cli.py` & `resource-schema-guard-rail-0.0.7/src/cli.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/PKG-INFO` & `resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resource-schema-guard-rail
-Version: 0.0.6
+Version: 0.0.7
 Summary: Schema Guard Rail
 Home-page: UNKNOWN
 Author: Amazon Web Services
 Author-email: aws-cloudformation-developers@amazon.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -15,16 +15,18 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CloudFormation - Resource Schema Guard Rail
+![Apache 2.0 License](https://img.shields.io/github/license/aws-cloudformation/resource-schema-guard-rail)
 [![Pull Request CI](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml/badge.svg?branch=main)](https://github.com/aws-cloudformation/resource-schema-guard-rail/actions/workflows/pr-ci.yml)
-
+[![PyPI](https://img.shields.io/pypi/v/resource-schema-guard-rail?label=pypi)](https://badge.fury.io/py/resource-schema-guard-rail)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/resource-schema-guard-rail?label=python)](https://pypi.org/project/resource-schema-guard-rail/)
 
 ### Notes
 This is not a stable version (Beta), it's still under development
 
 ## Overview
 AWS CloudFormation Resource Schema Guard Rail is an open-source tool, which uses [CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard/) policy-as-code evaluation engine to assess resource schema compliance. It validates json resource schemas against the AWS CloudFormation modeling best practices.
```

### Comparing `resource-schema-guard-rail-0.0.6/src/resource_schema_guard_rail.egg-info/SOURCES.txt` & `resource-schema-guard-rail-0.0.7/src/resource_schema_guard_rail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/data_types.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/data_types.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/runner.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/runner.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/stateful.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/stateful.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 Typical usage example:
 
     schema_v1 = ...
     schema_v2 = ...
     schema_meta_diff = schema_diff(schema_v1, schema_v2)
 """
+import json
 import re
 from copy import copy
 from enum import auto
 from functools import partial
 from typing import Any, Dict, Iterable
 
 import strenum
@@ -84,15 +85,15 @@
     """schema diff function to get formatted schema diff from deep diff"""
     deep_diff = DeepDiff(
         resolve_schema(previous_json),
         resolve_schema(current_json),
         ignore_order=True,
         verbose_level=2,
     )
-    print(_translate_meta_diff(deep_diff.to_dict()))
+    print(json.dumps(_translate_meta_diff(deep_diff.to_dict())))
     return _translate_meta_diff(deep_diff.to_dict())
 
 
 def _is_combiner_property(path_list):
     """This method accepts an array of steps.
     If set is not empty and it starts with `properties`
     and ends with combiner, then it's considered
```

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/core/templates/guard-result-pojo.output` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/core/templates/guard-result-pojo.output`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/combiners/schema-linter-combiner-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/schema-linter-core-arn-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/core/schema-linter-core-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/permissions/schema-linter-core-permission-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/stateful/schema-stateful-cfn-enforced-checks.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/rule_library/tags/schema-linter-core-tagging-rules.guard`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/arg_handler.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/arg_handler.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/common.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/common.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/logger.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/logger.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/miscellaneous.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `resource-schema-guard-rail-0.0.6/src/rpdk/guard_rail/utils/schema_utils.py` & `resource-schema-guard-rail-0.0.7/src/rpdk/guard_rail/utils/schema_utils.py`

 * *Files identical despite different names*

