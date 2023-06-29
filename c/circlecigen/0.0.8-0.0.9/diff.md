# Comparing `tmp/circlecigen-0.0.8.tar.gz` & `tmp/circlecigen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circlecigen-0.0.8.tar", last modified: Tue Jun 27 05:19:46 2023, max compression
+gzip compressed data, was "circlecigen-0.0.9.tar", last modified: Thu Jun 29 20:41:44 2023, max compression
```

## Comparing `circlecigen-0.0.8.tar` & `circlecigen-0.0.9.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.025237 circlecigen-0.0.8/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.circleci/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.codeclimate.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.pylintrc
--rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-27 05:19:41.000000 circlecigen-0.0.8/.python-version
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-27 05:19:41.000000 circlecigen-0.0.8/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26079 2023-06-27 05:19:46.029237 circlecigen-0.0.8/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-27 05:19:41.000000 circlecigen-0.0.8/Pipfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    25444 2023-06-27 05:19:41.000000 circlecigen-0.0.8/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:41.000000 circlecigen-0.0.8/__init__.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.025237 circlecigen-0.0.8/circlecigen.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26079 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-27 05:19:46.000000 circlecigen-0.0.8/circlecigen.egg-info/top_level.txt
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/env_test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      367 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/custom.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/default.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/dev.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/multi.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/nonprod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      587 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/post-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      312 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/pre-approve.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/prod.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-27 05:19:41.000000 circlecigen-0.0.8/env_test/template_generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-27 05:19:41.000000 circlecigen-0.0.8/notes.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-27 05:19:41.000000 circlecigen-0.0.8/op.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-27 05:19:41.000000 circlecigen-0.0.8/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-27 05:19:41.000000 circlecigen-0.0.8/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-27 05:19:46.029237 circlecigen-0.0.8/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-27 05:19:41.000000 circlecigen-0.0.8/setup.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-27 05:19:45.000000 circlecigen-0.0.8/src/_version.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3028 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6770 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2428 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-27 05:19:41.000000 circlecigen-0.0.8/src/utils.py
-drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-27 05:19:46.029237 circlecigen-0.0.8/test/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/generated_config_setup.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/nonprod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      146 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/nonprod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/prod-us-east-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      140 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/prod-us-west-2.tfvars.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/template_generated_config.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_circlecigen.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3444 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_template.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_tfvars.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-27 05:19:41.000000 circlecigen-0.0.8/test/test_utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.124463 circlecigen-0.0.9/
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/.circleci/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3995 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.circleci/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      350 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.codeclimate.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.gitignore
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      866 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    18369 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.pylintrc
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        7 2023-06-29 20:41:39.000000 circlecigen-0.0.9/.python-version
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1075 2023-06-29 20:41:39.000000 circlecigen-0.0.9/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-06-29 20:41:44.124463 circlecigen-0.0.9/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      432 2023-06-29 20:41:39.000000 circlecigen-0.0.9/Pipfile
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    25450 2023-06-29 20:41:39.000000 circlecigen-0.0.9/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:39.000000 circlecigen-0.0.9/__init__.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/circlecigen.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26085 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1224 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       52 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       26 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2023-06-29 20:41:44.000000 circlecigen-0.0.9/circlecigen.egg-info/top_level.txt
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/env_test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3037 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/custom.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       82 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/default.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       39 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/dev.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      782 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/multi.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       43 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/nonprod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      593 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/post-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      315 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/pre-approve.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       40 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/prod.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-29 20:41:39.000000 circlecigen-0.0.9/env_test/template_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      313 2023-06-29 20:41:39.000000 circlecigen-0.0.9/notes.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2023-06-29 20:41:39.000000 circlecigen-0.0.9/op.env
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      711 2023-06-29 20:41:39.000000 circlecigen-0.0.9/pyproject.toml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      365 2023-06-29 20:41:39.000000 circlecigen-0.0.9/requirements.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-06-29 20:41:44.124463 circlecigen-0.0.9/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      847 2023-06-29 20:41:39.000000 circlecigen-0.0.9/setup.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.120463 circlecigen-0.0.9/src/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      160 2023-06-29 20:41:44.000000 circlecigen-0.0.9/src/_version.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3028 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6770 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2430 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-06-29 20:41:39.000000 circlecigen-0.0.9/src/utils.py
+drwxr-sr-x   0 circleci  (3434) circleci  (3434)        0 2023-06-29 20:41:44.124463 circlecigen-0.0.9/test/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6273 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2222 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/generated_config_setup.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/nonprod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      147 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/nonprod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/prod-us-east-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      141 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/prod-us-west-2.tfvars.json
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3684 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/template_generated_config.yml
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_circlecigen.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3444 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_template.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2340 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_tfvars.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1490 2023-06-29 20:41:39.000000 circlecigen-0.0.9/test/test_utils.py
```

### Comparing `circlecigen-0.0.8/.circleci/config.yml` & `circlecigen-0.0.9/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/.pre-commit-config.yaml` & `circlecigen-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/.pylintrc` & `circlecigen-0.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/LICENSE` & `circlecigen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/PKG-INFO` & `circlecigen-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: circlecigen
-Version: 0.0.8
-Summary: Opinionated generation of continuation pipelines
-Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
-Author: Nic Cheneweth
-Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
-Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
-Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -274,40 +258,40 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the instance_name.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.
 
 ```yaml
       - terraform/plan:
-          name: {{env_instance}} change plan
+          name: {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           filters: {{filters}}{{priorapprovalrequired}}
 ```
 
 The indenting is important. This example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can pass any pipeline command found in any orb you have included, but more importantly from the config.yaml itself.  
 
 So, for the infra-dev role, circlecigen will create a workflow that runs a terraform plan job using the specific, associated _instance_.tfvar.json var-file. Each such instance runs in parallel.
 
 **.circleci/post-approve.yml**  
 
 Then specify the job to be run if the above plans are approved.  
 ```yaml
       - terraform/apply:
-          name: apply {{env_instance}} change plan
+          name: apply {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           after-terraform:
             - after-deployment-commands
           requires:
             - approve {{role}} changes
           filters: {{filters}}
@@ -681,20 +665,20 @@
 #### 2. Setup example for a job to run nightly integration tests
 
 In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
 
 We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
 ```yaml
       - integration-tests:
