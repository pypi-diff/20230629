# Comparing `tmp/pdm_utils-1.1.1.tar.gz` & `tmp/pdm_utils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/labad/git_repos/pdm_utils/dist/.tmp-myuksz7d/pdm_utils-1.1.1.tar", last modified: Tue Jun 27 23:53:05 2023, max compression
+gzip compressed data, was "/Users/labad/git_repos/pdm_utils/dist/.tmp-739l0s8f/pdm_utils-1.1.2.tar", last modified: Thu Jun 29 20:36:18 2023, max compression
```

## Comparing `pdm_utils-1.1.1.tar` & `pdm_utils-1.1.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.876086 pdm_utils-1.1.1/
--rw-r--r--   0 labad      (502) staff       (20)    35186 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/LICENSE
--rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-27 23:53:05.876290 pdm_utils-1.1.1/PKG-INFO
--rw-r--r--   0 labad      (502) staff       (20)      790 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/README.md
--rw-r--r--   0 labad      (502) staff       (20)       89 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/pyproject.toml
--rw-r--r--   0 labad      (502) staff       (20)     1507 2023-06-27 23:53:05.877116 pdm_utils-1.1.1/setup.cfg
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.813297 pdm_utils-1.1.1/src/
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.817928 pdm_utils-1.1.1/src/pdm_utils/
--rw-r--r--   0 labad      (502) staff       (20)      146 2023-06-27 23:21:45.000000 pdm_utils-1.1.1/src/pdm_utils/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)      114 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/__main__.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.835695 pdm_utils-1.1.1/src/pdm_utils/classes/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)    20060 2020-10-30 13:34:57.000000 pdm_utils-1.1.1/src/pdm_utils/classes/alchemyhandler.py
--rw-r--r--   0 labad      (502) staff       (20)     8100 2021-09-17 01:24:47.000000 pdm_utils-1.1.1/src/pdm_utils/classes/aragornhandler.py
--rw-r--r--   0 labad      (502) staff       (20)    10410 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/bundle.py
--rw-r--r--   0 labad      (502) staff       (20)    39957 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/cds.py
--rw-r--r--   0 labad      (502) staff       (20)     2461 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/cdspair.py
--rw-r--r--   0 labad      (502) staff       (20)     9923 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/dbcomparesummary.py
--rw-r--r--   0 labad      (502) staff       (20)      165 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/classes/error.py
--rw-r--r--   0 labad      (502) staff       (20)      696 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/evaluation.py
--rw-r--r--   0 labad      (502) staff       (20)     7966 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/fileio.py
--rw-r--r--   0 labad      (502) staff       (20)    23716 2021-09-17 01:24:47.000000 pdm_utils-1.1.1/src/pdm_utils/classes/filter.py
--rw-r--r--   0 labad      (502) staff       (20)    41595 2021-09-22 16:59:23.000000 pdm_utils-1.1.1/src/pdm_utils/classes/genome.py
--rw-r--r--   0 labad      (502) staff       (20)     5574 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/genomepair.py
--rw-r--r--   0 labad      (502) staff       (20)    18395 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/genometriad.py
--rw-r--r--   0 labad      (502) staff       (20)     1124 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/classes/progress.py
--rw-r--r--   0 labad      (502) staff       (20)     7244 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/randomfieldupdatehandler.py
--rw-r--r--   0 labad      (502) staff       (20)     4243 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/source.py
--rw-r--r--   0 labad      (502) staff       (20)     8694 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/ticket.py
--rw-r--r--   0 labad      (502) staff       (20)    37793 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/tmrna.py
--rw-r--r--   0 labad      (502) staff       (20)    64069 2021-09-22 15:49:23.000000 pdm_utils-1.1.1/src/pdm_utils/classes/trna.py
--rw-r--r--   0 labad      (502) staff       (20)     3694 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/classes/trnascansehandler.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.839451 pdm_utils-1.1.1/src/pdm_utils/constants/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/constants/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)     6185 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/constants/constants.py
--rw-r--r--   0 labad      (502) staff       (20)    10763 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/constants/db_schema_0.py
--rw-r--r--   0 labad      (502) staff       (20)    12305 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/constants/eval_descriptions.py
--rw-r--r--   0 labad      (502) staff       (20)    37168 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/constants/schema_conversions.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.857196 pdm_utils-1.1.1/src/pdm_utils/functions/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)     6113 2020-10-30 13:34:57.000000 pdm_utils-1.1.1/src/pdm_utils/functions/annotation.py
--rw-r--r--   0 labad      (502) staff       (20)    45918 2021-01-04 16:11:55.000000 pdm_utils-1.1.1/src/pdm_utils/functions/basic.py
--rw-r--r--   0 labad      (502) staff       (20)     2962 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/cartography.py
--rw-r--r--   0 labad      (502) staff       (20)     2182 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/configfile.py
--rw-r--r--   0 labad      (502) staff       (20)     2853 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/functions/deeptmhmm.py
--rw-r--r--   0 labad      (502) staff       (20)     4638 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/eval_modes.py
--rw-r--r--   0 labad      (502) staff       (20)     2301 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/fasta.py
--rw-r--r--   0 labad      (502) staff       (20)    10526 2021-03-23 03:57:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/fileio.py
--rw-r--r--   0 labad      (502) staff       (20)    30706 2021-09-22 16:59:23.000000 pdm_utils-1.1.1/src/pdm_utils/functions/flat_files.py
--rw-r--r--   0 labad      (502) staff       (20)     2858 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/multiprocess.py
--rw-r--r--   0 labad      (502) staff       (20)     5299 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/multithread.py
--rw-r--r--   0 labad      (502) staff       (20)    27400 2022-10-18 17:47:46.000000 pdm_utils-1.1.1/src/pdm_utils/functions/mysqldb.py
--rw-r--r--   0 labad      (502) staff       (20)    13414 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/mysqldb_basic.py
--rw-r--r--   0 labad      (502) staff       (20)     6605 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/ncbi.py
--rw-r--r--   0 labad      (502) staff       (20)    10972 2020-12-29 20:15:44.000000 pdm_utils-1.1.1/src/pdm_utils/functions/parsing.py
--rw-r--r--   0 labad      (502) staff       (20)    12611 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/phagesdb.py
--rw-r--r--   0 labad      (502) staff       (20)     8600 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/pham_alignment.py
--rw-r--r--   0 labad      (502) staff       (20)     9900 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/phameration.py
--rw-r--r--   0 labad      (502) staff       (20)     8473 2021-01-04 16:11:55.000000 pdm_utils-1.1.1/src/pdm_utils/functions/pipeline_shells.py
--rw-r--r--   0 labad      (502) staff       (20)     8828 2020-12-28 19:11:26.000000 pdm_utils-1.1.1/src/pdm_utils/functions/pipelines_basic.py
--rw-r--r--   0 labad      (502) staff       (20)    30269 2021-09-17 01:24:47.000000 pdm_utils-1.1.1/src/pdm_utils/functions/querying.py
--rw-r--r--   0 labad      (502) staff       (20)     6325 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/rpsblast.py
--rw-r--r--   0 labad      (502) staff       (20)     3475 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/server.py
--rw-r--r--   0 labad      (502) staff       (20)      978 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/functions/subprocess.py
--rw-r--r--   0 labad      (502) staff       (20)    11826 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/functions/tickets.py
--rw-r--r--   0 labad      (502) staff       (20)    15996 2021-01-04 16:11:55.000000 pdm_utils-1.1.1/src/pdm_utils/functions/url_basic.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.873569 pdm_utils-1.1.1/src/pdm_utils/pipelines/
--rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/__init__.py
--rw-r--r--   0 labad      (502) staff       (20)    27107 2023-06-27 23:12:34.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/cluster_db.py
--rwxr-xr-x   0 labad      (502) staff       (20)    60772 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/compare_db.py
--rw-r--r--   0 labad      (502) staff       (20)     8327 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/convert_db.py
--rw-r--r--   0 labad      (502) staff       (20)    33685 2021-09-22 16:59:23.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/export_db.py
--rw-r--r--   0 labad      (502) staff       (20)    17337 2023-06-27 23:13:56.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/find_domains.py
--rw-r--r--   0 labad      (502) staff       (20)      972 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/find_membrane.py
--rw-r--r--   0 labad      (502) staff       (20)    14635 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/find_transmembrane.py
--rwxr-xr-x   0 labad      (502) staff       (20)     7930 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/freeze_db.py
--rw-r--r--   0 labad      (502) staff       (20)    37362 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/get_data.py
--rw-r--r--   0 labad      (502) staff       (20)    16273 2021-01-05 20:20:36.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/get_db.py
--rw-r--r--   0 labad      (502) staff       (20)    10665 2020-10-30 13:34:57.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/get_gb_records.py
--rw-r--r--   0 labad      (502) staff       (20)    91016 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/import_genome.py
--rw-r--r--   0 labad      (502) staff       (20)    12771 2021-09-17 01:23:58.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/pham_finder.py
--rw-r--r--   0 labad      (502) staff       (20)    25213 2020-10-30 13:34:57.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/pham_review.py
--rw-r--r--   0 labad      (502) staff       (20)    10125 2023-06-18 16:32:34.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/phamerate.py
--rw-r--r--   0 labad      (502) staff       (20)     7937 2020-12-13 18:52:56.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/push_db.py
--rw-r--r--   0 labad      (502) staff       (20)    36843 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/revise.py
--rw-r--r--   0 labad      (502) staff       (20)     5642 2023-06-15 19:40:19.000000 pdm_utils-1.1.1/src/pdm_utils/pipelines/update_field.py
--rw-r--r--   0 labad      (502) staff       (20)     3630 2023-06-27 20:56:00.000000 pdm_utils-1.1.1/src/pdm_utils/run.py
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.820184 pdm_utils-1.1.1/src/pdm_utils.egg-info/
--rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/PKG-INFO
--rw-r--r--   0 labad      (502) staff       (20)     3061 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/SOURCES.txt
--rw-r--r--   0 labad      (502) staff       (20)        1 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/dependency_links.txt
--rw-r--r--   0 labad      (502) staff       (20)       54 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/entry_points.txt
--rw-r--r--   0 labad      (502) staff       (20)      239 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/requires.txt
--rw-r--r--   0 labad      (502) staff       (20)       10 2023-06-27 23:53:05.000000 pdm_utils-1.1.1/src/pdm_utils.egg-info/top_level.txt
-drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-27 23:53:05.875453 pdm_utils-1.1.1/tests/
--rw-r--r--   0 labad      (502) staff       (20)    20144 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/tests/test_data_utils.py
--rw-r--r--   0 labad      (502) staff       (20)    15441 2020-10-23 17:14:54.000000 pdm_utils-1.1.1/tests/test_db_utils.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.339707 pdm_utils-1.1.2/
+-rw-r--r--   0 labad      (502) staff       (20)    35186 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/LICENSE
+-rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-29 20:36:18.339915 pdm_utils-1.1.2/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)      790 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/README.md
+-rw-r--r--   0 labad      (502) staff       (20)       89 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/pyproject.toml
+-rw-r--r--   0 labad      (502) staff       (20)     1507 2023-06-29 20:36:18.341021 pdm_utils-1.1.2/setup.cfg
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.258626 pdm_utils-1.1.2/src/
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.263576 pdm_utils-1.1.2/src/pdm_utils/
+-rw-r--r--   0 labad      (502) staff       (20)      146 2023-06-29 20:31:03.000000 pdm_utils-1.1.2/src/pdm_utils/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)      114 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/__main__.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.285472 pdm_utils-1.1.2/src/pdm_utils/classes/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)    20060 2020-10-30 13:34:57.000000 pdm_utils-1.1.2/src/pdm_utils/classes/alchemyhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     8100 2021-09-17 01:24:47.000000 pdm_utils-1.1.2/src/pdm_utils/classes/aragornhandler.py
+-rw-r--r--   0 labad      (502) staff       (20)    10410 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/bundle.py
+-rw-r--r--   0 labad      (502) staff       (20)    39957 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/cds.py
+-rw-r--r--   0 labad      (502) staff       (20)     2461 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/cdspair.py
+-rw-r--r--   0 labad      (502) staff       (20)     9923 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/dbcomparesummary.py
+-rw-r--r--   0 labad      (502) staff       (20)      165 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/classes/error.py
+-rw-r--r--   0 labad      (502) staff       (20)      696 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/evaluation.py
+-rw-r--r--   0 labad      (502) staff       (20)     7966 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    23716 2021-09-17 01:24:47.000000 pdm_utils-1.1.2/src/pdm_utils/classes/filter.py
+-rw-r--r--   0 labad      (502) staff       (20)    41595 2021-09-22 16:59:23.000000 pdm_utils-1.1.2/src/pdm_utils/classes/genome.py
+-rw-r--r--   0 labad      (502) staff       (20)     5574 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/genomepair.py
+-rw-r--r--   0 labad      (502) staff       (20)    18395 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/genometriad.py
+-rw-r--r--   0 labad      (502) staff       (20)     1124 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/classes/progress.py
+-rw-r--r--   0 labad      (502) staff       (20)     7244 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/randomfieldupdatehandler.py
+-rw-r--r--   0 labad      (502) staff       (20)     4243 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/source.py
+-rw-r--r--   0 labad      (502) staff       (20)     8694 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/ticket.py
+-rw-r--r--   0 labad      (502) staff       (20)    37793 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/tmrna.py
+-rw-r--r--   0 labad      (502) staff       (20)    64069 2021-09-22 15:49:23.000000 pdm_utils-1.1.2/src/pdm_utils/classes/trna.py
+-rw-r--r--   0 labad      (502) staff       (20)     3694 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/classes/trnascansehandler.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.289022 pdm_utils-1.1.2/src/pdm_utils/constants/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/constants/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6185 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/constants/constants.py
+-rw-r--r--   0 labad      (502) staff       (20)    10763 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/constants/db_schema_0.py
+-rw-r--r--   0 labad      (502) staff       (20)    12305 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/constants/eval_descriptions.py
+-rw-r--r--   0 labad      (502) staff       (20)    37168 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/constants/schema_conversions.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.318398 pdm_utils-1.1.2/src/pdm_utils/functions/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)     6113 2020-10-30 13:34:57.000000 pdm_utils-1.1.2/src/pdm_utils/functions/annotation.py
+-rw-r--r--   0 labad      (502) staff       (20)    45918 2021-01-04 16:11:55.000000 pdm_utils-1.1.2/src/pdm_utils/functions/basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     2962 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/cartography.py
+-rw-r--r--   0 labad      (502) staff       (20)     2182 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/configfile.py
+-rw-r--r--   0 labad      (502) staff       (20)     2853 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/functions/deeptmhmm.py
+-rw-r--r--   0 labad      (502) staff       (20)     4638 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/eval_modes.py
+-rw-r--r--   0 labad      (502) staff       (20)     2301 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/fasta.py
+-rw-r--r--   0 labad      (502) staff       (20)    10526 2021-03-23 03:57:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/fileio.py
+-rw-r--r--   0 labad      (502) staff       (20)    30706 2021-09-22 16:59:23.000000 pdm_utils-1.1.2/src/pdm_utils/functions/flat_files.py
+-rw-r--r--   0 labad      (502) staff       (20)     2858 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/multiprocess.py
+-rw-r--r--   0 labad      (502) staff       (20)     5299 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/multithread.py
+-rw-r--r--   0 labad      (502) staff       (20)    27400 2022-10-18 17:47:46.000000 pdm_utils-1.1.2/src/pdm_utils/functions/mysqldb.py
+-rw-r--r--   0 labad      (502) staff       (20)    13414 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/mysqldb_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)     6605 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/ncbi.py
+-rw-r--r--   0 labad      (502) staff       (20)    10972 2020-12-29 20:15:44.000000 pdm_utils-1.1.2/src/pdm_utils/functions/parsing.py
+-rw-r--r--   0 labad      (502) staff       (20)    12611 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/phagesdb.py
+-rw-r--r--   0 labad      (502) staff       (20)     8600 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/pham_alignment.py
+-rw-r--r--   0 labad      (502) staff       (20)     9900 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/phameration.py
+-rw-r--r--   0 labad      (502) staff       (20)     8473 2021-01-04 16:11:55.000000 pdm_utils-1.1.2/src/pdm_utils/functions/pipeline_shells.py
+-rw-r--r--   0 labad      (502) staff       (20)     8828 2020-12-28 19:11:26.000000 pdm_utils-1.1.2/src/pdm_utils/functions/pipelines_basic.py
+-rw-r--r--   0 labad      (502) staff       (20)    30269 2021-09-17 01:24:47.000000 pdm_utils-1.1.2/src/pdm_utils/functions/querying.py
+-rw-r--r--   0 labad      (502) staff       (20)     6325 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/rpsblast.py
+-rw-r--r--   0 labad      (502) staff       (20)     3475 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/server.py
+-rw-r--r--   0 labad      (502) staff       (20)      978 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/functions/subprocess.py
+-rw-r--r--   0 labad      (502) staff       (20)    11826 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/functions/tickets.py
+-rw-r--r--   0 labad      (502) staff       (20)    15996 2021-01-04 16:11:55.000000 pdm_utils-1.1.2/src/pdm_utils/functions/url_basic.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.336879 pdm_utils-1.1.2/src/pdm_utils/pipelines/
+-rw-r--r--   0 labad      (502) staff       (20)        0 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/__init__.py
+-rw-r--r--   0 labad      (502) staff       (20)    27107 2023-06-27 23:12:34.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/cluster_db.py
+-rwxr-xr-x   0 labad      (502) staff       (20)    60772 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/compare_db.py
+-rw-r--r--   0 labad      (502) staff       (20)     8327 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/convert_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    33685 2021-09-22 16:59:23.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/export_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    17337 2023-06-27 23:13:56.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/find_domains.py
+-rw-r--r--   0 labad      (502) staff       (20)      972 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/find_membrane.py
+-rw-r--r--   0 labad      (502) staff       (20)    14635 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/find_transmembrane.py
+-rwxr-xr-x   0 labad      (502) staff       (20)     7930 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/freeze_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    37362 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/get_data.py
+-rw-r--r--   0 labad      (502) staff       (20)    16273 2021-01-05 20:20:36.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/get_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    10665 2020-10-30 13:34:57.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/get_gb_records.py
+-rw-r--r--   0 labad      (502) staff       (20)    91016 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/import_genome.py
+-rw-r--r--   0 labad      (502) staff       (20)    12771 2021-09-17 01:23:58.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/pham_finder.py
+-rw-r--r--   0 labad      (502) staff       (20)    25213 2020-10-30 13:34:57.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/pham_review.py
+-rw-r--r--   0 labad      (502) staff       (20)    10125 2023-06-18 16:32:34.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/phamerate.py
+-rw-r--r--   0 labad      (502) staff       (20)     7937 2020-12-13 18:52:56.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/push_db.py
+-rw-r--r--   0 labad      (502) staff       (20)    36843 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/revise.py
+-rw-r--r--   0 labad      (502) staff       (20)     5642 2023-06-15 19:40:19.000000 pdm_utils-1.1.2/src/pdm_utils/pipelines/update_field.py
+-rw-r--r--   0 labad      (502) staff       (20)     3630 2023-06-27 20:56:00.000000 pdm_utils-1.1.2/src/pdm_utils/run.py
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.266554 pdm_utils-1.1.2/src/pdm_utils.egg-info/
+-rw-r--r--   0 labad      (502) staff       (20)     1720 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/PKG-INFO
+-rw-r--r--   0 labad      (502) staff       (20)     3061 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 labad      (502) staff       (20)        1 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 labad      (502) staff       (20)       54 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/entry_points.txt
+-rw-r--r--   0 labad      (502) staff       (20)      239 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/requires.txt
+-rw-r--r--   0 labad      (502) staff       (20)       10 2023-06-29 20:36:18.000000 pdm_utils-1.1.2/src/pdm_utils.egg-info/top_level.txt
+drwxr-xr-x   0 labad      (502) staff       (20)        0 2023-06-29 20:36:18.338804 pdm_utils-1.1.2/tests/
+-rw-r--r--   0 labad      (502) staff       (20)    20144 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/tests/test_data_utils.py
+-rw-r--r--   0 labad      (502) staff       (20)    15441 2020-10-23 17:14:54.000000 pdm_utils-1.1.2/tests/test_db_utils.py
```

### Comparing `pdm_utils-1.1.1/LICENSE` & `pdm_utils-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/PKG-INFO` & `pdm_utils-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm_utils
-Version: 1.1.1
+Version: 1.1.2
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pdm_utils-1.1.1/README.md` & `pdm_utils-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/setup.cfg` & `pdm_utils-1.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 license_files = LICENSE
 name = pdm_utils
