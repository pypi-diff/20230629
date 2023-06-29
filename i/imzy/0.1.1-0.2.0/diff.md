# Comparing `tmp/imzy-0.1.1.tar.gz` & `tmp/imzy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imzy-0.1.1.tar", last modified: Thu Apr 13 17:43:59 2023, max compression
+gzip compressed data, was "imzy-0.2.0.tar", last modified: Thu Jun 29 16:59:22 2023, max compression
```

## Comparing `imzy-0.1.1.tar` & `imzy-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/.stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/workflows/greetings.yml
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-13 17:43:44.000000 imzy-0.1.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-13 17:43:44.000000 imzy-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-13 17:43:44.000000 imzy-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-13 17:43:44.000000 imzy-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-13 17:43:44.000000 imzy-0.1.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-13 17:43:59.482109 imzy-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-13 17:43:44.000000 imzy-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-13 17:43:44.000000 imzy-0.1.1/misc/test-comprehensive.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-13 17:43:44.000000 imzy-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 17:43:59.482109 imzy-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.478109 imzy-0.1.1/src/imzy/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/src/imzy/_centroids/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_centroids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_centroids/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_centroids/_hdf5_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_centroids/_memory_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_centroids/_zarr_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/src/imzy/_readers/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/src/imzy/_readers/imzml/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/_ims.py
--rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/_imzml.py
--rw-r--r--   0 runner    (1001) docker     (123)   174872 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/_ms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/_ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/_readers/imzml/_uo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-04-13 17:43:44.000000 imzy-0.1.1/src/imzy/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/src/imzy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-13 17:43:59.000000 imzy-0.1.1/src/imzy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-13 17:43:59.000000 imzy-0.1.1/src/imzy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:43:59.000000 imzy-0.1.1/src/imzy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-13 17:43:59.000000 imzy-0.1.1/src/imzy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-13 17:43:59.000000 imzy-0.1.1/src/imzy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:59.482109 imzy-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 17:43:44.000000 imzy-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-04-13 17:43:44.000000 imzy-0.1.1/tests/test_imzml.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-13 17:43:44.000000 imzy-0.1.1/tests/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-13 17:43:44.000000 imzy-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.424059 imzy-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.388059 imzy-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/.stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.388059 imzy-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.388059 imzy-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/workflows/greetings.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-29 16:59:07.000000 imzy-0.2.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 16:59:07.000000 imzy-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-29 16:59:07.000000 imzy-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-29 16:59:07.000000 imzy-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-29 16:59:07.000000 imzy-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-29 16:59:22.424059 imzy-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-29 16:59:07.000000 imzy-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.388059 imzy-0.2.0/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-29 16:59:07.000000 imzy-0.2.0/misc/test-comprehensive.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-29 16:59:07.000000 imzy-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 16:59:22.424059 imzy-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.380059 imzy-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.388059 imzy-0.2.0/src/imzy/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.392059 imzy-0.2.0/src/imzy/_centroids/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_centroids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_centroids/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_centroids/_hdf5_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_centroids/_memory_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_centroids/_zarr_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10105 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.392059 imzy-0.2.0/src/imzy/_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.408059 imzy-0.2.0/src/imzy/_readers/bruker/
+-rw-r--r--   0 runner    (1001) docker     (123)    41725 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/THIRD-PARTY-LICENSE-README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/_tdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/_tsf.py
+-rw-r--r--   0 runner    (1001) docker     (123) 13529648 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/libtimsdata.so
+-rw-r--r--   0 runner    (1001) docker     (123)  2861288 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/timsdata.dll
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/bruker/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.412059 imzy-0.2.0/src/imzy/_readers/imzml/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9884 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/_ims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19999 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/_imzml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   174872 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/_ms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/_ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17326 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/_readers/imzml/_uo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-06-29 16:59:07.000000 imzy-0.2.0/src/imzy/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.392059 imzy-0.2.0/src/imzy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5250 2023-06-29 16:59:22.000000 imzy-0.2.0/src/imzy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-29 16:59:22.000000 imzy-0.2.0/src/imzy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 16:59:22.000000 imzy-0.2.0/src/imzy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-29 16:59:22.000000 imzy-0.2.0/src/imzy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-29 16:59:22.000000 imzy-0.2.0/src/imzy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.412059 imzy-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.384059 imzy-0.2.0/tests/_test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.416059 imzy-0.2.0/tests/_test_data/example_tsf.d/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.420059 imzy-0.2.0/tests/_test_data/example_tsf.d/.icache/
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/.icache/frame_index_cache.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/ProjectCreationHelper
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/Storage.mcf_idx
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/SyncHelper
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/analysis.0.DataAnalysis.method
+-rw-r--r--   0 runner    (1001) docker     (123)    43957 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/analysis.0.result_c
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/analysis.content
+-rw-r--r--   0 runner    (1001) docker     (123)  1376256 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/analysis.tsf
+-rw-r--r--   0 runner    (1001) docker     (123)  3268608 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/analysis.tsf_bin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:22.424059 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/InstrumentSetup.isset
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/Maldi.method
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/diaSettings.diasqlite
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/lock.file
+-rw-r--r--   0 runner    (1001) docker     (123)   193471 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/microTOFQImpacTemAcquisition.method
+-rw-r--r--   0 runner    (1001) docker     (123)    45056 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/prmSettings.prmsqlite
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/_test_data/example_tsf.d/example_tsf.m/submethods.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/test_imzml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/test_tdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/test_tsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-29 16:59:07.000000 imzy-0.2.0/tests/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-29 16:59:07.000000 imzy-0.2.0/tox.ini
```

### Comparing `imzy-0.1.1/.github/.stale.yml` & `imzy-0.2.0/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/.github/dependabot.yml` & `imzy-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/.github/release-drafter.yml` & `imzy-0.2.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/.github/workflows/ci.yml` & `imzy-0.2.0/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       # if running a cron job, we add the --pre flag to test against pre-releases
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install .[test,zarr,hdf5] ${{ github.event_name == 'schedule' && '--pre' || ''  }}
 
       - name: Test