-          name: {{env_instance}} integration test
+          name: {{instance_name}} integration test
           context: << pipeline.parameters.context >>
           shell: << pipeline.parameters.shell-options >>
           executor-image: << pipeline.parameters.executor-image >>
-          instance_name: {{env_instance}}
-          workspace: {{env_instance}}
+          instance_name: {{instance_name}}
+          workspace: {{instance_name}}
           filters: {{filters}}
 ```
 
 The resulting pipeline from using the above custom template would then look like the following:
 ```yaml
 ---
 version: 2.1
@@ -787,8 +771,8 @@
           name: prod-us-east-2 integration test
           context: << pipeline.parameters.context >>
           shell: << pipeline.parameters.shell-options >>
           executor-image: << pipeline.parameters.executor-image >>
           instance_name: prod-us-east-2
           workspace: prod-us-east-2
           filters: *on-push-main
-```
+```
```

#### html2text {}

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.8 Summary: Opinionated
-generation of continuation pipelines Home-page: https://github.com/
-ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
-thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
-circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
-circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
-License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -134,32 +125,32 @@
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. All values in the
-env_instance.tfvars.json configuration are avaliable to be used in the jinja
+instance_name.tfvars.json configuration are avaliable to be used in the jinja
 template. Keep in mind that the same yaml template is used for each role so it
 will not work to have a value that ONLY exists in a single instance or role if
 the value appears in the yaml template. ```yaml - terraform/plan: name: {
-{env_instance}} change plan context: << pipeline.parameters.context >>
-workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment filters: {{filters}}{
-{priorapprovalrequired}} ``` The indenting is important. This example is using
-the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
-terraform). Note that in the before-terraform parameter you can pass any
-pipeline command found in any orb you have included, but more importantly from
-the config.yaml itself. So, for the infra-dev role, circlecigen will create a
-workflow that runs a terraform plan job using the specific, associated
+{instance_name}} change plan context: << pipeline.parameters.context >>
+workspace: {{instance_name}} var-file: {{envpath}}/{
+{instance_name}}.tfvars.json before-terraform: - set-environment filters: {
+{filters}}{{priorapprovalrequired}} ``` The indenting is important. This
+example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/
+orb/twdps/terraform). Note that in the before-terraform parameter you can pass
+any pipeline command found in any orb you have included, but more importantly
+from the config.yaml itself. So, for the infra-dev role, circlecigen will
+create a workflow that runs a terraform plan job using the specific, associated
 _instance_.tfvar.json var-file. Each such instance runs in parallel.
 **.circleci/post-approve.yml** Then specify the job to be run if the above
-plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+plans are approved. ```yaml - terraform/apply: name: apply {{instance_name}}
 change plan context: << pipeline.parameters.context >> workspace: {
-{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+{instance_name}} var-file: {{envpath}}/{{instance_name}}.tfvars.json before-
 terraform: - set-environment after-terraform: - after-deployment-commands
 requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
 this template will run terraform apply, and in addition to running the set-
 environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
@@ -263,29 +254,29 @@
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
 ``` #### 2. Setup example for a job to run nightly integration tests In this
 example we start by setting up the `environments/multi.json` and `environments/
 default.json` as from before. We also set up any relevant role-specific
 overrides, and the CircleCI config file (`.circleci/config.yml`) as from
 before. We then create a custom template file which will be specified with the
 `--template` flag. Let's use the example below: ```yaml - integration-tests:
-name: {{env_instance}} integration test context: << pipeline.parameters.context
->> shell: << pipeline.parameters.shell-options >> executor-image: <<
-pipeline.parameters.executor-image >> instance_name: {{env_instance}}
-workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
-from using the above custom template would then look like the following:
-```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
-push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
-setup-commands: parameters: ... steps: ... static-code-test-commands:
-parameters: ... steps: ... before-instance-specific-parallel-job-commands:
-parameters: ... steps: ... after-instance-specific-parallel-job-commands:
-parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
-image: ... steps: - setup-commands: parameters: << parameters... >> - static-
-code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
-parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
-tests: name: nonprod-us-west-2 integration test context: <<
+name: {{instance_name}} integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: {
+{instance_name}} workspace: {{instance_name}} filters: {{filters}} ``` The
+resulting pipeline from using the above custom template would then look like
+the following: ```yaml --- version: 2.1 orbs: continuation: circleci/
+continuation@0.3.1 on-push-main: &on-push-main branches: only: /main/ tags:
+ignore: /.*/ commands: setup-commands: parameters: ... steps: ... static-code-
+test-commands: parameters: ... steps: ... before-instance-specific-parallel-
+job-commands: parameters: ... steps: ... after-instance-specific-parallel-job-
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+integration-tests: name: nonprod-us-west-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
 integration-tests: name: nonprod-us-east-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
```

### Comparing `circlecigen-0.0.8/README.md` & `circlecigen-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: circlecigen
+Version: 0.0.9
+Summary: Opinionated generation of continuation pipelines
+Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
+Author: Nic Cheneweth
+Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
+Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
+Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 	<p>
 		<img alt="Thoughtworks Logo" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/thoughtworks_flamingo_wave.png?sanitize=true" width=200 />
     <br />
 		<img alt="DPS Title" src="https://raw.githubusercontent.com/ThoughtWorks-DPS/static/master/EMPCPlatformStarterKitsImage.png?sanitize=true" width=350/>
 	</p>
   <br />
@@ -258,40 +274,40 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the instance_name.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.
 
 ```yaml
       - terraform/plan:
-          name: {{env_instance}} change plan
+          name: {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           filters: {{filters}}{{priorapprovalrequired}}
 ```
 
 The indenting is important. This example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can pass any pipeline command found in any orb you have included, but more importantly from the config.yaml itself.  
 
 So, for the infra-dev role, circlecigen will create a workflow that runs a terraform plan job using the specific, associated _instance_.tfvar.json var-file. Each such instance runs in parallel.
 
 **.circleci/post-approve.yml**  
 
 Then specify the job to be run if the above plans are approved.  
 ```yaml
       - terraform/apply:
-          name: apply {{env_instance}} change plan
+          name: apply {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           after-terraform:
             - after-deployment-commands
           requires:
             - approve {{role}} changes
           filters: {{filters}}
@@ -665,20 +681,20 @@
 #### 2. Setup example for a job to run nightly integration tests
 
 In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
 
 We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
 ```yaml
       - integration-tests:
-          name: {{env_instance}} integration test
+          name: {{instance_name}} integration test
           context: << pipeline.parameters.context >>
           shell: << pipeline.parameters.shell-options >>
           executor-image: << pipeline.parameters.executor-image >>
