# Comparing `tmp/nomenklatura-3.0.1.tar.gz` & `tmp/nomenklatura-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.0.1.tar", last modified: Wed Jun 28 10:36:40 2023, max compression
+gzip compressed data, was "nomenklatura-3.0.3.tar", last modified: Thu Jun 29 07:34:13 2023, max compression
```

## Comparing `nomenklatura-3.0.1.tar` & `nomenklatura-3.0.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.773881 nomenklatura-3.0.1/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.773881 nomenklatura-3.0.1/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.777881 nomenklatura-3.0.1/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 10:36:40.773881 nomenklatura-3.0.1/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 10:36:15.000000 nomenklatura-3.0.1/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-28 10:36:40.000000 nomenklatura-3.0.1/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 10:36:40.781881 nomenklatura-3.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-28 10:34:39.000000 nomenklatura-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.386916 nomenklatura-3.0.3/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9974 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15934 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.390916 nomenklatura-3.0.3/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4722 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:34:13.386916 nomenklatura-3.0.3/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:33:48.000000 nomenklatura-3.0.3/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-29 07:34:13.000000 nomenklatura-3.0.3/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:34:13.394916 nomenklatura-3.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-29 07:32:11.000000 nomenklatura-3.0.3/setup.py
```

### Comparing `nomenklatura-3.0.1/LICENSE` & `nomenklatura-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/PKG-INFO` & `nomenklatura-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.0.1
+Version: 3.0.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.0.1/README.md` & `nomenklatura-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/cache.py` & `nomenklatura-3.0.3/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/cli.py` & `nomenklatura-3.0.3/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.0.3/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.0.3/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/catalog.py` & `nomenklatura-3.0.3/nomenklatura/dataset/catalog.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/coverage.py` & `nomenklatura-3.0.3/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/dataset.py` & `nomenklatura-3.0.3/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/publisher.py` & `nomenklatura-3.0.3/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/resource.py` & `nomenklatura-3.0.3/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/dataset/util.py` & `nomenklatura-3.0.3/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/db.py` & `nomenklatura-3.0.3/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/__init__.py` & `nomenklatura-3.0.3/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/aleph.py` & `nomenklatura-3.0.3/nomenklatura/enrich/aleph.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/common.py` & `nomenklatura-3.0.3/nomenklatura/enrich/common.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.0.3/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.0.3/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.0.3/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/enrich/yente.py` & `nomenklatura-3.0.3/nomenklatura/enrich/yente.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/entity.py` & `nomenklatura-3.0.3/nomenklatura/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     @property
     def statements(self) -> Generator[Statement, None, None]:
         if self.id is not None:
             yield Statement(
                 canonical_id=self.id,
                 entity_id=self.id,
                 prop=BASE_ID,
-                prop_type=BASE_ID,
                 schema=self.schema.name,
                 value=self.checksum(),
                 dataset=self.default_dataset,
             )
         yield from self._iter_stmt()
 
     @property
@@ -226,15 +225,14 @@
         ):
             if original_value is None and clean != value:
                 original_value = value
 
             stmt = Statement(
                 entity_id=self.id,
                 prop=prop.name,
-                prop_type=prop.type.name,
                 schema=schema or self.schema.name,
                 value=clean,
                 dataset=dataset or self.default_dataset,
                 lang=lang,
                 original_value=original_value,
                 first_seen=seen,
             )
```

### Comparing `nomenklatura-3.0.1/nomenklatura/index/entry.py` & `nomenklatura-3.0.3/nomenklatura/index/entry.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/index/index.py` & `nomenklatura-3.0.3/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/index/tokenizer.py` & `nomenklatura-3.0.3/nomenklatura/index/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/judgement.py` & `nomenklatura-3.0.3/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/__init__.py` & `nomenklatura-3.0.3/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.0.3/nomenklatura/matching/heuristic/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.0.3/nomenklatura/matching/heuristic/logic.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/pairs.py` & `nomenklatura-3.0.3/nomenklatura/matching/pairs.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/types.py` & `nomenklatura-3.0.3/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/util.py` & `nomenklatura-3.0.3/nomenklatura/matching/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/model.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/names.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/train.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v1/util.py` & `nomenklatura-3.0.3/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/model.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/names.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/train.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/matching/v2/util.py` & `nomenklatura-3.0.3/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/publish/dates.py` & `nomenklatura-3.0.3/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/publish/edges.py` & `nomenklatura-3.0.3/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/publish/names.py` & `nomenklatura-3.0.3/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/resolver/edge.py` & `nomenklatura-3.0.3/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/resolver/identifier.py` & `nomenklatura-3.0.3/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/resolver/resolver.py` & `nomenklatura-3.0.3/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/senzing.py` & `nomenklatura-3.0.3/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/statement/serialize.py` & `nomenklatura-3.0.3/nomenklatura/statement/serialize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import csv
+import _csv
 import click
 import orjson
 from pathlib import Path
 from io import TextIOWrapper