-version = 1.1.1
+version = 1.1.2
 author = Christian Gauthier
 author_email = chg60@pitt.edu
 description = MySQL phage genomics database management utilities
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/SEA-PHAGES/pdm_utils
 project_urls = 
@@ -27,15 +27,15 @@
 python_requires = >=3.7
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	biopython == 1.77
 	kaleido == 0.2.1
-	networkx >= 2.4
+	networkx >= 3.0
 	pandas == 2.0.2
 	paramiko >= 2.7.2
 	parasail == 1.3.4
 	phammseqs >= 1.0.4
 	psutil == 5.9.5
 	pybiolib >= 1.1.918
 	pymysql == 0.9.3
```

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/alchemyhandler.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/alchemyhandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/aragornhandler.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/aragornhandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/bundle.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/bundle.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/cds.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/cds.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/cdspair.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/cdspair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/dbcomparesummary.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/dbcomparesummary.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/evaluation.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/evaluation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/fileio.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/filter.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/filter.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/genome.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/genome.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/genomepair.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/genomepair.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/genometriad.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/genometriad.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/progress.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/progress.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/randomfieldupdatehandler.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/randomfieldupdatehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/source.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/source.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/ticket.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/ticket.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/tmrna.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/tmrna.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/trna.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/trna.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/classes/trnascansehandler.py` & `pdm_utils-1.1.2/src/pdm_utils/classes/trnascansehandler.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/constants/constants.py` & `pdm_utils-1.1.2/src/pdm_utils/constants/constants.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/constants/db_schema_0.py` & `pdm_utils-1.1.2/src/pdm_utils/constants/db_schema_0.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/constants/eval_descriptions.py` & `pdm_utils-1.1.2/src/pdm_utils/constants/eval_descriptions.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/constants/schema_conversions.py` & `pdm_utils-1.1.2/src/pdm_utils/constants/schema_conversions.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/annotation.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/annotation.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/basic.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/cartography.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/cartography.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/configfile.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/configfile.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/deeptmhmm.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/deeptmhmm.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/eval_modes.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/eval_modes.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/fasta.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/fasta.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/fileio.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/fileio.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/flat_files.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/flat_files.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/multiprocess.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/multiprocess.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/multithread.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/multithread.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/mysqldb.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/mysqldb.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/mysqldb_basic.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/mysqldb_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/ncbi.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/ncbi.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/parsing.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/parsing.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/phagesdb.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/phagesdb.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/pham_alignment.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/pham_alignment.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/phameration.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/phameration.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/pipeline_shells.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/pipeline_shells.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/pipelines_basic.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/pipelines_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/querying.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/querying.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/rpsblast.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/rpsblast.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/server.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/server.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/subprocess.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/subprocess.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/tickets.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/tickets.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/functions/url_basic.py` & `pdm_utils-1.1.2/src/pdm_utils/functions/url_basic.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/cluster_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/cluster_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/compare_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/compare_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/convert_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/convert_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/export_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/export_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/find_domains.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/find_domains.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/find_membrane.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/find_membrane.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/find_transmembrane.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/find_transmembrane.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/freeze_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/freeze_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/get_data.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/get_data.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/get_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/get_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/get_gb_records.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/get_gb_records.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/import_genome.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/import_genome.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/pham_finder.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/pham_finder.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/pham_review.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/pham_review.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/phamerate.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/phamerate.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/push_db.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/push_db.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/revise.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/revise.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/pipelines/update_field.py` & `pdm_utils-1.1.2/src/pdm_utils/pipelines/update_field.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils/run.py` & `pdm_utils-1.1.2/src/pdm_utils/run.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/src/pdm_utils.egg-info/PKG-INFO` & `pdm_utils-1.1.2/src/pdm_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-utils
-Version: 1.1.1
+Version: 1.1.2
 Summary: MySQL phage genomics database management utilities
 Home-page: https://github.com/SEA-PHAGES/pdm_utils
 Author: Christian Gauthier
 Author-email: chg60@pitt.edu
 Project-URL: Documentation, https://pdm-utils.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/SEA-PHAGES/pdm_utils/
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pdm_utils-1.1.1/src/pdm_utils.egg-info/SOURCES.txt` & `pdm_utils-1.1.2/src/pdm_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/tests/test_data_utils.py` & `pdm_utils-1.1.2/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `pdm_utils-1.1.1/tests/test_db_utils.py` & `pdm_utils-1.1.2/tests/test_db_utils.py`

 * *Files identical despite different names*