-          instance_name: {{env_instance}}
-          workspace: {{env_instance}}
+          instance_name: {{instance_name}}
+          workspace: {{instance_name}}
           filters: {{filters}}
 ```
 
 The resulting pipeline from using the above custom template would then look like the following:
 ```yaml
 ---
 version: 2.1
@@ -771,8 +787,8 @@
           name: prod-us-east-2 integration test
           context: << pipeline.parameters.context >>
           shell: << pipeline.parameters.shell-options >>
           executor-image: << pipeline.parameters.executor-image >>
           instance_name: prod-us-east-2
           workspace: prod-us-east-2
           filters: *on-push-main
-```
+```
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.9 Summary: Opinionated
+generation of continuation pipelines Home-page: https://github.com/
+ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
+thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
+circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
+circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
+License-File: LICENSE
                              [Thoughtworks Logo]
                                   [DPS Title]
 
                              **** circlecigen ****
 [https://dl.circleci.com/status-badge/img/gh/ThoughtWorks-DPS/circlecigen/tree/
   main.svg?style=shield] [https://img.shields.io/badge/license-MIT-blue.svg]
 
@@ -125,32 +134,32 @@
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. All values in the
-env_instance.tfvars.json configuration are avaliable to be used in the jinja
+instance_name.tfvars.json configuration are avaliable to be used in the jinja
 template. Keep in mind that the same yaml template is used for each role so it
 will not work to have a value that ONLY exists in a single instance or role if
 the value appears in the yaml template. ```yaml - terraform/plan: name: {
-{env_instance}} change plan context: << pipeline.parameters.context >>
-workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment filters: {{filters}}{
-{priorapprovalrequired}} ``` The indenting is important. This example is using
-the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
-terraform). Note that in the before-terraform parameter you can pass any
-pipeline command found in any orb you have included, but more importantly from
-the config.yaml itself. So, for the infra-dev role, circlecigen will create a
-workflow that runs a terraform plan job using the specific, associated
+{instance_name}} change plan context: << pipeline.parameters.context >>
+workspace: {{instance_name}} var-file: {{envpath}}/{
+{instance_name}}.tfvars.json before-terraform: - set-environment filters: {
+{filters}}{{priorapprovalrequired}} ``` The indenting is important. This
+example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/
+orb/twdps/terraform). Note that in the before-terraform parameter you can pass
+any pipeline command found in any orb you have included, but more importantly
+from the config.yaml itself. So, for the infra-dev role, circlecigen will
+create a workflow that runs a terraform plan job using the specific, associated
 _instance_.tfvar.json var-file. Each such instance runs in parallel.
 **.circleci/post-approve.yml** Then specify the job to be run if the above
-plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+plans are approved. ```yaml - terraform/apply: name: apply {{instance_name}}
 change plan context: << pipeline.parameters.context >> workspace: {
-{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+{instance_name}} var-file: {{envpath}}/{{instance_name}}.tfvars.json before-
 terraform: - set-environment after-terraform: - after-deployment-commands
 requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
 this template will run terraform apply, and in addition to running the set-
 environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
@@ -254,29 +263,29 @@
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
 ``` #### 2. Setup example for a job to run nightly integration tests In this
 example we start by setting up the `environments/multi.json` and `environments/
 default.json` as from before. We also set up any relevant role-specific
 overrides, and the CircleCI config file (`.circleci/config.yml`) as from
 before. We then create a custom template file which will be specified with the
 `--template` flag. Let's use the example below: ```yaml - integration-tests:
-name: {{env_instance}} integration test context: << pipeline.parameters.context
->> shell: << pipeline.parameters.shell-options >> executor-image: <<
-pipeline.parameters.executor-image >> instance_name: {{env_instance}}
-workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
-from using the above custom template would then look like the following:
-```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
-push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
-setup-commands: parameters: ... steps: ... static-code-test-commands:
-parameters: ... steps: ... before-instance-specific-parallel-job-commands:
-parameters: ... steps: ... after-instance-specific-parallel-job-commands:
-parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
-image: ... steps: - setup-commands: parameters: << parameters... >> - static-
-code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
-parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
-tests: name: nonprod-us-west-2 integration test context: <<
+name: {{instance_name}} integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: {
+{instance_name}} workspace: {{instance_name}} filters: {{filters}} ``` The
+resulting pipeline from using the above custom template would then look like
+the following: ```yaml --- version: 2.1 orbs: continuation: circleci/
+continuation@0.3.1 on-push-main: &on-push-main branches: only: /main/ tags:
+ignore: /.*/ commands: setup-commands: parameters: ... steps: ... static-code-
+test-commands: parameters: ... steps: ... before-instance-specific-parallel-
+job-commands: parameters: ... steps: ... after-instance-specific-parallel-job-
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+integration-tests: name: nonprod-us-west-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
 integration-tests: name: nonprod-us-east-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
```

### Comparing `circlecigen-0.0.8/circlecigen.egg-info/PKG-INFO` & `circlecigen-0.0.9/circlecigen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circlecigen
-Version: 0.0.8
+Version: 0.0.9
 Summary: Opinionated generation of continuation pipelines
 Home-page: https://github.com/ThoughtWorks-DPS/circlecigen
 Author: Nic Cheneweth
 Author-email: Nic Cheneweth <nchenewe@thoughtworks.com>
 Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/circlecigen
 Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/circlecigen/issues
 Classifier: Programming Language :: Python :: 3
@@ -274,40 +274,40 @@
 Next, the pipeline files.  
 
 **.circleci/config.yml**  
 Of course you must have the regular circleci pipeline file that responds to triggers and actually forms the basis of the generated pipeline. Everything in this file up through the Jobs: or workflow: directive (whichever comes first) forms the starting point for the generated pipeline.  
 
 **.circleci/pre-approve.yml**  
 
-This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the env_instance.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.    
+This file is a template that will be populate with instance specific info when the pipeline is generated from within the config.yml pipeline. All values in the instance_name.tfvars.json configuration are avaliable to be used in the jinja template. Keep in mind that the same yaml template is used for each role so it will not work to have a value that ONLY exists in a single instance or role if the value appears in the yaml template.
 
 ```yaml
       - terraform/plan:
-          name: {{env_instance}} change plan
+          name: {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           filters: {{filters}}{{priorapprovalrequired}}
 ```
 
 The indenting is important. This example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/terraform). Note that in the before-terraform parameter you can pass any pipeline command found in any orb you have included, but more importantly from the config.yaml itself.  
 
 So, for the infra-dev role, circlecigen will create a workflow that runs a terraform plan job using the specific, associated _instance_.tfvar.json var-file. Each such instance runs in parallel.
 
 **.circleci/post-approve.yml**  
 
 Then specify the job to be run if the above plans are approved.  
 ```yaml
       - terraform/apply:
-          name: apply {{env_instance}} change plan
+          name: apply {{instance_name}} change plan
           context: << pipeline.parameters.context >>
-          workspace: {{env_instance}}
-          var-file: {{envpath}}/{{env_instance}}.tfvars.json
+          workspace: {{instance_name}}
+          var-file: {{envpath}}/{{instance_name}}.tfvars.json
           before-terraform:
             - set-environment
           after-terraform:
             - after-deployment-commands
           requires:
             - approve {{role}} changes
           filters: {{filters}}
@@ -681,20 +681,20 @@
 #### 2. Setup example for a job to run nightly integration tests
 
 In this example we start by setting up the `environments/multi.json` and `environments/default.json` as from before. We also set up any relevant role-specific overrides, and the CircleCI config file (`.circleci/config.yml`) as from before.
 
 We then create a custom template file which will be specified with the `--template` flag. Let's use the example below:
 ```yaml
       - integration-tests:
-          name: {{env_instance}} integration test
+          name: {{instance_name}} integration test
           context: << pipeline.parameters.context >>
           shell: << pipeline.parameters.shell-options >>
           executor-image: << pipeline.parameters.executor-image >>
-          instance_name: {{env_instance}}
-          workspace: {{env_instance}}
+          instance_name: {{instance_name}}
+          workspace: {{instance_name}}
           filters: {{filters}}
 ```
 
 The resulting pipeline from using the above custom template would then look like the following:
 ```yaml
 ---
 version: 2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: circlecigen Version: 0.0.8 Summary: Opinionated
+Metadata-Version: 2.1 Name: circlecigen Version: 0.0.9 Summary: Opinionated
 generation of continuation pipelines Home-page: https://github.com/
 ThoughtWorks-DPS/circlecigen Author: Nic Cheneweth Author-email: Nic Cheneweth
 thoughtworks.com> Project-URL: Homepage, https://github.com/ThoughtWorks-DPS/
 circlecigen Project-URL: Bug Tracker, https://github.com/ThoughtWorks-DPS/
 circlecigen/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
@@ -134,32 +134,32 @@
 terraform. Next, the pipeline files. **.circleci/config.yml** Of course you
 must have the regular circleci pipeline file that responds to triggers and
 actually forms the basis of the generated pipeline. Everything in this file up
 through the Jobs: or workflow: directive (whichever comes first) forms the
 starting point for the generated pipeline. **.circleci/pre-approve.yml** This
 file is a template that will be populate with instance specific info when the
 pipeline is generated from within the config.yml pipeline. All values in the