-from typing import BinaryIO, Generator, Iterable, Type, Dict, Any
+from typing import BinaryIO, TextIO, Generator, Iterable, Type, Dict, Any, List
 from followthemoney.cli.util import MAX_LINE
 
 from nomenklatura.statement.statement import S
-from nomenklatura.util import pack_prop, unpack_prop, bool_text
+from nomenklatura.util import pack_prop, unpack_prop
 
 JSON = "json"
 CSV = "csv"
 PACK = "pack"
 FORMATS = [JSON, CSV, PACK]
 
 CSV_COLUMNS = [
@@ -60,26 +61,30 @@
     fh: BinaryIO, statement_type: Type[S]
 ) -> Generator[S, None, None]:
     wrapped = TextIOWrapper(fh, encoding="utf-8")
     for row in csv.DictReader(wrapped, dialect=csv.unix_dialect):
         yield statement_type.from_row(row)
 
 
+def unpack_row(row: List[str], statement_type: Type[S]) -> S:
+    data = dict(zip(PACK_COLUMNS, row))
+    data["canonical_id"] = data["entity_id"]
+    schema, prop_type, prop = unpack_prop(data["prop"])
+    data["schema"] = schema
+    data["prop"] = prop
+    data["prop_type"] = prop_type
+    return statement_type.from_row(data)
+
+
 def read_pack_statements(
     fh: BinaryIO, statement_type: Type[S]
 ) -> Generator[S, None, None]:
     wrapped = TextIOWrapper(fh, encoding="utf-8")
     for row in csv.reader(wrapped, dialect=csv.unix_dialect):
-        data = dict(zip(PACK_COLUMNS, row))
-        data["canonical_id"] = data["entity_id"]
-        schema, prop_type, prop = unpack_prop(data["prop"])
-        data["schema"] = schema
-        data["prop"] = prop
-        data["prop_type"] = prop_type
-        yield statement_type.from_row(data)
+        yield unpack_row(row, statement_type)
 
 
 def read_statements(
     fh: BinaryIO, format: str, statement_type: Type[S]
 ) -> Generator[S, None, None]:
     if format == CSV:
         yield from read_csv_statements(fh, statement_type)
@@ -128,24 +133,37 @@
     schema = row.pop("schema")
     if prop is None or schema is None:
         raise ValueError("Cannot pack statement without prop and schema")
     row["prop"] = pack_prop(schema, prop)
     return row
 
 
+def pack_row(stmt: S) -> List[Any]:
+    row = stmt.to_row()
+    prop = row.pop("prop")
+    schema = row.pop("schema")
+    if prop is None or schema is None:
+        raise ValueError("Cannot pack statement without prop and schema")
+    row["prop"] = pack_prop(schema, prop)
+    return [row.get(c) for c in PACK_COLUMNS]
+
+
+def pack_writer(fh: TextIO) -> "_csv._writer":
+    return csv.writer(
+        fh,
+        dialect=csv.unix_dialect,
+        quoting=csv.QUOTE_MINIMAL,
+    )
+
+
 def write_pack_statements(fh: BinaryIO, statements: Iterable[S]) -> None:
     with TextIOWrapper(fh, encoding="utf-8") as wrapped:
-        writer = csv.writer(
-            wrapped,
-            dialect=csv.unix_dialect,
-            quoting=csv.QUOTE_MINIMAL,
-        )
+        writer = pack_writer(wrapped)
         for stmt in statements:
-            row = pack_statement(stmt)
-            writer.writerow([row.get(c) for c in PACK_COLUMNS])
+            writer.writerow(pack_row(stmt))
 
 
 def write_statements(fh: BinaryIO, format: str, statements: Iterable[S]) -> None:
     if format == CSV:
         write_csv_statements(fh, statements)
     elif format == PACK:
         write_pack_statements(fh, statements)
```

### Comparing `nomenklatura-3.0.1/nomenklatura/statement/statement.py` & `nomenklatura-3.0.3/nomenklatura/statement/statement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import hashlib
 from sqlalchemy.engine import Row
 from typing import cast, TYPE_CHECKING
 from typing import Any, Dict, Generator, Optional, Type, TypeVar, TypedDict
 
-from nomenklatura.util import bool_text, datetime_iso, text_bool, BASE_ID
+from nomenklatura.util import bool_text, datetime_iso, text_bool
+from nomenklatura.util import get_prop_type, BASE_ID
 
 if TYPE_CHECKING:
     from nomenklatura.entity import CE
 
 S = TypeVar("S", bound="Statement")
 
 
@@ -58,15 +59,14 @@
         "last_seen",
     ]
 
     def __init__(
         self,
         entity_id: Optional[str],
         prop: str,
-        prop_type: str,
         schema: str,
         value: str,
         dataset: str,
         lang: Optional[str] = None,
         original_value: Optional[str] = None,
         first_seen: Optional[str] = None,
         target: Optional[bool] = False,
@@ -74,15 +74,15 @@
         id: Optional[str] = None,
         canonical_id: Optional[str] = None,
         last_seen: Optional[str] = None,
     ):
         self.entity_id = entity_id
         self.canonical_id = canonical_id or entity_id
         self.prop = prop
