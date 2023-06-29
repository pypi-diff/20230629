# Comparing `tmp/prismacloud-cli-0.6.8.tar.gz` & `tmp/prismacloud-cli-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prismacloud-cli-0.6.8.tar", last modified: Thu Feb  2 12:26:32 2023, max compression
+gzip compressed data, was "prismacloud-cli-0.6.9.tar", last modified: Fri Feb  3 14:55:06 2023, max compression
```

## Comparing `prismacloud-cli-0.6.8.tar` & `prismacloud-cli-0.6.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.720685 prismacloud-cli-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-02 12:26:32.720685 prismacloud-cli-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.712685 prismacloud-cli-0.6.8/prismacloud/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.712685 prismacloud-cli-0.6.8/prismacloud/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.716685 prismacloud-cli-0.6.8/prismacloud/cli/cspm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_pov.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_rql.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_saas_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_usage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.716685 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_audits.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_defenders.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_hosts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_intelligence.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_scans.py
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_users.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.720685 prismacloud-cli-0.6.8/prismacloud/cli/pccs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/pccs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/pccs/cmd_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/pccs/cmd_reviews.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/pccs/cmd_suppressions.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/prismacloud/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-02 12:26:32.720685 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-02 12:26:32.000000 prismacloud-cli-0.6.8/prismacloud_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-02 12:26:32.720685 prismacloud-cli-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-02 12:25:46.000000 prismacloud-cli-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.565876 prismacloud-cli-0.6.9/prismacloud/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.565876 prismacloud-cli-0.6.9/prismacloud/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    17828 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.569876 prismacloud-cli-0.6.9/prismacloud/cli/cspm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_pov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_rql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_saas_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_usage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_audits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_defenders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_host_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_intelligence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_scans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/prismacloud/cli/pccs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/pccs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12806 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/pccs/cmd_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/pccs/cmd_reviews.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/pccs/cmd_suppressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/prismacloud/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-03 14:55:06.000000 prismacloud-cli-0.6.9/prismacloud_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-02-03 14:55:06.573876 prismacloud-cli-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-02-03 14:54:21.000000 prismacloud-cli-0.6.9/setup.py
```

### Comparing `prismacloud-cli-0.6.8/LICENSE` & `prismacloud-cli-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/PKG-INFO` & `prismacloud-cli-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud-cli-0.6.8/README.md` & `prismacloud-cli-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/__init__.py` & `prismacloud-cli-0.6.9/prismacloud/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/api.py` & `prismacloud-cli-0.6.9/prismacloud/cli/api.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_alert.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_alert.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_cloud.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_cloud.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_compliance.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_compliance.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_licenses.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_licenses.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_policy.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_policy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_pov.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_pov.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_rql.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_rql.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,24 @@
     search_params = {}
     search_params["limit"] = 10000
     search_params["timeRange"] = {}
     search_params["timeRange"]["type"] = "relative"
     search_params["timeRange"]["value"] = {}
     search_params["timeRange"]["value"]["unit"] = unit
     search_params["timeRange"]["value"]["amount"] = amount
+
     search_params["withResourceJson"] = False
     search_params["query"] = query
 
     logging.debug("API - Getting the RQL results ...")
-    if query.startswith("config from"):
+    if query.startswith("config from iam"):
+        search_params["searchType"] = "iam"
+        search_params["timeRange"] = {"type": "to_now", "value": "epoch"}  # Latest results
+        result_list = pc_api.search_iam_read(search_params=search_params)
+    elif query.startswith("config from"):
         result_list = pc_api.search_config_read(search_params=search_params)
     elif query.startswith("network from"):
         result_list = pc_api.search_network_read(search_params=search_params)
     elif query.startswith("event from"):
         result_list = pc_api.search_event_read(search_params=search_params)
     else:
         logging.error("Unknown RQL query type (limited to: config|network|event).")
```

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cspm/cmd_saas_version.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cspm/cmd_saas_version.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_audits.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_audits.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_containers.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_containers.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_defenders.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_defenders.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_host_auto_deploy.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_host_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_hosts.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_hosts.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_images.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_images.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_logs.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_logs.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_monitor.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_monitor.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_policies.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_policies.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_registry.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_registry.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_scans.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_scans.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_serverless_auto_deploy.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/cwpp/cmd_stats.py` & `prismacloud-cli-0.6.9/prismacloud/cli/cwpp/cmd_stats.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/pccs/cmd_repositories.py` & `prismacloud-cli-0.6.9/prismacloud/cli/pccs/cmd_repositories.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud/cli/pccs/cmd_suppressions.py` & `prismacloud-cli-0.6.9/prismacloud/cli/pccs/cmd_suppressions.py`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/prismacloud_cli.egg-info/PKG-INFO` & `prismacloud-cli-0.6.9/prismacloud_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prismacloud-cli
-Version: 0.6.8
+Version: 0.6.9
 Summary: Prisma Cloud CLI
 Home-page: https://github.com/PaloAltoNetworks/prismacloud-cli
 Author: Steven de Boer, Simon Melotte, Tom Kishel
 Author-email: stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com
 License: BSD
 Keywords: prisma cloud cli
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `prismacloud-cli-0.6.8/prismacloud_cli.egg-info/SOURCES.txt` & `prismacloud-cli-0.6.9/prismacloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prismacloud-cli-0.6.8/setup.py` & `prismacloud-cli-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "pandas",
         "requests",
         "tabulate",
         "colorama",
         "update_checker",
         "pydantic",
         "datetime",
-        "prismacloud-api==5.1.4",
+        "prismacloud-api==5.1.5",
     ],
     name="prismacloud-cli",
     version=version,
     python_requires=">=3.7",
     author="Steven de Boer, Simon Melotte, Tom Kishel",
     author_email="stdeboer@paloaltonetworks.com, smelotte@paloaltonetworks.com, tkishel@paloaltonetworks.com",
     description=("Prisma Cloud CLI"),
```