-        run: pytest --color=yes --cov --cov-report=xml --cov-report=term-missing
+        run: pytest --color=yes --cov=imzy --cov-report=xml --cov-report=term-missing
 
       # If something goes wrong, we can open an issue in the repo
       - name: Report --pre Failures
         if: failure() && github.event_name == 'schedule'
         uses: JasonEtco/create-an-issue@v2
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
@@ -90,15 +90,15 @@
           twine check dist/*
           ls -lh dist
 
       - name: Build and publish
         run: twine upload --repository testpypi dist/*
         env:
           TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.TEST_PYPI_ALL_TOKEN }}
+          TWINE_PASSWORD: ${{ secrets.TEST_PYPI_TOKEN }}
 
       - uses: softprops/action-gh-release@v1
         with:
           generate_release_notes: true
 
   deploy:
     name: Deploy
@@ -122,12 +122,12 @@
           twine check dist/*
           ls -lh dist
 
       - name: Build and publish
         run: twine upload dist/*
         env:
           TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_ALL_TOKEN }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
 
       - uses: softprops/action-gh-release@v1
         with:
           generate_release_notes: true
```

### Comparing `imzy-0.1.1/.github/workflows/greetings.yml` & `imzy-0.2.0/.github/workflows/greetings.yml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/.pre-commit-config.yaml` & `imzy-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/LICENSE` & `imzy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/MANIFEST.in` & `imzy-0.2.0/MANIFEST.in`

 * *Files 20% similar despite different names*

```diff
@@ -21,7 +21,10 @@
 recursive-include imzy *.pyi
 include MANIFEST.in
 include setup.cfg
 
 # Always include
 global-include *.pyx
 global-include *.c
+global-include src *.dll
+global-include src *.so
+global-include src *.txt
```

### Comparing `imzy-0.1.1/Makefile` & `imzy-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/misc/test-comprehensive.yml` & `imzy-0.2.0/misc/test-comprehensive.yml`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/pyproject.toml` & `imzy-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
   "koyo"
 ]
 
 # extras
 # https://peps.python.org/pep-0621/#dependencies-optional-dependencies
 [project.optional-dependencies]
 test = [
-    "pytest>=6.0",
+    "pytest>=7.0",
     "pytest-cov",
 ]
 dev = [
     "black==22.1.0",
     "ipython",
     "mypy",
     "pdbpp",
@@ -138,14 +138,15 @@
 "tests/*.py" = ["D", "S"]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = ["tests"]
 filterwarnings = ["error"]
+addopts = "--maxfail 5 --durations=10 -rXxs"
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
 [tool.mypy]
 files = "src/**/"
 strict = true
 disallow_any_generics = false
 disallow_subclassing_any = false
