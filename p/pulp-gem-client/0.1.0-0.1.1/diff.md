# Comparing `tmp/pulp_gem-client-0.1.0.tar.gz` & `tmp/pulp_gem-client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp_gem-client-0.1.0.tar", last modified: Mon Jun 26 19:22:08 2023, max compression
+gzip compressed data, was "pulp_gem-client-0.1.1.tar", last modified: Thu Jun 29 19:15:47 2023, max compression
```

## Comparing `pulp_gem-client-0.1.0.tar` & `pulp_gem-client-0.1.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.197263 pulp_gem-client-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 19:22:08.197263 pulp_gem-client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.173263 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-26 19:22:08.000000 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-26 19:22:08.000000 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 19:22:08.000000 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-26 19:22:08.000000 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-26 19:22:08.000000 pulp_gem-client-0.1.0/pulp_gem_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.173263 pulp_gem-client-0.1.0/pulpcore/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.173263 pulp_gem-client-0.1.0/pulpcore/client/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.173263 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.177263 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/content_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    44493 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/distributions_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/publications_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46285 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/remotes_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    59676 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/repositories_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33518 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.185263 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_content.py
--rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_content_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    28909 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)    26296 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29302 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-26 19:22:08.197263 pulp_gem-client-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 19:22:08.197263 pulp_gem-client-0.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_async_operation_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_content_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_content_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_distributions_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_content_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_distribution_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_publication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_publication_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_remote_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_remote_response_hidden_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_gem_gem_repository_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_paginated_repository_version_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_paginatedgem_gem_content_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_paginatedgem_gem_distribution_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_paginatedgem_gem_publication_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-26 19:22:06.000000 pulp_gem-client-0.1.0/test/test_paginatedgem_gem_remote_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_paginatedgem_gem_repository_response_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_patchedgem_gem_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_patchedgem_gem_remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_patchedgem_gem_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_policy_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_publications_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_remotes_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repositories_gem_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repositories_gem_versions_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repository_add_remove_content.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repository_sync_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-26 19:22:07.000000 pulp_gem-client-0.1.0/test/test_repository_version_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.210408 pulp_gem-client-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 19:15:47.214408 pulp_gem-client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.190408 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-29 19:15:46.000000 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-29 19:15:47.000000 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 19:15:46.000000 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-29 19:15:46.000000 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-29 19:15:46.000000 pulp_gem-client-0.1.1/pulp_gem_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.190408 pulp_gem-client-0.1.1/pulpcore/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.190408 pulp_gem-client-0.1.1/pulpcore/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.190408 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.194408 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24743 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/content_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44493 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/distributions_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/publications_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46285 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/remotes_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59676 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/repositories_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33518 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13960 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.202408 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11572 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12513 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28909 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26296 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29302 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7915 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 19:15:47.214408 pulp_gem-client-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 19:15:47.210408 pulp_gem-client-0.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_async_operation_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_content_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_content_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_distributions_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_gem_gem_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_gem_gem_content_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_gem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-29 19:15:44.000000 pulp_gem-client-0.1.1/test/test_gem_gem_distribution_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_publication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_publication_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_remote_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_remote_response_hidden_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_gem_gem_repository_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginated_repository_version_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginatedgem_gem_content_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginatedgem_gem_distribution_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginatedgem_gem_publication_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginatedgem_gem_remote_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_paginatedgem_gem_repository_response_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_patchedgem_gem_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_patchedgem_gem_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_patchedgem_gem_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_policy_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_publications_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_remotes_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repositories_gem_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repositories_gem_versions_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repository_add_remove_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repository_sync_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-29 19:15:45.000000 pulp_gem-client-0.1.1/test/test_repository_version_response.py
```

### Comparing `pulp_gem-client-0.1.0/README.md` & `pulp_gem-client-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pulp_gem-client
 Fetch, Upload, Organize, and Distribute Software Packages
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: v3
-- Package version: 0.1.0
+- Package version: 0.1.1
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pulpproject.org](https://pulpproject.org)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `pulp_gem-client-0.1.0/pulp_gem_client.egg-info/SOURCES.txt` & `pulp_gem-client-0.1.1/pulp_gem_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/__init__.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: pulp-list@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 # import apis into sdk package
 from pulpcore.client.pulp_gem.api.content_gem_api import ContentGemApi
 from pulpcore.client.pulp_gem.api.distributions_gem_api import DistributionsGemApi
 from pulpcore.client.pulp_gem.api.publications_gem_api import PublicationsGemApi
 from pulpcore.client.pulp_gem.api.remotes_gem_api import RemotesGemApi
 from pulpcore.client.pulp_gem.api.repositories_gem_api import RepositoriesGemApi
```

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/__init__.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/content_gem_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/content_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/distributions_gem_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/distributions_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/publications_gem_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/publications_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/remotes_gem_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/remotes_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/repositories_gem_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/repositories_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api/repositories_gem_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/api_client.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.1.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.1.1/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/configuration.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -372,15 +372,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v3\n"\
-               "SDK Package Version: 0.1.0".\
+               "SDK Package Version: 0.1.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/exceptions.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/exceptions.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/__init__.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/async_operation_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/content_summary_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_content.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_content_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_distribution.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_publication.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_repository.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/gem_gem_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/paginatedgem_gem_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/patchedgem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/policy_enum.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repair.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repair.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_add_remove_content.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_sync_url.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/models/repository_version_response.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/models/repository_version_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/pulpcore/client/pulp_gem/rest.py` & `pulp_gem-client-0.1.1/pulpcore/client/pulp_gem/rest.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/setup.py` & `pulp_gem-client-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "pulp_gem-client"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `pulp_gem-client-0.1.0/test/test_async_operation_response.py` & `pulp_gem-client-0.1.1/test/test_async_operation_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_content_gem_api.py` & `pulp_gem-client-0.1.1/test/test_content_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_content_summary_response.py` & `pulp_gem-client-0.1.1/test/test_content_summary_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_distributions_gem_api.py` & `pulp_gem-client-0.1.1/test/test_distributions_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_content.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_content_response.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_content_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_distribution.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_distribution_response.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_distribution_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_publication.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_publication.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_publication_response.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_publication_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_remote.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_remote_response.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_remote_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_remote_response_hidden_fields.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_remote_response_hidden_fields.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_repository.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_gem_gem_repository_response.py` & `pulp_gem-client-0.1.1/test/test_gem_gem_repository_response.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginated_repository_version_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginated_repository_version_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginatedgem_gem_content_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginatedgem_gem_content_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginatedgem_gem_distribution_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginatedgem_gem_distribution_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginatedgem_gem_publication_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginatedgem_gem_publication_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginatedgem_gem_remote_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginatedgem_gem_remote_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_paginatedgem_gem_repository_response_list.py` & `pulp_gem-client-0.1.1/test/test_paginatedgem_gem_repository_response_list.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_patchedgem_gem_distribution.py` & `pulp_gem-client-0.1.1/test/test_patchedgem_gem_distribution.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_patchedgem_gem_remote.py` & `pulp_gem-client-0.1.1/test/test_patchedgem_gem_remote.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_patchedgem_gem_repository.py` & `pulp_gem-client-0.1.1/test/test_patchedgem_gem_repository.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_policy_enum.py` & `pulp_gem-client-0.1.1/test/test_policy_enum.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_publications_gem_api.py` & `pulp_gem-client-0.1.1/test/test_publications_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_remotes_gem_api.py` & `pulp_gem-client-0.1.1/test/test_remotes_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repair.py` & `pulp_gem-client-0.1.1/test/test_repair.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repositories_gem_api.py` & `pulp_gem-client-0.1.1/test/test_repositories_gem_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repositories_gem_versions_api.py` & `pulp_gem-client-0.1.1/test/test_repositories_gem_versions_api.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repository_add_remove_content.py` & `pulp_gem-client-0.1.1/test/test_repository_add_remove_content.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repository_sync_url.py` & `pulp_gem-client-0.1.1/test/test_repository_sync_url.py`

 * *Files identical despite different names*

### Comparing `pulp_gem-client-0.1.0/test/test_repository_version_response.py` & `pulp_gem-client-0.1.1/test/test_repository_version_response.py`

 * *Files identical despite different names*