-        self.prop_type = prop_type
+        self.prop_type = get_prop_type(schema, prop)
         self.schema = schema
         self.value = value
         self.dataset = dataset
         self.lang = lang
         self.original_value = original_value
         self.first_seen = first_seen
         self.last_seen = last_seen or first_seen
@@ -170,15 +170,14 @@
         return hashlib.sha1(key.encode("utf-8")).hexdigest()
 
     @classmethod
     def from_dict(cls: Type[S], data: StatementDict) -> S:
         return cls(
             entity_id=data["entity_id"],
             prop=data["prop"],
-            prop_type=data["prop_type"],
             schema=data["schema"],
             value=data["value"],
             dataset=data["dataset"],
             lang=data.get("lang", None),
             original_value=data.get("original_value", None),
             first_seen=data.get("first_seen", None),
             target=data.get("target"),
@@ -198,15 +197,14 @@
     @classmethod
     def from_db_row(cls: Type[S], row: Row) -> S:
         return cls(
             id=row.id,
             canonical_id=row.canonical_id,
             entity_id=row.entity_id,
             prop=row.prop,
-            prop_type=row.prop_type,
             schema=row.schema,
             value=row.value,
             dataset=row.dataset,
             lang=row.lang,
             original_value=row.original_value,
             first_seen=datetime_iso(row.first_seen),
             target=row.target,
@@ -224,28 +222,26 @@
         target: Optional[bool] = None,
         external: Optional[bool] = None,
     ) -> Generator[S, None, None]:
         if entity.id is not None:
             yield cls(
                 entity_id=entity.id,
                 prop=BASE_ID,
-                prop_type=BASE_ID,
                 schema=entity.schema.name,
                 value=entity.id,
                 dataset=dataset,
                 target=target,
                 external=external,
                 first_seen=first_seen,
                 last_seen=last_seen,
             )
         for prop, value in entity.itervalues():
             yield cls(
                 entity_id=entity.id,
                 prop=prop.name,
-                prop_type=prop.type.name,
                 schema=entity.schema.name,
                 value=value,
                 dataset=dataset,
                 target=target,
                 external=external,
                 first_seen=first_seen,
                 last_seen=last_seen,
```

### Comparing `nomenklatura-3.0.1/nomenklatura/store/__init__.py` & `nomenklatura-3.0.3/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/store/base.py` & `nomenklatura-3.0.3/nomenklatura/store/base.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/store/level.py` & `nomenklatura-3.0.3/nomenklatura/store/level.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/store/memory.py` & `nomenklatura-3.0.3/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/store/util.py` & `nomenklatura-3.0.3/nomenklatura/store/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,20 +29,19 @@
         value,
         lang,
         original_value,
         first_seen,
         last_seen,
         target,
     ) = orjson.loads(data)
-    schema, prop_type, prop = unpack_prop(prop_id)
+    schema, _, prop = unpack_prop(prop_id)
     return Statement(
         id=id,
         entity_id=entity_id,
         prop=prop,
-        prop_type=prop_type,
         schema=schema,
         value=value,
         lang=lang,
         dataset=dataset,
         original_value=original_value,
         first_seen=first_seen,
         last_seen=last_seen,
```

### Comparing `nomenklatura-3.0.1/nomenklatura/tui/app.py` & `nomenklatura-3.0.3/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/tui/comparison.py` & `nomenklatura-3.0.3/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/tui/util.py` & `nomenklatura-3.0.3/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura/util.py` & `nomenklatura-3.0.3/nomenklatura/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,18 +103,24 @@
 
 
 def pack_prop(schema: str, prop: str) -> str:
     return f"{schema}:{prop}"
 
 
 @cache
-def unpack_prop(id: str) -> Tuple[str, str, str]:
-    schema, prop = id.split(":", 1)
+def get_prop_type(schema: str, prop: str) -> str:
     if prop == BASE_ID:
-        return schema, BASE_ID, BASE_ID
+        return BASE_ID
     schema_obj = model.get(schema)
     if schema_obj is None:
         raise TypeError("Schema not found: %s" % schema)
     prop_obj = schema_obj.get(prop)
     if prop_obj is None:
         raise TypeError("Property not found: %s" % prop)
-    return schema, prop_obj.type.name, prop
+    return prop_obj.type.name
+
+
+@cache
+def unpack_prop(id: str) -> Tuple[str, str, str]:
+    schema, prop = id.split(":", 1)
+    prop_type = get_prop_type(schema, prop)
+    return schema, prop_type, prop
```

### Comparing `nomenklatura-3.0.1/nomenklatura/xref.py` & `nomenklatura-3.0.3/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.0.3/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.0.1
+Version: 3.0.3
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.0.1/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.0.3/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.0.1/setup.py` & `nomenklatura-3.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.0.1",
+    version="3.0.3",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
```