@@ -188,14 +189,17 @@
   "setup.py",
   "tests/**/*",
   "**/*_version.py",
   "Makefile",
   "tox.ini",
   "misc/*.yml"
 ]
+ignore-bad-ideas = [
+    "src/imzy/**/*.so",
+]
 
 # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 [tool.semantic_release]
 version_source = "tag_only"
 branch = "main"
 changelog_sections = "feature,fix,breaking,documentation,performance,chore,:boom:,:sparkles:,:children_crossing:,:lipstick:,:iphone:,:egg:,:chart_with_upwards_trend:,:ambulance:,:lock:,:bug:,:zap:,:goal_net:,:alien:,:wheelchair:,:speech_balloon:,:mag:,:apple:,:penguin:,:checkered_flag:,:robot:,:green_apple:,Other"
 # commit_parser=semantic_release.history.angular_parser
```

### Comparing `imzy-0.1.1/src/imzy/__init__.py` & `imzy-0.2.0/src/imzy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # type: ignore[attr-defined]
 """imzy: A new reader/writer interface to imzML and other imaging mass spectrometry formats."""
 
 
 from importlib import metadata as importlib_metadata
 
 from imzy._centroids import H5CentroidsStore, InMemoryStore, ZarrCentroidsStore
-from imzy._readers import IMZMLReader, get_reader
+from imzy._readers import IMZMLReader, TDFReader, TSFReader, get_reader
 
 
 def get_version() -> str:
     """Get version."""
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
         return "unknown"
 
 
 __version__: str = get_version()
-__all__ = ("IMZMLReader", "get_reader", "H5CentroidsStore", "ZarrCentroidsStore", "InMemoryStore")
+__all__ = (
+    "IMZMLReader",
+    "TDFReader",
+    "TSFReader",
+    "get_reader",
+    "H5CentroidsStore",
+    "ZarrCentroidsStore",
+    "InMemoryStore",
+)
```

### Comparing `imzy-0.1.1/src/imzy/_centroids/_base.py` & `imzy-0.2.0/src/imzy/_centroids/_base.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_centroids/_hdf5_store.py` & `imzy-0.2.0/src/imzy/_centroids/_hdf5_store.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_centroids/_memory_store.py` & `imzy-0.2.0/src/imzy/_centroids/_memory_store.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_centroids/_zarr_store.py` & `imzy-0.2.0/src/imzy/_centroids/_zarr_store.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_extract.py` & `imzy-0.2.0/src/imzy/_extract.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_readers/_base.py` & `imzy-0.2.0/src/imzy/_readers/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,55 @@
     _xyz_coordinates: ty.Optional[np.ndarray] = None
     _tic: ty.Optional[np.ndarray] = None
     _current = -1
 
     def __init__(self, path: PathLike):
         self.path = Path(path)
 
+    def _init(self):
+        """Method which is called to initialize the reader."""
+        raise NotImplementedError("Must implement method")
+
+    @property
+    def mz_min(self) -> float:
+        """Minimum m/z value."""
+        raise NotImplementedError("Must implement method")
+
+    @property
+    def mz_max(self) -> float:
+        """Maximum m/z value."""
+        raise NotImplementedError("Must implement method")
+
+    @property
+    def is_centroid(self) -> bool:
+        """Flag to indicate whether the data is in centroid or profile mode."""
+        raise NotImplementedError("Must implement method")
+
+    def get_spectrum(self, index: int):
+        """Return mass spectrum."""
+        return self._read_spectrum(index)
+
+    def get_summed_spectrum(self, indices: ty.Iterable[int], silent: bool = False):
+        """Sum pixel data to produce summed mass spectrum."""
+        raise NotImplementedError("Must implement method")
+
+    def _read_spectrum(self, index: int) -> ty.Tuple[np.ndarray, np.ndarray]:
+        raise NotImplementedError("Must implement method")
+
+    def _read_spectra(self, indices: ty.Optional[np.ndarray] = None) -> ty.Iterator[ty.Tuple[np.ndarray, np.ndarray]]:
+        raise NotImplementedError("Must implement method")
+
+    def reshape(self, array: np.ndarray, fill_value: float = 0) -> np.ndarray:
+        """Reshape vector into an image."""
+        raise NotImplementedError("Must implement method")
+
+    def reshape_batch(self, array: np.ndarray, fill_value: float = 0) -> np.ndarray:
+        """Reshape multiple vectors into a stack of images."""
+        raise NotImplementedError("Must implement method")
+
     def __iter__(self):
         return self
 
     def __next__(self):
         """Get next spectrum."""
         if self._current < self.n_pixels - 1:
             self._current += 1