-env_instance.tfvars.json configuration are avaliable to be used in the jinja
+instance_name.tfvars.json configuration are avaliable to be used in the jinja
 template. Keep in mind that the same yaml template is used for each role so it
 will not work to have a value that ONLY exists in a single instance or role if
 the value appears in the yaml template. ```yaml - terraform/plan: name: {
-{env_instance}} change plan context: << pipeline.parameters.context >>
-workspace: {{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json
-before-terraform: - set-environment filters: {{filters}}{
-{priorapprovalrequired}} ``` The indenting is important. This example is using
-the [twdps/terraform orb](https://circleci.com/developer/orbs/orb/twdps/
-terraform). Note that in the before-terraform parameter you can pass any
-pipeline command found in any orb you have included, but more importantly from
-the config.yaml itself. So, for the infra-dev role, circlecigen will create a
-workflow that runs a terraform plan job using the specific, associated
+{instance_name}} change plan context: << pipeline.parameters.context >>
+workspace: {{instance_name}} var-file: {{envpath}}/{
+{instance_name}}.tfvars.json before-terraform: - set-environment filters: {
+{filters}}{{priorapprovalrequired}} ``` The indenting is important. This
+example is using the [twdps/terraform orb](https://circleci.com/developer/orbs/
+orb/twdps/terraform). Note that in the before-terraform parameter you can pass
+any pipeline command found in any orb you have included, but more importantly
+from the config.yaml itself. So, for the infra-dev role, circlecigen will
+create a workflow that runs a terraform plan job using the specific, associated
 _instance_.tfvar.json var-file. Each such instance runs in parallel.
 **.circleci/post-approve.yml** Then specify the job to be run if the above
-plans are approved. ```yaml - terraform/apply: name: apply {{env_instance}}
+plans are approved. ```yaml - terraform/apply: name: apply {{instance_name}}
 change plan context: << pipeline.parameters.context >> workspace: {
-{env_instance}} var-file: {{envpath}}/{{env_instance}}.tfvars.json before-
+{instance_name}} var-file: {{envpath}}/{{instance_name}}.tfvars.json before-
 terraform: - set-environment after-terraform: - after-deployment-commands
 requires: - approve {{role}} changes filters: {{filters}} ``` As you can see,
 this template will run terraform apply, and in addition to running the set-
 environment command before the terraaform plan, it will also run an after-
 deployment-commands after a successful apply. In a real use-case, the after-
 terraform commands are typical integration and functional tests. #### The
 primary config.yml pipeline Below is the basic layout of config.yml where the
@@ -263,29 +263,29 @@
 apply: name: apply nonprod-ap-southwest-1 change plan ... filters: *on-tag-main
 ``` #### 2. Setup example for a job to run nightly integration tests In this
 example we start by setting up the `environments/multi.json` and `environments/
 default.json` as from before. We also set up any relevant role-specific
 overrides, and the CircleCI config file (`.circleci/config.yml`) as from
 before. We then create a custom template file which will be specified with the
 `--template` flag. Let's use the example below: ```yaml - integration-tests:
