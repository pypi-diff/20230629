# Comparing `tmp/pulp-gem-0.1.0.tar.gz` & `tmp/pulp-gem-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-gem-0.1.0.tar", last modified: Mon Jun 26 19:17:57 2023, max compression
+gzip compressed data, was "pulp-gem-0.1.1.tar", last modified: Thu Jun 29 19:11:43 2023, max compression
```

## Comparing `pulp-gem-0.1.0.tar` & `pulp-gem-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/COMMITMENT
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/functest_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.238227 pulp-gem-0.1.0/pulp_gem/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-26 19:17:55.000000 pulp-gem-0.1.0/pulp_gem/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/management/commands/datarepair-shallow-gems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0002_gemrepository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/app/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/publishing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/tasks/synchronizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/app/viewsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/functional/api/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_content_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_remotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_download_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_full_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/functional/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/pulp_gem/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pulp_gem/tests/unit/test_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:17:57.238227 pulp-gem-0.1.0/pulp_gem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-26 19:17:57.000000 pulp-gem-0.1.0/pulp_gem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:17:56.000000 pulp-gem-0.1.0/pulp_gem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 19:17:57.242227 pulp-gem-0.1.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-26 19:17:55.000000 pulp-gem-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/test_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 19:17:43.000000 pulp-gem-0.1.0/unittest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.706645 pulp-gem-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-29 19:11:41.000000 pulp-gem-0.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/COMMITMENT
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    18046 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 19:11:43.706645 pulp-gem-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/functest_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.698645 pulp-gem-0.1.1/pulp_gem/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-29 19:11:42.000000 pulp-gem-0.1.1/pulp_gem/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/app/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/app/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/management/commands/datarepair-shallow-gems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0002_gemrepository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/app/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/tasks/publishing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/tasks/synchronizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/app/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.702645 pulp-gem-0.1.1/pulp_gem/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.706645 pulp-gem-0.1.1/pulp_gem/tests/functional/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_crud_content_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_crud_remotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_download_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_full_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/functional/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.706645 pulp-gem-0.1.1/pulp_gem/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/unit/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pulp_gem/tests/unit/test_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:11:43.698645 pulp-gem-0.1.1/pulp_gem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:11:43.000000 pulp-gem-0.1.1/pulp_gem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 19:11:43.706645 pulp-gem-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-06-29 19:11:42.000000 pulp-gem-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/test_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 19:11:27.000000 pulp-gem-0.1.1/unittest_requirements.txt
```

### Comparing `pulp-gem-0.1.0/CHANGES.rst` & `pulp-gem-0.1.1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,27 @@
     To add a new change log entry, please see
     https://docs.pulpproject.org/en/3.0/nightly/contributing/git.html#changelog-update
 
     WARNING: Don't drop the next directive!
 
 .. towncrier release notes start
 
+0.1.1 (2023-06-29)
+==================
+
+Bugfixes
+--------
+
+- Fixed the detection of prerelease versions.
+  `#114 <https://github.com/pulp/pulp_gem/issues/114>`__
+
+
+----
+
+
 0.1.0 (2023-06-26)
 ==================
 
 Features
 --------
 
 - Added support for pull-through caching. Add a remote to a distribution to enable this feature.
```

### Comparing `pulp-gem-0.1.0/COMMITMENT` & `pulp-gem-0.1.1/COMMITMENT`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/COPYRIGHT` & `pulp-gem-0.1.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/LICENSE` & `pulp-gem-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/PKG-INFO` & `pulp-gem-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-gem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gemfile plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Project-URL: Documentation, https://docs.pulpproject.org/pulp_gem/
 Project-URL: Source, https://github.com/pulp/pulp_gem
```

### Comparing `pulp-gem-0.1.0/pulp_gem/app/management/commands/datarepair-shallow-gems.py` & `pulp-gem-0.1.1/pulp_gem/app/management/commands/datarepair-shallow-gems.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0001_initial.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0002_gemrepository.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0002_gemrepository.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0003_move_data_to_new_master_distribution_model.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0004_alter_gemcontent_content_ptr_and_more.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0005_rename_gemcontent_shallowgemcontent.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py` & `pulp-gem-0.1.1/pulp_gem/app/migrations/0006_gemremote_excludes_gemremote_includes_and_more.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/models.py` & `pulp-gem-0.1.1/pulp_gem/app/models.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/serializers.py` & `pulp-gem-0.1.1/pulp_gem/app/serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/tasks/publishing.py` & `pulp-gem-0.1.1/pulp_gem/app/tasks/publishing.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/app/tasks/synchronizing.py` & `pulp-gem-0.1.1/pulp_gem/app/tasks/synchronizing.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,26 @@
             versions_result = await versions_downloader.run()
             await pr_download_versions.aincrement()
 
         async with ProgressReport(message="Parsing versions list") as pr_parse_versions:
             async with ProgressReport(message="Parsing versions info") as pr_parse_info:
                 async for name, versions, md5_sum in read_versions(versions_result.path):
                     await pr_parse_versions.aincrement()
-                    if not NAME_REGEX.match(name):
+                    if not NAME_REGEX.fullmatch(name):
                         log.warn(f"Skipping invalid gem name: '{name}'.")
                         continue
                     if not self.remote.prereleases:
-                        versions = [version for version in versions if VERSION_REGEX.match(version)]
+                        versions = [
+                            version for version in versions if VERSION_REGEX.fullmatch(version)
+                        ]
                     else:
                         versions = [
                             version
                             for version in versions
-                            if PRERELEASE_VERSION_REGEX.match(version)
+                            if PRERELEASE_VERSION_REGEX.fullmatch(version)
                         ]
                     if self.remote.includes:
                         if name not in self.remote.includes:
                             continue
                         version_requirements = self.remote.includes[name]
                         if version_requirements is not None:
                             versions = [
```

### Comparing `pulp-gem-0.1.0/pulp_gem/app/viewsets.py` & `pulp-gem-0.1.1/pulp_gem/app/viewsets.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/specs.py` & `pulp-gem-0.1.1/pulp_gem/specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -97,15 +97,15 @@
                 continue
             name, versions, md5_sum = line.split(" ", maxsplit=2)
             versions = versions.split(",")
             entry = results.get(name) or ([], "")
             results[name] = (entry[0] + versions, md5_sum)
     for name, (versions, md5_sum) in results.items():
         # Sanitize name
-        if not NAME_REGEX.match(name):
+        if not NAME_REGEX.fullmatch(name):
             raise ValueError(f"Invalid gem name: {name}")
         yield name, versions, md5_sum
 
 
 async def read_info(relative_path, versions):
     # File starts with:
     #   ---
@@ -120,17 +120,17 @@
                 continue
             gem_info = {}
             front, back = line.split("|")
             version, dependencies = front.split(" ", maxsplit=1)
             if version not in versions:
                 continue
             # Sanitize version
-            if VERSION_REGEX.match(version):
+            if VERSION_REGEX.fullmatch(version):
                 gem_info["prerelease"] = False
-            elif PRERELEASE_VERSION_REGEX.match(version):
+            elif PRERELEASE_VERSION_REGEX.fullmatch(version):
                 gem_info["prerelease"] = True
             else:
                 raise ValueError(f"Invalid version string: {version}")
             gem_info["version"] = version
             dependencies = dependencies.strip()
             if dependencies:
                 gem_info["dependencies"] = dict(
@@ -205,20 +205,20 @@
         with archive.extractfile("metadata.gz") as md_file:
             data = yaml.load(gzip.decompress(md_file.read()), Loader=RubyMarshalYamlLoader)
     gem_info = {
         "name": data.values["name"],
         "version": data.values["version"].values["version"],
     }
     # Sanitize name
-    if not NAME_REGEX.match(gem_info["name"]):
+    if not NAME_REGEX.fullmatch(gem_info["name"]):
         raise ValueError(f"Invalid gem name: {gem_info['name']}")
     # Sanitize version
-    if VERSION_REGEX.match(gem_info["version"]):
+    if VERSION_REGEX.fullmatch(gem_info["version"]):
         gem_info["prerelease"] = False
-    elif PRERELEASE_VERSION_REGEX.match(gem_info["version"]):
+    elif PRERELEASE_VERSION_REGEX.fullmatch(gem_info["version"]):
         gem_info["prerelease"] = True
     else:
         raise ValueError(f"Invalid version string: {gem_info['version']}")
     for key in ("required_ruby_version", "required_rubygems_version"):
         if (requirement := data.values.get(key)) is not None:
             gem_info[key] = _collapse_requirement(requirement)
     if (dependencies := data.values.get("dependencies")) is not None:
```

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_content_unit.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_crud_content_unit.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_crud_remotes.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_crud_remotes.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_download_content.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_download_content.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_full_mirror.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_full_mirror.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_publish.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_publish.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/api/test_sync.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/api/test_sync.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/conftest.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/constants.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 GEM_REPO_PATH = urljoin(BASE_REPO_PATH, "gem/gem/")
 
 GEM_PUBLICATION_PATH = urljoin(BASE_PUBLICATION_PATH, "gem/gem/")
 
 GEM_FIXTURE_URL = urljoin(PULP_FIXTURES_BASE_URL, "gem/")
 """The URL to a gem repository."""
 
-GEM_FIXTURE_COUNT = 6
+GEM_FIXTURE_COUNT = 4
 """The number of content units available at :data:`GEM_FIXTURE_URL`."""
 # This is 4 stable gems. There are also 2 prerelease gems not currently synced.
 
 GEM_FIXTURE_SUMMARY = {GEM_CONTENT_NAME: GEM_FIXTURE_COUNT}
 """The desired content summary after syncing :data:`GEM_FIXTURE_URL`."""
 
 GEM_URL = urljoin(GEM_FIXTURE_URL, "gems/amber-1.0.0.gem")
```

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/functional/utils.py` & `pulp-gem-0.1.1/pulp_gem/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/unit/test_serializers.py` & `pulp-gem-0.1.1/pulp_gem/tests/unit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem/tests/unit/test_spec.py` & `pulp-gem-0.1.1/pulp_gem/tests/unit/test_spec.py`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pulp_gem.egg-info/PKG-INFO` & `pulp-gem-0.1.1/pulp_gem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pulp-gem
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gemfile plugin for the Pulp Project
 Home-page: https://pulpproject.org/
 Author: Pulp Project Developers
 Author-email: pulp-dev@redhat.com
 License: GPLv2+
 Project-URL: Documentation, https://docs.pulpproject.org/pulp_gem/
 Project-URL: Source, https://github.com/pulp/pulp_gem
```

### Comparing `pulp-gem-0.1.0/pulp_gem.egg-info/SOURCES.txt` & `pulp-gem-0.1.1/pulp_gem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/pyproject.toml` & `pulp-gem-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pulp-gem-0.1.0/setup.py` & `pulp-gem-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     requirements = requirements.readlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="pulp-gem",
-    version="0.1.0",
+    version="0.1.1",
     description="Gemfile plugin for the Pulp Project",
     long_description=long_description,
     license="GPLv2+",
     author="Pulp Project Developers",
     author_email="pulp-dev@redhat.com",
     url="https://pulpproject.org/",
     python_requires=">=3.8",
```