@@ -33,28 +74,14 @@
             self._current = -1
             raise StopIteration
 
     def __getitem__(self, item: int):
         """Retrieve spectrum."""
         return self.get_spectrum(item)
 
-    def _init(self):
-        """Method which is called to initialize the reader."""
-        raise NotImplementedError("Must implement method")
-
-    @property
-    def mz_min(self) -> float:
-        """Minimum m/z value."""
-        raise NotImplementedError("Must implement method")
-
-    @property
-    def mz_max(self) -> float:
-        """Maximum m/z value."""
-        raise NotImplementedError("Must implement method")
-
     @property
     def xyz_coordinates(self) -> np.ndarray:
         """Return xyz coordinates."""
         return self._xyz_coordinates
 
     @property
     def x_coordinates(self) -> np.ndarray:
@@ -77,41 +104,27 @@
         return np.arange(self.n_pixels)
 
     @property
     def n_pixels(self):
         """Return the total number of pixels in the dataset."""
         return len(self.x_coordinates)
 
-    @property
-    def is_centroid(self) -> bool:
-        """Flag to indicate whether the data is in centroid or profile mode."""
-        raise NotImplementedError("Must implement method")
-
-    def get_spectrum(self, index: int):
-        """Return mass spectrum."""
-        return self._read_spectrum(index)
-
-    def get_summed_spectrum(self, indices: ty.Iterable[int], silent: bool = False):
-        """Sum pixel data to produce summed mass spectrum."""
-        raise NotImplementedError("Must implement method")
-
-    def _read_spectrum(self, index: int) -> ty.Tuple[np.ndarray, np.ndarray]:
-        raise NotImplementedError("Must implement method")
-
-    def _read_spectra(self, indices: ty.Optional[np.ndarray] = None) -> ty.Iterator[ty.Tuple[np.ndarray, np.ndarray]]:
-        raise NotImplementedError("Must implement method")
-
     def get_chromatogram(self, indices: ty.Iterable[int]):
         """Return chromatogram."""
+        indices = np.asarray(indices)
+        array = np.zeros(len(indices), dtype=np.float32)
+        for y in self.spectra_iter(indices):
+            array += np.sum(y)
+        return array
 
     def get_tic(self, silent: bool = False) -> np.ndarray:
         """Return TIC image."""
         if self._tic is None:
             res = np.zeros(self.n_pixels)
-            for i, (_, y) in enumerate(self.iter_spectra(silent)):
+            for i, (_, y) in enumerate(self.spectra_iter(silent=silent)):
                 res[i] = y.sum()
             self._tic = res
         return self._tic
 
     def get_ion_image(
         self, mz: float, tol: float = None, ppm: float = None, fill_value: float = np.nan, silent: bool = False
     ) -> np.ndarray:
@@ -120,21 +133,21 @@
             raise ValueError("Please specify `tol` or `ppm`.")
         elif tol is not None and ppm is not None:
             raise ValueError("Please only specify `tol` or `ppm`.")
         func = find_between_tol if tol else find_between_ppm
         val = tol if tol else ppm
         res = np.full(self.n_pixels, dtype=np.float32, fill_value=fill_value)
         if self.is_centroid:
-            for i, (x, y) in enumerate(self.iter_spectra(silent)):
+            for i, (x, y) in enumerate(self.spectra_iter(silent=silent)):
                 mask = func(x, mz, val)
                 res[i] = y[mask].sum()
         else:
             x, _ = self[0]
             mask = func(x, mz, val)