-name: {{env_instance}} integration test context: << pipeline.parameters.context
->> shell: << pipeline.parameters.shell-options >> executor-image: <<
-pipeline.parameters.executor-image >> instance_name: {{env_instance}}
-workspace: {{env_instance}} filters: {{filters}} ``` The resulting pipeline
-from using the above custom template would then look like the following:
-```yaml --- version: 2.1 orbs: continuation: circleci/continuation@0.3.1 on-
-push-main: &on-push-main branches: only: /main/ tags: ignore: /.*/ commands:
-setup-commands: parameters: ... steps: ... static-code-test-commands:
-parameters: ... steps: ... before-instance-specific-parallel-job-commands:
-parameters: ... steps: ... after-instance-specific-parallel-job-commands:
-parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ... docker: -
-image: ... steps: - setup-commands: parameters: << parameters... >> - static-
-code-test-commands: parameters: << parameters... >> launch-dynamic-pipeline:
-parameters: ... workflows: version: 2 release-pipeline: jobs: - integration-
-tests: name: nonprod-us-west-2 integration test context: <<
+name: {{instance_name}} integration test context: <<
+pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
+executor-image: << pipeline.parameters.executor-image >> instance_name: {
+{instance_name}} workspace: {{instance_name}} filters: {{filters}} ``` The
+resulting pipeline from using the above custom template would then look like
+the following: ```yaml --- version: 2.1 orbs: continuation: circleci/
+continuation@0.3.1 on-push-main: &on-push-main branches: only: /main/ tags:
+ignore: /.*/ commands: setup-commands: parameters: ... steps: ... static-code-
+test-commands: parameters: ... steps: ... before-instance-specific-parallel-
+job-commands: parameters: ... steps: ... after-instance-specific-parallel-job-
+commands: parameters: ... steps: ... jobs: my-pre-deploy-jobs: parameters: ...
+docker: - image: ... steps: - setup-commands: parameters: << parameters... >> -
+static-code-test-commands: parameters: << parameters... >> launch-dynamic-
+pipeline: parameters: ... workflows: version: 2 release-pipeline: jobs: -
+integration-tests: name: nonprod-us-west-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-west-2 workspace: nonprod-us-west-2 filters: *on-push-main -
 integration-tests: name: nonprod-us-east-2 integration test context: <<
 pipeline.parameters.context >> shell: << pipeline.parameters.shell-options >>
 executor-image: << pipeline.parameters.executor-image >> instance_name:
 nonprod-us-east-2 workspace: nonprod-us-east-2 filters: *on-push-main -
```

### Comparing `circlecigen-0.0.8/circlecigen.egg-info/SOURCES.txt` & `circlecigen-0.0.9/circlecigen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/env_test/config.yml` & `circlecigen-0.0.9/env_test/config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/env_test/generated_config.yml` & `circlecigen-0.0.9/env_test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/env_test/multi.json` & `circlecigen-0.0.9/env_test/multi.json`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/env_test/template_generated_config.yml` & `circlecigen-0.0.9/env_test/template_generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/pyproject.toml` & `circlecigen-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/setup.py` & `circlecigen-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/src/circlecigen.py` & `circlecigen-0.0.9/src/circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/src/template.py` & `circlecigen-0.0.9/src/template.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/src/tfvars.py` & `circlecigen-0.0.9/src/tfvars.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             # merge matching instance.json
             if isfile(f"{envpath}/{instance}.json"):
                 instance_vars = merge(instance_vars,read_json_file(envpath, f"{instance}.json"))
             
             # merge any instance overrides in muilti.json into instance dict, intended to overwrite conflicts out of multi.json
             instance_vars = merge(instance_vars, pipeline[role][instance])
 
-            # set the env_instance to the current instance
+            # set the instance_name to the current instance
             instance_vars.update({
-                "env_instance": instance
+                "instance_name": instance
             })
             write_json_file(f"{envpath}/{instance}.tfvars.json", instance_vars)
     return nummber_of_files_to_generate(pipeline)
 
 def nummber_of_files_to_generate(pipeline):
     """calculate the number of total number of instances within the multi-role definition"""
     instance_count = 0
```

### Comparing `circlecigen-0.0.8/src/utils.py` & `circlecigen-0.0.9/src/utils.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/generated_config.yml` & `circlecigen-0.0.9/test/generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/generated_config_setup.yml` & `circlecigen-0.0.9/test/generated_config_setup.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/template_generated_config.yml` & `circlecigen-0.0.9/test/template_generated_config.yml`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/test_circlecigen.py` & `circlecigen-0.0.9/test/test_circlecigen.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/test_template.py` & `circlecigen-0.0.9/test/test_template.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/test_tfvars.py` & `circlecigen-0.0.9/test/test_tfvars.py`

 * *Files identical despite different names*

### Comparing `circlecigen-0.0.8/test/test_utils.py` & `circlecigen-0.0.9/test/test_utils.py`

 * *Files identical despite different names*