-            for i, (_, y) in enumerate(self.iter_spectra(silent)):
+            for i, (_, y) in enumerate(self.spectra_iter(silent=silent)):
                 res[i] = y[mask].sum()
         return self.reshape(res)
 
     def _get_ions(
         self,
         mzs: ty.Iterable[float],
         tol: float = None,
@@ -143,20 +156,20 @@
         silent: bool = False,
     ):
         mzs = np.asarray(mzs)
         mzs_min, mzs_max = get_mzs_for_tol(mzs, tol, ppm)
         res = np.full((self.n_pixels, len(mzs)), dtype=np.float32, fill_value=fill_value)
 
         if self.is_centroid:
-            for i, (x, y) in enumerate(self.iter_spectra(silent)):
+            for i, (x, y) in enumerate(self.spectra_iter(silent=silent)):
                 res[i] = accumulate_peaks_centroid(mzs_min, mzs_max, x, y)
         else:
             x, _ = self.get_spectrum(0)
             indices = find_between_batch(x, mzs_min, mzs_max)
-            for i, (_, y) in enumerate(self.iter_spectra(silent)):
+            for i, (_, y) in enumerate(self.spectra_iter(silent=silent)):
                 res[i] = accumulate_peaks_profile(indices, y)
         return res
 
     def get_ion_images(
         self,
         mzs: ty.Iterable[float],
         tol: float = None,
@@ -286,20 +299,13 @@
             mzs_min=mzs_min,
             mzs_max=mzs_max,
             indices=self.pixels,
             silent=silent,
         )
         return hdf_path
 
-    def reshape(self, array: np.ndarray, fill_value: float = 0) -> np.ndarray:
-        """Reshape vector into an image."""
-        raise NotImplementedError("Must implement method")
-
-    def reshape_batch(self, array: np.ndarray, fill_value: float = 0) -> np.ndarray:
-        """Reshape multiple vectors into a stack of images."""
-        raise NotImplementedError("Must implement method")
-
-    def iter_spectra(self, silent: bool = False):
+    def spectra_iter(self, indices: ty.Optional[ty.Iterable[int]] = None, silent: bool = False):
         """Yield spectra."""
+        indices = self.pixels if indices is None else np.asarray(indices)
         yield from tqdm(
-            self._read_spectra(), total=self.n_pixels, disable=silent, miniters=500, desc="Iterating spectra..."
+            self._read_spectra(indices), total=len(indices), disable=silent, miniters=500, desc="Iterating spectra..."
         )
```

### Comparing `imzy-0.1.1/src/imzy/_readers/imzml/_ims.py` & `imzy-0.2.0/src/imzy/_readers/imzml/_ims.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_readers/imzml/_imzml.py` & `imzy-0.2.0/src/imzy/_readers/imzml/_imzml.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_readers/imzml/_ms.py` & `imzy-0.2.0/src/imzy/_readers/imzml/_ms.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_readers/imzml/_ontology.py` & `imzy-0.2.0/src/imzy/_readers/imzml/_ontology.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/_readers/imzml/_uo.py` & `imzy-0.2.0/src/imzy/_readers/imzml/_uo.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/src/imzy/utilities.py` & `imzy-0.2.0/src/imzy/utilities.py`

 * *Files identical despite different names*

### Comparing `imzy-0.1.1/tests/test_imzml.py` & `imzy-0.2.0/tests/test_imzml.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     assert images.ndim == 3
     assert len(images) == 2
 
     images = reader.get_ion_images([500, 600], ppm=3)
     assert images.ndim == 3
     assert len(images) == 2
 
-    for x, y in reader.iter_spectra():
+    for x, y in reader.spectra_iter():
         assert x.shape == y.shape
 
     # get summed spectrum
     mz_min, mz_max = reader._estimate_mass_range()
     assert mz_min != mz_max
     mz_x, mz_y = reader.get_summed_spectrum(reader.pixels)
     assert mz_x.shape == mz_y.shape
```

### Comparing `imzy-0.1.1/tox.ini` & `imzy-0.2.0/tox.ini`

 * *Files identical despite different names*

